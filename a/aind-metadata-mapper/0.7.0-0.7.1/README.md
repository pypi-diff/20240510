# Comparing `tmp/aind_metadata_mapper-0.7.0.tar.gz` & `tmp/aind_metadata_mapper-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aind_metadata_mapper-0.7.0.tar", last modified: Sun May  5 21:04:15 2024, max compression
+gzip compressed data, was "aind_metadata_mapper-0.7.1.tar", last modified: Fri May 10 17:50:05 2024, max compression
```

## Comparing `aind_metadata_mapper-0.7.0.tar` & `aind_metadata_mapper-0.7.1.tar`

### file list

```diff
@@ -1,122 +1,121 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:04:15.985203 aind_metadata_mapper-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:04:15.961203 aind_metadata_mapper-0.7.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:04:15.969203 aind_metadata_mapper-0.7.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/.github/ISSUE_TEMPLATE/user-story.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:04:15.969203 aind_metadata_mapper-0.7.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/.github/workflows/tag_and_publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/.github/workflows/test_and_lint.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5492 2024-05-05 21:04:15.985203 aind_metadata_mapper-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4651 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:04:15.969203 aind_metadata_mapper-0.7.0/doc_template/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/doc_template/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/doc_template/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:04:15.969203 aind_metadata_mapper-0.7.0/doc_template/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:04:15.969203 aind_metadata_mapper-0.7.0/doc_template/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     8733 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/doc_template/source/_static/dark-logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)   259838 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/doc_template/source/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)     8712 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/doc_template/source/_static/light-logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/doc_template/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/doc_template/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:04:15.969203 aind_metadata_mapper-0.7.0/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     2642 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/examples/bergamo_session.py
--rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:04:15.969203 aind_metadata_mapper-0.7.0/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/scripts/singularity_build.def
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 21:04:15.985203 aind_metadata_mapper-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:04:15.965203 aind_metadata_mapper-0.7.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:04:15.969203 aind_metadata_mapper-0.7.0/src/aind_metadata_mapper/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/src/aind_metadata_mapper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:04:15.969203 aind_metadata_mapper-0.7.0/src/aind_metadata_mapper/bergamo/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/src/aind_metadata_mapper/bergamo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23421 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/src/aind_metadata_mapper/bergamo/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     7788 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/src/aind_metadata_mapper/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:04:15.973203 aind_metadata_mapper-0.7.0/src/aind_metadata_mapper/ephys/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/src/aind_metadata_mapper/ephys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5272 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/src/aind_metadata_mapper/ephys/session.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:04:15.973203 aind_metadata_mapper-0.7.0/src/aind_metadata_mapper/fib/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/src/aind_metadata_mapper/fib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8268 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/src/aind_metadata_mapper/fib/session.py
--rw-r--r--   0 runner    (1001) docker     (127)    12051 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/src/aind_metadata_mapper/gather_metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:04:15.973203 aind_metadata_mapper-0.7.0/src/aind_metadata_mapper/mesoscope/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/src/aind_metadata_mapper/mesoscope/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10357 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/src/aind_metadata_mapper/mesoscope/session.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:04:15.973203 aind_metadata_mapper-0.7.0/src/aind_metadata_mapper/neuropixels/
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/src/aind_metadata_mapper/neuropixels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2759 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/src/aind_metadata_mapper/neuropixels/mvr_rig.py
--rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/src/aind_metadata_mapper/neuropixels/neuropixels_rig.py
--rw-r--r--   0 runner    (1001) docker     (127)     5670 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/src/aind_metadata_mapper/neuropixels/open_ephys_rig.py
--rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/src/aind_metadata_mapper/neuropixels/sync_rig.py
--rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/src/aind_metadata_mapper/neuropixels/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:04:15.981203 aind_metadata_mapper-0.7.0/src/aind_metadata_mapper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5492 2024-05-05 21:04:15.000000 aind_metadata_mapper-0.7.0/src/aind_metadata_mapper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3945 2024-05-05 21:04:15.000000 aind_metadata_mapper-0.7.0/src/aind_metadata_mapper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 21:04:15.000000 aind_metadata_mapper-0.7.0/src/aind_metadata_mapper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-05 21:04:15.000000 aind_metadata_mapper-0.7.0/src/aind_metadata_mapper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-05 21:04:15.000000 aind_metadata_mapper-0.7.0/src/aind_metadata_mapper.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:04:15.973203 aind_metadata_mapper-0.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:04:15.965203 aind_metadata_mapper-0.7.0/tests/resources/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:04:15.973203 aind_metadata_mapper-0.7.0/tests/resources/bergamo/
--rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/tests/resources/bergamo/cropped_neuron50_00001.tif
--rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/tests/resources/bergamo/example_description0.txt
--rw-r--r--   0 runner    (1001) docker     (127)    76696 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/tests/resources/bergamo/example_metadata.txt.gz
--rw-r--r--   0 runner    (1001) docker     (127)     5875 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/tests/resources/bergamo/expected_session.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:04:15.977203 aind_metadata_mapper-0.7.0/tests/resources/ephys/
--rw-r--r--   0 runner    (1001) docker     (127)    11653 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/tests/resources/ephys/ephys_session.json
--rw-r--r--   0 runner    (1001) docker     (127)     8504 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/tests/resources/ephys/newscale_main.csv
--rw-r--r--   0 runner    (1001) docker     (127)     8504 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/tests/resources/ephys/newscale_surface_finding.csv
--rw-r--r--   0 runner    (1001) docker     (127)    53714 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/tests/resources/ephys/settings_main.xml
--rw-r--r--   0 runner    (1001) docker     (127)    53714 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/tests/resources/ephys/settings_surface_finding.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:04:15.977203 aind_metadata_mapper-0.7.0/tests/resources/fib/
--rw-r--r--   0 runner    (1001) docker     (127)    15663 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/tests/resources/fib/000000_ophys_rig.json
--rw-r--r--   0 runner    (1001) docker     (127)     4597 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/tests/resources/fib/000000_ophys_session.json
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/tests/resources/fib/example_from_teensy.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:04:15.977203 aind_metadata_mapper-0.7.0/tests/resources/gather_metadata_job/
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/tests/resources/gather_metadata_job/example_funding_multiple_response.json
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/tests/resources/gather_metadata_job/example_funding_response.json
--rw-r--r--   0 runner    (1001) docker     (127)     3481 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/tests/resources/gather_metadata_job/example_procedures_response.json
--rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/tests/resources/gather_metadata_job/example_subject_response.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:04:15.977203 aind_metadata_mapper-0.7.0/tests/resources/gather_metadata_job/metadata_files/
--rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/tests/resources/gather_metadata_job/metadata_files/data_description.json
--rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/tests/resources/gather_metadata_job/metadata_files/procedures.json
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/tests/resources/gather_metadata_job/metadata_files/processing.json
--rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/tests/resources/gather_metadata_job/metadata_files/subject.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:04:15.977203 aind_metadata_mapper-0.7.0/tests/resources/mesoscope/
--rw-r--r--   0 runner    (1001) docker     (127)     4168 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/tests/resources/mesoscope/0123456789_Behavior_20240212T091443.json
--rw-r--r--   0 runner    (1001) docker     (127)      991 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/tests/resources/mesoscope/0123456789_Eye_20240212T091443.json
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/tests/resources/mesoscope/0123456789_Face_20240212T091444.json
--rw-r--r--   0 runner    (1001) docker     (127)    15701 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/tests/resources/mesoscope/example_extract.json
--rw-r--r--   0 runner    (1001) docker     (127)     8002 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/tests/resources/mesoscope/example_platform.json
--rw-r--r--   0 runner    (1001) docker     (127)    12038 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/tests/resources/mesoscope/expected_session.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:04:15.981203 aind_metadata_mapper-0.7.0/tests/resources/neuropixels/
--rw-r--r--   0 runner    (1001) docker     (127)    39424 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/tests/resources/neuropixels/base-missing-probe_rig.json
--rw-r--r--   0 runner    (1001) docker     (127)    40853 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/tests/resources/neuropixels/base_rig.json
--rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/tests/resources/neuropixels/mvr.ini
--rw-r--r--   0 runner    (1001) docker     (127)    42611 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/tests/resources/neuropixels/mvr_rig.json
--rw-r--r--   0 runner    (1001) docker     (127)    42283 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/tests/resources/neuropixels/open-ephys-inferred_rig.json
--rw-r--r--   0 runner    (1001) docker     (127)    42266 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/tests/resources/neuropixels/open-ephys_rig.json
--rwxr-xr-x   0 runner    (1001) docker     (127)   136805 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/tests/resources/neuropixels/settings.mislabeled-probes-0.xml
--rwxr-xr-x   0 runner    (1001) docker     (127)   136805 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/tests/resources/neuropixels/settings.mislabeled-probes-1.xml
--rw-r--r--   0 runner    (1001) docker     (127)   132751 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/tests/resources/neuropixels/settings.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/tests/resources/neuropixels/sync.yml
--rw-r--r--   0 runner    (1001) docker     (127)    46653 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/tests/resources/neuropixels/sync_rig.json
--rw-r--r--   0 runner    (1001) docker     (127)    13902 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/tests/test_bergamo.py
--rw-r--r--   0 runner    (1001) docker     (127)     9895 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/tests/test_ephys.py
--rw-r--r--   0 runner    (1001) docker     (127)     4270 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/tests/test_fib.py
--rw-r--r--   0 runner    (1001) docker     (127)    17909 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/tests/test_gather_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     3314 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/tests/test_legacy_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     7750 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/tests/test_mesoscope.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:04:15.981203 aind_metadata_mapper-0.7.0/tests/test_neuropixels/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/tests/test_neuropixels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2796 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/tests/test_neuropixels/test_mvr_rig.py
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/tests/test_neuropixels/test_neuropixels_rig.py
--rw-r--r--   0 runner    (1001) docker     (127)     3324 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/tests/test_neuropixels/test_open_ephys_rig.py
--rw-r--r--   0 runner    (1001) docker     (127)     5123 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/tests/test_neuropixels/test_open_ephys_rig_inferrred.py
--rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/tests/test_neuropixels/test_sync_rig.py
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-05-05 21:04:06.000000 aind_metadata_mapper-0.7.0/tests/test_neuropixels/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:50:05.818958 aind_metadata_mapper-0.7.1/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-10 17:49:53.000000 aind_metadata_mapper-0.7.1/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:50:05.794958 aind_metadata_mapper-0.7.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:50:05.798958 aind_metadata_mapper-0.7.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-10 17:49:53.000000 aind_metadata_mapper-0.7.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-10 17:49:53.000000 aind_metadata_mapper-0.7.1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-10 17:49:53.000000 aind_metadata_mapper-0.7.1/.github/ISSUE_TEMPLATE/user-story.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:50:05.802958 aind_metadata_mapper-0.7.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-05-10 17:49:53.000000 aind_metadata_mapper-0.7.1/.github/workflows/tag_and_publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-10 17:49:53.000000 aind_metadata_mapper-0.7.1/.github/workflows/test_and_lint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-05-10 17:49:53.000000 aind_metadata_mapper-0.7.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-10 17:49:53.000000 aind_metadata_mapper-0.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5492 2024-05-10 17:50:05.814958 aind_metadata_mapper-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4651 2024-05-10 17:49:53.000000 aind_metadata_mapper-0.7.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:50:05.802958 aind_metadata_mapper-0.7.1/doc_template/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-10 17:49:53.000000 aind_metadata_mapper-0.7.1/doc_template/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-10 17:49:53.000000 aind_metadata_mapper-0.7.1/doc_template/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:50:05.802958 aind_metadata_mapper-0.7.1/doc_template/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:50:05.802958 aind_metadata_mapper-0.7.1/doc_template/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     8733 2024-05-10 17:49:53.000000 aind_metadata_mapper-0.7.1/doc_template/source/_static/dark-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   259838 2024-05-10 17:49:53.000000 aind_metadata_mapper-0.7.1/doc_template/source/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     8712 2024-05-10 17:49:53.000000 aind_metadata_mapper-0.7.1/doc_template/source/_static/light-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-05-10 17:49:53.000000 aind_metadata_mapper-0.7.1/doc_template/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-10 17:49:53.000000 aind_metadata_mapper-0.7.1/doc_template/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:50:05.802958 aind_metadata_mapper-0.7.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     2642 2024-05-10 17:49:53.000000 aind_metadata_mapper-0.7.1/examples/bergamo_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-05-10 17:49:53.000000 aind_metadata_mapper-0.7.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:50:05.802958 aind_metadata_mapper-0.7.1/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-10 17:49:53.000000 aind_metadata_mapper-0.7.1/scripts/singularity_build.def
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 17:50:05.818958 aind_metadata_mapper-0.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-10 17:49:53.000000 aind_metadata_mapper-0.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:50:05.798958 aind_metadata_mapper-0.7.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:50:05.802958 aind_metadata_mapper-0.7.1/src/aind_metadata_mapper/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-10 17:49:54.000000 aind_metadata_mapper-0.7.1/src/aind_metadata_mapper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:50:05.802958 aind_metadata_mapper-0.7.1/src/aind_metadata_mapper/bergamo/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-10 17:49:53.000000 aind_metadata_mapper-0.7.1/src/aind_metadata_mapper/bergamo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23421 2024-05-10 17:49:53.000000 aind_metadata_mapper-0.7.1/src/aind_metadata_mapper/bergamo/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7788 2024-05-10 17:49:53.000000 aind_metadata_mapper-0.7.1/src/aind_metadata_mapper/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:50:05.806959 aind_metadata_mapper-0.7.1/src/aind_metadata_mapper/dynamic_routing/
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-10 17:49:53.000000 aind_metadata_mapper-0.7.1/src/aind_metadata_mapper/dynamic_routing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2767 2024-05-10 17:49:53.000000 aind_metadata_mapper-0.7.1/src/aind_metadata_mapper/dynamic_routing/mvr_rig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-05-10 17:49:53.000000 aind_metadata_mapper-0.7.1/src/aind_metadata_mapper/dynamic_routing/neuropixels_rig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5440 2024-05-10 17:49:53.000000 aind_metadata_mapper-0.7.1/src/aind_metadata_mapper/dynamic_routing/open_ephys_rig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-05-10 17:49:53.000000 aind_metadata_mapper-0.7.1/src/aind_metadata_mapper/dynamic_routing/sync_rig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-05-10 17:49:53.000000 aind_metadata_mapper-0.7.1/src/aind_metadata_mapper/dynamic_routing/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:50:05.806959 aind_metadata_mapper-0.7.1/src/aind_metadata_mapper/ephys/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-10 17:49:53.000000 aind_metadata_mapper-0.7.1/src/aind_metadata_mapper/ephys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5272 2024-05-10 17:49:53.000000 aind_metadata_mapper-0.7.1/src/aind_metadata_mapper/ephys/session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:50:05.806959 aind_metadata_mapper-0.7.1/src/aind_metadata_mapper/fib/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-10 17:49:53.000000 aind_metadata_mapper-0.7.1/src/aind_metadata_mapper/fib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8268 2024-05-10 17:49:53.000000 aind_metadata_mapper-0.7.1/src/aind_metadata_mapper/fib/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12051 2024-05-10 17:49:53.000000 aind_metadata_mapper-0.7.1/src/aind_metadata_mapper/gather_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:50:05.806959 aind_metadata_mapper-0.7.1/src/aind_metadata_mapper/mesoscope/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-10 17:49:53.000000 aind_metadata_mapper-0.7.1/src/aind_metadata_mapper/mesoscope/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10357 2024-05-10 17:49:53.000000 aind_metadata_mapper-0.7.1/src/aind_metadata_mapper/mesoscope/session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:50:05.814958 aind_metadata_mapper-0.7.1/src/aind_metadata_mapper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5492 2024-05-10 17:50:05.000000 aind_metadata_mapper-0.7.1/src/aind_metadata_mapper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3937 2024-05-10 17:50:05.000000 aind_metadata_mapper-0.7.1/src/aind_metadata_mapper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 17:50:05.000000 aind_metadata_mapper-0.7.1/src/aind_metadata_mapper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-10 17:50:05.000000 aind_metadata_mapper-0.7.1/src/aind_metadata_mapper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-10 17:50:05.000000 aind_metadata_mapper-0.7.1/src/aind_metadata_mapper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:50:05.806959 aind_metadata_mapper-0.7.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-10 17:49:53.000000 aind_metadata_mapper-0.7.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:50:05.798958 aind_metadata_mapper-0.7.1/tests/resources/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:50:05.806959 aind_metadata_mapper-0.7.1/tests/resources/bergamo/
+-rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-05-10 17:49:53.000000 aind_metadata_mapper-0.7.1/tests/resources/bergamo/cropped_neuron50_00001.tif
+-rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-05-10 17:49:53.000000 aind_metadata_mapper-0.7.1/tests/resources/bergamo/example_description0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    76696 2024-05-10 17:49:53.000000 aind_metadata_mapper-0.7.1/tests/resources/bergamo/example_metadata.txt.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     5875 2024-05-10 17:49:53.000000 aind_metadata_mapper-0.7.1/tests/resources/bergamo/expected_session.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:50:05.810958 aind_metadata_mapper-0.7.1/tests/resources/ephys/
+-rw-r--r--   0 runner    (1001) docker     (127)    11653 2024-05-10 17:49:53.000000 aind_metadata_mapper-0.7.1/tests/resources/ephys/ephys_session.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8504 2024-05-10 17:49:53.000000 aind_metadata_mapper-0.7.1/tests/resources/ephys/newscale_main.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     8504 2024-05-10 17:49:53.000000 aind_metadata_mapper-0.7.1/tests/resources/ephys/newscale_surface_finding.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    53714 2024-05-10 17:49:53.000000 aind_metadata_mapper-0.7.1/tests/resources/ephys/settings_main.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    53714 2024-05-10 17:49:53.000000 aind_metadata_mapper-0.7.1/tests/resources/ephys/settings_surface_finding.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:50:05.810958 aind_metadata_mapper-0.7.1/tests/resources/fib/
+-rw-r--r--   0 runner    (1001) docker     (127)    15663 2024-05-10 17:49:53.000000 aind_metadata_mapper-0.7.1/tests/resources/fib/000000_ophys_rig.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4597 2024-05-10 17:49:53.000000 aind_metadata_mapper-0.7.1/tests/resources/fib/000000_ophys_session.json
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-10 17:49:53.000000 aind_metadata_mapper-0.7.1/tests/resources/fib/example_from_teensy.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:50:05.810958 aind_metadata_mapper-0.7.1/tests/resources/gather_metadata_job/
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-10 17:49:53.000000 aind_metadata_mapper-0.7.1/tests/resources/gather_metadata_job/example_funding_multiple_response.json
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-10 17:49:53.000000 aind_metadata_mapper-0.7.1/tests/resources/gather_metadata_job/example_funding_response.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3481 2024-05-10 17:49:53.000000 aind_metadata_mapper-0.7.1/tests/resources/gather_metadata_job/example_procedures_response.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-05-10 17:49:53.000000 aind_metadata_mapper-0.7.1/tests/resources/gather_metadata_job/example_subject_response.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:50:05.810958 aind_metadata_mapper-0.7.1/tests/resources/gather_metadata_job/metadata_files/
+-rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-05-10 17:49:53.000000 aind_metadata_mapper-0.7.1/tests/resources/gather_metadata_job/metadata_files/data_description.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-05-10 17:49:53.000000 aind_metadata_mapper-0.7.1/tests/resources/gather_metadata_job/metadata_files/procedures.json
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-05-10 17:49:53.000000 aind_metadata_mapper-0.7.1/tests/resources/gather_metadata_job/metadata_files/processing.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-05-10 17:49:53.000000 aind_metadata_mapper-0.7.1/tests/resources/gather_metadata_job/metadata_files/subject.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:50:05.810958 aind_metadata_mapper-0.7.1/tests/resources/mesoscope/
+-rw-r--r--   0 runner    (1001) docker     (127)     4168 2024-05-10 17:49:53.000000 aind_metadata_mapper-0.7.1/tests/resources/mesoscope/0123456789_Behavior_20240212T091443.json
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-05-10 17:49:53.000000 aind_metadata_mapper-0.7.1/tests/resources/mesoscope/0123456789_Eye_20240212T091443.json
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-10 17:49:53.000000 aind_metadata_mapper-0.7.1/tests/resources/mesoscope/0123456789_Face_20240212T091444.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15701 2024-05-10 17:49:53.000000 aind_metadata_mapper-0.7.1/tests/resources/mesoscope/example_extract.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8002 2024-05-10 17:49:53.000000 aind_metadata_mapper-0.7.1/tests/resources/mesoscope/example_platform.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12038 2024-05-10 17:49:53.000000 aind_metadata_mapper-0.7.1/tests/resources/mesoscope/expected_session.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:50:05.814958 aind_metadata_mapper-0.7.1/tests/resources/neuropixels/
+-rw-r--r--   0 runner    (1001) docker     (127)    39424 2024-05-10 17:49:53.000000 aind_metadata_mapper-0.7.1/tests/resources/neuropixels/base-missing-probe_rig.json
+-rw-r--r--   0 runner    (1001) docker     (127)    40853 2024-05-10 17:49:53.000000 aind_metadata_mapper-0.7.1/tests/resources/neuropixels/base_rig.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-05-10 17:49:53.000000 aind_metadata_mapper-0.7.1/tests/resources/neuropixels/mvr.ini
+-rw-r--r--   0 runner    (1001) docker     (127)    42611 2024-05-10 17:49:53.000000 aind_metadata_mapper-0.7.1/tests/resources/neuropixels/mvr_rig.json
+-rw-r--r--   0 runner    (1001) docker     (127)    42283 2024-05-10 17:49:53.000000 aind_metadata_mapper-0.7.1/tests/resources/neuropixels/open-ephys-inferred_rig.json
+-rw-r--r--   0 runner    (1001) docker     (127)    42266 2024-05-10 17:49:53.000000 aind_metadata_mapper-0.7.1/tests/resources/neuropixels/open-ephys_rig.json
+-rwxr-xr-x   0 runner    (1001) docker     (127)   136805 2024-05-10 17:49:53.000000 aind_metadata_mapper-0.7.1/tests/resources/neuropixels/settings.mislabeled-probes-0.xml
+-rwxr-xr-x   0 runner    (1001) docker     (127)   136805 2024-05-10 17:49:53.000000 aind_metadata_mapper-0.7.1/tests/resources/neuropixels/settings.mislabeled-probes-1.xml
+-rw-r--r--   0 runner    (1001) docker     (127)   132751 2024-05-10 17:49:53.000000 aind_metadata_mapper-0.7.1/tests/resources/neuropixels/settings.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-10 17:49:53.000000 aind_metadata_mapper-0.7.1/tests/resources/neuropixels/sync.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    46653 2024-05-10 17:49:53.000000 aind_metadata_mapper-0.7.1/tests/resources/neuropixels/sync_rig.json
+-rw-r--r--   0 runner    (1001) docker     (127)    13902 2024-05-10 17:49:53.000000 aind_metadata_mapper-0.7.1/tests/test_bergamo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:50:05.814958 aind_metadata_mapper-0.7.1/tests/test_dynamic_routing/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-10 17:49:53.000000 aind_metadata_mapper-0.7.1/tests/test_dynamic_routing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2877 2024-05-10 17:49:53.000000 aind_metadata_mapper-0.7.1/tests/test_dynamic_routing/test_mvr_rig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-05-10 17:49:53.000000 aind_metadata_mapper-0.7.1/tests/test_dynamic_routing/test_neuropixels_rig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7300 2024-05-10 17:49:53.000000 aind_metadata_mapper-0.7.1/tests/test_dynamic_routing/test_open_ephys_rig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-05-10 17:49:53.000000 aind_metadata_mapper-0.7.1/tests/test_dynamic_routing/test_sync_rig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-05-10 17:49:53.000000 aind_metadata_mapper-0.7.1/tests/test_dynamic_routing/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9895 2024-05-10 17:49:53.000000 aind_metadata_mapper-0.7.1/tests/test_ephys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4270 2024-05-10 17:49:53.000000 aind_metadata_mapper-0.7.1/tests/test_fib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17909 2024-05-10 17:49:53.000000 aind_metadata_mapper-0.7.1/tests/test_gather_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3314 2024-05-10 17:49:53.000000 aind_metadata_mapper-0.7.1/tests/test_legacy_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7750 2024-05-10 17:49:53.000000 aind_metadata_mapper-0.7.1/tests/test_mesoscope.py
```

### Comparing `aind_metadata_mapper-0.7.0/.github/ISSUE_TEMPLATE/bug_report.md` & `aind_metadata_mapper-0.7.1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.0/.github/ISSUE_TEMPLATE/feature_request.md` & `aind_metadata_mapper-0.7.1/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.0/.github/ISSUE_TEMPLATE/user-story.md` & `aind_metadata_mapper-0.7.1/.github/ISSUE_TEMPLATE/user-story.md`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.0/.github/workflows/tag_and_publish.yml` & `aind_metadata_mapper-0.7.1/.github/workflows/tag_and_publish.yml`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.0/.github/workflows/test_and_lint.yml` & `aind_metadata_mapper-0.7.1/.github/workflows/test_and_lint.yml`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.0/.gitignore` & `aind_metadata_mapper-0.7.1/.gitignore`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.0/LICENSE` & `aind_metadata_mapper-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.0/PKG-INFO` & `aind_metadata_mapper-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aind-metadata-mapper
-Version: 0.7.0
+Version: 0.7.1
 Summary: Generated from aind-library-template
 Author: Allen Institute for Neural Dynamics
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `aind_metadata_mapper-0.7.0/README.md` & `aind_metadata_mapper-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.0/doc_template/Makefile` & `aind_metadata_mapper-0.7.1/doc_template/Makefile`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.0/doc_template/make.bat` & `aind_metadata_mapper-0.7.1/doc_template/make.bat`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.0/doc_template/source/_static/dark-logo.svg` & `aind_metadata_mapper-0.7.1/doc_template/source/_static/dark-logo.svg`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.0/doc_template/source/_static/favicon.ico` & `aind_metadata_mapper-0.7.1/doc_template/source/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.0/doc_template/source/_static/light-logo.svg` & `aind_metadata_mapper-0.7.1/doc_template/source/_static/light-logo.svg`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.0/doc_template/source/conf.py` & `aind_metadata_mapper-0.7.1/doc_template/source/conf.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.0/examples/bergamo_session.py` & `aind_metadata_mapper-0.7.1/examples/bergamo_session.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.0/pyproject.toml` & `aind_metadata_mapper-0.7.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.0/src/aind_metadata_mapper/bergamo/session.py` & `aind_metadata_mapper-0.7.1/src/aind_metadata_mapper/bergamo/session.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.0/src/aind_metadata_mapper/core.py` & `aind_metadata_mapper-0.7.1/src/aind_metadata_mapper/core.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.0/src/aind_metadata_mapper/ephys/session.py` & `aind_metadata_mapper-0.7.1/src/aind_metadata_mapper/ephys/session.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.0/src/aind_metadata_mapper/fib/session.py` & `aind_metadata_mapper-0.7.1/src/aind_metadata_mapper/fib/session.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.0/src/aind_metadata_mapper/gather_metadata.py` & `aind_metadata_mapper-0.7.1/src/aind_metadata_mapper/gather_metadata.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.0/src/aind_metadata_mapper/mesoscope/session.py` & `aind_metadata_mapper-0.7.1/src/aind_metadata_mapper/mesoscope/session.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.0/src/aind_metadata_mapper/neuropixels/mvr_rig.py` & `aind_metadata_mapper-0.7.1/src/aind_metadata_mapper/dynamic_routing/mvr_rig.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 import logging
 from pathlib import Path
 from typing import Dict, List, Tuple
 
 from aind_data_schema.core.rig import Rig  # type: ignore
 from aind_data_schema.models.devices import Software  # type: ignore
 
-from aind_metadata_mapper.neuropixels import utils
-from aind_metadata_mapper.neuropixels.neuropixels_rig import (
+from aind_metadata_mapper.dynamic_routing import utils
+from aind_metadata_mapper.dynamic_routing.neuropixels_rig import (
     NeuropixelsRigContext,
     NeuropixelsRigEtl,
 )
 
 logger = logging.getLogger(__name__)
```

