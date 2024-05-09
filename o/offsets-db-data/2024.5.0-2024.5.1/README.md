# Comparing `tmp/offsets_db_data-2024.5.0.tar.gz` & `tmp/offsets_db_data-2024.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "offsets_db_data-2024.5.0.tar", last modified: Fri May  3 18:38:18 2024, max compression
+gzip compressed data, was "offsets_db_data-2024.5.1.tar", last modified: Thu May  9 22:40:38 2024, max compression
```

## Comparing `offsets_db_data-2024.5.0.tar` & `offsets_db_data-2024.5.1.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:38:18.807181 offsets_db_data-2024.5.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:38:18.799181 offsets_db_data-2024.5.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-03 18:38:08.000000 offsets_db_data-2024.5.0/.github/dependabot.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:38:18.799181 offsets_db_data-2024.5.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-05-03 18:38:08.000000 offsets_db_data-2024.5.0/.github/workflows/CI.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-05-03 18:38:08.000000 offsets_db_data-2024.5.0/.github/workflows/pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3156 2024-05-03 18:38:08.000000 offsets_db_data-2024.5.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-03 18:38:08.000000 offsets_db_data-2024.5.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 18:38:08.000000 offsets_db_data-2024.5.0/.prettierignore
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-03 18:38:08.000000 offsets_db_data-2024.5.0/.prettierrc.json
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-03 18:38:08.000000 offsets_db_data-2024.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4318 2024-05-03 18:38:18.807181 offsets_db_data-2024.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-05-03 18:38:08.000000 offsets_db_data-2024.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-05-03 18:38:08.000000 offsets_db_data-2024.5.0/TERMS_OF_DATA_ACCESS
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:38:18.799181 offsets_db_data-2024.5.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-05-03 18:38:08.000000 offsets_db_data-2024.5.0/docs/TERMS-OF-DATA-ACCESS.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:38:18.799181 offsets_db_data-2024.5.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)    26339 2024-05-03 18:38:08.000000 offsets_db_data-2024.5.0/docs/_static/monogram-dark-cropped.png
--rw-r--r--   0 runner    (1001) docker     (127)    23620 2024-05-03 18:38:08.000000 offsets_db_data-2024.5.0/docs/_static/monogram-light-cropped.png
--rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-05-03 18:38:08.000000 offsets_db_data-2024.5.0/docs/api.md
--rw-r--r--   0 runner    (1001) docker     (127)     2897 2024-05-03 18:38:08.000000 offsets_db_data-2024.5.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     3323 2024-05-03 18:38:08.000000 offsets_db_data-2024.5.0/docs/data-access.md
--rw-r--r--   0 runner    (1001) docker     (127)    18920 2024-05-03 18:38:08.000000 offsets_db_data-2024.5.0/docs/data-processing.md
--rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-05-03 18:38:08.000000 offsets_db_data-2024.5.0/docs/glossary.md
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-05-03 18:38:08.000000 offsets_db_data-2024.5.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-03 18:38:08.000000 offsets_db_data-2024.5.0/docs/install-offsets-db-data.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:38:18.803181 offsets_db_data-2024.5.0/offsets_db_data/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-03 18:38:08.000000 offsets_db_data-2024.5.0/offsets_db_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-03 18:38:18.000000 offsets_db_data-2024.5.0/offsets_db_data/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     7205 2024-05-03 18:38:08.000000 offsets_db_data-2024.5.0/offsets_db_data/apx.py
--rw-r--r--   0 runner    (1001) docker     (127)     5205 2024-05-03 18:38:08.000000 offsets_db_data-2024.5.0/offsets_db_data/arb.py
--rw-r--r--   0 runner    (1001) docker     (127)     6279 2024-05-03 18:38:08.000000 offsets_db_data-2024.5.0/offsets_db_data/catalog.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5480 2024-05-03 18:38:08.000000 offsets_db_data-2024.5.0/offsets_db_data/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:38:18.803181 offsets_db_data-2024.5.0/offsets_db_data/configs/
--rw-r--r--   0 runner    (1001) docker     (127)    84264 2024-05-03 18:38:08.000000 offsets_db_data-2024.5.0/offsets_db_data/configs/all-protocol-mapping.json
--rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-05-03 18:38:08.000000 offsets_db_data-2024.5.0/offsets_db_data/configs/credits-raw-columns-mapping.json
--rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-05-03 18:38:08.000000 offsets_db_data-2024.5.0/offsets_db_data/configs/projects-raw-columns-mapping.json
--rw-r--r--   0 runner    (1001) docker     (127)     3963 2024-05-03 18:38:08.000000 offsets_db_data-2024.5.0/offsets_db_data/credits.py
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-03 18:38:08.000000 offsets_db_data-2024.5.0/offsets_db_data/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     8586 2024-05-03 18:38:08.000000 offsets_db_data-2024.5.0/offsets_db_data/gld.py
--rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-05-03 18:38:08.000000 offsets_db_data-2024.5.0/offsets_db_data/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    10459 2024-05-03 18:38:08.000000 offsets_db_data-2024.5.0/offsets_db_data/projects.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 18:38:08.000000 offsets_db_data-2024.5.0/offsets_db_data/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-05-03 18:38:08.000000 offsets_db_data-2024.5.0/offsets_db_data/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)    12258 2024-05-03 18:38:08.000000 offsets_db_data-2024.5.0/offsets_db_data/vcs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:38:18.807181 offsets_db_data-2024.5.0/offsets_db_data.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4318 2024-05-03 18:38:18.000000 offsets_db_data-2024.5.0/offsets_db_data.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-05-03 18:38:18.000000 offsets_db_data-2024.5.0/offsets_db_data.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 18:38:18.000000 offsets_db_data-2024.5.0/offsets_db_data.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-03 18:38:18.000000 offsets_db_data-2024.5.0/offsets_db_data.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-03 18:38:18.000000 offsets_db_data-2024.5.0/offsets_db_data.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3140 2024-05-03 18:38:08.000000 offsets_db_data-2024.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-05-03 18:38:08.000000 offsets_db_data-2024.5.0/readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-03 18:38:08.000000 offsets_db_data-2024.5.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-03 18:38:08.000000 offsets_db_data-2024.5.0/requirements-docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-03 18:38:08.000000 offsets_db_data-2024.5.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 18:38:18.807181 offsets_db_data-2024.5.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:38:18.803181 offsets_db_data-2024.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 18:38:08.000000 offsets_db_data-2024.5.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4626 2024-05-03 18:38:08.000000 offsets_db_data-2024.5.0/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)    22092 2024-05-03 18:38:08.000000 offsets_db_data-2024.5.0/tests/test_vcs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:40:38.268908 offsets_db_data-2024.5.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:40:38.260908 offsets_db_data-2024.5.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-09 22:40:26.000000 offsets_db_data-2024.5.1/.github/dependabot.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:40:38.260908 offsets_db_data-2024.5.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-05-09 22:40:26.000000 offsets_db_data-2024.5.1/.github/workflows/CI.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-05-09 22:40:26.000000 offsets_db_data-2024.5.1/.github/workflows/pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3156 2024-05-09 22:40:26.000000 offsets_db_data-2024.5.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-09 22:40:26.000000 offsets_db_data-2024.5.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 22:40:26.000000 offsets_db_data-2024.5.1/.prettierignore
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-09 22:40:26.000000 offsets_db_data-2024.5.1/.prettierrc.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-09 22:40:26.000000 offsets_db_data-2024.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4318 2024-05-09 22:40:38.268908 offsets_db_data-2024.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-05-09 22:40:26.000000 offsets_db_data-2024.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-05-09 22:40:26.000000 offsets_db_data-2024.5.1/TERMS_OF_DATA_ACCESS
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:40:38.260908 offsets_db_data-2024.5.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-05-09 22:40:26.000000 offsets_db_data-2024.5.1/docs/TERMS-OF-DATA-ACCESS.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:40:38.260908 offsets_db_data-2024.5.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    26339 2024-05-09 22:40:26.000000 offsets_db_data-2024.5.1/docs/_static/monogram-dark-cropped.png
+-rw-r--r--   0 runner    (1001) docker     (127)    23620 2024-05-09 22:40:26.000000 offsets_db_data-2024.5.1/docs/_static/monogram-light-cropped.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-05-09 22:40:26.000000 offsets_db_data-2024.5.1/docs/api.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2897 2024-05-09 22:40:26.000000 offsets_db_data-2024.5.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3323 2024-05-09 22:40:26.000000 offsets_db_data-2024.5.1/docs/data-access.md
+-rw-r--r--   0 runner    (1001) docker     (127)    18920 2024-05-09 22:40:26.000000 offsets_db_data-2024.5.1/docs/data-processing.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-05-09 22:40:26.000000 offsets_db_data-2024.5.1/docs/glossary.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-05-09 22:40:26.000000 offsets_db_data-2024.5.1/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-09 22:40:26.000000 offsets_db_data-2024.5.1/docs/install-offsets-db-data.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:40:38.264908 offsets_db_data-2024.5.1/offsets_db_data/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-09 22:40:26.000000 offsets_db_data-2024.5.1/offsets_db_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-09 22:40:38.000000 offsets_db_data-2024.5.1/offsets_db_data/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7399 2024-05-09 22:40:26.000000 offsets_db_data-2024.5.1/offsets_db_data/apx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5205 2024-05-09 22:40:26.000000 offsets_db_data-2024.5.1/offsets_db_data/arb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6279 2024-05-09 22:40:26.000000 offsets_db_data-2024.5.1/offsets_db_data/catalog.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5480 2024-05-09 22:40:26.000000 offsets_db_data-2024.5.1/offsets_db_data/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:40:38.264908 offsets_db_data-2024.5.1/offsets_db_data/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)    84264 2024-05-09 22:40:26.000000 offsets_db_data-2024.5.1/offsets_db_data/configs/all-protocol-mapping.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-05-09 22:40:26.000000 offsets_db_data-2024.5.1/offsets_db_data/configs/credits-raw-columns-mapping.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-05-09 22:40:26.000000 offsets_db_data-2024.5.1/offsets_db_data/configs/projects-raw-columns-mapping.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3963 2024-05-09 22:40:26.000000 offsets_db_data-2024.5.1/offsets_db_data/credits.py
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-09 22:40:26.000000 offsets_db_data-2024.5.1/offsets_db_data/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8586 2024-05-09 22:40:26.000000 offsets_db_data-2024.5.1/offsets_db_data/gld.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-05-09 22:40:26.000000 offsets_db_data-2024.5.1/offsets_db_data/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10459 2024-05-09 22:40:26.000000 offsets_db_data-2024.5.1/offsets_db_data/projects.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 22:40:26.000000 offsets_db_data-2024.5.1/offsets_db_data/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-05-09 22:40:26.000000 offsets_db_data-2024.5.1/offsets_db_data/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12258 2024-05-09 22:40:26.000000 offsets_db_data-2024.5.1/offsets_db_data/vcs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:40:38.264908 offsets_db_data-2024.5.1/offsets_db_data.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4318 2024-05-09 22:40:38.000000 offsets_db_data-2024.5.1/offsets_db_data.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-05-09 22:40:38.000000 offsets_db_data-2024.5.1/offsets_db_data.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 22:40:38.000000 offsets_db_data-2024.5.1/offsets_db_data.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-09 22:40:38.000000 offsets_db_data-2024.5.1/offsets_db_data.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-09 22:40:38.000000 offsets_db_data-2024.5.1/offsets_db_data.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3140 2024-05-09 22:40:26.000000 offsets_db_data-2024.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-05-09 22:40:26.000000 offsets_db_data-2024.5.1/readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-09 22:40:26.000000 offsets_db_data-2024.5.1/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-09 22:40:26.000000 offsets_db_data-2024.5.1/requirements-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-09 22:40:26.000000 offsets_db_data-2024.5.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 22:40:38.268908 offsets_db_data-2024.5.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 22:40:38.264908 offsets_db_data-2024.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 22:40:26.000000 offsets_db_data-2024.5.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4626 2024-05-09 22:40:26.000000 offsets_db_data-2024.5.1/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22092 2024-05-09 22:40:26.000000 offsets_db_data-2024.5.1/tests/test_vcs.py
```

### Comparing `offsets_db_data-2024.5.0/.github/workflows/CI.yaml` & `offsets_db_data-2024.5.1/.github/workflows/CI.yaml`

 * *Files identical despite different names*

### Comparing `offsets_db_data-2024.5.0/.github/workflows/pypi.yaml` & `offsets_db_data-2024.5.1/.github/workflows/pypi.yaml`

 * *Files identical despite different names*

### Comparing `offsets_db_data-2024.5.0/.gitignore` & `offsets_db_data-2024.5.1/.gitignore`

 * *Files identical despite different names*

### Comparing `offsets_db_data-2024.5.0/.pre-commit-config.yaml` & `offsets_db_data-2024.5.1/.pre-commit-config.yaml`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 ci:
   autoupdate_schedule: monthly
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.5.0
+    rev: v4.6.0
     hooks:
       - id: trailing-whitespace
       - id: end-of-file-fixer
       - id: check-docstring-first
       - id: check-json
       - id: check-yaml
       - id: double-quote-string-fixer
       - id: debug-statements
       - id: mixed-line-ending
 
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: 'v0.3.5'
+    rev: 'v0.4.3'
     hooks:
       - id: ruff
         args: ['--fix']
       - id: ruff-format
 
   - repo: https://github.com/pre-commit/mirrors-prettier
     rev: v4.0.0-alpha.8
```

