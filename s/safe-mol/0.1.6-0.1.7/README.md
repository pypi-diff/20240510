# Comparing `tmp/safe-mol-0.1.6.tar.gz` & `tmp/safe_mol-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "safe-mol-0.1.6.tar", last modified: Thu Apr 11 15:23:04 2024, max compression
+gzip compressed data, was "safe_mol-0.1.7.tar", last modified: Fri May 10 15:51:34 2024, max compression
```

## Comparing `safe-mol-0.1.6.tar` & `safe_mol-0.1.7.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:23:04.484078 safe-mol-0.1.6/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:23:04.472078 safe-mol-0.1.6/.github/
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-11 15:19:06.000000 safe-mol-0.1.6/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-11 15:19:06.000000 safe-mol-0.1.6/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-11 15:19:06.000000 safe-mol-0.1.6/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-11 15:19:06.000000 safe-mol-0.1.6/.github/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:23:04.472078 safe-mol-0.1.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-11 15:19:06.000000 safe-mol-0.1.6/.github/workflows/code-check.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-11 15:19:06.000000 safe-mol-0.1.6/.github/workflows/doc.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3764 2024-04-11 15:19:06.000000 safe-mol-0.1.6/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-11 15:19:06.000000 safe-mol-0.1.6/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-11 15:19:06.000000 safe-mol-0.1.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-11 15:19:06.000000 safe-mol-0.1.6/DATA_LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11314 2024-04-11 15:19:06.000000 safe-mol-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10341 2024-04-11 15:23:04.484078 safe-mol-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8577 2024-04-11 15:19:06.000000 safe-mol-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:23:04.476078 safe-mol-0.1.6/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:23:04.476078 safe-mol-0.1.6/docs/api/
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-11 15:19:06.000000 safe-mol-0.1.6/docs/api/safe.md
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-11 15:19:06.000000 safe-mol-0.1.6/docs/api/safe.models.md
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-11 15:19:06.000000 safe-mol-0.1.6/docs/api/safe.viz.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:23:04.476078 safe-mol-0.1.6/docs/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:23:04.476078 safe-mol-0.1.6/docs/assets/js/
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-11 15:19:06.000000 safe-mol-0.1.6/docs/assets/js/google-analytics.js
--rw-r--r--   0 runner    (1001) docker     (127)    36030 2024-04-11 15:19:06.000000 safe-mol-0.1.6/docs/assets/safe-construction.svg
--rw-r--r--   0 runner    (1001) docker     (127)    86699 2024-04-11 15:19:06.000000 safe-mol-0.1.6/docs/assets/safe-tasks.svg
--rw-r--r--   0 runner    (1001) docker     (127)    30045 2024-04-11 15:19:06.000000 safe-mol-0.1.6/docs/cli.md
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-11 15:19:06.000000 safe-mol-0.1.6/docs/data_license.md
--rw-r--r--   0 runner    (1001) docker     (127)     8563 2024-04-11 15:19:06.000000 safe-mol-0.1.6/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-11 15:19:06.000000 safe-mol-0.1.6/docs/license.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:23:04.480078 safe-mol-0.1.6/docs/tutorials/
--rw-r--r--   0 runner    (1001) docker     (127)  1793089 2024-04-11 15:19:06.000000 safe-mol-0.1.6/docs/tutorials/design-with-safe.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    36563 2024-04-11 15:19:06.000000 safe-mol-0.1.6/docs/tutorials/extracting-representation-molfeat.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   138661 2024-04-11 15:19:06.000000 safe-mol-0.1.6/docs/tutorials/getting-started.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    91753 2024-04-11 15:19:06.000000 safe-mol-0.1.6/docs/tutorials/how-it-works.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-11 15:19:06.000000 safe-mol-0.1.6/env.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:23:04.472078 safe-mol-0.1.6/expts/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:23:04.480078 safe-mol-0.1.6/expts/config/
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-11 15:19:06.000000 safe-mol-0.1.6/expts/config/accelerate.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:23:04.480078 safe-mol-0.1.6/expts/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)      348 2024-04-11 15:19:06.000000 safe-mol-0.1.6/expts/scripts/slurm-data-build.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      349 2024-04-11 15:19:06.000000 safe-mol-0.1.6/expts/scripts/slurm-notebook.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)     1230 2024-04-11 15:19:06.000000 safe-mol-0.1.6/expts/scripts/slurm-tokenizer-train-custom.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)     1176 2024-04-11 15:19:06.000000 safe-mol-0.1.6/expts/scripts/slurm-tokenizer-train-small.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)     1168 2024-04-11 15:19:06.000000 safe-mol-0.1.6/expts/scripts/slurm-tokenizer-train.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      683 2024-04-11 15:19:06.000000 safe-mol-0.1.6/expts/scripts/train-small.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      688 2024-04-11 15:19:06.000000 safe-mol-0.1.6/expts/scripts/train.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:23:04.480078 safe-mol-0.1.6/expts/tokenizer/
--rw-r--r--   0 runner    (1001) docker     (127)    19689 2024-04-11 15:19:06.000000 safe-mol-0.1.6/expts/tokenizer/_tokenizer-custom-mini-test.json
--rw-r--r--   0 runner    (1001) docker     (127)    46319 2024-04-11 15:19:06.000000 safe-mol-0.1.6/expts/tokenizer/tokenizer-custom.json
--rw-r--r--   0 runner    (1001) docker     (127)     2743 2024-04-11 15:19:06.000000 safe-mol-0.1.6/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-04-11 15:19:06.000000 safe-mol-0.1.6/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:23:04.480078 safe-mol-0.1.6/safe/
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-11 15:19:06.000000 safe-mol-0.1.6/safe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-11 15:19:06.000000 safe-mol-0.1.6/safe/_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)    17588 2024-04-11 15:19:06.000000 safe-mol-0.1.6/safe/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)    39204 2024-04-11 15:19:06.000000 safe-mol-0.1.6/safe/sample.py
--rw-r--r--   0 runner    (1001) docker     (127)    25797 2024-04-11 15:19:06.000000 safe-mol-0.1.6/safe/tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:23:04.480078 safe-mol-0.1.6/safe/trainer/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-11 15:19:06.000000 safe-mol-0.1.6/safe/trainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15829 2024-04-11 15:19:06.000000 safe-mol-0.1.6/safe/trainer/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3690 2024-04-11 15:19:06.000000 safe-mol-0.1.6/safe/trainer/collator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:23:04.484078 safe-mol-0.1.6/safe/trainer/configs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 15:19:06.000000 safe-mol-0.1.6/safe/trainer/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-11 15:19:06.000000 safe-mol-0.1.6/safe/trainer/configs/default_config.json
--rw-r--r--   0 runner    (1001) docker     (127)     5355 2024-04-11 15:19:06.000000 safe-mol-0.1.6/safe/trainer/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9736 2024-04-11 15:19:06.000000 safe-mol-0.1.6/safe/trainer/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-04-11 15:19:06.000000 safe-mol-0.1.6/safe/trainer/trainer_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    22577 2024-04-11 15:19:06.000000 safe-mol-0.1.6/safe/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3509 2024-04-11 15:19:06.000000 safe-mol-0.1.6/safe/viz.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:23:04.484078 safe-mol-0.1.6/safe_mol.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10341 2024-04-11 15:23:04.000000 safe-mol-0.1.6/safe_mol.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-04-11 15:23:04.000000 safe-mol-0.1.6/safe_mol.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 15:23:04.000000 safe-mol-0.1.6/safe_mol.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-11 15:23:04.000000 safe-mol-0.1.6/safe_mol.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 15:23:00.000000 safe-mol-0.1.6/safe_mol.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-11 15:23:04.000000 safe-mol-0.1.6/safe_mol.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-11 15:23:04.000000 safe-mol-0.1.6/safe_mol.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 15:23:04.484078 safe-mol-0.1.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:23:04.484078 safe-mol-0.1.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-11 15:19:06.000000 safe-mol-0.1.6/tests/test_hgf_load.py
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-11 15:19:06.000000 safe-mol-0.1.6/tests/test_import.py
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-11 15:19:06.000000 safe-mol-0.1.6/tests/test_notebooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     4393 2024-04-11 15:19:06.000000 safe-mol-0.1.6/tests/test_safe.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:51:34.409455 safe_mol-0.1.7/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:51:34.397455 safe_mol-0.1.7/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-10 15:47:42.000000 safe_mol-0.1.7/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-10 15:47:42.000000 safe_mol-0.1.7/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-10 15:47:42.000000 safe_mol-0.1.7/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-10 15:47:42.000000 safe_mol-0.1.7/.github/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:51:34.397455 safe_mol-0.1.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-05-10 15:47:42.000000 safe_mol-0.1.7/.github/workflows/code-check.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-10 15:47:42.000000 safe_mol-0.1.7/.github/workflows/doc.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3764 2024-05-10 15:47:42.000000 safe_mol-0.1.7/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-10 15:47:42.000000 safe_mol-0.1.7/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-10 15:47:42.000000 safe_mol-0.1.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-10 15:47:42.000000 safe_mol-0.1.7/DATA_LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11314 2024-05-10 15:47:42.000000 safe_mol-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10341 2024-05-10 15:51:34.409455 safe_mol-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8577 2024-05-10 15:47:42.000000 safe_mol-0.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:51:34.401455 safe_mol-0.1.7/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:51:34.401455 safe_mol-0.1.7/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-10 15:47:42.000000 safe_mol-0.1.7/docs/api/safe.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-10 15:47:42.000000 safe_mol-0.1.7/docs/api/safe.models.md
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-10 15:47:42.000000 safe_mol-0.1.7/docs/api/safe.viz.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:51:34.401455 safe_mol-0.1.7/docs/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:51:34.401455 safe_mol-0.1.7/docs/assets/js/
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-10 15:47:42.000000 safe_mol-0.1.7/docs/assets/js/google-analytics.js
+-rw-r--r--   0 runner    (1001) docker     (127)    36030 2024-05-10 15:47:42.000000 safe_mol-0.1.7/docs/assets/safe-construction.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    86699 2024-05-10 15:47:42.000000 safe_mol-0.1.7/docs/assets/safe-tasks.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    30045 2024-05-10 15:47:42.000000 safe_mol-0.1.7/docs/cli.md
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-10 15:47:42.000000 safe_mol-0.1.7/docs/data_license.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8563 2024-05-10 15:47:42.000000 safe_mol-0.1.7/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-10 15:47:42.000000 safe_mol-0.1.7/docs/license.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:51:34.405455 safe_mol-0.1.7/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (127)  1793089 2024-05-10 15:47:42.000000 safe_mol-0.1.7/docs/tutorials/design-with-safe.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    36563 2024-05-10 15:47:42.000000 safe_mol-0.1.7/docs/tutorials/extracting-representation-molfeat.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   138661 2024-05-10 15:47:42.000000 safe_mol-0.1.7/docs/tutorials/getting-started.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    91753 2024-05-10 15:47:42.000000 safe_mol-0.1.7/docs/tutorials/how-it-works.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-10 15:47:42.000000 safe_mol-0.1.7/env.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:51:34.397455 safe_mol-0.1.7/expts/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:51:34.405455 safe_mol-0.1.7/expts/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-05-10 15:47:42.000000 safe_mol-0.1.7/expts/config/accelerate.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:51:34.405455 safe_mol-0.1.7/expts/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      348 2024-05-10 15:47:42.000000 safe_mol-0.1.7/expts/scripts/slurm-data-build.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      349 2024-05-10 15:47:42.000000 safe_mol-0.1.7/expts/scripts/slurm-notebook.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1230 2024-05-10 15:47:42.000000 safe_mol-0.1.7/expts/scripts/slurm-tokenizer-train-custom.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1176 2024-05-10 15:47:42.000000 safe_mol-0.1.7/expts/scripts/slurm-tokenizer-train-small.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1168 2024-05-10 15:47:42.000000 safe_mol-0.1.7/expts/scripts/slurm-tokenizer-train.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      683 2024-05-10 15:47:42.000000 safe_mol-0.1.7/expts/scripts/train-small.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      688 2024-05-10 15:47:42.000000 safe_mol-0.1.7/expts/scripts/train.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:51:34.405455 safe_mol-0.1.7/expts/tokenizer/
+-rw-r--r--   0 runner    (1001) docker     (127)    19689 2024-05-10 15:47:42.000000 safe_mol-0.1.7/expts/tokenizer/_tokenizer-custom-mini-test.json
+-rw-r--r--   0 runner    (1001) docker     (127)    46319 2024-05-10 15:47:42.000000 safe_mol-0.1.7/expts/tokenizer/tokenizer-custom.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2743 2024-05-10 15:47:42.000000 safe_mol-0.1.7/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-05-10 15:47:42.000000 safe_mol-0.1.7/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:51:34.405455 safe_mol-0.1.7/safe/
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-10 15:47:42.000000 safe_mol-0.1.7/safe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-10 15:47:42.000000 safe_mol-0.1.7/safe/_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18799 2024-05-10 15:47:42.000000 safe_mol-0.1.7/safe/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39204 2024-05-10 15:47:42.000000 safe_mol-0.1.7/safe/sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25797 2024-05-10 15:47:42.000000 safe_mol-0.1.7/safe/tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:51:34.409455 safe_mol-0.1.7/safe/trainer/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-10 15:47:42.000000 safe_mol-0.1.7/safe/trainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15829 2024-05-10 15:47:42.000000 safe_mol-0.1.7/safe/trainer/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3690 2024-05-10 15:47:42.000000 safe_mol-0.1.7/safe/trainer/collator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:51:34.409455 safe_mol-0.1.7/safe/trainer/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 15:47:42.000000 safe_mol-0.1.7/safe/trainer/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-05-10 15:47:42.000000 safe_mol-0.1.7/safe/trainer/configs/default_config.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5355 2024-05-10 15:47:42.000000 safe_mol-0.1.7/safe/trainer/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9736 2024-05-10 15:47:42.000000 safe_mol-0.1.7/safe/trainer/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-05-10 15:47:42.000000 safe_mol-0.1.7/safe/trainer/trainer_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22577 2024-05-10 15:47:42.000000 safe_mol-0.1.7/safe/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3509 2024-05-10 15:47:42.000000 safe_mol-0.1.7/safe/viz.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:51:34.409455 safe_mol-0.1.7/safe_mol.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10341 2024-05-10 15:51:34.000000 safe_mol-0.1.7/safe_mol.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-05-10 15:51:34.000000 safe_mol-0.1.7/safe_mol.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 15:51:34.000000 safe_mol-0.1.7/safe_mol.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-10 15:51:34.000000 safe_mol-0.1.7/safe_mol.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 15:51:30.000000 safe_mol-0.1.7/safe_mol.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-10 15:51:34.000000 safe_mol-0.1.7/safe_mol.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-10 15:51:34.000000 safe_mol-0.1.7/safe_mol.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 15:51:34.409455 safe_mol-0.1.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:51:34.409455 safe_mol-0.1.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-05-10 15:47:42.000000 safe_mol-0.1.7/tests/test_hgf_load.py
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-10 15:47:42.000000 safe_mol-0.1.7/tests/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-05-10 15:47:42.000000 safe_mol-0.1.7/tests/test_notebooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5533 2024-05-10 15:47:42.000000 safe_mol-0.1.7/tests/test_safe.py
```

### Comparing `safe-mol-0.1.6/.github/PULL_REQUEST_TEMPLATE.md` & `safe_mol-0.1.7/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `safe-mol-0.1.6/.github/workflows/code-check.yml` & `safe_mol-0.1.7/.github/workflows/code-check.yml`

 * *Files identical despite different names*

