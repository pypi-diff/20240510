# Comparing `tmp/napatrackmater-5.1.9.tar.gz` & `tmp/napatrackmater-5.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napatrackmater-5.1.9.tar", last modified: Wed May  1 22:12:22 2024, max compression
+gzip compressed data, was "napatrackmater-5.2.1.tar", last modified: Fri May 10 10:55:28 2024, max compression
```

## Comparing `napatrackmater-5.1.9.tar` & `napatrackmater-5.2.1.tar`

### file list

```diff
@@ -1,281 +1,281 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:12:22.450096 napatrackmater-5.1.9/
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:12:22.406096 napatrackmater-5.1.9/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:12:22.422096 napatrackmater-5.1.9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/.github/workflows/deploy.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/.travis.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     9639 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/MASTER.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:12:22.422096 napatrackmater-5.1.9/Notebooks/
--rw-r--r--   0 runner    (1001) docker     (127)    13692 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/Notebooks/Track_vector.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     4455 2024-05-01 22:12:22.450096 napatrackmater-5.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:12:22.418096 napatrackmater-5.1.9/_build/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:12:22.422096 napatrackmater-5.1.9/_build/.doctrees/
--rw-r--r--   0 runner    (1001) docker     (127)    33531 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/_build/.doctrees/MASTER.doctree
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:12:22.422096 napatrackmater-5.1.9/_build/.doctrees/Notebooks/
--rw-r--r--   0 runner    (1001) docker     (127)    29083 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/_build/.doctrees/Notebooks/Track_vector.doctree
--rw-r--r--   0 runner    (1001) docker     (127)    11990 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/_build/.doctrees/README.doctree
--rw-r--r--   0 runner    (1001) docker     (127)    36454 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/_build/.doctrees/environment.pickle
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:12:22.422096 napatrackmater-5.1.9/_build/html/
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/_build/html/.buildinfo
--rw-r--r--   0 runner    (1001) docker     (127)    29915 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/_build/html/MASTER.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:12:22.422096 napatrackmater-5.1.9/_build/html/Notebooks/
--rw-r--r--   0 runner    (1001) docker     (127)    66062 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/_build/html/Notebooks/Track_vector.html
--rw-r--r--   0 runner    (1001) docker     (127)    18885 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/_build/html/README.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:12:22.426096 napatrackmater-5.1.9/_build/html/_images/
--rw-r--r--   0 runner    (1001) docker     (127)    20293 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/_build/html/_images/ClusterDistributionPlot_time_point_97.png
--rw-r--r--   0 runner    (1001) docker     (127)    29672 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/_build/html/_images/ClusterNearnessPlot_time_point_97.png
--rw-r--r--   0 runner    (1001) docker     (127)   162373 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/_build/html/_images/ClusterPlot_time_point_97.png
--rw-r--r--   0 runner    (1001) docker     (127)    61613 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/_build/html/_images/FeatureMatrixPlot_time_point_97.png
--rw-r--r--   0 runner    (1001) docker     (127)    66872 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/_build/html/_images/QuadrantDistributionPlot_time_point_97.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:12:22.426096 napatrackmater-5.1.9/_build/html/_sources/
--rw-r--r--   0 runner    (1001) docker     (127)     9639 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/_build/html/_sources/MASTER.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:12:22.426096 napatrackmater-5.1.9/_build/html/_sources/Notebooks/
--rw-r--r--   0 runner    (1001) docker     (127)    13692 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/_build/html/_sources/Notebooks/Track_vector.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/_build/html/_sources/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:12:22.426096 napatrackmater-5.1.9/_build/html/_sphinx_design_static/
--rw-r--r--   0 runner    (1001) docker     (127)    48417 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/_build/html/_sphinx_design_static/design-style.4045f2051d55cab465a707391d5b2007.min.css
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/_build/html/_sphinx_design_static/design-tabs.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:12:22.430096 napatrackmater-5.1.9/_build/html/_static/
--rw-r--r--   0 runner    (1001) docker     (127)    14692 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/_build/html/_static/basic.css
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/_build/html/_static/check-solid.svg
--rw-r--r--   0 runner    (1001) docker     (127)     9031 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/_build/html/_static/clipboard.min.js
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/_build/html/_static/copy-button.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/_build/html/_static/copybutton.css
--rw-r--r--   0 runner    (1001) docker     (127)     8467 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/_build/html/_static/copybutton.js
--rw-r--r--   0 runner    (1001) docker     (127)     2698 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/_build/html/_static/copybutton_funcs.js
--rw-r--r--   0 runner    (1001) docker     (127)    48417 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/_build/html/_static/design-style.4045f2051d55cab465a707391d5b2007.min.css
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/_build/html/_static/design-tabs.js
--rw-r--r--   0 runner    (1001) docker     (127)    10766 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/_build/html/_static/doctools.js
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/_build/html/_static/documentation_options.js
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/_build/html/_static/file.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:12:22.430096 napatrackmater-5.1.9/_build/html/_static/images/
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/_build/html/_static/images/logo_binder.svg
--rw-r--r--   0 runner    (1001) docker     (127)     7601 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/_build/html/_static/images/logo_colab.png
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/_build/html/_static/images/logo_deepnote.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/_build/html/_static/images/logo_jupyterhub.svg
--rw-r--r--   0 runner    (1001) docker     (127)   287630 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/_build/html/_static/jquery-3.5.1.js
--rw-r--r--   0 runner    (1001) docker     (127)    89476 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/_build/html/_static/jquery.js
--rw-r--r--   0 runner    (1001) docker     (127)     6153 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/_build/html/_static/kapoorlablogo.png
--rw-r--r--   0 runner    (1001) docker     (127)    10854 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/_build/html/_static/language_data.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:12:22.418096 napatrackmater-5.1.9/_build/html/_static/locales/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:12:22.410096 napatrackmater-5.1.9/_build/html/_static/locales/ar/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:12:22.430096 napatrackmater-5.1.9/_build/html/_static/locales/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/_build/html/_static/locales/ar/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:12:22.410096 napatrackmater-5.1.9/_build/html/_static/locales/bg/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:12:22.430096 napatrackmater-5.1.9/_build/html/_static/locales/bg/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/_build/html/_static/locales/bg/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:12:22.410096 napatrackmater-5.1.9/_build/html/_static/locales/bn/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:12:22.430096 napatrackmater-5.1.9/_build/html/_static/locales/bn/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/_build/html/_static/locales/bn/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:12:22.410096 napatrackmater-5.1.9/_build/html/_static/locales/ca/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:12:22.430096 napatrackmater-5.1.9/_build/html/_static/locales/ca/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/_build/html/_static/locales/ca/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:12:22.410096 napatrackmater-5.1.9/_build/html/_static/locales/cs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:12:22.430096 napatrackmater-5.1.9/_build/html/_static/locales/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/_build/html/_static/locales/cs/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:12:22.410096 napatrackmater-5.1.9/_build/html/_static/locales/da/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:12:22.430096 napatrackmater-5.1.9/_build/html/_static/locales/da/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/_build/html/_static/locales/da/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:12:22.410096 napatrackmater-5.1.9/_build/html/_static/locales/de/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:12:22.434096 napatrackmater-5.1.9/_build/html/_static/locales/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/_build/html/_static/locales/de/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:12:22.410096 napatrackmater-5.1.9/_build/html/_static/locales/el/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:12:22.434096 napatrackmater-5.1.9/_build/html/_static/locales/el/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/_build/html/_static/locales/el/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:12:22.410096 napatrackmater-5.1.9/_build/html/_static/locales/eo/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:12:22.434096 napatrackmater-5.1.9/_build/html/_static/locales/eo/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/_build/html/_static/locales/eo/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:12:22.410096 napatrackmater-5.1.9/_build/html/_static/locales/es/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:12:22.434096 napatrackmater-5.1.9/_build/html/_static/locales/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/_build/html/_static/locales/es/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:12:22.410096 napatrackmater-5.1.9/_build/html/_static/locales/et/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:12:22.434096 napatrackmater-5.1.9/_build/html/_static/locales/et/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/_build/html/_static/locales/et/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:12:22.410096 napatrackmater-5.1.9/_build/html/_static/locales/fi/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:12:22.434096 napatrackmater-5.1.9/_build/html/_static/locales/fi/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/_build/html/_static/locales/fi/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:12:22.410096 napatrackmater-5.1.9/_build/html/_static/locales/fr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:12:22.434096 napatrackmater-5.1.9/_build/html/_static/locales/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/_build/html/_static/locales/fr/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:12:22.410096 napatrackmater-5.1.9/_build/html/_static/locales/hr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:12:22.434096 napatrackmater-5.1.9/_build/html/_static/locales/hr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/_build/html/_static/locales/hr/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:12:22.410096 napatrackmater-5.1.9/_build/html/_static/locales/id/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:12:22.434096 napatrackmater-5.1.9/_build/html/_static/locales/id/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/_build/html/_static/locales/id/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:12:22.410096 napatrackmater-5.1.9/_build/html/_static/locales/it/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:12:22.434096 napatrackmater-5.1.9/_build/html/_static/locales/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/_build/html/_static/locales/it/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:12:22.410096 napatrackmater-5.1.9/_build/html/_static/locales/iw/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:12:22.434096 napatrackmater-5.1.9/_build/html/_static/locales/iw/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/_build/html/_static/locales/iw/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:12:22.410096 napatrackmater-5.1.9/_build/html/_static/locales/ja/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:12:22.434096 napatrackmater-5.1.9/_build/html/_static/locales/ja/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/_build/html/_static/locales/ja/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:12:22.414096 napatrackmater-5.1.9/_build/html/_static/locales/ko/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:12:22.434096 napatrackmater-5.1.9/_build/html/_static/locales/ko/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/_build/html/_static/locales/ko/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:12:22.414096 napatrackmater-5.1.9/_build/html/_static/locales/lt/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:12:22.434096 napatrackmater-5.1.9/_build/html/_static/locales/lt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/_build/html/_static/locales/lt/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:12:22.414096 napatrackmater-5.1.9/_build/html/_static/locales/lv/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:12:22.434096 napatrackmater-5.1.9/_build/html/_static/locales/lv/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/_build/html/_static/locales/lv/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:12:22.414096 napatrackmater-5.1.9/_build/html/_static/locales/ml/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:12:22.434096 napatrackmater-5.1.9/_build/html/_static/locales/ml/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/_build/html/_static/locales/ml/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:12:22.414096 napatrackmater-5.1.9/_build/html/_static/locales/mr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:12:22.434096 napatrackmater-5.1.9/_build/html/_static/locales/mr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/_build/html/_static/locales/mr/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:12:22.414096 napatrackmater-5.1.9/_build/html/_static/locales/ms/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:12:22.434096 napatrackmater-5.1.9/_build/html/_static/locales/ms/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/_build/html/_static/locales/ms/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:12:22.414096 napatrackmater-5.1.9/_build/html/_static/locales/nl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:12:22.434096 napatrackmater-5.1.9/_build/html/_static/locales/nl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/_build/html/_static/locales/nl/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:12:22.414096 napatrackmater-5.1.9/_build/html/_static/locales/no/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:12:22.434096 napatrackmater-5.1.9/_build/html/_static/locales/no/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/_build/html/_static/locales/no/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:12:22.414096 napatrackmater-5.1.9/_build/html/_static/locales/pl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:12:22.434096 napatrackmater-5.1.9/_build/html/_static/locales/pl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/_build/html/_static/locales/pl/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:12:22.414096 napatrackmater-5.1.9/_build/html/_static/locales/pt/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:12:22.434096 napatrackmater-5.1.9/_build/html/_static/locales/pt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/_build/html/_static/locales/pt/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:12:22.414096 napatrackmater-5.1.9/_build/html/_static/locales/ro/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:12:22.434096 napatrackmater-5.1.9/_build/html/_static/locales/ro/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/_build/html/_static/locales/ro/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:12:22.414096 napatrackmater-5.1.9/_build/html/_static/locales/ru/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:12:22.434096 napatrackmater-5.1.9/_build/html/_static/locales/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/_build/html/_static/locales/ru/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:12:22.414096 napatrackmater-5.1.9/_build/html/_static/locales/sk/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:12:22.434096 napatrackmater-5.1.9/_build/html/_static/locales/sk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/_build/html/_static/locales/sk/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:12:22.414096 napatrackmater-5.1.9/_build/html/_static/locales/sl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:12:22.434096 napatrackmater-5.1.9/_build/html/_static/locales/sl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/_build/html/_static/locales/sl/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:12:22.414096 napatrackmater-5.1.9/_build/html/_static/locales/sr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:12:22.438096 napatrackmater-5.1.9/_build/html/_static/locales/sr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/_build/html/_static/locales/sr/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:12:22.414096 napatrackmater-5.1.9/_build/html/_static/locales/sv/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:12:22.438096 napatrackmater-5.1.9/_build/html/_static/locales/sv/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/_build/html/_static/locales/sv/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:12:22.414096 napatrackmater-5.1.9/_build/html/_static/locales/ta/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:12:22.438096 napatrackmater-5.1.9/_build/html/_static/locales/ta/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/_build/html/_static/locales/ta/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:12:22.414096 napatrackmater-5.1.9/_build/html/_static/locales/te/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:12:22.438096 napatrackmater-5.1.9/_build/html/_static/locales/te/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/_build/html/_static/locales/te/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:12:22.414096 napatrackmater-5.1.9/_build/html/_static/locales/tg/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:12:22.438096 napatrackmater-5.1.9/_build/html/_static/locales/tg/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/_build/html/_static/locales/tg/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:12:22.414096 napatrackmater-5.1.9/_build/html/_static/locales/th/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:12:22.438096 napatrackmater-5.1.9/_build/html/_static/locales/th/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/_build/html/_static/locales/th/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:12:22.418096 napatrackmater-5.1.9/_build/html/_static/locales/tl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:12:22.438096 napatrackmater-5.1.9/_build/html/_static/locales/tl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/_build/html/_static/locales/tl/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:12:22.418096 napatrackmater-5.1.9/_build/html/_static/locales/tr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:12:22.438096 napatrackmater-5.1.9/_build/html/_static/locales/tr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/_build/html/_static/locales/tr/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:12:22.418096 napatrackmater-5.1.9/_build/html/_static/locales/uk/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:12:22.438096 napatrackmater-5.1.9/_build/html/_static/locales/uk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/_build/html/_static/locales/uk/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:12:22.418096 napatrackmater-5.1.9/_build/html/_static/locales/ur/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:12:22.438096 napatrackmater-5.1.9/_build/html/_static/locales/ur/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/_build/html/_static/locales/ur/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:12:22.418096 napatrackmater-5.1.9/_build/html/_static/locales/vi/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:12:22.438096 napatrackmater-5.1.9/_build/html/_static/locales/vi/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/_build/html/_static/locales/vi/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:12:22.418096 napatrackmater-5.1.9/_build/html/_static/locales/zh_CN/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:12:22.438096 napatrackmater-5.1.9/_build/html/_static/locales/zh_CN/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/_build/html/_static/locales/zh_CN/LC_MESSAGES/booktheme.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:12:22.418096 napatrackmater-5.1.9/_build/html/_static/locales/zh_TW/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:12:22.438096 napatrackmater-5.1.9/_build/html/_static/locales/zh_TW/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/_build/html/_static/locales/zh_TW/LC_MESSAGES/booktheme.po
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/_build/html/_static/minus.png
--rw-r--r--   0 runner    (1001) docker     (127)    39364 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/_build/html/_static/mystnb.4510f1fc1dee50b3e5859aac5469c37c29e427902b24a333a5f9fcb2f0b3ac41.css
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/_build/html/_static/plus.png
--rw-r--r--   0 runner    (1001) docker     (127)    12757 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/_build/html/_static/pygments.css
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/_build/html/_static/sbt-webpack-macros.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:12:22.438096 napatrackmater-5.1.9/_build/html/_static/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)    80813 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/_build/html/_static/scripts/bootstrap.js
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/_build/html/_static/scripts/bootstrap.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)   335757 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/_build/html/_static/scripts/bootstrap.js.map
--rw-r--r--   0 runner    (1001) docker     (127)     4456 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/_build/html/_static/scripts/pydata-sphinx-theme.js
--rw-r--r--   0 runner    (1001) docker     (127)    19648 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/_build/html/_static/scripts/pydata-sphinx-theme.js.map
--rw-r--r--   0 runner    (1001) docker     (127)     3075 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/_build/html/_static/scripts/sphinx-book-theme.js
--rw-r--r--   0 runner    (1001) docker     (127)    13066 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/_build/html/_static/scripts/sphinx-book-theme.js.map
--rw-r--r--   0 runner    (1001) docker     (127)    16634 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/_build/html/_static/searchtools.js
--rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/_build/html/_static/sphinx-thebe.css
--rw-r--r--   0 runner    (1001) docker     (127)     3986 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/_build/html/_static/sphinx-thebe.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:12:22.442096 napatrackmater-5.1.9/_build/html/_static/styles/
--rw-r--r--   0 runner    (1001) docker     (127)   176654 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/_build/html/_static/styles/bootstrap.css
--rw-r--r--   0 runner    (1001) docker     (127)    63341 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/_build/html/_static/styles/pydata-sphinx-theme.css
--rw-r--r--   0 runner    (1001) docker     (127)    13841 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/_build/html/_static/styles/sphinx-book-theme.css
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/_build/html/_static/styles/theme.css
--rw-r--r--   0 runner    (1001) docker     (127)     3729 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/_build/html/_static/togglebutton.css
--rw-r--r--   0 runner    (1001) docker     (127)     7346 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/_build/html/_static/togglebutton.js
--rw-r--r--   0 runner    (1001) docker     (127)    68420 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/_build/html/_static/underscore-1.13.1.js
--rw-r--r--   0 runner    (1001) docker     (127)    19530 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/_build/html/_static/underscore.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:12:22.418096 napatrackmater-5.1.9/_build/html/_static/vendor/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:12:22.418096 napatrackmater-5.1.9/_build/html/_static/vendor/fontawesome/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:12:22.442096 napatrackmater-5.1.9/_build/html/_static/vendor/fontawesome/6.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     7427 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/_build/html/_static/vendor/fontawesome/6.1.2/LICENSE.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:12:22.442096 napatrackmater-5.1.9/_build/html/_static/vendor/fontawesome/6.1.2/css/
--rw-r--r--   0 runner    (1001) docker     (127)   101691 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/_build/html/_static/vendor/fontawesome/6.1.2/css/all.min.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:12:22.442096 napatrackmater-5.1.9/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/
--rw-r--r--   0 runner    (1001) docker     (127)   181264 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   105112 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    60236 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    24028 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.woff2
--rw-r--r--   0 runner    (1001) docker     (127)   389948 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   154840 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    10084 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     4776 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.woff2
--rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/_build/html/_static/webpack-macros.html
--rw-r--r--   0 runner    (1001) docker     (127)    11198 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/_build/html/genindex.html
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/_build/html/index.html
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/_build/html/objects.inv
--rw-r--r--   0 runner    (1001) docker     (127)    12010 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/_build/html/search.html
--rw-r--r--   0 runner    (1001) docker     (127)     7816 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/_build/html/searchindex.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:12:22.418096 napatrackmater-5.1.9/_build/jupyter_execute/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:12:22.442096 napatrackmater-5.1.9/_build/jupyter_execute/Notebooks/
--rw-r--r--   0 runner    (1001) docker     (127)    17500 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/_build/jupyter_execute/Notebooks/Track_vector.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/_config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/_toc.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:12:22.446096 napatrackmater-5.1.9/images/
--rw-r--r--   0 runner    (1001) docker     (127)    20293 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/images/ClusterDistributionPlot_time_point_97.png
--rw-r--r--   0 runner    (1001) docker     (127)    29672 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/images/ClusterNearnessPlot_time_point_97.png
--rw-r--r--   0 runner    (1001) docker     (127)   162373 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/images/ClusterPlot_time_point_97.png
--rw-r--r--   0 runner    (1001) docker     (127)    61613 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/images/FeatureMatrixPlot_time_point_97.png
--rw-r--r--   0 runner    (1001) docker     (127)    66872 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/images/QuadrantDistributionPlot_time_point_97.png
--rw-r--r--   0 runner    (1001) docker     (127)     6153 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/images/kapoorlablogo.png
--rw-r--r--   0 runner    (1001) docker     (127)     6153 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/images/kapoorlogo.png
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-05-01 22:12:22.450096 napatrackmater-5.1.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:12:22.418096 napatrackmater-5.1.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:12:22.446096 napatrackmater-5.1.9/src/napatrackmater/
--rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/src/napatrackmater/CloudAutoEncoder.py
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/src/napatrackmater/DeepEmbeddedClustering.py
--rw-r--r--   0 runner    (1001) docker     (127)   145682 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/src/napatrackmater/Trackmate.py
--rw-r--r--   0 runner    (1001) docker     (127)   135572 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/src/napatrackmater/Trackvector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3432 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/src/napatrackmater/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/src/napatrackmater/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    24585 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/src/napatrackmater/clustering.py
--rw-r--r--   0 runner    (1001) docker     (127)     3698 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/src/napatrackmater/fast_radius_regression.py
--rw-r--r--   0 runner    (1001) docker     (127)    13035 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/src/napatrackmater/fate_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     6603 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/src/napatrackmater/pretrained.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:12:22.450096 napatrackmater-5.1.9/src/napatrackmater.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4455 2024-05-01 22:12:22.000000 napatrackmater-5.1.9/src/napatrackmater.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7142 2024-05-01 22:12:22.000000 napatrackmater-5.1.9/src/napatrackmater.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 22:12:22.000000 napatrackmater-5.1.9/src/napatrackmater.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-01 22:12:22.000000 napatrackmater-5.1.9/src/napatrackmater.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-01 22:12:22.000000 napatrackmater-5.1.9/src/napatrackmater.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-05-01 22:12:10.000000 napatrackmater-5.1.9/update_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:55:28.626356 napatrackmater-5.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:55:28.582356 napatrackmater-5.2.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:55:28.598356 napatrackmater-5.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/.github/workflows/deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/.travis.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9639 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/MASTER.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:55:28.598356 napatrackmater-5.2.1/Notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)    13692 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/Notebooks/Track_vector.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     4455 2024-05-10 10:55:28.626356 napatrackmater-5.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:55:28.594356 napatrackmater-5.2.1/_build/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:55:28.598356 napatrackmater-5.2.1/_build/.doctrees/
+-rw-r--r--   0 runner    (1001) docker     (127)    33531 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/_build/.doctrees/MASTER.doctree
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:55:28.598356 napatrackmater-5.2.1/_build/.doctrees/Notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)    29083 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/_build/.doctrees/Notebooks/Track_vector.doctree
+-rw-r--r--   0 runner    (1001) docker     (127)    11990 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/_build/.doctrees/README.doctree
+-rw-r--r--   0 runner    (1001) docker     (127)    36454 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/_build/.doctrees/environment.pickle
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:55:28.598356 napatrackmater-5.2.1/_build/html/
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/_build/html/.buildinfo
+-rw-r--r--   0 runner    (1001) docker     (127)    29915 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/_build/html/MASTER.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:55:28.598356 napatrackmater-5.2.1/_build/html/Notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)    66062 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/_build/html/Notebooks/Track_vector.html
+-rw-r--r--   0 runner    (1001) docker     (127)    18885 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/_build/html/README.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:55:28.598356 napatrackmater-5.2.1/_build/html/_images/
+-rw-r--r--   0 runner    (1001) docker     (127)    20293 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/_build/html/_images/ClusterDistributionPlot_time_point_97.png
+-rw-r--r--   0 runner    (1001) docker     (127)    29672 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/_build/html/_images/ClusterNearnessPlot_time_point_97.png
+-rw-r--r--   0 runner    (1001) docker     (127)   162373 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/_build/html/_images/ClusterPlot_time_point_97.png
+-rw-r--r--   0 runner    (1001) docker     (127)    61613 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/_build/html/_images/FeatureMatrixPlot_time_point_97.png
+-rw-r--r--   0 runner    (1001) docker     (127)    66872 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/_build/html/_images/QuadrantDistributionPlot_time_point_97.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:55:28.598356 napatrackmater-5.2.1/_build/html/_sources/
+-rw-r--r--   0 runner    (1001) docker     (127)     9639 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/_build/html/_sources/MASTER.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:55:28.602356 napatrackmater-5.2.1/_build/html/_sources/Notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)    13692 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/_build/html/_sources/Notebooks/Track_vector.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/_build/html/_sources/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:55:28.602356 napatrackmater-5.2.1/_build/html/_sphinx_design_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    48417 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/_build/html/_sphinx_design_static/design-style.4045f2051d55cab465a707391d5b2007.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/_build/html/_sphinx_design_static/design-tabs.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:55:28.606356 napatrackmater-5.2.1/_build/html/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    14692 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/_build/html/_static/basic.css
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/_build/html/_static/check-solid.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     9031 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/_build/html/_static/clipboard.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/_build/html/_static/copy-button.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/_build/html/_static/copybutton.css
+-rw-r--r--   0 runner    (1001) docker     (127)     8467 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/_build/html/_static/copybutton.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2698 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/_build/html/_static/copybutton_funcs.js
+-rw-r--r--   0 runner    (1001) docker     (127)    48417 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/_build/html/_static/design-style.4045f2051d55cab465a707391d5b2007.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/_build/html/_static/design-tabs.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10766 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/_build/html/_static/doctools.js
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/_build/html/_static/documentation_options.js
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/_build/html/_static/file.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:55:28.606356 napatrackmater-5.2.1/_build/html/_static/images/
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/_build/html/_static/images/logo_binder.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     7601 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/_build/html/_static/images/logo_colab.png
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/_build/html/_static/images/logo_deepnote.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/_build/html/_static/images/logo_jupyterhub.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   287630 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/_build/html/_static/jquery-3.5.1.js
+-rw-r--r--   0 runner    (1001) docker     (127)    89476 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/_build/html/_static/jquery.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6153 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/_build/html/_static/kapoorlablogo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10854 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/_build/html/_static/language_data.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:55:28.594356 napatrackmater-5.2.1/_build/html/_static/locales/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:55:28.582356 napatrackmater-5.2.1/_build/html/_static/locales/ar/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:55:28.606356 napatrackmater-5.2.1/_build/html/_static/locales/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/_build/html/_static/locales/ar/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:55:28.586356 napatrackmater-5.2.1/_build/html/_static/locales/bg/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:55:28.606356 napatrackmater-5.2.1/_build/html/_static/locales/bg/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/_build/html/_static/locales/bg/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:55:28.586356 napatrackmater-5.2.1/_build/html/_static/locales/bn/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:55:28.606356 napatrackmater-5.2.1/_build/html/_static/locales/bn/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/_build/html/_static/locales/bn/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:55:28.586356 napatrackmater-5.2.1/_build/html/_static/locales/ca/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:55:28.606356 napatrackmater-5.2.1/_build/html/_static/locales/ca/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/_build/html/_static/locales/ca/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:55:28.586356 napatrackmater-5.2.1/_build/html/_static/locales/cs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:55:28.606356 napatrackmater-5.2.1/_build/html/_static/locales/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/_build/html/_static/locales/cs/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:55:28.586356 napatrackmater-5.2.1/_build/html/_static/locales/da/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:55:28.606356 napatrackmater-5.2.1/_build/html/_static/locales/da/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/_build/html/_static/locales/da/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:55:28.586356 napatrackmater-5.2.1/_build/html/_static/locales/de/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:55:28.606356 napatrackmater-5.2.1/_build/html/_static/locales/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/_build/html/_static/locales/de/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:55:28.586356 napatrackmater-5.2.1/_build/html/_static/locales/el/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:55:28.606356 napatrackmater-5.2.1/_build/html/_static/locales/el/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/_build/html/_static/locales/el/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:55:28.586356 napatrackmater-5.2.1/_build/html/_static/locales/eo/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:55:28.606356 napatrackmater-5.2.1/_build/html/_static/locales/eo/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/_build/html/_static/locales/eo/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:55:28.586356 napatrackmater-5.2.1/_build/html/_static/locales/es/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:55:28.610356 napatrackmater-5.2.1/_build/html/_static/locales/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/_build/html/_static/locales/es/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:55:28.586356 napatrackmater-5.2.1/_build/html/_static/locales/et/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:55:28.610356 napatrackmater-5.2.1/_build/html/_static/locales/et/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/_build/html/_static/locales/et/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:55:28.586356 napatrackmater-5.2.1/_build/html/_static/locales/fi/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:55:28.610356 napatrackmater-5.2.1/_build/html/_static/locales/fi/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/_build/html/_static/locales/fi/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:55:28.586356 napatrackmater-5.2.1/_build/html/_static/locales/fr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:55:28.610356 napatrackmater-5.2.1/_build/html/_static/locales/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/_build/html/_static/locales/fr/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:55:28.586356 napatrackmater-5.2.1/_build/html/_static/locales/hr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:55:28.610356 napatrackmater-5.2.1/_build/html/_static/locales/hr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/_build/html/_static/locales/hr/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:55:28.586356 napatrackmater-5.2.1/_build/html/_static/locales/id/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:55:28.610356 napatrackmater-5.2.1/_build/html/_static/locales/id/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/_build/html/_static/locales/id/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:55:28.586356 napatrackmater-5.2.1/_build/html/_static/locales/it/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:55:28.610356 napatrackmater-5.2.1/_build/html/_static/locales/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/_build/html/_static/locales/it/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:55:28.586356 napatrackmater-5.2.1/_build/html/_static/locales/iw/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:55:28.610356 napatrackmater-5.2.1/_build/html/_static/locales/iw/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/_build/html/_static/locales/iw/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:55:28.586356 napatrackmater-5.2.1/_build/html/_static/locales/ja/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:55:28.610356 napatrackmater-5.2.1/_build/html/_static/locales/ja/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/_build/html/_static/locales/ja/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:55:28.586356 napatrackmater-5.2.1/_build/html/_static/locales/ko/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:55:28.610356 napatrackmater-5.2.1/_build/html/_static/locales/ko/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/_build/html/_static/locales/ko/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:55:28.586356 napatrackmater-5.2.1/_build/html/_static/locales/lt/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:55:28.610356 napatrackmater-5.2.1/_build/html/_static/locales/lt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/_build/html/_static/locales/lt/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:55:28.586356 napatrackmater-5.2.1/_build/html/_static/locales/lv/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:55:28.610356 napatrackmater-5.2.1/_build/html/_static/locales/lv/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/_build/html/_static/locales/lv/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:55:28.586356 napatrackmater-5.2.1/_build/html/_static/locales/ml/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:55:28.610356 napatrackmater-5.2.1/_build/html/_static/locales/ml/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/_build/html/_static/locales/ml/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:55:28.590355 napatrackmater-5.2.1/_build/html/_static/locales/mr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:55:28.610356 napatrackmater-5.2.1/_build/html/_static/locales/mr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/_build/html/_static/locales/mr/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:55:28.590355 napatrackmater-5.2.1/_build/html/_static/locales/ms/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:55:28.610356 napatrackmater-5.2.1/_build/html/_static/locales/ms/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/_build/html/_static/locales/ms/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:55:28.590355 napatrackmater-5.2.1/_build/html/_static/locales/nl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:55:28.610356 napatrackmater-5.2.1/_build/html/_static/locales/nl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/_build/html/_static/locales/nl/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:55:28.590355 napatrackmater-5.2.1/_build/html/_static/locales/no/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:55:28.610356 napatrackmater-5.2.1/_build/html/_static/locales/no/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/_build/html/_static/locales/no/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:55:28.590355 napatrackmater-5.2.1/_build/html/_static/locales/pl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:55:28.610356 napatrackmater-5.2.1/_build/html/_static/locales/pl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/_build/html/_static/locales/pl/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:55:28.590355 napatrackmater-5.2.1/_build/html/_static/locales/pt/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:55:28.610356 napatrackmater-5.2.1/_build/html/_static/locales/pt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/_build/html/_static/locales/pt/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:55:28.590355 napatrackmater-5.2.1/_build/html/_static/locales/ro/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:55:28.610356 napatrackmater-5.2.1/_build/html/_static/locales/ro/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/_build/html/_static/locales/ro/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:55:28.590355 napatrackmater-5.2.1/_build/html/_static/locales/ru/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:55:28.610356 napatrackmater-5.2.1/_build/html/_static/locales/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/_build/html/_static/locales/ru/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:55:28.590355 napatrackmater-5.2.1/_build/html/_static/locales/sk/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:55:28.610356 napatrackmater-5.2.1/_build/html/_static/locales/sk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/_build/html/_static/locales/sk/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:55:28.590355 napatrackmater-5.2.1/_build/html/_static/locales/sl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:55:28.610356 napatrackmater-5.2.1/_build/html/_static/locales/sl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/_build/html/_static/locales/sl/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:55:28.590355 napatrackmater-5.2.1/_build/html/_static/locales/sr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:55:28.610356 napatrackmater-5.2.1/_build/html/_static/locales/sr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/_build/html/_static/locales/sr/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:55:28.590355 napatrackmater-5.2.1/_build/html/_static/locales/sv/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:55:28.610356 napatrackmater-5.2.1/_build/html/_static/locales/sv/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/_build/html/_static/locales/sv/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:55:28.590355 napatrackmater-5.2.1/_build/html/_static/locales/ta/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:55:28.610356 napatrackmater-5.2.1/_build/html/_static/locales/ta/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/_build/html/_static/locales/ta/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:55:28.590355 napatrackmater-5.2.1/_build/html/_static/locales/te/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:55:28.614356 napatrackmater-5.2.1/_build/html/_static/locales/te/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/_build/html/_static/locales/te/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:55:28.590355 napatrackmater-5.2.1/_build/html/_static/locales/tg/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:55:28.614356 napatrackmater-5.2.1/_build/html/_static/locales/tg/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/_build/html/_static/locales/tg/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:55:28.590355 napatrackmater-5.2.1/_build/html/_static/locales/th/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:55:28.614356 napatrackmater-5.2.1/_build/html/_static/locales/th/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/_build/html/_static/locales/th/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:55:28.590355 napatrackmater-5.2.1/_build/html/_static/locales/tl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:55:28.614356 napatrackmater-5.2.1/_build/html/_static/locales/tl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/_build/html/_static/locales/tl/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:55:28.590355 napatrackmater-5.2.1/_build/html/_static/locales/tr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:55:28.614356 napatrackmater-5.2.1/_build/html/_static/locales/tr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/_build/html/_static/locales/tr/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:55:28.590355 napatrackmater-5.2.1/_build/html/_static/locales/uk/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:55:28.614356 napatrackmater-5.2.1/_build/html/_static/locales/uk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/_build/html/_static/locales/uk/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:55:28.590355 napatrackmater-5.2.1/_build/html/_static/locales/ur/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:55:28.614356 napatrackmater-5.2.1/_build/html/_static/locales/ur/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/_build/html/_static/locales/ur/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:55:28.594356 napatrackmater-5.2.1/_build/html/_static/locales/vi/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:55:28.614356 napatrackmater-5.2.1/_build/html/_static/locales/vi/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/_build/html/_static/locales/vi/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:55:28.594356 napatrackmater-5.2.1/_build/html/_static/locales/zh_CN/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:55:28.614356 napatrackmater-5.2.1/_build/html/_static/locales/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/_build/html/_static/locales/zh_CN/LC_MESSAGES/booktheme.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:55:28.594356 napatrackmater-5.2.1/_build/html/_static/locales/zh_TW/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:55:28.614356 napatrackmater-5.2.1/_build/html/_static/locales/zh_TW/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/_build/html/_static/locales/zh_TW/LC_MESSAGES/booktheme.po
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/_build/html/_static/minus.png
+-rw-r--r--   0 runner    (1001) docker     (127)    39364 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/_build/html/_static/mystnb.4510f1fc1dee50b3e5859aac5469c37c29e427902b24a333a5f9fcb2f0b3ac41.css
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/_build/html/_static/plus.png
+-rw-r--r--   0 runner    (1001) docker     (127)    12757 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/_build/html/_static/pygments.css
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/_build/html/_static/sbt-webpack-macros.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:55:28.614356 napatrackmater-5.2.1/_build/html/_static/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)    80813 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/_build/html/_static/scripts/bootstrap.js
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/_build/html/_static/scripts/bootstrap.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   335757 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/_build/html/_static/scripts/bootstrap.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)     4456 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/_build/html/_static/scripts/pydata-sphinx-theme.js
+-rw-r--r--   0 runner    (1001) docker     (127)    19648 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/_build/html/_static/scripts/pydata-sphinx-theme.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)     3075 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/_build/html/_static/scripts/sphinx-book-theme.js
+-rw-r--r--   0 runner    (1001) docker     (127)    13066 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/_build/html/_static/scripts/sphinx-book-theme.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)    16634 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/_build/html/_static/searchtools.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/_build/html/_static/sphinx-thebe.css
+-rw-r--r--   0 runner    (1001) docker     (127)     3986 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/_build/html/_static/sphinx-thebe.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:55:28.618356 napatrackmater-5.2.1/_build/html/_static/styles/
+-rw-r--r--   0 runner    (1001) docker     (127)   176654 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/_build/html/_static/styles/bootstrap.css
+-rw-r--r--   0 runner    (1001) docker     (127)    63341 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/_build/html/_static/styles/pydata-sphinx-theme.css
+-rw-r--r--   0 runner    (1001) docker     (127)    13841 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/_build/html/_static/styles/sphinx-book-theme.css
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/_build/html/_static/styles/theme.css
+-rw-r--r--   0 runner    (1001) docker     (127)     3729 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/_build/html/_static/togglebutton.css
+-rw-r--r--   0 runner    (1001) docker     (127)     7346 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/_build/html/_static/togglebutton.js
+-rw-r--r--   0 runner    (1001) docker     (127)    68420 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/_build/html/_static/underscore-1.13.1.js
+-rw-r--r--   0 runner    (1001) docker     (127)    19530 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/_build/html/_static/underscore.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:55:28.594356 napatrackmater-5.2.1/_build/html/_static/vendor/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:55:28.594356 napatrackmater-5.2.1/_build/html/_static/vendor/fontawesome/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:55:28.618356 napatrackmater-5.2.1/_build/html/_static/vendor/fontawesome/6.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     7427 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/_build/html/_static/vendor/fontawesome/6.1.2/LICENSE.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:55:28.618356 napatrackmater-5.2.1/_build/html/_static/vendor/fontawesome/6.1.2/css/
+-rw-r--r--   0 runner    (1001) docker     (127)   101691 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/_build/html/_static/vendor/fontawesome/6.1.2/css/all.min.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:55:28.618356 napatrackmater-5.2.1/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/
+-rw-r--r--   0 runner    (1001) docker     (127)   181264 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   105112 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    60236 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    24028 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)   389948 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   154840 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    10084 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     4776 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/_build/html/_static/webpack-macros.html
+-rw-r--r--   0 runner    (1001) docker     (127)    11198 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/_build/html/genindex.html
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/_build/html/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/_build/html/objects.inv
+-rw-r--r--   0 runner    (1001) docker     (127)    12010 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/_build/html/search.html
+-rw-r--r--   0 runner    (1001) docker     (127)     7816 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/_build/html/searchindex.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:55:28.594356 napatrackmater-5.2.1/_build/jupyter_execute/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:55:28.618356 napatrackmater-5.2.1/_build/jupyter_execute/Notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)    17500 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/_build/jupyter_execute/Notebooks/Track_vector.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/_config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/_toc.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:55:28.622356 napatrackmater-5.2.1/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    20293 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/images/ClusterDistributionPlot_time_point_97.png
+-rw-r--r--   0 runner    (1001) docker     (127)    29672 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/images/ClusterNearnessPlot_time_point_97.png
+-rw-r--r--   0 runner    (1001) docker     (127)   162373 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/images/ClusterPlot_time_point_97.png
+-rw-r--r--   0 runner    (1001) docker     (127)    61613 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/images/FeatureMatrixPlot_time_point_97.png
+-rw-r--r--   0 runner    (1001) docker     (127)    66872 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/images/QuadrantDistributionPlot_time_point_97.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6153 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/images/kapoorlablogo.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6153 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/images/kapoorlogo.png
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-05-10 10:55:28.626356 napatrackmater-5.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:55:28.594356 napatrackmater-5.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:55:28.622356 napatrackmater-5.2.1/src/napatrackmater/
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/src/napatrackmater/CloudAutoEncoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/src/napatrackmater/DeepEmbeddedClustering.py
+-rw-r--r--   0 runner    (1001) docker     (127)   145682 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/src/napatrackmater/Trackmate.py
+-rw-r--r--   0 runner    (1001) docker     (127)   151746 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/src/napatrackmater/Trackvector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3710 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/src/napatrackmater/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/src/napatrackmater/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24585 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/src/napatrackmater/clustering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3698 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/src/napatrackmater/fast_radius_regression.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13035 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/src/napatrackmater/fate_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6603 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/src/napatrackmater/pretrained.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:55:28.622356 napatrackmater-5.2.1/src/napatrackmater.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4455 2024-05-10 10:55:28.000000 napatrackmater-5.2.1/src/napatrackmater.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7142 2024-05-10 10:55:28.000000 napatrackmater-5.2.1/src/napatrackmater.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 10:55:28.000000 napatrackmater-5.2.1/src/napatrackmater.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-10 10:55:28.000000 napatrackmater-5.2.1/src/napatrackmater.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-10 10:55:28.000000 napatrackmater-5.2.1/src/napatrackmater.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-05-10 10:55:18.000000 napatrackmater-5.2.1/update_version.py
```

### Comparing `napatrackmater-5.1.9/.github/workflows/deploy.yml` & `napatrackmater-5.2.1/.github/workflows/deploy.yml`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/.github/workflows/test_and_deploy.yml` & `napatrackmater-5.2.1/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/.gitignore` & `napatrackmater-5.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/.pre-commit-config.yaml` & `napatrackmater-5.2.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/.travis.yml` & `napatrackmater-5.2.1/.travis.yml`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/Dockerfile` & `napatrackmater-5.2.1/Dockerfile`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/LICENSE` & `napatrackmater-5.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/MASTER.md` & `napatrackmater-5.2.1/MASTER.md`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/Notebooks/Track_vector.ipynb` & `napatrackmater-5.2.1/Notebooks/Track_vector.ipynb`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/PKG-INFO` & `napatrackmater-5.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napatrackmater
-Version: 5.1.9
+Version: 5.2.1
 Summary: Import Trackmate XML files for Track Visualization and analysis in Napari.
 Home-page: https://github.com/Kapoorlabs-CAPED/napatrackmater
 Author: Varun Kapoor, Mari Tolonen, Jakub Sedzinski
 Author-email: randomaccessiblekapoor@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/Kapoorlabs-CAPED/napatrackmater/issues
 Project-URL: Documentation, https://github.com/Kapoorlabs-CAPED/napatrackmater#README.md
```

