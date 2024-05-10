# Comparing `tmp/ape-alchemy-0.7.1.tar.gz` & `tmp/ape-alchemy-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ape-alchemy-0.7.1.tar", last modified: Thu Jan 25 18:23:13 2024, max compression
+gzip compressed data, was "ape-alchemy-0.7.2.tar", last modified: Thu Apr 25 20:27:16 2024, max compression
```

## Comparing `ape-alchemy-0.7.1.tar` & `ape-alchemy-0.7.2.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 18:23:13.209567 ape-alchemy-0.7.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 18:23:13.205567 ape-alchemy-0.7.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 18:23:13.205567 ape-alchemy-0.7.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-01-25 18:22:12.000000 ape-alchemy-0.7.1/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-01-25 18:22:12.000000 ape-alchemy-0.7.1/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-01-25 18:22:12.000000 ape-alchemy-0.7.1/.github/ISSUE_TEMPLATE/work-item.md
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-01-25 18:22:12.000000 ape-alchemy-0.7.1/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-01-25 18:22:12.000000 ape-alchemy-0.7.1/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 18:23:13.205567 ape-alchemy-0.7.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-01-25 18:22:12.000000 ape-alchemy-0.7.1/.github/workflows/codeql.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-01-25 18:22:12.000000 ape-alchemy-0.7.1/.github/workflows/commitlint.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-01-25 18:22:12.000000 ape-alchemy-0.7.1/.github/workflows/docs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-01-25 18:22:12.000000 ape-alchemy-0.7.1/.github/workflows/draft.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-01-25 18:22:12.000000 ape-alchemy-0.7.1/.github/workflows/prtitle.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-01-25 18:22:12.000000 ape-alchemy-0.7.1/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4116 2024-01-25 18:22:12.000000 ape-alchemy-0.7.1/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-01-25 18:22:12.000000 ape-alchemy-0.7.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-01-25 18:22:12.000000 ape-alchemy-0.7.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-01-25 18:22:12.000000 ape-alchemy-0.7.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-01-25 18:22:12.000000 ape-alchemy-0.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3765 2024-01-25 18:23:13.209567 ape-alchemy-0.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-01-25 18:22:12.000000 ape-alchemy-0.7.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 18:23:13.209567 ape-alchemy-0.7.1/ape_alchemy/
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-01-25 18:22:12.000000 ape-alchemy-0.7.1/ape_alchemy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-01-25 18:22:12.000000 ape-alchemy-0.7.1/ape_alchemy/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    10542 2024-01-25 18:22:12.000000 ape-alchemy-0.7.1/ape_alchemy/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-25 18:22:12.000000 ape-alchemy-0.7.1/ape_alchemy/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-01-25 18:23:12.000000 ape-alchemy-0.7.1/ape_alchemy/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 18:23:13.209567 ape-alchemy-0.7.1/ape_alchemy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3765 2024-01-25 18:23:13.000000 ape-alchemy-0.7.1/ape_alchemy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-01-25 18:23:13.000000 ape-alchemy-0.7.1/ape_alchemy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-25 18:23:13.000000 ape-alchemy-0.7.1/ape_alchemy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-25 18:23:13.000000 ape-alchemy-0.7.1/ape_alchemy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-01-25 18:23:13.000000 ape-alchemy-0.7.1/ape_alchemy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-01-25 18:23:13.000000 ape-alchemy-0.7.1/ape_alchemy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-01-25 18:22:12.000000 ape-alchemy-0.7.1/build_docs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 18:23:13.209567 ape-alchemy-0.7.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 18:23:13.209567 ape-alchemy-0.7.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     3827 2024-01-25 18:22:12.000000 ape-alchemy-0.7.1/docs/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-01-25 18:22:12.000000 ape-alchemy-0.7.1/docs/_static/custom.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 18:23:13.209567 ape-alchemy-0.7.1/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)     9740 2024-01-25 18:22:12.000000 ape-alchemy-0.7.1/docs/_templates/layout.html
--rw-r--r--   0 runner    (1001) docker     (127)     3383 2024-01-25 18:22:12.000000 ape-alchemy-0.7.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)    20915 2024-01-25 18:22:12.000000 ape-alchemy-0.7.1/docs/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-01-25 18:22:12.000000 ape-alchemy-0.7.1/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)    11889 2024-01-25 18:22:12.000000 ape-alchemy-0.7.1/docs/logo.gif
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 18:23:13.209567 ape-alchemy-0.7.1/docs/methoddocs/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-01-25 18:22:12.000000 ape-alchemy-0.7.1/docs/methoddocs/exceptions.md
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-01-25 18:22:12.000000 ape-alchemy-0.7.1/docs/methoddocs/providers.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 18:23:13.209567 ape-alchemy-0.7.1/docs/userguides/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-01-25 18:22:12.000000 ape-alchemy-0.7.1/docs/userguides/quickstart.md
--rw-r--r--   0 runner    (1001) docker     (127)      990 2024-01-25 18:22:12.000000 ape-alchemy-0.7.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-01-25 18:23:13.209567 ape-alchemy-0.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4245 2024-01-25 18:22:12.000000 ape-alchemy-0.7.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 18:23:13.209567 ape-alchemy-0.7.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-25 18:22:12.000000 ape-alchemy-0.7.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2492 2024-01-25 18:22:12.000000 ape-alchemy-0.7.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-01-25 18:22:12.000000 ape-alchemy-0.7.1/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)     6806 2024-01-25 18:22:12.000000 ape-alchemy-0.7.1/tests/test_providers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:27:16.083819 ape-alchemy-0.7.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:27:16.079819 ape-alchemy-0.7.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:27:16.079819 ape-alchemy-0.7.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-25 20:26:23.000000 ape-alchemy-0.7.2/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-25 20:26:23.000000 ape-alchemy-0.7.2/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-04-25 20:26:23.000000 ape-alchemy-0.7.2/.github/ISSUE_TEMPLATE/work-item.md
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-25 20:26:23.000000 ape-alchemy-0.7.2/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-25 20:26:23.000000 ape-alchemy-0.7.2/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:27:16.079819 ape-alchemy-0.7.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-25 20:26:23.000000 ape-alchemy-0.7.2/.github/workflows/codeql.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-25 20:26:23.000000 ape-alchemy-0.7.2/.github/workflows/commitlint.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-04-25 20:26:23.000000 ape-alchemy-0.7.2/.github/workflows/docs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-25 20:26:23.000000 ape-alchemy-0.7.2/.github/workflows/draft.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-25 20:26:23.000000 ape-alchemy-0.7.2/.github/workflows/prtitle.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-25 20:26:23.000000 ape-alchemy-0.7.2/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3712 2024-04-25 20:26:23.000000 ape-alchemy-0.7.2/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-25 20:26:23.000000 ape-alchemy-0.7.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-25 20:26:23.000000 ape-alchemy-0.7.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-04-25 20:26:23.000000 ape-alchemy-0.7.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-04-25 20:26:23.000000 ape-alchemy-0.7.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3766 2024-04-25 20:27:16.083819 ape-alchemy-0.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2799 2024-04-25 20:26:23.000000 ape-alchemy-0.7.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:27:16.079819 ape-alchemy-0.7.2/ape_alchemy/
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-25 20:26:23.000000 ape-alchemy-0.7.2/ape_alchemy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-25 20:26:23.000000 ape-alchemy-0.7.2/ape_alchemy/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10465 2024-04-25 20:26:23.000000 ape-alchemy-0.7.2/ape_alchemy/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 20:26:23.000000 ape-alchemy-0.7.2/ape_alchemy/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-25 20:27:15.000000 ape-alchemy-0.7.2/ape_alchemy/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:27:16.083819 ape-alchemy-0.7.2/ape_alchemy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3766 2024-04-25 20:27:15.000000 ape-alchemy-0.7.2/ape_alchemy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-25 20:27:16.000000 ape-alchemy-0.7.2/ape_alchemy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 20:27:15.000000 ape-alchemy-0.7.2/ape_alchemy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 20:27:15.000000 ape-alchemy-0.7.2/ape_alchemy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-04-25 20:27:15.000000 ape-alchemy-0.7.2/ape_alchemy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-25 20:27:15.000000 ape-alchemy-0.7.2/ape_alchemy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-04-25 20:26:23.000000 ape-alchemy-0.7.2/build_docs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:27:16.083819 ape-alchemy-0.7.2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:27:16.083819 ape-alchemy-0.7.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     3827 2024-04-25 20:26:23.000000 ape-alchemy-0.7.2/docs/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-25 20:26:23.000000 ape-alchemy-0.7.2/docs/_static/custom.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:27:16.083819 ape-alchemy-0.7.2/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     9740 2024-04-25 20:26:23.000000 ape-alchemy-0.7.2/docs/_templates/layout.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3383 2024-04-25 20:26:23.000000 ape-alchemy-0.7.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20915 2024-04-25 20:26:23.000000 ape-alchemy-0.7.2/docs/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-25 20:26:23.000000 ape-alchemy-0.7.2/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11889 2024-04-25 20:26:23.000000 ape-alchemy-0.7.2/docs/logo.gif
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:27:16.083819 ape-alchemy-0.7.2/docs/methoddocs/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-25 20:26:23.000000 ape-alchemy-0.7.2/docs/methoddocs/exceptions.md
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-25 20:26:23.000000 ape-alchemy-0.7.2/docs/methoddocs/providers.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:27:16.083819 ape-alchemy-0.7.2/docs/userguides/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-25 20:26:23.000000 ape-alchemy-0.7.2/docs/userguides/quickstart.md
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-04-25 20:26:23.000000 ape-alchemy-0.7.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-25 20:27:16.083819 ape-alchemy-0.7.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4244 2024-04-25 20:26:23.000000 ape-alchemy-0.7.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:27:16.083819 ape-alchemy-0.7.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 20:26:23.000000 ape-alchemy-0.7.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-04-25 20:26:23.000000 ape-alchemy-0.7.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-04-25 20:26:23.000000 ape-alchemy-0.7.2/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6808 2024-04-25 20:26:23.000000 ape-alchemy-0.7.2/tests/test_providers.py
```

### Comparing `ape-alchemy-0.7.1/.github/ISSUE_TEMPLATE/bug.md` & `ape-alchemy-0.7.2/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `ape-alchemy-0.7.1/.github/ISSUE_TEMPLATE/feature.md` & `ape-alchemy-0.7.2/.github/ISSUE_TEMPLATE/feature.md`

 * *Files identical despite different names*

