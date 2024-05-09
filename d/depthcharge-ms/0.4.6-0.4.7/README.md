# Comparing `tmp/depthcharge_ms-0.4.6.tar.gz` & `tmp/depthcharge_ms-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "depthcharge_ms-0.4.6.tar", last modified: Wed May  8 06:00:31 2024, max compression
+gzip compressed data, was "depthcharge_ms-0.4.7.tar", last modified: Thu May  9 23:20:21 2024, max compression
```

## Comparing `depthcharge_ms-0.4.6.tar` & `depthcharge_ms-0.4.7.tar`

### file list

```diff
@@ -1,99 +1,99 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:00:31.304104 depthcharge_ms-0.4.6/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:00:31.288104 depthcharge_ms-0.4.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:00:31.292104 depthcharge_ms-0.4.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/.github/workflows/lint.yml
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5653 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     4973 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     3921 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-08 06:00:31.304104 depthcharge_ms-0.4.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:00:31.292104 depthcharge_ms-0.4.6/data/
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/data/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    12882 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/data/TMT10-Trial-8.mgf
--rw-r--r--   0 runner    (1001) docker     (127)   333839 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/data/TMT10-Trial-8.mzML
--rw-r--r--   0 runner    (1001) docker     (127)    67798 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/data/TMT10-Trial-8.mzXML
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:00:31.296105 depthcharge_ms-0.4.6/depthcharge/
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/depthcharge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/depthcharge/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:00:31.296105 depthcharge_ms-0.4.6/depthcharge/data/
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/depthcharge/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/depthcharge/data/analyte_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)    12035 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/depthcharge/data/arrow.py
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/depthcharge/data/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)    18146 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/depthcharge/data/parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/depthcharge/data/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)    18668 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/depthcharge/data/spectrum_datasets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:00:31.296105 depthcharge_ms-0.4.6/depthcharge/encoders/
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/depthcharge/encoders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6969 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/depthcharge/encoders/sinusoidal.py
--rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/depthcharge/feedforward.py
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/depthcharge/mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)    12905 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/depthcharge/primitives.py
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/depthcharge/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:00:31.296105 depthcharge_ms-0.4.6/depthcharge/tokenizers/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/depthcharge/tokenizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3996 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/depthcharge/tokenizers/molecules.py
--rw-r--r--   0 runner    (1001) docker     (127)    10042 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/depthcharge/tokenizers/peptides.py
--rw-r--r--   0 runner    (1001) docker     (127)     4948 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/depthcharge/tokenizers/tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:00:31.296105 depthcharge_ms-0.4.6/depthcharge/transformers/
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/depthcharge/transformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17251 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/depthcharge/transformers/analytes.py
--rw-r--r--   0 runner    (1001) docker     (127)     6812 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/depthcharge/transformers/spectra.py
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/depthcharge/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/depthcharge/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:00:31.304104 depthcharge_ms-0.4.6/depthcharge_ms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-08 06:00:31.000000 depthcharge_ms-0.4.6/depthcharge_ms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-05-08 06:00:31.000000 depthcharge_ms-0.4.6/depthcharge_ms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 06:00:31.000000 depthcharge_ms-0.4.6/depthcharge_ms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-08 06:00:31.000000 depthcharge_ms-0.4.6/depthcharge_ms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-08 06:00:31.000000 depthcharge_ms-0.4.6/depthcharge_ms.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:00:31.300104 depthcharge_ms-0.4.6/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     5653 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/docs/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     4973 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/docs/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     3921 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/docs/CONTRIBUTING.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:00:31.300104 depthcharge_ms-0.4.6/docs/api/
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/docs/api/datasets.md
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/docs/api/encoders.md
--rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/docs/api/index.md
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/docs/api/primitives.md
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/docs/api/tokenizers.md
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/docs/api/transformers.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:00:31.300104 depthcharge_ms-0.4.6/docs/getting-started/
--rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/docs/getting-started/installation.md
--rw-r--r--   0 runner    (1001) docker     (127)    10048 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/docs/getting-started/spectra.qmd
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:00:31.300104 depthcharge_ms-0.4.6/docs/stylesheets/
--rw-r--r--   0 runner    (1001) docker     (127)     3353 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/docs/stylesheets/extra.css
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 06:00:31.304104 depthcharge_ms-0.4.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:00:31.300104 depthcharge_ms-0.4.6/static/
--rw-r--r--   0 runner    (1001) docker     (127)    15364 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/static/icon.svg
--rw-r--r--   0 runner    (1001) docker     (127)    50058 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/static/logo-dark.png
--rw-r--r--   0 runner    (1001) docker     (127)    46385 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/static/logo-light.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:00:31.300104 depthcharge_ms-0.4.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3757 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:00:31.300104 depthcharge_ms-0.4.6/tests/unit_tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:00:31.304104 depthcharge_ms-0.4.6/tests/unit_tests/test_data/
--rw-r--r--   0 runner    (1001) docker     (127)     3284 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/tests/unit_tests/test_data/test_arrow.py
--rw-r--r--   0 runner    (1001) docker     (127)     6367 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/tests/unit_tests/test_data/test_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/tests/unit_tests/test_data/test_loaders.py
--rw-r--r--   0 runner    (1001) docker     (127)     5886 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/tests/unit_tests/test_data/test_parsers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:00:31.304104 depthcharge_ms-0.4.6/tests/unit_tests/test_encoders/
--rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/tests/unit_tests/test_encoders/test_sinusoidal.py
--rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/tests/unit_tests/test_feedforward.py
--rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/tests/unit_tests/test_primitives.py
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/tests/unit_tests/test_testing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:00:31.304104 depthcharge_ms-0.4.6/tests/unit_tests/test_tokenizers/
--rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/tests/unit_tests/test_tokenizers/test_molecules.py
--rw-r--r--   0 runner    (1001) docker     (127)     3458 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/tests/unit_tests/test_tokenizers/test_peptides.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:00:31.304104 depthcharge_ms-0.4.6/tests/unit_tests/test_transformers/
--rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/tests/unit_tests/test_transformers/test_analyte_transformers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/tests/unit_tests/test_transformers/test_spectrum_transformers.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-08 06:00:19.000000 depthcharge_ms-0.4.6/tests/unit_tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:20:21.747132 depthcharge_ms-0.4.7/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:20:21.731132 depthcharge_ms-0.4.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:20:21.735132 depthcharge_ms-0.4.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-05-09 23:20:09.000000 depthcharge_ms-0.4.7/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-05-09 23:20:09.000000 depthcharge_ms-0.4.7/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-05-09 23:20:09.000000 depthcharge_ms-0.4.7/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-09 23:20:09.000000 depthcharge_ms-0.4.7/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-09 23:20:09.000000 depthcharge_ms-0.4.7/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5847 2024-05-09 23:20:09.000000 depthcharge_ms-0.4.7/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4973 2024-05-09 23:20:09.000000 depthcharge_ms-0.4.7/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3921 2024-05-09 23:20:09.000000 depthcharge_ms-0.4.7/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-09 23:20:09.000000 depthcharge_ms-0.4.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-09 23:20:21.747132 depthcharge_ms-0.4.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-05-09 23:20:09.000000 depthcharge_ms-0.4.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-09 23:20:09.000000 depthcharge_ms-0.4.7/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:20:21.735132 depthcharge_ms-0.4.7/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-09 23:20:09.000000 depthcharge_ms-0.4.7/data/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    12882 2024-05-09 23:20:09.000000 depthcharge_ms-0.4.7/data/TMT10-Trial-8.mgf
+-rw-r--r--   0 runner    (1001) docker     (127)   333839 2024-05-09 23:20:09.000000 depthcharge_ms-0.4.7/data/TMT10-Trial-8.mzML
+-rw-r--r--   0 runner    (1001) docker     (127)    67798 2024-05-09 23:20:09.000000 depthcharge_ms-0.4.7/data/TMT10-Trial-8.mzXML
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:20:21.739132 depthcharge_ms-0.4.7/depthcharge/
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-09 23:20:09.000000 depthcharge_ms-0.4.7/depthcharge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-09 23:20:09.000000 depthcharge_ms-0.4.7/depthcharge/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:20:21.739132 depthcharge_ms-0.4.7/depthcharge/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-09 23:20:09.000000 depthcharge_ms-0.4.7/depthcharge/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-05-09 23:20:09.000000 depthcharge_ms-0.4.7/depthcharge/data/analyte_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12035 2024-05-09 23:20:09.000000 depthcharge_ms-0.4.7/depthcharge/data/arrow.py
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-05-09 23:20:09.000000 depthcharge_ms-0.4.7/depthcharge/data/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18146 2024-05-09 23:20:09.000000 depthcharge_ms-0.4.7/depthcharge/data/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-05-09 23:20:09.000000 depthcharge_ms-0.4.7/depthcharge/data/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18791 2024-05-09 23:20:09.000000 depthcharge_ms-0.4.7/depthcharge/data/spectrum_datasets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:20:21.739132 depthcharge_ms-0.4.7/depthcharge/encoders/
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-09 23:20:09.000000 depthcharge_ms-0.4.7/depthcharge/encoders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6969 2024-05-09 23:20:09.000000 depthcharge_ms-0.4.7/depthcharge/encoders/sinusoidal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-05-09 23:20:09.000000 depthcharge_ms-0.4.7/depthcharge/feedforward.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-05-09 23:20:09.000000 depthcharge_ms-0.4.7/depthcharge/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12905 2024-05-09 23:20:09.000000 depthcharge_ms-0.4.7/depthcharge/primitives.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-05-09 23:20:09.000000 depthcharge_ms-0.4.7/depthcharge/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:20:21.739132 depthcharge_ms-0.4.7/depthcharge/tokenizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-09 23:20:09.000000 depthcharge_ms-0.4.7/depthcharge/tokenizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3996 2024-05-09 23:20:09.000000 depthcharge_ms-0.4.7/depthcharge/tokenizers/molecules.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11192 2024-05-09 23:20:09.000000 depthcharge_ms-0.4.7/depthcharge/tokenizers/peptides.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4948 2024-05-09 23:20:09.000000 depthcharge_ms-0.4.7/depthcharge/tokenizers/tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:20:21.739132 depthcharge_ms-0.4.7/depthcharge/transformers/
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-09 23:20:09.000000 depthcharge_ms-0.4.7/depthcharge/transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17251 2024-05-09 23:20:09.000000 depthcharge_ms-0.4.7/depthcharge/transformers/analytes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6812 2024-05-09 23:20:09.000000 depthcharge_ms-0.4.7/depthcharge/transformers/spectra.py
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-05-09 23:20:09.000000 depthcharge_ms-0.4.7/depthcharge/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-09 23:20:09.000000 depthcharge_ms-0.4.7/depthcharge/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:20:21.747132 depthcharge_ms-0.4.7/depthcharge_ms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-09 23:20:21.000000 depthcharge_ms-0.4.7/depthcharge_ms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-05-09 23:20:21.000000 depthcharge_ms-0.4.7/depthcharge_ms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 23:20:21.000000 depthcharge_ms-0.4.7/depthcharge_ms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-09 23:20:21.000000 depthcharge_ms-0.4.7/depthcharge_ms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-09 23:20:21.000000 depthcharge_ms-0.4.7/depthcharge_ms.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:20:21.743132 depthcharge_ms-0.4.7/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     5847 2024-05-09 23:20:09.000000 depthcharge_ms-0.4.7/docs/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4973 2024-05-09 23:20:09.000000 depthcharge_ms-0.4.7/docs/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3921 2024-05-09 23:20:09.000000 depthcharge_ms-0.4.7/docs/CONTRIBUTING.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:20:21.743132 depthcharge_ms-0.4.7/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-09 23:20:09.000000 depthcharge_ms-0.4.7/docs/api/datasets.md
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-09 23:20:09.000000 depthcharge_ms-0.4.7/docs/api/encoders.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-05-09 23:20:09.000000 depthcharge_ms-0.4.7/docs/api/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-09 23:20:09.000000 depthcharge_ms-0.4.7/docs/api/primitives.md
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-09 23:20:09.000000 depthcharge_ms-0.4.7/docs/api/tokenizers.md
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-09 23:20:09.000000 depthcharge_ms-0.4.7/docs/api/transformers.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:20:21.743132 depthcharge_ms-0.4.7/docs/getting-started/
+-rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-05-09 23:20:09.000000 depthcharge_ms-0.4.7/docs/getting-started/installation.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10048 2024-05-09 23:20:09.000000 depthcharge_ms-0.4.7/docs/getting-started/spectra.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-09 23:20:09.000000 depthcharge_ms-0.4.7/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:20:21.743132 depthcharge_ms-0.4.7/docs/stylesheets/
+-rw-r--r--   0 runner    (1001) docker     (127)     3353 2024-05-09 23:20:09.000000 depthcharge_ms-0.4.7/docs/stylesheets/extra.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-05-09 23:20:09.000000 depthcharge_ms-0.4.7/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-05-09 23:20:09.000000 depthcharge_ms-0.4.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 23:20:21.747132 depthcharge_ms-0.4.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:20:21.743132 depthcharge_ms-0.4.7/static/
+-rw-r--r--   0 runner    (1001) docker     (127)    15364 2024-05-09 23:20:09.000000 depthcharge_ms-0.4.7/static/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    50058 2024-05-09 23:20:09.000000 depthcharge_ms-0.4.7/static/logo-dark.png
+-rw-r--r--   0 runner    (1001) docker     (127)    46385 2024-05-09 23:20:09.000000 depthcharge_ms-0.4.7/static/logo-light.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:20:21.743132 depthcharge_ms-0.4.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3757 2024-05-09 23:20:09.000000 depthcharge_ms-0.4.7/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:20:21.747132 depthcharge_ms-0.4.7/tests/unit_tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:20:21.747132 depthcharge_ms-0.4.7/tests/unit_tests/test_data/
+-rw-r--r--   0 runner    (1001) docker     (127)     3284 2024-05-09 23:20:09.000000 depthcharge_ms-0.4.7/tests/unit_tests/test_data/test_arrow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6483 2024-05-09 23:20:09.000000 depthcharge_ms-0.4.7/tests/unit_tests/test_data/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-05-09 23:20:09.000000 depthcharge_ms-0.4.7/tests/unit_tests/test_data/test_loaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5886 2024-05-09 23:20:09.000000 depthcharge_ms-0.4.7/tests/unit_tests/test_data/test_parsers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:20:21.747132 depthcharge_ms-0.4.7/tests/unit_tests/test_encoders/
+-rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-05-09 23:20:09.000000 depthcharge_ms-0.4.7/tests/unit_tests/test_encoders/test_sinusoidal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-05-09 23:20:09.000000 depthcharge_ms-0.4.7/tests/unit_tests/test_feedforward.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-05-09 23:20:09.000000 depthcharge_ms-0.4.7/tests/unit_tests/test_primitives.py
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-05-09 23:20:09.000000 depthcharge_ms-0.4.7/tests/unit_tests/test_testing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:20:21.747132 depthcharge_ms-0.4.7/tests/unit_tests/test_tokenizers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-05-09 23:20:09.000000 depthcharge_ms-0.4.7/tests/unit_tests/test_tokenizers/test_molecules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3458 2024-05-09 23:20:09.000000 depthcharge_ms-0.4.7/tests/unit_tests/test_tokenizers/test_peptides.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:20:21.747132 depthcharge_ms-0.4.7/tests/unit_tests/test_transformers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-05-09 23:20:09.000000 depthcharge_ms-0.4.7/tests/unit_tests/test_transformers/test_analyte_transformers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-05-09 23:20:09.000000 depthcharge_ms-0.4.7/tests/unit_tests/test_transformers/test_spectrum_transformers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-09 23:20:09.000000 depthcharge_ms-0.4.7/tests/unit_tests/test_version.py
```

### Comparing `depthcharge_ms-0.4.6/.github/workflows/docs.yml` & `depthcharge_ms-0.4.7/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.6/.github/workflows/lint.yml` & `depthcharge_ms-0.4.7/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.6/.github/workflows/publish.yml` & `depthcharge_ms-0.4.7/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.6/.github/workflows/tests.yml` & `depthcharge_ms-0.4.7/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.6/CHANGELOG.md` & `depthcharge_ms-0.4.7/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 # Changelog for Depthcharge
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
+## [v0.4.7]
+### Fixed
+- Add stop and start tokens for `AnnotatedSpectrumDataset`, when available.
+- When `reverse` is used for the `PeptideTokenizer`, automatically reverse the decoded peptide.
 
 ## [v0.4.6]
 ### Added
 - Added support for unsigned modification masses that don't quite conform to the Proforma standard.
 
 ## [v0.4.5]
 ### Changed
