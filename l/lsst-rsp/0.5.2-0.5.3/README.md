# Comparing `tmp/lsst_rsp-0.5.2.tar.gz` & `tmp/lsst_rsp-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lsst_rsp-0.5.2.tar", last modified: Mon Apr 22 23:47:58 2024, max compression
+gzip compressed data, was "lsst_rsp-0.5.3.tar", last modified: Thu May  9 23:19:22 2024, max compression
```

## Comparing `lsst_rsp-0.5.2.tar` & `lsst_rsp-0.5.3.tar`

### file list

```diff
@@ -1,78 +1,86 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:47:58.076074 lsst_rsp-0.5.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:47:58.068073 lsst_rsp-0.5.2/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-22 23:47:53.000000 lsst_rsp-0.5.2/.github/CODE_OF_CONDUCT
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-04-22 23:47:53.000000 lsst_rsp-0.5.2/.github/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-22 23:47:53.000000 lsst_rsp-0.5.2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:47:58.068073 lsst_rsp-0.5.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-04-22 23:47:53.000000 lsst_rsp-0.5.2/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-04-22 23:47:53.000000 lsst_rsp-0.5.2/.github/workflows/periodic-ci.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-04-22 23:47:53.000000 lsst_rsp-0.5.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-22 23:47:53.000000 lsst_rsp-0.5.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-22 23:47:53.000000 lsst_rsp-0.5.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-22 23:47:53.000000 lsst_rsp-0.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 23:47:53.000000 lsst_rsp-0.5.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-22 23:47:53.000000 lsst_rsp-0.5.2/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     5444 2024-04-22 23:47:58.076074 lsst_rsp-0.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-04-22 23:47:53.000000 lsst_rsp-0.5.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:47:58.068073 lsst_rsp-0.5.2/changelog.d/
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-22 23:47:53.000000 lsst_rsp-0.5.2/changelog.d/_template.md.jinja
--rw-r--r--   0 runner    (1001) docker     (127)     8309 2024-04-22 23:47:53.000000 lsst_rsp-0.5.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 23:47:58.076074 lsst_rsp-0.5.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:47:58.064073 lsst_rsp-0.5.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:47:58.068073 lsst_rsp-0.5.2/src/lsst/
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-22 23:47:53.000000 lsst_rsp-0.5.2/src/lsst/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:47:58.072073 lsst_rsp-0.5.2/src/lsst/rsp/
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-04-22 23:47:53.000000 lsst_rsp-0.5.2/src/lsst/rsp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2438 2024-04-22 23:47:53.000000 lsst_rsp-0.5.2/src/lsst/rsp/catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-04-22 23:47:53.000000 lsst_rsp-0.5.2/src/lsst/rsp/log.py
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-22 23:47:53.000000 lsst_rsp-0.5.2/src/lsst/rsp/service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:47:58.072073 lsst_rsp-0.5.2/src/lsst/rsp/startup/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 23:47:53.000000 lsst_rsp-0.5.2/src/lsst/rsp/startup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-22 23:47:53.000000 lsst_rsp-0.5.2/src/lsst/rsp/startup/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-04-22 23:47:53.000000 lsst_rsp-0.5.2/src/lsst/rsp/startup/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-04-22 23:47:53.000000 lsst_rsp-0.5.2/src/lsst/rsp/startup/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:47:58.072073 lsst_rsp-0.5.2/src/lsst/rsp/startup/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 23:47:53.000000 lsst_rsp-0.5.2/src/lsst/rsp/startup/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-04-22 23:47:53.000000 lsst_rsp-0.5.2/src/lsst/rsp/startup/models/noninteractive.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:47:58.072073 lsst_rsp-0.5.2/src/lsst/rsp/startup/services/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 23:47:53.000000 lsst_rsp-0.5.2/src/lsst/rsp/startup/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27930 2024-04-22 23:47:53.000000 lsst_rsp-0.5.2/src/lsst/rsp/startup/services/labrunner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:47:58.072073 lsst_rsp-0.5.2/src/lsst/rsp/startup/storage/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 23:47:53.000000 lsst_rsp-0.5.2/src/lsst/rsp/startup/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4717 2024-04-22 23:47:53.000000 lsst_rsp-0.5.2/src/lsst/rsp/startup/storage/command.py
--rw-r--r--   0 runner    (1001) docker     (127)     3067 2024-04-22 23:47:53.000000 lsst_rsp-0.5.2/src/lsst/rsp/startup/storage/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     5240 2024-04-22 23:47:53.000000 lsst_rsp-0.5.2/src/lsst/rsp/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:47:58.076074 lsst_rsp-0.5.2/src/lsst_rsp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5444 2024-04-22 23:47:58.000000 lsst_rsp-0.5.2/src/lsst_rsp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-04-22 23:47:58.000000 lsst_rsp-0.5.2/src/lsst_rsp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 23:47:58.000000 lsst_rsp-0.5.2/src/lsst_rsp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-22 23:47:58.000000 lsst_rsp-0.5.2/src/lsst_rsp.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-22 23:47:58.000000 lsst_rsp-0.5.2/src/lsst_rsp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-22 23:47:58.000000 lsst_rsp-0.5.2/src/lsst_rsp.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:47:58.076074 lsst_rsp-0.5.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-22 23:47:53.000000 lsst_rsp-0.5.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-04-22 23:47:53.000000 lsst_rsp-0.5.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    11534 2024-04-22 23:47:53.000000 lsst_rsp-0.5.2/tests/startup_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:47:58.064073 lsst_rsp-0.5.2/tests/support/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:47:58.076074 lsst_rsp-0.5.2/tests/support/files/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-22 23:47:53.000000 lsst_rsp-0.5.2/tests/support/files/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:47:58.076074 lsst_rsp-0.5.2/tests/support/files/etc/
--rw-r--r--   0 runner    (1001) docker     (127)    10287 2024-04-22 23:47:53.000000 lsst_rsp-0.5.2/tests/support/files/etc/dircolors.ansi-universal
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:47:58.076074 lsst_rsp-0.5.2/tests/support/files/etc/skel/
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-22 23:47:53.000000 lsst_rsp-0.5.2/tests/support/files/etc/skel/.gitconfig
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-04-22 23:47:53.000000 lsst_rsp-0.5.2/tests/support/files/etc/skel/.pythonrc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:47:58.076074 lsst_rsp-0.5.2/tests/support/files/etc/skel/notebooks/
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-22 23:47:53.000000 lsst_rsp-0.5.2/tests/support/files/etc/skel/notebooks/.user_setups
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:47:58.064073 lsst_rsp-0.5.2/tests/support/files/homedir/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:47:58.076074 lsst_rsp-0.5.2/tests/support/files/homedir/.lsst/
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-22 23:47:53.000000 lsst_rsp-0.5.2/tests/support/files/homedir/.lsst/aws-credentials.ini
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-22 23:47:53.000000 lsst_rsp-0.5.2/tests/support/files/homedir/.lsst/postgres-credentials.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:47:58.068073 lsst_rsp-0.5.2/tests/support/files/stack_top/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:47:58.076074 lsst_rsp-0.5.2/tests/support/files/stack_top/jupyterlab/
--rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-04-22 23:47:53.000000 lsst_rsp-0.5.2/tests/support/files/stack_top/jupyterlab/20-logging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:47:58.076074 lsst_rsp-0.5.2/tests/support/files/stack_top/jupyterlab/secrets/
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-22 23:47:53.000000 lsst_rsp-0.5.2/tests/support/files/stack_top/jupyterlab/secrets/aws-credentials.ini
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-22 23:47:53.000000 lsst_rsp-0.5.2/tests/support/files/stack_top/jupyterlab/secrets/postgres-credentials.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-22 23:47:53.000000 lsst_rsp-0.5.2/tests/utils_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-22 23:47:53.000000 lsst_rsp-0.5.2/tests/version_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-22 23:47:53.000000 lsst_rsp-0.5.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:19:22.308573 lsst_rsp-0.5.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:19:22.300573 lsst_rsp-0.5.3/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-09 23:19:17.000000 lsst_rsp-0.5.3/.github/CODE_OF_CONDUCT
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-09 23:19:17.000000 lsst_rsp-0.5.3/.github/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-09 23:19:17.000000 lsst_rsp-0.5.3/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:19:22.300573 lsst_rsp-0.5.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-05-09 23:19:17.000000 lsst_rsp-0.5.3/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-09 23:19:17.000000 lsst_rsp-0.5.3/.github/workflows/periodic-ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-05-09 23:19:17.000000 lsst_rsp-0.5.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-05-09 23:19:17.000000 lsst_rsp-0.5.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-05-09 23:19:17.000000 lsst_rsp-0.5.3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-05-09 23:19:17.000000 lsst_rsp-0.5.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 23:19:17.000000 lsst_rsp-0.5.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-09 23:19:17.000000 lsst_rsp-0.5.3/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     5514 2024-05-09 23:19:22.308573 lsst_rsp-0.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-05-09 23:19:17.000000 lsst_rsp-0.5.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:19:22.300573 lsst_rsp-0.5.3/changelog.d/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-09 23:19:17.000000 lsst_rsp-0.5.3/changelog.d/_template.md.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)     8347 2024-05-09 23:19:17.000000 lsst_rsp-0.5.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 23:19:22.308573 lsst_rsp-0.5.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:19:22.296573 lsst_rsp-0.5.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:19:22.300573 lsst_rsp-0.5.3/src/lsst/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-09 23:19:17.000000 lsst_rsp-0.5.3/src/lsst/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:19:22.300573 lsst_rsp-0.5.3/src/lsst/rsp/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-09 23:19:17.000000 lsst_rsp-0.5.3/src/lsst/rsp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2438 2024-05-09 23:19:17.000000 lsst_rsp-0.5.3/src/lsst/rsp/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-05-09 23:19:17.000000 lsst_rsp-0.5.3/src/lsst/rsp/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-05-09 23:19:17.000000 lsst_rsp-0.5.3/src/lsst/rsp/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-09 23:19:17.000000 lsst_rsp-0.5.3/src/lsst/rsp/service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:19:22.300573 lsst_rsp-0.5.3/src/lsst/rsp/startup/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 23:19:17.000000 lsst_rsp-0.5.3/src/lsst/rsp/startup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-09 23:19:17.000000 lsst_rsp-0.5.3/src/lsst/rsp/startup/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-05-09 23:19:17.000000 lsst_rsp-0.5.3/src/lsst/rsp/startup/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-05-09 23:19:17.000000 lsst_rsp-0.5.3/src/lsst/rsp/startup/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:19:22.300573 lsst_rsp-0.5.3/src/lsst/rsp/startup/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 23:19:17.000000 lsst_rsp-0.5.3/src/lsst/rsp/startup/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-05-09 23:19:17.000000 lsst_rsp-0.5.3/src/lsst/rsp/startup/models/noninteractive.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:19:22.300573 lsst_rsp-0.5.3/src/lsst/rsp/startup/services/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 23:19:17.000000 lsst_rsp-0.5.3/src/lsst/rsp/startup/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28035 2024-05-09 23:19:17.000000 lsst_rsp-0.5.3/src/lsst/rsp/startup/services/labrunner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:19:22.304573 lsst_rsp-0.5.3/src/lsst/rsp/startup/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 23:19:17.000000 lsst_rsp-0.5.3/src/lsst/rsp/startup/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4717 2024-05-09 23:19:17.000000 lsst_rsp-0.5.3/src/lsst/rsp/startup/storage/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3067 2024-05-09 23:19:17.000000 lsst_rsp-0.5.3/src/lsst/rsp/startup/storage/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5240 2024-05-09 23:19:17.000000 lsst_rsp-0.5.3/src/lsst/rsp/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:19:22.308573 lsst_rsp-0.5.3/src/lsst_rsp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5514 2024-05-09 23:19:22.000000 lsst_rsp-0.5.3/src/lsst_rsp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-05-09 23:19:22.000000 lsst_rsp-0.5.3/src/lsst_rsp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 23:19:22.000000 lsst_rsp-0.5.3/src/lsst_rsp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-09 23:19:22.000000 lsst_rsp-0.5.3/src/lsst_rsp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-09 23:19:22.000000 lsst_rsp-0.5.3/src/lsst_rsp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-09 23:19:22.000000 lsst_rsp-0.5.3/src/lsst_rsp.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:19:22.304573 lsst_rsp-0.5.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-09 23:19:17.000000 lsst_rsp-0.5.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-05-09 23:19:17.000000 lsst_rsp-0.5.3/tests/client_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-05-09 23:19:17.000000 lsst_rsp-0.5.3/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11534 2024-05-09 23:19:17.000000 lsst_rsp-0.5.3/tests/startup_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:19:22.296573 lsst_rsp-0.5.3/tests/support/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:19:22.304573 lsst_rsp-0.5.3/tests/support/files/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-09 23:19:17.000000 lsst_rsp-0.5.3/tests/support/files/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:19:22.296573 lsst_rsp-0.5.3/tests/support/files/client/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:19:22.296573 lsst_rsp-0.5.3/tests/support/files/client/jupyterlab/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:19:22.304573 lsst_rsp-0.5.3/tests/support/files/client/jupyterlab/environment/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-09 23:19:17.000000 lsst_rsp-0.5.3/tests/support/files/client/jupyterlab/environment/EXTERNAL_INSTANCE_URL
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:19:22.304573 lsst_rsp-0.5.3/tests/support/files/client/jupyterlab/secrets/
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-09 23:19:17.000000 lsst_rsp-0.5.3/tests/support/files/client/jupyterlab/secrets/token
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:19:22.304573 lsst_rsp-0.5.3/tests/support/files/etc/
+-rw-r--r--   0 runner    (1001) docker     (127)    10287 2024-05-09 23:19:17.000000 lsst_rsp-0.5.3/tests/support/files/etc/dircolors.ansi-universal
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:19:22.304573 lsst_rsp-0.5.3/tests/support/files/etc/skel/
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-09 23:19:17.000000 lsst_rsp-0.5.3/tests/support/files/etc/skel/.gitconfig
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-09 23:19:17.000000 lsst_rsp-0.5.3/tests/support/files/etc/skel/.pythonrc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:19:22.308573 lsst_rsp-0.5.3/tests/support/files/etc/skel/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-09 23:19:17.000000 lsst_rsp-0.5.3/tests/support/files/etc/skel/notebooks/.user_setups
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:19:22.296573 lsst_rsp-0.5.3/tests/support/files/homedir/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:19:22.308573 lsst_rsp-0.5.3/tests/support/files/homedir/.lsst/
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-09 23:19:17.000000 lsst_rsp-0.5.3/tests/support/files/homedir/.lsst/aws-credentials.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-09 23:19:17.000000 lsst_rsp-0.5.3/tests/support/files/homedir/.lsst/postgres-credentials.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:19:22.296573 lsst_rsp-0.5.3/tests/support/files/stack_top/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:19:22.308573 lsst_rsp-0.5.3/tests/support/files/stack_top/jupyterlab/
+-rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-05-09 23:19:17.000000 lsst_rsp-0.5.3/tests/support/files/stack_top/jupyterlab/20-logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:19:22.308573 lsst_rsp-0.5.3/tests/support/files/stack_top/jupyterlab/secrets/
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-09 23:19:17.000000 lsst_rsp-0.5.3/tests/support/files/stack_top/jupyterlab/secrets/aws-credentials.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-09 23:19:17.000000 lsst_rsp-0.5.3/tests/support/files/stack_top/jupyterlab/secrets/postgres-credentials.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-09 23:19:17.000000 lsst_rsp-0.5.3/tests/utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-09 23:19:17.000000 lsst_rsp-0.5.3/tests/version_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-05-09 23:19:17.000000 lsst_rsp-0.5.3/tox.ini
```

### Comparing `lsst_rsp-0.5.2/.github/CONTRIBUTING.md` & `lsst_rsp-0.5.3/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `lsst_rsp-0.5.2/.github/workflows/ci.yaml` & `lsst_rsp-0.5.3/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `lsst_rsp-0.5.2/.github/workflows/periodic-ci.yaml` & `lsst_rsp-0.5.3/.github/workflows/periodic-ci.yaml`

 * *Files identical despite different names*

### Comparing `lsst_rsp-0.5.2/.gitignore` & `lsst_rsp-0.5.3/.gitignore`

 * *Files identical despite different names*

### Comparing `lsst_rsp-0.5.2/.pre-commit-config.yaml` & `lsst_rsp-0.5.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lsst_rsp-0.5.2/LICENSE` & `lsst_rsp-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lsst_rsp-0.5.2/PKG-INFO` & `lsst_rsp-0.5.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lsst-rsp
-Version: 0.5.2
+Version: 0.5.3
 Summary: Utility functions for the Rubin Science Platform
 Author-email: "Association of Universities for Research in Astronomy, Inc. (AURA)" <sqre-admin@lists.lsst.org>
 License: MIT License
         
         Copyright (c) 2021-2024 Association of Universities for Research in Astronomy, Inc. (AURA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -40,22 +40,24 @@
 Classifier: Typing :: Typed
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: Deprecated<2
 Requires-Dist: IPython<9
 Requires-Dist: pyvo<2,>=1.5.0
+Requires-Dist: httpx<0.28
 Requires-Dist: structlog
 Requires-Dist: symbolicmode<3
 Provides-Extra: dev
 Requires-Dist: types-deprecated; extra == "dev"
 Requires-Dist: types-requests; extra == "dev"
 Requires-Dist: coverage[toml]; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-asyncio; extra == "dev"
+Requires-Dist: pytest-httpx; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: scriv; extra == "dev"
 
 # lsst-rsp
 
 This Python package provides utility functions for the [Rubin Science Platform](https://rsp.lsst.io/), primarily for use within the Notebook Aspect.
 These utility functions are documented in the [Notebook aspect documentation](https://rsp.lsst.io/guides/notebooks/index.html) for the Rubin Science Platform.
```

### Comparing `lsst_rsp-0.5.2/README.md` & `lsst_rsp-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `lsst_rsp-0.5.2/pyproject.toml` & `lsst_rsp-0.5.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     "Typing :: Typed",
 ]
 requires-python = ">=3.11"
 dependencies = [
     "Deprecated<2",
     "IPython<9",
     "pyvo>=1.5.0,<2",
+    "httpx<0.28",
     "structlog",  # Uses CalVer, not SemVer
     "symbolicmode<3",
 ]
 dynamic = ["version"]
 
 [[project.authors]]
 name = "Association of Universities for Research in Astronomy, Inc. (AURA)"
@@ -43,14 +44,15 @@
     # Typing
     "types-deprecated",
     "types-requests",
     # Testing
     "coverage[toml]",
     "pytest",
     "pytest-asyncio",
+    "pytest-httpx",
     "mypy",
     # Documentation
     "scriv",
 ]
 
 [project.urls]
 Homepage = "https://rsp.lsst.io/"
```

### Comparing `lsst_rsp-0.5.2/src/lsst/rsp/__init__.py` & `lsst_rsp-0.5.3/src/lsst/rsp/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 from .catalog import (
     get_catalog,
     get_obstap_service,
     get_tap_service,
     retrieve_query,
 )
+from .client import RSPClient
 from .log import IPythonHandler, forward_lsst_log
 from .service import get_datalink_result, get_siav2_service
 from .utils import (
     format_bytes,
     get_access_token,
     get_digest,
     get_hostname,
@@ -28,14 +29,15 @@
     # package is not installed
     __version__ = "0.0.0"
 
 
 __all__ = [
     "__version__",
     "IPythonHandler",
+    "RSPClient",
     "format_bytes",
     "forward_lsst_log",
     "get_access_token",
     "get_catalog",
     "get_datalink_result",
     "get_digest",
     "get_node",
```

### Comparing `lsst_rsp-0.5.2/src/lsst/rsp/catalog.py` & `lsst_rsp-0.5.3/src/lsst/rsp/catalog.py`

 * *Files identical despite different names*

### Comparing `lsst_rsp-0.5.2/src/lsst/rsp/log.py` & `lsst_rsp-0.5.3/src/lsst/rsp/log.py`

 * *Files identical despite different names*

### Comparing `lsst_rsp-0.5.2/src/lsst/rsp/service.py` & `lsst_rsp-0.5.3/src/lsst/rsp/service.py`

 * *Files identical despite different names*

### Comparing `lsst_rsp-0.5.2/src/lsst/rsp/startup/constants.py` & `lsst_rsp-0.5.3/src/lsst/rsp/startup/constants.py`

 * *Files identical despite different names*

### Comparing `lsst_rsp-0.5.2/src/lsst/rsp/startup/exceptions.py` & `lsst_rsp-0.5.3/src/lsst/rsp/startup/exceptions.py`

 * *Files identical despite different names*

### Comparing `lsst_rsp-0.5.2/src/lsst/rsp/startup/models/noninteractive.py` & `lsst_rsp-0.5.3/src/lsst/rsp/startup/models/noninteractive.py`

 * *Files identical despite different names*

### Comparing `lsst_rsp-0.5.2/src/lsst/rsp/startup/services/labrunner.py` & `lsst_rsp-0.5.3/src/lsst/rsp/startup/services/labrunner.py`

 * *Files 0% similar despite different names*

```diff
@@ -329,14 +329,17 @@
             if user_loghash in PREVIOUS_LOGGING_CHECKSUMS:
                 self._logger.debug(
                     f"User log profile '{user_loghash}' is"
                     " out-of-date; replacing with current version."
                 )
                 copy = True
         if copy:
+            pdir = user_profile.parent
+            if not pdir:
+                pdir.mkdir(parents=True)
             user_profile.write_bytes(
                 (TOP_DIR_PATH / "jupyterlab" / "20-logging.py").read_bytes()
             )
 
     def _copy_dircolors(self) -> None:
         self._logger.debug("Copying dircolors if needed")
         if not (self._home / ".dir_colors").exists():
```

### Comparing `lsst_rsp-0.5.2/src/lsst/rsp/startup/storage/command.py` & `lsst_rsp-0.5.3/src/lsst/rsp/startup/storage/command.py`

 * *Files identical despite different names*

### Comparing `lsst_rsp-0.5.2/src/lsst/rsp/startup/storage/logging.py` & `lsst_rsp-0.5.3/src/lsst/rsp/startup/storage/logging.py`

 * *Files identical despite different names*

### Comparing `lsst_rsp-0.5.2/src/lsst/rsp/utils.py` & `lsst_rsp-0.5.3/src/lsst/rsp/utils.py`

 * *Files identical despite different names*

### Comparing `lsst_rsp-0.5.2/src/lsst_rsp.egg-info/PKG-INFO` & `lsst_rsp-0.5.3/src/lsst_rsp.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lsst-rsp
-Version: 0.5.2
+Version: 0.5.3
 Summary: Utility functions for the Rubin Science Platform
 Author-email: "Association of Universities for Research in Astronomy, Inc. (AURA)" <sqre-admin@lists.lsst.org>
 License: MIT License
         
         Copyright (c) 2021-2024 Association of Universities for Research in Astronomy, Inc. (AURA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -40,22 +40,24 @@
 Classifier: Typing :: Typed
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: Deprecated<2
 Requires-Dist: IPython<9
 Requires-Dist: pyvo<2,>=1.5.0
+Requires-Dist: httpx<0.28
 Requires-Dist: structlog
 Requires-Dist: symbolicmode<3
 Provides-Extra: dev
 Requires-Dist: types-deprecated; extra == "dev"
 Requires-Dist: types-requests; extra == "dev"
 Requires-Dist: coverage[toml]; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-asyncio; extra == "dev"
+Requires-Dist: pytest-httpx; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: scriv; extra == "dev"
 
 # lsst-rsp
 
 This Python package provides utility functions for the [Rubin Science Platform](https://rsp.lsst.io/), primarily for use within the Notebook Aspect.
 These utility functions are documented in the [Notebook aspect documentation](https://rsp.lsst.io/guides/notebooks/index.html) for the Rubin Science Platform.
```

### Comparing `lsst_rsp-0.5.2/src/lsst_rsp.egg-info/SOURCES.txt` & `lsst_rsp-0.5.3/src/lsst_rsp.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 .github/dependabot.yml
 .github/workflows/ci.yaml
 .github/workflows/periodic-ci.yaml
 changelog.d/_template.md.jinja
 src/lsst/__init__.py
 src/lsst/rsp/__init__.py
 src/lsst/rsp/catalog.py
+src/lsst/rsp/client.py
 src/lsst/rsp/log.py
 src/lsst/rsp/service.py
 src/lsst/rsp/utils.py
 src/lsst/rsp/startup/__init__.py
 src/lsst/rsp/startup/cli.py
 src/lsst/rsp/startup/constants.py
 src/lsst/rsp/startup/exceptions.py
@@ -33,19 +34,22 @@
 src/lsst_rsp.egg-info/PKG-INFO
 src/lsst_rsp.egg-info/SOURCES.txt
 src/lsst_rsp.egg-info/dependency_links.txt
 src/lsst_rsp.egg-info/entry_points.txt
 src/lsst_rsp.egg-info/requires.txt
 src/lsst_rsp.egg-info/top_level.txt
 tests/__init__.py
+tests/client_test.py
 tests/conftest.py
 tests/startup_test.py
 tests/utils_test.py
 tests/version_test.py
 tests/support/files/README.md
+tests/support/files/client/jupyterlab/environment/EXTERNAL_INSTANCE_URL
+tests/support/files/client/jupyterlab/secrets/token
 tests/support/files/etc/dircolors.ansi-universal
 tests/support/files/etc/skel/.gitconfig
 tests/support/files/etc/skel/.pythonrc
 tests/support/files/etc/skel/notebooks/.user_setups
 tests/support/files/homedir/.lsst/aws-credentials.ini
 tests/support/files/homedir/.lsst/postgres-credentials.txt
 tests/support/files/stack_top/jupyterlab/20-logging.py
```

### Comparing `lsst_rsp-0.5.2/tests/conftest.py` & `lsst_rsp-0.5.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `lsst_rsp-0.5.2/tests/startup_test.py` & `lsst_rsp-0.5.3/tests/startup_test.py`

 * *Files identical despite different names*

### Comparing `lsst_rsp-0.5.2/tests/support/files/etc/dircolors.ansi-universal` & `lsst_rsp-0.5.3/tests/support/files/etc/dircolors.ansi-universal`

 * *Files identical despite different names*

### Comparing `lsst_rsp-0.5.2/tests/support/files/stack_top/jupyterlab/20-logging.py` & `lsst_rsp-0.5.3/tests/support/files/stack_top/jupyterlab/20-logging.py`

 * *Files identical despite different names*

### Comparing `lsst_rsp-0.5.2/tests/utils_test.py` & `lsst_rsp-0.5.3/tests/utils_test.py`

 * *Files identical despite different names*

### Comparing `lsst_rsp-0.5.2/tox.ini` & `lsst_rsp-0.5.3/tox.ini`

 * *Files identical despite different names*

