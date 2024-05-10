# Comparing `tmp/adafruit-circuitpython-display_shapes-2.8.2.tar.gz` & `tmp/adafruit_circuitpython_display_shapes-2.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-display_shapes-2.8.2.tar", last modified: Tue Jan 23 00:08:30 2024, max compression
+gzip compressed data, was "adafruit_circuitpython_display_shapes-2.8.3.tar", last modified: Fri May 10 21:32:24 2024, max compression
```

## Comparing `adafruit-circuitpython-display_shapes-2.8.2.tar` & `adafruit_circuitpython_display_shapes-2.8.3.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 00:08:30.969638 adafruit-circuitpython-display_shapes-2.8.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 00:08:30.957638 adafruit-circuitpython-display_shapes-2.8.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 00:08:30.961639 adafruit-circuitpython-display_shapes-2.8.2/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-01-23 00:08:18.000000 adafruit-circuitpython-display_shapes-2.8.2/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 00:08:30.961639 adafruit-circuitpython-display_shapes-2.8.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-01-23 00:08:18.000000 adafruit-circuitpython-display_shapes-2.8.2/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-01-23 00:08:18.000000 adafruit-circuitpython-display_shapes-2.8.2/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-01-23 00:08:18.000000 adafruit-circuitpython-display_shapes-2.8.2/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-01-23 00:08:18.000000 adafruit-circuitpython-display_shapes-2.8.2/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-01-23 00:08:18.000000 adafruit-circuitpython-display_shapes-2.8.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-01-23 00:08:18.000000 adafruit-circuitpython-display_shapes-2.8.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    13078 2024-01-23 00:08:18.000000 adafruit-circuitpython-display_shapes-2.8.2/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-01-23 00:08:18.000000 adafruit-circuitpython-display_shapes-2.8.2/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6147 2024-01-23 00:08:18.000000 adafruit-circuitpython-display_shapes-2.8.2/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-01-23 00:08:18.000000 adafruit-circuitpython-display_shapes-2.8.2/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 00:08:30.961639 adafruit-circuitpython-display_shapes-2.8.2/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (127)    16814 2024-01-23 00:08:18.000000 adafruit-circuitpython-display_shapes-2.8.2/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-01-23 00:08:18.000000 adafruit-circuitpython-display_shapes-2.8.2/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-01-23 00:08:18.000000 adafruit-circuitpython-display_shapes-2.8.2/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5888 2024-01-23 00:08:30.969638 adafruit-circuitpython-display_shapes-2.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5080 2024-01-23 00:08:18.000000 adafruit-circuitpython-display_shapes-2.8.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-01-23 00:08:18.000000 adafruit-circuitpython-display_shapes-2.8.2/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 00:08:30.965638 adafruit-circuitpython-display_shapes-2.8.2/adafruit_circuitpython_display_shapes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5888 2024-01-23 00:08:30.000000 adafruit-circuitpython-display_shapes-2.8.2/adafruit_circuitpython_display_shapes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-01-23 00:08:30.000000 adafruit-circuitpython-display_shapes-2.8.2/adafruit_circuitpython_display_shapes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-23 00:08:30.000000 adafruit-circuitpython-display_shapes-2.8.2/adafruit_circuitpython_display_shapes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-01-23 00:08:30.000000 adafruit-circuitpython-display_shapes-2.8.2/adafruit_circuitpython_display_shapes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-01-23 00:08:30.000000 adafruit-circuitpython-display_shapes-2.8.2/adafruit_circuitpython_display_shapes.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 00:08:30.965638 adafruit-circuitpython-display_shapes-2.8.2/adafruit_display_shapes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-23 00:08:24.000000 adafruit-circuitpython-display_shapes-2.8.2/adafruit_display_shapes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3626 2024-01-23 00:08:24.000000 adafruit-circuitpython-display_shapes-2.8.2/adafruit_display_shapes/arc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-01-23 00:08:24.000000 adafruit-circuitpython-display_shapes-2.8.2/adafruit_display_shapes/circle.py
--rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-01-23 00:08:24.000000 adafruit-circuitpython-display_shapes-2.8.2/adafruit_display_shapes/line.py
--rw-r--r--   0 runner    (1001) docker     (127)     9429 2024-01-23 00:08:24.000000 adafruit-circuitpython-display_shapes-2.8.2/adafruit_display_shapes/multisparkline.py
--rw-r--r--   0 runner    (1001) docker     (127)     5510 2024-01-23 00:08:24.000000 adafruit-circuitpython-display_shapes-2.8.2/adafruit_display_shapes/polygon.py
--rw-r--r--   0 runner    (1001) docker     (127)     3770 2024-01-23 00:08:24.000000 adafruit-circuitpython-display_shapes-2.8.2/adafruit_display_shapes/rect.py
--rw-r--r--   0 runner    (1001) docker     (127)     7000 2024-01-23 00:08:24.000000 adafruit-circuitpython-display_shapes-2.8.2/adafruit_display_shapes/roundrect.py
--rw-r--r--   0 runner    (1001) docker     (127)     3977 2024-01-23 00:08:24.000000 adafruit-circuitpython-display_shapes-2.8.2/adafruit_display_shapes/sparkline.py
--rw-r--r--   0 runner    (1001) docker     (127)     4845 2024-01-23 00:08:24.000000 adafruit-circuitpython-display_shapes-2.8.2/adafruit_display_shapes/triangle.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 00:08:30.965638 adafruit-circuitpython-display_shapes-2.8.2/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 00:08:30.965638 adafruit-circuitpython-display_shapes-2.8.2/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-01-23 00:08:18.000000 adafruit-circuitpython-display_shapes-2.8.2/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-01-23 00:08:18.000000 adafruit-circuitpython-display_shapes-2.8.2/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-01-23 00:08:18.000000 adafruit-circuitpython-display_shapes-2.8.2/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-01-23 00:08:18.000000 adafruit-circuitpython-display_shapes-2.8.2/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)     5451 2024-01-23 00:08:18.000000 adafruit-circuitpython-display_shapes-2.8.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-01-23 00:08:18.000000 adafruit-circuitpython-display_shapes-2.8.2/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-01-23 00:08:18.000000 adafruit-circuitpython-display_shapes-2.8.2/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)      981 2024-01-23 00:08:18.000000 adafruit-circuitpython-display_shapes-2.8.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-01-23 00:08:18.000000 adafruit-circuitpython-display_shapes-2.8.2/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-01-23 00:08:18.000000 adafruit-circuitpython-display_shapes-2.8.2/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 00:08:30.965638 adafruit-circuitpython-display_shapes-2.8.2/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-01-23 00:08:24.000000 adafruit-circuitpython-display_shapes-2.8.2/examples/display_shapes_arc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-01-23 00:08:24.000000 adafruit-circuitpython-display_shapes-2.8.2/examples/display_shapes_circle_animation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-01-23 00:08:24.000000 adafruit-circuitpython-display_shapes-2.8.2/examples/display_shapes_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-01-23 00:08:24.000000 adafruit-circuitpython-display_shapes-2.8.2/examples/display_shapes_simpletest_magtag.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4031 2024-01-23 00:08:24.000000 adafruit-circuitpython-display_shapes-2.8.2/examples/display_shapes_sparkline_simpletest.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5710 2024-01-23 00:08:24.000000 adafruit-circuitpython-display_shapes-2.8.2/examples/display_shapes_sparkline_ticks.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8564 2024-01-23 00:08:24.000000 adafruit-circuitpython-display_shapes-2.8.2/examples/display_shapes_sparkline_triple.py
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-01-23 00:08:18.000000 adafruit-circuitpython-display_shapes-2.8.2/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-01-23 00:08:24.000000 adafruit-circuitpython-display_shapes-2.8.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-01-23 00:08:18.000000 adafruit-circuitpython-display_shapes-2.8.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-23 00:08:30.969638 adafruit-circuitpython-display_shapes-2.8.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:32:24.828758 adafruit_circuitpython_display_shapes-2.8.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:32:24.820758 adafruit_circuitpython_display_shapes-2.8.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:32:24.820758 adafruit_circuitpython_display_shapes-2.8.3/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-10 21:32:16.000000 adafruit_circuitpython_display_shapes-2.8.3/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:32:24.820758 adafruit_circuitpython_display_shapes-2.8.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-10 21:32:16.000000 adafruit_circuitpython_display_shapes-2.8.3/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-10 21:32:16.000000 adafruit_circuitpython_display_shapes-2.8.3/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-05-10 21:32:16.000000 adafruit_circuitpython_display_shapes-2.8.3/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-10 21:32:16.000000 adafruit_circuitpython_display_shapes-2.8.3/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-05-10 21:32:16.000000 adafruit_circuitpython_display_shapes-2.8.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-10 21:32:16.000000 adafruit_circuitpython_display_shapes-2.8.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    13078 2024-05-10 21:32:16.000000 adafruit_circuitpython_display_shapes-2.8.3/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-10 21:32:16.000000 adafruit_circuitpython_display_shapes-2.8.3/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6147 2024-05-10 21:32:16.000000 adafruit_circuitpython_display_shapes-2.8.3/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-10 21:32:16.000000 adafruit_circuitpython_display_shapes-2.8.3/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:32:24.824758 adafruit_circuitpython_display_shapes-2.8.3/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (127)    16814 2024-05-10 21:32:16.000000 adafruit_circuitpython_display_shapes-2.8.3/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-10 21:32:16.000000 adafruit_circuitpython_display_shapes-2.8.3/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-10 21:32:16.000000 adafruit_circuitpython_display_shapes-2.8.3/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5888 2024-05-10 21:32:24.828758 adafruit_circuitpython_display_shapes-2.8.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5080 2024-05-10 21:32:16.000000 adafruit_circuitpython_display_shapes-2.8.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-10 21:32:16.000000 adafruit_circuitpython_display_shapes-2.8.3/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:32:24.828758 adafruit_circuitpython_display_shapes-2.8.3/adafruit_circuitpython_display_shapes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5888 2024-05-10 21:32:24.000000 adafruit_circuitpython_display_shapes-2.8.3/adafruit_circuitpython_display_shapes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-05-10 21:32:24.000000 adafruit_circuitpython_display_shapes-2.8.3/adafruit_circuitpython_display_shapes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 21:32:24.000000 adafruit_circuitpython_display_shapes-2.8.3/adafruit_circuitpython_display_shapes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-10 21:32:24.000000 adafruit_circuitpython_display_shapes-2.8.3/adafruit_circuitpython_display_shapes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-10 21:32:24.000000 adafruit_circuitpython_display_shapes-2.8.3/adafruit_circuitpython_display_shapes.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:32:24.824758 adafruit_circuitpython_display_shapes-2.8.3/adafruit_display_shapes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 21:32:22.000000 adafruit_circuitpython_display_shapes-2.8.3/adafruit_display_shapes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3626 2024-05-10 21:32:22.000000 adafruit_circuitpython_display_shapes-2.8.3/adafruit_display_shapes/arc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-05-10 21:32:22.000000 adafruit_circuitpython_display_shapes-2.8.3/adafruit_display_shapes/circle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-05-10 21:32:22.000000 adafruit_circuitpython_display_shapes-2.8.3/adafruit_display_shapes/line.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9340 2024-05-10 21:32:22.000000 adafruit_circuitpython_display_shapes-2.8.3/adafruit_display_shapes/multisparkline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5510 2024-05-10 21:32:22.000000 adafruit_circuitpython_display_shapes-2.8.3/adafruit_display_shapes/polygon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3770 2024-05-10 21:32:22.000000 adafruit_circuitpython_display_shapes-2.8.3/adafruit_display_shapes/rect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7000 2024-05-10 21:32:22.000000 adafruit_circuitpython_display_shapes-2.8.3/adafruit_display_shapes/roundrect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3977 2024-05-10 21:32:22.000000 adafruit_circuitpython_display_shapes-2.8.3/adafruit_display_shapes/sparkline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4845 2024-05-10 21:32:22.000000 adafruit_circuitpython_display_shapes-2.8.3/adafruit_display_shapes/triangle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:32:24.828758 adafruit_circuitpython_display_shapes-2.8.3/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:32:24.828758 adafruit_circuitpython_display_shapes-2.8.3/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-05-10 21:32:16.000000 adafruit_circuitpython_display_shapes-2.8.3/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-10 21:32:16.000000 adafruit_circuitpython_display_shapes-2.8.3/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-10 21:32:16.000000 adafruit_circuitpython_display_shapes-2.8.3/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-10 21:32:16.000000 adafruit_circuitpython_display_shapes-2.8.3/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)     5451 2024-05-10 21:32:16.000000 adafruit_circuitpython_display_shapes-2.8.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-05-10 21:32:16.000000 adafruit_circuitpython_display_shapes-2.8.3/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-10 21:32:16.000000 adafruit_circuitpython_display_shapes-2.8.3/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-05-10 21:32:16.000000 adafruit_circuitpython_display_shapes-2.8.3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-10 21:32:16.000000 adafruit_circuitpython_display_shapes-2.8.3/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-10 21:32:16.000000 adafruit_circuitpython_display_shapes-2.8.3/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:32:24.828758 adafruit_circuitpython_display_shapes-2.8.3/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-05-10 21:32:22.000000 adafruit_circuitpython_display_shapes-2.8.3/examples/display_shapes_arc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-05-10 21:32:22.000000 adafruit_circuitpython_display_shapes-2.8.3/examples/display_shapes_circle_animation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-05-10 21:32:22.000000 adafruit_circuitpython_display_shapes-2.8.3/examples/display_shapes_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-05-10 21:32:22.000000 adafruit_circuitpython_display_shapes-2.8.3/examples/display_shapes_simpletest_magtag.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4031 2024-05-10 21:32:22.000000 adafruit_circuitpython_display_shapes-2.8.3/examples/display_shapes_sparkline_simpletest.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5710 2024-05-10 21:32:22.000000 adafruit_circuitpython_display_shapes-2.8.3/examples/display_shapes_sparkline_ticks.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8564 2024-05-10 21:32:22.000000 adafruit_circuitpython_display_shapes-2.8.3/examples/display_shapes_sparkline_triple.py
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-10 21:32:16.000000 adafruit_circuitpython_display_shapes-2.8.3/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-05-10 21:32:22.000000 adafruit_circuitpython_display_shapes-2.8.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-10 21:32:16.000000 adafruit_circuitpython_display_shapes-2.8.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 21:32:24.828758 adafruit_circuitpython_display_shapes-2.8.3/setup.cfg
```

### Comparing `adafruit-circuitpython-display_shapes-2.8.2/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit_circuitpython_display_shapes-2.8.3/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-display_shapes-2.8.2/.gitignore` & `adafruit_circuitpython_display_shapes-2.8.3/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-display_shapes-2.8.2/.pre-commit-config.yaml` & `adafruit_circuitpython_display_shapes-2.8.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-display_shapes-2.8.2/.pylintrc` & `adafruit_circuitpython_display_shapes-2.8.3/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-display_shapes-2.8.2/CODE_OF_CONDUCT.md` & `adafruit_circuitpython_display_shapes-2.8.3/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-display_shapes-2.8.2/LICENSE` & `adafruit_circuitpython_display_shapes-2.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-display_shapes-2.8.2/LICENSES/CC-BY-4.0.txt` & `adafruit_circuitpython_display_shapes-2.8.3/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-display_shapes-2.8.2/LICENSES/MIT.txt` & `adafruit_circuitpython_display_shapes-2.8.3/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-display_shapes-2.8.2/LICENSES/Unlicense.txt` & `adafruit_circuitpython_display_shapes-2.8.3/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-display_shapes-2.8.2/PKG-INFO` & `adafruit_circuitpython_display_shapes-2.8.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-display_shapes
-Version: 2.8.2
+Version: 2.8.3
 Summary: Various common shapes for use with displayio
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_Display_Shapes
 Keywords: adafruit,blinka,circuitpython,micropython,display_shapes,shapes,displayio,drawing
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-display_shapes-2.8.2/README.rst` & `adafruit_circuitpython_display_shapes-2.8.3/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-display_shapes-2.8.2/adafruit_circuitpython_display_shapes.egg-info/PKG-INFO` & `adafruit_circuitpython_display_shapes-2.8.3/adafruit_circuitpython_display_shapes.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-display_shapes
-Version: 2.8.2
+Version: 2.8.3
 Summary: Various common shapes for use with displayio
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_Display_Shapes
 Keywords: adafruit,blinka,circuitpython,micropython,display_shapes,shapes,displayio,drawing
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-display_shapes-2.8.2/adafruit_circuitpython_display_shapes.egg-info/SOURCES.txt` & `adafruit_circuitpython_display_shapes-2.8.3/adafruit_circuitpython_display_shapes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-display_shapes-2.8.2/adafruit_display_shapes/arc.py` & `adafruit_circuitpython_display_shapes-2.8.3/adafruit_display_shapes/arc.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 try:
     import vectorio
 
     HAVE_VECTORIO = True
 except ImportError:
     HAVE_VECTORIO = False
 