### Comparing `safe-mol-0.1.6/.github/workflows/doc.yml` & `safe_mol-0.1.7/.github/workflows/doc.yml`

 * *Files identical despite different names*

### Comparing `safe-mol-0.1.6/.github/workflows/release.yml` & `safe_mol-0.1.7/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `safe-mol-0.1.6/.github/workflows/test.yml` & `safe_mol-0.1.7/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `safe-mol-0.1.6/.gitignore` & `safe_mol-0.1.7/.gitignore`

 * *Files identical despite different names*

### Comparing `safe-mol-0.1.6/LICENSE` & `safe_mol-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `safe-mol-0.1.6/PKG-INFO` & `safe_mol-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: safe-mol
-Version: 0.1.6
+Version: 0.1.7
 Summary: Implementation of the 'Gotta be SAFE: a new framework for molecular design' paper
 Author-email: Emmanuel Noutahi <emmanuel.noutahi@gmail.com>
 License: Apache-2.0
 Project-URL: Source Code, https://github.com/datamol-io/safe
 Project-URL: Bug Tracker, https://github.com/datamol-io/safe/issues
 Project-URL: Documentation, https://safe-docs.datamol.io/
 Keywords: safe,smiles,de novo,design,molecules
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: safe-mol Version: 0.1.6 Summary: Implementation of
+Metadata-Version: 2.1 Name: safe-mol Version: 0.1.7 Summary: Implementation of
 the 'Gotta be SAFE: a new framework for molecular design' paper Author-email:
 Emmanuel Noutahi
 gmail.com> License: Apache-2.0 Project-URL: Source Code, https://github.com/
 datamol-io/safe Project-URL: Bug Tracker, https://github.com/datamol-io/safe/
 issues Project-URL: Documentation, https://safe-docs.datamol.io/ Keywords:
 safe,smiles,de novo,design,molecules Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Developers Classifier:
```

### Comparing `safe-mol-0.1.6/README.md` & `safe_mol-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `safe-mol-0.1.6/docs/api/safe.models.md` & `safe_mol-0.1.7/docs/api/safe.models.md`

 * *Files identical despite different names*

### Comparing `safe-mol-0.1.6/docs/assets/safe-construction.svg` & `safe_mol-0.1.7/docs/assets/safe-construction.svg`

 * *Files identical despite different names*

### Comparing `safe-mol-0.1.6/docs/assets/safe-tasks.svg` & `safe_mol-0.1.7/docs/assets/safe-tasks.svg`

 * *Files identical despite different names*

### Comparing `safe-mol-0.1.6/docs/cli.md` & `safe_mol-0.1.7/docs/cli.md`

 * *Files identical despite different names*

### Comparing `safe-mol-0.1.6/docs/index.md` & `safe_mol-0.1.7/docs/index.md`

 * *Files identical despite different names*

### Comparing `safe-mol-0.1.6/docs/tutorials/design-with-safe.ipynb` & `safe_mol-0.1.7/docs/tutorials/design-with-safe.ipynb`

 * *Files identical despite different names*

### Comparing `safe-mol-0.1.6/docs/tutorials/extracting-representation-molfeat.ipynb` & `safe_mol-0.1.7/docs/tutorials/extracting-representation-molfeat.ipynb`

 * *Files identical despite different names*