### Comparing `aind_metadata_mapper-0.7.0/src/aind_metadata_mapper/neuropixels/neuropixels_rig.py` & `aind_metadata_mapper-0.7.1/src/aind_metadata_mapper/dynamic_routing/neuropixels_rig.py`

 * *Files 15% similar despite different names*

```diff
@@ -24,37 +24,49 @@
     and transforms them into an aind-data-schema rig.Rig instance.
     """
 
     def __init__(
         self,
         input_source: Path,
         output_directory: Path,
+        modification_date: Optional[date] = None,
     ):
         """Class constructor for Neuropixels rig etl class.
 
         Parameters
         ----------
         input_source : Path
           Can be a string or a Path
         output_directory : Path
           The directory where to save the json files.
         """
         self.input_source: Path = input_source
         self.output_directory = output_directory
+        self.modification_date = modification_date
 
     def _extract(self) -> Rig:
         """Extracts rig-related information from config files."""
-        return Rig.model_validate_json(
+        extracted = Rig.model_validate_json(
             self.input_source.read_text(),
         )
+        self.initial_model = extracted.model_copy(deep=True)
+        return extracted
 
     def _transform(self, extracted_source: Rig) -> Rig:
         """Transforms extracted rig context into aind-data-schema rig.Rig
         instance.
         """
+        if self.initial_model != extracted_source:
+            logger.debug("Rig model changed. Updating modification date.")
+            self.update_modification_date(
+                extracted_source, self.modification_date
+            )
+        else:
+            logger.debug("Rig model unchanged. Keeping modification date.")
+
         return extracted_source
 
     @classmethod
     def update_modification_date(
         cls,
         extracted_source: Rig,
         modification_date: Optional[date] = None,
```