### Comparing `offsets_db_data-2024.5.0/LICENSE` & `offsets_db_data-2024.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `offsets_db_data-2024.5.0/PKG-INFO` & `offsets_db_data-2024.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: offsets-db-data
-Version: 2024.5.0
+Version: 2024.5.1
 Summary: Monitoring the global carbon market
 Author-email: CarbonPlan <tech@carbonplan.org>
 License: MIT
 Project-URL: repository, https://github.com/carbonplan/offsets-db-data
 Project-URL: documentation, https://offsets-db-data.readthedocs.io/
 Project-URL: database web tool, https://carbonplan.org/research/offsets-db
 Project-URL: explainer, https://carbonplan.org/research/offsets-db-explainer
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: offsets-db-data Version: 2024.5.0 Summary:
+Metadata-Version: 2.1 Name: offsets-db-data Version: 2024.5.1 Summary:
 Monitoring the global carbon market Author-email: CarbonPlan
 carbonplan.org> License: MIT Project-URL: repository, https://github.com/
 carbonplan/offsets-db-data Project-URL: documentation, https://offsets-db-
 data.readthedocs.io/ Project-URL: database web tool, https://carbonplan.org/
 research/offsets-db Project-URL: explainer, https://carbonplan.org/research/
 offsets-db-explainer Classifier: Development Status :: 4 - Beta Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