-__version__ = "2.8.2"
+__version__ = "2.8.3"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_Display_Shapes.git"
 
 
 class Arc(displayio.Group):
     # pylint: disable=too-few-public-methods, invalid-name
     """An arc. Technically, an arc is a Group with one or two polygons.
```

### Comparing `adafruit-circuitpython-display_shapes-2.8.2/adafruit_display_shapes/circle.py` & `adafruit_circuitpython_display_shapes-2.8.3/adafruit_display_shapes/circle.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 try:
     from typing import Optional
 except ImportError:
     pass
 
 from adafruit_display_shapes.roundrect import RoundRect
 
-__version__ = "2.8.2"
+__version__ = "2.8.3"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_Display_Shapes.git"
 
 
 class Circle(RoundRect):
     # pylint: disable=too-few-public-methods, invalid-name
     """A circle.
```

### Comparing `adafruit-circuitpython-display_shapes-2.8.2/adafruit_display_shapes/line.py` & `adafruit_circuitpython_display_shapes-2.8.3/adafruit_display_shapes/line.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 try:
     from typing import Optional
 except ImportError:
     pass
 
 from adafruit_display_shapes.polygon import Polygon
 
-__version__ = "2.8.2"
+__version__ = "2.8.3"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_Display_Shapes.git"
 
 
 class Line(Polygon):
     # pylint: disable=too-many-arguments,invalid-name, too-few-public-methods
     """A line.
```

### Comparing `adafruit-circuitpython-display_shapes-2.8.2/adafruit_display_shapes/multisparkline.py` & `adafruit_circuitpython_display_shapes-2.8.3/adafruit_display_shapes/multisparkline.py`

 * *Files 2% similar despite different names*

```diff
@@ -168,18 +168,16 @@
         :param bool update: trigger recreation of primitives
 
         Note: when adding multiple values per sparkline it is more efficient to call
         this method with parameter 'update=False' and then to manually
         call the update()-method
         """
 
