# Comparing `tmp/aind_behavior_curriculum_template-0.0.1.tar.gz` & `tmp/aind_behavior_curriculum_template-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aind_behavior_curriculum_template-0.0.1.tar", last modified: Tue May  7 21:36:55 2024, max compression
+gzip compressed data, was "aind_behavior_curriculum_template-0.0.2.tar", last modified: Fri May 10 20:33:30 2024, max compression
```

## Comparing `aind_behavior_curriculum_template-0.0.1.tar` & `aind_behavior_curriculum_template-0.0.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 21:36:55.020510 aind_behavior_curriculum_template-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-07 21:36:44.000000 aind_behavior_curriculum_template-0.0.1/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 21:36:55.012510 aind_behavior_curriculum_template-0.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 21:36:55.016510 aind_behavior_curriculum_template-0.0.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-07 21:36:44.000000 aind_behavior_curriculum_template-0.0.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-07 21:36:44.000000 aind_behavior_curriculum_template-0.0.1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-07 21:36:44.000000 aind_behavior_curriculum_template-0.0.1/.github/ISSUE_TEMPLATE/user-story.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 21:36:55.016510 aind_behavior_curriculum_template-0.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-05-07 21:36:44.000000 aind_behavior_curriculum_template-0.0.1/.github/workflows/init.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4728 2024-05-07 21:36:44.000000 aind_behavior_curriculum_template-0.0.1/.github/workflows/tag_publish_upload.yml
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-07 21:36:44.000000 aind_behavior_curriculum_template-0.0.1/.github/workflows/test_and_lint.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-05-07 21:36:44.000000 aind_behavior_curriculum_template-0.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-07 21:36:44.000000 aind_behavior_curriculum_template-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6441 2024-05-07 21:36:55.020510 aind_behavior_curriculum_template-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5778 2024-05-07 21:36:44.000000 aind_behavior_curriculum_template-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 21:36:55.016510 aind_behavior_curriculum_template-0.0.1/doc_template/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-07 21:36:44.000000 aind_behavior_curriculum_template-0.0.1/doc_template/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-07 21:36:44.000000 aind_behavior_curriculum_template-0.0.1/doc_template/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 21:36:55.016510 aind_behavior_curriculum_template-0.0.1/doc_template/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 21:36:55.016510 aind_behavior_curriculum_template-0.0.1/doc_template/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     8733 2024-05-07 21:36:44.000000 aind_behavior_curriculum_template-0.0.1/doc_template/source/_static/dark-logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)   259838 2024-05-07 21:36:44.000000 aind_behavior_curriculum_template-0.0.1/doc_template/source/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)     8712 2024-05-07 21:36:44.000000 aind_behavior_curriculum_template-0.0.1/doc_template/source/_static/light-logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-05-07 21:36:44.000000 aind_behavior_curriculum_template-0.0.1/doc_template/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-07 21:36:44.000000 aind_behavior_curriculum_template-0.0.1/doc_template/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-05-07 21:36:44.000000 aind_behavior_curriculum_template-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 21:36:55.020510 aind_behavior_curriculum_template-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-07 21:36:44.000000 aind_behavior_curriculum_template-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 21:36:55.012510 aind_behavior_curriculum_template-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 21:36:55.016510 aind_behavior_curriculum_template-0.0.1/src/aind_behavior_curriculum_template/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-07 21:36:44.000000 aind_behavior_curriculum_template-0.0.1/src/aind_behavior_curriculum_template/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-07 21:36:44.000000 aind_behavior_curriculum_template-0.0.1/src/aind_behavior_curriculum_template/upload.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 21:36:55.020510 aind_behavior_curriculum_template-0.0.1/src/aind_behavior_curriculum_template.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6441 2024-05-07 21:36:54.000000 aind_behavior_curriculum_template-0.0.1/src/aind_behavior_curriculum_template.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      949 2024-05-07 21:36:55.000000 aind_behavior_curriculum_template-0.0.1/src/aind_behavior_curriculum_template.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 21:36:54.000000 aind_behavior_curriculum_template-0.0.1/src/aind_behavior_curriculum_template.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-07 21:36:54.000000 aind_behavior_curriculum_template-0.0.1/src/aind_behavior_curriculum_template.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-07 21:36:54.000000 aind_behavior_curriculum_template-0.0.1/src/aind_behavior_curriculum_template.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 21:36:55.020510 aind_behavior_curriculum_template-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-07 21:36:44.000000 aind_behavior_curriculum_template-0.0.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-07 21:36:44.000000 aind_behavior_curriculum_template-0.0.1/tests/test_example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:33:30.791608 aind_behavior_curriculum_template-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-10 20:33:20.000000 aind_behavior_curriculum_template-0.0.2/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:33:30.783609 aind_behavior_curriculum_template-0.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:33:30.783609 aind_behavior_curriculum_template-0.0.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-10 20:33:20.000000 aind_behavior_curriculum_template-0.0.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-10 20:33:20.000000 aind_behavior_curriculum_template-0.0.2/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-10 20:33:20.000000 aind_behavior_curriculum_template-0.0.2/.github/ISSUE_TEMPLATE/user-story.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:33:30.787608 aind_behavior_curriculum_template-0.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-05-10 20:33:20.000000 aind_behavior_curriculum_template-0.0.2/.github/workflows/init.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4728 2024-05-10 20:33:20.000000 aind_behavior_curriculum_template-0.0.2/.github/workflows/tag_publish_upload.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-10 20:33:20.000000 aind_behavior_curriculum_template-0.0.2/.github/workflows/test_and_lint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-05-10 20:33:20.000000 aind_behavior_curriculum_template-0.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-10 20:33:20.000000 aind_behavior_curriculum_template-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6528 2024-05-10 20:33:30.791608 aind_behavior_curriculum_template-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5865 2024-05-10 20:33:20.000000 aind_behavior_curriculum_template-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:33:30.787608 aind_behavior_curriculum_template-0.0.2/doc_template/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-10 20:33:20.000000 aind_behavior_curriculum_template-0.0.2/doc_template/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-10 20:33:20.000000 aind_behavior_curriculum_template-0.0.2/doc_template/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:33:30.787608 aind_behavior_curriculum_template-0.0.2/doc_template/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:33:30.787608 aind_behavior_curriculum_template-0.0.2/doc_template/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     8733 2024-05-10 20:33:20.000000 aind_behavior_curriculum_template-0.0.2/doc_template/source/_static/dark-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   259838 2024-05-10 20:33:20.000000 aind_behavior_curriculum_template-0.0.2/doc_template/source/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     8712 2024-05-10 20:33:20.000000 aind_behavior_curriculum_template-0.0.2/doc_template/source/_static/light-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-05-10 20:33:20.000000 aind_behavior_curriculum_template-0.0.2/doc_template/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-10 20:33:20.000000 aind_behavior_curriculum_template-0.0.2/doc_template/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-05-10 20:33:20.000000 aind_behavior_curriculum_template-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 20:33:30.791608 aind_behavior_curriculum_template-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-10 20:33:20.000000 aind_behavior_curriculum_template-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:33:30.783609 aind_behavior_curriculum_template-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:33:30.787608 aind_behavior_curriculum_template-0.0.2/src/aind_behavior_curriculum_template/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-10 20:33:21.000000 aind_behavior_curriculum_template-0.0.2/src/aind_behavior_curriculum_template/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-10 20:33:20.000000 aind_behavior_curriculum_template-0.0.2/src/aind_behavior_curriculum_template/upload.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:33:30.787608 aind_behavior_curriculum_template-0.0.2/src/aind_behavior_curriculum_template.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6528 2024-05-10 20:33:30.000000 aind_behavior_curriculum_template-0.0.2/src/aind_behavior_curriculum_template.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-05-10 20:33:30.000000 aind_behavior_curriculum_template-0.0.2/src/aind_behavior_curriculum_template.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 20:33:30.000000 aind_behavior_curriculum_template-0.0.2/src/aind_behavior_curriculum_template.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-10 20:33:30.000000 aind_behavior_curriculum_template-0.0.2/src/aind_behavior_curriculum_template.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-10 20:33:30.000000 aind_behavior_curriculum_template-0.0.2/src/aind_behavior_curriculum_template.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:33:30.787608 aind_behavior_curriculum_template-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-10 20:33:20.000000 aind_behavior_curriculum_template-0.0.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-10 20:33:20.000000 aind_behavior_curriculum_template-0.0.2/tests/test_example.py
```

### Comparing `aind_behavior_curriculum_template-0.0.1/.github/ISSUE_TEMPLATE/bug_report.md` & `aind_behavior_curriculum_template-0.0.2/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `aind_behavior_curriculum_template-0.0.1/.github/ISSUE_TEMPLATE/feature_request.md` & `aind_behavior_curriculum_template-0.0.2/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `aind_behavior_curriculum_template-0.0.1/.github/ISSUE_TEMPLATE/user-story.md` & `aind_behavior_curriculum_template-0.0.2/.github/ISSUE_TEMPLATE/user-story.md`

 * *Files identical despite different names*

### Comparing `aind_behavior_curriculum_template-0.0.1/.github/workflows/init.yml` & `aind_behavior_curriculum_template-0.0.2/.github/workflows/init.yml`

 * *Files identical despite different names*

### Comparing `aind_behavior_curriculum_template-0.0.1/.github/workflows/tag_publish_upload.yml` & `aind_behavior_curriculum_template-0.0.2/.github/workflows/tag_publish_upload.yml`

 * *Files identical despite different names*

### Comparing `aind_behavior_curriculum_template-0.0.1/.github/workflows/test_and_lint.yml` & `aind_behavior_curriculum_template-0.0.2/.github/workflows/test_and_lint.yml`

 * *Files identical despite different names*

### Comparing `aind_behavior_curriculum_template-0.0.1/.gitignore` & `aind_behavior_curriculum_template-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `aind_behavior_curriculum_template-0.0.1/LICENSE` & `aind_behavior_curriculum_template-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aind_behavior_curriculum_template-0.0.1/PKG-INFO` & `aind_behavior_curriculum_template-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aind-behavior-curriculum-template
-Version: 0.0.1
+Version: 0.0.2
 Summary: Generated from aind-behavior-curriculum-template
 Author: Allen Institute for Neural Dynamics
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -23,15 +23,16 @@
 [![License](https://img.shields.io/badge/license-MIT-brightgreen)](LICENSE)
 ![Code Style](https://img.shields.io/badge/code%20style-black-black)
 [![semantic-release: angular](https://img.shields.io/badge/semantic--release-angular-e10079?logo=semantic-release)](https://github.com/semantic-release/semantic-release)
 ![Interrogate](https://img.shields.io/badge/interrogate-100.0%25-brightgreen)
 ![Coverage](https://img.shields.io/badge/coverage-100%25-brightgreen?logo=codecov)
 ![Python](https://img.shields.io/badge/python->=3.11-blue?logo=python)
 
-
+## Important Note:
+To run Github Actions properly, please add svc-admin to your project!
 
 ## Usage
  - To use this template, click the green `Use this template` button and `Create new repository`.
  - After github initially creates the new repository, please wait an extra minute for the initialization scripts to finish organizing the repo.
  - To enable the automatic semantic version increments: in the repository go to `Settings` and `Collaborators and teams`. Click the green `Add people` button. Add `svc-aindscicomp` as an admin. Modify the file in `.github/workflows/tag_and_publish.yml` and remove the if statement in line 10. The semantic version will now be incremented every time a code is committed into the main branch.
  - To publish to PyPI, enable semantic versioning and uncomment the publish block in `.github/workflows/tag_and_publish.yml`. The code will now be published to PyPI every time the code is committed into the main branch.
  - The `.github/workflows/test_and_lint.yml` file will run automated tests and style checks every time a Pull Request is opened. If the checks are undesired, the `test_and_lint.yml` can be deleted. The strictness of the code coverage level, etc., can be modified by altering the configurations in the `pyproject.toml` file and the `.flake8` file.
@@ -107,14 +108,14 @@
 | `fix(pencil): stop graphite breaking when too much pressure applied`                                                                                                                             | ~~Patch~~ Fix Release, Default release                                                                          |
 | `feat(pencil): add 'graphiteWidth' option`                                                                                                                                                       | ~~Minor~~ Feature Release                                                                                       |
 | `perf(pencil): remove graphiteWidth option`<br><br>`BREAKING CHANGE: The graphiteWidth option has been removed.`<br>`The default graphite width of 10mm is always used for performance reasons.` | ~~Major~~ Breaking Release <br /> (Note that the `BREAKING CHANGE: ` token must be in the footer of the commit) |
 
 ### Documentation
 To generate the rst files source files for documentation, run
 ```bash