### Comparing `napatrackmater-5.1.9/README.md` & `napatrackmater-5.2.1/README.md`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/_build/.doctrees/MASTER.doctree` & `napatrackmater-5.2.1/_build/.doctrees/MASTER.doctree`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/_build/.doctrees/Notebooks/Track_vector.doctree` & `napatrackmater-5.2.1/_build/.doctrees/Notebooks/Track_vector.doctree`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/_build/.doctrees/README.doctree` & `napatrackmater-5.2.1/_build/.doctrees/README.doctree`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/_build/.doctrees/environment.pickle` & `napatrackmater-5.2.1/_build/.doctrees/environment.pickle`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/_build/html/MASTER.html` & `napatrackmater-5.2.1/_build/html/MASTER.html`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/_build/html/Notebooks/Track_vector.html` & `napatrackmater-5.2.1/_build/html/Notebooks/Track_vector.html`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/_build/html/README.html` & `napatrackmater-5.2.1/_build/html/README.html`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/_build/html/_images/ClusterDistributionPlot_time_point_97.png` & `napatrackmater-5.2.1/_build/html/_images/ClusterDistributionPlot_time_point_97.png`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/_build/html/_images/ClusterNearnessPlot_time_point_97.png` & `napatrackmater-5.2.1/_build/html/_images/ClusterNearnessPlot_time_point_97.png`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/_build/html/_images/ClusterPlot_time_point_97.png` & `napatrackmater-5.2.1/_build/html/_images/ClusterPlot_time_point_97.png`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/_build/html/_images/FeatureMatrixPlot_time_point_97.png` & `napatrackmater-5.2.1/_build/html/_images/FeatureMatrixPlot_time_point_97.png`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/_build/html/_images/QuadrantDistributionPlot_time_point_97.png` & `napatrackmater-5.2.1/_build/html/_images/QuadrantDistributionPlot_time_point_97.png`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/_build/html/_sources/MASTER.md` & `napatrackmater-5.2.1/_build/html/_sources/MASTER.md`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/_build/html/_sources/Notebooks/Track_vector.ipynb` & `napatrackmater-5.2.1/_build/html/_sources/Notebooks/Track_vector.ipynb`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/_build/html/_sources/README.md` & `napatrackmater-5.2.1/_build/html/_sources/README.md`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/_build/html/_sphinx_design_static/design-style.4045f2051d55cab465a707391d5b2007.min.css` & `napatrackmater-5.2.1/_build/html/_sphinx_design_static/design-style.4045f2051d55cab465a707391d5b2007.min.css`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/_build/html/_sphinx_design_static/design-tabs.js` & `napatrackmater-5.2.1/_build/html/_sphinx_design_static/design-tabs.js`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/_build/html/_static/basic.css` & `napatrackmater-5.2.1/_build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/_build/html/_static/clipboard.min.js` & `napatrackmater-5.2.1/_build/html/_static/clipboard.min.js`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/_build/html/_static/copybutton.css` & `napatrackmater-5.2.1/_build/html/_static/copybutton.css`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/_build/html/_static/copybutton.js` & `napatrackmater-5.2.1/_build/html/_static/copybutton.js`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/_build/html/_static/copybutton_funcs.js` & `napatrackmater-5.2.1/_build/html/_static/copybutton_funcs.js`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/_build/html/_static/design-style.4045f2051d55cab465a707391d5b2007.min.css` & `napatrackmater-5.2.1/_build/html/_static/design-style.4045f2051d55cab465a707391d5b2007.min.css`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/_build/html/_static/design-tabs.js` & `napatrackmater-5.2.1/_build/html/_static/design-tabs.js`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/_build/html/_static/doctools.js` & `napatrackmater-5.2.1/_build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/_build/html/_static/images/logo_binder.svg` & `napatrackmater-5.2.1/_build/html/_static/images/logo_binder.svg`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/_build/html/_static/images/logo_colab.png` & `napatrackmater-5.2.1/_build/html/_static/images/logo_colab.png`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/_build/html/_static/images/logo_deepnote.svg` & `napatrackmater-5.2.1/_build/html/_static/images/logo_deepnote.svg`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/_build/html/_static/images/logo_jupyterhub.svg` & `napatrackmater-5.2.1/_build/html/_static/images/logo_jupyterhub.svg`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/_build/html/_static/jquery-3.5.1.js` & `napatrackmater-5.2.1/_build/html/_static/jquery-3.5.1.js`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/_build/html/_static/jquery.js` & `napatrackmater-5.2.1/_build/html/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/_build/html/_static/kapoorlablogo.png` & `napatrackmater-5.2.1/_build/html/_static/kapoorlablogo.png`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/_build/html/_static/language_data.js` & `napatrackmater-5.2.1/_build/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/_build/html/_static/locales/ar/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.1/_build/html/_static/locales/ar/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/_build/html/_static/locales/bg/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.1/_build/html/_static/locales/bg/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/_build/html/_static/locales/bn/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.1/_build/html/_static/locales/bn/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/_build/html/_static/locales/ca/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.1/_build/html/_static/locales/ca/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/_build/html/_static/locales/cs/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.1/_build/html/_static/locales/cs/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/_build/html/_static/locales/da/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.1/_build/html/_static/locales/da/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/_build/html/_static/locales/de/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.1/_build/html/_static/locales/de/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/_build/html/_static/locales/el/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.1/_build/html/_static/locales/el/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/_build/html/_static/locales/eo/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.1/_build/html/_static/locales/eo/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/_build/html/_static/locales/es/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.1/_build/html/_static/locales/es/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/_build/html/_static/locales/et/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.1/_build/html/_static/locales/et/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/_build/html/_static/locales/fi/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.1/_build/html/_static/locales/fi/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/_build/html/_static/locales/fr/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.1/_build/html/_static/locales/fr/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/_build/html/_static/locales/hr/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.1/_build/html/_static/locales/hr/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/_build/html/_static/locales/id/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.1/_build/html/_static/locales/id/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/_build/html/_static/locales/it/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.1/_build/html/_static/locales/it/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/_build/html/_static/locales/iw/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.1/_build/html/_static/locales/iw/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/_build/html/_static/locales/ja/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.1/_build/html/_static/locales/ja/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/_build/html/_static/locales/ko/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.1/_build/html/_static/locales/ko/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/_build/html/_static/locales/lt/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.1/_build/html/_static/locales/lt/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/_build/html/_static/locales/lv/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.1/_build/html/_static/locales/lv/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/_build/html/_static/locales/ml/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.1/_build/html/_static/locales/ml/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/_build/html/_static/locales/mr/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.1/_build/html/_static/locales/mr/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/_build/html/_static/locales/ms/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.1/_build/html/_static/locales/ms/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/_build/html/_static/locales/nl/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.1/_build/html/_static/locales/nl/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/_build/html/_static/locales/no/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.1/_build/html/_static/locales/no/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/_build/html/_static/locales/pl/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.1/_build/html/_static/locales/pl/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/_build/html/_static/locales/pt/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.1/_build/html/_static/locales/pt/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/_build/html/_static/locales/ro/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.1/_build/html/_static/locales/ro/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/_build/html/_static/locales/ru/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.1/_build/html/_static/locales/ru/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/_build/html/_static/locales/sk/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.1/_build/html/_static/locales/sk/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/_build/html/_static/locales/sl/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.1/_build/html/_static/locales/sl/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/_build/html/_static/locales/sr/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.1/_build/html/_static/locales/sr/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/_build/html/_static/locales/sv/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.1/_build/html/_static/locales/sv/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/_build/html/_static/locales/ta/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.1/_build/html/_static/locales/ta/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/_build/html/_static/locales/te/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.1/_build/html/_static/locales/te/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/_build/html/_static/locales/tg/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.1/_build/html/_static/locales/tg/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/_build/html/_static/locales/th/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.1/_build/html/_static/locales/th/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/_build/html/_static/locales/tl/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.1/_build/html/_static/locales/tl/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/_build/html/_static/locales/tr/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.1/_build/html/_static/locales/tr/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/_build/html/_static/locales/uk/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.1/_build/html/_static/locales/uk/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/_build/html/_static/locales/ur/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.1/_build/html/_static/locales/ur/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/_build/html/_static/locales/vi/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.1/_build/html/_static/locales/vi/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/_build/html/_static/locales/zh_CN/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.1/_build/html/_static/locales/zh_CN/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/_build/html/_static/locales/zh_TW/LC_MESSAGES/booktheme.po` & `napatrackmater-5.2.1/_build/html/_static/locales/zh_TW/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/_build/html/_static/mystnb.4510f1fc1dee50b3e5859aac5469c37c29e427902b24a333a5f9fcb2f0b3ac41.css` & `napatrackmater-5.2.1/_build/html/_static/mystnb.4510f1fc1dee50b3e5859aac5469c37c29e427902b24a333a5f9fcb2f0b3ac41.css`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/_build/html/_static/pygments.css` & `napatrackmater-5.2.1/_build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/_build/html/_static/scripts/bootstrap.js` & `napatrackmater-5.2.1/_build/html/_static/scripts/bootstrap.js`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/_build/html/_static/scripts/bootstrap.js.map` & `napatrackmater-5.2.1/_build/html/_static/scripts/bootstrap.js.map`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/_build/html/_static/scripts/pydata-sphinx-theme.js` & `napatrackmater-5.2.1/_build/html/_static/scripts/pydata-sphinx-theme.js`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/_build/html/_static/scripts/pydata-sphinx-theme.js.map` & `napatrackmater-5.2.1/_build/html/_static/scripts/pydata-sphinx-theme.js.map`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/_build/html/_static/scripts/sphinx-book-theme.js` & `napatrackmater-5.2.1/_build/html/_static/scripts/sphinx-book-theme.js`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/_build/html/_static/scripts/sphinx-book-theme.js.map` & `napatrackmater-5.2.1/_build/html/_static/scripts/sphinx-book-theme.js.map`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/_build/html/_static/searchtools.js` & `napatrackmater-5.2.1/_build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/_build/html/_static/sphinx-thebe.css` & `napatrackmater-5.2.1/_build/html/_static/sphinx-thebe.css`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/_build/html/_static/sphinx-thebe.js` & `napatrackmater-5.2.1/_build/html/_static/sphinx-thebe.js`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/_build/html/_static/styles/bootstrap.css` & `napatrackmater-5.2.1/_build/html/_static/styles/bootstrap.css`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/_build/html/_static/styles/pydata-sphinx-theme.css` & `napatrackmater-5.2.1/_build/html/_static/styles/pydata-sphinx-theme.css`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/_build/html/_static/styles/sphinx-book-theme.css` & `napatrackmater-5.2.1/_build/html/_static/styles/sphinx-book-theme.css`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/_build/html/_static/togglebutton.css` & `napatrackmater-5.2.1/_build/html/_static/togglebutton.css`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/_build/html/_static/togglebutton.js` & `napatrackmater-5.2.1/_build/html/_static/togglebutton.js`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/_build/html/_static/underscore-1.13.1.js` & `napatrackmater-5.2.1/_build/html/_static/underscore-1.13.1.js`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/_build/html/_static/underscore.js` & `napatrackmater-5.2.1/_build/html/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/_build/html/_static/vendor/fontawesome/6.1.2/LICENSE.txt` & `napatrackmater-5.2.1/_build/html/_static/vendor/fontawesome/6.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/_build/html/_static/vendor/fontawesome/6.1.2/css/all.min.css` & `napatrackmater-5.2.1/_build/html/_static/vendor/fontawesome/6.1.2/css/all.min.css`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.ttf` & `napatrackmater-5.2.1/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.woff2` & `napatrackmater-5.2.1/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.ttf` & `napatrackmater-5.2.1/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.woff2` & `napatrackmater-5.2.1/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.ttf` & `napatrackmater-5.2.1/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.woff2` & `napatrackmater-5.2.1/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.ttf` & `napatrackmater-5.2.1/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.ttf`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.woff2` & `napatrackmater-5.2.1/_build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.woff2`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/_build/html/_static/webpack-macros.html` & `napatrackmater-5.2.1/_build/html/_static/webpack-macros.html`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/_build/html/genindex.html` & `napatrackmater-5.2.1/_build/html/genindex.html`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/_build/html/search.html` & `napatrackmater-5.2.1/_build/html/search.html`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/_build/html/searchindex.js` & `napatrackmater-5.2.1/_build/html/searchindex.js`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/_build/jupyter_execute/Notebooks/Track_vector.ipynb` & `napatrackmater-5.2.1/_build/jupyter_execute/Notebooks/Track_vector.ipynb`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/_config.yml` & `napatrackmater-5.2.1/_config.yml`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/images/ClusterDistributionPlot_time_point_97.png` & `napatrackmater-5.2.1/images/ClusterDistributionPlot_time_point_97.png`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/images/ClusterNearnessPlot_time_point_97.png` & `napatrackmater-5.2.1/images/ClusterNearnessPlot_time_point_97.png`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/images/ClusterPlot_time_point_97.png` & `napatrackmater-5.2.1/images/ClusterPlot_time_point_97.png`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/images/FeatureMatrixPlot_time_point_97.png` & `napatrackmater-5.2.1/images/FeatureMatrixPlot_time_point_97.png`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/images/QuadrantDistributionPlot_time_point_97.png` & `napatrackmater-5.2.1/images/QuadrantDistributionPlot_time_point_97.png`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/images/kapoorlablogo.png` & `napatrackmater-5.2.1/images/kapoorlablogo.png`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/images/kapoorlogo.png` & `napatrackmater-5.2.1/images/kapoorlogo.png`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/setup.cfg` & `napatrackmater-5.2.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/src/napatrackmater/CloudAutoEncoder.py` & `napatrackmater-5.2.1/src/napatrackmater/CloudAutoEncoder.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/src/napatrackmater/DeepEmbeddedClustering.py` & `napatrackmater-5.2.1/src/napatrackmater/DeepEmbeddedClustering.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/src/napatrackmater/Trackmate.py` & `napatrackmater-5.2.1/src/napatrackmater/Trackmate.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/src/napatrackmater/Trackvector.py` & `napatrackmater-5.2.1/src/napatrackmater/Trackvector.py`

 * *Files 3% similar despite different names*

