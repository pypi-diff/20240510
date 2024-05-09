# Comparing `tmp/kilosort-4.0.6.tar.gz` & `tmp/kilosort-4.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kilosort-4.0.6.tar", last modified: Sat Apr 27 00:27:17 2024, max compression
+gzip compressed data, was "kilosort-4.0.7.tar", last modified: Thu May  9 23:07:23 2024, max compression
```

## Comparing `kilosort-4.0.6.tar` & `kilosort-4.0.7.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:27:17.183471 kilosort-4.0.6/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:27:17.167471 kilosort-4.0.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:27:17.171471 kilosort-4.0.6/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-04-27 00:27:08.000000 kilosort-4.0.6/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-27 00:27:08.000000 kilosort-4.0.6/.github/ISSUE_TEMPLATE/feature_request.yml
--rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-27 00:27:08.000000 kilosort-4.0.6/.github/ISSUE_TEMPLATE/installation_issue.yml
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-27 00:27:08.000000 kilosort-4.0.6/.github/ISSUE_TEMPLATE/other.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:27:17.171471 kilosort-4.0.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-04-27 00:27:08.000000 kilosort-4.0.6/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-04-27 00:27:08.000000 kilosort-4.0.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-27 00:27:08.000000 kilosort-4.0.6/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3360 2024-04-27 00:27:08.000000 kilosort-4.0.6/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-27 00:27:08.000000 kilosort-4.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10348 2024-04-27 00:27:17.183471 kilosort-4.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8987 2024-04-27 00:27:08.000000 kilosort-4.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:27:17.171471 kilosort-4.0.6/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-27 00:27:08.000000 kilosort-4.0.6/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-27 00:27:08.000000 kilosort-4.0.6/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2892 2024-04-27 00:27:08.000000 kilosort-4.0.6/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     6082 2024-04-27 00:27:08.000000 kilosort-4.0.6/docs/drift.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6710 2024-04-27 00:27:08.000000 kilosort-4.0.6/docs/gui_guide.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-04-27 00:27:08.000000 kilosort-4.0.6/docs/hardware.rst
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-27 00:27:08.000000 kilosort-4.0.6/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-27 00:27:08.000000 kilosort-4.0.6/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-27 00:27:08.000000 kilosort-4.0.6/docs/multi_shank.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6080 2024-04-27 00:27:08.000000 kilosort-4.0.6/docs/parameters.rst
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-27 00:27:08.000000 kilosort-4.0.6/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:27:17.175471 kilosort-4.0.6/docs/tutorials/
--rw-r--r--   0 runner    (1001) docker     (127)     9953 2024-04-27 00:27:08.000000 kilosort-4.0.6/docs/tutorials/basic_example.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    13669 2024-04-27 00:27:08.000000 kilosort-4.0.6/docs/tutorials/load_data.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     8102 2024-04-27 00:27:08.000000 kilosort-4.0.6/docs/tutorials/make_probe.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-27 00:27:08.000000 kilosort-4.0.6/docs/tutorials/tutorials.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:27:17.175471 kilosort-4.0.6/kilosort/
--rw-r--r--   0 runner    (1001) docker     (127)     3566 2024-04-27 00:27:08.000000 kilosort-4.0.6/kilosort/CCG.py
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-27 00:27:08.000000 kilosort-4.0.6/kilosort/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-27 00:27:08.000000 kilosort-4.0.6/kilosort/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8533 2024-04-27 00:27:08.000000 kilosort-4.0.6/kilosort/bench.py
--rw-r--r--   0 runner    (1001) docker     (127)    14963 2024-04-27 00:27:08.000000 kilosort-4.0.6/kilosort/clustering_qr.py
--rw-r--r--   0 runner    (1001) docker     (127)     7482 2024-04-27 00:27:08.000000 kilosort-4.0.6/kilosort/datashift.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:27:17.179471 kilosort-4.0.6/kilosort/gui/
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-27 00:27:08.000000 kilosort-4.0.6/kilosort/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13532 2024-04-27 00:27:08.000000 kilosort-4.0.6/kilosort/gui/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)    22103 2024-04-27 00:27:08.000000 kilosort-4.0.6/kilosort/gui/data_view_box.py
--rw-r--r--   0 runner    (1001) docker     (127)     3133 2024-04-27 00:27:08.000000 kilosort-4.0.6/kilosort/gui/header_box.py
--rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-04-27 00:27:08.000000 kilosort-4.0.6/kilosort/gui/launch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-27 00:27:08.000000 kilosort-4.0.6/kilosort/gui/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    21165 2024-04-27 00:27:08.000000 kilosort-4.0.6/kilosort/gui/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     4760 2024-04-27 00:27:08.000000 kilosort-4.0.6/kilosort/gui/message_log_box.py
--rw-r--r--   0 runner    (1001) docker     (127)     8854 2024-04-27 00:27:08.000000 kilosort-4.0.6/kilosort/gui/minor_gui_elements.py
--rw-r--r--   0 runner    (1001) docker     (127)     4846 2024-04-27 00:27:08.000000 kilosort-4.0.6/kilosort/gui/palettes.py
--rw-r--r--   0 runner    (1001) docker     (127)     8073 2024-04-27 00:27:08.000000 kilosort-4.0.6/kilosort/gui/probe_view_box.py
--rw-r--r--   0 runner    (1001) docker     (127)     7204 2024-04-27 00:27:08.000000 kilosort-4.0.6/kilosort/gui/run_box.py
--rw-r--r--   0 runner    (1001) docker     (127)     6000 2024-04-27 00:27:08.000000 kilosort-4.0.6/kilosort/gui/sanity_plots.py
--rw-r--r--   0 runner    (1001) docker     (127)    33239 2024-04-27 00:27:08.000000 kilosort-4.0.6/kilosort/gui/settings_box.py
--rw-r--r--   0 runner    (1001) docker     (127)     4011 2024-04-27 00:27:08.000000 kilosort-4.0.6/kilosort/gui/sorter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2816 2024-04-27 00:27:08.000000 kilosort-4.0.6/kilosort/hierarchical.py
--rw-r--r--   0 runner    (1001) docker     (127)    36620 2024-04-27 00:27:08.000000 kilosort-4.0.6/kilosort/io.py
--rw-r--r--   0 runner    (1001) docker     (127)    13376 2024-04-27 00:27:08.000000 kilosort-4.0.6/kilosort/parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     4223 2024-04-27 00:27:08.000000 kilosort-4.0.6/kilosort/postprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)     4827 2024-04-27 00:27:08.000000 kilosort-4.0.6/kilosort/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)    20479 2024-04-27 00:27:08.000000 kilosort-4.0.6/kilosort/run_kilosort.py
--rw-r--r--   0 runner    (1001) docker     (127)    60034 2024-04-27 00:27:08.000000 kilosort-4.0.6/kilosort/simulation.py
--rw-r--r--   0 runner    (1001) docker     (127)     8730 2024-04-27 00:27:08.000000 kilosort-4.0.6/kilosort/spikedetect.py
--rw-r--r--   0 runner    (1001) docker     (127)     4586 2024-04-27 00:27:08.000000 kilosort-4.0.6/kilosort/swarmsplitter.py
--rw-r--r--   0 runner    (1001) docker     (127)     8345 2024-04-27 00:27:08.000000 kilosort-4.0.6/kilosort/template_matching.py
--rw-r--r--   0 runner    (1001) docker     (127)     3429 2024-04-27 00:27:08.000000 kilosort-4.0.6/kilosort/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3432 2024-04-27 00:27:08.000000 kilosort-4.0.6/kilosort/wTEMP.npz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:27:17.179471 kilosort-4.0.6/kilosort.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10348 2024-04-27 00:27:17.000000 kilosort-4.0.6/kilosort.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-04-27 00:27:17.000000 kilosort-4.0.6/kilosort.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 00:27:17.000000 kilosort-4.0.6/kilosort.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-27 00:27:17.000000 kilosort-4.0.6/kilosort.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-27 00:27:17.000000 kilosort-4.0.6/kilosort.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-27 00:27:08.000000 kilosort-4.0.6/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 00:27:17.183471 kilosort-4.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-04-27 00:27:08.000000 kilosort-4.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 00:27:17.179471 kilosort-4.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     7887 2024-04-27 00:27:08.000000 kilosort-4.0.6/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3118 2024-04-27 00:27:08.000000 kilosort-4.0.6/tests/test_clustering.py
--rw-r--r--   0 runner    (1001) docker     (127)     2632 2024-04-27 00:27:08.000000 kilosort-4.0.6/tests/test_dtype.py
--rw-r--r--   0 runner    (1001) docker     (127)     2647 2024-04-27 00:27:08.000000 kilosort-4.0.6/tests/test_full_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     6400 2024-04-27 00:27:08.000000 kilosort-4.0.6/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-04-27 00:27:08.000000 kilosort-4.0.6/tests/test_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     7256 2024-04-27 00:27:08.000000 kilosort-4.0.6/tests/test_preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-27 00:27:08.000000 kilosort-4.0.6/tests/test_spikedetect.py
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-27 00:27:08.000000 kilosort-4.0.6/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:07:23.300179 kilosort-4.0.7/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:07:23.284179 kilosort-4.0.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:07:23.288179 kilosort-4.0.7/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-05-09 23:07:14.000000 kilosort-4.0.7/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-09 23:07:14.000000 kilosort-4.0.7/.github/ISSUE_TEMPLATE/feature_request.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-05-09 23:07:14.000000 kilosort-4.0.7/.github/ISSUE_TEMPLATE/installation_issue.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-09 23:07:14.000000 kilosort-4.0.7/.github/ISSUE_TEMPLATE/other.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:07:23.288179 kilosort-4.0.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-05-09 23:07:14.000000 kilosort-4.0.7/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-05-09 23:07:14.000000 kilosort-4.0.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-09 23:07:14.000000 kilosort-4.0.7/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3360 2024-05-09 23:07:14.000000 kilosort-4.0.7/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-09 23:07:14.000000 kilosort-4.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10348 2024-05-09 23:07:23.300179 kilosort-4.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8987 2024-05-09 23:07:14.000000 kilosort-4.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:07:23.292179 kilosort-4.0.7/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-09 23:07:14.000000 kilosort-4.0.7/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-09 23:07:14.000000 kilosort-4.0.7/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2892 2024-05-09 23:07:14.000000 kilosort-4.0.7/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6082 2024-05-09 23:07:14.000000 kilosort-4.0.7/docs/drift.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6710 2024-05-09 23:07:14.000000 kilosort-4.0.7/docs/gui_guide.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-05-09 23:07:14.000000 kilosort-4.0.7/docs/hardware.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-09 23:07:14.000000 kilosort-4.0.7/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-09 23:07:14.000000 kilosort-4.0.7/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-09 23:07:14.000000 kilosort-4.0.7/docs/multi_shank.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6080 2024-05-09 23:07:14.000000 kilosort-4.0.7/docs/parameters.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-09 23:07:14.000000 kilosort-4.0.7/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:07:23.292179 kilosort-4.0.7/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (127)     9953 2024-05-09 23:07:14.000000 kilosort-4.0.7/docs/tutorials/basic_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    13669 2024-05-09 23:07:14.000000 kilosort-4.0.7/docs/tutorials/load_data.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     8102 2024-05-09 23:07:14.000000 kilosort-4.0.7/docs/tutorials/make_probe.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-09 23:07:14.000000 kilosort-4.0.7/docs/tutorials/tutorials.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:07:23.296179 kilosort-4.0.7/kilosort/
+-rw-r--r--   0 runner    (1001) docker     (127)     3566 2024-05-09 23:07:14.000000 kilosort-4.0.7/kilosort/CCG.py
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-09 23:07:14.000000 kilosort-4.0.7/kilosort/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-09 23:07:14.000000 kilosort-4.0.7/kilosort/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8533 2024-05-09 23:07:14.000000 kilosort-4.0.7/kilosort/bench.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14893 2024-05-09 23:07:14.000000 kilosort-4.0.7/kilosort/clustering_qr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7482 2024-05-09 23:07:14.000000 kilosort-4.0.7/kilosort/datashift.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:07:23.296179 kilosort-4.0.7/kilosort/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-09 23:07:14.000000 kilosort-4.0.7/kilosort/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13532 2024-05-09 23:07:14.000000 kilosort-4.0.7/kilosort/gui/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22166 2024-05-09 23:07:14.000000 kilosort-4.0.7/kilosort/gui/data_view_box.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3133 2024-05-09 23:07:14.000000 kilosort-4.0.7/kilosort/gui/header_box.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-05-09 23:07:14.000000 kilosort-4.0.7/kilosort/gui/launch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-09 23:07:14.000000 kilosort-4.0.7/kilosort/gui/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21624 2024-05-09 23:07:14.000000 kilosort-4.0.7/kilosort/gui/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4760 2024-05-09 23:07:14.000000 kilosort-4.0.7/kilosort/gui/message_log_box.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8854 2024-05-09 23:07:14.000000 kilosort-4.0.7/kilosort/gui/minor_gui_elements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4846 2024-05-09 23:07:14.000000 kilosort-4.0.7/kilosort/gui/palettes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8073 2024-05-09 23:07:14.000000 kilosort-4.0.7/kilosort/gui/probe_view_box.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7204 2024-05-09 23:07:14.000000 kilosort-4.0.7/kilosort/gui/run_box.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6000 2024-05-09 23:07:14.000000 kilosort-4.0.7/kilosort/gui/sanity_plots.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33239 2024-05-09 23:07:14.000000 kilosort-4.0.7/kilosort/gui/settings_box.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4011 2024-05-09 23:07:14.000000 kilosort-4.0.7/kilosort/gui/sorter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2816 2024-05-09 23:07:14.000000 kilosort-4.0.7/kilosort/hierarchical.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37007 2024-05-09 23:07:14.000000 kilosort-4.0.7/kilosort/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13081 2024-05-09 23:07:14.000000 kilosort-4.0.7/kilosort/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4223 2024-05-09 23:07:14.000000 kilosort-4.0.7/kilosort/postprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4827 2024-05-09 23:07:14.000000 kilosort-4.0.7/kilosort/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21027 2024-05-09 23:07:14.000000 kilosort-4.0.7/kilosort/run_kilosort.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60034 2024-05-09 23:07:14.000000 kilosort-4.0.7/kilosort/simulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8730 2024-05-09 23:07:14.000000 kilosort-4.0.7/kilosort/spikedetect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4586 2024-05-09 23:07:14.000000 kilosort-4.0.7/kilosort/swarmsplitter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8295 2024-05-09 23:07:14.000000 kilosort-4.0.7/kilosort/template_matching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3429 2024-05-09 23:07:14.000000 kilosort-4.0.7/kilosort/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3432 2024-05-09 23:07:14.000000 kilosort-4.0.7/kilosort/wTEMP.npz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:07:23.300179 kilosort-4.0.7/kilosort.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10348 2024-05-09 23:07:23.000000 kilosort-4.0.7/kilosort.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-05-09 23:07:23.000000 kilosort-4.0.7/kilosort.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 23:07:23.000000 kilosort-4.0.7/kilosort.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-09 23:07:23.000000 kilosort-4.0.7/kilosort.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-09 23:07:23.000000 kilosort-4.0.7/kilosort.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-09 23:07:14.000000 kilosort-4.0.7/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 23:07:23.300179 kilosort-4.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-05-09 23:07:14.000000 kilosort-4.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:07:23.300179 kilosort-4.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7887 2024-05-09 23:07:14.000000 kilosort-4.0.7/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3118 2024-05-09 23:07:14.000000 kilosort-4.0.7/tests/test_clustering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2632 2024-05-09 23:07:14.000000 kilosort-4.0.7/tests/test_dtype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2647 2024-05-09 23:07:14.000000 kilosort-4.0.7/tests/test_full_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6400 2024-05-09 23:07:14.000000 kilosort-4.0.7/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-05-09 23:07:14.000000 kilosort-4.0.7/tests/test_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7256 2024-05-09 23:07:14.000000 kilosort-4.0.7/tests/test_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-09 23:07:14.000000 kilosort-4.0.7/tests/test_spikedetect.py
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-05-09 23:07:14.000000 kilosort-4.0.7/tox.ini
```

### Comparing `kilosort-4.0.6/.github/ISSUE_TEMPLATE/bug_report.yml` & `kilosort-4.0.7/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.6/.github/ISSUE_TEMPLATE/feature_request.yml` & `kilosort-4.0.7/.github/ISSUE_TEMPLATE/feature_request.yml`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.6/.github/ISSUE_TEMPLATE/installation_issue.yml` & `kilosort-4.0.7/.github/ISSUE_TEMPLATE/installation_issue.yml`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.6/.github/workflows/test_and_deploy.yml` & `kilosort-4.0.7/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.6/.gitignore` & `kilosort-4.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.6/.readthedocs.yml` & `kilosort-4.0.7/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.6/CODE_OF_CONDUCT.md` & `kilosort-4.0.7/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.6/LICENSE` & `kilosort-4.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.6/PKG-INFO` & `kilosort-4.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kilosort
-Version: 4.0.6
+Version: 4.0.7
 Summary: spike sorting pipeline
 Home-page: https://github.com/MouseLand/kilosort
 Author: Marius Pachitariu
 Author-email: pachitarium@janelia.hhmi.org
 License: BSD
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `kilosort-4.0.6/README.md` & `kilosort-4.0.7/README.md`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.6/docs/Makefile` & `kilosort-4.0.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.6/docs/conf.py` & `kilosort-4.0.7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.6/docs/drift.rst` & `kilosort-4.0.7/docs/drift.rst`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.6/docs/gui_guide.rst` & `kilosort-4.0.7/docs/gui_guide.rst`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.6/docs/hardware.rst` & `kilosort-4.0.7/docs/hardware.rst`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.6/docs/index.rst` & `kilosort-4.0.7/docs/index.rst`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.6/docs/make.bat` & `kilosort-4.0.7/docs/make.bat`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.6/docs/multi_shank.rst` & `kilosort-4.0.7/docs/multi_shank.rst`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.6/docs/parameters.rst` & `kilosort-4.0.7/docs/parameters.rst`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.6/docs/tutorials/basic_example.ipynb` & `kilosort-4.0.7/docs/tutorials/basic_example.ipynb`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.6/docs/tutorials/load_data.ipynb` & `kilosort-4.0.7/docs/tutorials/load_data.ipynb`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.6/docs/tutorials/make_probe.ipynb` & `kilosort-4.0.7/docs/tutorials/make_probe.ipynb`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.6/kilosort/CCG.py` & `kilosort-4.0.7/kilosort/CCG.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.6/kilosort/bench.py` & `kilosort-4.0.7/kilosort/bench.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.6/kilosort/clustering_qr.py` & `kilosort-4.0.7/kilosort/clustering_qr.py`

 * *Files 1% similar despite different names*

```diff
@@ -301,15 +301,14 @@
         xy, iC = xy_up(ops)
         iclust_template = st[:,5].astype('int32')
         xcup, ycup = ops['xcup'], ops['ycup']
 
     dmin = ops['dmin']
     dminx = ops['dminx']
     nskip = ops['settings']['cluster_downsampling']
