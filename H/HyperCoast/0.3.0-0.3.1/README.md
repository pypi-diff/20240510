# Comparing `tmp/hypercoast-0.3.0.tar.gz` & `tmp/hypercoast-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hypercoast-0.3.0.tar", last modified: Wed May  8 15:21:38 2024, max compression
+gzip compressed data, was "hypercoast-0.3.1.tar", last modified: Thu May  9 20:09:57 2024, max compression
```

## Comparing `hypercoast-0.3.0.tar` & `hypercoast-0.3.1.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:21:38.513407 hypercoast-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-08 15:21:25.000000 hypercoast-0.3.0/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:21:38.501407 hypercoast-0.3.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:21:38.505407 hypercoast-0.3.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-08 15:21:25.000000 hypercoast-0.3.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-08 15:21:25.000000 hypercoast-0.3.0/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-08 15:21:25.000000 hypercoast-0.3.0/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:21:38.509407 hypercoast-0.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-05-08 15:21:25.000000 hypercoast-0.3.0/.github/workflows/docs-build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-08 15:21:25.000000 hypercoast-0.3.0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-08 15:21:25.000000 hypercoast-0.3.0/.github/workflows/installation.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-08 15:21:25.000000 hypercoast-0.3.0/.github/workflows/macos.yml
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-08 15:21:25.000000 hypercoast-0.3.0/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-05-08 15:21:25.000000 hypercoast-0.3.0/.github/workflows/ubuntu.yml
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-08 15:21:25.000000 hypercoast-0.3.0/.github/workflows/windows.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-05-08 15:21:25.000000 hypercoast-0.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-08 15:21:25.000000 hypercoast-0.3.0/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:21:38.513407 hypercoast-0.3.0/HyperCoast.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-05-08 15:21:38.000000 hypercoast-0.3.0/HyperCoast.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-05-08 15:21:38.000000 hypercoast-0.3.0/HyperCoast.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 15:21:38.000000 hypercoast-0.3.0/HyperCoast.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-08 15:21:38.000000 hypercoast-0.3.0/HyperCoast.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-08 15:21:38.000000 hypercoast-0.3.0/HyperCoast.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-08 15:21:38.000000 hypercoast-0.3.0/HyperCoast.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-08 15:21:25.000000 hypercoast-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-08 15:21:25.000000 hypercoast-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-05-08 15:21:38.513407 hypercoast-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-05-08 15:21:25.000000 hypercoast-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:21:38.509407 hypercoast-0.3.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-08 15:21:25.000000 hypercoast-0.3.0/docs/CNAME
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-08 15:21:25.000000 hypercoast-0.3.0/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 15:21:25.000000 hypercoast-0.3.0/docs/common.md
--rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-05-08 15:21:25.000000 hypercoast-0.3.0/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-08 15:21:25.000000 hypercoast-0.3.0/docs/emit.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:21:38.513407 hypercoast-0.3.0/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-05-08 15:21:25.000000 hypercoast-0.3.0/docs/examples/emit.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     4720 2024-05-08 15:21:25.000000 hypercoast-0.3.0/docs/examples/pace.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-08 15:21:25.000000 hypercoast-0.3.0/docs/faq.md
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-08 15:21:25.000000 hypercoast-0.3.0/docs/hypercoast.md
--rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-05-08 15:21:25.000000 hypercoast-0.3.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-05-08 15:21:25.000000 hypercoast-0.3.0/docs/installation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:21:38.513407 hypercoast-0.3.0/docs/overrides/
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-08 15:21:25.000000 hypercoast-0.3.0/docs/overrides/main.html
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-08 15:21:25.000000 hypercoast-0.3.0/docs/pace.md
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-08 15:21:25.000000 hypercoast-0.3.0/docs/ui.md
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-08 15:21:25.000000 hypercoast-0.3.0/docs/usage.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:21:38.513407 hypercoast-0.3.0/hypercoast/
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-08 15:21:25.000000 hypercoast-0.3.0/hypercoast/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4766 2024-05-08 15:21:25.000000 hypercoast-0.3.0/hypercoast/common.py
--rw-r--r--   0 runner    (1001) docker     (127)    37765 2024-05-08 15:21:25.000000 hypercoast-0.3.0/hypercoast/emit.py
--rw-r--r--   0 runner    (1001) docker     (127)    13949 2024-05-08 15:21:25.000000 hypercoast-0.3.0/hypercoast/hypercoast.py
--rw-r--r--   0 runner    (1001) docker     (127)    13730 2024-05-08 15:21:25.000000 hypercoast-0.3.0/hypercoast/pace.py
--rw-r--r--   0 runner    (1001) docker     (127)     9091 2024-05-08 15:21:25.000000 hypercoast-0.3.0/hypercoast/ui.py
--rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-05-08 15:21:25.000000 hypercoast-0.3.0/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-08 15:21:25.000000 hypercoast-0.3.0/pyproject-codespell.precommit-toml
--rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-05-08 15:21:25.000000 hypercoast-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-08 15:21:25.000000 hypercoast-0.3.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-08 15:21:25.000000 hypercoast-0.3.0/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 15:21:38.513407 hypercoast-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:21:38.513407 hypercoast-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-08 15:21:25.000000 hypercoast-0.3.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-08 15:21:25.000000 hypercoast-0.3.0/tests/test_hypercoast.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 20:09:57.206614 hypercoast-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-09 20:09:46.000000 hypercoast-0.3.1/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 20:09:57.194614 hypercoast-0.3.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 20:09:57.198614 hypercoast-0.3.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-09 20:09:46.000000 hypercoast-0.3.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-09 20:09:46.000000 hypercoast-0.3.1/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-09 20:09:46.000000 hypercoast-0.3.1/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 20:09:57.198614 hypercoast-0.3.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-05-09 20:09:46.000000 hypercoast-0.3.1/.github/workflows/docs-build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-09 20:09:46.000000 hypercoast-0.3.1/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-09 20:09:46.000000 hypercoast-0.3.1/.github/workflows/installation.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-09 20:09:46.000000 hypercoast-0.3.1/.github/workflows/macos.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-09 20:09:46.000000 hypercoast-0.3.1/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-05-09 20:09:46.000000 hypercoast-0.3.1/.github/workflows/ubuntu.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-09 20:09:46.000000 hypercoast-0.3.1/.github/workflows/windows.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-05-09 20:09:46.000000 hypercoast-0.3.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-09 20:09:46.000000 hypercoast-0.3.1/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 20:09:57.206614 hypercoast-0.3.1/HyperCoast.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-05-09 20:09:57.000000 hypercoast-0.3.1/HyperCoast.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-05-09 20:09:57.000000 hypercoast-0.3.1/HyperCoast.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 20:09:57.000000 hypercoast-0.3.1/HyperCoast.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-09 20:09:57.000000 hypercoast-0.3.1/HyperCoast.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-09 20:09:57.000000 hypercoast-0.3.1/HyperCoast.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-09 20:09:57.000000 hypercoast-0.3.1/HyperCoast.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-09 20:09:46.000000 hypercoast-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-09 20:09:46.000000 hypercoast-0.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-05-09 20:09:57.206614 hypercoast-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-05-09 20:09:46.000000 hypercoast-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 20:09:57.202614 hypercoast-0.3.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-09 20:09:46.000000 hypercoast-0.3.1/docs/CNAME
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-09 20:09:46.000000 hypercoast-0.3.1/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 20:09:46.000000 hypercoast-0.3.1/docs/common.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-05-09 20:09:46.000000 hypercoast-0.3.1/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-09 20:09:46.000000 hypercoast-0.3.1/docs/emit.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 20:09:57.202614 hypercoast-0.3.1/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-05-09 20:09:46.000000 hypercoast-0.3.1/docs/examples/emit.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     4720 2024-05-09 20:09:46.000000 hypercoast-0.3.1/docs/examples/pace.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-09 20:09:46.000000 hypercoast-0.3.1/docs/faq.md
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-09 20:09:46.000000 hypercoast-0.3.1/docs/hypercoast.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-05-09 20:09:46.000000 hypercoast-0.3.1/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-05-09 20:09:46.000000 hypercoast-0.3.1/docs/installation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 20:09:57.202614 hypercoast-0.3.1/docs/overrides/
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-09 20:09:46.000000 hypercoast-0.3.1/docs/overrides/main.html
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-09 20:09:46.000000 hypercoast-0.3.1/docs/pace.md
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-09 20:09:46.000000 hypercoast-0.3.1/docs/ui.md
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-09 20:09:46.000000 hypercoast-0.3.1/docs/usage.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 20:09:57.206614 hypercoast-0.3.1/hypercoast/
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-09 20:09:46.000000 hypercoast-0.3.1/hypercoast/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4766 2024-05-09 20:09:46.000000 hypercoast-0.3.1/hypercoast/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37765 2024-05-09 20:09:46.000000 hypercoast-0.3.1/hypercoast/emit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13933 2024-05-09 20:09:46.000000 hypercoast-0.3.1/hypercoast/hypercoast.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13745 2024-05-09 20:09:46.000000 hypercoast-0.3.1/hypercoast/pace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9091 2024-05-09 20:09:46.000000 hypercoast-0.3.1/hypercoast/ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-05-09 20:09:46.000000 hypercoast-0.3.1/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-09 20:09:46.000000 hypercoast-0.3.1/pyproject-codespell.precommit-toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-05-09 20:09:46.000000 hypercoast-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-09 20:09:46.000000 hypercoast-0.3.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-09 20:09:46.000000 hypercoast-0.3.1/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 20:09:57.206614 hypercoast-0.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 20:09:57.206614 hypercoast-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-09 20:09:46.000000 hypercoast-0.3.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-09 20:09:46.000000 hypercoast-0.3.1/tests/test_hypercoast.py
```

### Comparing `hypercoast-0.3.0/.github/workflows/docs-build.yml` & `hypercoast-0.3.1/.github/workflows/docs-build.yml`

 * *Files identical despite different names*

### Comparing `hypercoast-0.3.0/.github/workflows/docs.yml` & `hypercoast-0.3.1/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `hypercoast-0.3.0/.github/workflows/installation.yml` & `hypercoast-0.3.1/.github/workflows/installation.yml`

 * *Files identical despite different names*

