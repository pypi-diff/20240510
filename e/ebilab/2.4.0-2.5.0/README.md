# Comparing `tmp/ebilab-2.4.0.tar.gz` & `tmp/ebilab-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ebilab-2.4.0.tar", last modified: Thu Apr 11 10:04:27 2024, max compression
+gzip compressed data, was "ebilab-2.5.0.tar", last modified: Fri May 10 06:32:57 2024, max compression
```

## Comparing `ebilab-2.4.0.tar` & `ebilab-2.5.0.tar`

### file list

```diff
@@ -1,116 +1,116 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:04:27.075173 ebilab-2.4.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:04:27.055173 ebilab-2.4.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:04:27.063173 ebilab-2.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-11 10:04:17.000000 ebilab-2.4.0/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-11 10:04:17.000000 ebilab-2.4.0/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3322 2024-04-11 10:04:17.000000 ebilab-2.4.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-11 10:04:17.000000 ebilab-2.4.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-11 10:04:17.000000 ebilab-2.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-11 10:04:17.000000 ebilab-2.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-11 10:04:17.000000 ebilab-2.4.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-11 10:04:27.075173 ebilab-2.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-04-11 10:04:17.000000 ebilab-2.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:04:27.063173 ebilab-2.4.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-04-11 10:04:17.000000 ebilab-2.4.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-11 10:04:17.000000 ebilab-2.4.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-11 10:04:17.000000 ebilab-2.4.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:04:27.063173 ebilab-2.4.0/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:04:27.063173 ebilab-2.4.0/docs/source/api/
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-11 10:04:17.000000 ebilab-2.4.0/docs/source/api/ebilab.analysis.rst
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-11 10:04:17.000000 ebilab-2.4.0/docs/source/api/ebilab.experiment.devices.rst
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-11 10:04:17.000000 ebilab-2.4.0/docs/source/api/ebilab.experiment.devices.visa.rst
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-11 10:04:17.000000 ebilab-2.4.0/docs/source/api/ebilab.experiment.rst
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-11 10:04:17.000000 ebilab-2.4.0/docs/source/api/ebilab.project.rst
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-11 10:04:17.000000 ebilab-2.4.0/docs/source/api/ebilab.rst
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-11 10:04:17.000000 ebilab-2.4.0/docs/source/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4400 2024-04-11 10:04:17.000000 ebilab-2.4.0/docs/source/changelog-v2.0.0-pre.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5101 2024-04-11 10:04:17.000000 ebilab-2.4.0/docs/source/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-04-11 10:04:17.000000 ebilab-2.4.0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      853 2024-04-11 10:04:17.000000 ebilab-2.4.0/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-11 10:04:17.000000 ebilab-2.4.0/docs/source/installation.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:04:27.059173 ebilab-2.4.0/docs/source/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:04:27.059173 ebilab-2.4.0/docs/source/locale/en/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:04:27.067173 ebilab-2.4.0/docs/source/locale/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    12691 2024-04-11 10:04:17.000000 ebilab-2.4.0/docs/source/locale/en/LC_MESSAGES/api.po
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-04-11 10:04:17.000000 ebilab-2.4.0/docs/source/locale/en/LC_MESSAGES/changelog.po
--rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-04-11 10:04:17.000000 ebilab-2.4.0/docs/source/locale/en/LC_MESSAGES/index.po
--rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-04-11 10:04:17.000000 ebilab-2.4.0/docs/source/locale/en/LC_MESSAGES/installation.po
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-11 10:04:17.000000 ebilab-2.4.0/docs/source/locale/en/LC_MESSAGES/modules.po
--rw-r--r--   0 runner    (1001) docker     (127)    14754 2024-04-11 10:04:17.000000 ebilab-2.4.0/docs/source/locale/en/LC_MESSAGES/tutorial.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:04:27.067173 ebilab-2.4.0/docs/source/tutorial/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-11 10:04:17.000000 ebilab-2.4.0/docs/source/tutorial/analysis.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5886 2024-04-11 10:04:17.000000 ebilab-2.4.0/docs/source/tutorial/experiment.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-11 10:04:17.000000 ebilab-2.4.0/docs/source/tutorial/experiment_device.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3004 2024-04-11 10:04:17.000000 ebilab-2.4.0/docs/source/tutorial/version.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:04:27.067173 ebilab-2.4.0/ebilab/
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-11 10:04:17.000000 ebilab-2.4.0/ebilab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-11 10:04:17.000000 ebilab-2.4.0/ebilab/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5457 2024-04-11 10:04:17.000000 ebilab-2.4.0/ebilab/_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:04:27.067173 ebilab-2.4.0/ebilab/analysis/
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-11 10:04:17.000000 ebilab-2.4.0/ebilab/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-11 10:04:17.000000 ebilab-2.4.0/ebilab/analysis/_actions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-04-11 10:04:17.000000 ebilab-2.4.0/ebilab/analysis/_preprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)     4967 2024-04-11 10:04:17.000000 ebilab-2.4.0/ebilab/analysis/_process.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:04:27.059173 ebilab-2.4.0/ebilab/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:04:27.071174 ebilab-2.4.0/ebilab/data/project-template/
--rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-04-11 10:04:17.000000 ebilab-2.4.0/ebilab/data/project-template/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:04:27.059173 ebilab-2.4.0/ebilab/data/project-template/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:04:27.071174 ebilab-2.4.0/ebilab/data/project-template/data/input/
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-11 10:04:17.000000 ebilab-2.4.0/ebilab/data/project-template/data/input/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:04:27.071174 ebilab-2.4.0/ebilab/data/project-template/data/original/
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-11 10:04:17.000000 ebilab-2.4.0/ebilab/data/project-template/data/original/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:04:27.071174 ebilab-2.4.0/ebilab/data/project-template/data/output/
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-11 10:04:17.000000 ebilab-2.4.0/ebilab/data/project-template/data/output/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:04:27.071174 ebilab-2.4.0/ebilab/data/project-template/data/plot/
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-11 10:04:17.000000 ebilab-2.4.0/ebilab/data/project-template/data/plot/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 10:04:17.000000 ebilab-2.4.0/ebilab/data/project-template/ebilab.ini
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 10:04:17.000000 ebilab-2.4.0/ebilab/data/project-template/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:04:27.071174 ebilab-2.4.0/ebilab/experiment/
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-11 10:04:17.000000 ebilab-2.4.0/ebilab/experiment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9941 2024-04-11 10:04:17.000000 ebilab-2.4.0/ebilab/experiment/_experiment_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)    22180 2024-04-11 10:04:17.000000 ebilab-2.4.0/ebilab/experiment/_ui_tkinter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:04:27.071174 ebilab-2.4.0/ebilab/experiment/devices/
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-11 10:04:17.000000 ebilab-2.4.0/ebilab/experiment/devices/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:04:27.071174 ebilab-2.4.0/ebilab/experiment/devices/_visa/
--rw-r--r--   0 runner    (1001) docker     (127)      724 2024-04-11 10:04:17.000000 ebilab-2.4.0/ebilab/experiment/devices/_visa/A707.py
--rw-r--r--   0 runner    (1001) docker     (127)     2521 2024-04-11 10:04:17.000000 ebilab-2.4.0/ebilab/experiment/devices/_visa/E4980.py
--rw-r--r--   0 runner    (1001) docker     (127)     2981 2024-04-11 10:04:17.000000 ebilab-2.4.0/ebilab/experiment/devices/_visa/K34411A.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 10:04:17.000000 ebilab-2.4.0/ebilab/experiment/devices/_visa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4406 2024-04-11 10:04:17.000000 ebilab-2.4.0/ebilab/experiment/devices/visa.py
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-11 10:04:17.000000 ebilab-2.4.0/ebilab/experiment/options.py
--rw-r--r--   0 runner    (1001) docker     (127)    20598 2024-04-11 10:04:17.000000 ebilab-2.4.0/ebilab/icon.ico
--rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-04-11 10:04:17.000000 ebilab-2.4.0/ebilab/project.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:04:27.075173 ebilab-2.4.0/ebilab.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-11 10:04:26.000000 ebilab-2.4.0/ebilab.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-04-11 10:04:27.000000 ebilab-2.4.0/ebilab.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 10:04:26.000000 ebilab-2.4.0/ebilab.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-11 10:04:26.000000 ebilab-2.4.0/ebilab.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-11 10:04:26.000000 ebilab-2.4.0/ebilab.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-11 10:04:26.000000 ebilab-2.4.0/ebilab.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-11 10:04:17.000000 ebilab-2.4.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:04:27.071174 ebilab-2.4.0/sample/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-11 10:04:17.000000 ebilab-2.4.0/sample/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-11 10:04:17.000000 ebilab-2.4.0/sample/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-11 10:04:17.000000 ebilab-2.4.0/sample/cont_r.py
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-11 10:04:17.000000 ebilab-2.4.0/sample/multimeter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2916 2024-04-11 10:04:17.000000 ebilab-2.4.0/sample/random-walk.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:04:27.075173 ebilab-2.4.0/sample/recipes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 10:04:17.000000 ebilab-2.4.0/sample/recipes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-11 10:04:17.000000 ebilab-2.4.0/sample/recipes/do-nothing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-04-11 10:04:17.000000 ebilab-2.4.0/sample/recipes/random-walk.py
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-11 10:04:17.000000 ebilab-2.4.0/sample/voltage.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 10:04:27.075173 ebilab-2.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-04-11 10:04:17.000000 ebilab-2.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:04:27.075173 ebilab-2.4.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:04:27.075173 ebilab-2.4.0/tests/sample/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:04:27.059173 ebilab-2.4.0/tests/sample/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:04:27.075173 ebilab-2.4.0/tests/sample/data/input/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 10:04:17.000000 ebilab-2.4.0/tests/sample/data/input/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:04:27.075173 ebilab-2.4.0/tests/sample/data/original/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 10:04:17.000000 ebilab-2.4.0/tests/sample/data/original/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:04:27.075173 ebilab-2.4.0/tests/sample/data/output/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 10:04:17.000000 ebilab-2.4.0/tests/sample/data/output/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 10:04:17.000000 ebilab-2.4.0/tests/sample/ebilab.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:04:27.075173 ebilab-2.4.0/tests/sample/other_dir/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 10:04:17.000000 ebilab-2.4.0/tests/sample/other_dir/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-11 10:04:17.000000 ebilab-2.4.0/tests/test_paths.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:32:57.304190 ebilab-2.5.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:32:57.288190 ebilab-2.5.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:32:57.292190 ebilab-2.5.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-10 06:32:46.000000 ebilab-2.5.0/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-10 06:32:46.000000 ebilab-2.5.0/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3322 2024-05-10 06:32:46.000000 ebilab-2.5.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-10 06:32:46.000000 ebilab-2.5.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-10 06:32:46.000000 ebilab-2.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-10 06:32:46.000000 ebilab-2.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-10 06:32:46.000000 ebilab-2.5.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-10 06:32:57.304190 ebilab-2.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-05-10 06:32:46.000000 ebilab-2.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:32:57.292190 ebilab-2.5.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-05-10 06:32:46.000000 ebilab-2.5.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-10 06:32:46.000000 ebilab-2.5.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-10 06:32:46.000000 ebilab-2.5.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:32:57.292190 ebilab-2.5.0/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:32:57.292190 ebilab-2.5.0/docs/source/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-10 06:32:46.000000 ebilab-2.5.0/docs/source/api/ebilab.analysis.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-10 06:32:46.000000 ebilab-2.5.0/docs/source/api/ebilab.experiment.devices.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-10 06:32:46.000000 ebilab-2.5.0/docs/source/api/ebilab.experiment.devices.visa.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-10 06:32:46.000000 ebilab-2.5.0/docs/source/api/ebilab.experiment.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-10 06:32:46.000000 ebilab-2.5.0/docs/source/api/ebilab.project.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-10 06:32:46.000000 ebilab-2.5.0/docs/source/api/ebilab.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-10 06:32:46.000000 ebilab-2.5.0/docs/source/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4400 2024-05-10 06:32:46.000000 ebilab-2.5.0/docs/source/changelog-v2.0.0-pre.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5297 2024-05-10 06:32:46.000000 ebilab-2.5.0/docs/source/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-05-10 06:32:46.000000 ebilab-2.5.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-05-10 06:32:46.000000 ebilab-2.5.0/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-10 06:32:46.000000 ebilab-2.5.0/docs/source/installation.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:32:57.288190 ebilab-2.5.0/docs/source/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:32:57.288190 ebilab-2.5.0/docs/source/locale/en/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:32:57.296190 ebilab-2.5.0/docs/source/locale/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    12691 2024-05-10 06:32:46.000000 ebilab-2.5.0/docs/source/locale/en/LC_MESSAGES/api.po
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-05-10 06:32:46.000000 ebilab-2.5.0/docs/source/locale/en/LC_MESSAGES/changelog.po
+-rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-05-10 06:32:46.000000 ebilab-2.5.0/docs/source/locale/en/LC_MESSAGES/index.po
+-rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-05-10 06:32:46.000000 ebilab-2.5.0/docs/source/locale/en/LC_MESSAGES/installation.po
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-10 06:32:46.000000 ebilab-2.5.0/docs/source/locale/en/LC_MESSAGES/modules.po
+-rw-r--r--   0 runner    (1001) docker     (127)    14754 2024-05-10 06:32:46.000000 ebilab-2.5.0/docs/source/locale/en/LC_MESSAGES/tutorial.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:32:57.296190 ebilab-2.5.0/docs/source/tutorial/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-10 06:32:46.000000 ebilab-2.5.0/docs/source/tutorial/analysis.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5886 2024-05-10 06:32:46.000000 ebilab-2.5.0/docs/source/tutorial/experiment.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-10 06:32:46.000000 ebilab-2.5.0/docs/source/tutorial/experiment_device.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3004 2024-05-10 06:32:46.000000 ebilab-2.5.0/docs/source/tutorial/version.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:32:57.296190 ebilab-2.5.0/ebilab/
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-10 06:32:46.000000 ebilab-2.5.0/ebilab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-10 06:32:46.000000 ebilab-2.5.0/ebilab/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5457 2024-05-10 06:32:46.000000 ebilab-2.5.0/ebilab/_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:32:57.296190 ebilab-2.5.0/ebilab/analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-10 06:32:46.000000 ebilab-2.5.0/ebilab/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-05-10 06:32:46.000000 ebilab-2.5.0/ebilab/analysis/_actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-05-10 06:32:46.000000 ebilab-2.5.0/ebilab/analysis/_preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4967 2024-05-10 06:32:46.000000 ebilab-2.5.0/ebilab/analysis/_process.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:32:57.288190 ebilab-2.5.0/ebilab/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:32:57.296190 ebilab-2.5.0/ebilab/data/project-template/
+-rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-05-10 06:32:46.000000 ebilab-2.5.0/ebilab/data/project-template/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:32:57.288190 ebilab-2.5.0/ebilab/data/project-template/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:32:57.300190 ebilab-2.5.0/ebilab/data/project-template/data/input/
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-10 06:32:46.000000 ebilab-2.5.0/ebilab/data/project-template/data/input/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:32:57.300190 ebilab-2.5.0/ebilab/data/project-template/data/original/
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-10 06:32:46.000000 ebilab-2.5.0/ebilab/data/project-template/data/original/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:32:57.300190 ebilab-2.5.0/ebilab/data/project-template/data/output/
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-10 06:32:46.000000 ebilab-2.5.0/ebilab/data/project-template/data/output/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:32:57.300190 ebilab-2.5.0/ebilab/data/project-template/data/plot/
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-10 06:32:46.000000 ebilab-2.5.0/ebilab/data/project-template/data/plot/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 06:32:46.000000 ebilab-2.5.0/ebilab/data/project-template/ebilab.ini
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 06:32:46.000000 ebilab-2.5.0/ebilab/data/project-template/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:32:57.300190 ebilab-2.5.0/ebilab/experiment/
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-10 06:32:46.000000 ebilab-2.5.0/ebilab/experiment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9941 2024-05-10 06:32:46.000000 ebilab-2.5.0/ebilab/experiment/_experiment_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22180 2024-05-10 06:32:46.000000 ebilab-2.5.0/ebilab/experiment/_ui_tkinter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:32:57.300190 ebilab-2.5.0/ebilab/experiment/devices/
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-10 06:32:46.000000 ebilab-2.5.0/ebilab/experiment/devices/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:32:57.300190 ebilab-2.5.0/ebilab/experiment/devices/_visa/
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-05-10 06:32:46.000000 ebilab-2.5.0/ebilab/experiment/devices/_visa/A707.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2521 2024-05-10 06:32:46.000000 ebilab-2.5.0/ebilab/experiment/devices/_visa/E4980.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4002 2024-05-10 06:32:46.000000 ebilab-2.5.0/ebilab/experiment/devices/_visa/K34411A.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 06:32:46.000000 ebilab-2.5.0/ebilab/experiment/devices/_visa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4406 2024-05-10 06:32:46.000000 ebilab-2.5.0/ebilab/experiment/devices/visa.py
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-05-10 06:32:46.000000 ebilab-2.5.0/ebilab/experiment/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20598 2024-05-10 06:32:46.000000 ebilab-2.5.0/ebilab/icon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-05-10 06:32:46.000000 ebilab-2.5.0/ebilab/project.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:32:57.304190 ebilab-2.5.0/ebilab.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-10 06:32:57.000000 ebilab-2.5.0/ebilab.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2472 2024-05-10 06:32:57.000000 ebilab-2.5.0/ebilab.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 06:32:57.000000 ebilab-2.5.0/ebilab.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-10 06:32:57.000000 ebilab-2.5.0/ebilab.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-10 06:32:57.000000 ebilab-2.5.0/ebilab.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-10 06:32:57.000000 ebilab-2.5.0/ebilab.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-10 06:32:46.000000 ebilab-2.5.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:32:57.300190 ebilab-2.5.0/sample/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-10 06:32:46.000000 ebilab-2.5.0/sample/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-10 06:32:46.000000 ebilab-2.5.0/sample/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-10 06:32:46.000000 ebilab-2.5.0/sample/cont_r.py
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-10 06:32:46.000000 ebilab-2.5.0/sample/multimeter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2916 2024-05-10 06:32:46.000000 ebilab-2.5.0/sample/random-walk.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:32:57.300190 ebilab-2.5.0/sample/recipes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 06:32:46.000000 ebilab-2.5.0/sample/recipes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-10 06:32:46.000000 ebilab-2.5.0/sample/recipes/do-nothing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-05-10 06:32:46.000000 ebilab-2.5.0/sample/recipes/random-walk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-10 06:32:46.000000 ebilab-2.5.0/sample/voltage.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 06:32:57.304190 ebilab-2.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-05-10 06:32:46.000000 ebilab-2.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:32:57.300190 ebilab-2.5.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:32:57.300190 ebilab-2.5.0/tests/sample/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:32:57.288190 ebilab-2.5.0/tests/sample/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:32:57.304190 ebilab-2.5.0/tests/sample/data/input/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 06:32:46.000000 ebilab-2.5.0/tests/sample/data/input/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:32:57.304190 ebilab-2.5.0/tests/sample/data/original/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 06:32:46.000000 ebilab-2.5.0/tests/sample/data/original/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:32:57.304190 ebilab-2.5.0/tests/sample/data/output/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 06:32:46.000000 ebilab-2.5.0/tests/sample/data/output/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 06:32:46.000000 ebilab-2.5.0/tests/sample/ebilab.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:32:57.304190 ebilab-2.5.0/tests/sample/other_dir/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 06:32:46.000000 ebilab-2.5.0/tests/sample/other_dir/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-10 06:32:46.000000 ebilab-2.5.0/tests/test_paths.py
```

### Comparing `ebilab-2.4.0/.gitignore` & `ebilab-2.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `ebilab-2.4.0/LICENSE` & `ebilab-2.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ebilab-2.4.0/PKG-INFO` & `ebilab-2.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ebilab
-Version: 2.4.0
+Version: 2.5.0
 Summary: Python package for my research
 Home-page: https://ebilab.readthedocs.io/
 Author: Yusuke Ebihara
 Author-email: yusuke@ebihara.me
 Project-URL: GitHub repository, https://github.com/ebiyuu1121/ebilab
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ebilab-2.4.0/README.md` & `ebilab-2.5.0/README.md`

 * *Files identical despite different names*