-    ncomps = ops['settings']['cluster_pcs']
     ycent = y_centers(ops)
     xcent = x_centers(ops)
     nsp = st.shape[0]
 
     # Get positions of all grouping centers
     ycent_pos, xcent_pos = np.meshgrid(ycent, xcent)
     ycent_pos = torch.from_numpy(ycent_pos.flatten())
@@ -333,15 +332,15 @@
                    mininterval=10 if progress_bar else None):
         for jj in np.arange(len(xcent)):
             # Get data for all templates that were closest to this x,y center.
             ii = ii = kk + jj*ycent.size
             ix = (minimum_distance == ii)
             Xd, ch_min, ch_max, igood  = get_data_cpu(
                 ops, xy, iC, iclust_template, tF, ycent[kk], xcent[jj], dmin=dmin,
-                dminx=dminx, ncomps=ncomps, ix=ix
+                dminx=dminx, ix=ix
                 )
 
             if Xd is None:
                 nearby_chans_empty += 1
                 continue
             elif Xd.shape[0]<1000:
                 iclust = torch.zeros((Xd.shape[0],))
@@ -389,15 +388,15 @@
             'Wall is empty after `clustering_qr.run`, cannot continue clustering.'
         )
 
     return clu, Wall
 
 
 def get_data_cpu(ops, xy, iC, PID, tF, ycenter, xcenter, dmin=20, dminx=32,
-                 ncomps=64, ix=None, merge_dim=True):
+                 ix=None, merge_dim=True):
     PID =  torch.from_numpy(PID).long()
 
     #iU = ops['iU'].cpu().numpy()
     #iC = ops['iCC'][:, ops['iU']]    
     #xcup, ycup = ops['xc'][iU], ops['yc'][iU]
     #xy = np.vstack((xcup, ycup))
     #xy = torch.from_numpy(xy)