```diff
@@ -678,14 +678,50 @@
         )
         global_shape_dynamic_dataframe = global_shape_dynamic_dataframe.sort_values(
             by=["t"]
         )
 
         return global_shape_dynamic_dataframe
 
+    def build_closeness_dict(self, radius):
+        self.closeness_dict = {}
+
+        unique_time_points = set()
+        for track_data in self.unique_tracks.values():
+            for entry in track_data:
+                t, z, y, x = entry[1], entry[2], entry[3], entry[4]
+                unique_time_points.update(int(float(t)))
+
+        for time_point in unique_time_points:
+            coords = []
+            track_ids = []
+
+            for track_id, track_data in self.unique_tracks.items():
+                for entry in track_data:
+                    t, z, y, x = entry[1], entry[2], entry[3], entry[4]
+                    if t == time_point:
+                        coords.append([z, y, x])
+                        track_ids.append(track_id)
+
+            coords = np.array(coords)
+            track_ids = np.array(track_ids)
+
+            tree = cKDTree(coords)
+
+            closeness_dict_time_point = {}
+            for track_id, track_data in self.unique_tracks.items():
+                for entry in track_data:
+                    t, z, y, x = entry[1], entry[2], entry[3], entry[4]
+                    if t == time_point:
+                        closest_indices = tree.query_ball_point((z, y, x), r=radius)
+                        closest_track_ids = track_ids[np.concatenate(closest_indices)]
+                        closeness_dict_time_point[track_id] = list(closest_track_ids)
+
+            self.closeness_dict[time_point] = closeness_dict_time_point
+
 
 def _iterate_over_tracklets(
     track_data, training_tracklets, track_id, prediction=False, ignore_columns=[]
 ):
 
     shape_dynamic_dataframe = track_data[SHAPE_DYNAMIC_FEATURES].copy()
 
@@ -735,14 +771,79 @@
         dynamic_dataframe_list,
         full_dataframe_list,
     )
 
     return training_tracklets
 
 
+def _iterate_over_cell_type_tracklets(
+    track_data,
+    training_tracklets,
+    track_id,
+    prediction=False,
+    ignore_columns=[],
+    cell_type="Cell_Type_Label",
+):
+
+    shape_dynamic_dataframe = track_data[SHAPE_DYNAMIC_FEATURES].copy()
+
+    shape_dataframe = track_data[SHAPE_FEATURES].copy()
+
+    dynamic_dataframe = track_data[DYNAMIC_FEATURES].copy()
+
+    cell_type_track = int(float(track_data[cell_type].iloc[0]))
+
+    if not prediction:
+        full_dataframe = track_data[ALL_FEATURES].copy()
+    else:
+        full_dataframe = track_data[ALL_FEATURES - STATUS_FEATURES].copy()
+
+    if ignore_columns is not None:
+        for column in ignore_columns:
+            if column in full_dataframe.columns:
+                full_dataframe.drop(columns=[column], inplace=True)
+            if column in shape_dynamic_dataframe.columns:
+                shape_dynamic_dataframe.drop(columns=[column], inplace=True)
+            if column in shape_dataframe.columns:
+                shape_dataframe.drop(columns=[column], inplace=True)
+            if column in dynamic_dataframe.columns:
+                dynamic_dataframe.drop(columns=[column], inplace=True)
+
+    latent_columns = [
+        col for col in track_data.columns if col.startswith("latent_feature_number_")
+    ]
+    if latent_columns:
+        latent_features = track_data[latent_columns].copy()
+        full_dataframe = pd.concat([full_dataframe, latent_features], axis=1)
+        shape_dataframe = pd.concat([shape_dataframe, latent_features], axis=1)
+        shape_dynamic_dataframe = pd.concat(
+            [shape_dynamic_dataframe, latent_features], axis=1
+        )
+
+    # Drop rows with NaN values
+    shape_dynamic_dataframe.dropna(inplace=True)
+    shape_dataframe.dropna(inplace=True)
+    dynamic_dataframe.dropna(inplace=True)
+    full_dataframe.dropna(inplace=True)
+
+    shape_dynamic_dataframe_list = shape_dynamic_dataframe.to_dict(orient="records")
+    shape_dataframe_list = shape_dataframe.to_dict(orient="records")
+    dynamic_dataframe_list = dynamic_dataframe.to_dict(orient="records")
+    full_dataframe_list = full_dataframe.to_dict(orient="records")
+    training_tracklets[track_id] = (
+        shape_dynamic_dataframe_list,
+        shape_dataframe_list,
+        dynamic_dataframe_list,
+        full_dataframe_list,
+        cell_type_track,
+    )
+
+    return training_tracklets
+
+
 def create_dividing_prediction_tracklets(
     global_shape_dynamic_dataframe: pd.DataFrame, ignore_columns=[]
 ):
     training_tracklets = {}
     subset_dividing = global_shape_dynamic_dataframe[
         global_shape_dynamic_dataframe["Dividing"] == 1
     ]
@@ -828,14 +929,92 @@
         for column in ignore_columns:
             if column in modified_dataframe.columns:
                 modified_dataframe.drop(columns=[column], inplace=True)
 
     return training_tracklets, modified_dataframe
 
 
+def create_analysis_cell_type_tracklets(
+    global_shape_dynamic_dataframe: pd.DataFrame,
+    t_minus=None,
+    t_plus=None,
+    class_ratio=-1,
+    cell_type="Cell_Type_Labels",
+    ignore_columns=[],
+):
+    training_tracklets = {}
+    if t_minus is not None and t_plus is not None:
+        time_mask = (global_shape_dynamic_dataframe["t"] >= t_minus) & (
+            global_shape_dynamic_dataframe["t"] <= t_plus
+        )
+        local_shape_dynamic_dataframe = global_shape_dynamic_dataframe[time_mask]
+    else:
+        local_shape_dynamic_dataframe = global_shape_dynamic_dataframe
+
+    subset_dividing = local_shape_dynamic_dataframe[
+        local_shape_dynamic_dataframe["Dividing"] == 1
+    ]
+
+    subset_non_dividing = local_shape_dynamic_dataframe[
+        local_shape_dynamic_dataframe["Dividing"] == 0
+    ]
+    non_dividing_track_ids = subset_non_dividing["Track ID"].unique()
+    dividing_track_ids = subset_dividing["Track ID"].unique()
+    dividing_count = len(dividing_track_ids)
+    non_dividing_count = len(non_dividing_track_ids)
+    if non_dividing_count > dividing_count and class_ratio > 0:
+        non_dividing_track_ids = random.sample(
+            list(non_dividing_track_ids),
+            int(min(non_dividing_count, dividing_count * class_ratio)),
+        )
+    else:
+        dividing_track_ids = random.sample(list(dividing_track_ids), dividing_count)
+        non_dividing_track_ids = random.sample(
+            list(non_dividing_track_ids), non_dividing_count
+        )
+
+    for track_id in dividing_track_ids:
+        subset_dividing = subset_dividing.loc[
+            local_shape_dynamic_dataframe.duplicated(
+                subset=["t", "x", "y", "z"], keep=False
+            )
+        ]
+        track_data = local_shape_dynamic_dataframe[
+            (local_shape_dynamic_dataframe["Track ID"] == track_id)
+        ].sort_values(by="t")
+        if track_data.shape[0] > 0:
+            training_tracklets = _iterate_over_cell_type_tracklets(
+                track_data,
+                training_tracklets,
+                track_id,
+                ignore_columns=ignore_columns,
+                cell_type=cell_type,
+            )
+
+    for track_id in non_dividing_track_ids:
+        track_data = local_shape_dynamic_dataframe[
+            (local_shape_dynamic_dataframe["Track ID"] == track_id)
+        ].sort_values(by="t")
+        if track_data.shape[0] > 0:
+            training_tracklets = _iterate_over_cell_type_tracklets(
+                track_data,
+                training_tracklets,
+                track_id,
+                ignore_columns=ignore_columns,
+                cell_type=cell_type,
+            )
+    modified_dataframe = local_shape_dynamic_dataframe.copy()
+    if ignore_columns is not None:
+        for column in ignore_columns:
+            if column in modified_dataframe.columns:
+                modified_dataframe.drop(columns=[column], inplace=True)
+
+    return training_tracklets, modified_dataframe
+
+
 def append_data_to_npz(file_path, key, data):
     existing_data = np.load(file_path, allow_pickle=True)[key]
 
     training_data_key = []
     features_list = []
     label_dividing_list = []
     label_number_dividing_list = []
@@ -2228,14 +2407,175 @@
             cluster_eucledian_distance_map_shape_dynamic_dict,
             cluster_eucledian_distance_map_shape_dict,
             cluster_eucledian_distance_map_dynamic_dict,
             analysis_track_ids,
         )
 
 
+def convert_pseudo_tracks_to_simple_arrays(
+    analysis_vectors,
+    t_delta=10,
+    distance_vectors="shape",
+):
+
+    analysis_track_ids = []
+    shape_dynamic_eigenvectors_matrix = []
+    shape_eigenvectors_matrix = []
+    dynamic_eigenvectors_matrix = []
+    position_matrix = []
+    cell_type_ids = []
+    for track_id, (
+        shape_dynamic_dataframe_list,
+        shape_dataframe_list,
+        dynamic_dataframe_list,
+        full_dataframe_list,
+        cell_type_label,
+    ) in analysis_vectors.items():
+        shape_dynamic_track_array = np.array(
+            [
+                [item for item in record.values()]
+                for record in shape_dynamic_dataframe_list
+            ]
+        )
+        shape_track_array = np.array(
+            [[item for item in record.values()] for record in shape_dataframe_list]
+        )
+        dynamic_track_array = np.array(
+            [[item for item in record.values()] for record in dynamic_dataframe_list]
+        )
+        columns_of_interest = ["z", "y", "x"]
+        position_track_array = np.array(
+            [
+                [record[col] for col in columns_of_interest]
+                for record in full_dataframe_list
+            ]
+        )
+
+        if (
+            shape_dynamic_track_array.shape[0] > 1
+            and len(shape_dynamic_track_array.shape) > 1
+        ):
+
+            covariance_shape_dynamic = compute_raw_matrix(
+                shape_dynamic_track_array, t_delta=t_delta
+            )
+            covariance_shape = compute_raw_matrix(shape_track_array, t_delta=t_delta)
+
+            covariance_dynamic = compute_raw_matrix(
+                dynamic_track_array, t_delta=t_delta
+            )
+
+            position_computation = compute_raw_matrix(
+                position_track_array, t_delta=t_delta, take_center=True
+            )
+
+            if (
+                covariance_shape_dynamic is not None
+                and covariance_shape is not None
+                and covariance_dynamic is not None
+            ):
+
+                shape_dynamic_eigenvectors = covariance_shape_dynamic
+                shape_eigenvectors = covariance_shape
+                dynamic_eigenvectors = covariance_dynamic
+                position_vectors = position_computation
+                shape_dynamic_eigenvectors_matrix.extend(shape_dynamic_eigenvectors)
+                shape_eigenvectors_matrix.extend(shape_eigenvectors)
+                dynamic_eigenvectors_matrix.extend(dynamic_eigenvectors)
+                position_matrix.extend(position_vectors)
+                analysis_track_ids.append(track_id)
+                cell_type_ids.append(cell_type_label)
+    if (
+        len(shape_dynamic_eigenvectors_matrix) > 0
+        and len(dynamic_eigenvectors_matrix) > 0
+        and len(shape_eigenvectors_matrix) > 0
+    ):
+
+        (
+            shape_dynamic_eigenvectors_1d,
+            shape_eigenvectors_1d,
+            dynamic_eigenvectors_1d,
+            cluster_distance_map_shape_dynamic,
+            cluster_eucledian_distance_map_shape_dynamic,
+            cluster_distance_map_dynamic,
+            cluster_eucledian_distance_map_dynamic,
+            cluster_distance_map_shape,
+            cluster_eucledian_distance_map_shape,
+            analysis_track_ids,
+            cell_type_ids,
+        ) = pseudo_core_clustering(
+            shape_dynamic_eigenvectors_matrix,
+            shape_eigenvectors_matrix,
+            dynamic_eigenvectors_matrix,
+            position_matrix,
+            analysis_track_ids,
+            cell_type_ids,
+            distance_vectors=distance_vectors,
+        )
+
+        shape_dynamic_cluster_labels_dict = {
+            track_id: cluster_label
+            for track_id, cluster_label in zip(analysis_track_ids, cell_type_ids)
+        }
+        shape_cluster_labels_dict = {
+            track_id: cluster_label
+            for track_id, cluster_label in zip(analysis_track_ids, cell_type_ids)
+        }
+        dynamic_cluster_labels_dict = {
+            track_id: cluster_label
+            for track_id, cluster_label in zip(analysis_track_ids, cell_type_ids)
+        }
+
+        cluster_distance_map_shape_dynamic_dict = {
+            track_id: cluster_distance_map_shape_dynamic[cluster_label]
+            for track_id, cluster_label in zip(analysis_track_ids, cell_type_ids)
+        }
+
+        cluster_distance_map_shape_dict = {
+            track_id: cluster_distance_map_shape[cluster_label]
+            for track_id, cluster_label in zip(analysis_track_ids, cell_type_ids)
+        }
+
+        cluster_distance_map_dynamic_dict = {
+            track_id: cluster_distance_map_dynamic[cluster_label]
+            for track_id, cluster_label in zip(analysis_track_ids, cell_type_ids)
+        }
+
+        cluster_eucledian_distance_map_shape_dynamic_dict = {
+            track_id: cluster_eucledian_distance_map_shape_dynamic[cluster_label]
+            for track_id, cluster_label in zip(analysis_track_ids, cell_type_ids)
+        }
+
+        cluster_eucledian_distance_map_shape_dict = {
+            track_id: cluster_eucledian_distance_map_shape[cluster_label]
+            for track_id, cluster_label in zip(analysis_track_ids, cell_type_ids)
+        }
+
+        cluster_eucledian_distance_map_dynamic_dict = {
+            track_id: cluster_eucledian_distance_map_dynamic[cluster_label]
+            for track_id, cluster_label in zip(analysis_track_ids, cell_type_ids)
+        }
+
+        return (
+            shape_dynamic_eigenvectors_1d,
+            shape_eigenvectors_1d,
+            dynamic_eigenvectors_1d,
+            shape_dynamic_cluster_labels_dict,
+            shape_cluster_labels_dict,
+            dynamic_cluster_labels_dict,
+            cluster_distance_map_shape_dynamic_dict,
+            cluster_distance_map_shape_dict,
+            cluster_distance_map_dynamic_dict,
+            cluster_eucledian_distance_map_shape_dynamic_dict,
+            cluster_eucledian_distance_map_shape_dict,
+            cluster_eucledian_distance_map_dynamic_dict,
+            analysis_track_ids,
+        )
+
+
 def core_clustering(
     shape_dynamic_eigenvectors_matrix,
     shape_eigenvectors_matrix,
     dynamic_eigenvectors_matrix,
     position_matrix,
     analysis_track_ids,
     metric,
@@ -2518,14 +2858,89 @@
         best_cluster_eucledian_distance_map_shape_dynamic,
         best_cluster_eucledian_distance_map_shape,
         best_cluster_eucledian_distance_map_dynamic,
         analysis_track_ids,
     )
 
 
+def pseudo_core_clustering(
+    shape_dynamic_eigenvectors_matrix,
+    shape_eigenvectors_matrix,
+    dynamic_eigenvectors_matrix,
+    position_matrix,
+    analysis_track_ids,
+    cell_type_ids,
+    distance_vectors="shape",
+):
+
+    shape_dynamic_eigenvectors_3d = np.dstack(shape_dynamic_eigenvectors_matrix)
+    shape_eigenvectors_3d = np.dstack(shape_eigenvectors_matrix)
+    dynamic_eigenvectors_3d = np.dstack(dynamic_eigenvectors_matrix)
+    position_vectors_3d = np.dstack(position_matrix)
+
+    position_vector_2d = position_vectors_3d.reshape(len(analysis_track_ids), -1)
+    shape_dynamic_eigenvectors_2d = shape_dynamic_eigenvectors_3d.reshape(
+        len(analysis_track_ids), -1
+    )
+    shape_eigenvectors_2d = shape_eigenvectors_3d.reshape(len(analysis_track_ids), -1)
+    dynamic_eigenvectors_2d = dynamic_eigenvectors_3d.reshape(
+        len(analysis_track_ids), -1
+    )
+
+    shape_dynamic_eigenvectors_1d = np.array(shape_dynamic_eigenvectors_2d)
+    shape_eigenvectors_1d = np.array(shape_eigenvectors_2d)
+    dynamic_eigenvectors_1d = np.array(dynamic_eigenvectors_2d)
+    position_vector_1d = np.array(position_vector_2d)
+    compute_vectors_shape = shape_eigenvectors_1d
+    compute_vectors_dynamic = dynamic_eigenvectors_1d
+    if distance_vectors == "shape":
+        compute_vectors = shape_eigenvectors_1d
+    if distance_vectors == "dynamic":
+        compute_vectors = dynamic_eigenvectors_1d
+    if distance_vectors == "shape_and_dynamic":
+        compute_vectors = shape_dynamic_eigenvectors_1d
+    else:
+        compute_vectors = shape_eigenvectors_1d
+
+    cluster_distance_map_shape_dynamic = calculate_intercluster_distance(
+        compute_vectors, cell_type_ids
+    )
+    cluster_eucledian_distance_map_shape_dynamic = (
+        calculate_intercluster_eucledian_distance(position_vector_1d, cell_type_ids)
+    )
+
+    cluster_distance_map_dynamic = calculate_intercluster_distance(
+        compute_vectors_shape, cell_type_ids
+    )
+    cluster_eucledian_distance_map_dynamic = calculate_intercluster_eucledian_distance(
+        position_vector_1d, cell_type_ids
+    )
+
+    cluster_distance_map_shape = calculate_intercluster_distance(
+        compute_vectors_dynamic, cell_type_ids
+    )
+    cluster_eucledian_distance_map_shape = calculate_intercluster_eucledian_distance(
+        position_vector_1d, cell_type_ids
+    )
+
+    return (
+        shape_dynamic_eigenvectors_1d,
+        shape_eigenvectors_1d,
+        dynamic_eigenvectors_1d,
+        cluster_distance_map_shape_dynamic,
+        cluster_eucledian_distance_map_shape_dynamic,
+        cluster_distance_map_dynamic,
+        cluster_eucledian_distance_map_dynamic,
+        cluster_distance_map_shape,
+        cluster_eucledian_distance_map_shape,
+        analysis_track_ids,
+        cell_type_ids,
+    )
+
+
 def compute_raw_matrix(track_arrays, t_delta, take_center=False):
     track_duration = track_arrays.shape[0]
     t_delta = int(t_delta)
 
     if track_duration < t_delta:
         repetitions = t_delta - track_duration
         last_row = track_arrays[-1, :]
@@ -2997,31 +3412,33 @@
 ):
 
     for trackmate_track_id in unique_trackmate_track_ids:
         subset = global_shape_dynamic_dataframe[
             (global_shape_dynamic_dataframe["TrackMate Track ID"] == trackmate_track_id)
         ].sort_values(by="t")
         sorted_subset = sorted(subset["Track ID"].unique())
-        for count, tracklet_id in enumerate(sorted_subset):
+        for tracklet_id in sorted_subset:
 
             dividing_track_track_data = global_shape_dynamic_dataframe[
                 (global_shape_dynamic_dataframe["Track ID"] == tracklet_id)
             ].sort_values(by="t")
-            generation_id = int(float(dividing_track_track_data["Generation ID"][0]))
+            generation_id = int(
+                float(dividing_track_track_data["Generation ID"].iloc[0])
+            )
 
             track_start_time = dividing_track_track_data["t"].min()
             track_end_time = dividing_track_track_data["t"].max()
 
-            if count == 0:
+            if generation_id == 0:
                 zero_gen_tracklets[trackmate_track_id] = (
                     tracklet_id,
                     track_start_time,
                     track_end_time,
                 )
-            elif count > 0:
+            elif generation_id > 0:
                 if trackmate_track_id in daughter_generations[generation_id]:
                     daughter_generations[generation_id][trackmate_track_id].append(
                         (tracklet_id, track_start_time, track_end_time)
                     )
                 else:
                     daughter_generations[generation_id][trackmate_track_id] = [
                         (tracklet_id, track_start_time, track_end_time)
@@ -3241,14 +3658,19 @@
 
 
 def create_cluster_plot(
     dataframe,
     cluster_type,
     cluster_distance_type,
     cluster_eucledian_distance_type,
+    unique_col_names=[
+        "Cluster_Label_Distances",
+        "Cluster_Label_Eucledian_Distances",
+        "Cluster_Label",
+    ],
     negate_cluster_type=None,
     track_duration=0,
     show_plot=False,
     negate_cluster_distance_type=None,
     negate_cluster_eucledian_distance_type=None,
 ):
 
@@ -3325,15 +3747,15 @@
             append_name = "Shape_Dynamic_"
         elif re.search(r"\bShape\b", cluster_column):
             append_name = "Shape_"
         elif re.search(r"\bDynamic\b", cluster_column):
             append_name = "Dynamic_"
 
         tinit = time_veto
-    df_time_clusters_melted[append_name + "Cluster_Label"] = data
+    df_time_clusters_melted[append_name + unique_col_names[-1]] = data
 
     data = []
     eucledian_data = []
     tinit = 0
     for index, cluster_distance_column in enumerate(cluster_distance_columns):
         if index == len(cluster_distance_columns) - 1:
             time_veto = dataframe["t"].max()
@@ -3381,34 +3803,32 @@
             (df_time_clusters_melted["t"] > tstart)
             & (df_time_clusters_melted["t"] <= tend)
         ]
 
         eucledian_data.extend(filtered_df[cluster_eucledian_distance_column].tolist())
         tinit = time_veto
 
-    df_time_clusters_melted[append_name + "Cluster_Label_Distances"] = data
-    df_time_clusters_melted[
-        append_name + "Cluster_Label_Eucledian_Distances"
-    ] = eucledian_data
+    df_time_clusters_melted[append_name + unique_col_names[0]] = data
+    df_time_clusters_melted[append_name + unique_col_names[1]] = eucledian_data
 
     df_time_clusters_melted = df_time_clusters_melted.drop(columns=cluster_columns)
     df_time_clusters_melted = df_time_clusters_melted.drop(
         columns=cluster_distance_columns
     )
     df_time_clusters_melted = df_time_clusters_melted.drop(
         columns=cluster_eucledian_distance_columns
     )
     df_time_clusters_melted = df_time_clusters_melted.dropna(
-        subset=append_name + "Cluster_Label"
+        subset=append_name + unique_col_names[-1]
     )
     df_time_clusters_melted = df_time_clusters_melted.dropna(
-        subset=append_name + "Cluster_Label_Distances"
+        subset=append_name + unique_col_names[0]
     )
     df_time_clusters_melted = df_time_clusters_melted.dropna(
-        subset=append_name + "Cluster_Label_Eucledian_Distances"
+        subset=append_name + unique_col_names[1]
     )
 
     return df_time_clusters_melted
 
 
 def extract_number_from_string(string):
     pattern = r"\d+\.?\d*"
@@ -3429,15 +3849,15 @@
         by="Track Duration", ascending=False
     )
 
     unique_trackmate_track_ids = sorted_dividing_dataframe[
         "TrackMate Track ID"
     ].unique()
     zero_gen_tracklets = {}
-    daughter_generations = {i: {} for i in range(1, generation_max)}
+    daughter_generations = {i: {} for i in range(1, generation_max + 1)}
     get_zero_gen_daughter_generations(
         unique_trackmate_track_ids,
         global_shape_dynamic_dataframe,
         zero_gen_tracklets,
         daughter_generations,
     )
```