```

### Comparing `offsets_db_data-2024.5.0/README.md` & `offsets_db_data-2024.5.1/README.md`

 * *Files identical despite different names*

### Comparing `offsets_db_data-2024.5.0/TERMS_OF_DATA_ACCESS` & `offsets_db_data-2024.5.1/TERMS_OF_DATA_ACCESS`

 * *Files identical despite different names*

### Comparing `offsets_db_data-2024.5.0/docs/TERMS-OF-DATA-ACCESS.md` & `offsets_db_data-2024.5.1/docs/TERMS-OF-DATA-ACCESS.md`

 * *Files identical despite different names*

### Comparing `offsets_db_data-2024.5.0/docs/_static/monogram-dark-cropped.png` & `offsets_db_data-2024.5.1/docs/_static/monogram-dark-cropped.png`

 * *Files identical despite different names*

### Comparing `offsets_db_data-2024.5.0/docs/_static/monogram-light-cropped.png` & `offsets_db_data-2024.5.1/docs/_static/monogram-light-cropped.png`

 * *Files identical despite different names*

### Comparing `offsets_db_data-2024.5.0/docs/api.md` & `offsets_db_data-2024.5.1/docs/api.md`

 * *Files identical despite different names*

### Comparing `offsets_db_data-2024.5.0/docs/conf.py` & `offsets_db_data-2024.5.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `offsets_db_data-2024.5.0/docs/data-access.md` & `offsets_db_data-2024.5.1/docs/data-access.md`

 * *Files identical despite different names*