```

### Comparing `kilosort-4.0.6/kilosort/datashift.py` & `kilosort-4.0.7/kilosort/datashift.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.6/kilosort/gui/__init__.py` & `kilosort-4.0.7/kilosort/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.6/kilosort/gui/converter.py` & `kilosort-4.0.7/kilosort/gui/converter.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.6/kilosort/gui/data_view_box.py` & `kilosort-4.0.7/kilosort/gui/data_view_box.py`

 * *Files 1% similar despite different names*

```diff
@@ -555,25 +555,25 @@
             filt_binary_file,
             to_display,
             start_time,
             end_time
     ):
 
         if self.raw_button.isChecked():
-            colormap_min, colormap_max = -32.0, 32.0
             raw_traces = binary_file[start_time:end_time].cpu().numpy()
+            colormap_min = np.percentile(raw_traces, 0.5)
+            colormap_max = np.percentile(raw_traces, 99.5)
             self.add_image_to_plot(
                 raw_traces[to_display, :].T,
                 colormap_min,
                 colormap_max,
             )
 
         elif self.whitened_button.isChecked():
             whitened_traces = filt_binary_file[start_time:end_time].cpu().numpy()
-
             colormap_min, colormap_max = -4.0, 4.0
             self.add_image_to_plot(
                 whitened_traces[to_display, :].T,
                 colormap_min,
                 colormap_max,
             )