### Comparing `aind_metadata_mapper-0.7.0/src/aind_metadata_mapper/neuropixels/open_ephys_rig.py` & `aind_metadata_mapper-0.7.1/src/aind_metadata_mapper/dynamic_routing/open_ephys_rig.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 """ETL for the Open Ephys config."""
 
 import logging
-from datetime import date
 from pathlib import Path
 from typing import List, Optional, Tuple
 from xml.etree import ElementTree
 
 from aind_data_schema.core.rig import Rig  # type: ignore
 from pydantic import BaseModel
 
-from aind_metadata_mapper.neuropixels import utils
-from aind_metadata_mapper.neuropixels.neuropixels_rig import (
+from aind_metadata_mapper.dynamic_routing import utils
+from aind_metadata_mapper.dynamic_routing.neuropixels_rig import (
     NeuropixelsRigContext,
     NeuropixelsRigEtl,
 )
 
 logger = logging.getLogger(__name__)
 
 
@@ -39,24 +38,22 @@
 
     def __init__(
         self,
         input_source: Path,
         output_directory: Path,
         open_ephys_settings_sources: List[Path],
         probe_manipulator_serial_numbers: List[Tuple[str, str]] = [],
-        modification_date: Optional[date] = None,
         **kwargs,
     ):
         """Class constructor for Open Ephys rig etl class."""
         super().__init__(input_source, output_directory, **kwargs)
         self.open_ephys_settings_sources = open_ephys_settings_sources
         self.probe_manipulator_serial_numbers = (
             probe_manipulator_serial_numbers
         )
-        self.modification_date = modification_date
 
     def _extract(self) -> ExtractContext:
         """Extracts Open Ephys-related probe information from config files."""
         current = super()._extract()
         versions = []
         probes = []
         for source in self.open_ephys_settings_sources:
@@ -155,12 +152,8 @@
                     ],
                     model=probe.model,
                     serial_number=probe.serial_number,
                 )
                 if updated:
                     break
 