-        lines_to_update = []
         for i, value in enumerate(values):
             if value is not None:
-                lines_to_update.append(i)
                 top = self.y_tops[i]
                 bottom = self.y_bottoms[i]
                 if (
                     self._buffers[i].len() >= self._max_items
                 ):  # if list is full, remove the first item
                     first = self._buffers[i].pop()
                     # check if boundaries have to be updated
@@ -193,16 +191,16 @@
                     bottom = value if not bottom else min(value, bottom)
                 if self.y_maxs[i] is None:
                     top = value if not top else max(value, top)
 
                 self.y_tops[i] = top
                 self.y_bottoms[i] = bottom
 
-        if update and lines_to_update:
-            self.update_line(lines_to_update)
+                if update:
+                    self.update_line(i)
 
     def _add_point(
         self,
         line: int,
         x: int,
         value: float,
     ) -> None:
```

### Comparing `adafruit-circuitpython-display_shapes-2.8.2/adafruit_display_shapes/polygon.py` & `adafruit_circuitpython_display_shapes-2.8.3/adafruit_display_shapes/polygon.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 try:
     from typing import Optional, List, Tuple
 except ImportError:
     pass
 
 import displayio
 
-__version__ = "2.8.2"
+__version__ = "2.8.3"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_Display_Shapes.git"
 
 
 class Polygon(displayio.TileGrid):
     """A polygon.
 
     :param list points: A list of (x, y) tuples of the points
```

### Comparing `adafruit-circuitpython-display_shapes-2.8.2/adafruit_display_shapes/rect.py` & `adafruit_circuitpython_display_shapes-2.8.3/adafruit_display_shapes/rect.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 try:
     from typing import Optional
 except ImportError:
     pass
 
 import displayio
 
-__version__ = "2.8.2"
+__version__ = "2.8.3"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_Display_Shapes.git"
 
 
 class Rect(displayio.TileGrid):
     """A rectangle.
 
     :param int x: The x-position of the top left corner.