```

### Comparing `kilosort-4.0.6/kilosort/gui/header_box.py` & `kilosort-4.0.7/kilosort/gui/header_box.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.6/kilosort/gui/launch.py` & `kilosort-4.0.7/kilosort/gui/launch.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.6/kilosort/gui/logger.py` & `kilosort-4.0.7/kilosort/gui/logger.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.6/kilosort/gui/main.py` & `kilosort-4.0.7/kilosort/gui/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -233,14 +233,21 @@
                 )
             self.settings_message_splitter.restoreState(
                 self.qt_settings.value('settings_message_splitter')
                 )
             self.left_right_splitter.restoreState(
                 self.qt_settings.value('left_right_splitter')
                 )
+        else:
+            # Default to 25/75 split for left/right, 50/50 for settings/probe
+            # NOTE: The large values are used so that QT will divide the extra
+            #       pixels proportionally between the split widgets, which is
+            #       much simpler than figuring out the exact pixel positions.
+            self.left_right_splitter.setSizes([250000, 750000])
+            self.settings_probe_splitter.setSizes([500000, 500000])
 
         # Connect signals
         self.header_box.reset_gui_button.clicked.connect(self.reset_gui)
         self.settings_box.settingsUpdated.connect(self.load_data)
         self.settings_box.previewProbe.connect(self.probe_view_box.preview_probe)
         # Don't allow spike sorting to run until new data has actually
         # been loaded.