### Comparing `ebilab-2.4.0/docs/Makefile` & `ebilab-2.5.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ebilab-2.4.0/docs/make.bat` & `ebilab-2.5.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ebilab-2.4.0/docs/source/api/ebilab.analysis.rst` & `ebilab-2.5.0/docs/source/api/ebilab.analysis.rst`

 * *Files identical despite different names*

### Comparing `ebilab-2.4.0/docs/source/changelog-v2.0.0-pre.rst` & `ebilab-2.5.0/docs/source/changelog-v2.0.0-pre.rst`

 * *Files identical despite different names*

### Comparing `ebilab-2.4.0/docs/source/conf.py` & `ebilab-2.5.0/docs/source/conf.py`

 * *Files 13% similar despite different names*

```diff
@@ -34,10 +34,11 @@
 
 extensions = [
     'sphinx.ext.autodoc',  # ソースコード読み込み用
     'sphinx.ext.viewcode',  # ハイライト済みのソースコードへのリンクを追加
     'sphinx.ext.todo',  # ToDoアイテムのサポート
     'sphinx.ext.napoleon', #googleスタイルやNumpyスタイルでdocstringを記述した際に必要
     'sphinx.ext.autosummary',
+    'myst_parser', # for markdown
 ]
 
 autosummary_generate = False
```