```

### Comparing `depthcharge_ms-0.4.6/CODE_OF_CONDUCT.md` & `depthcharge_ms-0.4.7/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.6/CONTRIBUTING.md` & `depthcharge_ms-0.4.7/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.6/LICENSE` & `depthcharge_ms-0.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.6/PKG-INFO` & `depthcharge_ms-0.4.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: depthcharge-ms
-Version: 0.4.6
+Version: 0.4.7
 Summary: A mass spectrometry toolkit for deep learning with Transformer models.
 Author-email: "William E. Fondrie" <fondriew@gmail.com>
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/wfondrie/depthcharge
 Project-URL: Documentation, https://wfondrie.github.io/depthcharge
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `depthcharge_ms-0.4.6/README.md` & `depthcharge_ms-0.4.7/README.md`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.6/data/TMT10-Trial-8.mgf` & `depthcharge_ms-0.4.7/data/TMT10-Trial-8.mgf`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.6/data/TMT10-Trial-8.mzML` & `depthcharge_ms-0.4.7/data/TMT10-Trial-8.mzML`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.6/data/TMT10-Trial-8.mzXML` & `depthcharge_ms-0.4.7/data/TMT10-Trial-8.mzXML`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.6/depthcharge/__init__.py` & `depthcharge_ms-0.4.7/depthcharge/__init__.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.6/depthcharge/data/analyte_datasets.py` & `depthcharge_ms-0.4.7/depthcharge/data/analyte_datasets.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.6/depthcharge/data/arrow.py` & `depthcharge_ms-0.4.7/depthcharge/data/arrow.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.6/depthcharge/data/fields.py` & `depthcharge_ms-0.4.7/depthcharge/data/fields.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.6/depthcharge/data/parsers.py` & `depthcharge_ms-0.4.7/depthcharge/data/parsers.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.6/depthcharge/data/preprocessing.py` & `depthcharge_ms-0.4.7/depthcharge/data/preprocessing.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.6/depthcharge/data/spectrum_datasets.py` & `depthcharge_ms-0.4.7/depthcharge/data/spectrum_datasets.py`

 * *Files 2% similar despite different names*