### Comparing `offsets_db_data-2024.5.0/docs/data-processing.md` & `offsets_db_data-2024.5.1/docs/data-processing.md`

 * *Files identical despite different names*

### Comparing `offsets_db_data-2024.5.0/docs/glossary.md` & `offsets_db_data-2024.5.1/docs/glossary.md`

 * *Files identical despite different names*

### Comparing `offsets_db_data-2024.5.0/docs/index.md` & `offsets_db_data-2024.5.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `offsets_db_data-2024.5.0/docs/install-offsets-db-data.md` & `offsets_db_data-2024.5.1/docs/install-offsets-db-data.md`

 * *Files identical despite different names*

### Comparing `offsets_db_data-2024.5.0/offsets_db_data/apx.py` & `offsets_db_data-2024.5.1/offsets_db_data/apx.py`

 * *Files 3% similar despite different names*

```diff
@@ -75,17 +75,21 @@
 
     columns = {v: k for k, v in column_mapping.items()}
 
     data = (
         df.set_registry(registry_name=registry_name)
         .determine_transaction_type(download_type=download_type)
         .rename(columns=columns)
-        .convert_to_datetime(columns=['transaction_date'])
     )
 
+    # split the date and time and keeping only the date. this helps with the inconsistency in the date format
+    data['transaction_date'] = data['transaction_date'].str.split().str[0]
+
+    data = data.convert_to_datetime(columns=['transaction_date'])
+
     if download_type == 'issuances':
         data = data.aggregate_issuance_transactions()
 
     data = data.validate(schema=credit_without_id_schema)
     if arb is not None and not arb.empty:
         data = data.merge_with_arb(arb=arb)
     return data
```

