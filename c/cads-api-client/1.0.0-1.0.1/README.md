# Comparing `tmp/cads_api_client-1.0.0.tar.gz` & `tmp/cads_api_client-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cads_api_client-1.0.0.tar", last modified: Thu May  2 10:11:55 2024, max compression
+gzip compressed data, was "cads_api_client-1.0.1.tar", last modified: Fri May 10 12:58:06 2024, max compression
```

## Comparing `cads_api_client-1.0.0.tar` & `cads_api_client-1.0.1.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:11:55.322057 cads_api_client-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-05-02 10:11:42.000000 cads_api_client-1.0.0/.cruft.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:11:55.314057 cads_api_client-1.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:11:55.318057 cads_api_client-1.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     6455 2024-05-02 10:11:42.000000 cads_api_client-1.0.0/.github/workflows/on-push.yml
--rw-r--r--   0 runner    (1001) docker     (127)     8827 2024-05-02 10:11:42.000000 cads_api_client-1.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-02 10:11:42.000000 cads_api_client-1.0.0/.pre-commit-config-cruft.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-05-02 10:11:42.000000 cads_api_client-1.0.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-02 10:11:42.000000 cads_api_client-1.0.0/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)    11346 2024-05-02 10:11:42.000000 cads_api_client-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-02 10:11:42.000000 cads_api_client-1.0.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)    16585 2024-05-02 10:11:55.322057 cads_api_client-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2769 2024-05-02 10:11:42.000000 cads_api_client-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:11:55.318057 cads_api_client-1.0.0/cads_api_client/
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-02 10:11:42.000000 cads_api_client-1.0.0/cads_api_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3659 2024-05-02 10:11:42.000000 cads_api_client-1.0.0/cads_api_client/api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-05-02 10:11:42.000000 cads_api_client-1.0.0/cads_api_client/catalogue.py
--rw-r--r--   0 runner    (1001) docker     (127)      853 2024-05-02 10:11:42.000000 cads_api_client-1.0.0/cads_api_client/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5768 2024-05-02 10:11:42.000000 cads_api_client-1.0.0/cads_api_client/legacy_api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    15219 2024-05-02 10:11:42.000000 cads_api_client-1.0.0/cads_api_client/processing.py
--rw-r--r--   0 runner    (1001) docker     (127)      985 2024-05-02 10:11:42.000000 cads_api_client-1.0.0/cads_api_client/profile.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 10:11:42.000000 cads_api_client-1.0.0/cads_api_client/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-02 10:11:55.000000 cads_api_client-1.0.0/cads_api_client/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:11:55.322057 cads_api_client-1.0.0/cads_api_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16585 2024-05-02 10:11:55.000000 cads_api_client-1.0.0/cads_api_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-02 10:11:55.000000 cads_api_client-1.0.0/cads_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 10:11:55.000000 cads_api_client-1.0.0/cads_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-02 10:11:55.000000 cads_api_client-1.0.0/cads_api_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-02 10:11:55.000000 cads_api_client-1.0.0/cads_api_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:11:55.318057 cads_api_client-1.0.0/ci/
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-02 10:11:42.000000 cads_api_client-1.0.0/ci/environment-ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-02 10:11:42.000000 cads_api_client-1.0.0/ci/environment-integration.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:11:55.318057 cads_api_client-1.0.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-02 10:11:42.000000 cads_api_client-1.0.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:11:55.322057 cads_api_client-1.0.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 10:11:42.000000 cads_api_client-1.0.0/docs/_static/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:11:55.322057 cads_api_client-1.0.0/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 10:11:42.000000 cads_api_client-1.0.0/docs/_templates/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-05-02 10:11:42.000000 cads_api_client-1.0.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-02 10:11:42.000000 cads_api_client-1.0.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-02 10:11:42.000000 cads_api_client-1.0.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-02 10:11:42.000000 cads_api_client-1.0.0/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:11:55.322057 cads_api_client-1.0.0/notebooks/
--rw-r--r--   0 runner    (1001) docker     (127)    15779 2024-05-02 10:11:42.000000 cads_api_client-1.0.0/notebooks/cads_api_client_test.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    44415 2024-05-02 10:11:42.000000 cads_api_client-1.0.0/notebooks/cads_api_constraints_test.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    12254 2024-05-02 10:11:42.000000 cads_api_client-1.0.0/notebooks/cads_api_filters_and_pagination_tests.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     4751 2024-05-02 10:11:42.000000 cads_api_client-1.0.0/notebooks/cads_api_licences_tests.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-05-02 10:11:42.000000 cads_api_client-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 10:11:55.322057 cads_api_client-1.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:11:55.322057 cads_api_client-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-02 10:11:42.000000 cads_api_client-1.0.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-05-02 10:11:42.000000 cads_api_client-1.0.0/tests/integration_test_10_catalogue.py
--rw-r--r--   0 runner    (1001) docker     (127)     3025 2024-05-02 10:11:42.000000 cads_api_client-1.0.0/tests/integration_test_20_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)     4602 2024-05-02 10:11:42.000000 cads_api_client-1.0.0/tests/integration_test_30_remote.py
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-02 10:11:42.000000 cads_api_client-1.0.0/tests/integration_test_40_api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-05-02 10:11:42.000000 cads_api_client-1.0.0/tests/integration_test_50_legacy_api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-02 10:11:42.000000 cads_api_client-1.0.0/tests/test_00_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-05-02 10:11:42.000000 cads_api_client-1.0.0/tests/test_10_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    11089 2024-05-02 10:11:42.000000 cads_api_client-1.0.0/tests/test_10_processing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:58:06.514692 cads_api_client-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-05-10 12:57:57.000000 cads_api_client-1.0.1/.cruft.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:58:06.506692 cads_api_client-1.0.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:58:06.506692 cads_api_client-1.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     6455 2024-05-10 12:57:57.000000 cads_api_client-1.0.1/.github/workflows/on-push.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     8827 2024-05-10 12:57:57.000000 cads_api_client-1.0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-10 12:57:57.000000 cads_api_client-1.0.1/.pre-commit-config-cruft.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-05-10 12:57:57.000000 cads_api_client-1.0.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-10 12:57:57.000000 cads_api_client-1.0.1/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)    11346 2024-05-10 12:57:57.000000 cads_api_client-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-10 12:57:57.000000 cads_api_client-1.0.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    16585 2024-05-10 12:58:06.514692 cads_api_client-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2769 2024-05-10 12:57:57.000000 cads_api_client-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:58:06.510692 cads_api_client-1.0.1/cads_api_client/
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-10 12:57:57.000000 cads_api_client-1.0.1/cads_api_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3659 2024-05-10 12:57:57.000000 cads_api_client-1.0.1/cads_api_client/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-05-10 12:57:57.000000 cads_api_client-1.0.1/cads_api_client/catalogue.py
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-05-10 12:57:57.000000 cads_api_client-1.0.1/cads_api_client/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5768 2024-05-10 12:57:57.000000 cads_api_client-1.0.1/cads_api_client/legacy_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15821 2024-05-10 12:57:57.000000 cads_api_client-1.0.1/cads_api_client/processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-05-10 12:57:57.000000 cads_api_client-1.0.1/cads_api_client/profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 12:57:57.000000 cads_api_client-1.0.1/cads_api_client/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-10 12:58:06.000000 cads_api_client-1.0.1/cads_api_client/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:58:06.514692 cads_api_client-1.0.1/cads_api_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16585 2024-05-10 12:58:06.000000 cads_api_client-1.0.1/cads_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-10 12:58:06.000000 cads_api_client-1.0.1/cads_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 12:58:06.000000 cads_api_client-1.0.1/cads_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-10 12:58:06.000000 cads_api_client-1.0.1/cads_api_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-10 12:58:06.000000 cads_api_client-1.0.1/cads_api_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:58:06.510692 cads_api_client-1.0.1/ci/
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-10 12:57:57.000000 cads_api_client-1.0.1/ci/environment-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-10 12:57:57.000000 cads_api_client-1.0.1/ci/environment-integration.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:58:06.510692 cads_api_client-1.0.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-10 12:57:57.000000 cads_api_client-1.0.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:58:06.510692 cads_api_client-1.0.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 12:57:57.000000 cads_api_client-1.0.1/docs/_static/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:58:06.510692 cads_api_client-1.0.1/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 12:57:57.000000 cads_api_client-1.0.1/docs/_templates/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-05-10 12:57:57.000000 cads_api_client-1.0.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-10 12:57:57.000000 cads_api_client-1.0.1/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-10 12:57:57.000000 cads_api_client-1.0.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-10 12:57:57.000000 cads_api_client-1.0.1/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:58:06.510692 cads_api_client-1.0.1/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)    15779 2024-05-10 12:57:57.000000 cads_api_client-1.0.1/notebooks/cads_api_client_test.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    44415 2024-05-10 12:57:57.000000 cads_api_client-1.0.1/notebooks/cads_api_constraints_test.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    12254 2024-05-10 12:57:57.000000 cads_api_client-1.0.1/notebooks/cads_api_filters_and_pagination_tests.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     4751 2024-05-10 12:57:57.000000 cads_api_client-1.0.1/notebooks/cads_api_licences_tests.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-05-10 12:57:57.000000 cads_api_client-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 12:58:06.514692 cads_api_client-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:58:06.514692 cads_api_client-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-10 12:57:57.000000 cads_api_client-1.0.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-05-10 12:57:57.000000 cads_api_client-1.0.1/tests/integration_test_10_catalogue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3025 2024-05-10 12:57:57.000000 cads_api_client-1.0.1/tests/integration_test_20_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4602 2024-05-10 12:57:57.000000 cads_api_client-1.0.1/tests/integration_test_30_remote.py
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-10 12:57:57.000000 cads_api_client-1.0.1/tests/integration_test_40_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-05-10 12:57:57.000000 cads_api_client-1.0.1/tests/integration_test_50_legacy_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-10 12:57:57.000000 cads_api_client-1.0.1/tests/test_00_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-05-10 12:57:57.000000 cads_api_client-1.0.1/tests/test_10_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14768 2024-05-10 12:57:57.000000 cads_api_client-1.0.1/tests/test_10_processing.py
```

### Comparing `cads_api_client-1.0.0/.github/workflows/on-push.yml` & `cads_api_client-1.0.1/.github/workflows/on-push.yml`

 * *Files identical despite different names*

### Comparing `cads_api_client-1.0.0/.gitignore` & `cads_api_client-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `cads_api_client-1.0.0/.pre-commit-config.yaml` & `cads_api_client-1.0.1/.pre-commit-config.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
   - id: mixed-line-ending
 - repo: https://github.com/keewis/blackdoc
   rev: v0.3.9
   hooks:
   - id: blackdoc
     additional_dependencies: [black==23.11.0]
 - repo: https://github.com/astral-sh/ruff-pre-commit
-  rev: v0.4.2
+  rev: v0.4.3
   hooks:
   - id: ruff
     args: [--fix, --show-fixes]
   - id: ruff-format
 - repo: https://github.com/executablebooks/mdformat
   rev: 0.7.17
   hooks:
```