```diff
@@ -363,15 +363,17 @@
         -------
         dict of str to tensors or lists
             The batch of data as a Python dict.
 
         """
         batch = super()._to_tensor(batch)
         batch[self.annotations] = self.tokenizer.tokenize(
-            batch[self.annotations]
+            batch[self.annotations],
+            add_start=self.tokenizer.start_token is not None,
+            add_stop=self.tokenizer.stop_token is not None,
         )
         return batch
 
     @classmethod
     def from_lance(
         cls,
         path: PathLike,
```

### Comparing `depthcharge_ms-0.4.6/depthcharge/encoders/sinusoidal.py` & `depthcharge_ms-0.4.7/depthcharge/encoders/sinusoidal.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.6/depthcharge/feedforward.py` & `depthcharge_ms-0.4.7/depthcharge/feedforward.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.6/depthcharge/mixins.py` & `depthcharge_ms-0.4.7/depthcharge/mixins.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.6/depthcharge/primitives.py` & `depthcharge_ms-0.4.7/depthcharge/primitives.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.6/depthcharge/testing.py` & `depthcharge_ms-0.4.7/depthcharge/testing.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.6/depthcharge/tokenizers/molecules.py` & `depthcharge_ms-0.4.7/depthcharge/tokenizers/molecules.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.6/depthcharge/tokenizers/peptides.py` & `depthcharge_ms-0.4.7/depthcharge/tokenizers/peptides.py`

 * *Files 4% similar despite different names*