```

### Comparing `kilosort-4.0.6/kilosort/gui/message_log_box.py` & `kilosort-4.0.7/kilosort/gui/message_log_box.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.6/kilosort/gui/minor_gui_elements.py` & `kilosort-4.0.7/kilosort/gui/minor_gui_elements.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.6/kilosort/gui/palettes.py` & `kilosort-4.0.7/kilosort/gui/palettes.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.6/kilosort/gui/probe_view_box.py` & `kilosort-4.0.7/kilosort/gui/probe_view_box.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.6/kilosort/gui/run_box.py` & `kilosort-4.0.7/kilosort/gui/run_box.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.6/kilosort/gui/sanity_plots.py` & `kilosort-4.0.7/kilosort/gui/sanity_plots.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     # Amplitude of spike over time and depth
     p1 = plot_window.plot_widget.addPlot(
         row=0, col=0, labels={'left': 'Depth (um)', 'bottom': 'Time (s)'}
     )
     p1.setTitle('Spike amplitude across time and depth', color='black')
 
     x = st0[:,0]  # spike time in seconds
-    y = st0[:,5]  # depth of spike center in microns
+    y = st0[:,1]  # depth of spike center in microns
     z = st0[:,2]  # spike amplitude (data)
     z[z < 10] = 10
     z[z > 100] = 100
 
     bin_idx = np.digitize(z, np.logspace(1, 2, 90))
     cm = matplotlib.colormaps['binary']
     brushes = np.empty_like(z, dtype=object)