### Comparing `ebilab-2.4.0/docs/source/index.rst` & `ebilab-2.5.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `ebilab-2.4.0/docs/source/installation.rst` & `ebilab-2.5.0/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `ebilab-2.4.0/docs/source/locale/en/LC_MESSAGES/api.po` & `ebilab-2.5.0/docs/source/locale/en/LC_MESSAGES/api.po`

 * *Files identical despite different names*

### Comparing `ebilab-2.4.0/docs/source/locale/en/LC_MESSAGES/changelog.po` & `ebilab-2.5.0/docs/source/locale/en/LC_MESSAGES/changelog.po`

 * *Files identical despite different names*

### Comparing `ebilab-2.4.0/docs/source/locale/en/LC_MESSAGES/index.po` & `ebilab-2.5.0/docs/source/locale/en/LC_MESSAGES/index.po`

 * *Files identical despite different names*

### Comparing `ebilab-2.4.0/docs/source/locale/en/LC_MESSAGES/installation.po` & `ebilab-2.5.0/docs/source/locale/en/LC_MESSAGES/installation.po`

 * *Files identical despite different names*

### Comparing `ebilab-2.4.0/docs/source/locale/en/LC_MESSAGES/modules.po` & `ebilab-2.5.0/docs/source/locale/en/LC_MESSAGES/modules.po`

 * *Files identical despite different names*

