# Comparing `tmp/mtg_ssm-2.6.8.dev3.tar.gz` & `tmp/mtg_ssm-2.6.8.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mtg_ssm-2.6.8.dev3.tar", last modified: Tue Mar 12 06:13:42 2024, max compression
+gzip compressed data, was "mtg_ssm-2.6.8.dev4.tar", last modified: Fri May 10 21:17:54 2024, max compression
```

## Comparing `mtg_ssm-2.6.8.dev3.tar` & `mtg_ssm-2.6.8.dev4.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 06:13:42.630324 mtg_ssm-2.6.8.dev3/
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-03-12 06:13:38.000000 mtg_ssm-2.6.8.dev3/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 06:13:42.618324 mtg_ssm-2.6.8.dev3/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-03-12 06:13:38.000000 mtg_ssm-2.6.8.dev3/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 06:13:42.618324 mtg_ssm-2.6.8.dev3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-03-12 06:13:38.000000 mtg_ssm-2.6.8.dev3/.github/workflows/integration.yml
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-03-12 06:13:38.000000 mtg_ssm-2.6.8.dev3/.github/workflows/pre-commit.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-03-12 06:13:38.000000 mtg_ssm-2.6.8.dev3/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-03-12 06:13:38.000000 mtg_ssm-2.6.8.dev3/.github/workflows/run-tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-03-12 06:13:38.000000 mtg_ssm-2.6.8.dev3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-03-12 06:13:38.000000 mtg_ssm-2.6.8.dev3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-03-12 06:13:38.000000 mtg_ssm-2.6.8.dev3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)    13040 2024-03-12 06:13:42.630324 mtg_ssm-2.6.8.dev3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10578 2024-03-12 06:13:38.000000 mtg_ssm-2.6.8.dev3/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-03-12 06:13:38.000000 mtg_ssm-2.6.8.dev3/TODO.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 06:13:42.618324 mtg_ssm-2.6.8.dev3/mtg_ssm/
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-03-12 06:13:38.000000 mtg_ssm-2.6.8.dev3/mtg_ssm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-03-12 06:13:42.000000 mtg_ssm-2.6.8.dev3/mtg_ssm/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 06:13:42.618324 mtg_ssm-2.6.8.dev3/mtg_ssm/containers/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-03-12 06:13:38.000000 mtg_ssm-2.6.8.dev3/mtg_ssm/containers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2540 2024-03-12 06:13:38.000000 mtg_ssm-2.6.8.dev3/mtg_ssm/containers/bundles.py
--rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-03-12 06:13:38.000000 mtg_ssm-2.6.8.dev3/mtg_ssm/containers/collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3017 2024-03-12 06:13:38.000000 mtg_ssm-2.6.8.dev3/mtg_ssm/containers/counts.py
--rw-r--r--   0 runner    (1001) docker     (127)     4573 2024-03-12 06:13:38.000000 mtg_ssm-2.6.8.dev3/mtg_ssm/containers/indexes.py
--rw-r--r--   0 runner    (1001) docker     (127)     4669 2024-03-12 06:13:38.000000 mtg_ssm-2.6.8.dev3/mtg_ssm/containers/legacy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 06:13:42.622325 mtg_ssm-2.6.8.dev3/mtg_ssm/mtg/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-12 06:13:38.000000 mtg_ssm-2.6.8.dev3/mtg_ssm/mtg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-03-12 06:13:38.000000 mtg_ssm-2.6.8.dev3/mtg_ssm/mtg/util.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-12 06:13:38.000000 mtg_ssm-2.6.8.dev3/mtg_ssm/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 06:13:42.622325 mtg_ssm-2.6.8.dev3/mtg_ssm/scryfall/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-03-12 06:13:38.000000 mtg_ssm-2.6.8.dev3/mtg_ssm/scryfall/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-03-12 06:13:38.000000 mtg_ssm-2.6.8.dev3/mtg_ssm/scryfall/fetcher.py
--rw-r--r--   0 runner    (1001) docker     (127)    11814 2024-03-12 06:13:38.000000 mtg_ssm-2.6.8.dev3/mtg_ssm/scryfall/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 06:13:42.622325 mtg_ssm-2.6.8.dev3/mtg_ssm/serialization/
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-03-12 06:13:38.000000 mtg_ssm-2.6.8.dev3/mtg_ssm/serialization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2561 2024-03-12 06:13:38.000000 mtg_ssm-2.6.8.dev3/mtg_ssm/serialization/csv.py
--rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-03-12 06:13:38.000000 mtg_ssm-2.6.8.dev3/mtg_ssm/serialization/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)    11075 2024-03-12 06:13:38.000000 mtg_ssm-2.6.8.dev3/mtg_ssm/serialization/xlsx.py
--rw-r--r--   0 runner    (1001) docker     (127)    10317 2024-03-12 06:13:38.000000 mtg_ssm-2.6.8.dev3/mtg_ssm/ssm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 06:13:42.626325 mtg_ssm-2.6.8.dev3/mtg_ssm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13040 2024-03-12 06:13:42.000000 mtg_ssm-2.6.8.dev3/mtg_ssm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-03-12 06:13:42.000000 mtg_ssm-2.6.8.dev3/mtg_ssm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-12 06:13:42.000000 mtg_ssm-2.6.8.dev3/mtg_ssm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-03-12 06:13:42.000000 mtg_ssm-2.6.8.dev3/mtg_ssm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-03-12 06:13:42.000000 mtg_ssm-2.6.8.dev3/mtg_ssm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-12 06:13:42.000000 mtg_ssm-2.6.8.dev3/mtg_ssm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3944 2024-03-12 06:13:38.000000 mtg_ssm-2.6.8.dev3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-12 06:13:42.630324 mtg_ssm-2.6.8.dev3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 06:13:42.622325 mtg_ssm-2.6.8.dev3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-03-12 06:13:38.000000 mtg_ssm-2.6.8.dev3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2738 2024-03-12 06:13:38.000000 mtg_ssm-2.6.8.dev3/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 06:13:42.622325 mtg_ssm-2.6.8.dev3/tests/containers/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-03-12 06:13:38.000000 mtg_ssm-2.6.8.dev3/tests/containers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3539 2024-03-12 06:13:38.000000 mtg_ssm-2.6.8.dev3/tests/containers/test_bundles.py
--rw-r--r--   0 runner    (1001) docker     (127)     6713 2024-03-12 06:13:38.000000 mtg_ssm-2.6.8.dev3/tests/containers/test_counts.py
--rw-r--r--   0 runner    (1001) docker     (127)    11862 2024-03-12 06:13:38.000000 mtg_ssm-2.6.8.dev3/tests/containers/test_indexes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3436 2024-03-12 06:13:38.000000 mtg_ssm-2.6.8.dev3/tests/containers/test_legacy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 06:13:42.626325 mtg_ssm-2.6.8.dev3/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-03-12 06:13:38.000000 mtg_ssm-2.6.8.dev3/tests/data/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-03-12 06:13:38.000000 mtg_ssm-2.6.8.dev3/tests/data/bulk_data.json
--rw-r--r--   0 runner    (1001) docker     (127)   517458 2024-03-12 06:13:38.000000 mtg_ssm-2.6.8.dev3/tests/data/cards.json
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-03-12 06:13:38.000000 mtg_ssm-2.6.8.dev3/tests/data/migrations.json
--rw-r--r--   0 runner    (1001) docker     (127)    31317 2024-03-12 06:13:38.000000 mtg_ssm-2.6.8.dev3/tests/data/sets.json
--rw-r--r--   0 runner    (1001) docker     (127)    15912 2024-03-12 06:13:38.000000 mtg_ssm-2.6.8.dev3/tests/data/sets1.json
--rw-r--r--   0 runner    (1001) docker     (127)    15519 2024-03-12 06:13:38.000000 mtg_ssm-2.6.8.dev3/tests/data/sets2.json
--rwxr-xr-x   0 runner    (1001) docker     (127)     6549 2024-03-12 06:13:38.000000 mtg_ssm-2.6.8.dev3/tests/gen_testdata.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 06:13:42.626325 mtg_ssm-2.6.8.dev3/tests/mtg/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-03-12 06:13:38.000000 mtg_ssm-2.6.8.dev3/tests/mtg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-03-12 06:13:38.000000 mtg_ssm-2.6.8.dev3/tests/mtg/test_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 06:13:42.626325 mtg_ssm-2.6.8.dev3/tests/scryfall/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-03-12 06:13:38.000000 mtg_ssm-2.6.8.dev3/tests/scryfall/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-03-12 06:13:38.000000 mtg_ssm-2.6.8.dev3/tests/scryfall/test_fetcher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 06:13:42.626325 mtg_ssm-2.6.8.dev3/tests/serialization/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-03-12 06:13:38.000000 mtg_ssm-2.6.8.dev3/tests/serialization/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 06:13:42.626325 mtg_ssm-2.6.8.dev3/tests/serialization/__snapshots__/
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-03-12 06:13:38.000000 mtg_ssm-2.6.8.dev3/tests/serialization/__snapshots__/test_csv.ambr
--rw-r--r--   0 runner    (1001) docker     (127)    22061 2024-03-12 06:13:38.000000 mtg_ssm-2.6.8.dev3/tests/serialization/__snapshots__/test_xlsx.ambr
--rw-r--r--   0 runner    (1001) docker     (127)     4823 2024-03-12 06:13:38.000000 mtg_ssm-2.6.8.dev3/tests/serialization/test_csv.py
--rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-03-12 06:13:38.000000 mtg_ssm-2.6.8.dev3/tests/serialization/test_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     6467 2024-03-12 06:13:38.000000 mtg_ssm-2.6.8.dev3/tests/serialization/test_xlsx.py
--rw-r--r--   0 runner    (1001) docker     (127)    16220 2024-03-12 06:13:38.000000 mtg_ssm-2.6.8.dev3/tests/test_ssm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:17:54.330349 mtg_ssm-2.6.8.dev4/
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-10 21:17:49.000000 mtg_ssm-2.6.8.dev4/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:17:54.314349 mtg_ssm-2.6.8.dev4/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-10 21:17:49.000000 mtg_ssm-2.6.8.dev4/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:17:54.314349 mtg_ssm-2.6.8.dev4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-10 21:17:49.000000 mtg_ssm-2.6.8.dev4/.github/workflows/integration.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-10 21:17:49.000000 mtg_ssm-2.6.8.dev4/.github/workflows/pre-commit.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-10 21:17:49.000000 mtg_ssm-2.6.8.dev4/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-05-10 21:17:49.000000 mtg_ssm-2.6.8.dev4/.github/workflows/run-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-05-10 21:17:49.000000 mtg_ssm-2.6.8.dev4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-05-10 21:17:49.000000 mtg_ssm-2.6.8.dev4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-05-10 21:17:49.000000 mtg_ssm-2.6.8.dev4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    13040 2024-05-10 21:17:54.330349 mtg_ssm-2.6.8.dev4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10578 2024-05-10 21:17:49.000000 mtg_ssm-2.6.8.dev4/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-10 21:17:49.000000 mtg_ssm-2.6.8.dev4/TODO.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:17:54.318349 mtg_ssm-2.6.8.dev4/mtg_ssm/
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-10 21:17:49.000000 mtg_ssm-2.6.8.dev4/mtg_ssm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-10 21:17:54.000000 mtg_ssm-2.6.8.dev4/mtg_ssm/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:17:54.318349 mtg_ssm-2.6.8.dev4/mtg_ssm/containers/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-10 21:17:49.000000 mtg_ssm-2.6.8.dev4/mtg_ssm/containers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2540 2024-05-10 21:17:49.000000 mtg_ssm-2.6.8.dev4/mtg_ssm/containers/bundles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-05-10 21:17:49.000000 mtg_ssm-2.6.8.dev4/mtg_ssm/containers/collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3017 2024-05-10 21:17:49.000000 mtg_ssm-2.6.8.dev4/mtg_ssm/containers/counts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4573 2024-05-10 21:17:49.000000 mtg_ssm-2.6.8.dev4/mtg_ssm/containers/indexes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4669 2024-05-10 21:17:49.000000 mtg_ssm-2.6.8.dev4/mtg_ssm/containers/legacy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:17:54.318349 mtg_ssm-2.6.8.dev4/mtg_ssm/mtg/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-10 21:17:49.000000 mtg_ssm-2.6.8.dev4/mtg_ssm/mtg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-05-10 21:17:49.000000 mtg_ssm-2.6.8.dev4/mtg_ssm/mtg/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 21:17:49.000000 mtg_ssm-2.6.8.dev4/mtg_ssm/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:17:54.318349 mtg_ssm-2.6.8.dev4/mtg_ssm/scryfall/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-10 21:17:49.000000 mtg_ssm-2.6.8.dev4/mtg_ssm/scryfall/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-05-10 21:17:49.000000 mtg_ssm-2.6.8.dev4/mtg_ssm/scryfall/fetcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11834 2024-05-10 21:17:49.000000 mtg_ssm-2.6.8.dev4/mtg_ssm/scryfall/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:17:54.318349 mtg_ssm-2.6.8.dev4/mtg_ssm/serialization/
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-10 21:17:49.000000 mtg_ssm-2.6.8.dev4/mtg_ssm/serialization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2561 2024-05-10 21:17:49.000000 mtg_ssm-2.6.8.dev4/mtg_ssm/serialization/csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-05-10 21:17:49.000000 mtg_ssm-2.6.8.dev4/mtg_ssm/serialization/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11075 2024-05-10 21:17:49.000000 mtg_ssm-2.6.8.dev4/mtg_ssm/serialization/xlsx.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10317 2024-05-10 21:17:49.000000 mtg_ssm-2.6.8.dev4/mtg_ssm/ssm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:17:54.326349 mtg_ssm-2.6.8.dev4/mtg_ssm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13040 2024-05-10 21:17:54.000000 mtg_ssm-2.6.8.dev4/mtg_ssm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-05-10 21:17:54.000000 mtg_ssm-2.6.8.dev4/mtg_ssm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 21:17:54.000000 mtg_ssm-2.6.8.dev4/mtg_ssm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-10 21:17:54.000000 mtg_ssm-2.6.8.dev4/mtg_ssm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-10 21:17:54.000000 mtg_ssm-2.6.8.dev4/mtg_ssm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-10 21:17:54.000000 mtg_ssm-2.6.8.dev4/mtg_ssm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3944 2024-05-10 21:17:49.000000 mtg_ssm-2.6.8.dev4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 21:17:54.330349 mtg_ssm-2.6.8.dev4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:17:54.322349 mtg_ssm-2.6.8.dev4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-10 21:17:49.000000 mtg_ssm-2.6.8.dev4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2738 2024-05-10 21:17:49.000000 mtg_ssm-2.6.8.dev4/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:17:54.322349 mtg_ssm-2.6.8.dev4/tests/containers/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-10 21:17:49.000000 mtg_ssm-2.6.8.dev4/tests/containers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3539 2024-05-10 21:17:49.000000 mtg_ssm-2.6.8.dev4/tests/containers/test_bundles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6713 2024-05-10 21:17:49.000000 mtg_ssm-2.6.8.dev4/tests/containers/test_counts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11862 2024-05-10 21:17:49.000000 mtg_ssm-2.6.8.dev4/tests/containers/test_indexes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3436 2024-05-10 21:17:49.000000 mtg_ssm-2.6.8.dev4/tests/containers/test_legacy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:17:54.322349 mtg_ssm-2.6.8.dev4/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-10 21:17:49.000000 mtg_ssm-2.6.8.dev4/tests/data/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-10 21:17:49.000000 mtg_ssm-2.6.8.dev4/tests/data/bulk_data.json
+-rw-r--r--   0 runner    (1001) docker     (127)   517458 2024-05-10 21:17:49.000000 mtg_ssm-2.6.8.dev4/tests/data/cards.json
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-05-10 21:17:49.000000 mtg_ssm-2.6.8.dev4/tests/data/migrations.json
+-rw-r--r--   0 runner    (1001) docker     (127)    31317 2024-05-10 21:17:49.000000 mtg_ssm-2.6.8.dev4/tests/data/sets.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15912 2024-05-10 21:17:49.000000 mtg_ssm-2.6.8.dev4/tests/data/sets1.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15519 2024-05-10 21:17:49.000000 mtg_ssm-2.6.8.dev4/tests/data/sets2.json
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6549 2024-05-10 21:17:49.000000 mtg_ssm-2.6.8.dev4/tests/gen_testdata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:17:54.322349 mtg_ssm-2.6.8.dev4/tests/mtg/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-10 21:17:49.000000 mtg_ssm-2.6.8.dev4/tests/mtg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-10 21:17:49.000000 mtg_ssm-2.6.8.dev4/tests/mtg/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:17:54.326349 mtg_ssm-2.6.8.dev4/tests/scryfall/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-10 21:17:49.000000 mtg_ssm-2.6.8.dev4/tests/scryfall/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-05-10 21:17:49.000000 mtg_ssm-2.6.8.dev4/tests/scryfall/test_fetcher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:17:54.326349 mtg_ssm-2.6.8.dev4/tests/serialization/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-10 21:17:49.000000 mtg_ssm-2.6.8.dev4/tests/serialization/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:17:54.326349 mtg_ssm-2.6.8.dev4/tests/serialization/__snapshots__/
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-10 21:17:49.000000 mtg_ssm-2.6.8.dev4/tests/serialization/__snapshots__/test_csv.ambr
+-rw-r--r--   0 runner    (1001) docker     (127)    22061 2024-05-10 21:17:49.000000 mtg_ssm-2.6.8.dev4/tests/serialization/__snapshots__/test_xlsx.ambr
+-rw-r--r--   0 runner    (1001) docker     (127)     4823 2024-05-10 21:17:49.000000 mtg_ssm-2.6.8.dev4/tests/serialization/test_csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-05-10 21:17:49.000000 mtg_ssm-2.6.8.dev4/tests/serialization/test_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6467 2024-05-10 21:17:49.000000 mtg_ssm-2.6.8.dev4/tests/serialization/test_xlsx.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16220 2024-05-10 21:17:49.000000 mtg_ssm-2.6.8.dev4/tests/test_ssm.py
```

### Comparing `mtg_ssm-2.6.8.dev3/.github/workflows/integration.yml` & `mtg_ssm-2.6.8.dev4/.github/workflows/integration.yml`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.8.dev3/.github/workflows/publish.yml` & `mtg_ssm-2.6.8.dev4/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.8.dev3/.github/workflows/run-tests.yml` & `mtg_ssm-2.6.8.dev4/.github/workflows/run-tests.yml`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.8.dev3/.gitignore` & `mtg_ssm-2.6.8.dev4/.gitignore`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.8.dev3/.pre-commit-config.yaml` & `mtg_ssm-2.6.8.dev4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.8.dev3/LICENSE.txt` & `mtg_ssm-2.6.8.dev4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.8.dev3/PKG-INFO` & `mtg_ssm-2.6.8.dev4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mtg_ssm
-Version: 2.6.8.dev3
+Version: 2.6.8.dev4
 Summary: A tool to manage Magic: the Gathering collection spreadsheets
 Author-email: George Leslie-Waksman <waksman@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/gwax/mtg_ssm
 Project-URL: Bug Tracker, https://github.com/gwax/mtg_ssm/issues
 Keywords: mtg,magic,collection,tracking,spreadsheet
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `mtg_ssm-2.6.8.dev3/README.rst` & `mtg_ssm-2.6.8.dev4/README.rst`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.8.dev3/mtg_ssm/containers/bundles.py` & `mtg_ssm-2.6.8.dev4/mtg_ssm/containers/bundles.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.8.dev3/mtg_ssm/containers/collection.py` & `mtg_ssm-2.6.8.dev4/mtg_ssm/containers/collection.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.8.dev3/mtg_ssm/containers/counts.py` & `mtg_ssm-2.6.8.dev4/mtg_ssm/containers/counts.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.8.dev3/mtg_ssm/containers/indexes.py` & `mtg_ssm-2.6.8.dev4/mtg_ssm/containers/indexes.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.8.dev3/mtg_ssm/containers/legacy.py` & `mtg_ssm-2.6.8.dev4/mtg_ssm/containers/legacy.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.8.dev3/mtg_ssm/mtg/util.py` & `mtg_ssm-2.6.8.dev4/mtg_ssm/mtg/util.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.8.dev3/mtg_ssm/scryfall/fetcher.py` & `mtg_ssm-2.6.8.dev4/mtg_ssm/scryfall/fetcher.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.8.dev3/mtg_ssm/scryfall/models.py` & `mtg_ssm-2.6.8.dev4/mtg_ssm/scryfall/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,14 +114,15 @@
     LESSON = "lesson"
     MIRACLE = "miracle"
     MOONELDRAZIDFC = "mooneldrazidfc"
     MOONREVERSEMOONDFC = "moonreversemoondfc"
     NYXBORN = "nyxborn"
     NYXTOUCHED = "nyxtouched"
     ORIGINPWDFC = "originpwdfc"
+    PROMO = "promo"
     SHATTEREDGLASS = "shatteredglass"
     SHOWCASE = "showcase"
     SNOW = "snow"
     STAMPED = "stamped"
     SUNMOONDFC = "sunmoondfc"
     TEXTLESS = "textless"
     THICK = "thick"
```