### Comparing `safe-mol-0.1.6/docs/tutorials/getting-started.ipynb` & `safe_mol-0.1.7/docs/tutorials/getting-started.ipynb`

 * *Files identical despite different names*

### Comparing `safe-mol-0.1.6/docs/tutorials/how-it-works.ipynb` & `safe_mol-0.1.7/docs/tutorials/how-it-works.ipynb`

 * *Files identical despite different names*

### Comparing `safe-mol-0.1.6/env.yml` & `safe_mol-0.1.7/env.yml`

 * *Files 13% similar despite different names*

```diff
@@ -30,17 +30,18 @@
   - ruff
   - pytest >=6.0
   - nbconvert
   - jupyterlab
   - nbconvert
   - ipywidgets
 
-  # Doc
-  - mkdocs
-  - mkdocs-material >=7.1.1
-  - mkdocs-material-extensions
-  - mkdocstrings
-  - mkdocstrings-python
-  - mkdocs-jupyter
-  - markdown-include
-  - mdx_truly_sane_lists
-  - mike >=1.0.0
+  - pip:
+    - mkdocs <1.6.0
+    - mkdocs-material >=7.1.1
+    - mkdocs-material-extensions
+    - mkdocstrings
+    - mkdocstrings-python
+    - mkdocs-jupyter
+    - markdown-include
+    - markdown-include
+    - mdx_truly_sane_lists
+    - mike >=1.0.0
```

