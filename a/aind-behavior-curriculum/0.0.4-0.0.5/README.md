# Comparing `tmp/aind_behavior_curriculum-0.0.4.tar.gz` & `tmp/aind_behavior_curriculum-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aind_behavior_curriculum-0.0.4.tar", last modified: Tue May  7 20:55:19 2024, max compression
+gzip compressed data, was "aind_behavior_curriculum-0.0.5.tar", last modified: Fri May 10 18:47:07 2024, max compression
```

## Comparing `aind_behavior_curriculum-0.0.4.tar` & `aind_behavior_curriculum-0.0.5.tar`

### file list

```diff
@@ -1,70 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:55:19.532108 aind_behavior_curriculum-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-07 20:55:10.000000 aind_behavior_curriculum-0.0.4/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:55:19.524108 aind_behavior_curriculum-0.0.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:55:19.524108 aind_behavior_curriculum-0.0.4/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-07 20:55:10.000000 aind_behavior_curriculum-0.0.4/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-07 20:55:10.000000 aind_behavior_curriculum-0.0.4/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-07 20:55:10.000000 aind_behavior_curriculum-0.0.4/.github/ISSUE_TEMPLATE/user-story.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:55:19.524108 aind_behavior_curriculum-0.0.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3088 2024-05-07 20:55:10.000000 aind_behavior_curriculum-0.0.4/.github/workflows/tag_and_publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-07 20:55:10.000000 aind_behavior_curriculum-0.0.4/.github/workflows/test_and_lint.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-05-07 20:55:10.000000 aind_behavior_curriculum-0.0.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-07 20:55:10.000000 aind_behavior_curriculum-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6477 2024-05-07 20:55:19.532108 aind_behavior_curriculum-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5768 2024-05-07 20:55:10.000000 aind_behavior_curriculum-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:55:19.532108 aind_behavior_curriculum-0.0.4/aind_behavior_curriculum.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6477 2024-05-07 20:55:19.000000 aind_behavior_curriculum-0.0.4/aind_behavior_curriculum.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-05-07 20:55:19.000000 aind_behavior_curriculum-0.0.4/aind_behavior_curriculum.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 20:55:19.000000 aind_behavior_curriculum-0.0.4/aind_behavior_curriculum.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-07 20:55:19.000000 aind_behavior_curriculum-0.0.4/aind_behavior_curriculum.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-07 20:55:19.000000 aind_behavior_curriculum-0.0.4/aind_behavior_curriculum.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:55:19.528108 aind_behavior_curriculum-0.0.4/doc_template/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-07 20:55:10.000000 aind_behavior_curriculum-0.0.4/doc_template/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-07 20:55:10.000000 aind_behavior_curriculum-0.0.4/doc_template/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:55:19.528108 aind_behavior_curriculum-0.0.4/doc_template/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:55:19.528108 aind_behavior_curriculum-0.0.4/doc_template/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     8733 2024-05-07 20:55:10.000000 aind_behavior_curriculum-0.0.4/doc_template/source/_static/dark-logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)   259838 2024-05-07 20:55:10.000000 aind_behavior_curriculum-0.0.4/doc_template/source/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)     8712 2024-05-07 20:55:10.000000 aind_behavior_curriculum-0.0.4/doc_template/source/_static/light-logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-05-07 20:55:10.000000 aind_behavior_curriculum-0.0.4/doc_template/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-07 20:55:10.000000 aind_behavior_curriculum-0.0.4/doc_template/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:55:19.524108 aind_behavior_curriculum-0.0.4/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:55:19.528108 aind_behavior_curriculum-0.0.4/examples/example_project/
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-07 20:55:10.000000 aind_behavior_curriculum-0.0.4/examples/example_project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5435 2024-05-07 20:55:10.000000 aind_behavior_curriculum-0.0.4/examples/example_project/curriculum.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:55:19.528108 aind_behavior_curriculum-0.0.4/examples/example_project/diagrams/
--rw-r--r--   0 runner    (1001) docker     (127)    54759 2024-05-07 20:55:10.000000 aind_behavior_curriculum-0.0.4/examples/example_project/diagrams/my_curr_diagram.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:55:19.528108 aind_behavior_curriculum-0.0.4/examples/example_project/jsons/
--rw-r--r--   0 runner    (1001) docker     (127)     5345 2024-05-07 20:55:10.000000 aind_behavior_curriculum-0.0.4/examples/example_project/jsons/curr_instance.json
--rw-r--r--   0 runner    (1001) docker     (127)    12354 2024-05-07 20:55:10.000000 aind_behavior_curriculum-0.0.4/examples/example_project/jsons/schema.json
--rw-r--r--   0 runner    (1001) docker     (127)    11108 2024-05-07 20:55:10.000000 aind_behavior_curriculum-0.0.4/examples/example_project/jsons/schema_manual_union.json
--rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-05-07 20:55:10.000000 aind_behavior_curriculum-0.0.4/examples/example_project/jsons/stage_instance.json
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-07 20:55:10.000000 aind_behavior_curriculum-0.0.4/examples/example_project/jsons/task_instance.json
--rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-05-07 20:55:10.000000 aind_behavior_curriculum-0.0.4/examples/example_project/jsons/task_schema.json
--rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-05-07 20:55:10.000000 aind_behavior_curriculum-0.0.4/examples/example_project/task.py
--rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-05-07 20:55:10.000000 aind_behavior_curriculum-0.0.4/examples/example_project/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:55:19.528108 aind_behavior_curriculum-0.0.4/examples/example_project_2/
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-07 20:55:10.000000 aind_behavior_curriculum-0.0.4/examples/example_project_2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7867 2024-05-07 20:55:10.000000 aind_behavior_curriculum-0.0.4/examples/example_project_2/curriculum.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:55:19.532108 aind_behavior_curriculum-0.0.4/examples/example_project_2/diagrams/
--rw-r--r--   0 runner    (1001) docker     (127)    36267 2024-05-07 20:55:10.000000 aind_behavior_curriculum-0.0.4/examples/example_project_2/diagrams/p_triangle_curr_diagram.png
--rw-r--r--   0 runner    (1001) docker     (127)    40434 2024-05-07 20:55:10.000000 aind_behavior_curriculum-0.0.4/examples/example_project_2/diagrams/s_triangle_curr_diagram.png
--rw-r--r--   0 runner    (1001) docker     (127)    22657 2024-05-07 20:55:10.000000 aind_behavior_curriculum-0.0.4/examples/example_project_2/diagrams/track_curr_diagram.png
--rw-r--r--   0 runner    (1001) docker     (127)    30415 2024-05-07 20:55:10.000000 aind_behavior_curriculum-0.0.4/examples/example_project_2/diagrams/tree_curr_diagram.png
--rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-05-07 20:55:10.000000 aind_behavior_curriculum-0.0.4/examples/example_project_2/trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-05-07 20:55:10.000000 aind_behavior_curriculum-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 20:55:19.532108 aind_behavior_curriculum-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-07 20:55:10.000000 aind_behavior_curriculum-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:55:19.524108 aind_behavior_curriculum-0.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:55:19.532108 aind_behavior_curriculum-0.0.4/src/aind_behavior_curriculum/
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-07 20:55:11.000000 aind_behavior_curriculum-0.0.4/src/aind_behavior_curriculum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-07 20:55:10.000000 aind_behavior_curriculum-0.0.4/src/aind_behavior_curriculum/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    32998 2024-05-07 20:55:10.000000 aind_behavior_curriculum-0.0.4/src/aind_behavior_curriculum/curriculum.py
--rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-05-07 20:55:10.000000 aind_behavior_curriculum-0.0.4/src/aind_behavior_curriculum/curriculum_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-05-07 20:55:10.000000 aind_behavior_curriculum-0.0.4/src/aind_behavior_curriculum/task.py
--rw-r--r--   0 runner    (1001) docker     (127)    13220 2024-05-07 20:55:10.000000 aind_behavior_curriculum-0.0.4/src/aind_behavior_curriculum/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:55:19.532108 aind_behavior_curriculum-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-07 20:55:10.000000 aind_behavior_curriculum-0.0.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16299 2024-05-07 20:55:10.000000 aind_behavior_curriculum-0.0.4/tests/test_curriculum.py
--rw-r--r--   0 runner    (1001) docker     (127)     2825 2024-05-07 20:55:10.000000 aind_behavior_curriculum-0.0.4/tests/test_task.py
--rw-r--r--   0 runner    (1001) docker     (127)    25660 2024-05-07 20:55:10.000000 aind_behavior_curriculum-0.0.4/tests/test_trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 18:47:07.866021 aind_behavior_curriculum-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-10 18:46:59.000000 aind_behavior_curriculum-0.0.5/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 18:47:07.854021 aind_behavior_curriculum-0.0.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 18:47:07.858021 aind_behavior_curriculum-0.0.5/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-10 18:46:59.000000 aind_behavior_curriculum-0.0.5/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-10 18:46:59.000000 aind_behavior_curriculum-0.0.5/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-10 18:46:59.000000 aind_behavior_curriculum-0.0.5/.github/ISSUE_TEMPLATE/user-story.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 18:47:07.858021 aind_behavior_curriculum-0.0.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3088 2024-05-10 18:46:59.000000 aind_behavior_curriculum-0.0.5/.github/workflows/tag_and_publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-10 18:46:59.000000 aind_behavior_curriculum-0.0.5/.github/workflows/test_and_lint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-05-10 18:46:59.000000 aind_behavior_curriculum-0.0.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-10 18:46:59.000000 aind_behavior_curriculum-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10239 2024-05-10 18:47:07.866021 aind_behavior_curriculum-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9530 2024-05-10 18:46:59.000000 aind_behavior_curriculum-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 18:47:07.862022 aind_behavior_curriculum-0.0.5/aind_behavior_curriculum.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10239 2024-05-10 18:47:07.000000 aind_behavior_curriculum-0.0.5/aind_behavior_curriculum.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-05-10 18:47:07.000000 aind_behavior_curriculum-0.0.5/aind_behavior_curriculum.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 18:47:07.000000 aind_behavior_curriculum-0.0.5/aind_behavior_curriculum.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-10 18:47:07.000000 aind_behavior_curriculum-0.0.5/aind_behavior_curriculum.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-10 18:47:07.000000 aind_behavior_curriculum-0.0.5/aind_behavior_curriculum.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 18:47:07.858021 aind_behavior_curriculum-0.0.5/doc_template/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-10 18:46:59.000000 aind_behavior_curriculum-0.0.5/doc_template/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-10 18:46:59.000000 aind_behavior_curriculum-0.0.5/doc_template/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 18:47:07.858021 aind_behavior_curriculum-0.0.5/doc_template/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 18:47:07.858021 aind_behavior_curriculum-0.0.5/doc_template/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     8733 2024-05-10 18:46:59.000000 aind_behavior_curriculum-0.0.5/doc_template/source/_static/dark-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   259838 2024-05-10 18:46:59.000000 aind_behavior_curriculum-0.0.5/doc_template/source/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     8712 2024-05-10 18:46:59.000000 aind_behavior_curriculum-0.0.5/doc_template/source/_static/light-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-05-10 18:46:59.000000 aind_behavior_curriculum-0.0.5/doc_template/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-10 18:46:59.000000 aind_behavior_curriculum-0.0.5/doc_template/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 18:47:07.854021 aind_behavior_curriculum-0.0.5/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 18:47:07.858021 aind_behavior_curriculum-0.0.5/examples/example_project/
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-10 18:46:59.000000 aind_behavior_curriculum-0.0.5/examples/example_project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5435 2024-05-10 18:46:59.000000 aind_behavior_curriculum-0.0.5/examples/example_project/curriculum.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 18:47:07.858021 aind_behavior_curriculum-0.0.5/examples/example_project/diagrams/
+-rw-r--r--   0 runner    (1001) docker     (127)    17362 2024-05-10 18:46:59.000000 aind_behavior_curriculum-0.0.5/examples/example_project/diagrams/high_level_curr_diagram.png
+-rw-r--r--   0 runner    (1001) docker     (127)    54759 2024-05-10 18:46:59.000000 aind_behavior_curriculum-0.0.5/examples/example_project/diagrams/my_curr_diagram.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 18:47:07.862022 aind_behavior_curriculum-0.0.5/examples/example_project/jsons/
+-rw-r--r--   0 runner    (1001) docker     (127)     5345 2024-05-10 18:46:59.000000 aind_behavior_curriculum-0.0.5/examples/example_project/jsons/curr_instance.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12354 2024-05-10 18:46:59.000000 aind_behavior_curriculum-0.0.5/examples/example_project/jsons/schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11108 2024-05-10 18:46:59.000000 aind_behavior_curriculum-0.0.5/examples/example_project/jsons/schema_manual_union.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-05-10 18:46:59.000000 aind_behavior_curriculum-0.0.5/examples/example_project/jsons/stage_instance.json
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-10 18:46:59.000000 aind_behavior_curriculum-0.0.5/examples/example_project/jsons/task_instance.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-05-10 18:46:59.000000 aind_behavior_curriculum-0.0.5/examples/example_project/jsons/task_schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-05-10 18:46:59.000000 aind_behavior_curriculum-0.0.5/examples/example_project/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-05-10 18:46:59.000000 aind_behavior_curriculum-0.0.5/examples/example_project/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 18:47:07.862022 aind_behavior_curriculum-0.0.5/examples/example_project_2/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-10 18:46:59.000000 aind_behavior_curriculum-0.0.5/examples/example_project_2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7867 2024-05-10 18:46:59.000000 aind_behavior_curriculum-0.0.5/examples/example_project_2/curriculum.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 18:47:07.862022 aind_behavior_curriculum-0.0.5/examples/example_project_2/diagrams/
+-rw-r--r--   0 runner    (1001) docker     (127)    36267 2024-05-10 18:46:59.000000 aind_behavior_curriculum-0.0.5/examples/example_project_2/diagrams/p_triangle_curr_diagram.png
+-rw-r--r--   0 runner    (1001) docker     (127)    40434 2024-05-10 18:46:59.000000 aind_behavior_curriculum-0.0.5/examples/example_project_2/diagrams/s_triangle_curr_diagram.png
+-rw-r--r--   0 runner    (1001) docker     (127)    22657 2024-05-10 18:46:59.000000 aind_behavior_curriculum-0.0.5/examples/example_project_2/diagrams/track_curr_diagram.png
+-rw-r--r--   0 runner    (1001) docker     (127)    30415 2024-05-10 18:46:59.000000 aind_behavior_curriculum-0.0.5/examples/example_project_2/diagrams/tree_curr_diagram.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-05-10 18:46:59.000000 aind_behavior_curriculum-0.0.5/examples/example_project_2/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-05-10 18:46:59.000000 aind_behavior_curriculum-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 18:47:07.866021 aind_behavior_curriculum-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-10 18:46:59.000000 aind_behavior_curriculum-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 18:47:07.854021 aind_behavior_curriculum-0.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 18:47:07.862022 aind_behavior_curriculum-0.0.5/src/aind_behavior_curriculum/
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-10 18:46:59.000000 aind_behavior_curriculum-0.0.5/src/aind_behavior_curriculum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-10 18:46:59.000000 aind_behavior_curriculum-0.0.5/src/aind_behavior_curriculum/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32954 2024-05-10 18:46:59.000000 aind_behavior_curriculum-0.0.5/src/aind_behavior_curriculum/curriculum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-05-10 18:46:59.000000 aind_behavior_curriculum-0.0.5/src/aind_behavior_curriculum/curriculum_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-05-10 18:46:59.000000 aind_behavior_curriculum-0.0.5/src/aind_behavior_curriculum/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13220 2024-05-10 18:46:59.000000 aind_behavior_curriculum-0.0.5/src/aind_behavior_curriculum/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 18:47:07.862022 aind_behavior_curriculum-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-10 18:46:59.000000 aind_behavior_curriculum-0.0.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16299 2024-05-10 18:46:59.000000 aind_behavior_curriculum-0.0.5/tests/test_curriculum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2825 2024-05-10 18:46:59.000000 aind_behavior_curriculum-0.0.5/tests/test_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25660 2024-05-10 18:46:59.000000 aind_behavior_curriculum-0.0.5/tests/test_trainer.py
```

### Comparing `aind_behavior_curriculum-0.0.4/.github/ISSUE_TEMPLATE/bug_report.md` & `aind_behavior_curriculum-0.0.5/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `aind_behavior_curriculum-0.0.4/.github/ISSUE_TEMPLATE/feature_request.md` & `aind_behavior_curriculum-0.0.5/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `aind_behavior_curriculum-0.0.4/.github/ISSUE_TEMPLATE/user-story.md` & `aind_behavior_curriculum-0.0.5/.github/ISSUE_TEMPLATE/user-story.md`

 * *Files identical despite different names*

### Comparing `aind_behavior_curriculum-0.0.4/.github/workflows/tag_and_publish.yml` & `aind_behavior_curriculum-0.0.5/.github/workflows/tag_and_publish.yml`

 * *Files identical despite different names*

### Comparing `aind_behavior_curriculum-0.0.4/.github/workflows/test_and_lint.yml` & `aind_behavior_curriculum-0.0.5/.github/workflows/test_and_lint.yml`

 * *Files identical despite different names*

### Comparing `aind_behavior_curriculum-0.0.4/.gitignore` & `aind_behavior_curriculum-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `aind_behavior_curriculum-0.0.4/LICENSE` & `aind_behavior_curriculum-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `aind_behavior_curriculum-0.0.4/aind_behavior_curriculum.egg-info/SOURCES.txt` & `aind_behavior_curriculum-0.0.5/aind_behavior_curriculum.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 doc_template/source/_static/dark-logo.svg
 doc_template/source/_static/favicon.ico
 doc_template/source/_static/light-logo.svg
 examples/example_project/__init__.py
 examples/example_project/curriculum.py
 examples/example_project/task.py
 examples/example_project/trainer.py