```

### Comparing `kilosort-4.0.6/kilosort/gui/settings_box.py` & `kilosort-4.0.7/kilosort/gui/settings_box.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.6/kilosort/gui/sorter.py` & `kilosort-4.0.7/kilosort/gui/sorter.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.6/kilosort/hierarchical.py` & `kilosort-4.0.7/kilosort/hierarchical.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.6/kilosort/io.py` & `kilosort-4.0.7/kilosort/io.py`

 * *Files 1% similar despite different names*

```diff
@@ -153,21 +153,26 @@
 
     # probe properties
     chan_map = probe['chanMap']
     channel_positions = np.stack((probe['xc'], probe['yc']), axis=-1)
     np.save((results_dir / 'channel_map.npy'), chan_map)
     np.save((results_dir / 'channel_positions.npy'), channel_positions)
 
-    # whitening matrix ** saving real whitening matrix doesn't work with phy currently
-    whitening_mat = ops['Wrot'].cpu().numpy()
-    np.save((results_dir / 'whitening_mat_dat.npy'), whitening_mat)
-    whitening_mat = 0.005 * np.eye(len(chan_map), dtype='float32')
-    whitening_mat_inv = np.linalg.inv(whitening_mat + 1e-5 * np.eye(whitening_mat.shape[0]))
-    np.save((results_dir / 'whitening_mat.npy'), whitening_mat)
-    np.save((results_dir / 'whitening_mat_inv.npy'), whitening_mat_inv)
+    # whitening matrix
+    whitening_mat = ops['Wrot']
+    np.save((results_dir / 'whitening_mat_dat.npy'), whitening_mat.cpu())
+    # NOTE: commented out for reference, this was different in KS 2.5 because
+    #       the binary file was already whitened.
+    # whitening_mat = 0.005 * np.eye(len(chan_map), dtype='float32')
+    whitening_mat_inv = torch.inverse(
+        whitening_mat
+        + 1e-5 * torch.eye(whitening_mat.shape[0]).to(whitening_mat.device)
+        )
+    np.save((results_dir / 'whitening_mat.npy'), whitening_mat.cpu())
+    np.save((results_dir / 'whitening_mat_inv.npy'), whitening_mat_inv.cpu())
 
     # spike properties
     spike_times = st[:,0].astype('int64') + imin  # shift by minimum sample index
     spike_templates = st[:,1].astype('int32')
     spike_clusters = clu
     xs, ys = compute_spike_positions(st, tF, ops)
     spike_positions = np.vstack([xs, ys]).T