### Comparing `hypercoast-0.3.0/.github/workflows/macos.yml` & `hypercoast-0.3.1/.github/workflows/macos.yml`

 * *Files identical despite different names*

### Comparing `hypercoast-0.3.0/.github/workflows/pypi.yml` & `hypercoast-0.3.1/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `hypercoast-0.3.0/.github/workflows/ubuntu.yml` & `hypercoast-0.3.1/.github/workflows/ubuntu.yml`

 * *Files identical despite different names*

### Comparing `hypercoast-0.3.0/.github/workflows/windows.yml` & `hypercoast-0.3.1/.github/workflows/windows.yml`

 * *Files identical despite different names*

### Comparing `hypercoast-0.3.0/.gitignore` & `hypercoast-0.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `hypercoast-0.3.0/.pre-commit-config.yaml` & `hypercoast-0.3.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `hypercoast-0.3.0/HyperCoast.egg-info/PKG-INFO` & `hypercoast-0.3.1/HyperCoast.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HyperCoast
-Version: 0.3.0
+Version: 0.3.1
 Summary: A Python package for processing hyperspectral data in coastal regions
 Author-email: Qiusheng Wu <giswqs@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/opengeos/HyperCoast
 Keywords: HyperCoast
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `hypercoast-0.3.0/HyperCoast.egg-info/SOURCES.txt` & `hypercoast-0.3.1/HyperCoast.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hypercoast-0.3.0/LICENSE` & `hypercoast-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hypercoast-0.3.0/PKG-INFO` & `hypercoast-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HyperCoast
-Version: 0.3.0
+Version: 0.3.1
 Summary: A Python package for processing hyperspectral data in coastal regions
 Author-email: Qiusheng Wu <giswqs@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/opengeos/HyperCoast
 Keywords: HyperCoast
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `hypercoast-0.3.0/README.md` & `hypercoast-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `hypercoast-0.3.0/docs/contributing.md` & `hypercoast-0.3.1/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `hypercoast-0.3.0/docs/examples/emit.ipynb` & `hypercoast-0.3.1/docs/examples/emit.ipynb`

 * *Files identical despite different names*

### Comparing `hypercoast-0.3.0/docs/examples/pace.ipynb` & `hypercoast-0.3.1/docs/examples/pace.ipynb`

 * *Files identical despite different names*

### Comparing `hypercoast-0.3.0/docs/index.md` & `hypercoast-0.3.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `hypercoast-0.3.0/docs/installation.md` & `hypercoast-0.3.1/docs/installation.md`

 * *Files identical despite different names*