+examples/example_project/diagrams/high_level_curr_diagram.png
 examples/example_project/diagrams/my_curr_diagram.png
 examples/example_project/jsons/curr_instance.json
 examples/example_project/jsons/schema.json
 examples/example_project/jsons/schema_manual_union.json
 examples/example_project/jsons/stage_instance.json
 examples/example_project/jsons/task_instance.json
 examples/example_project/jsons/task_schema.json
```

### Comparing `aind_behavior_curriculum-0.0.4/doc_template/Makefile` & `aind_behavior_curriculum-0.0.5/doc_template/Makefile`

 * *Files identical despite different names*

### Comparing `aind_behavior_curriculum-0.0.4/doc_template/make.bat` & `aind_behavior_curriculum-0.0.5/doc_template/make.bat`

 * *Files identical despite different names*

### Comparing `aind_behavior_curriculum-0.0.4/doc_template/source/_static/dark-logo.svg` & `aind_behavior_curriculum-0.0.5/doc_template/source/_static/dark-logo.svg`

 * *Files identical despite different names*

### Comparing `aind_behavior_curriculum-0.0.4/doc_template/source/_static/favicon.ico` & `aind_behavior_curriculum-0.0.5/doc_template/source/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `aind_behavior_curriculum-0.0.4/doc_template/source/_static/light-logo.svg` & `aind_behavior_curriculum-0.0.5/doc_template/source/_static/light-logo.svg`

 * *Files identical despite different names*

