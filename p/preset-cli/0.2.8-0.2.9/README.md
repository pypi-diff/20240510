# Comparing `tmp/preset-cli-0.2.8.tar.gz` & `tmp/preset-cli-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "preset-cli-0.2.8.tar", last modified: Wed Sep 13 16:38:01 2023, max compression
+gzip compressed data, was "preset-cli-0.2.9.tar", last modified: Wed Jan 10 15:31:04 2024, max compression
```

## Comparing `preset-cli-0.2.8.tar` & `preset-cli-0.2.9.tar`

### file list

```diff
@@ -1,150 +1,150 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 16:38:01.680925 preset-cli-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (127)      593 2023-09-13 16:37:51.000000 preset-cli-0.2.8/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)      125 2023-09-13 16:37:51.000000 preset-cli-0.2.8/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 16:38:01.636925 preset-cli-0.2.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 16:38:01.648925 preset-cli-0.2.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      929 2023-09-13 16:37:51.000000 preset-cli-0.2.8/.github/workflows/python-package-daily.yml
--rw-r--r--   0 runner    (1001) docker     (127)      984 2023-09-13 16:37:51.000000 preset-cli-0.2.8/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2023-09-13 16:37:51.000000 preset-cli-0.2.8/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      610 2023-09-13 16:37:51.000000 preset-cli-0.2.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       58 2023-09-13 16:37:51.000000 preset-cli-0.2.8/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2261 2023-09-13 16:37:51.000000 preset-cli-0.2.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      191 2023-09-13 16:37:51.000000 preset-cli-0.2.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)      490 2023-09-13 16:37:51.000000 preset-cli-0.2.8/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)       81 2023-09-13 16:37:51.000000 preset-cli-0.2.8/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)    12064 2023-09-13 16:37:51.000000 preset-cli-0.2.8/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)    13862 2023-09-13 16:37:51.000000 preset-cli-0.2.8/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-09-13 16:37:51.000000 preset-cli-0.2.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      732 2023-09-13 16:37:51.000000 preset-cli-0.2.8/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)    26220 2023-09-13 16:38:01.680925 preset-cli-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    24105 2023-09-13 16:37:51.000000 preset-cli-0.2.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       19 2023-09-13 16:37:51.000000 preset-cli-0.2.8/dev-requirements.in
--rw-r--r--   0 runner    (1001) docker     (127)     1499 2023-09-13 16:37:51.000000 preset-cli-0.2.8/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 16:38:01.652925 preset-cli-0.2.8/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2023-09-13 16:37:51.000000 preset-cli-0.2.8/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 16:38:01.652925 preset-cli-0.2.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2023-09-13 16:37:51.000000 preset-cli-0.2.8/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       41 2023-09-13 16:37:51.000000 preset-cli-0.2.8/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (127)       43 2023-09-13 16:37:51.000000 preset-cli-0.2.8/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9753 2023-09-13 16:37:51.000000 preset-cli-0.2.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2023-09-13 16:37:51.000000 preset-cli-0.2.8/docs/contributing.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 16:38:01.652925 preset-cli-0.2.8/docs/images/
--rw-r--r--   0 runner    (1001) docker     (127)   271378 2023-09-13 16:37:51.000000 preset-cli-0.2.8/docs/images/export_dashboards.png
--rw-r--r--   0 runner    (1001) docker     (127)     2325 2023-09-13 16:37:51.000000 preset-cli-0.2.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       67 2023-09-13 16:37:51.000000 preset-cli-0.2.8/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (127)       39 2023-09-13 16:37:51.000000 preset-cli-0.2.8/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (127)      233 2023-09-13 16:37:51.000000 preset-cli-0.2.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 16:38:01.636925 preset-cli-0.2.8/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 16:38:01.652925 preset-cli-0.2.8/examples/exports/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 16:38:01.652925 preset-cli-0.2.8/examples/exports/charts/
--rw-r--r--   0 runner    (1001) docker     (127)      946 2023-09-13 16:37:51.000000 preset-cli-0.2.8/examples/exports/charts/Total_count_134.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 16:38:01.652925 preset-cli-0.2.8/examples/exports/dashboards/
--rw-r--r--   0 runner    (1001) docker     (127)      920 2023-09-13 16:37:51.000000 preset-cli-0.2.8/examples/exports/dashboards/White_label_test.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 16:38:01.652925 preset-cli-0.2.8/examples/exports/databases/
--rw-r--r--   0 runner    (1001) docker     (127)      452 2023-09-13 16:37:51.000000 preset-cli-0.2.8/examples/exports/databases/Google_Sheets.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 16:38:01.636925 preset-cli-0.2.8/examples/exports/datasets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 16:38:01.652925 preset-cli-0.2.8/examples/exports/datasets/Google_Sheets/
--rw-r--r--   0 runner    (1001) docker     (127)      943 2023-09-13 16:37:51.000000 preset-cli-0.2.8/examples/exports/datasets/Google_Sheets/country_cnt.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 16:38:01.656925 preset-cli-0.2.8/examples/exports/functions/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2023-09-13 16:37:51.000000 preset-cli-0.2.8/examples/exports/functions/demo.py
--rw-r--r--   0 runner    (1001) docker     (127)       61 2023-09-13 16:37:51.000000 preset-cli-0.2.8/examples/exports/metadata.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      355 2023-09-13 16:37:51.000000 preset-cli-0.2.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       10 2023-09-13 16:37:51.000000 preset-cli-0.2.8/requirements.in
--rw-r--r--   0 runner    (1001) docker     (127)      850 2023-09-13 16:37:51.000000 preset-cli-0.2.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2118 2023-09-13 16:38:01.680925 preset-cli-0.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      708 2023-09-13 16:37:51.000000 preset-cli-0.2.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 16:38:01.640925 preset-cli-0.2.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 16:38:01.656925 preset-cli-0.2.8/src/preset_cli/
--rw-r--r--   0 runner    (1001) docker     (127)      404 2023-09-13 16:37:51.000000 preset-cli-0.2.8/src/preset_cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 16:38:01.656925 preset-cli-0.2.8/src/preset_cli/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-13 16:37:51.000000 preset-cli-0.2.8/src/preset_cli/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 16:38:01.660925 preset-cli-0.2.8/src/preset_cli/api/clients/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-13 16:37:51.000000 preset-cli-0.2.8/src/preset_cli/api/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21072 2023-09-13 16:37:51.000000 preset-cli-0.2.8/src/preset_cli/api/clients/dbt.py
--rw-r--r--   0 runner    (1001) docker     (127)     8520 2023-09-13 16:37:51.000000 preset-cli-0.2.8/src/preset_cli/api/clients/preset.py
--rw-r--r--   0 runner    (1001) docker     (127)    39273 2023-09-13 16:37:51.000000 preset-cli-0.2.8/src/preset_cli/api/clients/superset.py
--rw-r--r--   0 runner    (1001) docker     (127)      454 2023-09-13 16:37:51.000000 preset-cli-0.2.8/src/preset_cli/api/operators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 16:38:01.660925 preset-cli-0.2.8/src/preset_cli/auth/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-13 16:37:51.000000 preset-cli-0.2.8/src/preset_cli/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      794 2023-09-13 16:37:51.000000 preset-cli-0.2.8/src/preset_cli/auth/jwt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1694 2023-09-13 16:37:51.000000 preset-cli-0.2.8/src/preset_cli/auth/lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2023-09-13 16:37:51.000000 preset-cli-0.2.8/src/preset_cli/auth/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     1602 2023-09-13 16:37:51.000000 preset-cli-0.2.8/src/preset_cli/auth/preset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2245 2023-09-13 16:37:51.000000 preset-cli-0.2.8/src/preset_cli/auth/superset.py
--rw-r--r--   0 runner    (1001) docker     (127)      400 2023-09-13 16:37:51.000000 preset-cli-0.2.8/src/preset_cli/auth/token.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 16:38:01.664925 preset-cli-0.2.8/src/preset_cli/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-13 16:37:51.000000 preset-cli-0.2.8/src/preset_cli/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20200 2023-09-13 16:37:51.000000 preset-cli-0.2.8/src/preset_cli/cli/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 16:38:01.664925 preset-cli-0.2.8/src/preset_cli/cli/superset/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-13 16:37:51.000000 preset-cli-0.2.8/src/preset_cli/cli/superset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8974 2023-09-13 16:37:51.000000 preset-cli-0.2.8/src/preset_cli/cli/superset/export.py
--rw-r--r--   0 runner    (1001) docker     (127)     1809 2023-09-13 16:37:51.000000 preset-cli-0.2.8/src/preset_cli/cli/superset/import_.py
--rw-r--r--   0 runner    (1001) docker     (127)     3607 2023-09-13 16:37:51.000000 preset-cli-0.2.8/src/preset_cli/cli/superset/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     5136 2023-09-13 16:37:51.000000 preset-cli-0.2.8/src/preset_cli/cli/superset/sql.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 16:38:01.664925 preset-cli-0.2.8/src/preset_cli/cli/superset/sync/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-13 16:37:51.000000 preset-cli-0.2.8/src/preset_cli/cli/superset/sync/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 16:38:01.668925 preset-cli-0.2.8/src/preset_cli/cli/superset/sync/dbt/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-13 16:37:51.000000 preset-cli-0.2.8/src/preset_cli/cli/superset/sync/dbt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13977 2023-09-13 16:37:51.000000 preset-cli-0.2.8/src/preset_cli/cli/superset/sync/dbt/command.py
--rw-r--r--   0 runner    (1001) docker     (127)     3080 2023-09-13 16:37:51.000000 preset-cli-0.2.8/src/preset_cli/cli/superset/sync/dbt/databases.py
--rw-r--r--   0 runner    (1001) docker     (127)     8427 2023-09-13 16:37:51.000000 preset-cli-0.2.8/src/preset_cli/cli/superset/sync/dbt/datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     5541 2023-09-13 16:37:51.000000 preset-cli-0.2.8/src/preset_cli/cli/superset/sync/dbt/exposures.py
--rw-r--r--   0 runner    (1001) docker     (127)    14063 2023-09-13 16:37:51.000000 preset-cli-0.2.8/src/preset_cli/cli/superset/sync/dbt/lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     3554 2023-09-13 16:37:51.000000 preset-cli-0.2.8/src/preset_cli/cli/superset/sync/dbt/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)      480 2023-09-13 16:37:51.000000 preset-cli-0.2.8/src/preset_cli/cli/superset/sync/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 16:38:01.668925 preset-cli-0.2.8/src/preset_cli/cli/superset/sync/native/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-13 16:37:51.000000 preset-cli-0.2.8/src/preset_cli/cli/superset/sync/native/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12026 2023-09-13 16:37:51.000000 preset-cli-0.2.8/src/preset_cli/cli/superset/sync/native/command.py
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2023-09-13 16:37:51.000000 preset-cli-0.2.8/src/preset_cli/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3282 2023-09-13 16:37:51.000000 preset-cli-0.2.8/src/preset_cli/lib.py
--rw-r--r--   0 runner    (1001) docker     (127)      231 2023-09-13 16:37:51.000000 preset-cli-0.2.8/src/preset_cli/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 16:38:01.656925 preset-cli-0.2.8/src/preset_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    26220 2023-09-13 16:38:01.000000 preset-cli-0.2.8/src/preset_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3468 2023-09-13 16:38:01.000000 preset-cli-0.2.8/src/preset_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-13 16:38:01.000000 preset-cli-0.2.8/src/preset_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      119 2023-09-13 16:38:01.000000 preset-cli-0.2.8/src/preset_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-13 16:38:01.000000 preset-cli-0.2.8/src/preset_cli.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      573 2023-09-13 16:38:01.000000 preset-cli-0.2.8/src/preset_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2023-09-13 16:38:01.000000 preset-cli-0.2.8/src/preset_cli.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 16:38:01.668925 preset-cli-0.2.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-13 16:37:51.000000 preset-cli-0.2.8/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 16:38:01.668925 preset-cli-0.2.8/tests/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-13 16:37:51.000000 preset-cli-0.2.8/tests/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 16:38:01.672925 preset-cli-0.2.8/tests/api/clients/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-13 16:37:51.000000 preset-cli-0.2.8/tests/api/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    53266 2023-09-13 16:37:51.000000 preset-cli-0.2.8/tests/api/clients/dbt_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    14306 2023-09-13 16:37:51.000000 preset-cli-0.2.8/tests/api/clients/preset_test.py
--rw-r--r--   0 runner    (1001) docker     (127)   112580 2023-09-13 16:37:51.000000 preset-cli-0.2.8/tests/api/clients/superset_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 16:38:01.672925 preset-cli-0.2.8/tests/auth/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-13 16:37:51.000000 preset-cli-0.2.8/tests/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1568 2023-09-13 16:37:51.000000 preset-cli-0.2.8/tests/auth/jwt_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2198 2023-09-13 16:37:51.000000 preset-cli-0.2.8/tests/auth/lib_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      743 2023-09-13 16:37:51.000000 preset-cli-0.2.8/tests/auth/main_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2772 2023-09-13 16:37:51.000000 preset-cli-0.2.8/tests/auth/preset_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2414 2023-09-13 16:37:51.000000 preset-cli-0.2.8/tests/auth/superset_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 16:38:01.676925 preset-cli-0.2.8/tests/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-13 16:37:51.000000 preset-cli-0.2.8/tests/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    52395 2023-09-13 16:37:51.000000 preset-cli-0.2.8/tests/cli/main_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 16:38:01.676925 preset-cli-0.2.8/tests/cli/superset/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-13 16:37:51.000000 preset-cli-0.2.8/tests/cli/superset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23405 2023-09-13 16:37:51.000000 preset-cli-0.2.8/tests/cli/superset/export_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2881 2023-09-13 16:37:51.000000 preset-cli-0.2.8/tests/cli/superset/import_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3778 2023-09-13 16:37:51.000000 preset-cli-0.2.8/tests/cli/superset/main_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    11781 2023-09-13 16:37:51.000000 preset-cli-0.2.8/tests/cli/superset/sql_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 16:38:01.676925 preset-cli-0.2.8/tests/cli/superset/sync/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-13 16:37:51.000000 preset-cli-0.2.8/tests/cli/superset/sync/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 16:38:01.676925 preset-cli-0.2.8/tests/cli/superset/sync/dbt/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-13 16:37:51.000000 preset-cli-0.2.8/tests/cli/superset/sync/dbt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    44862 2023-09-13 16:37:51.000000 preset-cli-0.2.8/tests/cli/superset/sync/dbt/command_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    12870 2023-09-13 16:37:51.000000 preset-cli-0.2.8/tests/cli/superset/sync/dbt/databases_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    40272 2023-09-13 16:37:51.000000 preset-cli-0.2.8/tests/cli/superset/sync/dbt/datasets_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    28144 2023-09-13 16:37:51.000000 preset-cli-0.2.8/tests/cli/superset/sync/dbt/exposures_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    18083 2023-09-13 16:37:51.000000 preset-cli-0.2.8/tests/cli/superset/sync/dbt/lib_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     9424 2023-09-13 16:37:51.000000 preset-cli-0.2.8/tests/cli/superset/sync/dbt/manifest.json
--rw-r--r--   0 runner    (1001) docker     (127)    12183 2023-09-13 16:37:51.000000 preset-cli-0.2.8/tests/cli/superset/sync/dbt/metrics_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 16:38:01.676925 preset-cli-0.2.8/tests/cli/superset/sync/native/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-13 16:37:51.000000 preset-cli-0.2.8/tests/cli/superset/sync/native/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31905 2023-09-13 16:37:51.000000 preset-cli-0.2.8/tests/cli/superset/sync/native/command_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      278 2023-09-13 16:37:51.000000 preset-cli-0.2.8/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3006 2023-09-13 16:37:51.000000 preset-cli-0.2.8/tests/lib_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2007 2023-09-13 16:37:51.000000 preset-cli-0.2.8/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 15:31:04.973593 preset-cli-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-01-10 15:30:56.000000 preset-cli-0.2.9/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-01-10 15:30:56.000000 preset-cli-0.2.9/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 15:31:04.945593 preset-cli-0.2.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 15:31:04.953593 preset-cli-0.2.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-01-10 15:30:56.000000 preset-cli-0.2.9/.github/workflows/python-package-daily.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-01-10 15:30:56.000000 preset-cli-0.2.9/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-01-10 15:30:56.000000 preset-cli-0.2.9/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-01-10 15:30:56.000000 preset-cli-0.2.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-01-10 15:30:56.000000 preset-cli-0.2.9/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2261 2024-01-10 15:30:56.000000 preset-cli-0.2.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-01-10 15:30:56.000000 preset-cli-0.2.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-01-10 15:30:56.000000 preset-cli-0.2.9/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-01-10 15:30:56.000000 preset-cli-0.2.9/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    12241 2024-01-10 15:30:56.000000 preset-cli-0.2.9/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    13862 2024-01-10 15:30:56.000000 preset-cli-0.2.9/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-10 15:30:56.000000 preset-cli-0.2.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-01-10 15:30:56.000000 preset-cli-0.2.9/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    26216 2024-01-10 15:31:04.973593 preset-cli-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    24105 2024-01-10 15:30:56.000000 preset-cli-0.2.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-01-10 15:30:56.000000 preset-cli-0.2.9/dev-requirements.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-01-10 15:30:56.000000 preset-cli-0.2.9/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 15:31:04.953593 preset-cli-0.2.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-01-10 15:30:56.000000 preset-cli-0.2.9/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 15:31:04.953593 preset-cli-0.2.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-01-10 15:30:56.000000 preset-cli-0.2.9/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-01-10 15:30:56.000000 preset-cli-0.2.9/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-01-10 15:30:56.000000 preset-cli-0.2.9/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9753 2024-01-10 15:30:56.000000 preset-cli-0.2.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-01-10 15:30:56.000000 preset-cli-0.2.9/docs/contributing.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 15:31:04.953593 preset-cli-0.2.9/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (127)   271378 2024-01-10 15:30:56.000000 preset-cli-0.2.9/docs/images/export_dashboards.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-01-10 15:30:56.000000 preset-cli-0.2.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-01-10 15:30:56.000000 preset-cli-0.2.9/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-01-10 15:30:56.000000 preset-cli-0.2.9/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-01-10 15:30:56.000000 preset-cli-0.2.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 15:31:04.945593 preset-cli-0.2.9/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 15:31:04.957594 preset-cli-0.2.9/examples/exports/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 15:31:04.957594 preset-cli-0.2.9/examples/exports/charts/
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-01-10 15:30:56.000000 preset-cli-0.2.9/examples/exports/charts/Total_count_134.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 15:31:04.957594 preset-cli-0.2.9/examples/exports/dashboards/
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-01-10 15:30:56.000000 preset-cli-0.2.9/examples/exports/dashboards/White_label_test.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 15:31:04.957594 preset-cli-0.2.9/examples/exports/databases/
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-01-10 15:30:56.000000 preset-cli-0.2.9/examples/exports/databases/Google_Sheets.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 15:31:04.945593 preset-cli-0.2.9/examples/exports/datasets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 15:31:04.957594 preset-cli-0.2.9/examples/exports/datasets/Google_Sheets/
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-01-10 15:30:56.000000 preset-cli-0.2.9/examples/exports/datasets/Google_Sheets/country_cnt.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 15:31:04.957594 preset-cli-0.2.9/examples/exports/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-01-10 15:30:56.000000 preset-cli-0.2.9/examples/exports/functions/demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-01-10 15:30:56.000000 preset-cli-0.2.9/examples/exports/metadata.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-01-10 15:30:56.000000 preset-cli-0.2.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-01-10 15:30:56.000000 preset-cli-0.2.9/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-01-10 15:30:56.000000 preset-cli-0.2.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-01-10 15:31:04.973593 preset-cli-0.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-01-10 15:30:56.000000 preset-cli-0.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 15:31:04.949593 preset-cli-0.2.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 15:31:04.957594 preset-cli-0.2.9/src/preset_cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-01-10 15:30:56.000000 preset-cli-0.2.9/src/preset_cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 15:31:04.957594 preset-cli-0.2.9/src/preset_cli/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-10 15:30:56.000000 preset-cli-0.2.9/src/preset_cli/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 15:31:04.957594 preset-cli-0.2.9/src/preset_cli/api/clients/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-10 15:30:56.000000 preset-cli-0.2.9/src/preset_cli/api/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24933 2024-01-10 15:30:56.000000 preset-cli-0.2.9/src/preset_cli/api/clients/dbt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8520 2024-01-10 15:30:56.000000 preset-cli-0.2.9/src/preset_cli/api/clients/preset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39628 2024-01-10 15:30:56.000000 preset-cli-0.2.9/src/preset_cli/api/clients/superset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-01-10 15:30:56.000000 preset-cli-0.2.9/src/preset_cli/api/operators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 15:31:04.961593 preset-cli-0.2.9/src/preset_cli/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-10 15:30:56.000000 preset-cli-0.2.9/src/preset_cli/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-01-10 15:30:56.000000 preset-cli-0.2.9/src/preset_cli/auth/jwt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-01-10 15:30:56.000000 preset-cli-0.2.9/src/preset_cli/auth/lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-01-10 15:30:56.000000 preset-cli-0.2.9/src/preset_cli/auth/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-01-10 15:30:56.000000 preset-cli-0.2.9/src/preset_cli/auth/preset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-01-10 15:30:56.000000 preset-cli-0.2.9/src/preset_cli/auth/superset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-01-10 15:30:56.000000 preset-cli-0.2.9/src/preset_cli/auth/token.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 15:31:04.961593 preset-cli-0.2.9/src/preset_cli/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-10 15:30:56.000000 preset-cli-0.2.9/src/preset_cli/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20200 2024-01-10 15:30:56.000000 preset-cli-0.2.9/src/preset_cli/cli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 15:31:04.961593 preset-cli-0.2.9/src/preset_cli/cli/superset/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-10 15:30:56.000000 preset-cli-0.2.9/src/preset_cli/cli/superset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8974 2024-01-10 15:30:56.000000 preset-cli-0.2.9/src/preset_cli/cli/superset/export.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-01-10 15:30:56.000000 preset-cli-0.2.9/src/preset_cli/cli/superset/import_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3607 2024-01-10 15:30:56.000000 preset-cli-0.2.9/src/preset_cli/cli/superset/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5144 2024-01-10 15:30:56.000000 preset-cli-0.2.9/src/preset_cli/cli/superset/sql.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 15:31:04.961593 preset-cli-0.2.9/src/preset_cli/cli/superset/sync/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-10 15:30:56.000000 preset-cli-0.2.9/src/preset_cli/cli/superset/sync/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 15:31:04.965593 preset-cli-0.2.9/src/preset_cli/cli/superset/sync/dbt/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-10 15:30:56.000000 preset-cli-0.2.9/src/preset_cli/cli/superset/sync/dbt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15632 2024-01-10 15:30:56.000000 preset-cli-0.2.9/src/preset_cli/cli/superset/sync/dbt/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3080 2024-01-10 15:30:56.000000 preset-cli-0.2.9/src/preset_cli/cli/superset/sync/dbt/databases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7649 2024-01-10 15:30:56.000000 preset-cli-0.2.9/src/preset_cli/cli/superset/sync/dbt/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5704 2024-01-10 15:30:56.000000 preset-cli-0.2.9/src/preset_cli/cli/superset/sync/dbt/exposures.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14063 2024-01-10 15:30:56.000000 preset-cli-0.2.9/src/preset_cli/cli/superset/sync/dbt/lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10445 2024-01-10 15:30:56.000000 preset-cli-0.2.9/src/preset_cli/cli/superset/sync/dbt/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-01-10 15:30:56.000000 preset-cli-0.2.9/src/preset_cli/cli/superset/sync/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 15:31:04.965593 preset-cli-0.2.9/src/preset_cli/cli/superset/sync/native/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-10 15:30:56.000000 preset-cli-0.2.9/src/preset_cli/cli/superset/sync/native/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12026 2024-01-10 15:30:56.000000 preset-cli-0.2.9/src/preset_cli/cli/superset/sync/native/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-01-10 15:30:56.000000 preset-cli-0.2.9/src/preset_cli/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3282 2024-01-10 15:30:56.000000 preset-cli-0.2.9/src/preset_cli/lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-01-10 15:30:56.000000 preset-cli-0.2.9/src/preset_cli/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 15:31:04.969593 preset-cli-0.2.9/src/preset_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    26216 2024-01-10 15:31:04.000000 preset-cli-0.2.9/src/preset_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3468 2024-01-10 15:31:04.000000 preset-cli-0.2.9/src/preset_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-10 15:31:04.000000 preset-cli-0.2.9/src/preset_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-01-10 15:31:04.000000 preset-cli-0.2.9/src/preset_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-10 15:31:04.000000 preset-cli-0.2.9/src/preset_cli.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-01-10 15:31:04.000000 preset-cli-0.2.9/src/preset_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-01-10 15:31:04.000000 preset-cli-0.2.9/src/preset_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 15:31:04.965593 preset-cli-0.2.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-10 15:30:56.000000 preset-cli-0.2.9/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 15:31:04.965593 preset-cli-0.2.9/tests/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-10 15:30:56.000000 preset-cli-0.2.9/tests/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 15:31:04.965593 preset-cli-0.2.9/tests/api/clients/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-10 15:30:56.000000 preset-cli-0.2.9/tests/api/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55176 2024-01-10 15:30:56.000000 preset-cli-0.2.9/tests/api/clients/dbt_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14306 2024-01-10 15:30:56.000000 preset-cli-0.2.9/tests/api/clients/preset_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)   112580 2024-01-10 15:30:56.000000 preset-cli-0.2.9/tests/api/clients/superset_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 15:31:04.965593 preset-cli-0.2.9/tests/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-10 15:30:56.000000 preset-cli-0.2.9/tests/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-01-10 15:30:56.000000 preset-cli-0.2.9/tests/auth/jwt_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-01-10 15:30:56.000000 preset-cli-0.2.9/tests/auth/lib_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-01-10 15:30:56.000000 preset-cli-0.2.9/tests/auth/main_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2772 2024-01-10 15:30:56.000000 preset-cli-0.2.9/tests/auth/preset_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-01-10 15:30:56.000000 preset-cli-0.2.9/tests/auth/superset_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 15:31:04.965593 preset-cli-0.2.9/tests/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-10 15:30:56.000000 preset-cli-0.2.9/tests/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52395 2024-01-10 15:30:56.000000 preset-cli-0.2.9/tests/cli/main_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 15:31:04.969593 preset-cli-0.2.9/tests/cli/superset/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-10 15:30:56.000000 preset-cli-0.2.9/tests/cli/superset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23405 2024-01-10 15:30:56.000000 preset-cli-0.2.9/tests/cli/superset/export_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2881 2024-01-10 15:30:56.000000 preset-cli-0.2.9/tests/cli/superset/import_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3778 2024-01-10 15:30:56.000000 preset-cli-0.2.9/tests/cli/superset/main_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11781 2024-01-10 15:30:56.000000 preset-cli-0.2.9/tests/cli/superset/sql_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 15:31:04.969593 preset-cli-0.2.9/tests/cli/superset/sync/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-10 15:30:56.000000 preset-cli-0.2.9/tests/cli/superset/sync/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 15:31:04.969593 preset-cli-0.2.9/tests/cli/superset/sync/dbt/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-10 15:30:56.000000 preset-cli-0.2.9/tests/cli/superset/sync/dbt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48570 2024-01-10 15:30:56.000000 preset-cli-0.2.9/tests/cli/superset/sync/dbt/command_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12870 2024-01-10 15:30:56.000000 preset-cli-0.2.9/tests/cli/superset/sync/dbt/databases_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40103 2024-01-10 15:30:56.000000 preset-cli-0.2.9/tests/cli/superset/sync/dbt/datasets_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28182 2024-01-10 15:30:56.000000 preset-cli-0.2.9/tests/cli/superset/sync/dbt/exposures_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18083 2024-01-10 15:30:56.000000 preset-cli-0.2.9/tests/cli/superset/sync/dbt/lib_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9666 2024-01-10 15:30:56.000000 preset-cli-0.2.9/tests/cli/superset/sync/dbt/manifest.json
+-rw-r--r--   0 runner    (1001) docker     (127)    24986 2024-01-10 15:30:56.000000 preset-cli-0.2.9/tests/cli/superset/sync/dbt/metrics_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 15:31:04.969593 preset-cli-0.2.9/tests/cli/superset/sync/native/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-10 15:30:56.000000 preset-cli-0.2.9/tests/cli/superset/sync/native/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31905 2024-01-10 15:30:56.000000 preset-cli-0.2.9/tests/cli/superset/sync/native/command_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-01-10 15:30:56.000000 preset-cli-0.2.9/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3006 2024-01-10 15:30:56.000000 preset-cli-0.2.9/tests/lib_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-01-10 15:30:56.000000 preset-cli-0.2.9/tox.ini
```

### Comparing `preset-cli-0.2.8/.coveragerc` & `preset-cli-0.2.9/.coveragerc`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.8/.github/workflows/python-package-daily.yml` & `preset-cli-0.2.9/.github/workflows/python-package-daily.yml`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.8/.github/workflows/python-package.yml` & `preset-cli-0.2.9/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.8/.github/workflows/python-publish.yml` & `preset-cli-0.2.9/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.8/.gitignore` & `preset-cli-0.2.9/.gitignore`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.8/.pre-commit-config.yaml` & `preset-cli-0.2.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.8/CHANGELOG.rst` & `preset-cli-0.2.9/CHANGELOG.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 =========
 Changelog
 =========
 
 Next
 ====
 
+Version 0.2.9 - 2024-01-10
+==========================
+
+- Initial support for syncing metrics from dbt/MetricFlow (`#256 <https://github.com/preset-io/backend-sdk/pull/256>_`).
+
 Version 0.2.8 - 2023-09-12
 ==========================
 
 - The Jinja rendering/escaping logic for content migration was improved (`#237 <https://github.com/preset-io/backend-sdk/pull/237>_`).
 - It's now possible to specify dbt models to be synced using the file name/path  (`#242 <https://github.com/preset-io/backend-sdk/pull/242>_`).
 
 Version 0.2.7 - 2023-09-08