### Comparing `cads_api_client-1.0.0/LICENSE` & `cads_api_client-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cads_api_client-1.0.0/Makefile` & `cads_api_client-1.0.1/Makefile`

 * *Files identical despite different names*

### Comparing `cads_api_client-1.0.0/PKG-INFO` & `cads_api_client-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cads-api-client
-Version: 1.0.0
+Version: 1.0.1
 Summary: CADS API Python client
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `cads_api_client-1.0.0/README.md` & `cads_api_client-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `cads_api_client-1.0.0/cads_api_client/__init__.py` & `cads_api_client-1.0.1/cads_api_client/__init__.py`

 * *Files identical despite different names*

### Comparing `cads_api_client-1.0.0/cads_api_client/api_client.py` & `cads_api_client-1.0.1/cads_api_client/api_client.py`

 * *Files identical despite different names*

### Comparing `cads_api_client-1.0.0/cads_api_client/catalogue.py` & `cads_api_client-1.0.1/cads_api_client/catalogue.py`

 * *Files identical despite different names*

### Comparing `cads_api_client-1.0.0/cads_api_client/config.py` & `cads_api_client-1.0.1/cads_api_client/config.py`

 * *Files identical despite different names*

### Comparing `cads_api_client-1.0.0/cads_api_client/legacy_api_client.py` & `cads_api_client-1.0.1/cads_api_client/legacy_api_client.py`

 * *Files identical despite different names*

### Comparing `cads_api_client-1.0.0/cads_api_client/processing.py` & `cads_api_client-1.0.1/cads_api_client/processing.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,25 +25,38 @@
     pass
 
 
 class DownloadError(RuntimeError):
     pass
 
 