-sphinx-apidoc -o doc_template/source/ src 
+sphinx-apidoc -o doc_template/source/ src
 ```
 Then to create the documentation HTML files, run
 ```bash
 sphinx-build -b html doc_template/source/ doc_template/build/html
 ```
 More info on sphinx installation can be found [here](https://www.sphinx-doc.org/en/master/usage/installation.html).
```

### Comparing `aind_behavior_curriculum_template-0.0.1/README.md` & `aind_behavior_curriculum_template-0.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 [![License](https://img.shields.io/badge/license-MIT-brightgreen)](LICENSE)
 ![Code Style](https://img.shields.io/badge/code%20style-black-black)
 [![semantic-release: angular](https://img.shields.io/badge/semantic--release-angular-e10079?logo=semantic-release)](https://github.com/semantic-release/semantic-release)
 ![Interrogate](https://img.shields.io/badge/interrogate-100.0%25-brightgreen)
 ![Coverage](https://img.shields.io/badge/coverage-100%25-brightgreen?logo=codecov)
 ![Python](https://img.shields.io/badge/python->=3.11-blue?logo=python)
 
-
+## Important Note:
+To run Github Actions properly, please add svc-admin to your project!
 
 ## Usage
  - To use this template, click the green `Use this template` button and `Create new repository`.
  - After github initially creates the new repository, please wait an extra minute for the initialization scripts to finish organizing the repo.
  - To enable the automatic semantic version increments: in the repository go to `Settings` and `Collaborators and teams`. Click the green `Add people` button. Add `svc-aindscicomp` as an admin. Modify the file in `.github/workflows/tag_and_publish.yml` and remove the if statement in line 10. The semantic version will now be incremented every time a code is committed into the main branch.
  - To publish to PyPI, enable semantic versioning and uncomment the publish block in `.github/workflows/tag_and_publish.yml`. The code will now be published to PyPI every time the code is committed into the main branch.
  - The `.github/workflows/test_and_lint.yml` file will run automated tests and style checks every time a Pull Request is opened. If the checks are undesired, the `test_and_lint.yml` can be deleted. The strictness of the code coverage level, etc., can be modified by altering the configurations in the `pyproject.toml` file and the `.flake8` file.
@@ -87,14 +88,14 @@
 | `fix(pencil): stop graphite breaking when too much pressure applied`                                                                                                                             | ~~Patch~~ Fix Release, Default release                                                                          |
 | `feat(pencil): add 'graphiteWidth' option`                                                                                                                                                       | ~~Minor~~ Feature Release                                                                                       |
 | `perf(pencil): remove graphiteWidth option`<br><br>`BREAKING CHANGE: The graphiteWidth option has been removed.`<br>`The default graphite width of 10mm is always used for performance reasons.` | ~~Major~~ Breaking Release <br /> (Note that the `BREAKING CHANGE: ` token must be in the footer of the commit) |
 
 ### Documentation
 To generate the rst files source files for documentation, run
 ```bash
-sphinx-apidoc -o doc_template/source/ src 
+sphinx-apidoc -o doc_template/source/ src
 ```
 Then to create the documentation HTML files, run
 ```bash
 sphinx-build -b html doc_template/source/ doc_template/build/html
 ```
 More info on sphinx installation can be found [here](https://www.sphinx-doc.org/en/master/usage/installation.html).
```

### Comparing `aind_behavior_curriculum_template-0.0.1/doc_template/Makefile` & `aind_behavior_curriculum_template-0.0.2/doc_template/Makefile`

 * *Files identical despite different names*

### Comparing `aind_behavior_curriculum_template-0.0.1/doc_template/make.bat` & `aind_behavior_curriculum_template-0.0.2/doc_template/make.bat`

 * *Files identical despite different names*

### Comparing `aind_behavior_curriculum_template-0.0.1/doc_template/source/_static/dark-logo.svg` & `aind_behavior_curriculum_template-0.0.2/doc_template/source/_static/dark-logo.svg`

 * *Files identical despite different names*

### Comparing `aind_behavior_curriculum_template-0.0.1/doc_template/source/_static/favicon.ico` & `aind_behavior_curriculum_template-0.0.2/doc_template/source/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `aind_behavior_curriculum_template-0.0.1/doc_template/source/_static/light-logo.svg` & `aind_behavior_curriculum_template-0.0.2/doc_template/source/_static/light-logo.svg`

 * *Files identical despite different names*

### Comparing `aind_behavior_curriculum_template-0.0.1/doc_template/source/conf.py` & `aind_behavior_curriculum_template-0.0.2/doc_template/source/conf.py`

 * *Files identical despite different names*

### Comparing `aind_behavior_curriculum_template-0.0.1/pyproject.toml` & `aind_behavior_curriculum_template-0.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aind_behavior_curriculum_template-0.0.1/src/aind_behavior_curriculum_template.egg-info/PKG-INFO` & `aind_behavior_curriculum_template-0.0.2/src/aind_behavior_curriculum_template.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aind-behavior-curriculum-template
-Version: 0.0.1
+Version: 0.0.2
 Summary: Generated from aind-behavior-curriculum-template
 Author: Allen Institute for Neural Dynamics
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -23,15 +23,16 @@
 [![License](https://img.shields.io/badge/license-MIT-brightgreen)](LICENSE)
 ![Code Style](https://img.shields.io/badge/code%20style-black-black)
 [![semantic-release: angular](https://img.shields.io/badge/semantic--release-angular-e10079?logo=semantic-release)](https://github.com/semantic-release/semantic-release)
 ![Interrogate](https://img.shields.io/badge/interrogate-100.0%25-brightgreen)
 ![Coverage](https://img.shields.io/badge/coverage-100%25-brightgreen?logo=codecov)
 ![Python](https://img.shields.io/badge/python->=3.11-blue?logo=python)
 
-
+## Important Note:
+To run Github Actions properly, please add svc-admin to your project!
 
 ## Usage
  - To use this template, click the green `Use this template` button and `Create new repository`.
  - After github initially creates the new repository, please wait an extra minute for the initialization scripts to finish organizing the repo.
  - To enable the automatic semantic version increments: in the repository go to `Settings` and `Collaborators and teams`. Click the green `Add people` button. Add `svc-aindscicomp` as an admin. Modify the file in `.github/workflows/tag_and_publish.yml` and remove the if statement in line 10. The semantic version will now be incremented every time a code is committed into the main branch.
  - To publish to PyPI, enable semantic versioning and uncomment the publish block in `.github/workflows/tag_and_publish.yml`. The code will now be published to PyPI every time the code is committed into the main branch.
  - The `.github/workflows/test_and_lint.yml` file will run automated tests and style checks every time a Pull Request is opened. If the checks are undesired, the `test_and_lint.yml` can be deleted. The strictness of the code coverage level, etc., can be modified by altering the configurations in the `pyproject.toml` file and the `.flake8` file.
@@ -107,14 +108,14 @@
 | `fix(pencil): stop graphite breaking when too much pressure applied`                                                                                                                             | ~~Patch~~ Fix Release, Default release                                                                          |
 | `feat(pencil): add 'graphiteWidth' option`                                                                                                                                                       | ~~Minor~~ Feature Release                                                                                       |
 | `perf(pencil): remove graphiteWidth option`<br><br>`BREAKING CHANGE: The graphiteWidth option has been removed.`<br>`The default graphite width of 10mm is always used for performance reasons.` | ~~Major~~ Breaking Release <br /> (Note that the `BREAKING CHANGE: ` token must be in the footer of the commit) |
 
 ### Documentation
 To generate the rst files source files for documentation, run
 ```bash
-sphinx-apidoc -o doc_template/source/ src 
+sphinx-apidoc -o doc_template/source/ src
 ```
 Then to create the documentation HTML files, run
 ```bash
 sphinx-build -b html doc_template/source/ doc_template/build/html
 ```
 More info on sphinx installation can be found [here](https://www.sphinx-doc.org/en/master/usage/installation.html).
```

### Comparing `aind_behavior_curriculum_template-0.0.1/src/aind_behavior_curriculum_template.egg-info/SOURCES.txt` & `aind_behavior_curriculum_template-0.0.2/src/aind_behavior_curriculum_template.egg-info/SOURCES.txt`

 * *Files identical despite different names*