```

### Comparing `preset-cli-0.2.8/CONTRIBUTING.rst` & `preset-cli-0.2.9/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.8/Makefile` & `preset-cli-0.2.9/Makefile`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.8/PKG-INFO` & `preset-cli-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: preset-cli
-Version: 0.2.8
+Version: 0.2.9
 Summary: A CLI to interact with Preset (https://preset.io/) workspaces.
 Home-page: https://github.com/preset-io/backend-sdk
 Author: Beto Dealmeida
 Author-email: beto@preset.io
 License: Other/Proprietary License
 Project-URL: Documentation, https://github.com/preset-io/backend-sdk/blob/master/README.rst
 Platform: any
@@ -31,15 +31,15 @@
 Requires-Dist: prison>=0.2.1
 Requires-Dist: prompt-toolkit>=3.0.24
 Requires-Dist: pygments>=2.11.2
 Requires-Dist: python-graphql-client>=0.4.3
 Requires-Dist: requests>=2.26.0
 Requires-Dist: rich>=12.3.0
 Requires-Dist: sqlalchemy<2,>=1.4
-Requires-Dist: sqlparse>=0.4.3
+Requires-Dist: sqlglot>=19
 Requires-Dist: tabulate>=0.8.9
 Requires-Dist: typing-extensions>=4.0.1
 Requires-Dist: yarl>=1.7.2
 Requires-Dist: greenlet>=1.1.3
 Requires-Dist: aiohttp>=3.8.3
 Provides-Extra: testing
 Requires-Dist: setuptools; extra == "testing"
```