+def error_json_to_message(error_json: dict[str, Any]) -> str:
+    error_messages = [
+        str(error_json[key])
+        for key in ("title", "traceback", "detail")
+        if key in error_json
+    ]
+    if trace_id := error_json.get("trace_id"):
+        error_messages.append(f"Trace ID is {trace_id}")
+    return "\n".join(error_messages)
+
+
 def cads_raise_for_status(response: requests.Response) -> None:
     if response.status_code > 499:
         response.raise_for_status()
     if response.status_code > 399:
         error_json = None
         try:
             error_json = response.json()
         except Exception:
             pass
         if error_json is not None:
-            raise RuntimeError(f"{response.status_code} Client Error: {error_json}")
+            raise RuntimeError(
+                f"{response.status_code} Client Error: {error_json_to_message(error_json)}"
+            )
         else:
             response.raise_for_status()
 
 
 @attrs.define(slots=False)
 class ApiResponse:
     response: requests.Response
@@ -55,15 +68,21 @@
         cls: Type[T_ApiResponse],
         *args: Any,
         raise_for_status: bool = True,
         session: requests.Session = requests.api,  # type: ignore
         retry_options: Dict[str, Any] = {"maximum_tries": 2, "retry_after": 10},
         **kwargs: Any,
     ) -> T_ApiResponse:
+        method = kwargs["method"] if "method" in kwargs else args[0]
+        url = kwargs["url"] if "url" in kwargs else args[1]
+        inputs = kwargs.get("json", {}).get("inputs", {})
+        logger.debug(f"{method.upper()} {url} {inputs}")
         response = multiurl.robust(session.request, **retry_options)(*args, **kwargs)
+        logger.debug(f"REPLY {response.text}")
+
         if raise_for_status:
             cads_raise_for_status(response)
         self = cls(response, headers=kwargs.get("headers", {}), session=session)
         self.log_messages()
         return self
 
     @functools.cached_property
@@ -164,14 +183,15 @@
         session: requests.Session = requests.api,  # type: ignore
     ):
         self.url = url
         self.sleep_max = sleep_max
         self.headers = headers
         self.session = session
         self.log_start_time = None
+        logger.debug(f"Request UID is {self.request_uid}")
 
     def log_metadata(self, metadata: dict[str, Any]) -> None:
         logs = metadata.get("log", [])
         for self.log_start_time, message in sorted(logs):
             level = 20
             for severity in ("DEBUG", "INFO", "WARNING", "ERROR", "CRITICAL"):
                 if message.startswith(severity):
@@ -192,14 +212,15 @@
 
         params = {"log": True}
         if self.log_start_time:
             params["logStartTime"] = self.log_start_time
 
         logger.debug(f"GET {self.url}")
         requests_response = get(url=self.url, headers=self.headers, params=params)
+        logger.debug(f"REPLY {requests_response.text}")
         requests_response.raise_for_status()
         json = requests_response.json()
         self.log_metadata(json.get("metadata", {}))
         return str(json["status"])
 
     @property
     def status(self) -> str:
@@ -218,22 +239,15 @@
                 # workaround for the server-side 404 due to database replicas out od sync
                 time.sleep(1)
                 break
             elif status == "failed":
                 # workaround for the server-side 404 due to database replicas out od sync
                 time.sleep(1)
                 results = multiurl.robust(self.make_results, **retry_options)(self.url)
-                info = results.json
-                error_message = "processing failed"
-                if info.get("title"):
-                    error_message = f'{info["title"]}'
-                if info.get("detail"):
-                    error_message = error_message + f': {info["detail"]}'
-                raise ProcessingFailedError(error_message)
-                break
+                raise ProcessingFailedError(error_json_to_message(results.json))
             elif status in ("accepted", "running"):
                 sleep *= 1.5
                 if sleep > self.sleep_max:
                     sleep = self.sleep_max
             else:
                 raise ProcessingFailedError(f"Unknown API state {status!r}")
             logger.debug(f"result not ready, waiting for {sleep} seconds")
@@ -246,15 +260,19 @@
 
     def make_results(self, url: Optional[str] = None) -> Results:
         if url is None:
             url = self.url
         status = self.status
         if status not in ("successful", "failed"):
             raise ValueError(f"Result not ready, job is {status}")
+
+        logger.debug(f"GET {url}")
         request_response = self.session.get(url, headers=self.headers)