-        self.update_modification_date(
-            extracted_source.current, self.modification_date
-        )
-
         return super()._transform(extracted_source.current)
```

### Comparing `aind_metadata_mapper-0.7.0/src/aind_metadata_mapper/neuropixels/sync_rig.py` & `aind_metadata_mapper-0.7.1/src/aind_metadata_mapper/dynamic_routing/sync_rig.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 from pathlib import Path
 
 from aind_data_schema.core.rig import Rig  # type: ignore
 from aind_data_schema.models.devices import DAQChannel  # type: ignore
 from pydantic import BaseModel
 
-from aind_metadata_mapper.neuropixels import utils
-from aind_metadata_mapper.neuropixels.neuropixels_rig import (
+from aind_metadata_mapper.dynamic_routing import utils
+from aind_metadata_mapper.dynamic_routing.neuropixels_rig import (
     NeuropixelsRigContext,
     NeuropixelsRigEtl,
 )
 
 
 class SyncChannel(BaseModel):
     """Extracted Sync daq channel information."""
```

### Comparing `aind_metadata_mapper-0.7.0/src/aind_metadata_mapper/neuropixels/utils.py` & `aind_metadata_mapper-0.7.1/src/aind_metadata_mapper/dynamic_routing/utils.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.0/src/aind_metadata_mapper.egg-info/PKG-INFO` & `aind_metadata_mapper-0.7.1/src/aind_metadata_mapper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aind-metadata-mapper
-Version: 0.7.0
+Version: 0.7.1
 Summary: Generated from aind-library-template
 Author: Allen Institute for Neural Dynamics
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `aind_metadata_mapper-0.7.0/tests/resources/bergamo/cropped_neuron50_00001.tif` & `aind_metadata_mapper-0.7.1/tests/resources/bergamo/cropped_neuron50_00001.tif`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.0/tests/resources/bergamo/example_description0.txt` & `aind_metadata_mapper-0.7.1/tests/resources/bergamo/example_description0.txt`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.0/tests/resources/bergamo/example_metadata.txt.gz` & `aind_metadata_mapper-0.7.1/tests/resources/bergamo/example_metadata.txt.gz`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.0/tests/resources/bergamo/expected_session.json` & `aind_metadata_mapper-0.7.1/tests/resources/bergamo/expected_session.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.0/tests/resources/ephys/ephys_session.json` & `aind_metadata_mapper-0.7.1/tests/resources/ephys/ephys_session.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.0/tests/resources/ephys/newscale_main.csv` & `aind_metadata_mapper-0.7.1/tests/resources/ephys/newscale_main.csv`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.0/tests/resources/ephys/newscale_surface_finding.csv` & `aind_metadata_mapper-0.7.1/tests/resources/ephys/newscale_surface_finding.csv`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.0/tests/resources/ephys/settings_main.xml` & `aind_metadata_mapper-0.7.1/tests/resources/ephys/settings_main.xml`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.0/tests/resources/ephys/settings_surface_finding.xml` & `aind_metadata_mapper-0.7.1/tests/resources/ephys/settings_surface_finding.xml`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.0/tests/resources/fib/000000_ophys_rig.json` & `aind_metadata_mapper-0.7.1/tests/resources/fib/000000_ophys_rig.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.0/tests/resources/fib/000000_ophys_session.json` & `aind_metadata_mapper-0.7.1/tests/resources/fib/000000_ophys_session.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.0/tests/resources/gather_metadata_job/example_funding_multiple_response.json` & `aind_metadata_mapper-0.7.1/tests/resources/gather_metadata_job/example_funding_multiple_response.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.0/tests/resources/gather_metadata_job/example_procedures_response.json` & `aind_metadata_mapper-0.7.1/tests/resources/gather_metadata_job/example_procedures_response.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.0/tests/resources/gather_metadata_job/example_subject_response.json` & `aind_metadata_mapper-0.7.1/tests/resources/gather_metadata_job/example_subject_response.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.0/tests/resources/gather_metadata_job/metadata_files/data_description.json` & `aind_metadata_mapper-0.7.1/tests/resources/gather_metadata_job/metadata_files/data_description.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.0/tests/resources/gather_metadata_job/metadata_files/procedures.json` & `aind_metadata_mapper-0.7.1/tests/resources/gather_metadata_job/metadata_files/procedures.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.0/tests/resources/gather_metadata_job/metadata_files/processing.json` & `aind_metadata_mapper-0.7.1/tests/resources/gather_metadata_job/metadata_files/processing.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.0/tests/resources/gather_metadata_job/metadata_files/subject.json` & `aind_metadata_mapper-0.7.1/tests/resources/gather_metadata_job/metadata_files/subject.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.0/tests/resources/mesoscope/0123456789_Behavior_20240212T091443.json` & `aind_metadata_mapper-0.7.1/tests/resources/mesoscope/0123456789_Behavior_20240212T091443.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.0/tests/resources/mesoscope/0123456789_Eye_20240212T091443.json` & `aind_metadata_mapper-0.7.1/tests/resources/mesoscope/0123456789_Eye_20240212T091443.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.0/tests/resources/mesoscope/0123456789_Face_20240212T091444.json` & `aind_metadata_mapper-0.7.1/tests/resources/mesoscope/0123456789_Face_20240212T091444.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.0/tests/resources/mesoscope/example_extract.json` & `aind_metadata_mapper-0.7.1/tests/resources/mesoscope/example_extract.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.0/tests/resources/mesoscope/example_platform.json` & `aind_metadata_mapper-0.7.1/tests/resources/mesoscope/example_platform.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.0/tests/resources/mesoscope/expected_session.json` & `aind_metadata_mapper-0.7.1/tests/resources/mesoscope/expected_session.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.0/tests/resources/neuropixels/base-missing-probe_rig.json` & `aind_metadata_mapper-0.7.1/tests/resources/neuropixels/base-missing-probe_rig.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.0/tests/resources/neuropixels/base_rig.json` & `aind_metadata_mapper-0.7.1/tests/resources/neuropixels/base_rig.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.0/tests/resources/neuropixels/mvr.ini` & `aind_metadata_mapper-0.7.1/tests/resources/neuropixels/mvr.ini`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.0/tests/resources/neuropixels/mvr_rig.json` & `aind_metadata_mapper-0.7.1/tests/resources/neuropixels/mvr_rig.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.0/tests/resources/neuropixels/open-ephys-inferred_rig.json` & `aind_metadata_mapper-0.7.1/tests/resources/neuropixels/open-ephys-inferred_rig.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.0/tests/resources/neuropixels/open-ephys_rig.json` & `aind_metadata_mapper-0.7.1/tests/resources/neuropixels/open-ephys_rig.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.0/tests/resources/neuropixels/settings.mislabeled-probes-0.xml` & `aind_metadata_mapper-0.7.1/tests/resources/neuropixels/settings.mislabeled-probes-0.xml`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.0/tests/resources/neuropixels/settings.mislabeled-probes-1.xml` & `aind_metadata_mapper-0.7.1/tests/resources/neuropixels/settings.mislabeled-probes-1.xml`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.0/tests/resources/neuropixels/settings.xml` & `aind_metadata_mapper-0.7.1/tests/resources/neuropixels/settings.xml`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.0/tests/resources/neuropixels/sync.yml` & `aind_metadata_mapper-0.7.1/tests/resources/neuropixels/sync.yml`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.0/tests/resources/neuropixels/sync_rig.json` & `aind_metadata_mapper-0.7.1/tests/resources/neuropixels/sync_rig.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.0/tests/test_bergamo.py` & `aind_metadata_mapper-0.7.1/tests/test_bergamo.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.0/tests/test_ephys.py` & `aind_metadata_mapper-0.7.1/tests/test_ephys.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.0/tests/test_fib.py` & `aind_metadata_mapper-0.7.1/tests/test_fib.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.0/tests/test_gather_metadata.py` & `aind_metadata_mapper-0.7.1/tests/test_gather_metadata.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.0/tests/test_legacy_core.py` & `aind_metadata_mapper-0.7.1/tests/test_legacy_core.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.0/tests/test_mesoscope.py` & `aind_metadata_mapper-0.7.1/tests/test_mesoscope.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.7.0/tests/test_neuropixels/test_mvr_rig.py` & `aind_metadata_mapper-0.7.1/tests/test_dynamic_routing/test_mvr_rig.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 """Tests for the MVR rig ETL."""
 
 import os
 import unittest
 from pathlib import Path
 from unittest.mock import MagicMock, patch
 
-from aind_metadata_mapper.neuropixels.mvr_rig import MvrRigEtl  # type: ignore
-from tests.test_neuropixels import utils as test_utils
+from aind_metadata_mapper.dynamic_routing.mvr_rig import (  # type: ignore
+     MvrRigEtl,
+)
+from tests.test_dynamic_routing import utils as test_utils
 
 RESOURCES_DIR = (
     Path(os.path.dirname(os.path.realpath(__file__)))
     / ".."
     / "resources"
     / "neuropixels"
 )
@@ -26,14 +28,15 @@
             self.output_dir,
             RESOURCES_DIR / "mvr.ini",
             mvr_mapping={
                 "Camera 1": test_utils.SIDE_CAMERA_ASSEMBLY_NAME,
                 "Camera 2": test_utils.EYE_CAMERA_ASSEMBLY_NAME,
                 "Camera 3": test_utils.FORWARD_CAMERA_ASSEMBLY_NAME,
             },
+            modification_date=self.expected.modification_date,
         )
         extracted = etl._extract()
         transformed = etl._transform(extracted)
         self.assertEqual(transformed, self.expected)
 
     @patch("aind_data_schema.base.AindCoreModel.write_standard_file")
     def test_run_job(self, mock_write_standard_file: MagicMock):
```

### Comparing `aind_metadata_mapper-0.7.0/tests/test_neuropixels/test_neuropixels_rig.py` & `aind_metadata_mapper-0.7.1/tests/test_dynamic_routing/test_neuropixels_rig.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Tests for the neuropixels open ephys rig ETL with inferred probe mapping."""
 
 import os
 import unittest
 from datetime import date
 from pathlib import Path
 
-from aind_metadata_mapper.neuropixels.neuropixels_rig import (  # type: ignore
+from aind_metadata_mapper.dynamic_routing.neuropixels_rig import (
     NeuropixelsRigEtl,
 )
 
 RESOURCES_DIR = (
     Path(os.path.dirname(os.path.realpath(__file__)))
     / ".."
     / "resources"
```

### Comparing `aind_metadata_mapper-0.7.0/tests/test_neuropixels/test_sync_rig.py` & `aind_metadata_mapper-0.7.1/tests/test_dynamic_routing/test_sync_rig.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """Tests for Sync rig ETL."""
 
 import os
 import unittest
 from pathlib import Path
 from unittest.mock import MagicMock, patch
 
-from aind_metadata_mapper.neuropixels.sync_rig import (  # type: ignore
+from aind_metadata_mapper.dynamic_routing.sync_rig import (  # type: ignore
     SyncRigEtl,
 )
-from tests.test_neuropixels import utils as test_utils
+from tests.test_dynamic_routing import utils as test_utils
 
 RESOURCES_DIR = (
     Path(os.path.dirname(os.path.realpath(__file__)))
     / ".."
     / "resources"
     / "neuropixels"
 )
@@ -23,14 +23,15 @@
 
     def test_transform(self):
         """Test etl transform."""
         etl = SyncRigEtl(
             self.input_source,
             self.output_dir,
             RESOURCES_DIR / "sync.yml",
+            modification_date=self.expected.modification_date,
         )
         extracted = etl._extract()
         transformed = etl._transform(extracted)
         self.assertEqual(transformed, self.expected)
 
     @patch("aind_data_schema.base.AindCoreModel.write_standard_file")
     def test_etl(
```

### Comparing `aind_metadata_mapper-0.7.0/tests/test_neuropixels/utils.py` & `aind_metadata_mapper-0.7.1/tests/test_dynamic_routing/utils.py`

 * *Files identical despite different names*