### Comparing `aind_behavior_curriculum-0.0.4/doc_template/source/conf.py` & `aind_behavior_curriculum-0.0.5/doc_template/source/conf.py`

 * *Files identical despite different names*

### Comparing `aind_behavior_curriculum-0.0.4/examples/example_project/curriculum.py` & `aind_behavior_curriculum-0.0.5/examples/example_project/curriculum.py`

 * *Files identical despite different names*

### Comparing `aind_behavior_curriculum-0.0.4/examples/example_project/diagrams/my_curr_diagram.png` & `aind_behavior_curriculum-0.0.5/examples/example_project/diagrams/my_curr_diagram.png`

 * *Files identical despite different names*

### Comparing `aind_behavior_curriculum-0.0.4/examples/example_project/jsons/curr_instance.json` & `aind_behavior_curriculum-0.0.5/examples/example_project/jsons/curr_instance.json`

 * *Files identical despite different names*

### Comparing `aind_behavior_curriculum-0.0.4/examples/example_project/jsons/schema.json` & `aind_behavior_curriculum-0.0.5/examples/example_project/jsons/schema.json`

 * *Files identical despite different names*

### Comparing `aind_behavior_curriculum-0.0.4/examples/example_project/jsons/schema_manual_union.json` & `aind_behavior_curriculum-0.0.5/examples/example_project/jsons/schema_manual_union.json`

 * *Files identical despite different names*

