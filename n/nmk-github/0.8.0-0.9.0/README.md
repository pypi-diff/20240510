# Comparing `tmp/nmk-github-0.8.0.tar.gz` & `tmp/nmk-github-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nmk-github-0.8.0.tar", last modified: Sat Jan 14 15:10:20 2023, max compression
+gzip compressed data, was "nmk-github-0.9.0.tar", last modified: Sun Jan 15 10:51:23 2023, max compression
```

## Comparing `nmk-github-0.8.0.tar` & `nmk-github-0.9.0.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-14 15:10:20.124858 nmk-github-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-01-14 15:09:56.000000 nmk-github-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-01-14 15:10:20.124858 nmk-github-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-01-14 15:10:19.000000 nmk-github-0.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-01-14 15:10:20.124858 nmk-github-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-01-14 15:10:19.000000 nmk-github-0.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-14 15:10:20.124858 nmk-github-0.8.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-14 15:10:20.124858 nmk-github-0.8.0/src/nmk_github/
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-01-14 15:09:56.000000 nmk-github-0.8.0/src/nmk_github/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-01-14 15:09:56.000000 nmk-github-0.8.0/src/nmk_github/action.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-01-14 15:09:56.000000 nmk-github-0.8.0/src/nmk_github/action.yml
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-01-14 15:09:56.000000 nmk-github-0.8.0/src/nmk_github/badges.yml
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-01-14 15:09:56.000000 nmk-github-0.8.0/src/nmk_github/plugin-defs.yml
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-01-14 15:09:56.000000 nmk-github-0.8.0/src/nmk_github/plugin.yml
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-01-14 15:09:56.000000 nmk-github-0.8.0/src/nmk_github/python.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-14 15:10:20.124858 nmk-github-0.8.0/src/nmk_github/templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-14 15:09:56.000000 nmk-github-0.8.0/src/nmk_github/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-01-14 15:09:56.000000 nmk-github-0.8.0/src/nmk_github/templates/build.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-14 15:10:20.124858 nmk-github-0.8.0/src/nmk_github.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-01-14 15:10:20.000000 nmk-github-0.8.0/src/nmk_github.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-01-14 15:10:20.000000 nmk-github-0.8.0/src/nmk_github.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-14 15:10:20.000000 nmk-github-0.8.0/src/nmk_github.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-01-14 15:10:20.000000 nmk-github-0.8.0/src/nmk_github.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-01-14 15:10:20.000000 nmk-github-0.8.0/src/nmk_github.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-15 10:51:23.433702 nmk-github-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-01-15 10:50:58.000000 nmk-github-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-01-15 10:51:23.433702 nmk-github-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-01-15 10:51:22.000000 nmk-github-0.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-01-15 10:51:23.433702 nmk-github-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-01-15 10:51:22.000000 nmk-github-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-15 10:51:23.433702 nmk-github-0.9.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-15 10:51:23.433702 nmk-github-0.9.0/src/nmk_github/
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-01-15 10:50:58.000000 nmk-github-0.9.0/src/nmk_github/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-01-15 10:50:58.000000 nmk-github-0.9.0/src/nmk_github/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-01-15 10:50:58.000000 nmk-github-0.9.0/src/nmk_github/action.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-01-15 10:50:58.000000 nmk-github-0.9.0/src/nmk_github/badges.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-01-15 10:50:58.000000 nmk-github-0.9.0/src/nmk_github/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-01-15 10:50:58.000000 nmk-github-0.9.0/src/nmk_github/plugin-defs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-01-15 10:50:58.000000 nmk-github-0.9.0/src/nmk_github/plugin.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-01-15 10:50:58.000000 nmk-github-0.9.0/src/nmk_github/python.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-15 10:51:23.433702 nmk-github-0.9.0/src/nmk_github/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-15 10:50:58.000000 nmk-github-0.9.0/src/nmk_github/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-01-15 10:50:58.000000 nmk-github-0.9.0/src/nmk_github/templates/build.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-15 10:51:23.433702 nmk-github-0.9.0/src/nmk_github.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-01-15 10:51:23.000000 nmk-github-0.9.0/src/nmk_github.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-01-15 10:51:23.000000 nmk-github-0.9.0/src/nmk_github.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-15 10:51:23.000000 nmk-github-0.9.0/src/nmk_github.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-01-15 10:51:23.000000 nmk-github-0.9.0/src/nmk_github.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-01-15 10:51:23.000000 nmk-github-0.9.0/src/nmk_github.egg-info/top_level.txt
```

### Comparing `nmk-github-0.8.0/LICENSE` & `nmk-github-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nmk-github-0.8.0/PKG-INFO` & `nmk-github-0.9.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,35 @@
 Metadata-Version: 2.1
 Name: nmk-github