### Comparing `ape-alchemy-0.7.1/.github/ISSUE_TEMPLATE/work-item.md` & `ape-alchemy-0.7.2/.github/ISSUE_TEMPLATE/work-item.md`

 * *Files identical despite different names*

### Comparing `ape-alchemy-0.7.1/.github/release-drafter.yml` & `ape-alchemy-0.7.2/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `ape-alchemy-0.7.1/.github/workflows/codeql.yaml` & `ape-alchemy-0.7.2/.github/workflows/codeql.yaml`

 * *Files identical despite different names*

### Comparing `ape-alchemy-0.7.1/.github/workflows/commitlint.yaml` & `ape-alchemy-0.7.2/.github/workflows/commitlint.yaml`

 * *Files identical despite different names*

### Comparing `ape-alchemy-0.7.1/.github/workflows/docs.yaml` & `ape-alchemy-0.7.2/.github/workflows/docs.yaml`

 * *Files 26% similar despite different names*

```diff
@@ -1,57 +1,59 @@
-name: Docs
-
-on:
-    push:
-        branches: [main]
-    release:
-        types: [released]
-    pull_request:
-        types: [opened, synchronize]
-
-jobs:
-    docs:
-        runs-on: ubuntu-latest
-
-        steps:
-        - uses: actions/checkout@v3
-
-        - name: Setup Python
-          uses: actions/setup-python@v4
-          with:
-              python-version: "3.10"
-
-        - name: Install Dependencies
-          run: |
-            python -m pip install --upgrade pip
-            pip install .[doc]
-
-        - name: Build HTML artifact
-          run: python build_docs.py
-
-        - name: Upload HTML artifact
-          uses: actions/upload-artifact@v1
-          with:
-              name: DocumentationHTML
-              path: docs/_build/ape-alchemy
-
-        - name: Commit and publish documentation changes to gh-pages branch
-          run: |
-              if [[ "${GITHUB_EVENT_NAME}" =~ "pull_request" ]]; then
-                echo "skipping 'git commit' step for PR"
-              else
-                git clone https://github.com/${GITHUB_REPOSITORY} --branch gh-pages --single-branch gh-pages
-                cp -r docs/_build/ape-alchemy/* gh-pages/
-                cd gh-pages
-                touch .nojekyll
-                git config --local user.email "action@github.com"
-                git config --local user.name "GitHub Action"
-                git add .
-                git commit -m "Update documentation" -a || true
-              fi
-        - name: Push changes
-          uses: ad-m/github-push-action@master
-          if: ${{ github.event_name != 'pull_request' }}
-          with:
-              branch: gh-pages
-              directory: gh-pages
-              github_token: ${{ secrets.GITHUB_TOKEN }}
+name: Docs
+
+on:
+    push:
+        branches: [main]
+    release:
+        types: [released]
+    pull_request:
+        types: [opened, synchronize]
+
+jobs:
+    docs:
+        runs-on: ubuntu-latest
+        permissions:
+          contents: write
+
+        steps:
+        - uses: actions/checkout@v3
+
+        - name: Setup Python
+          uses: actions/setup-python@v4
+          with:
+              python-version: "3.10"
+
+        - name: Install Dependencies
+          run: |
+            python -m pip install --upgrade pip
+            pip install .[doc]
+
+        - name: Build HTML artifact
+          run: python build_docs.py
+
+        - name: Upload HTML artifact
+          uses: actions/upload-artifact@v1
+          with:
+              name: DocumentationHTML
+              path: docs/_build/ape-alchemy
+
+        - name: Commit and publish documentation changes to gh-pages branch
+          run: |
+              if [[ "${GITHUB_EVENT_NAME}" =~ "pull_request" ]]; then
+                echo "skipping 'git commit' step for PR"
+              else
+                git clone https://github.com/${GITHUB_REPOSITORY} --branch gh-pages --single-branch gh-pages
+                cp -r docs/_build/ape-alchemy/* gh-pages/
+                cd gh-pages
+                touch .nojekyll
+                git config --local user.email "action@github.com"
+                git config --local user.name "GitHub Action"
+                git add .
+                git commit -m "Update documentation" -a || true
+              fi
+        - name: Push changes
+          uses: ad-m/github-push-action@master
+          if: ${{ github.event_name != 'pull_request' }}
+          with:
+              branch: gh-pages
+              directory: gh-pages
+              github_token: ${{ secrets.GITHUB_TOKEN }}
```