### Comparing `ebilab-2.4.0/docs/source/locale/en/LC_MESSAGES/tutorial.po` & `ebilab-2.5.0/docs/source/locale/en/LC_MESSAGES/tutorial.po`

 * *Files identical despite different names*

### Comparing `ebilab-2.4.0/docs/source/tutorial/analysis.rst` & `ebilab-2.5.0/docs/source/tutorial/analysis.rst`

 * *Files identical despite different names*

### Comparing `ebilab-2.4.0/docs/source/tutorial/experiment.rst` & `ebilab-2.5.0/docs/source/tutorial/experiment.rst`

 * *Files identical despite different names*

### Comparing `ebilab-2.4.0/docs/source/tutorial/experiment_device.rst` & `ebilab-2.5.0/docs/source/tutorial/experiment_device.rst`

 * *Files identical despite different names*

### Comparing `ebilab-2.4.0/docs/source/tutorial/version.rst` & `ebilab-2.5.0/docs/source/tutorial/version.rst`

 * *Files identical despite different names*

### Comparing `ebilab-2.4.0/ebilab/__init__.py` & `ebilab-2.5.0/ebilab/__init__.py`

 * *Files identical despite different names*

### Comparing `ebilab-2.4.0/ebilab/_cli.py` & `ebilab-2.5.0/ebilab/_cli.py`

 * *Files identical despite different names*

