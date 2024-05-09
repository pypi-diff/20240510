# Comparing `tmp/perturbopy-0.5.2.tar.gz` & `tmp/perturbopy-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "perturbopy-0.5.2.tar", last modified: Wed Nov  8 21:39:53 2023, max compression
+gzip compressed data, was "perturbopy-0.5.3.tar", last modified: Thu May  9 22:31:41 2024, max compression
```

## Comparing `perturbopy-0.5.2.tar` & `perturbopy-0.5.3.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 kliavinekss   (501) staff       (20)        0 2023-11-08 21:39:53.265108 perturbopy-0.5.2/
--rw-r--r--   0 kliavinekss   (501) staff       (20)    35149 2023-07-28 19:19:00.000000 perturbopy-0.5.2/LICENSE
--rw-r--r--   0 kliavinekss   (501) staff       (20)       40 2023-08-28 19:19:24.000000 perturbopy-0.5.2/MANIFEST.in
--rw-r--r--   0 kliavinekss   (501) staff       (20)     2063 2023-11-08 21:39:53.265179 perturbopy-0.5.2/PKG-INFO
--rw-r--r--   0 kliavinekss   (501) staff       (20)     1819 2023-09-18 22:49:12.000000 perturbopy-0.5.2/README.md
--rw-r--r--   0 kliavinekss   (501) staff       (20)      132 2023-11-08 21:39:53.265416 perturbopy-0.5.2/setup.cfg
--rw-r--r--   0 kliavinekss   (501) staff       (20)      794 2023-11-08 21:37:47.000000 perturbopy-0.5.2/setup.py
-drwxr-xr-x   0 kliavinekss   (501) staff       (20)        0 2023-11-08 21:39:53.256023 perturbopy-0.5.2/src/
-drwxr-xr-x   0 kliavinekss   (501) staff       (20)        0 2023-11-08 21:39:53.258279 perturbopy-0.5.2/src/perturbopy/
--rw-r--r--   0 kliavinekss   (501) staff       (20)      108 2023-08-07 20:45:34.000000 perturbopy-0.5.2/src/perturbopy/__init__.py
--rw-r--r--   0 kliavinekss   (501) staff       (20)     8694 2023-09-20 22:13:44.000000 perturbopy-0.5.2/src/perturbopy/conftest.py
-drwxr-xr-x   0 kliavinekss   (501) staff       (20)        0 2023-11-08 21:39:53.259280 perturbopy-0.5.2/src/perturbopy/io_utils/
--rw-r--r--   0 kliavinekss   (501) staff       (20)       82 2023-07-28 19:19:00.000000 perturbopy-0.5.2/src/perturbopy/io_utils/__init__.py
--rw-r--r--   0 kliavinekss   (501) staff       (20)      707 2023-11-07 21:51:43.000000 perturbopy-0.5.2/src/perturbopy/io_utils/io.py
-drwxr-xr-x   0 kliavinekss   (501) staff       (20)        0 2023-11-08 21:39:53.259420 perturbopy-0.5.2/src/perturbopy/postproc/
--rw-r--r--   0 kliavinekss   (501) staff       (20)      522 2023-09-11 17:49:22.000000 perturbopy-0.5.2/src/perturbopy/postproc/__init__.py
-drwxr-xr-x   0 kliavinekss   (501) staff       (20)        0 2023-11-08 21:39:53.261066 perturbopy-0.5.2/src/perturbopy/postproc/calc_modes/
--rw-r--r--   0 kliavinekss   (501) staff       (20)       82 2023-07-28 19:19:00.000000 perturbopy-0.5.2/src/perturbopy/postproc/calc_modes/__init__.py
--rw-r--r--   0 kliavinekss   (501) staff       (20)     9558 2023-09-13 16:18:02.000000 perturbopy-0.5.2/src/perturbopy/postproc/calc_modes/bands.py
--rw-r--r--   0 kliavinekss   (501) staff       (20)     3797 2023-09-11 17:49:22.000000 perturbopy-0.5.2/src/perturbopy/postproc/calc_modes/calc_mode.py
--rw-r--r--   0 kliavinekss   (501) staff       (20)      838 2023-09-11 17:49:22.000000 perturbopy-0.5.2/src/perturbopy/postproc/calc_modes/dyna_indiv_run.py
--rw-r--r--   0 kliavinekss   (501) staff       (20)     3145 2023-09-19 23:50:23.000000 perturbopy-0.5.2/src/perturbopy/postproc/calc_modes/dyna_pp.py
--rw-r--r--   0 kliavinekss   (501) staff       (20)     6611 2023-11-03 23:37:15.000000 perturbopy-0.5.2/src/perturbopy/postproc/calc_modes/dyna_run.py
--rw-r--r--   0 kliavinekss   (501) staff       (20)     7224 2023-09-19 23:50:23.000000 perturbopy-0.5.2/src/perturbopy/postproc/calc_modes/ephmat.py
--rw-r--r--   0 kliavinekss   (501) staff       (20)     4569 2023-09-11 17:49:22.000000 perturbopy-0.5.2/src/perturbopy/postproc/calc_modes/imsigma.py
--rw-r--r--   0 kliavinekss   (501) staff       (20)     3021 2023-09-13 16:18:02.000000 perturbopy-0.5.2/src/perturbopy/postproc/calc_modes/phdisp.py
--rw-r--r--   0 kliavinekss   (501) staff       (20)     6248 2023-09-19 23:50:23.000000 perturbopy-0.5.2/src/perturbopy/postproc/calc_modes/trans.py
-drwxr-xr-x   0 kliavinekss   (501) staff       (20)        0 2023-11-08 21:39:53.261582 perturbopy-0.5.2/src/perturbopy/postproc/dbs/
--rw-r--r--   0 kliavinekss   (501) staff       (20)       82 2023-07-28 19:19:00.000000 perturbopy-0.5.2/src/perturbopy/postproc/dbs/__init__.py
--rw-r--r--   0 kliavinekss   (501) staff       (20)    10753 2023-09-11 17:49:22.000000 perturbopy-0.5.2/src/perturbopy/postproc/dbs/recip_pt_db.py
--rw-r--r--   0 kliavinekss   (501) staff       (20)     1406 2023-09-11 17:49:22.000000 perturbopy-0.5.2/src/perturbopy/postproc/dbs/units_dict.py
-drwxr-xr-x   0 kliavinekss   (501) staff       (20)        0 2023-11-08 21:39:53.262371 perturbopy-0.5.2/src/perturbopy/postproc/utils/
--rw-r--r--   0 kliavinekss   (501) staff       (20)       82 2023-07-28 19:19:00.000000 perturbopy-0.5.2/src/perturbopy/postproc/utils/__init__.py
--rw-r--r--   0 kliavinekss   (501) staff       (20)    10310 2023-09-11 17:49:22.000000 perturbopy-0.5.2/src/perturbopy/postproc/utils/constants.py
--rw-r--r--   0 kliavinekss   (501) staff       (20)     8155 2023-09-11 17:49:22.000000 perturbopy-0.5.2/src/perturbopy/postproc/utils/lattice.py
--rw-r--r--   0 kliavinekss   (501) staff       (20)     7736 2023-09-19 23:50:23.000000 perturbopy-0.5.2/src/perturbopy/postproc/utils/plot_tools.py
--rw-r--r--   0 kliavinekss   (501) staff       (20)     6263 2023-09-11 17:49:22.000000 perturbopy-0.5.2/src/perturbopy/postproc/utils/timing.py
--rw-r--r--   0 kliavinekss   (501) staff       (20)       14 2023-09-19 17:29:26.000000 perturbopy-0.5.2/src/perturbopy/setup.cfg
-drwxr-xr-x   0 kliavinekss   (501) staff       (20)        0 2023-11-08 21:39:53.262547 perturbopy-0.5.2/src/perturbopy/test_utils/
--rw-r--r--   0 kliavinekss   (501) staff       (20)       67 2023-07-28 19:27:33.000000 perturbopy-0.5.2/src/perturbopy/test_utils/__init__.py
-drwxr-xr-x   0 kliavinekss   (501) staff       (20)        0 2023-11-08 21:39:53.263160 perturbopy-0.5.2/src/perturbopy/test_utils/compare_data/
--rw-r--r--   0 kliavinekss   (501) staff       (20)       79 2023-07-28 19:27:33.000000 perturbopy-0.5.2/src/perturbopy/test_utils/compare_data/__init__.py
--rw-r--r--   0 kliavinekss   (501) staff       (20)     1675 2023-11-03 23:37:15.000000 perturbopy-0.5.2/src/perturbopy/test_utils/compare_data/compare.py
--rw-r--r--   0 kliavinekss   (501) staff       (20)    11891 2023-11-04 00:15:41.000000 perturbopy-0.5.2/src/perturbopy/test_utils/compare_data/h5.py
--rw-r--r--   0 kliavinekss   (501) staff       (20)     9935 2023-11-03 23:37:15.000000 perturbopy-0.5.2/src/perturbopy/test_utils/compare_data/yaml.py
-drwxr-xr-x   0 kliavinekss   (501) staff       (20)        0 2023-11-08 21:39:53.263852 perturbopy-0.5.2/src/perturbopy/test_utils/run_test/
--rw-r--r--   0 kliavinekss   (501) staff       (20)       84 2023-07-28 19:27:33.000000 perturbopy-0.5.2/src/perturbopy/test_utils/run_test/__init__.py
--rw-r--r--   0 kliavinekss   (501) staff       (20)     6611 2023-08-18 16:44:59.000000 perturbopy-0.5.2/src/perturbopy/test_utils/run_test/env_utils.py
--rw-r--r--   0 kliavinekss   (501) staff       (20)    16071 2023-11-08 21:27:08.000000 perturbopy-0.5.2/src/perturbopy/test_utils/run_test/run_utils.py
--rw-r--r--   0 kliavinekss   (501) staff       (20)    19014 2023-09-18 16:02:08.000000 perturbopy-0.5.2/src/perturbopy/test_utils/run_test/test_driver.py
-drwxr-xr-x   0 kliavinekss   (501) staff       (20)        0 2023-11-08 21:39:53.264172 perturbopy-0.5.2/src/perturbopy/testing_code/
--rw-r--r--   0 kliavinekss   (501) staff       (20)        0 2023-08-11 16:28:30.000000 perturbopy-0.5.2/src/perturbopy/testing_code/__init__.py
--rw-r--r--   0 kliavinekss   (501) staff       (20)     3511 2023-11-03 23:37:15.000000 perturbopy-0.5.2/src/perturbopy/testing_code/test_functions.py
--rw-r--r--   0 kliavinekss   (501) staff       (20)      187 2023-08-16 19:12:43.000000 perturbopy-0.5.2/src/perturbopy/tests_use.py
-drwxr-xr-x   0 kliavinekss   (501) staff       (20)        0 2023-11-08 21:39:53.259000 perturbopy-0.5.2/src/perturbopy.egg-info/
--rw-r--r--   0 kliavinekss   (501) staff       (20)     2063 2023-11-08 21:39:53.000000 perturbopy-0.5.2/src/perturbopy.egg-info/PKG-INFO
--rw-r--r--   0 kliavinekss   (501) staff       (20)     1884 2023-11-08 21:39:53.000000 perturbopy-0.5.2/src/perturbopy.egg-info/SOURCES.txt
--rw-r--r--   0 kliavinekss   (501) staff       (20)        1 2023-11-08 21:39:53.000000 perturbopy-0.5.2/src/perturbopy.egg-info/dependency_links.txt
--rw-r--r--   0 kliavinekss   (501) staff       (20)      123 2023-11-08 21:39:53.000000 perturbopy-0.5.2/src/perturbopy.egg-info/requires.txt
--rw-r--r--   0 kliavinekss   (501) staff       (20)       11 2023-11-08 21:39:53.000000 perturbopy-0.5.2/src/perturbopy.egg-info/top_level.txt
-drwxr-xr-x   0 kliavinekss   (501) staff       (20)        0 2023-11-08 21:39:53.264953 perturbopy-0.5.2/tests/
--rw-r--r--   0 kliavinekss   (501) staff       (20)     2962 2023-09-11 17:49:22.000000 perturbopy-0.5.2/tests/test_bands_calc_mode.py
--rw-r--r--   0 kliavinekss   (501) staff       (20)     5069 2023-09-11 17:49:22.000000 perturbopy-0.5.2/tests/test_constants.py
--rw-r--r--   0 kliavinekss   (501) staff       (20)     9145 2023-09-11 17:49:22.000000 perturbopy-0.5.2/tests/test_lattice.py
--rw-r--r--   0 kliavinekss   (501) staff       (20)     2178 2023-09-11 17:49:22.000000 perturbopy-0.5.2/tests/test_plot_tools.py
--rw-r--r--   0 kliavinekss   (501) staff       (20)     5934 2023-07-28 19:19:00.000000 perturbopy-0.5.2/tests/test_recip_pt_dbs.py
+drwxr-xr-x   0 kliavinekss   (501) staff       (20)        0 2024-05-09 22:31:41.876478 perturbopy-0.5.3/
+-rw-r--r--   0 kliavinekss   (501) staff       (20)    35149 2023-07-28 19:19:00.000000 perturbopy-0.5.3/LICENSE
+-rw-r--r--   0 kliavinekss   (501) staff       (20)       40 2023-08-28 19:19:24.000000 perturbopy-0.5.3/MANIFEST.in
+-rw-r--r--   0 kliavinekss   (501) staff       (20)     2369 2024-05-09 22:31:41.876387 perturbopy-0.5.3/PKG-INFO
+-rw-r--r--   0 kliavinekss   (501) staff       (20)     1819 2023-09-18 22:49:12.000000 perturbopy-0.5.3/README.md
+-rw-r--r--   0 kliavinekss   (501) staff       (20)      132 2024-05-09 22:31:41.876725 perturbopy-0.5.3/setup.cfg
+-rw-r--r--   0 kliavinekss   (501) staff       (20)      794 2024-05-09 22:31:19.000000 perturbopy-0.5.3/setup.py
+drwxr-xr-x   0 kliavinekss   (501) staff       (20)        0 2024-05-09 22:31:41.862108 perturbopy-0.5.3/src/
+drwxr-xr-x   0 kliavinekss   (501) staff       (20)        0 2024-05-09 22:31:41.865083 perturbopy-0.5.3/src/perturbopy/
+-rw-r--r--   0 kliavinekss   (501) staff       (20)      108 2023-08-07 20:45:34.000000 perturbopy-0.5.3/src/perturbopy/__init__.py
+-rw-r--r--   0 kliavinekss   (501) staff       (20)     8694 2023-09-20 22:13:44.000000 perturbopy-0.5.3/src/perturbopy/conftest.py
+drwxr-xr-x   0 kliavinekss   (501) staff       (20)        0 2024-05-09 22:31:41.866259 perturbopy-0.5.3/src/perturbopy/io_utils/
+-rw-r--r--   0 kliavinekss   (501) staff       (20)       82 2023-07-28 19:19:00.000000 perturbopy-0.5.3/src/perturbopy/io_utils/__init__.py
+-rw-r--r--   0 kliavinekss   (501) staff       (20)      707 2023-11-07 21:51:43.000000 perturbopy-0.5.3/src/perturbopy/io_utils/io.py
+drwxr-xr-x   0 kliavinekss   (501) staff       (20)        0 2024-05-09 22:31:41.866596 perturbopy-0.5.3/src/perturbopy/postproc/
+-rw-r--r--   0 kliavinekss   (501) staff       (20)      522 2023-09-11 17:49:22.000000 perturbopy-0.5.3/src/perturbopy/postproc/__init__.py
+drwxr-xr-x   0 kliavinekss   (501) staff       (20)        0 2024-05-09 22:31:41.869946 perturbopy-0.5.3/src/perturbopy/postproc/calc_modes/
+-rw-r--r--   0 kliavinekss   (501) staff       (20)       82 2023-07-28 19:19:00.000000 perturbopy-0.5.3/src/perturbopy/postproc/calc_modes/__init__.py
+-rw-r--r--   0 kliavinekss   (501) staff       (20)     9558 2023-09-13 16:18:02.000000 perturbopy-0.5.3/src/perturbopy/postproc/calc_modes/bands.py
+-rw-r--r--   0 kliavinekss   (501) staff       (20)     3797 2023-09-11 17:49:22.000000 perturbopy-0.5.3/src/perturbopy/postproc/calc_modes/calc_mode.py
+-rw-r--r--   0 kliavinekss   (501) staff       (20)      838 2023-09-11 17:49:22.000000 perturbopy-0.5.3/src/perturbopy/postproc/calc_modes/dyna_indiv_run.py
+-rw-r--r--   0 kliavinekss   (501) staff       (20)     3145 2023-09-19 23:50:23.000000 perturbopy-0.5.3/src/perturbopy/postproc/calc_modes/dyna_pp.py
+-rw-r--r--   0 kliavinekss   (501) staff       (20)     6611 2023-11-03 23:37:15.000000 perturbopy-0.5.3/src/perturbopy/postproc/calc_modes/dyna_run.py
+-rw-r--r--   0 kliavinekss   (501) staff       (20)     7224 2023-09-19 23:50:23.000000 perturbopy-0.5.3/src/perturbopy/postproc/calc_modes/ephmat.py
+-rw-r--r--   0 kliavinekss   (501) staff       (20)     4569 2023-09-11 17:49:22.000000 perturbopy-0.5.3/src/perturbopy/postproc/calc_modes/imsigma.py
+-rw-r--r--   0 kliavinekss   (501) staff       (20)     3021 2023-09-13 16:18:02.000000 perturbopy-0.5.3/src/perturbopy/postproc/calc_modes/phdisp.py
+-rw-r--r--   0 kliavinekss   (501) staff       (20)     6248 2023-09-19 23:50:23.000000 perturbopy-0.5.3/src/perturbopy/postproc/calc_modes/trans.py
+drwxr-xr-x   0 kliavinekss   (501) staff       (20)        0 2024-05-09 22:31:41.870859 perturbopy-0.5.3/src/perturbopy/postproc/dbs/
+-rw-r--r--   0 kliavinekss   (501) staff       (20)       82 2023-07-28 19:19:00.000000 perturbopy-0.5.3/src/perturbopy/postproc/dbs/__init__.py
+-rw-r--r--   0 kliavinekss   (501) staff       (20)    10753 2023-09-11 17:49:22.000000 perturbopy-0.5.3/src/perturbopy/postproc/dbs/recip_pt_db.py
+-rw-r--r--   0 kliavinekss   (501) staff       (20)     1406 2023-09-11 17:49:22.000000 perturbopy-0.5.3/src/perturbopy/postproc/dbs/units_dict.py
+drwxr-xr-x   0 kliavinekss   (501) staff       (20)        0 2024-05-09 22:31:41.871822 perturbopy-0.5.3/src/perturbopy/postproc/utils/
+-rw-r--r--   0 kliavinekss   (501) staff       (20)       82 2023-07-28 19:19:00.000000 perturbopy-0.5.3/src/perturbopy/postproc/utils/__init__.py
+-rw-r--r--   0 kliavinekss   (501) staff       (20)    10310 2023-09-11 17:49:22.000000 perturbopy-0.5.3/src/perturbopy/postproc/utils/constants.py
+-rw-r--r--   0 kliavinekss   (501) staff       (20)     8155 2023-09-11 17:49:22.000000 perturbopy-0.5.3/src/perturbopy/postproc/utils/lattice.py
+-rw-r--r--   0 kliavinekss   (501) staff       (20)     7736 2023-09-19 23:50:23.000000 perturbopy-0.5.3/src/perturbopy/postproc/utils/plot_tools.py
+-rw-r--r--   0 kliavinekss   (501) staff       (20)     6263 2023-09-11 17:49:22.000000 perturbopy-0.5.3/src/perturbopy/postproc/utils/timing.py
+-rw-r--r--   0 kliavinekss   (501) staff       (20)       14 2023-09-19 17:29:26.000000 perturbopy-0.5.3/src/perturbopy/setup.cfg
+drwxr-xr-x   0 kliavinekss   (501) staff       (20)        0 2024-05-09 22:31:41.872035 perturbopy-0.5.3/src/perturbopy/test_utils/
+-rw-r--r--   0 kliavinekss   (501) staff       (20)       67 2023-07-28 19:27:33.000000 perturbopy-0.5.3/src/perturbopy/test_utils/__init__.py
+drwxr-xr-x   0 kliavinekss   (501) staff       (20)        0 2024-05-09 22:31:41.873348 perturbopy-0.5.3/src/perturbopy/test_utils/compare_data/
+-rw-r--r--   0 kliavinekss   (501) staff       (20)       79 2023-07-28 19:27:33.000000 perturbopy-0.5.3/src/perturbopy/test_utils/compare_data/__init__.py
+-rw-r--r--   0 kliavinekss   (501) staff       (20)     1675 2023-11-03 23:37:15.000000 perturbopy-0.5.3/src/perturbopy/test_utils/compare_data/compare.py
+-rw-r--r--   0 kliavinekss   (501) staff       (20)    11891 2023-11-04 00:15:41.000000 perturbopy-0.5.3/src/perturbopy/test_utils/compare_data/h5.py
+-rw-r--r--   0 kliavinekss   (501) staff       (20)    10761 2024-05-09 20:55:17.000000 perturbopy-0.5.3/src/perturbopy/test_utils/compare_data/yaml.py
+drwxr-xr-x   0 kliavinekss   (501) staff       (20)        0 2024-05-09 22:31:41.874590 perturbopy-0.5.3/src/perturbopy/test_utils/run_test/
+-rw-r--r--   0 kliavinekss   (501) staff       (20)       84 2023-07-28 19:27:33.000000 perturbopy-0.5.3/src/perturbopy/test_utils/run_test/__init__.py
+-rw-r--r--   0 kliavinekss   (501) staff       (20)     6611 2023-08-18 16:44:59.000000 perturbopy-0.5.3/src/perturbopy/test_utils/run_test/env_utils.py
+-rw-r--r--   0 kliavinekss   (501) staff       (20)    16071 2023-11-08 21:27:08.000000 perturbopy-0.5.3/src/perturbopy/test_utils/run_test/run_utils.py
+-rw-r--r--   0 kliavinekss   (501) staff       (20)    19014 2023-09-18 16:02:08.000000 perturbopy-0.5.3/src/perturbopy/test_utils/run_test/test_driver.py
+drwxr-xr-x   0 kliavinekss   (501) staff       (20)        0 2024-05-09 22:31:41.874910 perturbopy-0.5.3/src/perturbopy/testing_code/
+-rw-r--r--   0 kliavinekss   (501) staff       (20)        0 2023-08-11 16:28:30.000000 perturbopy-0.5.3/src/perturbopy/testing_code/__init__.py
+-rw-r--r--   0 kliavinekss   (501) staff       (20)     3511 2023-11-03 23:37:15.000000 perturbopy-0.5.3/src/perturbopy/testing_code/test_functions.py
+-rw-r--r--   0 kliavinekss   (501) staff       (20)      238 2024-05-09 20:55:17.000000 perturbopy-0.5.3/src/perturbopy/tests_use.py
+drwxr-xr-x   0 kliavinekss   (501) staff       (20)        0 2024-05-09 22:31:41.865932 perturbopy-0.5.3/src/perturbopy.egg-info/
+-rw-r--r--   0 kliavinekss   (501) staff       (20)     2369 2024-05-09 22:31:41.000000 perturbopy-0.5.3/src/perturbopy.egg-info/PKG-INFO
+-rw-r--r--   0 kliavinekss   (501) staff       (20)     1884 2024-05-09 22:31:41.000000 perturbopy-0.5.3/src/perturbopy.egg-info/SOURCES.txt
+-rw-r--r--   0 kliavinekss   (501) staff       (20)        1 2024-05-09 22:31:41.000000 perturbopy-0.5.3/src/perturbopy.egg-info/dependency_links.txt
+-rw-r--r--   0 kliavinekss   (501) staff       (20)      123 2024-05-09 22:31:41.000000 perturbopy-0.5.3/src/perturbopy.egg-info/requires.txt
+-rw-r--r--   0 kliavinekss   (501) staff       (20)       11 2024-05-09 22:31:41.000000 perturbopy-0.5.3/src/perturbopy.egg-info/top_level.txt
+drwxr-xr-x   0 kliavinekss   (501) staff       (20)        0 2024-05-09 22:31:41.875789 perturbopy-0.5.3/tests/
+-rw-r--r--   0 kliavinekss   (501) staff       (20)     2962 2023-09-11 17:49:22.000000 perturbopy-0.5.3/tests/test_bands_calc_mode.py
+-rw-r--r--   0 kliavinekss   (501) staff       (20)     5069 2023-09-11 17:49:22.000000 perturbopy-0.5.3/tests/test_constants.py
+-rw-r--r--   0 kliavinekss   (501) staff       (20)     9145 2023-09-11 17:49:22.000000 perturbopy-0.5.3/tests/test_lattice.py
+-rw-r--r--   0 kliavinekss   (501) staff       (20)     2178 2023-09-11 17:49:22.000000 perturbopy-0.5.3/tests/test_plot_tools.py
+-rw-r--r--   0 kliavinekss   (501) staff       (20)     5934 2023-07-28 19:19:00.000000 perturbopy-0.5.3/tests/test_recip_pt_dbs.py
```

### Comparing `perturbopy-0.5.2/LICENSE` & `perturbopy-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `perturbopy-0.5.2/PKG-INFO` & `perturbopy-0.5.3/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,7 @@
-Metadata-Version: 2.1
-Name: perturbopy
-Version: 0.5.2
-Summary: Suite of Python scripts for Perturbo testing and postprocessing
-Requires-Python: >=3.7.12
-Description-Content-Type: text/markdown
-Provides-Extra: interactive
-License-File: LICENSE
-
 # perturbopy - Python suite for Perturbo postprocessing and testing
 
 This package provides utilities to postprocess and test the Perturbo code, which is an open-source software to compute from first principles the scattering processes between charge carriers (electrons and holes) and phonons, defects, and photons in solid state materials, including metals, semiconductors, oxides, and insulators. Perturbo is written in modern Fortran, including efficient MPI and OpenMP parallelization, allowing to perform calculations efficient on supercomputers using up to ~100,000 cores. Read more about the main code Perturbo [here](https://perturbo-code.github.io/index.html).
 
 Perturbopy provides a user-friendly object-oriented environment to postprocess Perturbo calculations, such as band structure interpolation, electron transport, ultrafast carrier dynamics, and many more. Using Perturbopy, a user can easily load the Perturbo output files (HDF5 or YAML) into Python objects, perform calculations, and visualize data.
 
 The second purpose of the Perturbopy package is to test the main Perturbo code. After a compilation of the Perturbo code on a new machine or after a new implementation, it is always a good practice to run the testsuite, verifying that the existing functionality was not affected, and add new test cases to ensure that the newly implemented features will be compatible with future implementations. Perturbopy, using the `pytest` package, provides extensive testing of Perturbo, allowing for both serial and parallel runs.
```