@@ -500,16 +505,20 @@
         if self.file is None:
             raise ValueError('Binary file has been closed, data not accessible.')
 
         if ibatch==0:
             bstart = self.imin
             bend = self.imin + self.NT + self.nt
         else:
-            bstart = self.imin + (ibatch * self.NT) - self.nt
-            bend = min(self.imax, bstart + self.NT + 2*self.nt)
+            # Casting to uint64 is to prevent overflow for long recordings.
+            # It's done multiple times because python is stubborn about
+            # switching things back to default types.
+            ibatch = np.uint64(ibatch)
+            bstart = np.uint64(self.imin + (ibatch * self.NT) - self.nt)
+            bend = min(self.imax, np.uint64(bstart + self.NT + 2*self.nt))
         data = self.file[bstart : bend]
         data = data.T
         # Shift data to +/- 2**15
         if self.dtype == 'uint16':
             data = data.astype('float32')
             data = data - 2**15
```

### Comparing `kilosort-4.0.6/kilosort/parameters.py` & `kilosort-4.0.7/kilosort/parameters.py`

 * *Files 2% similar despite different names*

```diff
@@ -317,23 +317,14 @@
         'description':
             """
             Inverse fraction of nodes used as landmarks during clustering
             (can be 1, but that slows down the optimization). 
             """
     },
 