### Comparing `napatrackmater-5.1.9/src/napatrackmater/__init__.py` & `napatrackmater-5.2.1/src/napatrackmater/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from .pretrained import register_model, register_aliases, clear_models_and_aliases
 from .clustering import Clustering
 from .Trackmate import TrackMate, get_feature_dict
+
 from .Trackvector import (
     TrackVector,
     convert_tracks_to_arrays,
     unsupervised_clustering,
     simple_unsupervised_clustering,
     supervised_clustering,
     create_global_gt_dataframe,
@@ -19,15 +20,20 @@
     load_prediction_data,
     create_embeddings_with_gt,
     create_analysis_tracklets,
     create_dividing_prediction_tracklets,
     convert_tracks_to_simple_arrays,
     local_track_covaraince,
     cell_fate_recipe,
+    core_clustering,
+    pseudo_core_clustering,
+    convert_pseudo_tracks_to_simple_arrays,
+    create_analysis_cell_type_tracklets,
 )
+
 from .CloudAutoEncoder import CloudAutoEncoder
 import json
 from csbdeep.utils.tf import keras_import
 from tifffile import imread
 import os
 
 get_file = keras_import("utils", "get_file")
@@ -88,14 +94,18 @@
     "plot_metrics_from_npz",
     "load_prediction_data",
     "create_embeddings_with_gt",
     "create_analysis_tracklets",
     "local_track_covaraince",
     "create_dividing_prediction_tracklets",
     "cell_fate_recipe",