```diff
@@ -160,20 +160,58 @@
 
         pep = pep.split()
         if self.reverse:
             pep.reverse()
 
         return pep
 
+    def detokenize(
+        self,
+        tokens: torch.Tensor,
+        join: bool = True,
+        trim_start_token: bool = True,
+        trim_stop_token: bool = True,
+    ) -> list[str] | list[list[str]]:
+        """Retreive sequences from tokens.
+
+        Parameters
+        ----------
+        tokens : torch.Tensor of shape (n_sequences, max_length)
+            The zero-padded tensor of integerized tokens to decode.
+        join : bool, optional
+            Join tokens into strings?
+        trim_start_token : bool, optional
+            Remove the start token from the beginning of a sequence.
+        trim_stop_token : bool, optional
+            Remove the stop token from the end of a sequence.
+
+        Returns
+        -------
+        list[str] or list[list[str]]
+            The decoded sequences each as a string or list or strings.
+
+        """
+        decoded = super().detokenize(
+            tokens=tokens,
+            join=join,
+            trim_start_token=trim_start_token,
+            trim_stop_token=trim_start_token,
+        )
+
+        if self.reverse:
+            decoded = [d[::-1] for d in decoded]
+
+        return decoded
+
     @classmethod
     def from_proforma(
         cls,
         sequences: Iterable[str],
         replace_isoleucine_with_leucine: bool = False,
-        reverse: bool = True,
+        reverse: bool = False,
         start_token: str | None = None,
         stop_token: str | None = "$",
     ) -> PeptideTokenizer:
         """Create a tokenizer with the observed peptide modications.
 
         Modifications are parsed from ProForma 2.0-compliant peptide strings
         and added to the vocabulary.
@@ -234,15 +272,15 @@
             start_token,
             stop_token,
         )
 
     @staticmethod
     def from_massivekb(
         replace_isoleucine_with_leucine: bool = False,
-        reverse: bool = True,
+        reverse: bool = False,
         start_token: str | None = None,
         stop_token: str | None = "$",
     ) -> MskbPeptideTokenizer:
         """Create a tokenizer with the observed peptide modications.
 
         Modifications are parsed from MassIVE-KB peptide strings
         and added to the vocabulary.
```