+        logger.debug(f"REPLY {request_response.text}")
+
         response = ApiResponse(request_response, session=self.session)
         try:
             results_url = response.get_link_href(rel="results")
         except RuntimeError:
             results_url = f"{url}/results"
         results = Results.from_request(
             "get",
```

### Comparing `cads_api_client-1.0.0/cads_api_client/profile.py` & `cads_api_client-1.0.1/cads_api_client/profile.py`

 * *Files identical despite different names*

### Comparing `cads_api_client-1.0.0/cads_api_client.egg-info/PKG-INFO` & `cads_api_client-1.0.1/cads_api_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cads-api-client
-Version: 1.0.0
+Version: 1.0.1
 Summary: CADS API Python client
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `cads_api_client-1.0.0/cads_api_client.egg-info/SOURCES.txt` & `cads_api_client-1.0.1/cads_api_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cads_api_client-1.0.0/docs/Makefile` & `cads_api_client-1.0.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cads_api_client-1.0.0/docs/conf.py` & `cads_api_client-1.0.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `cads_api_client-1.0.0/docs/make.bat` & `cads_api_client-1.0.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cads_api_client-1.0.0/notebooks/cads_api_client_test.ipynb` & `cads_api_client-1.0.1/notebooks/cads_api_client_test.ipynb`

 * *Files identical despite different names*

### Comparing `cads_api_client-1.0.0/notebooks/cads_api_constraints_test.ipynb` & `cads_api_client-1.0.1/notebooks/cads_api_constraints_test.ipynb`

 * *Files identical despite different names*

### Comparing `cads_api_client-1.0.0/notebooks/cads_api_filters_and_pagination_tests.ipynb` & `cads_api_client-1.0.1/notebooks/cads_api_filters_and_pagination_tests.ipynb`

 * *Files identical despite different names*

### Comparing `cads_api_client-1.0.0/notebooks/cads_api_licences_tests.ipynb` & `cads_api_client-1.0.1/notebooks/cads_api_licences_tests.ipynb`

 * *Files identical despite different names*

### Comparing `cads_api_client-1.0.0/pyproject.toml` & `cads_api_client-1.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cads_api_client-1.0.0/tests/conftest.py` & `cads_api_client-1.0.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `cads_api_client-1.0.0/tests/integration_test_10_catalogue.py` & `cads_api_client-1.0.1/tests/integration_test_10_catalogue.py`

 * *Files identical despite different names*

### Comparing `cads_api_client-1.0.0/tests/integration_test_20_processing.py` & `cads_api_client-1.0.1/tests/integration_test_20_processing.py`

 * *Files identical despite different names*

### Comparing `cads_api_client-1.0.0/tests/integration_test_30_remote.py` & `cads_api_client-1.0.1/tests/integration_test_30_remote.py`

 * *Files identical despite different names*

### Comparing `cads_api_client-1.0.0/tests/integration_test_40_api_client.py` & `cads_api_client-1.0.1/tests/integration_test_40_api_client.py`

 * *Files identical despite different names*

### Comparing `cads_api_client-1.0.0/tests/integration_test_50_legacy_api_client.py` & `cads_api_client-1.0.1/tests/integration_test_50_legacy_api_client.py`

 * *Files identical despite different names*

### Comparing `cads_api_client-1.0.0/tests/test_10_config.py` & `cads_api_client-1.0.1/tests/test_10_config.py`

 * *Files identical despite different names*

### Comparing `cads_api_client-1.0.0/tests/test_10_processing.py` & `cads_api_client-1.0.1/tests/test_10_processing.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,43 @@
+import json
 import logging
 
 import pytest
 import responses
 from responses.matchers import json_params_matcher
 
 import cads_api_client
 
 COLLECTION_ID = "reanalysis-era5-pressure-levels"
 JOB_RUNNING_ID = "9bfc1362-2832-48e1-a235-359267420bb1"
 JOB_SUCCESSFUL_ID = "9bfc1362-2832-48e1-a235-359267420bb2"
+JOB_FAILED_ID = "9bfc1362-2832-48e1-a235-359267420bb3"
 
 CATALOGUE_URL = "http://localhost:8080/api/catalogue"
 COLLECTIONS_URL = "http://localhost:8080/api/catalogue/v1/datasets"
 COLLECTION_URL = (
     "http://localhost:8080/api/catalogue/v1/collections/reanalysis-era5-pressure-levels"
 )
 PROCESS_URL = f"http://localhost:8080/api/retrieve/v1/processes/{COLLECTION_ID}"
 EXECUTE_URL = f"{PROCESS_URL}/execute"
 
 JOB_RUNNING_URL = f"http://localhost:8080/api/retrieve/v1/jobs/{JOB_RUNNING_ID}"
 JOB_SUCCESSFUL_URL = f"http://localhost:8080/api/retrieve/v1/jobs/{JOB_SUCCESSFUL_ID}"
+JOB_FAILED_URL = f"http://localhost:8080/api/retrieve/v1/jobs/{JOB_FAILED_ID}"
 
 RESULT_RUNNING_URL = (
     f"http://localhost:8080/api/retrieve/v1/jobs/{JOB_RUNNING_ID}/results"
 )
 RESULT_SUCCESSFUL_URL = (
     f"http://localhost:8080/api/retrieve/v1/jobs/{JOB_SUCCESSFUL_ID}/results"
 )
+RESULT_FAILED_URL = (
+    f"http://localhost:8080/api/retrieve/v1/jobs/{JOB_FAILED_ID}/results"
+)
+
 
 CATALOGUE_JSON = {
     "type": "Catalog",
     "id": "stac-fastapi",
     "links": [
         {"rel": "self", "type": "application/json", "href": f"{CATALOGUE_URL}/v1"},
         {"rel": "root", "type": "application/json", "href": f"{CATALOGUE_URL}/v1"},
@@ -136,15 +143,18 @@
             "schema": {
                 "type": "array",
                 "items": {"enum": ["temperature", "vorticity"], "type": "string"},
             },
         },
         "year": {
             "title": "Year",
-            "schema": {"type": "array", "items": {"enum": ["2022"], "type": "string"}},
+            "schema": {
+                "type": "array",
+                "items": {"enum": ["2022", "0000"], "type": "string"},
+            },
         },
     },
     "outputs": {
         "download_url": {
             "schema": {"type": "string", "format": "url"},
         }
     },
@@ -215,14 +225,44 @@
         "log": [
             ["2024-02-09T09:14:47.811223", "This is a log"],
             ["2024-02-09T09:14:50.811223", "WARNING: This is a warning log"],
         ]
     },
 }
 