### Comparing `ape-alchemy-0.7.1/.github/workflows/prtitle.yaml` & `ape-alchemy-0.7.2/.github/workflows/prtitle.yaml`

 * *Files identical despite different names*

### Comparing `ape-alchemy-0.7.1/.github/workflows/publish.yaml` & `ape-alchemy-0.7.2/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `ape-alchemy-0.7.1/.github/workflows/test.yaml` & `ape-alchemy-0.7.2/.github/workflows/test.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -83,27 +83,23 @@
             python -m pip install --upgrade pip
             pip install .[test]
 
         - name: Run Tests
           run: pytest -m "not fuzzing" -s --cov=src -n auto
           env:
             WEB3_ETHEREUM_MAINNET_ALCHEMY_API_KEY: ${{ secrets.WEB3_ETHEREUM_MAINNET_ALCHEMY_API_KEY }}
-            WEB3_ETHEREUM_GOERLI_ALCHEMY_API_KEY: ${{ secrets.WEB3_ETHEREUM_GOERLI_ALCHEMY_API_KEY }}
             WEB3_ETHEREUM_SEPOLIA_ALCHEMY_API_KEY: ${{ secrets.WEB3_ETHEREUM_SEPOLIA_ALCHEMY_API_KEY }}
             WEB3_ARBITRUM_MAINNET_ALCHEMY_API_KEY: ${{ secrets.WEB3_ARBITRUM_MAINNET_ALCHEMY_API_KEY }}