### Comparing `perturbopy-0.5.2/setup.py` & `perturbopy-0.5.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
     
 setup(
     name='perturbopy',
-    version='0.5.2',
+    version='0.5.3',
     description="Suite of Python scripts for Perturbo testing and postprocessing",
     long_description=long_description,
     long_description_content_type="text/markdown",
     python_requires='>=3.7.12',
     include_package_data=True,
     install_requires=[
         'numpy>=1.21.4',
```

### Comparing `perturbopy-0.5.2/src/perturbopy/conftest.py` & `perturbopy-0.5.3/src/perturbopy/conftest.py`

 * *Files identical despite different names*

### Comparing `perturbopy-0.5.2/src/perturbopy/io_utils/io.py` & `perturbopy-0.5.3/src/perturbopy/io_utils/io.py`

 * *Files identical despite different names*

### Comparing `perturbopy-0.5.2/src/perturbopy/postproc/__init__.py` & `perturbopy-0.5.3/src/perturbopy/postproc/__init__.py`

 * *Files identical despite different names*

### Comparing `perturbopy-0.5.2/src/perturbopy/postproc/calc_modes/bands.py` & `perturbopy-0.5.3/src/perturbopy/postproc/calc_modes/bands.py`

 * *Files identical despite different names*

### Comparing `perturbopy-0.5.2/src/perturbopy/postproc/calc_modes/calc_mode.py` & `perturbopy-0.5.3/src/perturbopy/postproc/calc_modes/calc_mode.py`

 * *Files identical despite different names*

### Comparing `perturbopy-0.5.2/src/perturbopy/postproc/calc_modes/dyna_indiv_run.py` & `perturbopy-0.5.3/src/perturbopy/postproc/calc_modes/dyna_indiv_run.py`

 * *Files identical despite different names*

### Comparing `perturbopy-0.5.2/src/perturbopy/postproc/calc_modes/dyna_pp.py` & `perturbopy-0.5.3/src/perturbopy/postproc/calc_modes/dyna_pp.py`

 * *Files identical despite different names*

### Comparing `perturbopy-0.5.2/src/perturbopy/postproc/calc_modes/dyna_run.py` & `perturbopy-0.5.3/src/perturbopy/postproc/calc_modes/dyna_run.py`

 * *Files identical despite different names*

### Comparing `perturbopy-0.5.2/src/perturbopy/postproc/calc_modes/ephmat.py` & `perturbopy-0.5.3/src/perturbopy/postproc/calc_modes/ephmat.py`

 * *Files identical despite different names*

### Comparing `perturbopy-0.5.2/src/perturbopy/postproc/calc_modes/imsigma.py` & `perturbopy-0.5.3/src/perturbopy/postproc/calc_modes/imsigma.py`

 * *Files identical despite different names*

### Comparing `perturbopy-0.5.2/src/perturbopy/postproc/calc_modes/phdisp.py` & `perturbopy-0.5.3/src/perturbopy/postproc/calc_modes/phdisp.py`

 * *Files identical despite different names*

### Comparing `perturbopy-0.5.2/src/perturbopy/postproc/calc_modes/trans.py` & `perturbopy-0.5.3/src/perturbopy/postproc/calc_modes/trans.py`

 * *Files identical despite different names*

### Comparing `perturbopy-0.5.2/src/perturbopy/postproc/dbs/recip_pt_db.py` & `perturbopy-0.5.3/src/perturbopy/postproc/dbs/recip_pt_db.py`

 * *Files identical despite different names*

### Comparing `perturbopy-0.5.2/src/perturbopy/postproc/dbs/units_dict.py` & `perturbopy-0.5.3/src/perturbopy/postproc/dbs/units_dict.py`

 * *Files identical despite different names*

### Comparing `perturbopy-0.5.2/src/perturbopy/postproc/utils/constants.py` & `perturbopy-0.5.3/src/perturbopy/postproc/utils/constants.py`

 * *Files identical despite different names*

### Comparing `perturbopy-0.5.2/src/perturbopy/postproc/utils/lattice.py` & `perturbopy-0.5.3/src/perturbopy/postproc/utils/lattice.py`

 * *Files identical despite different names*

### Comparing `perturbopy-0.5.2/src/perturbopy/postproc/utils/plot_tools.py` & `perturbopy-0.5.3/src/perturbopy/postproc/utils/plot_tools.py`

 * *Files identical despite different names*

### Comparing `perturbopy-0.5.2/src/perturbopy/postproc/utils/timing.py` & `perturbopy-0.5.3/src/perturbopy/postproc/utils/timing.py`

 * *Files identical despite different names*

### Comparing `perturbopy-0.5.2/src/perturbopy/test_utils/compare_data/compare.py` & `perturbopy-0.5.3/src/perturbopy/test_utils/compare_data/compare.py`

 * *Files identical despite different names*

### Comparing `perturbopy-0.5.2/src/perturbopy/test_utils/compare_data/h5.py` & `perturbopy-0.5.3/src/perturbopy/test_utils/compare_data/h5.py`

 * *Files identical despite different names*

### Comparing `perturbopy-0.5.2/src/perturbopy/test_utils/compare_data/yaml.py` & `perturbopy-0.5.3/src/perturbopy/test_utils/compare_data/yaml.py`

 * *Files 4% similar despite different names*

```diff
@@ -117,14 +117,25 @@
         elif isinstance(item1, list):
             equal_value, diff, output_res = equal_list(item1, item2, key, ig_n_tol, item_path)
 
         elif isinstance(item1, Number):
             equal_value, diff, output_res = equal_scalar(item1, item2, key, ig_n_tol)
 
         elif isinstance(item1, str):
+            item1 = item1.lower()
+            item2 = item2.lower()
+
+            # Some Fortran compilers output 'Infinity' while others output
+            # 'Inf'.  Convert all such strings to 'inf' so that infinity
+            # values compare equal.
+            if item1.endswith('infinity'):
+                item1 = item1.lower()[:-5]
+            if item2.endswith('infinity'):
+                item2 = item2.lower()[:-5]
+
             equal_value = item1 == item2
             diff = f'{item1} {item2}'
 
         elif isinstance(item1, type(None)):
             equal_value = item1 == item2
             diff = None
 
@@ -217,16 +228,27 @@
         elif isinstance(dict1[key], list):
             equal_value, diff, output_res = equal_list(dict1[key], dict2[key], key, ig_n_tol, key_path)
 
         elif isinstance(dict1[key], Number):
             equal_value, diff, output_res = equal_scalar(dict1[key], dict2[key], key, ig_n_tol)
 
         elif isinstance(dict1[key], str):
-            equal_value = dict1[key] == dict2[key]
-            diff = f'{dict1[key]} {dict2[key]}'
+            item1 = dict1[key].lower()
+            item2 = dict2[key].lower()
+
+            # Some Fortran compilers output 'Infinity' while others output
+            # 'Inf'.  Convert all such strings to 'inf' so that infinity
+            # values compare equal.
+            if item1.endswith('infinity'):
+                item1 = item1[:-5]
+            if item2.endswith('infinity'):
+                item2 = item2[:-5]
+
+            equal_value = item1 == item2
+            diff = f'{item1} {item2}'
 
         elif isinstance(dict1[key], type(None)):
             equal_value = dict1[key] == dict2[key]
             diff = None
 
         else:
             errmsg = (f'dict must only contain values of type dict, list, scalar, None, or str '
```

### Comparing `perturbopy-0.5.2/src/perturbopy/test_utils/run_test/env_utils.py` & `perturbopy-0.5.3/src/perturbopy/test_utils/run_test/env_utils.py`

 * *Files identical despite different names*

### Comparing `perturbopy-0.5.2/src/perturbopy/test_utils/run_test/run_utils.py` & `perturbopy-0.5.3/src/perturbopy/test_utils/run_test/run_utils.py`

 * *Files identical despite different names*

### Comparing `perturbopy-0.5.2/src/perturbopy/test_utils/run_test/test_driver.py` & `perturbopy-0.5.3/src/perturbopy/test_utils/run_test/test_driver.py`

 * *Files identical despite different names*

### Comparing `perturbopy-0.5.2/src/perturbopy/testing_code/test_functions.py` & `perturbopy-0.5.3/src/perturbopy/testing_code/test_functions.py`

 * *Files identical despite different names*

### Comparing `perturbopy-0.5.2/src/perturbopy.egg-info/SOURCES.txt` & `perturbopy-0.5.3/src/perturbopy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `perturbopy-0.5.2/tests/test_bands_calc_mode.py` & `perturbopy-0.5.3/tests/test_bands_calc_mode.py`

 * *Files identical despite different names*

### Comparing `perturbopy-0.5.2/tests/test_constants.py` & `perturbopy-0.5.3/tests/test_constants.py`

 * *Files identical despite different names*

### Comparing `perturbopy-0.5.2/tests/test_lattice.py` & `perturbopy-0.5.3/tests/test_lattice.py`

 * *Files identical despite different names*

### Comparing `perturbopy-0.5.2/tests/test_plot_tools.py` & `perturbopy-0.5.3/tests/test_plot_tools.py`

 * *Files identical despite different names*

### Comparing `perturbopy-0.5.2/tests/test_recip_pt_dbs.py` & `perturbopy-0.5.3/tests/test_recip_pt_dbs.py`

 * *Files identical despite different names*