-Version: 0.8.0
+Version: 0.9.0
 Summary: Github plugin for nmk build system
 Home-page: https://github.com/dynod/nmk-github
 Author: The dynod project
 Maintainer: The dynod project
 License: Mozilla Public License Version 2.0
 Description: # nmk-github
         Github plugin for **`nmk`** build system
         
         <!-- NMK-BADGES-BEGIN -->
         [![License: MPL](https://img.shields.io/github/license/dynod/nmk-github)](https://github.com/dynod/nmk-github/blob/main/LICENSE)
         [![Checks](https://img.shields.io/github/actions/workflow/status/dynod/nmk-github/build.yml?branch=main&label=build%20%26%20u.t.)](https://github.com/dynod/nmk-github/actions?query=branch%3Amain)
+        [![Issues](https://img.shields.io/github/issues-search/dynod/nmk?label=issues&query=is%3Aopen+is%3Aissue+label%3Aplugin%3Agithub)](https://github.com/dynod/nmk/issues?q=is%3Aopen+is%3Aissue+label%3Aplugin%3Agithub)
         [![Supported python versions](https://img.shields.io/badge/python-3.8%20--%203.11-blue)](https://www.python.org/)
         [![PyPI](https://img.shields.io/pypi/v/nmk-github)](https://pypi.org/project/nmk-github/)
         [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+        [![Flake8 analysis result](https://img.shields.io/badge/flake8-0-green)](https://flake8.pycqa.org/)
+        [![Code coverage](https://img.shields.io/codecov/c/github/dynod/nmk-github)](https://app.codecov.io/gh/dynod/nmk-github)
         <!-- NMK-BADGES-END -->
         
         This plugin adds support for Github features in an **`nmk`** project:
         * [Github workflow file](https://docs.github.com/en/actions/using-workflows/workflow-syntax-for-github-actions) generation
-        * README badges generation (link to license + build action status; only if [**`nmk-badges`**](https://github.com/dynod/nmk-badges) plugin is also used)
+        * README badges generation (if [**`nmk-badges`**](https://github.com/dynod/nmk-badges) plugin is also used):
+          * link to license
+          * build action status
+          * opened issues
         
         ## Usage
         
         To use this plugin in your **`nmk`** project, insert this reference:
         ```
         refs:
             - pip://nmk-github!plugin.yml
```

### Comparing `nmk-github-0.8.0/README.md` & `nmk-github-0.9.0/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,27 @@
 # nmk-github
 Github plugin for **`nmk`** build system
 
 <!-- NMK-BADGES-BEGIN -->
 [![License: MPL](https://img.shields.io/github/license/dynod/nmk-github)](https://github.com/dynod/nmk-github/blob/main/LICENSE)
 [![Checks](https://img.shields.io/github/actions/workflow/status/dynod/nmk-github/build.yml?branch=main&label=build%20%26%20u.t.)](https://github.com/dynod/nmk-github/actions?query=branch%3Amain)
+[![Issues](https://img.shields.io/github/issues-search/dynod/nmk?label=issues&query=is%3Aopen+is%3Aissue+label%3Aplugin%3Agithub)](https://github.com/dynod/nmk/issues?q=is%3Aopen+is%3Aissue+label%3Aplugin%3Agithub)
 [![Supported python versions](https://img.shields.io/badge/python-3.8%20--%203.11-blue)](https://www.python.org/)
 [![PyPI](https://img.shields.io/pypi/v/nmk-github)](https://pypi.org/project/nmk-github/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Flake8 analysis result](https://img.shields.io/badge/flake8-0-green)](https://flake8.pycqa.org/)
+[![Code coverage](https://img.shields.io/codecov/c/github/dynod/nmk-github)](https://app.codecov.io/gh/dynod/nmk-github)
 <!-- NMK-BADGES-END -->
 
 This plugin adds support for Github features in an **`nmk`** project:
 * [Github workflow file](https://docs.github.com/en/actions/using-workflows/workflow-syntax-for-github-actions) generation
-* README badges generation (link to license + build action status; only if [**`nmk-badges`**](https://github.com/dynod/nmk-badges) plugin is also used)
+* README badges generation (if [**`nmk-badges`**](https://github.com/dynod/nmk-badges) plugin is also used):
+  * link to license
+  * build action status
+  * opened issues
 
 ## Usage
 
 To use this plugin in your **`nmk`** project, insert this reference:
 ```
 refs:
     - pip://nmk-github!plugin.yml
```

### Comparing `nmk-github-0.8.0/setup.cfg` & `nmk-github-0.9.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 ignore = E203,E501,B902,W503
 jobs = auto
 exclude = 
 	__pycache__
 
 [metadata]
 name = nmk-github
-version = 0.8.0
+version = 0.9.0
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = Mozilla Public License Version 2.0
 classifiers = 
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
```

### Comparing `nmk-github-0.8.0/src/nmk_github/__init__.py` & `nmk-github-0.9.0/src/nmk_github/__init__.py`

 * *Files identical despite different names*

### Comparing `nmk-github-0.8.0/src/nmk_github/action.py` & `nmk-github-0.9.0/src/nmk_github/action.py`

 * *Files identical despite different names*

### Comparing `nmk-github-0.8.0/src/nmk_github/action.yml` & `nmk-github-0.9.0/src/nmk_github/action.yml`

 * *Files 19% similar despite different names*

```diff
@@ -14,14 +14,22 @@
     githubOSImages:
         - ubuntu-latest
         - windows-latest
 
     # Build command for github action
     githubCommand: source loadme.sh nmk tests
 
+    # Github user
+    githubUser:
+        __resolver__: nmk_github.info.GithubUserResolver
+
+    # Github repository
+    githubRepo:
+        __resolver__: nmk_github.info.GithubRepoResolver
+
 tasks:
     # Github action file generation
     gh.actions:
         description: Generate Github action file
         emoji: ":octopus:.:clapper_board:"
         appendToDeps: setup
         input: ${githubActionTemplate}
```

### Comparing `nmk-github-0.8.0/src/nmk_github/templates/build.yml` & `nmk-github-0.9.0/src/nmk_github/templates/build.yml`

 * *Files identical despite different names*

### Comparing `nmk-github-0.8.0/src/nmk_github.egg-info/PKG-INFO` & `nmk-github-0.9.0/src/nmk_github.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,35 @@
 Metadata-Version: 2.1
 Name: nmk-github
-Version: 0.8.0
+Version: 0.9.0
 Summary: Github plugin for nmk build system
 Home-page: https://github.com/dynod/nmk-github
 Author: The dynod project
 Maintainer: The dynod project
 License: Mozilla Public License Version 2.0
 Description: # nmk-github
         Github plugin for **`nmk`** build system
         
         <!-- NMK-BADGES-BEGIN -->
         [![License: MPL](https://img.shields.io/github/license/dynod/nmk-github)](https://github.com/dynod/nmk-github/blob/main/LICENSE)
         [![Checks](https://img.shields.io/github/actions/workflow/status/dynod/nmk-github/build.yml?branch=main&label=build%20%26%20u.t.)](https://github.com/dynod/nmk-github/actions?query=branch%3Amain)
+        [![Issues](https://img.shields.io/github/issues-search/dynod/nmk?label=issues&query=is%3Aopen+is%3Aissue+label%3Aplugin%3Agithub)](https://github.com/dynod/nmk/issues?q=is%3Aopen+is%3Aissue+label%3Aplugin%3Agithub)
         [![Supported python versions](https://img.shields.io/badge/python-3.8%20--%203.11-blue)](https://www.python.org/)
         [![PyPI](https://img.shields.io/pypi/v/nmk-github)](https://pypi.org/project/nmk-github/)
         [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+        [![Flake8 analysis result](https://img.shields.io/badge/flake8-0-green)](https://flake8.pycqa.org/)
+        [![Code coverage](https://img.shields.io/codecov/c/github/dynod/nmk-github)](https://app.codecov.io/gh/dynod/nmk-github)
         <!-- NMK-BADGES-END -->
         
         This plugin adds support for Github features in an **`nmk`** project:
         * [Github workflow file](https://docs.github.com/en/actions/using-workflows/workflow-syntax-for-github-actions) generation
-        * README badges generation (link to license + build action status; only if [**`nmk-badges`**](https://github.com/dynod/nmk-badges) plugin is also used)
+        * README badges generation (if [**`nmk-badges`**](https://github.com/dynod/nmk-badges) plugin is also used):
+          * link to license
+          * build action status
+          * opened issues
         
         ## Usage
         
         To use this plugin in your **`nmk`** project, insert this reference:
         ```
         refs:
             - pip://nmk-github!plugin.yml
```