### Comparing `preset-cli-0.2.8/README.rst` & `preset-cli-0.2.9/README.rst`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.8/dev-requirements.txt` & `preset-cli-0.2.9/dev-requirements.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #
-# This file is autogenerated by pip-compile with python 3.8
-# To update, run:
+# This file is autogenerated by pip-compile with Python 3.8
+# by the following command:
 #
 #    pip-compile --no-annotate dev-requirements.in
 #
 -e file:.
 aiohttp==3.8.3
 aiosignal==1.2.0
 appdirs==1.4.4
@@ -63,15 +63,15 @@
 pyyaml==6.0
 requests==2.27.1
 requests-mock==1.9.3
 rich==12.5.1
 six==1.16.0
 soupsieve==2.3.2.post1
 sqlalchemy==1.4.40
-sqlparse==0.4.3
+sqlglot==20.7.1
 tabulate==0.8.10
 toml==0.10.2
 tomli==2.0.1
 tomlkit==0.11.6
 typing-extensions==4.3.0
 urllib3==1.26.9
 virtualenv==20.16.3
```

### Comparing `preset-cli-0.2.8/docs/Makefile` & `preset-cli-0.2.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.8/docs/conf.py` & `preset-cli-0.2.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.8/docs/images/export_dashboards.png` & `preset-cli-0.2.9/docs/images/export_dashboards.png`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.8/docs/index.rst` & `preset-cli-0.2.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.8/examples/exports/charts/Total_count_134.yaml` & `preset-cli-0.2.9/examples/exports/charts/Total_count_134.yaml`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.8/examples/exports/dashboards/White_label_test.yaml` & `preset-cli-0.2.9/examples/exports/dashboards/White_label_test.yaml`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.8/examples/exports/datasets/Google_Sheets/country_cnt.yaml` & `preset-cli-0.2.9/examples/exports/datasets/Google_Sheets/country_cnt.yaml`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.8/requirements.txt` & `preset-cli-0.2.9/requirements.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #
-# This file is autogenerated by pip-compile with python 3.8
-# To update, run:
+# This file is autogenerated by pip-compile with Python 3.8
+# by the following command:
 #
 #    pip-compile --no-annotate
 #
 -e file:.
 aiohttp==3.8.3
 aiosignal==1.2.0
 appdirs==1.4.4
@@ -36,14 +36,14 @@
 pytz==2022.1
 pyyaml==6.0
 requests==2.27.1
 rich==12.3.0
 six==1.16.0
 soupsieve==2.3.2.post1
 sqlalchemy==1.4.35
-sqlparse==0.4.3
+sqlglot==20.7.1
 tabulate==0.8.9
 typing-extensions==4.2.0
 urllib3==1.26.9
 wcwidth==0.2.5
 websockets==10.3
 yarl==1.7.2
```

### Comparing `preset-cli-0.2.8/setup.cfg` & `preset-cli-0.2.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 	prison>=0.2.1
 	prompt-toolkit>=3.0.24
 	pygments>=2.11.2
 	python-graphql-client>=0.4.3
 	requests>=2.26.0
 	rich>=12.3.0
 	sqlalchemy>=1.4,<2
-	sqlparse>=0.4.3
+	sqlglot>=19
 	tabulate>=0.8.9
 	typing-extensions>=4.0.1
 	yarl>=1.7.2
 	greenlet>=1.1.3  # required for Python 3.11
 	aiohttp>=3.8.3
 
 [options.packages.find]
```

### Comparing `preset-cli-0.2.8/setup.py` & `preset-cli-0.2.9/setup.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.8/src/preset_cli/api/clients/dbt.py` & `preset-cli-0.2.9/src/preset_cli/api/clients/dbt.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,15 +20,18 @@
 
 from preset_cli import __version__
 from preset_cli.auth.main import Auth
 
 _logger = logging.getLogger(__name__)
 
 REST_ENDPOINT = URL("https://cloud.getdbt.com/")
-GRAPHQL_ENDPOINT = URL("https://metadata.cloud.getdbt.com/graphql")
+METADATA_GRAPHQL_ENDPOINT = URL("https://metadata.cloud.getdbt.com/graphql")
+SEMANTIC_LAYER_GRAPHQL_ENDPOINT = URL(
+    "https://semantic-layer.cloud.getdbt.com/api/graphql",
+)
 
 
 class PostelSchema(Schema):
     """
     Be liberal in what you accept, and conservative in what you send.
 
     A schema that allows unknown fields. This way if the API returns new fields that
@@ -468,15 +471,15 @@
     type = PostelEnumField(TimeType, required=True)
     interval = fields.Integer(allow_none=True)
     hours = fields.List(fields.Integer(), allow_none=True)
 
 
 class StringOrSchema(fields.Field):
     """
-    Dynamic schema constructor for fields that could have a string or another schema
+    Dynamic schema constructor for fields that could have a string or another schema.
     """
 
     def __init__(self, nested_schema, *args, **kwargs):
         self.nested_schema = nested_schema
         super().__init__(*args, **kwargs)
 
     def _deserialize(self, value, attr, data, **kwargs):
@@ -583,14 +586,58 @@
     type = fields.String()
     unique_id = fields.String(data_key="uniqueId")
     # dbt >= 1.3
     calculation_method = fields.String()
     expression = fields.String()
 
 
+class MFMetricType(str, Enum):
+    """
+    Type of the MetricFlow metric.
+    """
+
+    SIMPLE = "SIMPLE"
+    RATIO = "RATIO"
+    CUMULATIVE = "CUMULATIVE"
+    DERIVED = "DERIVED"
+
+
+class MFMetricSchema(PostelSchema):
+    """
+    Schema for a MetricFlow metric.
+    """
+
+    name = fields.String()
+    description = fields.String()
+    type = PostelEnumField(MFMetricType)
+
+
+class MFSQLEngine(str, Enum):
+    """
+    Databases supported by MetricFlow.
+    """
+
+    BIGQUERY = "BIGQUERY"
+    DUCKDB = "DUCKDB"
+    REDSHIFT = "REDSHIFT"
+    POSTGRES = "POSTGRES"
+    SNOWFLAKE = "SNOWFLAKE"
+    DATABRICKS = "DATABRICKS"
+
+
+class MFMetricWithSQLSchema(MFMetricSchema):
+    """
+    MetricFlow metric with dialect and SQL, as well as model.
+    """
+
+    sql = fields.String()
+    dialect = PostelEnumField(MFSQLEngine)
+    model = fields.String()
+
+
 class DataResponse(TypedDict):
     """
     Type for the GraphQL response.
     """
 
     data: Dict[str, Any]
 
@@ -598,33 +645,26 @@
 class DBTClient:  # pylint: disable=too-few-public-methods
 
     """
     A client for the dbt API.
     """
 
     def __init__(self, auth: Auth):
-        self.graphql_client = GraphqlClient(endpoint=GRAPHQL_ENDPOINT)
+        self.metadata_graphql_client = GraphqlClient(endpoint=METADATA_GRAPHQL_ENDPOINT)
+        self.semantic_layer_graphql_client = GraphqlClient(
+            endpoint=SEMANTIC_LAYER_GRAPHQL_ENDPOINT,
+        )
         self.baseurl = REST_ENDPOINT
 
         self.session = auth.session
         self.session.headers.update(auth.get_headers())
         self.session.headers["User-Agent"] = "Preset CLI"
         self.session.headers["X-Client-Version"] = __version__
         self.session.headers["X-dbt-partner-source"] = "preset"
 
-    def execute(self, query: str, **variables: Any) -> DataResponse:
-        """
-        Run a GraphQL query.
-        """
-        return self.graphql_client.execute(
-            query=query,
-            variables=variables,
-            headers=self.session.headers,
-        )
-
     def get_accounts(self) -> List[AccountSchema]:
         """
         List all accounts.
         """
         url = self.baseurl / "api/v2/accounts/"
         _logger.debug("GET %s", url)
         response = self.session.get(url)
@@ -679,45 +719,54 @@
         return jobs
 
     def get_models(self, job_id: int) -> List[ModelSchema]:
         """
         Fetch all available models.
         """
         query = """