### Comparing `mtg_ssm-2.6.8.dev3/mtg_ssm/serialization/csv.py` & `mtg_ssm-2.6.8.dev4/mtg_ssm/serialization/csv.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.8.dev3/mtg_ssm/serialization/interface.py` & `mtg_ssm-2.6.8.dev4/mtg_ssm/serialization/interface.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.8.dev3/mtg_ssm/serialization/xlsx.py` & `mtg_ssm-2.6.8.dev4/mtg_ssm/serialization/xlsx.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.8.dev3/mtg_ssm/ssm.py` & `mtg_ssm-2.6.8.dev4/mtg_ssm/ssm.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.8.dev3/mtg_ssm.egg-info/PKG-INFO` & `mtg_ssm-2.6.8.dev4/mtg_ssm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mtg_ssm
-Version: 2.6.8.dev3
+Version: 2.6.8.dev4
 Summary: A tool to manage Magic: the Gathering collection spreadsheets
 Author-email: George Leslie-Waksman <waksman@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/gwax/mtg_ssm
 Project-URL: Bug Tracker, https://github.com/gwax/mtg_ssm/issues
 Keywords: mtg,magic,collection,tracking,spreadsheet
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `mtg_ssm-2.6.8.dev3/mtg_ssm.egg-info/SOURCES.txt` & `mtg_ssm-2.6.8.dev4/mtg_ssm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.8.dev3/pyproject.toml` & `mtg_ssm-2.6.8.dev4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.8.dev3/tests/conftest.py` & `mtg_ssm-2.6.8.dev4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.8.dev3/tests/containers/test_bundles.py` & `mtg_ssm-2.6.8.dev4/tests/containers/test_bundles.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.8.dev3/tests/containers/test_counts.py` & `mtg_ssm-2.6.8.dev4/tests/containers/test_counts.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.8.dev3/tests/containers/test_indexes.py` & `mtg_ssm-2.6.8.dev4/tests/containers/test_indexes.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.8.dev3/tests/containers/test_legacy.py` & `mtg_ssm-2.6.8.dev4/tests/containers/test_legacy.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.8.dev3/tests/data/bulk_data.json` & `mtg_ssm-2.6.8.dev4/tests/data/bulk_data.json`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.8.dev3/tests/data/cards.json` & `mtg_ssm-2.6.8.dev4/tests/data/cards.json`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.8.dev3/tests/data/migrations.json` & `mtg_ssm-2.6.8.dev4/tests/data/migrations.json`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.8.dev3/tests/data/sets.json` & `mtg_ssm-2.6.8.dev4/tests/data/sets.json`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.8.dev3/tests/data/sets1.json` & `mtg_ssm-2.6.8.dev4/tests/data/sets1.json`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.8.dev3/tests/data/sets2.json` & `mtg_ssm-2.6.8.dev4/tests/data/sets2.json`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.8.dev3/tests/gen_testdata.py` & `mtg_ssm-2.6.8.dev4/tests/gen_testdata.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.8.dev3/tests/mtg/test_util.py` & `mtg_ssm-2.6.8.dev4/tests/mtg/test_util.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.8.dev3/tests/scryfall/test_fetcher.py` & `mtg_ssm-2.6.8.dev4/tests/scryfall/test_fetcher.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.8.dev3/tests/serialization/__snapshots__/test_csv.ambr` & `mtg_ssm-2.6.8.dev4/tests/serialization/__snapshots__/test_csv.ambr`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.8.dev3/tests/serialization/__snapshots__/test_xlsx.ambr` & `mtg_ssm-2.6.8.dev4/tests/serialization/__snapshots__/test_xlsx.ambr`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.8.dev3/tests/serialization/test_csv.py` & `mtg_ssm-2.6.8.dev4/tests/serialization/test_csv.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.8.dev3/tests/serialization/test_interface.py` & `mtg_ssm-2.6.8.dev4/tests/serialization/test_interface.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.8.dev3/tests/serialization/test_xlsx.py` & `mtg_ssm-2.6.8.dev4/tests/serialization/test_xlsx.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.8.dev3/tests/test_ssm.py` & `mtg_ssm-2.6.8.dev4/tests/test_ssm.py`

 * *Files identical despite different names*