-            WEB3_ARBITRUM_GOERLI_ALCHEMY_API_KEY: ${{ secrets.WEB3_ARBITRUM_GOERLI_ALCHEMY_API_KEY }}
             WEB3_ARBITRUM_SEPOLIA_ALCHEMY_API_KEY: ${{ secrets.WEB3_ARBITRUM_SEPOLIA_ALCHEMY_API_KEY }}
             WEB3_BASE_MAINNET_ALCHEMY_API_KEY: ${{ secrets.WEB3_BASE_MAINNET_ALCHEMY_API_KEY }}
-            WEB3_BASE_GOERLI_ALCHEMY_API_KEY: ${{ secrets.WEB3_BASE_GOERLI_ALCHEMY_API_KEY }}
             WEB3_BASE_SEPOLIA_ALCHEMY_API_KEY: ${{ secrets.WEB3_BASE_SEPOLIA_ALCHEMY_API_KEY }}
             WEB3_OPTIMISM_MAINNET_ALCHEMY_API_KEY: ${{ secrets.WEB3_OPTIMISM_MAINNET_ALCHEMY_API_KEY }}
-            WEB3_OPTIMISM_GOERLI_ALCHEMY_API_KEY: ${{ secrets.WEB3_OPTIMISM_GOERLI_ALCHEMY_API_KEY }}
             WEB3_OPTIMISM_SEPOLIA_ALCHEMY_API_KEY: ${{ secrets.WEB3_OPTIMISM_SEPOLIA_ALCHEMY_API_KEY }}
             WEB3_POLYGON_MAINNET_ALCHEMY_API_KEY: ${{ secrets.WEB3_POLYGON_MAINNET_ALCHEMY_API_KEY }}