-            query ($jobId: Int!) {
-                models(jobId: $jobId) {
-                    uniqueId
-                    dependsOn
-                    childrenL1
-                    name
-                    database
-                    schema
-                    description
-                    meta
-                    tags
-                    columns {
+            query Models($jobId: BigInt!) {
+                job(id: $jobId) {
+                    models {
+                        uniqueId
+                        dependsOn
+                        childrenL1
                         name
+                        database
+                        schema
                         description
+                        meta
+                        tags
+                        columns {
+                            name
+                            description
+                            type
+                        }
                     }
                 }
             }
         """
-        payload = self.execute(query, jobId=job_id)
+        payload = self.metadata_graphql_client.execute(
+            query=query,
+            variables={"jobId": job_id},
+            headers=self.session.headers,
+        )
 
         model_schema = ModelSchema()
-        models = [model_schema.load(model) for model in payload["data"]["models"]]
+        models = [
+            model_schema.load(model) for model in payload["data"]["job"]["models"]
+        ]
 
         return models
 
-    def get_metrics(self, job_id: int) -> List[Any]:
+    def get_og_metrics(self, job_id: int) -> List[MetricSchema]:
         """
         Fetch all available metrics.
         """
         query = """
-            query ($jobId: Int!) {
+            query GetMetrics($jobId: Int!) {
                 metrics(jobId: $jobId) {
                     uniqueId
                     name
                     label
                     type
                     sql
                     filters {
@@ -727,21 +776,106 @@
                     }
                     dependsOn
                     description
                     meta
                 }
             }
         """
-        payload = self.execute(query, jobId=job_id)
+        payload = self.metadata_graphql_client.execute(
+            query=query,
+            variables={"jobId": job_id},
+            headers=self.session.headers,
+        )
 
         metric_schema = MetricSchema()
         metrics = [metric_schema.load(metric) for metric in payload["data"]["metrics"]]
 
         return metrics
 
+    def get_sl_metrics(self, environment_id: int) -> List[MFMetricSchema]:
+        """
+        Fetch all available metrics.
+        """
+        query = """
+            query GetMetrics($environmentId: BigInt!) {
+                metrics(environmentId: $environmentId) {
+                    name
+                    description
+                    type
+                }
+            }
+        """
+        payload = self.semantic_layer_graphql_client.execute(
+            query=query,
+            variables={"environmentId": environment_id},
+            headers=self.session.headers,
+        )
+
+        metric_schema = MFMetricSchema()
+        metrics = [metric_schema.load(metric) for metric in payload["data"]["metrics"]]
+
+        return metrics
+
+    def get_sl_metric_sql(self, metric: str, environment_id: int) -> Optional[str]:
+        """
+        Fetch metric SQL.
+
+        We fetch one metric at a time because if one metric fails to compile, the entire
+        query fails.
+        """
+        query = """
+            mutation CompileSql($environmentId: BigInt!, $metricsInput: [MetricInput!]) {
+                compileSql(
+                    environmentId: $environmentId
+                    metrics: $metricsInput
+                    groupBy: []
+                ) {
+                    sql
+                }
+            }
+        """
+        payload = self.semantic_layer_graphql_client.execute(
+            query=query,
+            variables={
+                "environmentId": environment_id,
+                "metricsInput": [{"name": metric}],
+            },
+            headers=self.session.headers,
+        )
+
+        if payload["data"] is None:
+            errors = "\n\n".join(
+                error["message"] for error in payload.get("errors", [])
+            )
+            _logger.warning("Unable to convert metric %s: %s", metric, errors)
+            return None
+
+        return payload["data"]["compileSql"]["sql"]
+
+    def get_sl_dialect(self, environment_id: int) -> MFSQLEngine:
+        """
+        Get the dialect used in the MetricFlow project.
+        """
+        query = """
+            query GetEnvironmentInfo($environmentId: BigInt!) {
+                environmentInfo(environmentId: $environmentId) {
+                    dialect
+                }
+            }
+        """
+        payload = self.semantic_layer_graphql_client.execute(
+            query=query,
+            variables={"environmentId": environment_id},
+            headers=self.session.headers,
+        )
+
+        return MFSQLEngine(payload["data"]["environmentInfo"]["dialect"])
+
+    # def get_sl_metric_sql(self,
+
     def get_database_name(self, job_id: int) -> str:
         """
         Return the database name.
 
         This is done by querying all models in a job. As far as I know there should be
         only one database associated with them.
         """
```

### Comparing `preset-cli-0.2.8/src/preset_cli/api/clients/preset.py` & `preset-cli-0.2.9/src/preset_cli/api/clients/preset.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.8/src/preset_cli/api/clients/superset.py` & `preset-cli-0.2.9/src/preset_cli/api/clients/superset.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 A simple client for running SQL queries (and more) against Superset:
 
     >>> from yarl import URL
     >>> from preset_cli.api.clients.superset import SupersetClient
-    >>> from preset_cli.auth.password import UsernamePasswordAuth
+    >>> from preset_cli.auth.superset import UsernamePasswordAuth
     >>> url = URL("http://localhost:8088/")
     >>> auth = UsernamePasswordAuth(url, "admin", "admin")  # doctest: +SKIP
     >>> client = SupersetClient(url, auth)  # doctest: +SKIP
     >>> sql = "SELECT platform, rank FROM video_game_sales LIMIT 2"
     >>> print(client.run_query(database_id=1, sql=sql))  # doctest: +SKIP
       platform  rank
     0      Wii     1
@@ -132,14 +132,34 @@
         "isNew": False,
         "label": expression,
         "optionName": f"metric_{uuid4()}",
         "sqlExpression": expression,
     }
 
 
+class SupersetMetricDefinition(TypedDict, total=False):
+    """
+    Definition of a Superset metric.
+
+    Used in the PUT API for datasets.
+    """
+
+    id: int
+    expression: str
+    metric_name: str
+    metric_type: str
+    verbose_name: str
+    description: str
+    extra: str
+    warning_text: str
+    d3format: str
+    currency: str
+    uuid: str
+
+
 class ColumnType(TypedDict):
     """
     Schema for an adhoc column in the Chart API.
     """
 
     label: str
     sqlExpression: str
```

### Comparing `preset-cli-0.2.8/src/preset_cli/auth/jwt.py` & `preset-cli-0.2.9/src/preset_cli/auth/jwt.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.8/src/preset_cli/auth/lib.py` & `preset-cli-0.2.9/src/preset_cli/auth/lib.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.8/src/preset_cli/auth/main.py` & `preset-cli-0.2.9/src/preset_cli/auth/main.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.8/src/preset_cli/auth/preset.py` & `preset-cli-0.2.9/src/preset_cli/auth/preset.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.8/src/preset_cli/auth/superset.py` & `preset-cli-0.2.9/src/preset_cli/auth/superset.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.8/src/preset_cli/cli/main.py` & `preset-cli-0.2.9/src/preset_cli/cli/main.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.8/src/preset_cli/cli/superset/export.py` & `preset-cli-0.2.9/src/preset_cli/cli/superset/export.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.8/src/preset_cli/cli/superset/import_.py` & `preset-cli-0.2.9/src/preset_cli/cli/superset/import_.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.8/src/preset_cli/cli/superset/main.py` & `preset-cli-0.2.9/src/preset_cli/cli/superset/main.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.8/src/preset_cli/cli/superset/sql.py` & `preset-cli-0.2.9/src/preset_cli/cli/superset/sql.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,22 +11,22 @@
 from prompt_toolkit import PromptSession
 from prompt_toolkit.completion import WordCompleter
 from prompt_toolkit.history import FileHistory
 from prompt_toolkit.lexers import PygmentsLexer
 from prompt_toolkit.styles.pygments import style_from_pygments_cls
 from pygments.lexers.sql import SqlLexer
 from pygments.styles import get_style_by_name
-from sqlparse.keywords import KEYWORDS
+from sqlglot.tokens import Tokenizer
 from tabulate import tabulate
 from yarl import URL
 
 from preset_cli.api.clients.superset import SupersetClient
 from preset_cli.exceptions import SupersetError
 
-sql_completer = WordCompleter(list(KEYWORDS))
+sql_completer = WordCompleter(list(Tokenizer.KEYWORDS))
 style = style_from_pygments_cls(get_style_by_name("stata-dark"))
 
 
 @click.command()
 @click.option(
     "--database-id",
     default=None,
```

### Comparing `preset-cli-0.2.8/src/preset_cli/cli/superset/sync/dbt/command.py` & `preset-cli-0.2.9/src/preset_cli/cli/superset/sync/dbt/command.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,27 +2,38 @@
 A command to sync dbt models/metrics to Superset and charts/dashboards back as exposures.
 """
 
 import os.path
 import sys
 import warnings
 from pathlib import Path
-from typing import Optional, Tuple
+from typing import List, Optional, Tuple
 
 import click
 import yaml
 from yarl import URL
 
-from preset_cli.api.clients.dbt import DBTClient, MetricSchema, ModelSchema
+from preset_cli.api.clients.dbt import (
+    DBTClient,
+    JobSchema,
+    MetricSchema,
+    MFMetricWithSQLSchema,
+    ModelSchema,
+)
 from preset_cli.api.clients.superset import SupersetClient
 from preset_cli.auth.token import TokenAuth
 from preset_cli.cli.superset.sync.dbt.databases import sync_database
 from preset_cli.cli.superset.sync.dbt.datasets import sync_datasets
 from preset_cli.cli.superset.sync.dbt.exposures import ModelKey, sync_exposures
 from preset_cli.cli.superset.sync.dbt.lib import apply_select
+from preset_cli.cli.superset.sync.dbt.metrics import (
+    MultipleModelsError,
+    get_model_from_sql,
+    get_superset_metrics_per_model,
+)
 from preset_cli.exceptions import DatabaseNotFoundError
 
 
 @click.command()
 @click.argument("file", type=click.Path(exists=True, resolve_path=True))
 @click.option("--project", help="Name of the dbt project", default=None)
 @click.option("--target", help="Target name", default=None)
@@ -176,33 +187,32 @@
         if config["resource_type"] == "model":
             # conform to the same schema that dbt Cloud uses for models
             unique_id = config["uniqueId"] = config["unique_id"]
             config["children"] = configs["child_map"][unique_id]
             config["columns"] = list(config["columns"].values())
             models.append(model_schema.load(config))
     models = apply_select(models, select, exclude)
-    model_map = {
-        ModelKey(model["schema"], model["name"]): f"ref('{model['name']}')"
-        for model in models
-    }
+    model_map = {ModelKey(model["schema"], model["name"]): model for model in models}
 
     if exposures_only:
         datasets = [
             dataset
             for dataset in client.get_datasets()
             if ModelKey(dataset["schema"], dataset["table_name"]) in model_map
         ]
     else:
-        metrics = []
+        og_metrics = []
         metric_schema = MetricSchema()
         for config in configs["metrics"].values():
             # conform to the same schema that dbt Cloud uses for metrics
             config["dependsOn"] = config.pop("depends_on")["nodes"]
             config["uniqueId"] = config.pop("unique_id")
-            metrics.append(metric_schema.load(config))
+            og_metrics.append(metric_schema.load(config))
+
+        superset_metrics = get_superset_metrics_per_model(og_metrics)
 
         try:
             database = sync_database(
                 client,
                 Path(profiles),
                 project,
                 profile,
@@ -214,15 +224,15 @@
         except DatabaseNotFoundError:
             click.echo("No database was found, pass ``--import-db`` to create")
             return
 
         datasets = sync_datasets(
             client,
             models,
-            metrics,
+            superset_metrics,
             database,
             disallow_edits,
             external_url_prefix,
             reload_columns=reload_columns,
             merge_metadata=merge_metadata,
         )
 
@@ -278,46 +288,55 @@
         except Exception:  # pylint: disable=broad-except
             choice = -1
         if 0 < choice <= len(projects):
             return projects[choice - 1]["id"]
         click.echo("Invalid choice")
 
 
-def get_job_id(
+def get_job(
     client: DBTClient,
     account_id: Optional[int] = None,
     project_id: Optional[int] = None,
-) -> int:
+    job_id: Optional[int] = None,
+) -> JobSchema:
     """
     Prompt users for a job ID.
     """
     if account_id is None:
         account_id = get_account_id(client)
     if project_id is None:
         project_id = get_project_id(client, account_id)
 
     jobs = client.get_jobs(account_id, project_id)
     if not jobs:
         click.echo(click.style("No jobs available", fg="bright_red"))
         sys.exit(1)
-    if len(jobs) == 1:
-        return jobs[0]["id"]
 
-    click.echo("Choose a job:")
-    for i, job in enumerate(jobs):
-        click.echo(f'({i+1}) {job["name"]}')
+    if job_id is None:
+        if len(jobs) == 1:
+            return jobs[0]
 
-    while True:
-        try:
-            choice = int(input("> "))
-        except Exception:  # pylint: disable=broad-except
-            choice = -1
-        if 0 < choice <= len(jobs):
-            return jobs[choice - 1]["id"]
-        click.echo("Invalid choice")
+        click.echo("Choose a job:")
+        for i, job in enumerate(jobs):
+            click.echo(f'({i+1}) {job["name"]}')
+
+        while True:
+            try:
+                choice = int(input("> "))
+            except Exception:  # pylint: disable=broad-except
+                choice = -1
+            if 0 < choice <= len(jobs):
+                return jobs[choice - 1]
+            click.echo("Invalid choice")
+
+    for job in jobs:
+        if job["id"] == job_id:
+            return job
+
+    raise ValueError(f"Job {job_id} not available")
 
 
 @click.command()
 @click.argument("token")
 @click.argument("job_id", type=click.INT, required=False, default=None)
 @click.option(
     "--disallow-edits",
@@ -403,48 +422,77 @@
             ),
         )
         sys.exit(1)
 
     reload_columns = not (preserve_columns or preserve_metadata or merge_metadata)
     preserve_metadata = preserve_columns if preserve_columns else preserve_metadata
 
-    if job_id is None:
-        job_id = get_job_id(dbt_client)
+    try:
+        job = get_job(dbt_client, job_id=job_id)
+    except ValueError:
+        click.echo(click.style(f"Job {job_id} not available", fg="bright_red"))
+        sys.exit(2)
 
     # with dbt cloud the database must already exist
-    database_name = dbt_client.get_database_name(job_id)
+    database_name = dbt_client.get_database_name(job["id"])
     databases = superset_client.get_databases(database_name=database_name)
     if not databases:
         click.echo(f'No database named "{database_name}" was found')
         return
     if len(databases) > 1:
         raise Exception("More than one database with the same name found")
 
     # need to get the database by itself so the response has the SQLAlchemy URI
     database = superset_client.get_database(databases[0]["id"])
 
-    models = dbt_client.get_models(job_id)
+    models = dbt_client.get_models(job["id"])
     models = apply_select(models, select, exclude)
-    model_map = {
-        ModelKey(model["schema"], model["name"]): f"ref('{model['name']}')"
-        for model in models
-    }
-    metrics = dbt_client.get_metrics(job_id)
+    model_map = {ModelKey(model["schema"], model["name"]): model for model in models}
+
+    # original dbt <= 1.6 metrics
+    og_metrics = dbt_client.get_og_metrics(job["id"])
+
+    # MetricFlow metrics
+    dialect = dbt_client.get_sl_dialect(job["environment_id"])
+    mf_metric_schema = MFMetricWithSQLSchema()
+    sl_metrics: List[MFMetricWithSQLSchema] = []
+    for metric in dbt_client.get_sl_metrics(job["environment_id"]):
+        sql = dbt_client.get_sl_metric_sql(metric["name"], job["environment_id"])
+        if sql is not None:
+            try:
+                model = get_model_from_sql(sql, dialect, model_map)
+            except MultipleModelsError:
+                continue
+
+            sl_metrics.append(
+                mf_metric_schema.load(
+                    {
+                        "name": metric["name"],
+                        "type": metric["type"],
+                        "description": metric["description"],
+                        "sql": sql,
+                        "dialect": dialect.value,
+                        "model": model["unique_id"],
+                    },
+                ),
+            )
+
+    superset_metrics = get_superset_metrics_per_model(og_metrics, sl_metrics)
 
     if exposures_only:
         datasets = [
             dataset
             for dataset in superset_client.get_datasets()
             if ModelKey(dataset["schema"], dataset["table_name"]) in model_map
         ]
     else:
         datasets = sync_datasets(
             superset_client,
             models,
-            metrics,
+            superset_metrics,
             database,
             disallow_edits,
             external_url_prefix,
             reload_columns=reload_columns,
             merge_metadata=merge_metadata,
         )
```

### Comparing `preset-cli-0.2.8/src/preset_cli/cli/superset/sync/dbt/databases.py` & `preset-cli-0.2.9/src/preset_cli/cli/superset/sync/dbt/databases.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.8/src/preset_cli/cli/superset/sync/dbt/datasets.py` & `preset-cli-0.2.9/src/preset_cli/cli/superset/sync/dbt/datasets.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,21 +9,17 @@
 from typing import Any, Dict, List, Optional
 
 from sqlalchemy.engine import create_engine
 from sqlalchemy.engine.url import URL as SQLAlchemyURL
 from sqlalchemy.engine.url import make_url
 from yarl import URL
 
-from preset_cli.api.clients.dbt import MetricSchema, ModelSchema
-from preset_cli.api.clients.superset import SupersetClient
+from preset_cli.api.clients.dbt import ModelSchema
+from preset_cli.api.clients.superset import SupersetClient, SupersetMetricDefinition
 from preset_cli.api.operators import OneToMany
-from preset_cli.cli.superset.sync.dbt.metrics import (
-    get_metric_expression,
-    get_metrics_for_model,
-)
 
 DEFAULT_CERTIFICATION = {"details": "This table is produced by dbt"}
 
 _logger = logging.getLogger(__name__)
 
 
 def model_in_database(model: ModelSchema, url: SQLAlchemyURL) -> bool:
@@ -79,15 +75,15 @@
 
     return client.create_dataset(**kwargs)
 
 
 def sync_datasets(  # pylint: disable=too-many-locals, too-many-branches, too-many-arguments, too-many-statements # noqa:C901
     client: SupersetClient,
     models: List[ModelSchema],
-    metrics: List[MetricSchema],
+    metrics: Dict[str, List[SupersetMetricDefinition]],
     database: Any,
     disallow_edits: bool,
     external_url_prefix: str,
     certification: Optional[Dict[str, Any]] = None,
     reload_columns: bool = True,
     merge_metadata: bool = False,
 ) -> List[Any]:
@@ -142,45 +138,31 @@
                 {},
             ),  # include any additional or custom field specified in model.meta.superset.extra
         }
 
         dataset_metrics = []
         current_metrics = {}
         model_metrics = {
-            metric["name"]: metric for metric in get_metrics_for_model(model, metrics)
+            metric["metric_name"]: metric
+            for metric in metrics.get(model["unique_id"], [])
         }
 
         if not reload_columns:
             current_metrics = {
                 metric["metric_name"]: metric
                 for metric in client.get_dataset(dataset["id"])["metrics"]
             }
             for name, metric in current_metrics.items():
                 # remove data that is not part of the update payload
                 metric = clean_metadata(metric)
                 if not merge_metadata or name not in model_metrics:
                     dataset_metrics.append(metric)
 
-        for name, metric in model_metrics.items():
-            meta = metric.get("meta", {})
-            kwargs = meta.pop("superset", {})
-
+        for name, metric_definition in model_metrics.items():
             if reload_columns or name not in current_metrics or merge_metadata:
-                metric_definition = {
-                    "expression": get_metric_expression(name, model_metrics),
-                    "metric_name": name,
-                    "metric_type": (
-                        metric.get("type")  # dbt < 1.3
-                        or metric.get("calculation_method")  # dbt >= 1.3
-                    ),
-                    "verbose_name": metric.get("label", name),
-                    "description": metric.get("description", ""),
-                    "extra": json.dumps(meta),
-                    **kwargs,  # include additional metric metadata defined in metric.meta.superset
-                }
                 if merge_metadata and name in current_metrics:
                     metric_definition["id"] = current_metrics[name]["id"]
                 dataset_metrics.append(metric_definition)
 
         # update dataset metadata from dbt and clearing metrics
         update = {
             "description": model.get("description", ""),
```

### Comparing `preset-cli-0.2.8/src/preset_cli/cli/superset/sync/dbt/exposures.py` & `preset-cli-0.2.9/src/preset_cli/cli/superset/sync/dbt/exposures.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import json
 import re
 from pathlib import Path
 from typing import Any, Dict, List, NamedTuple, Optional
 
 import yaml
 
+from preset_cli.api.clients.dbt import ModelSchema
 from preset_cli.api.clients.superset import SupersetClient
 
 # XXX: DashboardResponseType and DatasetResponseType
 
 
 class ModelKey(NamedTuple):
     """
@@ -22,15 +23,15 @@
     schema: Optional[str]
     table: str
 
 
 def get_chart_depends_on(
     client: SupersetClient,
     chart: Any,
-    model_map: Dict[ModelKey, str],
+    model_map: Dict[ModelKey, ModelSchema],
 ) -> List[str]:
     """
     Get all the dbt dependencies for a given chart.
     """
 
     # imported charts have a null query context until loaded in Explore for the first time.
     # in that case, we can get the dataset id from the params
@@ -46,23 +47,24 @@
     dataset = client.get_dataset(dataset_id)
     extra = json.loads(dataset["extra"] or "{}")
     if "depends_on" in extra:
         return [extra["depends_on"]]
 
     key = ModelKey(dataset["schema"], dataset["table_name"])
     if dataset["datasource_type"] == "table" and key in model_map:
-        return [model_map[key]]
+        model = model_map[key]
+        return [f"ref('{model['name']}')"]
 
     return []
 
 
 def get_dashboard_depends_on(
     client: SupersetClient,
     dashboard: Any,
-    model_map: Dict[ModelKey, str],
+    model_map: Dict[ModelKey, ModelSchema],
 ) -> List[str]:
     """
     Get all the dbt dependencies for a given dashboard.
     """
 
     url = client.baseurl / "api/v1/dashboard" / str(dashboard["id"]) / "datasets"
 
@@ -81,24 +83,25 @@
         except json.decoder.JSONDecodeError:
             extra = {}
 
         key = ModelKey(full_dataset["schema"], full_dataset["table_name"])
         if "depends_on" in extra:
             depends_on.append(extra["depends_on"])
         elif full_dataset["datasource_type"] == "table" and key in model_map:
-            depends_on.append(model_map[key])
+            model = model_map[key]
+            depends_on.append(f"ref('{model['name']}')")
 
     return depends_on
 
 
 def sync_exposures(  # pylint: disable=too-many-locals
     client: SupersetClient,
     exposures_path: Path,
     datasets: List[Any],
-    model_map: Dict[ModelKey, str],
+    model_map: Dict[ModelKey, ModelSchema],
 ) -> None:
     """
     Write dashboards back to dbt as exposures.
     """
     exposures = []
     charts_ids = set()
     dashboards_ids = set()
```

### Comparing `preset-cli-0.2.8/src/preset_cli/cli/superset/sync/dbt/lib.py` & `preset-cli-0.2.9/src/preset_cli/cli/superset/sync/dbt/lib.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.8/src/preset_cli/cli/superset/sync/native/command.py` & `preset-cli-0.2.9/src/preset_cli/cli/superset/sync/native/command.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.8/src/preset_cli/exceptions.py` & `preset-cli-0.2.9/src/preset_cli/exceptions.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.8/src/preset_cli/lib.py` & `preset-cli-0.2.9/src/preset_cli/lib.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.8/src/preset_cli.egg-info/PKG-INFO` & `preset-cli-0.2.9/src/preset_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: preset-cli
-Version: 0.2.8
+Version: 0.2.9
 Summary: A CLI to interact with Preset (https://preset.io/) workspaces.
 Home-page: https://github.com/preset-io/backend-sdk
 Author: Beto Dealmeida
 Author-email: beto@preset.io
 License: Other/Proprietary License
 Project-URL: Documentation, https://github.com/preset-io/backend-sdk/blob/master/README.rst
 Platform: any
@@ -31,15 +31,15 @@
 Requires-Dist: prison>=0.2.1
 Requires-Dist: prompt-toolkit>=3.0.24
 Requires-Dist: pygments>=2.11.2
 Requires-Dist: python-graphql-client>=0.4.3
 Requires-Dist: requests>=2.26.0
 Requires-Dist: rich>=12.3.0
 Requires-Dist: sqlalchemy<2,>=1.4
-Requires-Dist: sqlparse>=0.4.3
+Requires-Dist: sqlglot>=19
 Requires-Dist: tabulate>=0.8.9
 Requires-Dist: typing-extensions>=4.0.1
 Requires-Dist: yarl>=1.7.2
 Requires-Dist: greenlet>=1.1.3
 Requires-Dist: aiohttp>=3.8.3
 Provides-Extra: testing
 Requires-Dist: setuptools; extra == "testing"
```

### Comparing `preset-cli-0.2.8/src/preset_cli.egg-info/SOURCES.txt` & `preset-cli-0.2.9/src/preset_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.8/src/preset_cli.egg-info/requires.txt` & `preset-cli-0.2.9/src/preset_cli.egg-info/requires.txt`

 * *Files 20% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 prison>=0.2.1
 prompt-toolkit>=3.0.24
 pygments>=2.11.2
 python-graphql-client>=0.4.3
 requests>=2.26.0
 rich>=12.3.0
 sqlalchemy<2,>=1.4
-sqlparse>=0.4.3
+sqlglot>=19
 tabulate>=0.8.9
 typing-extensions>=4.0.1
 yarl>=1.7.2
 greenlet>=1.1.3
 aiohttp>=3.8.3
 
 [:python_version < "3.8"]
```

### Comparing `preset-cli-0.2.8/tests/api/clients/dbt_test.py` & `preset-cli-0.2.9/tests/api/clients/dbt_test.py`

 * *Files 13% similar despite different names*

```diff
@@ -33,41 +33,14 @@
         B = 1
 
     assert isinstance(PostelEnumField(StrEnum, allow_none=True), fields.String)
     assert isinstance(PostelEnumField(IntEnum, allow_none=False), fields.Integer)
     assert isinstance(PostelEnumField(RawEnum), fields.Raw)
 
 
-def test_dbt_client_execute(mocker: MockerFixture) -> None:
-    """
-    Test the ``execute`` method.
-    """
-    GraphqlClient = mocker.patch("preset_cli.api.clients.dbt.GraphqlClient")
-    auth = Auth()
-    client = DBTClient(auth)
-    query = """
-        query ($jobId: Int!) {
-            models(jobId: $jobId) {
-                uniqueId
-                name
-                database
-                schema
-                description
-                meta
-            }
-        }
-    """
-    client.execute(query, jobId=1)
-    GraphqlClient().execute.assert_called_with(
-        query=query,
-        variables={"jobId": 1},
-        headers=client.session.headers,
-    )
-
-
 def test_dbt_client_get_accounts(requests_mock: Mocker) -> None:
     """
     Test the ``get_accounts`` method.
     """
     requests_mock.get(
         "https://cloud.getdbt.com/api/v2/accounts/",
         json={
@@ -1074,48 +1047,50 @@
 def test_dbt_client_get_models(mocker: MockerFixture) -> None:
     """
     Test the ``get_models`` method.
     """
     GraphqlClient = mocker.patch("preset_cli.api.clients.dbt.GraphqlClient")
     GraphqlClient().execute.return_value = {
         "data": {
-            "models": [
-                {
-                    "uniqueId": "model.jaffle_shop.customers",
-                    "name": "customers",
-                    "database": "dbt-tutorial-347100",
-                    "schema": "dbt_beto",
-                    "description": "One record per customer",
-                    "meta": {"superset": {"cache_timeout": 600}},
-                },
-                {
-                    "uniqueId": "model.jaffle_shop.stg_customers",
-                    "name": "stg_customers",
-                    "database": "dbt-tutorial-347100",
-                    "schema": "dbt_beto",
-                    "description": "This model cleans up customer data",
-                    "meta": {},
-                },
-                {
-                    "uniqueId": "model.jaffle_shop.stg_orders",
-                    "name": "stg_orders",
-                    "database": "dbt-tutorial-347100",
-                    "schema": "dbt_beto",
-                    "description": "This model cleans up order data",
-                    "meta": {},
-                },
-                {
-                    "uniqueId": "model.metrics.dbt_metrics_default_calendar",
-                    "name": "dbt_metrics_default_calendar",
-                    "database": "dbt-tutorial-347100",
-                    "schema": "dbt_beto",
-                    "description": "",
-                    "meta": {},
-                },
-            ],
+            "job": {
+                "models": [
+                    {
+                        "uniqueId": "model.jaffle_shop.customers",
+                        "name": "customers",
+                        "database": "dbt-tutorial-347100",
+                        "schema": "dbt_beto",
+                        "description": "One record per customer",
+                        "meta": {"superset": {"cache_timeout": 600}},
+                    },
+                    {
+                        "uniqueId": "model.jaffle_shop.stg_customers",
+                        "name": "stg_customers",
+                        "database": "dbt-tutorial-347100",
+                        "schema": "dbt_beto",
+                        "description": "This model cleans up customer data",
+                        "meta": {},
+                    },
+                    {
+                        "uniqueId": "model.jaffle_shop.stg_orders",
+                        "name": "stg_orders",
+                        "database": "dbt-tutorial-347100",
+                        "schema": "dbt_beto",
+                        "description": "This model cleans up order data",
+                        "meta": {},
+                    },
+                    {
+                        "uniqueId": "model.metrics.dbt_metrics_default_calendar",
+                        "name": "dbt_metrics_default_calendar",
+                        "database": "dbt-tutorial-347100",
+                        "schema": "dbt_beto",
+                        "description": "",
+                        "meta": {},
+                    },
+                ],
+            },
         },
     }
     auth = Auth()
     client = DBTClient(auth)
     assert client.get_models(108380) == [
         {
             "schema": "dbt_beto",
@@ -1148,17 +1123,17 @@
             "meta": {},
             "database": "dbt-tutorial-347100",
             "name": "dbt_metrics_default_calendar",
         },
     ]
 
 
-def test_dbt_client_get_metrics(mocker: MockerFixture) -> None:
+def test_dbt_client_get_og_metrics(mocker: MockerFixture) -> None:
     """
-    Test the ``get_metrics`` method.
+    Test the ``get_og_metrics`` method.
     """
     GraphqlClient = mocker.patch("preset_cli.api.clients.dbt.GraphqlClient")
     GraphqlClient().execute.return_value = {
         "data": {
             "metrics": [
                 {
                     "uniqueId": "metric.jaffle_shop.new_customers",
@@ -1174,15 +1149,15 @@
                     "meta": {},
                 },
             ],
         },
     }
     auth = Auth()
     client = DBTClient(auth)
-    assert client.get_metrics(108380) == [
+    assert client.get_og_metrics(108380) == [
         {
             "meta": {},
             "name": "new_customers",
             "type": "count",
             "label": "New Customers",
             "unique_id": "metric.jaffle_shop.new_customers",
             "description": "The number of paid customers using the product",
@@ -1196,61 +1171,63 @@
 def test_dbt_client_get_database_name(mocker: MockerFixture) -> None:
     """
     Test the ``get_database_name`` method.
     """
     GraphqlClient = mocker.patch("preset_cli.api.clients.dbt.GraphqlClient")
     GraphqlClient().execute.return_value = {
         "data": {
-            "models": [
-                {
-                    "uniqueId": "model.jaffle_shop.customers",
-                    "name": "customers",
-                    "database": "dbt-tutorial-347100",
-                    "schema": "dbt_beto",
-                    "description": "One record per customer",
-                    "meta": {"superset": {"cache_timeout": 600}},
-                },
-                {
-                    "uniqueId": "model.jaffle_shop.stg_customers",
-                    "name": "stg_customers",
-                    "database": "dbt-tutorial-347100",
-                    "schema": "dbt_beto",
-                    "description": "This model cleans up customer data",
-                    "meta": {},
-                },
-                {
-                    "uniqueId": "model.jaffle_shop.stg_orders",
-                    "name": "stg_orders",
-                    "database": "dbt-tutorial-347100",
-                    "schema": "dbt_beto",
-                    "description": "This model cleans up order data",
-                    "meta": {},
-                },
-                {
-                    "uniqueId": "model.metrics.dbt_metrics_default_calendar",
-                    "name": "dbt_metrics_default_calendar",
-                    "database": "dbt-tutorial-347100",
-                    "schema": "dbt_beto",
-                    "description": "",
-                    "meta": {},
-                },
-            ],
+            "job": {
+                "models": [
+                    {
+                        "uniqueId": "model.jaffle_shop.customers",
+                        "name": "customers",
+                        "database": "dbt-tutorial-347100",
+                        "schema": "dbt_beto",
+                        "description": "One record per customer",
+                        "meta": {"superset": {"cache_timeout": 600}},
+                    },
+                    {
+                        "uniqueId": "model.jaffle_shop.stg_customers",
+                        "name": "stg_customers",
+                        "database": "dbt-tutorial-347100",
+                        "schema": "dbt_beto",
+                        "description": "This model cleans up customer data",
+                        "meta": {},
+                    },
+                    {
+                        "uniqueId": "model.jaffle_shop.stg_orders",
+                        "name": "stg_orders",
+                        "database": "dbt-tutorial-347100",
+                        "schema": "dbt_beto",
+                        "description": "This model cleans up order data",
+                        "meta": {},
+                    },
+                    {
+                        "uniqueId": "model.metrics.dbt_metrics_default_calendar",
+                        "name": "dbt_metrics_default_calendar",
+                        "database": "dbt-tutorial-347100",
+                        "schema": "dbt_beto",
+                        "description": "",
+                        "meta": {},
+                    },
+                ],
+            },
         },
     }
     auth = Auth()
     client = DBTClient(auth)
     assert client.get_database_name(108380) == "dbt-tutorial-347100"
 
 
 def test_dbt_client_get_database_name_no_models(mocker: MockerFixture) -> None:
     """
     Test the ``get_database_name`` method when there are no models.
     """
     GraphqlClient = mocker.patch("preset_cli.api.clients.dbt.GraphqlClient")
-    GraphqlClient().execute.return_value = {"data": {"models": []}}
+    GraphqlClient().execute.return_value = {"data": {"job": {"models": []}}}
     auth = Auth()
     client = DBTClient(auth)
 
     with pytest.raises(Exception) as excinfo:
         client.get_database_name(108380)
     assert str(excinfo.value) == "No models found, can't determine database name"
 
@@ -1260,33 +1237,106 @@
     Test the ``get_database_name`` method when there are multiple databases.
 
     This shouldn't happen.
     """
     GraphqlClient = mocker.patch("preset_cli.api.clients.dbt.GraphqlClient")
     GraphqlClient().execute.return_value = {
         "data": {
-            "models": [
-                {
-                    "uniqueId": "model.jaffle_shop.customers",
-                    "name": "customers",
-                    "database": "database_two",
-                    "schema": "dbt_beto",
-                    "description": "One record per customer",
-                    "meta": {"superset": {"cache_timeout": 600}},
-                },
-                {
-                    "uniqueId": "model.jaffle_shop.stg_customers",
-                    "name": "stg_customers",
-                    "database": "database_one",
-                    "schema": "dbt_beto",
-                    "description": "This model cleans up customer data",
-                    "meta": {},
-                },
-            ],
+            "job": {
+                "models": [
+                    {
+                        "uniqueId": "model.jaffle_shop.customers",
+                        "name": "customers",
+                        "database": "database_two",
+                        "schema": "dbt_beto",
+                        "description": "One record per customer",
+                        "meta": {"superset": {"cache_timeout": 600}},
+                    },
+                    {
+                        "uniqueId": "model.jaffle_shop.stg_customers",
+                        "name": "stg_customers",
+                        "database": "database_one",
+                        "schema": "dbt_beto",
+                        "description": "This model cleans up customer data",
+                        "meta": {},
+                    },
+                ],
+            },
         },
     }
     auth = Auth()
     client = DBTClient(auth)
 
     with pytest.raises(Exception) as excinfo:
         client.get_database_name(108380)
     assert str(excinfo.value) == "Multiple databases found"
+
+
+def test_dbt_client_get_sl_metrics(mocker: MockerFixture) -> None:
+    """
+    Test the ``get_sl_metrics`` method.
+    """
+    GraphqlClient = mocker.patch("preset_cli.api.clients.dbt.GraphqlClient")
+    GraphqlClient().execute.return_value = {
+        "data": {
+            "metrics": [
+                {"name": "a", "description": "A", "type": "SIMPLE"},
+            ],
+        },
+    }
+    auth = Auth()
+    client = DBTClient(auth)
+
+    assert client.get_sl_metrics(108380) == [
+        {"name": "a", "description": "A", "type": "SIMPLE"},
+    ]
+
+
+def test_dbt_client_get_sl_metric_sql(mocker: MockerFixture) -> None:
+    """
+    Test the ``get_sl_metric_sql`` method.
+    """
+    GraphqlClient = mocker.patch("preset_cli.api.clients.dbt.GraphqlClient")
+    GraphqlClient().execute.return_value = {
+        "data": {"compileSql": {"sql": "SELECT 1 FROM a"}},
+    }
+    auth = Auth()
+    client = DBTClient(auth)
+
+    assert client.get_sl_metric_sql("metric", 108380) == "SELECT 1 FROM a"
+
+
+def test_dbt_client_get_sl_metric_sql_error(mocker: MockerFixture) -> None:
+    """
+    Test the ``get_sl_metric_sql`` method when there's an error.
+    """
+    _logger = mocker.patch("preset_cli.api.clients.dbt._logger")
+    GraphqlClient = mocker.patch("preset_cli.api.clients.dbt.GraphqlClient")
+    GraphqlClient().execute.return_value = {
+        "data": None,
+        "errors": [
+            {"message": "Something went wrong"},
+        ],
+    }
+    auth = Auth()
+    client = DBTClient(auth)
+
+    assert client.get_sl_metric_sql("metric", 108380) is None
+    _logger.warning.assert_called_with(
+        "Unable to convert metric %s: %s",
+        "metric",
+        "Something went wrong",
+    )
+
+
+def test_dbt_client_get_sl_dialect(mocker: MockerFixture) -> None:
+    """
+    Test the ``get_sl_dialect`` method.
+    """
+    GraphqlClient = mocker.patch("preset_cli.api.clients.dbt.GraphqlClient")
+    GraphqlClient().execute.return_value = {
+        "data": {"environmentInfo": {"dialect": "BIGQUERY"}},
+    }
+    auth = Auth()
+    client = DBTClient(auth)
+
+    assert client.get_sl_dialect(108380) == "BIGQUERY"
```

### Comparing `preset-cli-0.2.8/tests/api/clients/preset_test.py` & `preset-cli-0.2.9/tests/api/clients/preset_test.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.8/tests/api/clients/superset_test.py` & `preset-cli-0.2.9/tests/api/clients/superset_test.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.8/tests/auth/jwt_test.py` & `preset-cli-0.2.9/tests/auth/jwt_test.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.8/tests/auth/lib_test.py` & `preset-cli-0.2.9/tests/auth/lib_test.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.8/tests/auth/main_test.py` & `preset-cli-0.2.9/tests/auth/main_test.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.8/tests/auth/preset_test.py` & `preset-cli-0.2.9/tests/auth/preset_test.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.8/tests/auth/superset_test.py` & `preset-cli-0.2.9/tests/auth/superset_test.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.8/tests/cli/main_test.py` & `preset-cli-0.2.9/tests/cli/main_test.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.8/tests/cli/superset/export_test.py` & `preset-cli-0.2.9/tests/cli/superset/export_test.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.8/tests/cli/superset/import_test.py` & `preset-cli-0.2.9/tests/cli/superset/import_test.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.8/tests/cli/superset/main_test.py` & `preset-cli-0.2.9/tests/cli/superset/main_test.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.8/tests/cli/superset/sql_test.py` & `preset-cli-0.2.9/tests/cli/superset/sql_test.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.8/tests/cli/superset/sync/dbt/command_test.py` & `preset-cli-0.2.9/tests/cli/superset/sync/dbt/command_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,18 +9,19 @@
 
 import pytest
 import yaml
 from click.testing import CliRunner
 from pyfakefs.fake_filesystem import FakeFilesystem
 from pytest_mock import MockerFixture
 
+from preset_cli.api.clients.dbt import MFSQLEngine
 from preset_cli.cli.superset.main import superset_cli
 from preset_cli.cli.superset.sync.dbt.command import (
     get_account_id,
-    get_job_id,
+    get_job,
     get_project_id,
 )
 from preset_cli.exceptions import DatabaseNotFoundError
 
 dirname, _ = os.path.split(os.path.abspath(__file__))
 with open(os.path.join(dirname, "manifest.json"), encoding="utf-8") as fp:
     manifest_contents = fp.read()
@@ -122,14 +123,27 @@
         "time_grains": [],
         "tags": [],
         "refs": [["messages_channels"]],
         "dimensions": [],
     },
 ]
 
+superset_metrics = {
+    "model.superset_examples.messages_channels": [
+        {
+            "description": "",
+            "expression": "COUNT(*)",
+            "extra": "{}",
+            "metric_name": "cnt",
+            "metric_type": "count",
+            "verbose_name": "",
+        },
+    ],
+}
+
 dbt_cloud_models = [
     {
         "database": "examples_dev",
         "description": "",
         "meta": {},
         "name": "messages_channels",
         "schema": "public",
@@ -145,14 +159,31 @@
         "label": "",
         "meta": {},
         "name": "cnt",
         "sql": "*",
         "type": "count",
         "unique_id": "metric.superset_examples.cnt",
     },
+    {
+        "depends_on": ["a", "b"],
+        "description": "",
+        "filters": [],
+        "label": "",
+        "meta": {},
+        "name": "multiple parents",
+        "sql": "*",
+        "type": "count",
+        "unique_id": "c",
+    },
+]
+
+dbt_metricflow_metrics = [
+    {"name": "a", "type": "Simple", "description": "The simplest metric"},
+    {"name": "b", "type": "derived", "description": "Too complex for Superset"},
+    {"name": "c", "type": "derived", "description": "Multiple models"},
 ]
 
 
 def test_dbt_core(mocker: MockerFixture, fs: FakeFilesystem) -> None:
     """
     Test the ``dbt-core`` command.
     """
@@ -206,26 +237,26 @@
         False,
         "",
     )
 
     sync_datasets.assert_called_with(
         client,
         dbt_core_models,
-        dbt_core_metrics,
+        superset_metrics,
         sync_database(),
         False,
         "",
         reload_columns=True,
         merge_metadata=False,
     )
     sync_exposures.assert_called_with(
         client,
         exposures,
         sync_datasets(),
-        {("public", "messages_channels"): "ref('messages_channels')"},
+        {("public", "messages_channels"): dbt_core_models[0]},
     )
 
 
 def test_dbt_core_preserve_metadata(
     mocker: MockerFixture,
     fs: FakeFilesystem,
 ) -> None:
@@ -283,26 +314,26 @@
         False,
         "",
     )
 
     sync_datasets.assert_called_with(
         client,
         dbt_core_models,
-        dbt_core_metrics,
+        superset_metrics,
         sync_database(),
         False,
         "",
         reload_columns=False,
         merge_metadata=False,
     )
     sync_exposures.assert_called_with(
         client,
         exposures,
         sync_datasets(),
-        {("public", "messages_channels"): "ref('messages_channels')"},
+        {("public", "messages_channels"): dbt_core_models[0]},
     )
 
 
 def test_dbt_core_preserve_columns(
     mocker: MockerFixture,
     fs: FakeFilesystem,
 ) -> None:
@@ -353,15 +384,15 @@
         False,
         "",
     )
 
     sync_datasets.assert_called_with(
         client,
         dbt_core_models,
-        dbt_core_metrics,
+        superset_metrics,
         sync_database(),
         False,
         "",
         reload_columns=False,
         merge_metadata=False,
     )
 
@@ -424,26 +455,26 @@
         False,
         "",
     )
 
     sync_datasets.assert_called_with(
         client,
         dbt_core_models,
-        dbt_core_metrics,
+        superset_metrics,
         sync_database(),
         False,
         "",
         reload_columns=False,
         merge_metadata=True,
     )
     sync_exposures.assert_called_with(
         client,
         exposures,
         sync_datasets(),
-        {("public", "messages_channels"): "ref('messages_channels')"},
+        {("public", "messages_channels"): dbt_core_models[0]},
     )
 
 
 def test_dbt_core_preserve_and_merge(
     mocker: MockerFixture,
     fs: FakeFilesystem,
 ) -> None:
@@ -696,56 +727,29 @@
             "root_path": "/Users/beto/Projects/dbt-examples/superset_examples",
             "extra_ctes_injected": True,
             "package_name": "superset_examples",
             "unrendered_config": {"materialized": "view"},
             "refs": [],
         },
     ]
-    metrics = [
-        {
-            "meta": {},
-            "depends_on": ["model.superset_examples.messages_channels"],
-            "unique_id": "metric.superset_examples.cnt",
-            "label": "",
-            "sql": "*",
-            "type": "count",
-            "name": "cnt",
-            "description": "",
-            "filters": [],
-            "model": "ref('messages_channels')",
-            "sources": [],
-            "original_file_path": "models/slack/schema.yml",
-            "resource_type": "metric",
-            "tags": [],
-            "path": "slack/schema.yml",
-            "created_at": 1642630986.1942852,
-            "fqn": ["superset_examples", "slack", "cnt"],
-            "package_name": "superset_examples",
-            "timestamp": None,
-            "root_path": "/Users/beto/Projects/dbt-examples/superset_examples",
-            "time_grains": [],
-            "refs": [["messages_channels"]],
-            "dimensions": [],
-        },
-    ]
     sync_datasets.assert_called_with(
         client,
         models,
-        metrics,
+        superset_metrics,
         sync_database(),
         False,
         "",
         reload_columns=True,
         merge_metadata=False,
     )
     sync_exposures.assert_called_with(
         client,
         exposures,
         sync_datasets(),
-        {("public", "messages_channels"): "ref('messages_channels')"},
+        {("public", "messages_channels"): dbt_core_models[0]},
     )
 
 
 def test_dbt_core_no_exposures(mocker: MockerFixture, fs: FakeFilesystem) -> None:
     """
     Test the ``dbt-core`` command when no exposures file is passed.
     """