### Comparing `hypercoast-0.3.0/hypercoast/common.py` & `hypercoast-0.3.1/hypercoast/common.py`

 * *Files identical despite different names*

### Comparing `hypercoast-0.3.0/hypercoast/emit.py` & `hypercoast-0.3.1/hypercoast/emit.py`

 * *Files identical despite different names*

### Comparing `hypercoast-0.3.0/hypercoast/hypercoast.py` & `hypercoast-0.3.1/hypercoast/hypercoast.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import ipyleaflet
 import leafmap
 import xarray as xr
 import numpy as np
 from .common import download_file, netcdf_groups
 from .emit import read_emit, plot_emit, viz_emit, emit_to_netcdf, emit_to_image
 from .pace import *
+from .ui import SpectralWidget
 
 
 class Map(leafmap.Map):
     """
     A class that extends leafmap.Map to provide additional functionality for hypercoast.
 
     Attributes:
@@ -34,15 +35,14 @@
 
         Args:
             **kwargs: Arbitrary keyword arguments that are passed to the parent class's add_layer method.
         """
 
         if isinstance(obj, str):
             if obj == "spectral":
-                from .ui import SpectralWidget
 
                 SpectralWidget(self, position=position)
                 self.set_plot_options(add_marker_cluster=True)
             else:
                 super().add(obj, **kwargs)
 
         else:
```

### Comparing `hypercoast-0.3.0/hypercoast/pace.py` & `hypercoast-0.3.1/hypercoast/pace.py`

 * *Files 1% similar despite different names*

```diff
@@ -294,15 +294,15 @@
 
     grid_lat = np.linspace(lat.min(), lat.max(), lat.shape[0])
     grid_lon = np.linspace(lon.min(), lon.max(), lon.shape[1])
     grid_lon_2d, grid_lat_2d = np.meshgrid(grid_lon, grid_lat)
 
     gridded_data_dict = {}
     for wavelength in wavelengths:
-        data = dataset.sel(wavelength=wavelength)["Rrs"]
+        data = dataset.sel(wavelength=wavelength, method=method)["Rrs"]
         gridded_data = griddata(
             (lat.data.flatten(), lon.data.flatten()),
             data.data.flatten(),
             (grid_lat_2d, grid_lon_2d),
             method=method,
         )
         gridded_data_dict[wavelength] = gridded_data
```

### Comparing `hypercoast-0.3.0/hypercoast/ui.py` & `hypercoast-0.3.1/hypercoast/ui.py`

 * *Files identical despite different names*

### Comparing `hypercoast-0.3.0/mkdocs.yml` & `hypercoast-0.3.1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `hypercoast-0.3.0/pyproject.toml` & `hypercoast-0.3.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "HyperCoast"
-version = "0.3.0"
+version = "0.3.1"
 dynamic = [
     "dependencies",
 ]
 description = "A Python package for processing hyperspectral data in coastal regions"
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = [
@@ -48,15 +48,15 @@
 
 
 [tool.distutils.bdist_wheel]
 universal = true
 
 
 [tool.bumpversion]
-current_version = "0.3.0"
+current_version = "0.3.1"
 commit = true
 tag = true
 
 [[tool.bumpversion.files]]
 filename = "pyproject.toml"
 search = 'version = "{current_version}"'
 replace = 'version = "{new_version}"'
```