### Comparing `aind_behavior_curriculum-0.0.4/examples/example_project/jsons/stage_instance.json` & `aind_behavior_curriculum-0.0.5/examples/example_project/jsons/stage_instance.json`

 * *Files identical despite different names*

### Comparing `aind_behavior_curriculum-0.0.4/examples/example_project/jsons/task_schema.json` & `aind_behavior_curriculum-0.0.5/examples/example_project/jsons/task_schema.json`

 * *Files identical despite different names*

### Comparing `aind_behavior_curriculum-0.0.4/examples/example_project/task.py` & `aind_behavior_curriculum-0.0.5/examples/example_project/task.py`

 * *Files identical despite different names*

### Comparing `aind_behavior_curriculum-0.0.4/examples/example_project/trainer.py` & `aind_behavior_curriculum-0.0.5/examples/example_project/trainer.py`

 * *Files identical despite different names*

### Comparing `aind_behavior_curriculum-0.0.4/examples/example_project_2/curriculum.py` & `aind_behavior_curriculum-0.0.5/examples/example_project_2/curriculum.py`

 * *Files identical despite different names*

### Comparing `aind_behavior_curriculum-0.0.4/examples/example_project_2/diagrams/p_triangle_curr_diagram.png` & `aind_behavior_curriculum-0.0.5/examples/example_project_2/diagrams/p_triangle_curr_diagram.png`

 * *Files identical despite different names*