### Comparing `offsets_db_data-2024.5.0/offsets_db_data/arb.py` & `offsets_db_data-2024.5.1/offsets_db_data/arb.py`

 * *Files identical despite different names*

### Comparing `offsets_db_data-2024.5.0/offsets_db_data/catalog.yaml` & `offsets_db_data-2024.5.1/offsets_db_data/catalog.yaml`

 * *Files identical despite different names*

### Comparing `offsets_db_data-2024.5.0/offsets_db_data/common.py` & `offsets_db_data-2024.5.1/offsets_db_data/common.py`

 * *Files identical despite different names*

### Comparing `offsets_db_data-2024.5.0/offsets_db_data/configs/all-protocol-mapping.json` & `offsets_db_data-2024.5.1/offsets_db_data/configs/all-protocol-mapping.json`

 * *Files identical despite different names*

### Comparing `offsets_db_data-2024.5.0/offsets_db_data/configs/credits-raw-columns-mapping.json` & `offsets_db_data-2024.5.1/offsets_db_data/configs/credits-raw-columns-mapping.json`

 * *Files identical despite different names*

### Comparing `offsets_db_data-2024.5.0/offsets_db_data/configs/projects-raw-columns-mapping.json` & `offsets_db_data-2024.5.1/offsets_db_data/configs/projects-raw-columns-mapping.json`

 * *Files identical despite different names*

### Comparing `offsets_db_data-2024.5.0/offsets_db_data/credits.py` & `offsets_db_data-2024.5.1/offsets_db_data/credits.py`

 * *Files identical despite different names*

### Comparing `offsets_db_data-2024.5.0/offsets_db_data/gld.py` & `offsets_db_data-2024.5.1/offsets_db_data/gld.py`

 * *Files identical despite different names*

### Comparing `offsets_db_data-2024.5.0/offsets_db_data/models.py` & `offsets_db_data-2024.5.1/offsets_db_data/models.py`

 * *Files identical despite different names*

### Comparing `offsets_db_data-2024.5.0/offsets_db_data/projects.py` & `offsets_db_data-2024.5.1/offsets_db_data/projects.py`

 * *Files identical despite different names*

### Comparing `offsets_db_data-2024.5.0/offsets_db_data/registry.py` & `offsets_db_data-2024.5.1/offsets_db_data/registry.py`

 * *Files identical despite different names*

### Comparing `offsets_db_data-2024.5.0/offsets_db_data/vcs.py` & `offsets_db_data-2024.5.1/offsets_db_data/vcs.py`

 * *Files identical despite different names*

### Comparing `offsets_db_data-2024.5.0/offsets_db_data.egg-info/PKG-INFO` & `offsets_db_data-2024.5.1/offsets_db_data.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: offsets-db-data
-Version: 2024.5.0
+Version: 2024.5.1
 Summary: Monitoring the global carbon market
 Author-email: CarbonPlan <tech@carbonplan.org>
 License: MIT
 Project-URL: repository, https://github.com/carbonplan/offsets-db-data
 Project-URL: documentation, https://offsets-db-data.readthedocs.io/
 Project-URL: database web tool, https://carbonplan.org/research/offsets-db
 Project-URL: explainer, https://carbonplan.org/research/offsets-db-explainer
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: offsets-db-data Version: 2024.5.0 Summary:
+Metadata-Version: 2.1 Name: offsets-db-data Version: 2024.5.1 Summary:
 Monitoring the global carbon market Author-email: CarbonPlan
 carbonplan.org> License: MIT Project-URL: repository, https://github.com/
 carbonplan/offsets-db-data Project-URL: documentation, https://offsets-db-
 data.readthedocs.io/ Project-URL: database web tool, https://carbonplan.org/
 research/offsets-db Project-URL: explainer, https://carbonplan.org/research/
 offsets-db-explainer Classifier: Development Status :: 4 - Beta Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
```

### Comparing `offsets_db_data-2024.5.0/offsets_db_data.egg-info/SOURCES.txt` & `offsets_db_data-2024.5.1/offsets_db_data.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `offsets_db_data-2024.5.0/pyproject.toml` & `offsets_db_data-2024.5.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `offsets_db_data-2024.5.0/readthedocs.yml` & `offsets_db_data-2024.5.1/readthedocs.yml`

 * *Files identical despite different names*

### Comparing `offsets_db_data-2024.5.0/tests/test_integration.py` & `offsets_db_data-2024.5.1/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `offsets_db_data-2024.5.0/tests/test_vcs.py` & `offsets_db_data-2024.5.1/tests/test_vcs.py`

 * *Files identical despite different names*