### Comparing `safe-mol-0.1.6/expts/scripts/slurm-tokenizer-train-custom.sh` & `safe_mol-0.1.7/expts/scripts/slurm-tokenizer-train-custom.sh`

 * *Files identical despite different names*

### Comparing `safe-mol-0.1.6/expts/scripts/slurm-tokenizer-train-small.sh` & `safe_mol-0.1.7/expts/scripts/slurm-tokenizer-train-small.sh`

 * *Files identical despite different names*

### Comparing `safe-mol-0.1.6/expts/scripts/slurm-tokenizer-train.sh` & `safe_mol-0.1.7/expts/scripts/slurm-tokenizer-train.sh`

 * *Files identical despite different names*

### Comparing `safe-mol-0.1.6/expts/scripts/train-small.sh` & `safe_mol-0.1.7/expts/scripts/train-small.sh`

 * *Files identical despite different names*

### Comparing `safe-mol-0.1.6/expts/scripts/train.sh` & `safe_mol-0.1.7/expts/scripts/train.sh`

 * *Files identical despite different names*

### Comparing `safe-mol-0.1.6/expts/tokenizer/_tokenizer-custom-mini-test.json` & `safe_mol-0.1.7/expts/tokenizer/_tokenizer-custom-mini-test.json`

 * *Files identical despite different names*

### Comparing `safe-mol-0.1.6/expts/tokenizer/tokenizer-custom.json` & `safe_mol-0.1.7/expts/tokenizer/tokenizer-custom.json`

 * *Files identical despite different names*

### Comparing `safe-mol-0.1.6/mkdocs.yml` & `safe_mol-0.1.7/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `safe-mol-0.1.6/pyproject.toml` & `safe_mol-0.1.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `safe-mol-0.1.6/safe/converter.py` & `safe_mol-0.1.7/safe/converter.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from contextlib import suppress
 from typing import Callable, List, Optional, Union
 
 import datamol as dm
 import numpy as np
 from rdkit import Chem
 from rdkit.Chem import BRICS
+from loguru import logger
 
 from ._exception import SAFEDecodeError, SAFEEncodeError, SAFEFragmentationError
 from .utils import standardize_attach
 
 
 class SAFEConverter:
     """Molecule line notation conversion from SMILES to SAFE
@@ -30,60 +31,67 @@
         * Any possible attachment points (`attach`)
 
         Furthermore, you can also provide your own slicing algorithm, which should return a pair of atoms
         corresponding to the bonds to break.
 
     """
 