### Comparing `depthcharge_ms-0.4.6/depthcharge/tokenizers/tokenizer.py` & `depthcharge_ms-0.4.7/depthcharge/tokenizers/tokenizer.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.6/depthcharge/transformers/analytes.py` & `depthcharge_ms-0.4.7/depthcharge/transformers/analytes.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.6/depthcharge/transformers/spectra.py` & `depthcharge_ms-0.4.7/depthcharge/transformers/spectra.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.6/depthcharge/utils.py` & `depthcharge_ms-0.4.7/depthcharge/utils.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.6/depthcharge_ms.egg-info/PKG-INFO` & `depthcharge_ms-0.4.7/depthcharge_ms.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: depthcharge-ms
-Version: 0.4.6
+Version: 0.4.7
 Summary: A mass spectrometry toolkit for deep learning with Transformer models.
 Author-email: "William E. Fondrie" <fondriew@gmail.com>
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/wfondrie/depthcharge
 Project-URL: Documentation, https://wfondrie.github.io/depthcharge
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `depthcharge_ms-0.4.6/depthcharge_ms.egg-info/SOURCES.txt` & `depthcharge_ms-0.4.7/depthcharge_ms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.6/docs/CHANGELOG.md` & `depthcharge_ms-0.4.7/docs/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 # Changelog for Depthcharge
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
+## [v0.4.7]
+### Fixed
+- Add stop and start tokens for `AnnotatedSpectrumDataset`, when available.
+- When `reverse` is used for the `PeptideTokenizer`, automatically reverse the decoded peptide.
 
 ## [v0.4.6]
 ### Added
 - Added support for unsigned modification masses that don't quite conform to the Proforma standard.
 
 ## [v0.4.5]
 ### Changed
```