```

### Comparing `adafruit-circuitpython-display_shapes-2.8.2/adafruit_display_shapes/roundrect.py` & `adafruit_circuitpython_display_shapes-2.8.3/adafruit_display_shapes/roundrect.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 try:
     from typing import Optional
 except ImportError:
     pass
 
 import displayio
 
-__version__ = "2.8.2"
+__version__ = "2.8.3"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_Display_Shapes.git"
 
 
 class RoundRect(displayio.TileGrid):
     # pylint: disable=too-many-arguments
     """A round-corner rectangle.
```

### Comparing `adafruit-circuitpython-display_shapes-2.8.2/adafruit_display_shapes/sparkline.py` & `adafruit_circuitpython_display_shapes-2.8.3/adafruit_display_shapes/sparkline.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-display_shapes-2.8.2/adafruit_display_shapes/triangle.py` & `adafruit_circuitpython_display_shapes-2.8.3/adafruit_display_shapes/triangle.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 try:
     from typing import Optional
 except ImportError:
     pass
 
 from adafruit_display_shapes.polygon import Polygon
 
-__version__ = "2.8.2"
+__version__ = "2.8.3"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_Display_Shapes.git"
 
 
 class Triangle(Polygon):
     # pylint: disable=too-many-arguments,invalid-name
     """A triangle.