-            WEB3_POLYGON_MUMBAI_ALCHEMY_API_KEY: ${{ secrets.WEB3_POLYGON_MUMBAI_ALCHEMY_API_KEY }}
+            WEB3_POLYGON_AMOY_ALCHEMY_API_KEY: ${{ secrets.WEB3_POLYGON_AMOY_ALCHEMY_API_KEY }}
 
 # NOTE: uncomment this block after you've marked tests with @pytest.mark.fuzzing
 #    fuzzing:
 #        runs-on: ubuntu-latest
 #
 #        strategy:
 #            fail-fast: true
```

### Comparing `ape-alchemy-0.7.1/.gitignore` & `ape-alchemy-0.7.2/.gitignore`

 * *Files identical despite different names*

### Comparing `ape-alchemy-0.7.1/.pre-commit-config.yaml` & `ape-alchemy-0.7.2/.pre-commit-config.yaml`

 * *Files 13% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 repos:
 -   repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.5.0
+    rev: v4.6.0
     hooks:
     -   id: check-yaml
 
 -   repo: https://github.com/pre-commit/mirrors-isort
     rev: v5.10.1
     hooks:
       - id: isort
 
 -   repo: https://github.com/psf/black
-    rev: 23.12.0
+    rev: 24.3.0
     hooks:
       - id: black
         name: black
 
 -   repo: https://github.com/pycqa/flake8
-    rev: 6.1.0
+    rev: 7.0.0
     hooks:
     -   id: flake8
 
 -   repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v1.7.1
+    rev: v1.9.0
     hooks:
     -   id: mypy
         additional_dependencies: [types-PyYAML, types-requests, pydantic, types-setuptools]
 
 -   repo: https://github.com/executablebooks/mdformat
     rev: 0.7.17
     hooks:
```