@@ -866,15 +870,15 @@
             str(profiles),
             "--exposures",
             str(exposures),
         ],
         catch_exceptions=False,
     )
     assert result.exit_code == 0
-    assert result.output == "No database was found, pass ``--import-db`` to create\n"
+    assert "No database was found, pass ``--import-db`` to create" in result.output
 
 
 def test_dbt_core_disallow_edits_superset(
     mocker: MockerFixture,
     fs: FakeFilesystem,
 ) -> None:
     """
@@ -956,17 +960,28 @@
     DBTClient = mocker.patch(
         "preset_cli.cli.superset.sync.dbt.command.DBTClient",
     )
     dbt_client = DBTClient()
     sync_datasets = mocker.patch(
         "preset_cli.cli.superset.sync.dbt.command.sync_datasets",
     )
+    mocker.patch(
+        "preset_cli.cli.superset.sync.dbt.command.get_job",
+        return_value={"id": 123, "name": "My job", "environment_id": 456},
+    )
 
     dbt_client.get_models.return_value = dbt_cloud_models
-    dbt_client.get_metrics.return_value = dbt_cloud_metrics
+    dbt_client.get_og_metrics.return_value = dbt_cloud_metrics
+    dbt_client.get_sl_dialect.return_value = MFSQLEngine.BIGQUERY
+    dbt_client.get_sl_metrics.return_value = dbt_metricflow_metrics
+    dbt_client.get_sl_metric_sql.side_effect = [
+        "SELECT COUNT(*) FROM public.messages_channels",
+        "SELECT COUNT(*) FROM public.messages_channels JOIN some_other_table",
+        None,
+    ]
     database = mocker.MagicMock()
     superset_client.get_databases.return_value = [database]
     superset_client.get_database.return_value = database
 
     runner = CliRunner()
     result = runner.invoke(
         superset_cli,
@@ -979,15 +994,33 @@
         ],
         catch_exceptions=False,
     )
     assert result.exit_code == 0
     sync_datasets.assert_called_with(
         superset_client,
         dbt_cloud_models,
-        dbt_cloud_metrics,
+        {
+            "model.superset_examples.messages_channels": [
+                {
+                    "description": "",
+                    "expression": "COUNT(*)",
+                    "extra": "{}",
+                    "metric_name": "cnt",
+                    "metric_type": "count",
+                    "verbose_name": "",
+                },
+                {
+                    "description": "The simplest metric",
+                    "expression": "COUNT(*)",
+                    "metric_name": "a",
+                    "metric_type": "Simple",
+                    "verbose_name": "a",
+                },
+            ],
+        },
         database,
         False,
         "",
         reload_columns=True,
         merge_metadata=False,
     )
 
@@ -1004,17 +1037,21 @@
     DBTClient = mocker.patch(
         "preset_cli.cli.superset.sync.dbt.command.DBTClient",
     )
     dbt_client = DBTClient()
     sync_datasets = mocker.patch(
         "preset_cli.cli.superset.sync.dbt.command.sync_datasets",
     )
+    mocker.patch(
+        "preset_cli.cli.superset.sync.dbt.command.get_job",
+        return_value={"id": 123, "name": "My job", "environment_id": 456},
+    )
 
     dbt_client.get_models.return_value = dbt_cloud_models
-    dbt_client.get_metrics.return_value = dbt_cloud_metrics
+    dbt_client.get_og_metrics.return_value = dbt_cloud_metrics
     database = mocker.MagicMock()
     superset_client.get_databases.return_value = [database]
     superset_client.get_database.return_value = database
 
     runner = CliRunner()
     result = runner.invoke(
         superset_cli,
@@ -1028,15 +1065,15 @@
         ],
         catch_exceptions=False,
     )
     assert result.exit_code == 0
     sync_datasets.assert_called_with(
         superset_client,
         dbt_cloud_models,
-        dbt_cloud_metrics,
+        superset_metrics,
         database,
         False,
         "",
         reload_columns=False,
         merge_metadata=False,
     )
 
@@ -1053,17 +1090,21 @@
     DBTClient = mocker.patch(
         "preset_cli.cli.superset.sync.dbt.command.DBTClient",
     )
     dbt_client = DBTClient()
     sync_datasets = mocker.patch(
         "preset_cli.cli.superset.sync.dbt.command.sync_datasets",
     )
+    mocker.patch(
+        "preset_cli.cli.superset.sync.dbt.command.get_job",
+        return_value={"id": 123, "name": "My job", "environment_id": 456},
+    )
 
     dbt_client.get_models.return_value = dbt_cloud_models
-    dbt_client.get_metrics.return_value = dbt_cloud_metrics
+    dbt_client.get_og_metrics.return_value = dbt_cloud_metrics
     database = mocker.MagicMock()
     superset_client.get_databases.return_value = [database]
     superset_client.get_database.return_value = database
 
     runner = CliRunner()
     result = runner.invoke(
         superset_cli,
@@ -1077,15 +1118,15 @@
         ],
         catch_exceptions=False,
     )
     assert result.exit_code == 0
     sync_datasets.assert_called_with(
         superset_client,
         dbt_cloud_models,
-        dbt_cloud_metrics,
+        superset_metrics,
         database,
         False,
         "",
         reload_columns=False,
         merge_metadata=False,
     )
 
@@ -1102,17 +1143,21 @@
     DBTClient = mocker.patch(
         "preset_cli.cli.superset.sync.dbt.command.DBTClient",
     )
     dbt_client = DBTClient()
     sync_datasets = mocker.patch(
         "preset_cli.cli.superset.sync.dbt.command.sync_datasets",
     )
+    mocker.patch(
+        "preset_cli.cli.superset.sync.dbt.command.get_job",
+        return_value={"id": 123, "name": "My job", "environment_id": 456},
+    )
 
     dbt_client.get_models.return_value = dbt_cloud_models
-    dbt_client.get_metrics.return_value = dbt_cloud_metrics
+    dbt_client.get_og_metrics.return_value = dbt_cloud_metrics
     database = mocker.MagicMock()
     superset_client.get_databases.return_value = [database]
     superset_client.get_database.return_value = database
 
     runner = CliRunner()
     result = runner.invoke(
         superset_cli,
@@ -1126,15 +1171,15 @@
         ],
         catch_exceptions=False,
     )
     assert result.exit_code == 0
     sync_datasets.assert_called_with(
         superset_client,
         dbt_cloud_models,
-        dbt_cloud_metrics,
+        superset_metrics,
         database,
         False,
         "",
         reload_columns=False,
         merge_metadata=True,
     )
 
@@ -1177,18 +1222,20 @@
     )
     dbt_client = DBTClient()
     sync_datasets = mocker.patch(
         "preset_cli.cli.superset.sync.dbt.command.sync_datasets",
     )
 
     dbt_client.get_models.return_value = dbt_cloud_models
-    dbt_client.get_metrics.return_value = dbt_cloud_metrics
+    dbt_client.get_og_metrics.return_value = dbt_cloud_metrics
     dbt_client.get_accounts.return_value = [{"id": 1, "name": "My account"}]
     dbt_client.get_projects.return_value = [{"id": 1000, "name": "My project"}]
-    dbt_client.get_jobs.return_value = [{"id": 123, "name": "My job"}]
+    dbt_client.get_jobs.return_value = [
+        {"id": 123, "name": "My job", "environment_id": 456},
+    ]
     database = mocker.MagicMock()
     superset_client.get_databases.return_value = [database]
     superset_client.get_database.return_value = database
 
     runner = CliRunner()
     result = runner.invoke(
         superset_cli,
@@ -1199,19 +1246,19 @@
             "XXX",
         ],
         catch_exceptions=False,
     )
     assert result.exit_code == 0
     dbt_client.get_database_name.assert_called_with(123)
     dbt_client.get_models.assert_called_with(123)
-    dbt_client.get_metrics.assert_called_with(123)
+    dbt_client.get_og_metrics.assert_called_with(123)
     sync_datasets.assert_called_with(
         superset_client,
         dbt_cloud_models,
-        dbt_cloud_metrics,
+        superset_metrics,
         database,
         False,
         "",
         reload_columns=True,
         merge_metadata=False,
     )
 
@@ -1278,49 +1325,70 @@
     client.get_projects.return_value = [
         {"id": 1, "name": "My project"},
     ]
     assert get_project_id(client) == 1
     client.get_projects.assert_called_with(42)
 
 
-def test_get_job_id(mocker: MockerFixture) -> None:
+def test_get_job(mocker: MockerFixture) -> None:
     """
