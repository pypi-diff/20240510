# Comparing `tmp/audbackend-1.0.1.tar.gz` & `tmp/audbackend-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audbackend-1.0.1.tar", last modified: Wed Oct 18 08:10:29 2023, max compression
+gzip compressed data, was "audbackend-1.0.2.tar", last modified: Tue Feb 13 10:35:37 2024, max compression
```

## Comparing `audbackend-1.0.1.tar` & `audbackend-1.0.2.tar`

### file list

```diff
@@ -1,67 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 08:10:29.919777 audbackend-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2023-10-18 08:10:11.000000 audbackend-1.0.1/.coveragerc.Linux
--rw-r--r--   0 runner    (1001) docker     (127)       75 2023-10-18 08:10:11.000000 audbackend-1.0.1/.coveragerc.Windows
--rw-r--r--   0 runner    (1001) docker     (127)       73 2023-10-18 08:10:11.000000 audbackend-1.0.1/.coveragerc.macOS
--rw-r--r--   0 runner    (1001) docker     (127)      196 2023-10-18 08:10:11.000000 audbackend-1.0.1/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 08:10:29.879777 audbackend-1.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 08:10:29.895777 audbackend-1.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      862 2023-10-18 08:10:11.000000 audbackend-1.0.1/.github/workflows/doc.yml
--rw-r--r--   0 runner    (1001) docker     (127)      513 2023-10-18 08:10:11.000000 audbackend-1.0.1/.github/workflows/linter.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2020 2023-10-18 08:10:11.000000 audbackend-1.0.1/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2023-10-18 08:10:11.000000 audbackend-1.0.1/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      104 2023-10-18 08:10:11.000000 audbackend-1.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      573 2023-10-18 08:10:11.000000 audbackend-1.0.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6184 2023-10-18 08:10:11.000000 audbackend-1.0.1/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3583 2023-10-18 08:10:11.000000 audbackend-1.0.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2023-10-18 08:10:11.000000 audbackend-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3922 2023-10-18 08:10:29.919777 audbackend-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1355 2023-10-18 08:10:11.000000 audbackend-1.0.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 08:10:29.895777 audbackend-1.0.1/audbackend/
--rw-r--r--   0 runner    (1001) docker     (127)      797 2023-10-18 08:10:11.000000 audbackend-1.0.1/audbackend/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 08:10:29.903777 audbackend-1.0.1/audbackend/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-18 08:10:11.000000 audbackend-1.0.1/audbackend/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6064 2023-10-18 08:10:11.000000 audbackend-1.0.1/audbackend/core/api.py
--rw-r--r--   0 runner    (1001) docker     (127)    13235 2023-10-18 08:10:11.000000 audbackend-1.0.1/audbackend/core/artifactory.py
--rw-r--r--   0 runner    (1001) docker     (127)    25462 2023-10-18 08:10:11.000000 audbackend-1.0.1/audbackend/core/backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     1501 2023-10-18 08:10:11.000000 audbackend-1.0.1/audbackend/core/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      680 2023-10-18 08:10:11.000000 audbackend-1.0.1/audbackend/core/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     8815 2023-10-18 08:10:11.000000 audbackend-1.0.1/audbackend/core/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (127)      912 2023-10-18 08:10:11.000000 audbackend-1.0.1/audbackend/core/repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     3189 2023-10-18 08:10:11.000000 audbackend-1.0.1/audbackend/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 08:10:29.899777 audbackend-1.0.1/audbackend.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3922 2023-10-18 08:10:29.000000 audbackend-1.0.1/audbackend.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1251 2023-10-18 08:10:29.000000 audbackend-1.0.1/audbackend.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-18 08:10:29.000000 audbackend-1.0.1/audbackend.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      121 2023-10-18 08:10:29.000000 audbackend-1.0.1/audbackend.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2023-10-18 08:10:29.000000 audbackend-1.0.1/audbackend.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 08:10:29.911777 audbackend-1.0.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 08:10:29.883777 audbackend-1.0.1/docs/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 08:10:29.911777 audbackend-1.0.1/docs/_templates/autosummary/
--rw-r--r--   0 runner    (1001) docker     (127)      103 2023-10-18 08:10:11.000000 audbackend-1.0.1/docs/_templates/autosummary/base.rst
--rw-r--r--   0 runner    (1001) docker     (127)      547 2023-10-18 08:10:11.000000 audbackend-1.0.1/docs/_templates/autosummary/class.rst
--rw-r--r--   0 runner    (1001) docker     (127)      112 2023-10-18 08:10:11.000000 audbackend-1.0.1/docs/_templates/autosummary/function.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 08:10:29.911777 audbackend-1.0.1/docs/api-src/
--rw-r--r--   0 runner    (1001) docker     (127)      653 2023-10-18 08:10:11.000000 audbackend-1.0.1/docs/api-src/audbackend.rst
--rw-r--r--   0 runner    (1001) docker     (127)       30 2023-10-18 08:10:11.000000 audbackend-1.0.1/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2318 2023-10-18 08:10:11.000000 audbackend-1.0.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2023-10-18 08:10:11.000000 audbackend-1.0.1/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)       12 2023-10-18 08:10:11.000000 audbackend-1.0.1/docs/genindex.rst
--rw-r--r--   0 runner    (1001) docker     (127)      505 2023-10-18 08:10:11.000000 audbackend-1.0.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      584 2023-10-18 08:10:11.000000 audbackend-1.0.1/docs/install.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1666 2023-10-18 08:10:11.000000 audbackend-1.0.1/docs/legacy.rst
--rw-r--r--   0 runner    (1001) docker     (127)      111 2023-10-18 08:10:11.000000 audbackend-1.0.1/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)    16091 2023-10-18 08:10:11.000000 audbackend-1.0.1/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4838 2023-10-18 08:10:11.000000 audbackend-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       10 2023-10-18 08:10:11.000000 audbackend-1.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-18 08:10:29.919777 audbackend-1.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 08:10:29.915778 audbackend-1.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2442 2023-10-18 08:10:11.000000 audbackend-1.0.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 08:10:29.919777 audbackend-1.0.1/tests/misc/
--rw-r--r--   0 runner    (1001) docker     (127)      971 2023-10-18 08:10:11.000000 audbackend-1.0.1/tests/misc/cleanup_artifactory.py
--rw-r--r--   0 runner    (1001) docker     (127)       37 2023-10-18 08:10:11.000000 audbackend-1.0.1/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4850 2023-10-18 08:10:11.000000 audbackend-1.0.1/tests/singlefolder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2203 2023-10-18 08:10:11.000000 audbackend-1.0.1/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     5755 2023-10-18 08:10:11.000000 audbackend-1.0.1/tests/test_artifactory.py
--rw-r--r--   0 runner    (1001) docker     (127)    23709 2023-10-18 08:10:11.000000 audbackend-1.0.1/tests/test_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     4084 2023-10-18 08:10:11.000000 audbackend-1.0.1/tests/test_filesystem.py
--rw-r--r--   0 runner    (1001) docker     (127)      144 2023-10-18 08:10:11.000000 audbackend-1.0.1/tests/test_filesystem_only.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 10:35:37.252229 audbackend-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-02-13 10:35:30.000000 audbackend-1.0.2/.coveragerc.Linux
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-02-13 10:35:30.000000 audbackend-1.0.2/.coveragerc.Windows
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-02-13 10:35:30.000000 audbackend-1.0.2/.coveragerc.macOS
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-02-13 10:35:30.000000 audbackend-1.0.2/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 10:35:37.240229 audbackend-1.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 10:35:37.244229 audbackend-1.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-02-13 10:35:30.000000 audbackend-1.0.2/.github/workflows/doc.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-02-13 10:35:30.000000 audbackend-1.0.2/.github/workflows/linter.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-02-13 10:35:30.000000 audbackend-1.0.2/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-02-13 10:35:30.000000 audbackend-1.0.2/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-02-13 10:35:30.000000 audbackend-1.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-02-13 10:35:30.000000 audbackend-1.0.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6496 2024-02-13 10:35:30.000000 audbackend-1.0.2/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3583 2024-02-13 10:35:30.000000 audbackend-1.0.2/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-02-13 10:35:30.000000 audbackend-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3922 2024-02-13 10:35:37.252229 audbackend-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-02-13 10:35:30.000000 audbackend-1.0.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 10:35:37.244229 audbackend-1.0.2/audbackend/
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-02-13 10:35:30.000000 audbackend-1.0.2/audbackend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 10:35:37.248229 audbackend-1.0.2/audbackend/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 10:35:30.000000 audbackend-1.0.2/audbackend/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6064 2024-02-13 10:35:30.000000 audbackend-1.0.2/audbackend/core/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13229 2024-02-13 10:35:30.000000 audbackend-1.0.2/audbackend/core/artifactory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25608 2024-02-13 10:35:30.000000 audbackend-1.0.2/audbackend/core/backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-02-13 10:35:30.000000 audbackend-1.0.2/audbackend/core/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-02-13 10:35:30.000000 audbackend-1.0.2/audbackend/core/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8815 2024-02-13 10:35:30.000000 audbackend-1.0.2/audbackend/core/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-02-13 10:35:30.000000 audbackend-1.0.2/audbackend/core/repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3189 2024-02-13 10:35:30.000000 audbackend-1.0.2/audbackend/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 10:35:37.252229 audbackend-1.0.2/audbackend.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3922 2024-02-13 10:35:37.000000 audbackend-1.0.2/audbackend.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-02-13 10:35:37.000000 audbackend-1.0.2/audbackend.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-13 10:35:37.000000 audbackend-1.0.2/audbackend.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-02-13 10:35:37.000000 audbackend-1.0.2/audbackend.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-02-13 10:35:37.000000 audbackend-1.0.2/audbackend.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 10:35:37.248229 audbackend-1.0.2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 10:35:37.248229 audbackend-1.0.2/docs/api-src/
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-02-13 10:35:30.000000 audbackend-1.0.2/docs/api-src/audbackend.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-02-13 10:35:30.000000 audbackend-1.0.2/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-02-13 10:35:30.000000 audbackend-1.0.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-02-13 10:35:30.000000 audbackend-1.0.2/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-02-13 10:35:30.000000 audbackend-1.0.2/docs/genindex.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-02-13 10:35:30.000000 audbackend-1.0.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-02-13 10:35:30.000000 audbackend-1.0.2/docs/install.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1666 2024-02-13 10:35:30.000000 audbackend-1.0.2/docs/legacy.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-02-13 10:35:30.000000 audbackend-1.0.2/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    16091 2024-02-13 10:35:30.000000 audbackend-1.0.2/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4838 2024-02-13 10:35:30.000000 audbackend-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-13 10:35:30.000000 audbackend-1.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-13 10:35:37.252229 audbackend-1.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 10:35:37.252229 audbackend-1.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-02-13 10:35:30.000000 audbackend-1.0.2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 10:35:37.252229 audbackend-1.0.2/tests/misc/
+-rw-r--r--   0 runner    (1001) docker     (127)      971 2024-02-13 10:35:30.000000 audbackend-1.0.2/tests/misc/cleanup_artifactory.py
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-02-13 10:35:30.000000 audbackend-1.0.2/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4850 2024-02-13 10:35:30.000000 audbackend-1.0.2/tests/singlefolder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-02-13 10:35:30.000000 audbackend-1.0.2/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5777 2024-02-13 10:35:30.000000 audbackend-1.0.2/tests/test_artifactory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23797 2024-02-13 10:35:30.000000 audbackend-1.0.2/tests/test_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4084 2024-02-13 10:35:30.000000 audbackend-1.0.2/tests/test_filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-02-13 10:35:30.000000 audbackend-1.0.2/tests/test_filesystem_only.py
```

### Comparing `audbackend-1.0.1/.github/workflows/doc.yml` & `audbackend-1.0.2/.github/workflows/doc.yml`

 * *Files identical despite different names*

### Comparing `audbackend-1.0.1/.github/workflows/linter.yml` & `audbackend-1.0.2/.github/workflows/linter.yml`

 * *Files identical despite different names*

### Comparing `audbackend-1.0.1/.github/workflows/publish.yml` & `audbackend-1.0.2/.github/workflows/publish.yml`

 * *Files 20% similar despite different names*

```diff
@@ -5,38 +5,42 @@
     tags:
       - 'v*' # Push events to matching v*, i.e. v1.0, v20.15.10
 
 jobs:
   deploy:
 
     runs-on: ubuntu-latest