### Comparing `ape-alchemy-0.7.1/CONTRIBUTING.md` & `ape-alchemy-0.7.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ape-alchemy-0.7.1/LICENSE` & `ape-alchemy-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ape-alchemy-0.7.1/PKG-INFO` & `ape-alchemy-0.7.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ape-alchemy
-Version: 0.7.1
+Version: 0.7.2
 Summary: ape-alchemy: Alchemy provider plugins
 Home-page: https://github.com/ApeWorX/ape-alchemy
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Keywords: ethereum
 Classifier: Development Status :: 5 - Production/Stable
@@ -84,15 +84,15 @@
 ```bash
 export WEB3_ALCHEMY_PROJECT_ID=MY_API_TOKEN=<value-of-secret-key>
 ```
 
 To use the Alchemy provider plugin in most commands, set it via the `--network` option:
 
 ```bash
-ape console --network ethereum:goerli:alchemy
+ape console --network ethereum:sepolia:alchemy
 ```
 
 To connect to Alchemy from a Python script, use the `networks` top-level manager:
 
 ```python
 from ape import networks
```

### Comparing `ape-alchemy-0.7.1/README.md` & `ape-alchemy-0.7.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 ```bash
 export WEB3_ALCHEMY_PROJECT_ID=MY_API_TOKEN=<value-of-secret-key>
 ```
 
 To use the Alchemy provider plugin in most commands, set it via the `--network` option:
 
 ```bash
-ape console --network ethereum:goerli:alchemy
+ape console --network ethereum:sepolia:alchemy
 ```
 
 To connect to Alchemy from a Python script, use the `networks` top-level manager:
 
 ```python
 from ape import networks
```

### Comparing `ape-alchemy-0.7.1/ape_alchemy/exceptions.py` & `ape-alchemy-0.7.2/ape_alchemy/exceptions.py`

 * *Files identical despite different names*

### Comparing `ape-alchemy-0.7.1/ape_alchemy/provider.py` & `ape-alchemy-0.7.2/ape_alchemy/provider.py`

 * *Files 5% similar despite different names*

```diff
@@ -98,20 +98,19 @@
     def connection_str(self) -> str:
         return self.uri
 
     def connect(self):
         self._web3 = Web3(HTTPProvider(self.uri))
         try:
             # Any chain that *began* as PoA needs the middleware for pre-merge blocks
-            ethereum_goerli = 5
-            base = (8453, 84531)
-            optimism = (10, 420)
-            polygon = (137, 80001)
+            base = 8453
+            optimism = 10
+            polygon = 137
 
-            if self._web3.eth.chain_id in (ethereum_goerli, *base, *optimism, *polygon):
+            if self._web3.eth.chain_id in (base, optimism, polygon):
                 self._web3.middleware_onion.inject(geth_poa_middleware, layer=0)
 
             self._web3.eth.set_gas_price_strategy(rpc_gas_price_strategy)
         except Exception as err:
             raise ProviderError(f"Failed to connect to Alchemy.\n{repr(err)}") from err
 
     def disconnect(self):
```

### Comparing `ape-alchemy-0.7.1/ape_alchemy.egg-info/PKG-INFO` & `ape-alchemy-0.7.2/ape_alchemy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ape-alchemy
-Version: 0.7.1
+Version: 0.7.2
 Summary: ape-alchemy: Alchemy provider plugins
 Home-page: https://github.com/ApeWorX/ape-alchemy
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Keywords: ethereum
 Classifier: Development Status :: 5 - Production/Stable