-    Test the ``get_job_id`` helper.
+    Test the ``get_job`` helper.
     """
     client = mocker.MagicMock()
 
     client.get_jobs.return_value = []
     with pytest.raises(SystemExit) as excinfo:
-        get_job_id(client, account_id=42, project_id=43)
+        get_job(client, account_id=42, project_id=43)
     assert excinfo.type == SystemExit
     assert excinfo.value.code == 1
 
     client.get_jobs.return_value = [
-        {"id": 1, "name": "My job"},
+        {"id": 1, "name": "My job", "environment_id": 456},
     ]
-    assert get_job_id(client, account_id=42, project_id=43) == 1
+    assert get_job(client, account_id=42, project_id=43) == {
+        "id": 1,
+        "name": "My job",
+        "environment_id": 456,
+    }
 
     client.get_jobs.return_value = [
-        {"id": 1, "name": "My job"},
-        {"id": 3, "name": "My other job"},
+        {"id": 1, "name": "My job", "environment_id": 456},
+        {"id": 3, "name": "My other job", "environment_id": 456},
     ]
+    assert get_job(client, account_id=42, project_id=43, job_id=3) == {
+        "id": 3,
+        "name": "My other job",
+        "environment_id": 456,
+    }
+    with pytest.raises(ValueError) as excinfo:
+        get_job(client, account_id=42, project_id=43, job_id=2)
+    assert str(excinfo.value) == "Job 2 not available"
+
     mocker.patch(
         "preset_cli.cli.superset.sync.dbt.command.input",
         side_effect=["invalid", "2"],
     )
-    assert get_job_id(client, account_id=42, project_id=43) == 3
+    assert get_job(client, account_id=42, project_id=43) == {
+        "id": 3,
+        "name": "My other job",
+        "environment_id": 456,
+    }
 
     mocker.patch(
         "preset_cli.cli.superset.sync.dbt.command.get_account_id",
         return_value=42,
     )
     client.get_jobs.return_value = [
-        {"id": 1, "name": "My job"},
+        {"id": 1, "name": "My job", "environment_id": 456},
     ]
-    assert get_job_id(client, project_id=43) == 1
+    assert get_job(client, project_id=43) == {
+        "id": 1,
+        "name": "My job",
+        "environment_id": 456,
+    }
     client.get_jobs.assert_called_with(42, 43)
 
 
 def test_dbt_cloud_no_database(mocker: MockerFixture) -> None:
     """
     Test the ``dbt-cloud`` command when no database is found.
     """
@@ -1331,14 +1399,18 @@
     mocker.patch("preset_cli.cli.superset.main.UsernamePasswordAuth")
     DBTClient = mocker.patch(
         "preset_cli.cli.superset.sync.dbt.command.DBTClient",
     )
     dbt_client = DBTClient()
     dbt_client.get_database_name.return_value = "my_db"
     superset_client.get_databases.return_value = []
+    mocker.patch(
+        "preset_cli.cli.superset.sync.dbt.command.get_job",
+        return_value={"id": 123, "name": "My job", "environment_id": 456},
+    )
 
     runner = CliRunner()
     result = runner.invoke(
         superset_cli,
         [
             "https://superset.example.org/",
             "sync",
@@ -1348,14 +1420,50 @@
         ],
         catch_exceptions=False,
     )
     assert result.exit_code == 0
     assert result.output == 'No database named "my_db" was found\n'
 
 
+def test_dbt_cloud_invalid_job_id(mocker: MockerFixture) -> None:
+    """
+    Test the ``dbt-cloud`` command when an invalid job ID is passed.
+    """
+    SupersetClient = mocker.patch(
+        "preset_cli.cli.superset.sync.dbt.command.SupersetClient",
+    )
+    superset_client = SupersetClient()
+    mocker.patch("preset_cli.cli.superset.main.UsernamePasswordAuth")
+    DBTClient = mocker.patch(
+        "preset_cli.cli.superset.sync.dbt.command.DBTClient",
+    )
+    dbt_client = DBTClient()
+    dbt_client.get_database_name.return_value = "my_db"
+    superset_client.get_databases.return_value = []
+    mocker.patch(
+        "preset_cli.cli.superset.sync.dbt.command.get_job",
+        side_effect=ValueError("Job 123 not available"),
+    )
+
+    runner = CliRunner()
+    result = runner.invoke(
+        superset_cli,
+        [
+            "https://superset.example.org/",
+            "sync",
+            "dbt-cloud",
+            "XXX",
+            "123",
+        ],
+        catch_exceptions=False,
+    )
+    assert result.exit_code == 2
+    assert result.output == "Job 123 not available\n"
+
+
 def test_dbt_cloud_multiple_databases(mocker: MockerFixture) -> None:
     """
     Test the ``dbt-cloud`` command when multiple databases are found.
 
     This should never happen, since Supersret has a uniqueness contraint on the table
     name. Nevertheless, test this for completeness.
     """
@@ -1369,14 +1477,18 @@
     )
     dbt_client = DBTClient()
     dbt_client.get_database_name.return_value = "my_db"
     superset_client.get_databases.return_value = [
         mocker.MagicMock(),
         mocker.MagicMock(),
     ]
+    mocker.patch(
+        "preset_cli.cli.superset.sync.dbt.command.get_job",
+        return_value={"id": 123, "name": "My job", "environment_id": 456},
+    )
 
     runner = CliRunner()
     with pytest.raises(Exception) as excinfo:
         runner.invoke(
             superset_cli,
             [
                 "https://superset.example.org/",
@@ -1443,15 +1555,15 @@
     sync_datasets.assert_not_called()
     sync_exposures.assert_called_with(
         client,
         exposures,
         [
             {"schema": "public", "table_name": "messages_channels"},
         ],
-        {("public", "messages_channels"): "ref('messages_channels')"},
+        {("public", "messages_channels"): dbt_core_models[0]},
     )
 
 
 def test_dbt_cloud_exposures_only(mocker: MockerFixture, fs: FakeFilesystem) -> None:
     """
     Test the ``--exposures-only`` option with dbt cloud.
     """
@@ -1475,17 +1587,21 @@
     dbt_client = DBTClient()
     sync_datasets = mocker.patch(
         "preset_cli.cli.superset.sync.dbt.command.sync_datasets",
     )
     sync_exposures = mocker.patch(
         "preset_cli.cli.superset.sync.dbt.command.sync_exposures",
     )
+    mocker.patch(
+        "preset_cli.cli.superset.sync.dbt.command.get_job",
+        return_value={"id": 123, "name": "My job", "environment_id": 456},
+    )
 
     dbt_client.get_models.return_value = dbt_cloud_models
-    dbt_client.get_metrics.return_value = dbt_cloud_metrics
+    dbt_client.get_og_metrics.return_value = dbt_cloud_metrics
     database = mocker.MagicMock()
     superset_client.get_databases.return_value = [database]
     superset_client.get_database.return_value = database
 
     runner = CliRunner()
     result = runner.invoke(
         superset_cli,
@@ -1505,9 +1621,9 @@
     sync_datasets.assert_not_called()
     sync_exposures.assert_called_with(
         superset_client,
         exposures,
         [
             {"schema": "public", "table_name": "messages_channels"},
         ],
-        {("public", "messages_channels"): "ref('messages_channels')"},
+        {("public", "messages_channels"): dbt_cloud_models[0]},
     )
```

### Comparing `preset-cli-0.2.8/tests/cli/superset/sync/dbt/databases_test.py` & `preset-cli-0.2.9/tests/cli/superset/sync/dbt/databases_test.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.8/tests/cli/superset/sync/dbt/datasets_test.py` & `preset-cli-0.2.9/tests/cli/superset/sync/dbt/datasets_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,44 +1,43 @@
 """
 Tests for ``preset_cli.cli.superset.sync.dbt.datasets``.
 """
 # pylint: disable=invalid-name, too-many-lines
 
 import copy
 import json
-from typing import List, cast
+from typing import Dict, List, cast
 from unittest import mock
 
 import pytest
 from pytest_mock import MockerFixture
 from sqlalchemy.engine.url import make_url
 
 from preset_cli.api.clients.dbt import MetricSchema, ModelSchema
+from preset_cli.api.clients.superset import SupersetMetricDefinition
 from preset_cli.cli.superset.sync.dbt.datasets import (
     create_dataset,
     model_in_database,
     sync_datasets,
 )
 
 metric_schema = MetricSchema()
-metrics: List[MetricSchema] = [
-    metric_schema.load(
+
+metrics: Dict[str, List[SupersetMetricDefinition]] = {
+    "model.superset_examples.messages_channels": [
         {
-            "depends_on": ["model.superset_examples.messages_channels"],
             "description": "",
-            "filters": [],
-            "meta": {},
-            "name": "cnt",
-            "label": "",
-            "sql": "*",
-            "type": "count",
-            "unique_id": "metric.superset_examples.cnt",
+            "expression": "COUNT(*)",
+            "extra": "{}",
+            "metric_name": "cnt",
+            "metric_type": "count",
+            "verbose_name": "",
         },
-    ),
-]
+    ],
+}
 
 model_schema = ModelSchema()
 models: List[ModelSchema] = [
     model_schema.load(
         {
             "database": "examples_dev",
             "schema": "public",
@@ -230,15 +229,15 @@
     client.get_dataset.return_value = {
         "columns": [{"column_name": "id", "is_dttm": False}],
     }
 
     sync_datasets(
         client=client,
         models=models,
-        metrics=[],
+        metrics={},
         database={"id": 1, "sqlalchemy_uri": "postgresql://user@host/examples_dev"},
         disallow_edits=False,
         external_url_prefix="",
     )
     client.create_dataset.assert_has_calls(
         [
             mock.call(database=1, schema="public", table_name="messages_channels"),
@@ -286,15 +285,15 @@
     client.get_dataset.return_value = {
         "columns": [{"column_name": "id", "is_dttm": False}],
     }
 
     sync_datasets(
         client=client,
         models=models,
-        metrics=[],
+        metrics={},
         database={"id": 1, "sqlalchemy_uri": "postgresql://user@host/examples_dev"},
         disallow_edits=False,
         external_url_prefix="",
         certification={"details": "This dataset is synced from dbt Cloud"},
     )
     client.create_dataset.assert_has_calls(
         [
@@ -519,26 +518,23 @@
 def test_sync_datasets_preserve_metadata(mocker: MockerFixture) -> None:
     """
     Test ``sync_datasets`` with preserve_metadata set to True.
     Metrics should be merged (Preset as the source of truth).
     """
     client = mocker.MagicMock()
     metrics_ = copy.deepcopy(metrics)
-    metrics_.append(
+    metrics_["model.superset_examples.messages_channels"].append(
         metric_schema.load(
             {
-                "depends_on": ["model.superset_examples.messages_channels"],
                 "description": "",
-                "filters": [],
-                "meta": {},
-                "name": "max_id",
-                "label": "",
-                "sql": "id",
-                "type": "max",
-                "unique_id": "metric.superset_examples.cnt",
+                "expression": "MAX(id)",
+                "extra": "{}",
+                "metric_name": "max_id",
+                "metric_type": "max",
+                "verbose_name": "",
             },
         ),
     )
     client.get_datasets.side_effect = [[{"id": 1}], [{"id": 2}], [{"id": 3}]]
     client.get_dataset.return_value = {
         "columns": [
             {
@@ -637,26 +633,23 @@
 def test_sync_datasets_merge_metadata(mocker: MockerFixture) -> None:
     """
     Test ``sync_datasets`` with merge_metadata set to True.
     Metrics should be merged (dbt as the source of truth).
     """
     client = mocker.MagicMock()
     metrics_ = copy.deepcopy(metrics)
-    metrics_.append(
+    metrics_["model.superset_examples.messages_channels"].append(
         metric_schema.load(
             {
-                "depends_on": ["model.superset_examples.messages_channels"],
                 "description": "",
-                "filters": [],
-                "meta": {},
-                "name": "max_id",
-                "label": "",
-                "sql": "id",
-                "type": "max",
-                "unique_id": "metric.superset_examples.cnt",
+                "expression": "MAX(id)",
+                "extra": "{}",
+                "metric_name": "max_id",
+                "metric_type": "max",
+                "verbose_name": "",
             },
         ),
     )
     client.get_datasets.side_effect = [[{"id": 1}], [{"id": 2}], [{"id": 3}]]
     client.get_dataset.return_value = {
         "columns": [
             {
```

### Comparing `preset-cli-0.2.8/tests/cli/superset/sync/dbt/exposures_test.py` & `preset-cli-0.2.9/tests/cli/superset/sync/dbt/exposures_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -754,15 +754,15 @@
     modified_dataset_response["result"]["extra"] = None  # type: ignore
     client.get_dataset.return_value = modified_dataset_response["result"]
 
     key = ModelKey("public", "messages_channels")
     depends_on = get_chart_depends_on(
         client,
         chart_response["result"],
-        {key: "ref('messages_channels')"},
+        {key: {"name": "messages_channels"}},  # type: ignore
     )
     assert depends_on == ["ref('messages_channels')"]
 
 
 def test_get_chart_depends_on_exception(
     mocker: MockerFixture,
 ) -> None:
@@ -794,10 +794,10 @@
     session = client.auth.session
     session.get().json.return_value = datasets_response
 
     key = ModelKey("public", "messages_channels")
     depends_on = get_dashboard_depends_on(
         client,
         dashboard_response["result"],
-        {key: "ref('messages_channels')"},
+        {key: {"name": "messages_channels"}},  # type: ignore
     )
     assert depends_on == ["ref('messages_channels')"]
```

### Comparing `preset-cli-0.2.8/tests/cli/superset/sync/dbt/lib_test.py` & `preset-cli-0.2.9/tests/cli/superset/sync/dbt/lib_test.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.8/tests/cli/superset/sync/dbt/manifest.json` & `preset-cli-0.2.9/tests/cli/superset/sync/dbt/manifest.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9375%*

 * *Differences: {"'metrics'": "{'c': OrderedDict([('depends_on', OrderedDict([('nodes', ['a', 'b'])])), "*

 * *              "('description', ''), ('filters', []), ('label', ''), ('meta', OrderedDict()), "*

 * *              "('name', 'multiple parents'), ('sql', '*'), ('type', 'count'), ('unique_id', "*

 * *              "'c')])}"}*

```diff
@@ -8,14 +8,30 @@
             "model.superset_examples.messages_channels"
         ],
         "source.superset_examples.public.messages": [
             "model.superset_examples.messages_channels"
         ]
     },
     "metrics": {
+        "c": {
+            "depends_on": {
+                "nodes": [
+                    "a",
+                    "b"
+                ]
+            },
+            "description": "",
+            "filters": [],
+            "label": "",
+            "meta": {},
+            "name": "multiple parents",
+            "sql": "*",
+            "type": "count",
+            "unique_id": "c"
+        },
         "metric.superset_examples.cnt": {
             "created_at": 1642630986.1942852,
             "depends_on": {
                 "macros": [],
                 "nodes": [
                     "model.superset_examples.messages_channels"
                 ]
```

### Comparing `preset-cli-0.2.8/tests/cli/superset/sync/native/command_test.py` & `preset-cli-0.2.9/tests/cli/superset/sync/native/command_test.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.8/tests/lib_test.py` & `preset-cli-0.2.9/tests/lib_test.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.8/tox.ini` & `preset-cli-0.2.9/tox.ini`

 * *Files identical despite different names*