### Comparing `aind_behavior_curriculum-0.0.4/examples/example_project_2/diagrams/s_triangle_curr_diagram.png` & `aind_behavior_curriculum-0.0.5/examples/example_project_2/diagrams/s_triangle_curr_diagram.png`

 * *Files identical despite different names*

### Comparing `aind_behavior_curriculum-0.0.4/examples/example_project_2/diagrams/track_curr_diagram.png` & `aind_behavior_curriculum-0.0.5/examples/example_project_2/diagrams/track_curr_diagram.png`

 * *Files identical despite different names*

### Comparing `aind_behavior_curriculum-0.0.4/examples/example_project_2/diagrams/tree_curr_diagram.png` & `aind_behavior_curriculum-0.0.5/examples/example_project_2/diagrams/tree_curr_diagram.png`

 * *Files identical despite different names*

### Comparing `aind_behavior_curriculum-0.0.4/examples/example_project_2/trainer.py` & `aind_behavior_curriculum-0.0.5/examples/example_project_2/trainer.py`

 * *Files identical despite different names*

### Comparing `aind_behavior_curriculum-0.0.4/pyproject.toml` & `aind_behavior_curriculum-0.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aind_behavior_curriculum-0.0.4/src/aind_behavior_curriculum/base.py` & `aind_behavior_curriculum-0.0.5/src/aind_behavior_curriculum/base.py`

 * *Files identical despite different names*