```

### Comparing `adafruit-circuitpython-display_shapes-2.8.2/docs/_static/favicon.ico` & `adafruit_circuitpython_display_shapes-2.8.3/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-display_shapes-2.8.2/docs/api.rst` & `adafruit_circuitpython_display_shapes-2.8.3/docs/api.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-display_shapes-2.8.2/docs/conf.py` & `adafruit_circuitpython_display_shapes-2.8.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-display_shapes-2.8.2/docs/examples.rst` & `adafruit_circuitpython_display_shapes-2.8.3/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-display_shapes-2.8.2/docs/index.rst` & `adafruit_circuitpython_display_shapes-2.8.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-display_shapes-2.8.2/examples/display_shapes_arc.py` & `adafruit_circuitpython_display_shapes-2.8.3/examples/display_shapes_arc.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-display_shapes-2.8.2/examples/display_shapes_circle_animation.py` & `adafruit_circuitpython_display_shapes-2.8.3/examples/display_shapes_circle_animation.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-display_shapes-2.8.2/examples/display_shapes_simpletest.py` & `adafruit_circuitpython_display_shapes-2.8.3/examples/display_shapes_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-display_shapes-2.8.2/examples/display_shapes_simpletest_magtag.py` & `adafruit_circuitpython_display_shapes-2.8.3/examples/display_shapes_simpletest_magtag.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-display_shapes-2.8.2/examples/display_shapes_sparkline_simpletest.py` & `adafruit_circuitpython_display_shapes-2.8.3/examples/display_shapes_sparkline_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-display_shapes-2.8.2/examples/display_shapes_sparkline_ticks.py` & `adafruit_circuitpython_display_shapes-2.8.3/examples/display_shapes_sparkline_ticks.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-display_shapes-2.8.2/examples/display_shapes_sparkline_triple.py` & `adafruit_circuitpython_display_shapes-2.8.3/examples/display_shapes_sparkline_triple.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-display_shapes-2.8.2/pyproject.toml` & `adafruit_circuitpython_display_shapes-2.8.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-display_shapes"
 description = "Various common shapes for use with displayio"
-version = "2.8.2"
+version = "2.8.3"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_Display_Shapes"}
 keywords = [
     "adafruit",
```