-    SUPPORTED_SLICERS = ["hr", "recap", "mmpa", "attach", "brics"]
+    SUPPORTED_SLICERS = ["hr", "rotatable", "recap", "mmpa", "attach", "brics"]
     __SLICE_SMARTS = {
         "hr": ["[*]!@-[*]"],  # any non ring single bond
         "recap": [
-            "[C;$(C=O)]!@-N",  # amides and urea
-            "[C;$(C=O)]!@-O",  # esters
-            "C!@-[N;!$(NC=O)]",  # amines
-            "C!@-[O;!$(NC=O)]",  # ether
-            "[CX3]!@=[CX3]",  # olefin
-            "[N+X4]!@-C",  # quaternary nitrogen
-            "n!@-C",  # aromatic N - aliphatic C
-            "[$([NR][CR]=O)]!@-C",  # lactam nitrogen - aliphatic carbon
-            "c!@-c",  # aromatic C - aromatic C
-            "N!@-[$(S(=O)=O)]",  # sulphonamides
+            "[$([C;!$(C([#7])[#7])](=!@[O]))]!@[$([#7;+0;!D1])]",
+            "[$(C=!@O)]!@[$([O;+0])]",
+            "[$([N;!D1;+0;!$(N-C=[#7,#8,#15,#16])](-!@[*]))]-!@[$([*])]",
+            "[$(C(=!@O)([#7;+0;D2,D3])!@[#7;+0;D2,D3])]!@[$([#7;+0;D2,D3])]",
+            "[$([O;+0](-!@[#6!$(C=O)])-!@[#6!$(C=O)])]-!@[$([#6!$(C=O)])]",
+            "C=!@C",
+            "[N;+1;D4]!@[#6]",
+            "[$([n;+0])]-!@C",
+            "[$([O]=[C]-@[N;+0])]-!@[$([C])]",
+            "c-!@c",
+            "[$([#7;+0;D2,D3])]-!@[$([S](=[O])=[O])]",
         ],
         "mmpa": ["[#6+0;!$(*=,#[!#6])]!@!=!#[*]"],  # classical mmpa slicing smarts
         "attach": ["[*]!@[*]"],  # any potential attachment point, including hydrogens when explicit
+        "rotatable": ["[!$(*#*)&!D1]-&!@[!$(*#*)&!D1]"],
     }
 
     def __init__(
         self,
         slicer: Optional[Union[str, List[str], Callable]] = "brics",
         require_hs: Optional[bool] = None,
         use_original_opener_for_attach: bool = True,
+        ignore_stereo: bool = False,
     ):
         """Constructor for the SAFE converter
 
         Args:
             slicer: slicer algorithm to use for encoding.
                 Can either be one of the supported slicing algorithm (SUPPORTED_SLICERS)
                 or a custom callable that returns the bond ids that can be sliced.
             require_hs: whether the slicing algorithm require the molecule to have hydrogen explictly added.
                 `attach` slicer requires adding hydrogens.
             use_original_opener_for_attach: whether to use the original branch opener digit when adding back
                 mapping number to attachment points, or use simple enumeration.
+            ignore_stereo: RDKIT does not support some particular SAFE subset when stereochemistry is defined.
 
         """
         self.slicer = slicer
         if isinstance(slicer, str) and slicer.lower() in self.SUPPORTED_SLICERS:
             self.slicer = self.__SLICE_SMARTS.get(slicer.lower(), slicer)
         if self.slicer != "brics" and isinstance(self.slicer, str):
             self.slicer = [self.slicer]
         if isinstance(self.slicer, (list, tuple)):
             self.slicer = [dm.from_smarts(x) for x in self.slicer]
+            if any(x is None for x in self.slicer):
+                raise ValueError(f"Slicer: {slicer} cannot be valid")
         self.require_hs = require_hs or (slicer == "attach")
         self.use_original_opener_for_attach = use_original_opener_for_attach