### Comparing `depthcharge_ms-0.4.6/docs/CODE_OF_CONDUCT.md` & `depthcharge_ms-0.4.7/docs/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.6/docs/CONTRIBUTING.md` & `depthcharge_ms-0.4.7/docs/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.6/docs/api/index.md` & `depthcharge_ms-0.4.7/docs/api/index.md`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.6/docs/getting-started/installation.md` & `depthcharge_ms-0.4.7/docs/getting-started/installation.md`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.6/docs/getting-started/spectra.qmd` & `depthcharge_ms-0.4.7/docs/getting-started/spectra.qmd`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.6/docs/index.md` & `depthcharge_ms-0.4.7/docs/index.md`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.6/docs/stylesheets/extra.css` & `depthcharge_ms-0.4.7/docs/stylesheets/extra.css`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.6/mkdocs.yml` & `depthcharge_ms-0.4.7/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.6/pyproject.toml` & `depthcharge_ms-0.4.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.6/static/icon.svg` & `depthcharge_ms-0.4.7/static/icon.svg`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.6/static/logo-dark.png` & `depthcharge_ms-0.4.7/static/logo-dark.png`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.6/static/logo-light.png` & `depthcharge_ms-0.4.7/static/logo-light.png`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.6/tests/conftest.py` & `depthcharge_ms-0.4.7/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.6/tests/unit_tests/test_data/test_arrow.py` & `depthcharge_ms-0.4.7/tests/unit_tests/test_data/test_arrow.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.6/tests/unit_tests/test_data/test_datasets.py` & `depthcharge_ms-0.4.7/tests/unit_tests/test_data/test_datasets.py`

 * *Files 24% similar despite different names*