@@ -84,15 +84,15 @@
 ```bash
 export WEB3_ALCHEMY_PROJECT_ID=MY_API_TOKEN=<value-of-secret-key>
 ```
 
 To use the Alchemy provider plugin in most commands, set it via the `--network` option:
 
 ```bash
-ape console --network ethereum:goerli:alchemy
+ape console --network ethereum:sepolia:alchemy
 ```
 
 To connect to Alchemy from a Python script, use the `networks` top-level manager:
 
 ```python
 from ape import networks
```

### Comparing `ape-alchemy-0.7.1/ape_alchemy.egg-info/SOURCES.txt` & `ape-alchemy-0.7.2/ape_alchemy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ape-alchemy-0.7.1/ape_alchemy.egg-info/requires.txt` & `ape-alchemy-0.7.2/ape_alchemy.egg-info/requires.txt`

 * *Files 6% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 ape-polygon
 pytest>=6.0
 pytest-xdist
 pytest-cov
 pytest-mock
 hypothesis<7.0,>=6.2.0
 websocket-client
-black<24,>=23.12.0
-mypy<2,>=1.7.1
+black<25,>=24.3.0
+mypy<2,>=1.9.0
 types-setuptools
 types-requests
-flake8<7,>=6.1.0
+flake8<8,>=7.0.0
 flake8-breakpoint<2,>=1.1.0
 flake8-print<6,>=5.0.0
 isort<6,>=5.10.1
 mdformat>=0.7.17
 mdformat-gfm>=0.3.5
 mdformat-frontmatter>=0.4.1
 mdformat-pyproject>=0.0.1
@@ -48,19 +48,19 @@
 sphinx-click<5,>=4.4.0
 Sphinx<7,>=6.1.3
 sphinx_rtd_theme<2,>=1.2.0
 sphinxcontrib-napoleon>=0.7
 sphinx-plausible<0.2,>=0.1.2
 
 [lint]
-black<24,>=23.12.0
-mypy<2,>=1.7.1
+black<25,>=24.3.0
+mypy<2,>=1.9.0
 types-setuptools
 types-requests
-flake8<7,>=6.1.0
+flake8<8,>=7.0.0
 flake8-breakpoint<2,>=1.1.0
 flake8-print<6,>=5.0.0
 isort<6,>=5.10.1
 mdformat>=0.7.17
 mdformat-gfm>=0.3.5
 mdformat-frontmatter>=0.4.1
 mdformat-pyproject>=0.0.1
```

### Comparing `ape-alchemy-0.7.1/build_docs.py` & `ape-alchemy-0.7.2/build_docs.py`

 * *Files identical despite different names*

### Comparing `ape-alchemy-0.7.1/docs/_static/custom.css` & `ape-alchemy-0.7.2/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `ape-alchemy-0.7.1/docs/_static/custom.js` & `ape-alchemy-0.7.2/docs/_static/custom.js`

 * *Files identical despite different names*

### Comparing `ape-alchemy-0.7.1/docs/_templates/layout.html` & `ape-alchemy-0.7.2/docs/_templates/layout.html`

 * *Files identical despite different names*

### Comparing `ape-alchemy-0.7.1/docs/conf.py` & `ape-alchemy-0.7.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ape-alchemy-0.7.1/docs/favicon.ico` & `ape-alchemy-0.7.2/docs/favicon.ico`

 * *Files identical despite different names*

### Comparing `ape-alchemy-0.7.1/docs/logo.gif` & `ape-alchemy-0.7.2/docs/logo.gif`

 * *Files identical despite different names*

