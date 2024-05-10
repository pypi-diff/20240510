# Comparing `tmp/aind_behavior_curriculum-0.0.6.tar.gz` & `tmp/aind_behavior_curriculum-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aind_behavior_curriculum-0.0.6.tar", last modified: Fri May 10 19:07:19 2024, max compression
+gzip compressed data, was "aind_behavior_curriculum-0.0.7.tar", last modified: Fri May 10 19:09:19 2024, max compression
```

## Comparing `aind_behavior_curriculum-0.0.6.tar` & `aind_behavior_curriculum-0.0.7.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:07:19.109240 aind_behavior_curriculum-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-10 19:07:09.000000 aind_behavior_curriculum-0.0.6/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:07:19.097240 aind_behavior_curriculum-0.0.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:07:19.101240 aind_behavior_curriculum-0.0.6/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-10 19:07:09.000000 aind_behavior_curriculum-0.0.6/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-10 19:07:09.000000 aind_behavior_curriculum-0.0.6/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-10 19:07:09.000000 aind_behavior_curriculum-0.0.6/.github/ISSUE_TEMPLATE/user-story.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:07:19.101240 aind_behavior_curriculum-0.0.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3088 2024-05-10 19:07:09.000000 aind_behavior_curriculum-0.0.6/.github/workflows/tag_and_publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-10 19:07:09.000000 aind_behavior_curriculum-0.0.6/.github/workflows/test_and_lint.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-05-10 19:07:09.000000 aind_behavior_curriculum-0.0.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-10 19:07:09.000000 aind_behavior_curriculum-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10256 2024-05-10 19:07:19.109240 aind_behavior_curriculum-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9547 2024-05-10 19:07:09.000000 aind_behavior_curriculum-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:07:19.109240 aind_behavior_curriculum-0.0.6/aind_behavior_curriculum.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10256 2024-05-10 19:07:19.000000 aind_behavior_curriculum-0.0.6/aind_behavior_curriculum.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-05-10 19:07:19.000000 aind_behavior_curriculum-0.0.6/aind_behavior_curriculum.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 19:07:19.000000 aind_behavior_curriculum-0.0.6/aind_behavior_curriculum.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-10 19:07:19.000000 aind_behavior_curriculum-0.0.6/aind_behavior_curriculum.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-10 19:07:19.000000 aind_behavior_curriculum-0.0.6/aind_behavior_curriculum.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:07:19.101240 aind_behavior_curriculum-0.0.6/doc_template/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-10 19:07:09.000000 aind_behavior_curriculum-0.0.6/doc_template/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-10 19:07:09.000000 aind_behavior_curriculum-0.0.6/doc_template/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:07:19.101240 aind_behavior_curriculum-0.0.6/doc_template/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:07:19.105240 aind_behavior_curriculum-0.0.6/doc_template/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     8733 2024-05-10 19:07:09.000000 aind_behavior_curriculum-0.0.6/doc_template/source/_static/dark-logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)   259838 2024-05-10 19:07:09.000000 aind_behavior_curriculum-0.0.6/doc_template/source/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)     8712 2024-05-10 19:07:09.000000 aind_behavior_curriculum-0.0.6/doc_template/source/_static/light-logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-05-10 19:07:09.000000 aind_behavior_curriculum-0.0.6/doc_template/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-10 19:07:09.000000 aind_behavior_curriculum-0.0.6/doc_template/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:07:19.097240 aind_behavior_curriculum-0.0.6/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:07:19.105240 aind_behavior_curriculum-0.0.6/examples/example_project/
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-10 19:07:09.000000 aind_behavior_curriculum-0.0.6/examples/example_project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5435 2024-05-10 19:07:09.000000 aind_behavior_curriculum-0.0.6/examples/example_project/curriculum.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:07:19.105240 aind_behavior_curriculum-0.0.6/examples/example_project/diagrams/
--rw-r--r--   0 runner    (1001) docker     (127)    17362 2024-05-10 19:07:09.000000 aind_behavior_curriculum-0.0.6/examples/example_project/diagrams/high_level_curr_diagram.png
--rw-r--r--   0 runner    (1001) docker     (127)    54759 2024-05-10 19:07:09.000000 aind_behavior_curriculum-0.0.6/examples/example_project/diagrams/my_curr_diagram.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:07:19.105240 aind_behavior_curriculum-0.0.6/examples/example_project/jsons/
--rw-r--r--   0 runner    (1001) docker     (127)     5345 2024-05-10 19:07:09.000000 aind_behavior_curriculum-0.0.6/examples/example_project/jsons/curr_instance.json
--rw-r--r--   0 runner    (1001) docker     (127)    12354 2024-05-10 19:07:09.000000 aind_behavior_curriculum-0.0.6/examples/example_project/jsons/schema.json
--rw-r--r--   0 runner    (1001) docker     (127)    11108 2024-05-10 19:07:09.000000 aind_behavior_curriculum-0.0.6/examples/example_project/jsons/schema_manual_union.json
--rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-05-10 19:07:09.000000 aind_behavior_curriculum-0.0.6/examples/example_project/jsons/stage_instance.json
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-10 19:07:09.000000 aind_behavior_curriculum-0.0.6/examples/example_project/jsons/task_instance.json
--rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-05-10 19:07:09.000000 aind_behavior_curriculum-0.0.6/examples/example_project/jsons/task_schema.json
--rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-05-10 19:07:09.000000 aind_behavior_curriculum-0.0.6/examples/example_project/task.py
--rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-05-10 19:07:09.000000 aind_behavior_curriculum-0.0.6/examples/example_project/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:07:19.105240 aind_behavior_curriculum-0.0.6/examples/example_project_2/
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-10 19:07:09.000000 aind_behavior_curriculum-0.0.6/examples/example_project_2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7867 2024-05-10 19:07:09.000000 aind_behavior_curriculum-0.0.6/examples/example_project_2/curriculum.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:07:19.109240 aind_behavior_curriculum-0.0.6/examples/example_project_2/diagrams/
--rw-r--r--   0 runner    (1001) docker     (127)    36267 2024-05-10 19:07:09.000000 aind_behavior_curriculum-0.0.6/examples/example_project_2/diagrams/p_triangle_curr_diagram.png
--rw-r--r--   0 runner    (1001) docker     (127)    40434 2024-05-10 19:07:09.000000 aind_behavior_curriculum-0.0.6/examples/example_project_2/diagrams/s_triangle_curr_diagram.png
--rw-r--r--   0 runner    (1001) docker     (127)    22657 2024-05-10 19:07:09.000000 aind_behavior_curriculum-0.0.6/examples/example_project_2/diagrams/track_curr_diagram.png
--rw-r--r--   0 runner    (1001) docker     (127)    30415 2024-05-10 19:07:09.000000 aind_behavior_curriculum-0.0.6/examples/example_project_2/diagrams/tree_curr_diagram.png
--rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-05-10 19:07:09.000000 aind_behavior_curriculum-0.0.6/examples/example_project_2/trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-05-10 19:07:09.000000 aind_behavior_curriculum-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 19:07:19.109240 aind_behavior_curriculum-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-10 19:07:09.000000 aind_behavior_curriculum-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:07:19.097240 aind_behavior_curriculum-0.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:07:19.109240 aind_behavior_curriculum-0.0.6/src/aind_behavior_curriculum/
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-10 19:07:09.000000 aind_behavior_curriculum-0.0.6/src/aind_behavior_curriculum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-10 19:07:09.000000 aind_behavior_curriculum-0.0.6/src/aind_behavior_curriculum/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    32954 2024-05-10 19:07:09.000000 aind_behavior_curriculum-0.0.6/src/aind_behavior_curriculum/curriculum.py
--rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-05-10 19:07:09.000000 aind_behavior_curriculum-0.0.6/src/aind_behavior_curriculum/curriculum_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-05-10 19:07:09.000000 aind_behavior_curriculum-0.0.6/src/aind_behavior_curriculum/task.py
--rw-r--r--   0 runner    (1001) docker     (127)    13220 2024-05-10 19:07:09.000000 aind_behavior_curriculum-0.0.6/src/aind_behavior_curriculum/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:07:19.109240 aind_behavior_curriculum-0.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-10 19:07:09.000000 aind_behavior_curriculum-0.0.6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16299 2024-05-10 19:07:09.000000 aind_behavior_curriculum-0.0.6/tests/test_curriculum.py
--rw-r--r--   0 runner    (1001) docker     (127)     2825 2024-05-10 19:07:09.000000 aind_behavior_curriculum-0.0.6/tests/test_task.py
--rw-r--r--   0 runner    (1001) docker     (127)    25660 2024-05-10 19:07:09.000000 aind_behavior_curriculum-0.0.6/tests/test_trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:09:19.730752 aind_behavior_curriculum-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-10 19:09:11.000000 aind_behavior_curriculum-0.0.7/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:09:19.718752 aind_behavior_curriculum-0.0.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:09:19.722752 aind_behavior_curriculum-0.0.7/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-10 19:09:11.000000 aind_behavior_curriculum-0.0.7/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-10 19:09:11.000000 aind_behavior_curriculum-0.0.7/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-10 19:09:11.000000 aind_behavior_curriculum-0.0.7/.github/ISSUE_TEMPLATE/user-story.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:09:19.722752 aind_behavior_curriculum-0.0.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3088 2024-05-10 19:09:11.000000 aind_behavior_curriculum-0.0.7/.github/workflows/tag_and_publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-10 19:09:11.000000 aind_behavior_curriculum-0.0.7/.github/workflows/test_and_lint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-05-10 19:09:11.000000 aind_behavior_curriculum-0.0.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-10 19:09:11.000000 aind_behavior_curriculum-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10321 2024-05-10 19:09:19.730752 aind_behavior_curriculum-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9612 2024-05-10 19:09:11.000000 aind_behavior_curriculum-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:09:19.726752 aind_behavior_curriculum-0.0.7/aind_behavior_curriculum.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10321 2024-05-10 19:09:19.000000 aind_behavior_curriculum-0.0.7/aind_behavior_curriculum.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-05-10 19:09:19.000000 aind_behavior_curriculum-0.0.7/aind_behavior_curriculum.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 19:09:19.000000 aind_behavior_curriculum-0.0.7/aind_behavior_curriculum.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-10 19:09:19.000000 aind_behavior_curriculum-0.0.7/aind_behavior_curriculum.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-10 19:09:19.000000 aind_behavior_curriculum-0.0.7/aind_behavior_curriculum.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:09:19.722752 aind_behavior_curriculum-0.0.7/doc_template/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-10 19:09:11.000000 aind_behavior_curriculum-0.0.7/doc_template/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-10 19:09:11.000000 aind_behavior_curriculum-0.0.7/doc_template/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:09:19.722752 aind_behavior_curriculum-0.0.7/doc_template/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:09:19.722752 aind_behavior_curriculum-0.0.7/doc_template/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     8733 2024-05-10 19:09:11.000000 aind_behavior_curriculum-0.0.7/doc_template/source/_static/dark-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   259838 2024-05-10 19:09:11.000000 aind_behavior_curriculum-0.0.7/doc_template/source/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     8712 2024-05-10 19:09:11.000000 aind_behavior_curriculum-0.0.7/doc_template/source/_static/light-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-05-10 19:09:11.000000 aind_behavior_curriculum-0.0.7/doc_template/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-10 19:09:11.000000 aind_behavior_curriculum-0.0.7/doc_template/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:09:19.718752 aind_behavior_curriculum-0.0.7/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:09:19.722752 aind_behavior_curriculum-0.0.7/examples/example_project/
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-10 19:09:11.000000 aind_behavior_curriculum-0.0.7/examples/example_project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5435 2024-05-10 19:09:11.000000 aind_behavior_curriculum-0.0.7/examples/example_project/curriculum.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:09:19.722752 aind_behavior_curriculum-0.0.7/examples/example_project/diagrams/
+-rw-r--r--   0 runner    (1001) docker     (127)    17362 2024-05-10 19:09:11.000000 aind_behavior_curriculum-0.0.7/examples/example_project/diagrams/high_level_curr_diagram.png
+-rw-r--r--   0 runner    (1001) docker     (127)    54759 2024-05-10 19:09:11.000000 aind_behavior_curriculum-0.0.7/examples/example_project/diagrams/my_curr_diagram.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:09:19.726752 aind_behavior_curriculum-0.0.7/examples/example_project/jsons/
+-rw-r--r--   0 runner    (1001) docker     (127)     5345 2024-05-10 19:09:11.000000 aind_behavior_curriculum-0.0.7/examples/example_project/jsons/curr_instance.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12354 2024-05-10 19:09:11.000000 aind_behavior_curriculum-0.0.7/examples/example_project/jsons/schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11108 2024-05-10 19:09:11.000000 aind_behavior_curriculum-0.0.7/examples/example_project/jsons/schema_manual_union.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-05-10 19:09:11.000000 aind_behavior_curriculum-0.0.7/examples/example_project/jsons/stage_instance.json
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-10 19:09:11.000000 aind_behavior_curriculum-0.0.7/examples/example_project/jsons/task_instance.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-05-10 19:09:11.000000 aind_behavior_curriculum-0.0.7/examples/example_project/jsons/task_schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-05-10 19:09:11.000000 aind_behavior_curriculum-0.0.7/examples/example_project/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-05-10 19:09:11.000000 aind_behavior_curriculum-0.0.7/examples/example_project/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:09:19.726752 aind_behavior_curriculum-0.0.7/examples/example_project_2/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-10 19:09:11.000000 aind_behavior_curriculum-0.0.7/examples/example_project_2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7867 2024-05-10 19:09:11.000000 aind_behavior_curriculum-0.0.7/examples/example_project_2/curriculum.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:09:19.726752 aind_behavior_curriculum-0.0.7/examples/example_project_2/diagrams/
+-rw-r--r--   0 runner    (1001) docker     (127)    36267 2024-05-10 19:09:11.000000 aind_behavior_curriculum-0.0.7/examples/example_project_2/diagrams/p_triangle_curr_diagram.png
+-rw-r--r--   0 runner    (1001) docker     (127)    40434 2024-05-10 19:09:11.000000 aind_behavior_curriculum-0.0.7/examples/example_project_2/diagrams/s_triangle_curr_diagram.png
+-rw-r--r--   0 runner    (1001) docker     (127)    22657 2024-05-10 19:09:11.000000 aind_behavior_curriculum-0.0.7/examples/example_project_2/diagrams/track_curr_diagram.png
+-rw-r--r--   0 runner    (1001) docker     (127)    30415 2024-05-10 19:09:11.000000 aind_behavior_curriculum-0.0.7/examples/example_project_2/diagrams/tree_curr_diagram.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-05-10 19:09:11.000000 aind_behavior_curriculum-0.0.7/examples/example_project_2/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-05-10 19:09:11.000000 aind_behavior_curriculum-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 19:09:19.730752 aind_behavior_curriculum-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-10 19:09:11.000000 aind_behavior_curriculum-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:09:19.718752 aind_behavior_curriculum-0.0.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:09:19.726752 aind_behavior_curriculum-0.0.7/src/aind_behavior_curriculum/
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-10 19:09:11.000000 aind_behavior_curriculum-0.0.7/src/aind_behavior_curriculum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-10 19:09:11.000000 aind_behavior_curriculum-0.0.7/src/aind_behavior_curriculum/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32954 2024-05-10 19:09:11.000000 aind_behavior_curriculum-0.0.7/src/aind_behavior_curriculum/curriculum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-05-10 19:09:11.000000 aind_behavior_curriculum-0.0.7/src/aind_behavior_curriculum/curriculum_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-05-10 19:09:11.000000 aind_behavior_curriculum-0.0.7/src/aind_behavior_curriculum/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13220 2024-05-10 19:09:11.000000 aind_behavior_curriculum-0.0.7/src/aind_behavior_curriculum/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:09:19.726752 aind_behavior_curriculum-0.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-10 19:09:11.000000 aind_behavior_curriculum-0.0.7/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16299 2024-05-10 19:09:11.000000 aind_behavior_curriculum-0.0.7/tests/test_curriculum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2825 2024-05-10 19:09:11.000000 aind_behavior_curriculum-0.0.7/tests/test_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25660 2024-05-10 19:09:11.000000 aind_behavior_curriculum-0.0.7/tests/test_trainer.py
```

### Comparing `aind_behavior_curriculum-0.0.6/.github/ISSUE_TEMPLATE/bug_report.md` & `aind_behavior_curriculum-0.0.7/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `aind_behavior_curriculum-0.0.6/.github/ISSUE_TEMPLATE/feature_request.md` & `aind_behavior_curriculum-0.0.7/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `aind_behavior_curriculum-0.0.6/.github/ISSUE_TEMPLATE/user-story.md` & `aind_behavior_curriculum-0.0.7/.github/ISSUE_TEMPLATE/user-story.md`

 * *Files identical despite different names*

### Comparing `aind_behavior_curriculum-0.0.6/.github/workflows/tag_and_publish.yml` & `aind_behavior_curriculum-0.0.7/.github/workflows/tag_and_publish.yml`

 * *Files identical despite different names*

### Comparing `aind_behavior_curriculum-0.0.6/.github/workflows/test_and_lint.yml` & `aind_behavior_curriculum-0.0.7/.github/workflows/test_and_lint.yml`

 * *Files identical despite different names*

### Comparing `aind_behavior_curriculum-0.0.6/.gitignore` & `aind_behavior_curriculum-0.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `aind_behavior_curriculum-0.0.6/LICENSE` & `aind_behavior_curriculum-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `aind_behavior_curriculum-0.0.6/PKG-INFO` & `aind_behavior_curriculum-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aind-behavior-curriculum
-Version: 0.0.6
+Version: 0.0.7
 Summary: Generated from aind-library-template
 Author: Allen Institute for Neural Dynamics
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -28,14 +28,18 @@
 [![semantic-release: angular](https://img.shields.io/badge/semantic--release-angular-e10079?logo=semantic-release)](https://github.com/semantic-release/semantic-release)
 ![Interrogate](https://img.shields.io/badge/interrogate-100.0%25-brightgreen)
 ![Coverage](https://img.shields.io/badge/coverage-100%25-brightgreen?logo=codecov)
 ![Python](https://img.shields.io/badge/python->=3.11-blue?logo=python)
 
 A core problem in mice training is accurately keeping track of each mouse's training stage and accurately setting the corresponding rig parameters. As the number of behavior studies, research assistants, and mice increase, manual tracking and parameter input is prone to human error. This library provides a flexible framework for defining mice curriculum enabling mouse training to be automated.
 
+## Installation
+```bash
+pip install aind-behavior-curriculum
+```
 
 ## Documentation
 
 ### Understanding a Curriculum
 
 A **``Curriculum``** is structured as a graph of training **``Stages``**.
 Each **``Stage``**  is associated with a **``Task``**, which is a set of rig parameters.
```

### Comparing `aind_behavior_curriculum-0.0.6/README.md` & `aind_behavior_curriculum-0.0.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,18 @@
 [![semantic-release: angular](https://img.shields.io/badge/semantic--release-angular-e10079?logo=semantic-release)](https://github.com/semantic-release/semantic-release)
 ![Interrogate](https://img.shields.io/badge/interrogate-100.0%25-brightgreen)
 ![Coverage](https://img.shields.io/badge/coverage-100%25-brightgreen?logo=codecov)
 ![Python](https://img.shields.io/badge/python->=3.11-blue?logo=python)
 
 A core problem in mice training is accurately keeping track of each mouse's training stage and accurately setting the corresponding rig parameters. As the number of behavior studies, research assistants, and mice increase, manual tracking and parameter input is prone to human error. This library provides a flexible framework for defining mice curriculum enabling mouse training to be automated.
 
+## Installation
+```bash
+pip install aind-behavior-curriculum
+```
 
 ## Documentation
 
 ### Understanding a Curriculum
 
 A **``Curriculum``** is structured as a graph of training **``Stages``**.
 Each **``Stage``**  is associated with a **``Task``**, which is a set of rig parameters.
```

### Comparing `aind_behavior_curriculum-0.0.6/aind_behavior_curriculum.egg-info/PKG-INFO` & `aind_behavior_curriculum-0.0.7/aind_behavior_curriculum.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aind-behavior-curriculum
-Version: 0.0.6
+Version: 0.0.7
 Summary: Generated from aind-library-template
 Author: Allen Institute for Neural Dynamics
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -28,14 +28,18 @@
 [![semantic-release: angular](https://img.shields.io/badge/semantic--release-angular-e10079?logo=semantic-release)](https://github.com/semantic-release/semantic-release)
 ![Interrogate](https://img.shields.io/badge/interrogate-100.0%25-brightgreen)
 ![Coverage](https://img.shields.io/badge/coverage-100%25-brightgreen?logo=codecov)
 ![Python](https://img.shields.io/badge/python->=3.11-blue?logo=python)
 
 A core problem in mice training is accurately keeping track of each mouse's training stage and accurately setting the corresponding rig parameters. As the number of behavior studies, research assistants, and mice increase, manual tracking and parameter input is prone to human error. This library provides a flexible framework for defining mice curriculum enabling mouse training to be automated.
 
+## Installation
+```bash
+pip install aind-behavior-curriculum
+```
 
 ## Documentation
 
 ### Understanding a Curriculum
 
 A **``Curriculum``** is structured as a graph of training **``Stages``**.
 Each **``Stage``**  is associated with a **``Task``**, which is a set of rig parameters.
```

### Comparing `aind_behavior_curriculum-0.0.6/aind_behavior_curriculum.egg-info/SOURCES.txt` & `aind_behavior_curriculum-0.0.7/aind_behavior_curriculum.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aind_behavior_curriculum-0.0.6/doc_template/Makefile` & `aind_behavior_curriculum-0.0.7/doc_template/Makefile`

 * *Files identical despite different names*

### Comparing `aind_behavior_curriculum-0.0.6/doc_template/make.bat` & `aind_behavior_curriculum-0.0.7/doc_template/make.bat`

 * *Files identical despite different names*

### Comparing `aind_behavior_curriculum-0.0.6/doc_template/source/_static/dark-logo.svg` & `aind_behavior_curriculum-0.0.7/doc_template/source/_static/dark-logo.svg`

 * *Files identical despite different names*

### Comparing `aind_behavior_curriculum-0.0.6/doc_template/source/_static/favicon.ico` & `aind_behavior_curriculum-0.0.7/doc_template/source/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `aind_behavior_curriculum-0.0.6/doc_template/source/_static/light-logo.svg` & `aind_behavior_curriculum-0.0.7/doc_template/source/_static/light-logo.svg`

 * *Files identical despite different names*

### Comparing `aind_behavior_curriculum-0.0.6/doc_template/source/conf.py` & `aind_behavior_curriculum-0.0.7/doc_template/source/conf.py`

 * *Files identical despite different names*

### Comparing `aind_behavior_curriculum-0.0.6/examples/example_project/curriculum.py` & `aind_behavior_curriculum-0.0.7/examples/example_project/curriculum.py`

 * *Files identical despite different names*

### Comparing `aind_behavior_curriculum-0.0.6/examples/example_project/diagrams/high_level_curr_diagram.png` & `aind_behavior_curriculum-0.0.7/examples/example_project/diagrams/high_level_curr_diagram.png`

 * *Files identical despite different names*

### Comparing `aind_behavior_curriculum-0.0.6/examples/example_project/diagrams/my_curr_diagram.png` & `aind_behavior_curriculum-0.0.7/examples/example_project/diagrams/my_curr_diagram.png`

 * *Files identical despite different names*

### Comparing `aind_behavior_curriculum-0.0.6/examples/example_project/jsons/curr_instance.json` & `aind_behavior_curriculum-0.0.7/examples/example_project/jsons/curr_instance.json`

 * *Files identical despite different names*

### Comparing `aind_behavior_curriculum-0.0.6/examples/example_project/jsons/schema.json` & `aind_behavior_curriculum-0.0.7/examples/example_project/jsons/schema.json`

 * *Files identical despite different names*

### Comparing `aind_behavior_curriculum-0.0.6/examples/example_project/jsons/schema_manual_union.json` & `aind_behavior_curriculum-0.0.7/examples/example_project/jsons/schema_manual_union.json`

 * *Files identical despite different names*

### Comparing `aind_behavior_curriculum-0.0.6/examples/example_project/jsons/stage_instance.json` & `aind_behavior_curriculum-0.0.7/examples/example_project/jsons/stage_instance.json`

 * *Files identical despite different names*

### Comparing `aind_behavior_curriculum-0.0.6/examples/example_project/jsons/task_schema.json` & `aind_behavior_curriculum-0.0.7/examples/example_project/jsons/task_schema.json`

 * *Files identical despite different names*

### Comparing `aind_behavior_curriculum-0.0.6/examples/example_project/task.py` & `aind_behavior_curriculum-0.0.7/examples/example_project/task.py`

 * *Files identical despite different names*

### Comparing `aind_behavior_curriculum-0.0.6/examples/example_project/trainer.py` & `aind_behavior_curriculum-0.0.7/examples/example_project/trainer.py`

 * *Files identical despite different names*

### Comparing `aind_behavior_curriculum-0.0.6/examples/example_project_2/curriculum.py` & `aind_behavior_curriculum-0.0.7/examples/example_project_2/curriculum.py`

 * *Files identical despite different names*

### Comparing `aind_behavior_curriculum-0.0.6/examples/example_project_2/diagrams/p_triangle_curr_diagram.png` & `aind_behavior_curriculum-0.0.7/examples/example_project_2/diagrams/p_triangle_curr_diagram.png`

 * *Files identical despite different names*

### Comparing `aind_behavior_curriculum-0.0.6/examples/example_project_2/diagrams/s_triangle_curr_diagram.png` & `aind_behavior_curriculum-0.0.7/examples/example_project_2/diagrams/s_triangle_curr_diagram.png`

 * *Files identical despite different names*

### Comparing `aind_behavior_curriculum-0.0.6/examples/example_project_2/diagrams/track_curr_diagram.png` & `aind_behavior_curriculum-0.0.7/examples/example_project_2/diagrams/track_curr_diagram.png`

 * *Files identical despite different names*

### Comparing `aind_behavior_curriculum-0.0.6/examples/example_project_2/diagrams/tree_curr_diagram.png` & `aind_behavior_curriculum-0.0.7/examples/example_project_2/diagrams/tree_curr_diagram.png`

 * *Files identical despite different names*

### Comparing `aind_behavior_curriculum-0.0.6/examples/example_project_2/trainer.py` & `aind_behavior_curriculum-0.0.7/examples/example_project_2/trainer.py`

 * *Files identical despite different names*

### Comparing `aind_behavior_curriculum-0.0.6/pyproject.toml` & `aind_behavior_curriculum-0.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aind_behavior_curriculum-0.0.6/src/aind_behavior_curriculum/base.py` & `aind_behavior_curriculum-0.0.7/src/aind_behavior_curriculum/base.py`

 * *Files identical despite different names*

### Comparing `aind_behavior_curriculum-0.0.6/src/aind_behavior_curriculum/curriculum.py` & `aind_behavior_curriculum-0.0.7/src/aind_behavior_curriculum/curriculum.py`

 * *Files identical despite different names*

### Comparing `aind_behavior_curriculum-0.0.6/src/aind_behavior_curriculum/curriculum_utils.py` & `aind_behavior_curriculum-0.0.7/src/aind_behavior_curriculum/curriculum_utils.py`

 * *Files identical despite different names*

### Comparing `aind_behavior_curriculum-0.0.6/src/aind_behavior_curriculum/task.py` & `aind_behavior_curriculum-0.0.7/src/aind_behavior_curriculum/task.py`

 * *Files identical despite different names*

### Comparing `aind_behavior_curriculum-0.0.6/src/aind_behavior_curriculum/trainer.py` & `aind_behavior_curriculum-0.0.7/src/aind_behavior_curriculum/trainer.py`

 * *Files identical despite different names*

### Comparing `aind_behavior_curriculum-0.0.6/tests/test_curriculum.py` & `aind_behavior_curriculum-0.0.7/tests/test_curriculum.py`

 * *Files identical despite different names*

### Comparing `aind_behavior_curriculum-0.0.6/tests/test_task.py` & `aind_behavior_curriculum-0.0.7/tests/test_task.py`

 * *Files identical despite different names*

### Comparing `aind_behavior_curriculum-0.0.6/tests/test_trainer.py` & `aind_behavior_curriculum-0.0.7/tests/test_trainer.py`

 * *Files identical despite different names*