+    "core_clustering",
+    "pseudo_core_clustering",
+    "convert_pseudo_tracks_to_simple_arrays",
+    "create_analysis_cell_type_tracklets",
 )
 
 clear_models_and_aliases(CloudAutoEncoder)
 
 register_model(
     CloudAutoEncoder,
     "xenopus_nuclei_autoencoder",
```

### Comparing `napatrackmater-5.1.9/src/napatrackmater/clustering.py` & `napatrackmater-5.2.1/src/napatrackmater/clustering.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/src/napatrackmater/fast_radius_regression.py` & `napatrackmater-5.2.1/src/napatrackmater/fast_radius_regression.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/src/napatrackmater/fate_mapping.py` & `napatrackmater-5.2.1/src/napatrackmater/fate_mapping.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/src/napatrackmater/pretrained.py` & `napatrackmater-5.2.1/src/napatrackmater/pretrained.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/src/napatrackmater.egg-info/PKG-INFO` & `napatrackmater-5.2.1/src/napatrackmater.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napatrackmater
-Version: 5.1.9
+Version: 5.2.1
 Summary: Import Trackmate XML files for Track Visualization and analysis in Napari.
 Home-page: https://github.com/Kapoorlabs-CAPED/napatrackmater
 Author: Varun Kapoor, Mari Tolonen, Jakub Sedzinski
 Author-email: randomaccessiblekapoor@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/Kapoorlabs-CAPED/napatrackmater/issues
 Project-URL: Documentation, https://github.com/Kapoorlabs-CAPED/napatrackmater#README.md
```

### Comparing `napatrackmater-5.1.9/src/napatrackmater.egg-info/SOURCES.txt` & `napatrackmater-5.2.1/src/napatrackmater.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `napatrackmater-5.1.9/update_version.py` & `napatrackmater-5.2.1/update_version.py`

 * *Files identical despite different names*

