# Comparing `tmp/dynamicio-5.0.0rc2.tar.gz` & `tmp/dynamicio-5.0.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dynamicio-5.0.0rc2.tar", last modified: Thu May 11 16:17:35 2023, max compression
+gzip compressed data, was "dynamicio-5.0.0rc3.tar", last modified: Tue Feb 27 13:31:11 2024, max compression
```

## Comparing `dynamicio-5.0.0rc2.tar` & `dynamicio-5.0.0rc3.tar`

### file list

```diff
@@ -1,52 +1,76 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-11 16:17:35.051582 dynamicio-5.0.0rc2/
--rw-r--r--   0 circleci  (3434) circleci  (3434)    35149 2023-05-11 16:17:23.000000 dynamicio-5.0.0rc2/LICENSE
--rw-r--r--   0 circleci  (3434) circleci  (3434)    39883 2023-05-11 16:17:35.051582 dynamicio-5.0.0rc2/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)    39394 2023-05-11 16:17:23.000000 dynamicio-5.0.0rc2/README.md
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-11 16:17:35.047582 dynamicio-5.0.0rc2/dynamicio/
--rw-r--r--   0 circleci  (3434) circleci  (3434)       78 2023-05-11 16:17:23.000000 dynamicio-5.0.0rc2/dynamicio/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3151 2023-05-11 16:17:23.000000 dynamicio-5.0.0rc2/dynamicio/inject.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-11 16:17:35.047582 dynamicio-5.0.0rc2/dynamicio/io/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      289 2023-05-11 16:17:23.000000 dynamicio-5.0.0rc2/dynamicio/io/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-11 16:17:35.047582 dynamicio-5.0.0rc2/dynamicio/io/file/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      224 2023-05-11 16:17:23.000000 dynamicio-5.0.0rc2/dynamicio/io/file/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1407 2023-05-11 16:17:23.000000 dynamicio-5.0.0rc2/dynamicio/io/file/csv.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1665 2023-05-11 16:17:23.000000 dynamicio-5.0.0rc2/dynamicio/io/file/hdf.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1401 2023-05-11 16:17:23.000000 dynamicio-5.0.0rc2/dynamicio/io/file/json.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1441 2023-05-11 16:17:23.000000 dynamicio-5.0.0rc2/dynamicio/io/file/parquet.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3476 2023-05-11 16:17:23.000000 dynamicio-5.0.0rc2/dynamicio/io/kafka.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1959 2023-05-11 16:17:23.000000 dynamicio-5.0.0rc2/dynamicio/io/keyed.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7242 2023-05-11 16:17:23.000000 dynamicio-5.0.0rc2/dynamicio/io/postgres.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-11 16:17:35.051582 dynamicio-5.0.0rc2/dynamicio/io/s3/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      221 2023-05-11 16:17:23.000000 dynamicio-5.0.0rc2/dynamicio/io/s3/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2322 2023-05-11 16:17:23.000000 dynamicio-5.0.0rc2/dynamicio/io/s3/contexts.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2065 2023-05-11 16:17:23.000000 dynamicio-5.0.0rc2/dynamicio/io/s3/csv.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4881 2023-05-11 16:17:23.000000 dynamicio-5.0.0rc2/dynamicio/io/s3/hdf.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2062 2023-05-11 16:17:23.000000 dynamicio-5.0.0rc2/dynamicio/io/s3/json.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2108 2023-05-11 16:17:23.000000 dynamicio-5.0.0rc2/dynamicio/io/s3/parquet.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      522 2023-05-11 16:17:23.000000 dynamicio-5.0.0rc2/dynamicio/utils.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)       76 2023-05-11 16:17:23.000000 dynamicio-5.0.0rc2/dynamicio/validators.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-11 16:17:35.047582 dynamicio-5.0.0rc2/dynamicio.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)    39883 2023-05-11 16:17:35.000000 dynamicio-5.0.0rc2/dynamicio.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1007 2023-05-11 16:17:35.000000 dynamicio-5.0.0rc2/dynamicio.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-05-11 16:17:35.000000 dynamicio-5.0.0rc2/dynamicio.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       48 2023-05-11 16:17:35.000000 dynamicio-5.0.0rc2/dynamicio.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      309 2023-05-11 16:17:35.000000 dynamicio-5.0.0rc2/dynamicio.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       16 2023-05-11 16:17:35.000000 dynamicio-5.0.0rc2/dynamicio.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      705 2023-05-11 16:17:23.000000 dynamicio-5.0.0rc2/pyproject.toml
--rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2023-05-11 16:17:35.051582 dynamicio-5.0.0rc2/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1888 2023-05-11 16:17:23.000000 dynamicio-5.0.0rc2/setup.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-11 16:17:35.051582 dynamicio-5.0.0rc2/tests/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-05-11 16:17:23.000000 dynamicio-5.0.0rc2/tests/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      525 2023-05-11 16:17:23.000000 dynamicio-5.0.0rc2/tests/conftest.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      125 2023-05-11 16:17:23.000000 dynamicio-5.0.0rc2/tests/constants.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-11 16:17:35.051582 dynamicio-5.0.0rc2/tests/s3/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-05-11 16:17:23.000000 dynamicio-5.0.0rc2/tests/s3/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      762 2023-05-11 16:17:23.000000 dynamicio-5.0.0rc2/tests/s3/conftest.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3063 2023-05-11 16:17:23.000000 dynamicio-5.0.0rc2/tests/s3/test_hdf.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2693 2023-05-11 16:17:23.000000 dynamicio-5.0.0rc2/tests/s3/test_s3_implementations.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1444 2023-05-11 16:17:23.000000 dynamicio-5.0.0rc2/tests/test_file_implementations.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2315 2023-05-11 16:17:23.000000 dynamicio-5.0.0rc2/tests/test_inject.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1006 2023-05-11 16:17:23.000000 dynamicio-5.0.0rc2/tests/test_kafka.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1747 2023-05-11 16:17:23.000000 dynamicio-5.0.0rc2/tests/test_keyed.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7329 2023-05-11 16:17:23.000000 dynamicio-5.0.0rc2/tests/test_postgres.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2103 2023-05-11 16:17:23.000000 dynamicio-5.0.0rc2/tests/test_validations.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-02-27 13:31:11.447204 dynamicio-5.0.0rc3/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    35149 2024-02-27 13:30:58.000000 dynamicio-5.0.0rc3/LICENSE
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    39883 2024-02-27 13:31:11.447204 dynamicio-5.0.0rc3/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    39394 2024-02-27 13:30:58.000000 dynamicio-5.0.0rc3/README.md
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-02-27 13:31:11.439204 dynamicio-5.0.0rc3/demo/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-02-27 13:30:58.000000 dynamicio-5.0.0rc3/demo/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-02-27 13:31:11.439204 dynamicio-5.0.0rc3/demo/src/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      835 2024-02-27 13:30:58.000000 dynamicio-5.0.0rc3/demo/src/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      873 2024-02-27 13:30:58.000000 dynamicio-5.0.0rc3/demo/src/__main__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      198 2024-02-27 13:30:58.000000 dynamicio-5.0.0rc3/demo/src/constants.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      510 2024-02-27 13:30:58.000000 dynamicio-5.0.0rc3/demo/src/environment.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      972 2024-02-27 13:30:58.000000 dynamicio-5.0.0rc3/demo/src/io.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1904 2024-02-27 13:30:58.000000 dynamicio-5.0.0rc3/demo/src/runner_selection.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-02-27 13:31:11.439204 dynamicio-5.0.0rc3/demo/src/runners/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-02-27 13:30:58.000000 dynamicio-5.0.0rc3/demo/src/runners/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1203 2024-02-27 13:30:58.000000 dynamicio-5.0.0rc3/demo/src/runners/staging.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1397 2024-02-27 13:30:58.000000 dynamicio-5.0.0rc3/demo/src/runners/transform.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-02-27 13:31:11.443204 dynamicio-5.0.0rc3/demo/tests/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-02-27 13:30:58.000000 dynamicio-5.0.0rc3/demo/tests/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      820 2024-02-27 13:30:58.000000 dynamicio-5.0.0rc3/demo/tests/conftest.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      372 2024-02-27 13:30:58.000000 dynamicio-5.0.0rc3/demo/tests/constants.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-02-27 13:31:11.443204 dynamicio-5.0.0rc3/demo/tests/runners/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-02-27 13:30:58.000000 dynamicio-5.0.0rc3/demo/tests/runners/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-02-27 13:30:58.000000 dynamicio-5.0.0rc3/demo/tests/runners/conftest.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      404 2024-02-27 13:30:58.000000 dynamicio-5.0.0rc3/demo/tests/runners/test_staging.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      412 2024-02-27 13:30:58.000000 dynamicio-5.0.0rc3/demo/tests/runners/test_transform.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2068 2024-02-27 13:30:58.000000 dynamicio-5.0.0rc3/demo/tests/test_pipeline.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1180 2024-02-27 13:30:58.000000 dynamicio-5.0.0rc3/demo/tests/test_runner_selection.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-02-27 13:31:11.443204 dynamicio-5.0.0rc3/dynamicio/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1786 2024-02-27 13:30:58.000000 dynamicio-5.0.0rc3/dynamicio/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       66 2024-02-27 13:30:58.000000 dynamicio-5.0.0rc3/dynamicio/__main__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3711 2024-02-27 13:30:58.000000 dynamicio-5.0.0rc3/dynamicio/cli.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-02-27 13:31:11.443204 dynamicio-5.0.0rc3/dynamicio/config/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      134 2024-02-27 13:30:58.000000 dynamicio-5.0.0rc3/dynamicio/config/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     9530 2024-02-27 13:30:58.000000 dynamicio-5.0.0rc3/dynamicio/config/io_config.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-02-27 13:31:11.443204 dynamicio-5.0.0rc3/dynamicio/config/pydantic/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      408 2024-02-27 13:30:58.000000 dynamicio-5.0.0rc3/dynamicio/config/pydantic/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1415 2024-02-27 13:30:58.000000 dynamicio-5.0.0rc3/dynamicio/config/pydantic/config.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     9295 2024-02-27 13:30:58.000000 dynamicio-5.0.0rc3/dynamicio/config/pydantic/io_resources.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3270 2024-02-27 13:30:58.000000 dynamicio-5.0.0rc3/dynamicio/config/pydantic/table_schema.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    13784 2024-02-27 13:30:58.000000 dynamicio-5.0.0rc3/dynamicio/core.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3172 2024-02-27 13:30:58.000000 dynamicio-5.0.0rc3/dynamicio/errors.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5841 2024-02-27 13:30:58.000000 dynamicio-5.0.0rc3/dynamicio/metrics.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-02-27 13:31:11.447204 dynamicio-5.0.0rc3/dynamicio/mixins/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      321 2024-02-27 13:30:58.000000 dynamicio-5.0.0rc3/dynamicio/mixins/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4875 2024-02-27 13:30:58.000000 dynamicio-5.0.0rc3/dynamicio/mixins/utils.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7816 2024-02-27 13:30:58.000000 dynamicio-5.0.0rc3/dynamicio/mixins/with_kafka.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11316 2024-02-27 13:30:58.000000 dynamicio-5.0.0rc3/dynamicio/mixins/with_local.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8017 2024-02-27 13:30:58.000000 dynamicio-5.0.0rc3/dynamicio/mixins/with_postgres.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    18850 2024-02-27 13:30:58.000000 dynamicio-5.0.0rc3/dynamicio/mixins/with_s3.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-02-27 13:30:58.000000 dynamicio-5.0.0rc3/dynamicio/py.typed
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    13239 2024-02-27 13:30:58.000000 dynamicio-5.0.0rc3/dynamicio/validations.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-02-27 13:31:11.443204 dynamicio-5.0.0rc3/dynamicio.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    39883 2024-02-27 13:31:11.000000 dynamicio-5.0.0rc3/dynamicio.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1563 2024-02-27 13:31:11.000000 dynamicio-5.0.0rc3/dynamicio.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2024-02-27 13:31:11.000000 dynamicio-5.0.0rc3/dynamicio.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       48 2024-02-27 13:31:11.000000 dynamicio-5.0.0rc3/dynamicio.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      321 2024-02-27 13:31:11.000000 dynamicio-5.0.0rc3/dynamicio.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       21 2024-02-27 13:31:11.000000 dynamicio-5.0.0rc3/dynamicio.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      705 2024-02-27 13:30:58.000000 dynamicio-5.0.0rc3/pyproject.toml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2024-02-27 13:31:11.447204 dynamicio-5.0.0rc3/setup.cfg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1924 2024-02-27 13:30:58.000000 dynamicio-5.0.0rc3/setup.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-02-27 13:31:11.447204 dynamicio-5.0.0rc3/tests/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-02-27 13:30:58.000000 dynamicio-5.0.0rc3/tests/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    34498 2024-02-27 13:30:58.000000 dynamicio-5.0.0rc3/tests/conftest.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      469 2024-02-27 13:30:58.000000 dynamicio-5.0.0rc3/tests/constants.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-02-27 13:31:11.447204 dynamicio-5.0.0rc3/tests/mocking/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-02-27 13:30:58.000000 dynamicio-5.0.0rc3/tests/mocking/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4755 2024-02-27 13:30:58.000000 dynamicio-5.0.0rc3/tests/mocking/io.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      764 2024-02-27 13:30:58.000000 dynamicio-5.0.0rc3/tests/mocking/models.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    14102 2024-02-27 13:30:58.000000 dynamicio-5.0.0rc3/tests/test_cli.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6460 2024-02-27 13:30:58.000000 dynamicio-5.0.0rc3/tests/test_config.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    43997 2024-02-27 13:30:58.000000 dynamicio-5.0.0rc3/tests/test_core.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6108 2024-02-27 13:30:58.000000 dynamicio-5.0.0rc3/tests/test_metrics.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      485 2024-02-27 13:30:58.000000 dynamicio-5.0.0rc3/tests/test_table_schema.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    16810 2024-02-27 13:30:58.000000 dynamicio-5.0.0rc3/tests/test_validations.py
```

### Comparing `dynamicio-5.0.0rc2/LICENSE` & `dynamicio-5.0.0rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `dynamicio-5.0.0rc2/PKG-INFO` & `dynamicio-5.0.0rc3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynamicio
-Version: 5.0.0rc2
+Version: 5.0.0rc3
 Summary: Panda's wrapper for IO operations
 Author: Christos Hadjinikolis, Radu Ghitescu
 Author-email: christos.hadjinikolis@gmail.com, radu.ghitescu@gmail.com
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `dynamicio-5.0.0rc2/README.md` & `dynamicio-5.0.0rc3/README.md`

 * *Files identical despite different names*

### Comparing `dynamicio-5.0.0rc2/dynamicio.egg-info/PKG-INFO` & `dynamicio-5.0.0rc3/dynamicio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynamicio
-Version: 5.0.0rc2
+Version: 5.0.0rc3
 Summary: Panda's wrapper for IO operations
 Author: Christos Hadjinikolis, Radu Ghitescu
 Author-email: christos.hadjinikolis@gmail.com, radu.ghitescu@gmail.com
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `dynamicio-5.0.0rc2/pyproject.toml` & `dynamicio-5.0.0rc3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=62"]
 build-backend = "setuptools.build_meta"
 
 [tool.black]
 py38 = true
-line-length = 120
+line-length = 185
 include = '\.pyi?$'
 exclude = '''
 (
   /(
       \.git
     | \.mypy_cache
     | \.github
```

### Comparing `dynamicio-5.0.0rc2/setup.py` & `dynamicio-5.0.0rc3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Packaging and distribution configuration."""
 import os
+import warnings
 
 import setuptools
 
 VERSION_FILE = "./VERSION"
 
 
 def get_readme():
@@ -31,15 +32,16 @@
     if version is not None:
         return version
 
     if os.path.exists(VERSION_FILE):
         with open(VERSION_FILE, "r") as f:
             return f.read().strip()
 
-    raise ValueError("Could not determine build version")
+    warnings.warn("Could not determine build version")
+    return '0.0.0dev0'
 
 
 def read_requirements(file_path):
     """Reads a requirements file and returns a list of strings, each being a requirements.
 
     Args:
         file_path (str):
```