### Comparing `ebilab-2.4.0/ebilab/analysis/_actions.py` & `ebilab-2.5.0/ebilab/analysis/_actions.py`

 * *Files identical despite different names*

### Comparing `ebilab-2.4.0/ebilab/analysis/_preprocess.py` & `ebilab-2.5.0/ebilab/analysis/_preprocess.py`

 * *Files identical despite different names*

### Comparing `ebilab-2.4.0/ebilab/analysis/_process.py` & `ebilab-2.5.0/ebilab/analysis/_process.py`

 * *Files identical despite different names*

### Comparing `ebilab-2.4.0/ebilab/data/project-template/.gitignore` & `ebilab-2.5.0/ebilab/data/project-template/.gitignore`

 * *Files identical despite different names*

### Comparing `ebilab-2.4.0/ebilab/experiment/_experiment_controller.py` & `ebilab-2.5.0/ebilab/experiment/_experiment_controller.py`

 * *Files identical despite different names*

### Comparing `ebilab-2.4.0/ebilab/experiment/_ui_tkinter.py` & `ebilab-2.5.0/ebilab/experiment/_ui_tkinter.py`

 * *Files identical despite different names*

### Comparing `ebilab-2.4.0/ebilab/experiment/devices/_visa/A707.py` & `ebilab-2.5.0/ebilab/experiment/devices/_visa/A707.py`

 * *Files 22% similar despite different names*