+JOB_FAILED_JSON = {
+    "processID": f"{COLLECTION_ID}",
+    "type": "process",
+    "jobID": f"{JOB_FAILED_ID}",
+    "status": "failed",
+    "created": "2022-09-02T17:30:48.201213",
+    "started": "2022-09-02T17:32:43.890617",
+    "finished": "2022-09-02T17:32:54.308120",
+    "updated": "2022-09-02T17:32:54.308116",
+    "links": [
+        {"href": f"{JOB_FAILED_ID}", "rel": "self", "type": "application/json"},
+        {
+            "href": f"http://localhost:8080/api/retrieve/v1/jobs/{JOB_FAILED_ID}/results",
+            "rel": "results",
+        },
+        {
+            "href": f"{JOB_FAILED_URL}",
+            "rel": "monitor",
+            "type": "application/json",
+            "title": "job status info",
+        },
+    ],
+    "metadata": {
+        "log": [
+            ["2024-02-09T09:14:47.811223", "This is a log"],
+            ["2024-02-09T09:14:50.811223", "WARNING: This is a warning log"],
+        ]
+    },
+}
+
 RESULT_SUCCESSFUL_JSON = {
     "asset": {
         "value": {
             "type": "application/netcdf",
             "href": "./e7d452a747061ab880887d88814bfb0c27593a73cb7736d2dc340852",
             "file:checksum": "e7d452a747061ab880887d88814bfb0c27593a73cb7736d2dc340852",
             "file:size": 8,
@@ -240,14 +280,23 @@
 RESULT_RUNNING_JSON = {
     "type": "http://www.opengis.net/def/exceptions/ogcapi-processes-1/1.0/result-not-ready",
     "title": "job results not ready",
     "detail": "job 8b7a1f3d-04b1-425d-96f1-f0634d02ee7f results are not yet ready",
     "instance": "http://127.0.0.1:8080/api/retrieve/v1/jobs/8b7a1f3d-04b1-425d-96f1-f0634d02ee7f/results",
 }
 
+RESULT_FAILED_JSON = {
+    "type": "job results failed",
+    "title": "job failed",
+    "status": 400,
+    "instance": "http://127.0.0.1:8080/api/retrieve/v1/jobs/02135eee-39a8-4d1f-8cd7-87682de5b981/results",
+    "trace_id": "ca3e7170-1ce2-48fc-97f8-bbe64fafce44",
+    "traceback": "This is a traceback",
+}
+
 
 def responses_add() -> None:
     responses.add(
         responses.GET,
         url=f"{CATALOGUE_URL}/v1/",
         json=CATALOGUE_JSON,
         content_type="application/json",
@@ -291,14 +340,42 @@
     responses.add(
         responses.GET,
         url=JOB_SUCCESSFUL_URL,
         json=JOB_SUCCESSFUL_JSON,
         content_type="application/json",
     )
 
+    responses.add(
+        responses.POST,
+        url=EXECUTE_URL,
+        json=JOB_FAILED_JSON,
+        match=[
+            json_params_matcher(
+                {
+                    "inputs": {"variable": "temperature", "year": "0000"},
+                }
+            )
+        ],
+        content_type="application/json",
+    )
+
+    responses.add(
+        responses.GET,
+        url=JOB_FAILED_URL,
+        json=JOB_FAILED_JSON,
+        content_type="application/json",
+    )
+
+    responses.add(
+        responses.GET,
+        url=RESULT_FAILED_URL,
+        json=RESULT_FAILED_JSON,
+        content_type="application/json",
+    )
+
 
 @responses.activate
 def test_catalogue_collections() -> None:
     responses_add()
 
     catalogue = cads_api_client.Catalogue(CATALOGUE_URL)
 
@@ -334,37 +411,85 @@
     catalogue = cads_api_client.Catalogue(CATALOGUE_URL)
     collection = catalogue.collection(COLLECTION_ID)
     remote = collection.submit(variable="temperature", year="2022")
     remote.wait_on_result()
 
 
 @responses.activate
-def test_log_messages(caplog: pytest.LogCaptureFixture) -> None:
+def test_wait_on_result_failed() -> None:
+    responses_add()
+
+    catalogue = cads_api_client.Catalogue(CATALOGUE_URL)
+    collection = catalogue.collection(COLLECTION_ID)
+    remote = collection.submit(variable="temperature", year="0000")
+    with pytest.raises(
+        cads_api_client.processing.ProcessingFailedError,
+        match="job failed\nThis is a traceback\nTrace ID is ca3e7170-1ce2-48fc-97f8-bbe64fafce44",
+    ):
+        remote.wait_on_result()
+
+
+@responses.activate
+def test_remote_logs(caplog: pytest.LogCaptureFixture) -> None:
     responses_add()
 
     catalogue = cads_api_client.Catalogue(CATALOGUE_URL)
     collection = catalogue.collection(COLLECTION_ID)
 
     with caplog.at_level(logging.DEBUG, logger="cads_api_client.processing"):
         remote = collection.submit(variable="temperature", year="2022")
         remote.wait_on_result()
 
     assert caplog.record_tuples == [
         (
             "cads_api_client.processing",
+            10,
+            "GET http://localhost:8080/api/retrieve/v1/processes/reanalysis-era5-pressure-levels {}",
+        ),
+        (
+            "cads_api_client.processing",
+            10,
+            f"REPLY {json.dumps(PROCESS_JSON)}",
+        ),
+        (
+            "cads_api_client.processing",
             30,
             "[2023-12-12T13:00:00] This is a warning message",
         ),
         (
             "cads_api_client.processing",
             20,
             "[2023-12-12T14:00:00] This is a success message",
         ),
         (
             "cads_api_client.processing",
             10,
+            (
+                "POST http://localhost:8080/api/retrieve/v1/processes/"
+                "reanalysis-era5-pressure-levels/execute "
+                "{'variable': 'temperature', 'year': '2022'}"
+            ),
+        ),
+        (
+            "cads_api_client.processing",
+            10,
+            f"REPLY {json.dumps(JOB_SUCCESSFUL_JSON)}",
+        ),
+        (
+            "cads_api_client.processing",
+            10,
+            "Request UID is 9bfc1362-2832-48e1-a235-359267420bb2",
+        ),
+        (
+            "cads_api_client.processing",
+            10,
             "GET http://localhost:8080/api/retrieve/v1/jobs/9bfc1362-2832-48e1-a235-359267420bb2",
         ),
+        (
+            "cads_api_client.processing",
+            10,
+            f"REPLY {json.dumps(JOB_SUCCESSFUL_JSON)}",
+        ),
         ("cads_api_client.processing", 20, "This is a log"),
         ("cads_api_client.processing", 30, "This is a warning log"),
         ("cads_api_client.processing", 20, "status has been updated to successful"),
     ]
```