+        self.ignore_stereo = ignore_stereo
 
     @staticmethod
     def randomize(mol: dm.Mol, rng: Optional[int] = None):
         """Randomize the position of the atoms in a mol.
 
         Args:
             mol: molecules to randomize
@@ -254,14 +262,18 @@
         # inp = dm.reactions.convert_attach_to_isotope(inp, as_smiles=True)
 
         # TODO(maclandrol): RDKit supports some extended form of ring closure, up to 5 digits
         # https://www.rdkit.org/docs/RDKit_Book.html#ring-closures and I should try to include them
         branch_numbers = self._find_branch_number(inp)
 
         mol = dm.to_mol(inp, remove_hs=False)
+        potential_stereos = Chem.FindPotentialStereo(mol)
+        has_stereo_bonds = any(x.type == Chem.StereoType.Bond_Double for x in potential_stereos)
+        if self.ignore_stereo:
+            mol = dm.remove_stereochemistry(mol)
 
         bond_map_id = 1
         for atom in mol.GetAtoms():
             if atom.GetAtomicNum() == 0:
                 atom.SetAtomMapNum(0)
                 atom.SetIsotope(bond_map_id)
                 bond_map_id += 1
@@ -340,48 +352,58 @@
             starting_num += 1
 
         # now we need to remove all the parenthesis around digit only number
         wrong_attach = re.compile(r"\(([\%\d]*)\)")
         scaffold_str = wrong_attach.sub(r"\g<1>", scaffold_str)
         # furthermore, we autoapply rdkit-compatible digit standardization.
         if rdkit_safe:
-            pattern = r"\(([=-@#]?)(%?\d{1,2})\)"
+            pattern = r"\(([=-@#\/\\]{0,2})(%?\d{1,2})\)"
             replacement = r"\g<1>\g<2>"
             scaffold_str = re.sub(pattern, replacement, scaffold_str)
+        if not self.ignore_stereo and has_stereo_bonds and not dm.same_mol(scaffold_str, inp):
+            logger.warning(
+                "Ignoring stereo is disabled, but molecule has stereochemistry interferring with SAFE representation"
+            )
         return scaffold_str
 
 
 def encode(
     inp: Union[str, dm.Mol],
     canonical: bool = True,
     randomize: Optional[bool] = False,
     seed: Optional[int] = None,
     slicer: Optional[Union[List[str], str, Callable]] = None,
     require_hs: Optional[bool] = None,
     constraints: Optional[List[dm.Mol]] = None,
+    ignore_stereo: Optional[bool] = False,
 ):
     """
     Convert input smiles to SAFE representation
 
     Args:
         inp: input smiles
         canonical: whether to return canonical SAFE string. Defaults to True
         randomize: whether to randomize the safe string encoding. Will be ignored if canonical is provided
         seed: optional seed to use when allowing randomization of the SAFE encoding.
         slicer: slicer algorithm to use for encoding. Defaults to "brics".
         require_hs: whether the slicing algorithm require the molecule to have hydrogen explictly added.
         constraints: List of molecules or pattern to preserve during the SAFE construction.