```diff
@@ -69,22 +69,26 @@
     )
     spec = dataset[0]
     assert len(spec) == 8
     assert spec["mz_array"].shape == (
         1,
         14,
     )
-    torch.testing.assert_close(spec["seq"], tokenizer.tokenize(["LESLIEK"]))
+    torch.testing.assert_close(
+        spec["seq"], tokenizer.tokenize(["LESLIEK"], add_stop=True)
+    )
 
     spec2 = dataset[3]
     assert spec2["mz_array"].shape == (
         1,
         24,
     )
-    torch.testing.assert_close(spec2["seq"], tokenizer.tokenize(["EDITHR"]))
+    torch.testing.assert_close(
+        spec2["seq"], tokenizer.tokenize(["EDITHR"], add_stop=True)
+    )
 
 
 def test_load(tokenizer, tmp_path, mgf_small):
     """Test saving and loading a dataset."""
     db_path = tmp_path / "test.lance"
 
     AnnotatedSpectrumDataset(
@@ -102,19 +106,23 @@
     )
 
     dataset = AnnotatedSpectrumDataset.from_lance(db_path, "seq", tokenizer, 1)
 
     spec = dataset[0]
     assert len(spec) == 8
     assert spec["mz_array"].shape == (1, 14)
-    torch.testing.assert_close(spec["seq"], tokenizer.tokenize(["LESLIEK"]))
+    torch.testing.assert_close(
+        spec["seq"], tokenizer.tokenize(["LESLIEK"], add_stop=True)
+    )
 
     spec2 = dataset[1]
     assert spec2["mz_array"].shape == (1, 24)
-    torch.testing.assert_close(spec2["seq"], tokenizer.tokenize(["EDITHR"]))
+    torch.testing.assert_close(
+        spec2["seq"], tokenizer.tokenize(["EDITHR"], add_stop=True)
+    )
 
     dataset = SpectrumDataset.from_lance(db_path, 1)
     spec = dataset[0]
     assert len(spec) == 8
     assert spec["peak_file"] == ["small.mgf"]
     assert spec["scan_id"] == ["0"]
     assert spec["ms_level"] == 2
```