```diff
@@ -18,15 +18,21 @@
     def close_only(self, contacts: List[str]):
         """
         Open all switch and close only specified switch
 
         Args:
             contacts (list): like `["A2", "B4", "C5"]`
         """
-        string = ",".join([contact for contact in contacts])
-        self.visa_write(f'E0P0C{string}X')
+        if len(contacts) == 0:
+            self.visa_write(f'E0P0X')
+        else:
+            string = ",".join([contact for contact in contacts])
+            self.visa_write(f'E0P0C{string}X')
         sleep(0.1)
 
+    def open_all(self):
+        self.close_only([])
+
 if is_mock_enabled:
     class A707:
         def close_only(self, contacts: List[str]):
             pass
```

### Comparing `ebilab-2.4.0/ebilab/experiment/devices/_visa/E4980.py` & `ebilab-2.5.0/ebilab/experiment/devices/_visa/E4980.py`

 * *Files identical despite different names*

### Comparing `ebilab-2.4.0/ebilab/experiment/devices/_visa/K34411A.py` & `ebilab-2.5.0/ebilab/experiment/devices/_visa/K34411A.py`

 * *Files 26% similar despite different names*

```diff
@@ -43,14 +43,43 @@
         if range == "auto":
             self.visa_write("RES:RANG:AUTO ON")
         else:
             self.visa_write(f"RES:RANG {range}")
 
         val = self.visa_query("READ?")
         return float(val)
+    
+    def measure_resistance_4w(self, *, nplc: Optional[str]=None, range: str="auto"):
+        """
+        Measure resistance once by 4 wire method
+
+        Args:
+            nplc (Optional[str]): String from
+                {"0.001", "0.002", "0.006", "0.02", "0.06", "0.2", "1", "2", "10", "100"}
+            range (Optional[str]): String from
+                {"auto", "1E+2", "1E+3", "1E+4", "1E+5", "1E+6", "1E+7", "1E+8", "1E+9"}
+        """
+
+        # validate input
+        if nplc and nplc not in self._option_nplc:
+            raise ValueError(f"NPLC value \"{nplc}\" is invalid.")
+        if range not in self._option_r_range:
+            raise ValueError(f"Range value \"{range}\" is invalid.")
+
+        self.visa_write("CONF:FRES")
+        if nplc:
+            self.visa_write(f"FRES:NPLC {nplc}")
+
+        if range == "auto":
+            self.visa_write("FRES:RANG:AUTO ON")
+        else:
+            self.visa_write(f"FRES:RANG {range}")
+
+        val = self.visa_query("READ?")
+        return float(val)
 
     def measure_voltage(self, *, nplc: Optional[str]=None, range: str = "auto"):
         """
         Measure resistance once
 
         Args:
             nplc (Optional[str]): String from
```