### Comparing `aind_behavior_curriculum-0.0.4/src/aind_behavior_curriculum/curriculum.py` & `aind_behavior_curriculum-0.0.5/src/aind_behavior_curriculum/curriculum.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 import subprocess
 import warnings
 from importlib import import_module
 from pathlib import Path
 from typing import Any, Callable, Dict, Generic, List, Tuple, TypeVar
 
 import boto3
-from botocore.exceptions import ClientError
 from jinja2 import Template
 from pydantic import Field, GetJsonSchemaHandler, field_validator
 from pydantic.json_schema import JsonSchemaValue
 from pydantic_core import core_schema
 
 from aind_behavior_curriculum import (
     AindBehaviorModel,
```

### Comparing `aind_behavior_curriculum-0.0.4/src/aind_behavior_curriculum/curriculum_utils.py` & `aind_behavior_curriculum-0.0.5/src/aind_behavior_curriculum/curriculum_utils.py`

 * *Files identical despite different names*

### Comparing `aind_behavior_curriculum-0.0.4/src/aind_behavior_curriculum/task.py` & `aind_behavior_curriculum-0.0.5/src/aind_behavior_curriculum/task.py`

 * *Files identical despite different names*

### Comparing `aind_behavior_curriculum-0.0.4/src/aind_behavior_curriculum/trainer.py` & `aind_behavior_curriculum-0.0.5/src/aind_behavior_curriculum/trainer.py`

 * *Files identical despite different names*

### Comparing `aind_behavior_curriculum-0.0.4/tests/test_curriculum.py` & `aind_behavior_curriculum-0.0.5/tests/test_curriculum.py`

 * *Files identical despite different names*

### Comparing `aind_behavior_curriculum-0.0.4/tests/test_task.py` & `aind_behavior_curriculum-0.0.5/tests/test_task.py`

 * *Files identical despite different names*

### Comparing `aind_behavior_curriculum-0.0.4/tests/test_trainer.py` & `aind_behavior_curriculum-0.0.5/tests/test_trainer.py`

 * *Files identical despite different names*