-    'cluster_pcs': {
-        'gui_name': 'cluster pcs', 'type': int, 'min': 1, 'max': np.inf,
-        'exclude': [], 'default': 64, 'step': 'clustering',
-        'description':
-            """
-            Maximum number of spatiotemporal PC features used for clustering.
-            """
-    },
-
     'x_centers': {
         'gui_name': 'x centers', 'type': int, 'min': 1,
         'max': np.inf, 'exclude': [], 'default': None, 'step': 'clustering',
         'description':
             """
             Number of x-positions to use when determining center points for
             template groupings. If None, this will be determined automatically
```

### Comparing `kilosort-4.0.6/kilosort/postprocessing.py` & `kilosort-4.0.7/kilosort/postprocessing.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.6/kilosort/preprocessing.py` & `kilosort-4.0.7/kilosort/preprocessing.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.6/kilosort/run_kilosort.py` & `kilosort-4.0.7/kilosort/run_kilosort.py`

 * *Files 1% similar despite different names*

```diff
@@ -195,14 +195,19 @@
         elif 'probe_path' in settings: probe_path = Path(settings['probe_path']).resolve()
         else: raise ValueError('no probe_name or probe_path provided, set probe_name=')
         if not probe_path.exists():
             raise FileExistsError(f"probe_path '{probe_path}' does not exist")
         
         probe  = io.load_probe(probe_path)
         print(f"using probe {probe_path.name}")
+    else:
+        # Make sure xc, yc are float32, otherwise there are casting problems
+        # with some pytorch functions.
+        probe['xc'] = probe['xc'].astype(np.float32)
+        probe['yc'] = probe['yc'].astype(np.float32)
 
     return filename, data_dir, results_dir, probe
 
 
 def initialize_ops(settings, probe, data_dtype, do_CAR, invert_sign, device) -> dict:
     """Package settings and probe information into a single `ops` dictionary."""
 
@@ -413,14 +418,22 @@
     tic = time.time()
     print('\nExtracting spikes using cluster waveforms')
     st, tF, ops = template_matching.extract(ops, bfile, Wall3, device=device,
                                                  progress_bar=progress_bar)
     print(f'{len(st)} spikes extracted in {time.time()-tic : .2f}s; ' +
             f'total {time.time()-tic0 : .2f}s')
 
+    negative_spikes = (st[:,0] < 0).sum()
+    if negative_spikes > 0:
+        print(
+            f'{negative_spikes} spikes with negative spike times were detected.\n'
+            'We are aware of an issue causing this to happen for a small number '
+            'of spikes, and are working on a fix.'
+            )
+
     return st, tF, Wall, clu
 
 
 def cluster_spikes(st, tF, ops, device, bfile, tic0=np.nan, progress_bar=None):
     tic = time.time()
     print('\nFinal clustering')
     clu, Wall = clustering_qr.run(ops, st, tF,  mode = 'template', device=device,
```

### Comparing `kilosort-4.0.6/kilosort/simulation.py` & `kilosort-4.0.7/kilosort/simulation.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.6/kilosort/spikedetect.py` & `kilosort-4.0.7/kilosort/spikedetect.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.6/kilosort/swarmsplitter.py` & `kilosort-4.0.7/kilosort/swarmsplitter.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.6/kilosort/template_matching.py` & `kilosort-4.0.7/kilosort/template_matching.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,16 +41,15 @@
         nsp = len(stt)   
         if k+nsp>st.shape[0]:                     
             st = np.concatenate((st, np.zeros_like(st)), 0)
             tF  = torch.cat((tF,  torch.zeros_like(tF)), 0)
 
         stt = stt.double()
         #st[k:k+nsp,0] = ((stt[:,0]-nt)/ops['fs'] + ibatch * (ops['batch_size']/ops['fs'])).cpu().numpy()
-        left_pad = 0 if ibatch == 0 else nt
-        st[k:k+nsp,0] = ((stt[:,0]-left_pad) + ibatch * (ops['batch_size'])).cpu().numpy() - nt//2 + ops['nt0min']
+        st[k:k+nsp,0] = ((stt[:,0]-nt) + ibatch * (ops['batch_size'])).cpu().numpy() - nt//2 + ops['nt0min']
 
         st[k:k+nsp,1] = stt[:,1].cpu().numpy()
         st[k:k+nsp,2] = amps[:,0].cpu().numpy()
         
         tF[k:k+nsp]  = xfeat.transpose(0,1).cpu()#.numpy()
 
         k+= nsp
```

### Comparing `kilosort-4.0.6/kilosort/utils.py` & `kilosort-4.0.7/kilosort/utils.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.6/kilosort/wTEMP.npz` & `kilosort-4.0.7/kilosort/wTEMP.npz`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.6/kilosort.egg-info/PKG-INFO` & `kilosort-4.0.7/kilosort.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kilosort
-Version: 4.0.6
+Version: 4.0.7
 Summary: spike sorting pipeline
 Home-page: https://github.com/MouseLand/kilosort
 Author: Marius Pachitariu
 Author-email: pachitarium@janelia.hhmi.org
 License: BSD
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `kilosort-4.0.6/kilosort.egg-info/SOURCES.txt` & `kilosort-4.0.7/kilosort.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.6/setup.py` & `kilosort-4.0.7/setup.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.6/tests/conftest.py` & `kilosort-4.0.7/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.6/tests/test_clustering.py` & `kilosort-4.0.7/tests/test_clustering.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.6/tests/test_dtype.py` & `kilosort-4.0.7/tests/test_dtype.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.6/tests/test_full_pipeline.py` & `kilosort-4.0.7/tests/test_full_pipeline.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.6/tests/test_io.py` & `kilosort-4.0.7/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.6/tests/test_parameters.py` & `kilosort-4.0.7/tests/test_parameters.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.6/tests/test_preprocessing.py` & `kilosort-4.0.7/tests/test_preprocessing.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.6/tox.ini` & `kilosort-4.0.7/tox.ini`

 * *Files identical despite different names*