### Comparing `ebilab-2.4.0/ebilab/experiment/devices/visa.py` & `ebilab-2.5.0/ebilab/experiment/devices/visa.py`

 * *Files identical despite different names*

### Comparing `ebilab-2.4.0/ebilab/experiment/options.py` & `ebilab-2.5.0/ebilab/experiment/options.py`

 * *Files identical despite different names*

### Comparing `ebilab-2.4.0/ebilab/icon.ico` & `ebilab-2.5.0/ebilab/icon.ico`

 * *Files identical despite different names*

### Comparing `ebilab-2.4.0/ebilab/project.py` & `ebilab-2.5.0/ebilab/project.py`

 * *Files identical despite different names*

### Comparing `ebilab-2.4.0/ebilab.egg-info/PKG-INFO` & `ebilab-2.5.0/ebilab.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ebilab
-Version: 2.4.0
+Version: 2.5.0
 Summary: Python package for my research
 Home-page: https://ebilab.readthedocs.io/
 Author: Yusuke Ebihara
 Author-email: yusuke@ebihara.me
 Project-URL: GitHub repository, https://github.com/ebiyuu1121/ebilab
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ebilab-2.4.0/ebilab.egg-info/SOURCES.txt` & `ebilab-2.5.0/ebilab.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 setup.py
 .github/workflows/ci.yaml
 .github/workflows/release.yaml
 docs/Makefile
 docs/make.bat
 docs/requirements.txt
 docs/source/changelog-v2.0.0-pre.rst
-docs/source/changelog.rst
+docs/source/changelog.md
 docs/source/conf.py
 docs/source/index.rst
 docs/source/installation.rst
 docs/source/api/ebilab.analysis.rst
 docs/source/api/ebilab.experiment.devices.rst
 docs/source/api/ebilab.experiment.devices.visa.rst
 docs/source/api/ebilab.experiment.rst
```

### Comparing `ebilab-2.4.0/sample/cont_r.py` & `ebilab-2.5.0/sample/cont_r.py`

 * *Files identical despite different names*

### Comparing `ebilab-2.4.0/sample/random-walk.py` & `ebilab-2.5.0/sample/random-walk.py`

 * *Files identical despite different names*

### Comparing `ebilab-2.4.0/sample/recipes/random-walk.py` & `ebilab-2.5.0/sample/recipes/random-walk.py`

 * *Files identical despite different names*

### Comparing `ebilab-2.4.0/sample/voltage.py` & `ebilab-2.5.0/sample/voltage.py`

 * *Files identical despite different names*

### Comparing `ebilab-2.4.0/setup.py` & `ebilab-2.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `ebilab-2.4.0/tests/test_paths.py` & `ebilab-2.5.0/tests/test_paths.py`

 * *Files identical despite different names*