### Comparing `ape-alchemy-0.7.1/pyproject.toml` & `ape-alchemy-0.7.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ape-alchemy-0.7.1/setup.py` & `ape-alchemy-0.7.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,19 +12,19 @@
         "pytest-xdist",  # Multi-process runner
         "pytest-cov",  # Coverage analyzer plugin
         "pytest-mock",  # For creating mocks
         "hypothesis>=6.2.0,<7.0",  # Strategy-based fuzzer
         "websocket-client",  # Used for web socket integration testing
     ],
     "lint": [
-        "black>=23.12.0,<24",  # Auto-formatter and linter
-        "mypy>=1.7.1,<2",  # Static type analyzer
+        "black>=24.3.0,<25",  # Auto-formatter and linter
+        "mypy>=1.9.0,<2",  # Static type analyzer
         "types-setuptools",  # Needed for mypy type shed
         "types-requests",  # Needed for mypy type shed
-        "flake8>=6.1.0,<7",  # Style linter
+        "flake8>=7.0.0,<8",  # Style linter
         "flake8-breakpoint>=1.1.0,<2",  # Detect breakpoints left in code
         "flake8-print>=5.0.0,<6",  # Detect print statements left in code
         "isort>=5.10.1,<6",  # Import sorting linter
         "mdformat>=0.7.17",  # Auto-formatter for markdown
         "mdformat-gfm>=0.3.5",  # Needed for formatting GitHub-flavored markdown
         "mdformat-frontmatter>=0.4.1",  # Needed for frontmatters-style headers in issue templates
         "mdformat-pyproject>=0.0.1",  # Allows configuring in pyproject.toml
```

### Comparing `ape-alchemy-0.7.1/tests/conftest.py` & `ape-alchemy-0.7.2/tests/conftest.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 FEATURE_NOT_AVAILABLE_BECAUSE_OF_TIER_RESPONSE = (
     "trace_transaction is not available on the Free tier - "
     "upgrade to Growth or Enterprise for access. See available methods at "
     "https://docs.alchemy.com/alchemy/documentation/apis"
 )
 FEATURE_NOT_AVAILABLE_BECAUSE_OF_NETWORK_RESPONSE = (
-    "trace_transaction is not available on the ETH_GOERLI. "
+    "trace_transaction is not available on the ETH_SEPOLIA. "
     "For more information see our docs: "
     "https://docs.alchemy.com/alchemy/documentation/apis/ethereum"
 )
 
 
 @pytest.fixture
 def accounts():
@@ -88,8 +88,8 @@
     response.json.return_value = {"error": {"message": request.param}}
     error = HTTPError(response=response)
     return error
 
 
 @pytest.fixture
 def alchemy_provider(networks) -> Alchemy:
-    return networks.ethereum.goerli.get_provider("alchemy")
+    return networks.ethereum.sepolia.get_provider("alchemy")
```

### Comparing `ape-alchemy-0.7.1/tests/test_integration.py` & `ape-alchemy-0.7.2/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `ape-alchemy-0.7.1/tests/test_providers.py` & `ape-alchemy-0.7.2/tests/test_providers.py`

 * *Files 5% similar despite different names*

```diff
@@ -111,16 +111,16 @@
 def test_when_no_api_key_raises_error(missing_token, alchemy_provider):
     with pytest.raises(
         MissingProjectKeyError,
         match=re.escape(
             "Must set one of "
             "$WEB3_ALCHEMY_PROJECT_ID, "
             "$WEB3_ALCHEMY_API_KEY, "
-            "$WEB3_ETHEREUM_GOERLI_ALCHEMY_PROJECT_ID, "
-            "$WEB3_ETHEREUM_GOERLI_ALCHEMY_API_KEY."
+            "$WEB3_ETHEREUM_SEPOLIA_ALCHEMY_PROJECT_ID, "
+            "$WEB3_ETHEREUM_SEPOLIA_ALCHEMY_API_KEY."
         ),
     ):
         alchemy_provider.connect()
 
 
 def test_send_transaction_reverts(token, alchemy_provider, mock_web3, transaction):
     expected_revert_message = "EXPECTED REVERT MESSAGE"
```