+        ignore_stereo: RDKIT does not support some particular SAFE subset when stereochemistry is defined.
     """
     if slicer is None:
         slicer = "brics"
     with dm.without_rdkit_log():
-        safe_obj = SAFEConverter(slicer=slicer, require_hs=require_hs)
+        safe_obj = SAFEConverter(slicer=slicer, require_hs=require_hs, ignore_stereo=ignore_stereo)
         try:
             encoded = safe_obj.encoder(
-                inp, canonical=canonical, randomize=randomize, constraints=constraints, seed=seed
+                inp,
+                canonical=canonical,
+                randomize=randomize,
+                constraints=constraints,
+                seed=seed,
             )
         except SAFEFragmentationError as e:
             raise e
         except Exception as e:
             raise SAFEEncodeError(f"Failed to encode {inp} with {slicer}") from e
         return encoded
```

### Comparing `safe-mol-0.1.6/safe/sample.py` & `safe_mol-0.1.7/safe/sample.py`

 * *Files identical despite different names*

### Comparing `safe-mol-0.1.6/safe/tokenizer.py` & `safe_mol-0.1.7/safe/tokenizer.py`

 * *Files identical despite different names*

### Comparing `safe-mol-0.1.6/safe/trainer/cli.py` & `safe_mol-0.1.7/safe/trainer/cli.py`

 * *Files identical despite different names*

### Comparing `safe-mol-0.1.6/safe/trainer/collator.py` & `safe_mol-0.1.7/safe/trainer/collator.py`

 * *Files identical despite different names*

### Comparing `safe-mol-0.1.6/safe/trainer/configs/default_config.json` & `safe_mol-0.1.7/safe/trainer/configs/default_config.json`

 * *Files identical despite different names*

### Comparing `safe-mol-0.1.6/safe/trainer/data_utils.py` & `safe_mol-0.1.7/safe/trainer/data_utils.py`

 * *Files identical despite different names*

### Comparing `safe-mol-0.1.6/safe/trainer/model.py` & `safe_mol-0.1.7/safe/trainer/model.py`

 * *Files identical despite different names*

### Comparing `safe-mol-0.1.6/safe/trainer/trainer_utils.py` & `safe_mol-0.1.7/safe/trainer/trainer_utils.py`

 * *Files identical despite different names*

### Comparing `safe-mol-0.1.6/safe/utils.py` & `safe_mol-0.1.7/safe/utils.py`

 * *Files identical despite different names*

### Comparing `safe-mol-0.1.6/safe/viz.py` & `safe_mol-0.1.7/safe/viz.py`

 * *Files identical despite different names*

### Comparing `safe-mol-0.1.6/safe_mol.egg-info/PKG-INFO` & `safe_mol-0.1.7/safe_mol.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: safe-mol
-Version: 0.1.6
+Version: 0.1.7
 Summary: Implementation of the 'Gotta be SAFE: a new framework for molecular design' paper
 Author-email: Emmanuel Noutahi <emmanuel.noutahi@gmail.com>
 License: Apache-2.0
 Project-URL: Source Code, https://github.com/datamol-io/safe
 Project-URL: Bug Tracker, https://github.com/datamol-io/safe/issues
 Project-URL: Documentation, https://safe-docs.datamol.io/
 Keywords: safe,smiles,de novo,design,molecules
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: safe-mol Version: 0.1.6 Summary: Implementation of
+Metadata-Version: 2.1 Name: safe-mol Version: 0.1.7 Summary: Implementation of
 the 'Gotta be SAFE: a new framework for molecular design' paper Author-email:
 Emmanuel Noutahi
 gmail.com> License: Apache-2.0 Project-URL: Source Code, https://github.com/
 datamol-io/safe Project-URL: Bug Tracker, https://github.com/datamol-io/safe/
 issues Project-URL: Documentation, https://safe-docs.datamol.io/ Keywords:
 safe,smiles,de novo,design,molecules Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Developers Classifier:
```

### Comparing `safe-mol-0.1.6/safe_mol.egg-info/SOURCES.txt` & `safe_mol-0.1.7/safe_mol.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `safe-mol-0.1.6/tests/test_hgf_load.py` & `safe_mol-0.1.7/tests/test_hgf_load.py`

 * *Files identical despite different names*

### Comparing `safe-mol-0.1.6/tests/test_notebooks.py` & `safe_mol-0.1.7/tests/test_notebooks.py`

 * *Files identical despite different names*

### Comparing `safe-mol-0.1.6/tests/test_safe.py` & `safe_mol-0.1.7/tests/test_safe.py`

 * *Files 15% similar despite different names*

```diff
@@ -117,7 +117,32 @@
         "[H][C@@]12CC[C@@]3(CCC(=O)O3)[C@@]1(C)CC[C@@]1([H])[C@@]2([H])[C@@]([H])(CC2=CC(=O)CC[C@]12C)SC(C)=O",
         "[H][C@@]12C[C@H](C)[C@](OC(=O)CC)(C(=O)COC(=O)CC)[C@@]1(C)C[C@H](O)[C@@]1(Cl)[C@@]2([H])CCC2=CC(=O)C=C[C@]12C",
         "[H][C@@]12CC[C@@](O)(C#C)[C@@]1(CC)CC[C@]1([H])[C@@]3([H])CCC(=O)C=C3CC[C@@]21[H]",
     ]
     for fused_ring in FUSED_RING_LIST:
         output_string = safe.decode(safe.encode(fused_ring))
         assert dm.same_mol(fused_ring, output_string)
+
+
+def test_stereochemistry_issue():
+    STEREO_MOL_LIST = [
+        "CC(=C\\c1ccccc1)/N=C/C(=O)O",
+        "CC(=C/c1ccccc1)/N=C/C(=O)O",
+        "CC(=C\\c1ccccc1)/N=C\\C(=O)O",
+        "CC(=C/c1ccccc1)/N=C\\C(=O)O",
+        "CC(=Cc1ccccc1)N=CC(=O)O",
+        "Cc1ccc(-n2c(C)cc(/C=N/Nc3ccc([N+](=O)[O-])cn3)c2C)c(C)c1",
+        "Cc1ccc(-n2c(C)cc(/C=N\\Nc3ccc([N+](=O)[O-])cn3)c2C)c(C)c1",
+    ]
+    for mol in STEREO_MOL_LIST:
+        output_string = safe.encode(mol, ignore_stereo=False, slicer="rotatable")
+        assert dm.same_mol(mol, output_string)
+
+    # now let's test failure case where we fail because we split on a double bond
+    output = safe.encode(STEREO_MOL_LIST[0], ignore_stereo=False, slicer="brics")
+    assert dm.same_mol(STEREO_MOL_LIST[0], output) is False
+    same_stereo = [dm.remove_stereochemistry(dm.to_mol(x)) for x in [output, STEREO_MOL_LIST[0]]]
+    assert dm.same_mol(same_stereo[0], same_stereo[1])
+
+    # check if we ignore the stereo
+    output = safe.encode(STEREO_MOL_LIST[0], ignore_stereo=True, slicer="brics")
+    assert dm.same_mol(dm.remove_stereochemistry(dm.to_mol(STEREO_MOL_LIST[0])), output)
```