+    environment: release
+    permissions:
+      contents: write
+      id-token: write
+    concurrency:
+      group: ${{ github.workflow }}-${{ github.ref }}
 
     steps:
     - uses: actions/checkout@v3
       with:
         fetch-depth: 2
 
     - name: Set up Python
       uses: actions/setup-python@v4
       with:
         python-version: '3.8'
 
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
-        pip install build twine virtualenv
+        pip install build virtualenv
 
     # PyPI package
-    - name: Build and publish
-      env:
-        TWINE_USERNAME: ${{ secrets.PYPI_USERNAME }}
-        TWINE_PASSWORD: ${{ secrets.PYPI_PASSWORD }}
-      run: |
-        python -m build
-        python -m twine upload dist/*
+    - name: Build Python package
+      run: python -m build
+
+    - name: Publish Python package to PyPI
+      uses: pypa/gh-action-pypi-publish@release/v1
 
     # Documentation
     - name: Install doc dependencies
       run: |
         pip install -r requirements.txt
         pip install -r docs/requirements.txt
 
@@ -52,21 +56,22 @@
 
     # Github release
     - name: Read CHANGELOG
       id: changelog
       run: |
         # Get bullet points from last CHANGELOG entry
         CHANGELOG=$(git diff -U0 HEAD^ HEAD | grep '^[+][\* ]' | sed 's/\+//')
-        # Support for multiline, see
-        # https://github.com/actions/create-release/pull/11#issuecomment-640071918
-        CHANGELOG="${CHANGELOG//'%'/'%25'}"
-        CHANGELOG="${CHANGELOG//$'\n'/'%0A'}"
-        CHANGELOG="${CHANGELOG//$'\r'/'%0D'}"
         echo "Got changelog: $CHANGELOG"
-        echo "body=$CHANGELOG" >> $GITHUB_OUTPUT
+        # Support for multiline, see
+        # https://docs.github.com/en/actions/using-workflows/workflow-commands-for-github-actions#multiline-strings
+        {
+          echo 'body<<EOF'
+          echo "$CHANGELOG"
+          echo EOF
+        } >> "$GITHUB_OUTPUT"
 
     - name: Create release on Github
       id: create_release
       uses: softprops/action-gh-release@v1
       env:
         GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
       with:
```

### Comparing `audbackend-1.0.1/.github/workflows/test.yml` & `audbackend-1.0.2/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `audbackend-1.0.1/.pre-commit-config.yaml` & `audbackend-1.0.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `audbackend-1.0.1/CHANGELOG.rst` & `audbackend-1.0.2/CHANGELOG.rst`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,28 @@
 
 All notable changes to this project will be documented in this file.
 
 The format is based on `Keep a Changelog`_,
 and this project adheres to `Semantic Versioning`_.
 
 
+Version 1.0.2 (2024-02-13)
+--------------------------
+
+* Added: support for accessing
+  remote and virtual repositories
+  on Artifactory
+* Fixed: match the ``pattern`` argument
+  of ``audbackend.Backend.ls()``
+  to file basenames
+* Fixed: typo in raises section
+  of the docstring
+  of ``audbackend.exists()``
+
+
 Version 1.0.1 (2023-10-18)
 --------------------------
 
 * Added: ``regex`` argument
   to ``audbackend.Backend._use_legacy_file_structure()``
   to support providing regex pattern
   in the ``extensions`` argument
```

### Comparing `audbackend-1.0.1/CONTRIBUTING.rst` & `audbackend-1.0.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `audbackend-1.0.1/LICENSE` & `audbackend-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `audbackend-1.0.1/PKG-INFO` & `audbackend-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audbackend
-Version: 1.0.1
+Version: 1.0.2
 Summary: Backends to access Artifactory and local file system
 Author-email: Johannes Wagner <jwagner@audeering.com>, Hagen Wierstorf <hwierstorf@audeering.com>
 License: MIT License
         
         Copyright (c) 2021 audEERING GmbH and Contributors
         
         Authors:
```

### Comparing `audbackend-1.0.1/README.rst` & `audbackend-1.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `audbackend-1.0.1/audbackend/__init__.py` & `audbackend-1.0.2/audbackend/__init__.py`

 * *Files identical despite different names*

### Comparing `audbackend-1.0.1/audbackend/core/api.py` & `audbackend-1.0.2/audbackend/core/api.py`

 * *Files identical despite different names*

### Comparing `audbackend-1.0.1/audbackend/core/artifactory.py` & `audbackend-1.0.2/audbackend/core/artifactory.py`

 * *Files 0% similar despite different names*

```diff
@@ -148,15 +148,15 @@
 
         self._username, self._api_key = _authentication(host)
         path = _artifactory_path(
             self.host,
             self._username,
             self._api_key,
         )
-        self._repo = path.find_repository_local(self.repository)
+        self._repo = path.find_repository(self.repository)
 
         # to support legacy file structure
         # see _use_legacy_file_structure()
         self._legacy_extensions = []
         self._legacy_file_structure = False
         self._legacy_file_structure_regex = False
```

### Comparing `audbackend-1.0.1/audbackend/core/backend.py` & `audbackend-1.0.2/audbackend/core/backend.py`

 * *Files 1% similar despite different names*

```diff
@@ -180,15 +180,15 @@
 
         Returns:
             ``True`` if file exists
 
         Raises:
             BackendError: if ``suppress_backend_errors`` is ``False``
                 and an error is raised on the backend,
-                e.g. ``path`` does not exist
+                e.g. due to a connection timeout
             ValueError: if ``path`` does not start with ``'/'`` or
                 does not match ``'[A-Za-z0-9/._-]+'``
             ValueError: if ``version`` is empty or
                 does not match ``'[A-Za-z0-9._-]+'``
 
         Examples:
             >>> backend.exists('/f.ext', '1.0.0')
@@ -504,14 +504,16 @@
             [('/a.zip', '1.0.0'), ('/a/b.ext', '1.0.0'), ('/f.ext', '1.0.0'), ('/f.ext', '2.0.0')]
             >>> backend.ls(latest_version=True)
             [('/a.zip', '1.0.0'), ('/a/b.ext', '1.0.0'), ('/f.ext', '2.0.0')]
             >>> backend.ls('/f.ext')
             [('/f.ext', '1.0.0'), ('/f.ext', '2.0.0')]
             >>> backend.ls(pattern='*.ext')
             [('/a/b.ext', '1.0.0'), ('/f.ext', '1.0.0'), ('/f.ext', '2.0.0')]
+            >>> backend.ls(pattern='b.*')
+            [('/a/b.ext', '1.0.0')]
             >>> backend.ls('/a/')
             [('/a/b.ext', '1.0.0')]
 
         """  # noqa: E501
         path = utils.check_path(path)
         paths = utils.call_function_on_backend(
             self._ls,
@@ -521,15 +523,18 @@
         )
         if not paths:
             return paths
 
         paths = sorted(paths)
 
         if pattern:
-            paths = [(p, v) for p, v in paths if fnmatch.fnmatch(p, pattern)]
+            paths = [
+                (p, v) for p, v in paths
+                if fnmatch.fnmatch(os.path.basename(p), pattern)
+            ]
 
         if latest_version:
             # d[path] = ['1.0.0', '2.0.0']
             d = {}
             for p, v in paths:
                 if p not in d:
                     d[p] = []
```

### Comparing `audbackend-1.0.1/audbackend/core/conftest.py` & `audbackend-1.0.2/audbackend/core/conftest.py`

 * *Files identical despite different names*

### Comparing `audbackend-1.0.1/audbackend/core/errors.py` & `audbackend-1.0.2/audbackend/core/errors.py`

 * *Files identical despite different names*

### Comparing `audbackend-1.0.1/audbackend/core/filesystem.py` & `audbackend-1.0.2/audbackend/core/filesystem.py`

 * *Files identical despite different names*

### Comparing `audbackend-1.0.1/audbackend/core/repository.py` & `audbackend-1.0.2/audbackend/core/repository.py`

 * *Files identical despite different names*

### Comparing `audbackend-1.0.1/audbackend/core/utils.py` & `audbackend-1.0.2/audbackend/core/utils.py`

 * *Files identical despite different names*

### Comparing `audbackend-1.0.1/audbackend.egg-info/PKG-INFO` & `audbackend-1.0.2/audbackend.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audbackend
-Version: 1.0.1
+Version: 1.0.2
 Summary: Backends to access Artifactory and local file system
 Author-email: Johannes Wagner <jwagner@audeering.com>, Hagen Wierstorf <hwierstorf@audeering.com>
 License: MIT License
         
         Copyright (c) 2021 audEERING GmbH and Contributors
         
         Authors:
```

### Comparing `audbackend-1.0.1/audbackend.egg-info/SOURCES.txt` & `audbackend-1.0.2/audbackend.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -34,17 +34,14 @@
 docs/contributing.rst
 docs/genindex.rst
 docs/index.rst
 docs/install.rst
 docs/legacy.rst
 docs/requirements.txt
 docs/usage.rst
-docs/_templates/autosummary/base.rst
-docs/_templates/autosummary/class.rst
-docs/_templates/autosummary/function.rst
 docs/api-src/audbackend.rst
 tests/conftest.py
 tests/requirements.txt
 tests/singlefolder.py
 tests/test_api.py
 tests/test_artifactory.py
 tests/test_backend.py
```

### Comparing `audbackend-1.0.1/docs/api-src/audbackend.rst` & `audbackend-1.0.2/docs/api-src/audbackend.rst`

 * *Files identical despite different names*

### Comparing `audbackend-1.0.1/docs/conf.py` & `audbackend-1.0.2/docs/conf.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 from datetime import date
-import os
-import shutil
 
 import toml
 
 import audeer
 
 import audbackend
 
@@ -26,25 +24,23 @@
 exclude_patterns = [
     'api-src',
     'build',
     'tests',
     'Thumbs.db',
     '.DS_Store',
 ]
-templates_path = ['_templates']
 pygments_style = None
 extensions = [
     'jupyter_sphinx',
-    'sphinx.ext.autodoc',
     'sphinx.ext.napoleon',
-    'sphinx.ext.autosummary',
     'sphinx.ext.intersphinx',
     'sphinx.ext.viewcode',
     'sphinx_autodoc_typehints',
     'sphinx_copybutton',
+    'sphinx_apipages',
 ]
 
 napoleon_use_ivar = True  # List of class attributes
 autodoc_inherit_docstrings = False  # disable docstring inheritance
 intersphinx_mapping = {
     'audeer': ('https://audeering.github.io/audeer/', None),
     'pandas': ('https://pandas.pydata.org/pandas-docs/stable/', None),
@@ -55,35 +51,19 @@
 ]
 # Ignore package dependencies during building the docs
 # This fixes URL link issues with pandas and sphinx_autodoc_typehints
 autodoc_mock_imports = [
     'pandas',
 ]
 
-# Disable auto-generation of TOC entries in the API
-# https://github.com/sphinx-doc/sphinx/issues/6316
-toc_object_entries = False
-
 
 # HTML --------------------------------------------------------------------
 html_theme = 'sphinx_audeering_theme'
 html_theme_options = {
     'display_version': True,
     'logo_only': False,
     'footer_links': False,
 }
 html_context = {
     'display_github': True,
 }
 html_title = title
-
-
-# Copy API (sub-)module RST files to docs/api/ folder ---------------------
-audeer.rmdir('api')
-audeer.mkdir('api')
-api_src_files = audeer.list_file_names('api-src')
-api_dst_files = [
-    audeer.path('api', os.path.basename(src_file))
-    for src_file in api_src_files
-]
-for src_file, dst_file in zip(api_src_files, api_dst_files):
-    shutil.copyfile(src_file, dst_file)
```

### Comparing `audbackend-1.0.1/docs/install.rst` & `audbackend-1.0.2/docs/install.rst`

 * *Files identical despite different names*

### Comparing `audbackend-1.0.1/docs/legacy.rst` & `audbackend-1.0.2/docs/legacy.rst`

 * *Files identical despite different names*

### Comparing `audbackend-1.0.1/docs/usage.rst` & `audbackend-1.0.2/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `audbackend-1.0.1/pyproject.toml` & `audbackend-1.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `audbackend-1.0.1/tests/conftest.py` & `audbackend-1.0.2/tests/conftest.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,15 +40,17 @@
 
 
 @pytest.fixture(scope='function', autouse=False)
 def owner(request):
     r"""Return expected owner value."""
     name = request.param
     if name == 'artifactory':
-        owner = 'audeering-unittest'
+        owner = audbackend.core.artifactory._authentication(
+            'audeering.jfrog.io/artifactory'
+        )[0]
     else:
         if os.name == 'nt':
             owner = 'Administrators'
         else:
             owner = getpass.getuser()
 
     yield owner
```

### Comparing `audbackend-1.0.1/tests/misc/cleanup_artifactory.py` & `audbackend-1.0.2/tests/misc/cleanup_artifactory.py`

 * *Files identical despite different names*

### Comparing `audbackend-1.0.1/tests/singlefolder.py` & `audbackend-1.0.2/tests/singlefolder.py`

 * *Files identical despite different names*

### Comparing `audbackend-1.0.1/tests/test_api.py` & `audbackend-1.0.2/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `audbackend-1.0.1/tests/test_artifactory.py` & `audbackend-1.0.2/tests/test_artifactory.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import os
 
-import dohq_artifactory
 import pytest
 
 import audeer
 
 import audbackend
 
 
@@ -66,16 +65,18 @@
     username = 'bad'
     api_key = 'bad'
     with open(config_path, 'w') as fp:
         fp.write(f'[{host}]\n')
         fp.write(f'username = {username}\n')
         fp.write(f'password = {api_key}\n')
 
-    with pytest.raises(dohq_artifactory.exception.ArtifactoryException):
-        audbackend.Artifactory(host, 'repository')
+    backend = audbackend.Artifactory(host, 'repository')
+    assert backend._username == username
+    assert backend._api_key == api_key
+    assert backend._repo is None
 
 
 @pytest.mark.parametrize(
     'backend',
     ['artifactory'],
     indirect=True,
 )
```

### Comparing `audbackend-1.0.1/tests/test_backend.py` & `audbackend-1.0.2/tests/test_backend.py`

 * *Files 0% similar despite different names*

```diff
@@ -590,14 +590,16 @@
         ('/', True, None, root_latest + sub_latest + hidden_latest),
         ('/', False, '*.foo', root_foo + sub + hidden),
         ('/', True, '*.foo', root_foo + sub_latest + hidden_latest),
         ('/sub/', False, None, sub),
         ('/sub/', True, None, sub_latest),
         ('/sub/', False, '*.bar', []),
         ('/sub/', True, '*.bar', []),
+        ('/sub/', False, 'file.*', sub),
+        ('/sub/', True, 'file.*', sub_latest),
         ('/.sub/', False, None, hidden),
         ('/.sub/', True, None, hidden_latest),
         ('/file.bar', False, None, root_bar),
         ('/file.bar', True, None, root_bar_latest),
         ('/sub/file.foo', False, None, sub),
         ('/sub/file.foo', True, None, sub_latest),
         ('/.sub/.file.foo', False, None, hidden),
```

### Comparing `audbackend-1.0.1/tests/test_filesystem.py` & `audbackend-1.0.2/tests/test_filesystem.py`

 * *Files identical despite different names*