### Comparing `depthcharge_ms-0.4.6/tests/unit_tests/test_data/test_loaders.py` & `depthcharge_ms-0.4.7/tests/unit_tests/test_data/test_loaders.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,15 +70,15 @@
     loader = DataLoader(dset, num_workers=0)
     batch = next(iter(loader))
     assert len(batch) == 8
     assert batch["mz_array"].shape == (1, 1, 13)
     assert isinstance(batch["mz_array"], torch.Tensor)
     torch.testing.assert_close(
         batch["seq"][0, ...],
-        tokenizer.tokenize(["LESLIEK"]),
+        tokenizer.tokenize(["LESLIEK"], add_stop=True),
     )
 
 
 def test_analyte_loader():
     """Test our peptid data loader."""
     seqs = ["LESLIE", "EDITH", "PEPTIDE"]
     charges = torch.tensor([5, 3, 1])
```

### Comparing `depthcharge_ms-0.4.6/tests/unit_tests/test_data/test_parsers.py` & `depthcharge_ms-0.4.7/tests/unit_tests/test_data/test_parsers.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.6/tests/unit_tests/test_encoders/test_sinusoidal.py` & `depthcharge_ms-0.4.7/tests/unit_tests/test_encoders/test_sinusoidal.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.6/tests/unit_tests/test_feedforward.py` & `depthcharge_ms-0.4.7/tests/unit_tests/test_feedforward.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.6/tests/unit_tests/test_primitives.py` & `depthcharge_ms-0.4.7/tests/unit_tests/test_primitives.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.6/tests/unit_tests/test_testing.py` & `depthcharge_ms-0.4.7/tests/unit_tests/test_testing.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.6/tests/unit_tests/test_tokenizers/test_molecules.py` & `depthcharge_ms-0.4.7/tests/unit_tests/test_tokenizers/test_molecules.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.6/tests/unit_tests/test_tokenizers/test_peptides.py` & `depthcharge_ms-0.4.7/tests/unit_tests/test_tokenizers/test_peptides.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,15 +58,15 @@
         replace_isoleucine_with_leucine=False,
         reverse=True,
     )
     tokens = proforma.tokenize(["LESLIEK"], to_strings=True)[0]
     assert tokens == list("KEILSEL")
     tokens = proforma.tokenize(["LESLIEK"])
     orig = proforma.detokenize(tokens)
-    assert orig == ["KEILSEL"]
+    assert orig == ["LESLIEK"]
 
     tokens = proforma.tokenize("LESLIEK", True, True, True)[0]
     assert "".join(tokens) == "KEILSEL$"
 
     # Test a non-canonical AA:
     with pytest.raises(KeyError):
         PeptideTokenizer.from_proforma("TOBIN")
```

### Comparing `depthcharge_ms-0.4.6/tests/unit_tests/test_transformers/test_analyte_transformers.py` & `depthcharge_ms-0.4.7/tests/unit_tests/test_transformers/test_analyte_transformers.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.6/tests/unit_tests/test_transformers/test_spectrum_transformers.py` & `depthcharge_ms-0.4.7/tests/unit_tests/test_transformers/test_spectrum_transformers.py`

 * *Files identical despite different names*

### Comparing `depthcharge_ms-0.4.6/tests/unit_tests/test_version.py` & `depthcharge_ms-0.4.7/tests/unit_tests/test_version.py`

 * *Files identical despite different names*

