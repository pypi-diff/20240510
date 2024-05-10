# Comparing `tmp/radical_analytics-1.52.0.tar.gz` & `tmp/radical.analytics-1.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "radical_analytics-1.52.0.tar", last modified: Mon Apr 15 09:56:04 2024, max compression
+gzip compressed data, was "radical.analytics-1.6.7.tar", last modified: Thu Jul  8 08:08:44 2021, max compression
```

## Comparing `radical_analytics-1.52.0.tar` & `radical.analytics-1.6.7.tar`

### file list

```diff
@@ -1,71 +1,103 @@
-drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-04-15 09:56:04.017857 radical_analytics-1.52.0/
--rw-rw-r--   0 merzky    (1000) merzky    (1000)     9975 2021-09-24 08:24:17.000000 radical_analytics-1.52.0/API.md
--rw-rw-r--   0 merzky    (1000) merzky    (1000)    10004 2024-04-15 09:55:59.000000 radical_analytics-1.52.0/CHANGES.md
--rw-rw-r--   0 merzky    (1000) merzky    (1000)     1300 2024-04-15 09:55:56.000000 radical_analytics-1.52.0/LICENSE.md
--rw-rw-r--   0 merzky    (1000) merzky    (1000)      209 2024-04-15 09:55:56.000000 radical_analytics-1.52.0/MANIFEST.in
--rw-r--r--   0 merzky    (1000) merzky    (1000)     2540 2024-04-15 09:56:04.017857 radical_analytics-1.52.0/PKG-INFO
--rw-rw-r--   0 merzky    (1000) merzky    (1000)     1139 2021-09-24 08:24:17.000000 radical_analytics-1.52.0/README.md
--rw-rw-r--   0 merzky    (1000) merzky    (1000)        7 2024-04-15 09:55:56.000000 radical_analytics-1.52.0/VERSION
-drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-04-15 09:56:04.017857 radical_analytics-1.52.0/bin/
--rwxrwxr-x   0 merzky    (1000) merzky    (1000)     5032 2024-04-15 09:55:56.000000 radical_analytics-1.52.0/bin/radical-analytics-check
--rwxrwxr-x   0 merzky    (1000) merzky    (1000)     6006 2024-04-15 09:55:56.000000 radical_analytics-1.52.0/bin/radical-analytics-inspect
--rwxrwxr-x   0 merzky    (1000) merzky    (1000)     3637 2024-04-15 09:55:56.000000 radical_analytics-1.52.0/bin/radical-analytics-parse-profile.py
--rwxrwxr-x   0 merzky    (1000) merzky    (1000)    10588 2024-04-15 09:55:56.000000 radical_analytics-1.52.0/bin/radical-analytics-plot.py
--rwxrwxr-x   0 merzky    (1000) merzky    (1000)       88 2021-09-24 08:24:17.000000 radical_analytics-1.52.0/bin/radical-analytics-version
--rwxrwxr-x   0 merzky    (1000) merzky    (1000)    36969 2021-09-24 08:24:17.000000 radical_analytics-1.52.0/bin/radical-analytics-wrangler.py
-drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-04-15 09:56:04.017857 radical_analytics-1.52.0/bin/rp_inspect/
--rwxrwxr-x   0 merzky    (1000) merzky    (1000)     3198 2024-04-15 09:55:56.000000 radical_analytics-1.52.0/bin/rp_inspect/plot_conc.py
--rwxrwxr-x   0 merzky    (1000) merzky    (1000)     4965 2024-04-15 09:55:56.000000 radical_analytics-1.52.0/bin/rp_inspect/plot_dur.py
--rwxrwxr-x   0 merzky    (1000) merzky    (1000)     2957 2024-04-15 09:55:56.000000 radical_analytics-1.52.0/bin/rp_inspect/plot_rate.py
--rwxrwxr-x   0 merzky    (1000) merzky    (1000)     4833 2024-04-15 09:55:56.000000 radical_analytics-1.52.0/bin/rp_inspect/plot_state.py
--rwxrwxr-x   0 merzky    (1000) merzky    (1000)     6922 2024-04-15 09:55:56.000000 radical_analytics-1.52.0/bin/rp_inspect/plot_util.py
--rwxrwxr-x   0 merzky    (1000) merzky    (1000)    10135 2024-04-15 09:55:56.000000 radical_analytics-1.52.0/bin/rp_inspect/plot_util_2.py
-drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-04-15 09:56:04.013857 radical_analytics-1.52.0/docs/
-drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-04-15 09:56:04.017857 radical_analytics-1.52.0/docs/source/
--rw-rw-r--   0 merzky    (1000) merzky    (1000)     2763 2024-04-15 09:55:56.000000 radical_analytics-1.52.0/docs/source/README.md
--rw-rw-r--   0 merzky    (1000) merzky    (1000)    14624 2024-04-15 09:55:56.000000 radical_analytics-1.52.0/docs/source/metrics.md
-drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-04-15 09:56:04.017857 radical_analytics-1.52.0/examples/
--rwxrwxr-x   0 merzky    (1000) merzky    (1000)     3017 2021-09-24 08:24:17.000000 radical_analytics-1.52.0/examples/00_session_describe_rp.py
--rwxrwxr-x   0 merzky    (1000) merzky    (1000)     2514 2021-09-24 08:24:17.000000 radical_analytics-1.52.0/examples/01_session_list_rp.py
--rwxrwxr-x   0 merzky    (1000) merzky    (1000)     4166 2021-09-24 08:24:17.000000 radical_analytics-1.52.0/examples/02_session_get_rp.py
--rwxrwxr-x   0 merzky    (1000) merzky    (1000)     3036 2021-09-24 08:24:17.000000 radical_analytics-1.52.0/examples/03_session_filter_rp.py
--rwxrwxr-x   0 merzky    (1000) merzky    (1000)     4465 2021-09-24 08:24:17.000000 radical_analytics-1.52.0/examples/04_session_duration_rp.py
--rwxrwxr-x   0 merzky    (1000) merzky    (1000)     1520 2021-09-24 08:24:17.000000 radical_analytics-1.52.0/examples/05_relationsships.py
--rwxrwxr-x   0 merzky    (1000) merzky    (1000)     4856 2021-09-24 08:24:17.000000 radical_analytics-1.52.0/examples/06_events.py
--rwxrwxr-x   0 merzky    (1000) merzky    (1000)     1289 2021-09-24 08:24:17.000000 radical_analytics-1.52.0/examples/06_ra_events.py
--rwxrwxr-x   0 merzky    (1000) merzky    (1000)     4827 2021-09-24 08:24:17.000000 radical_analytics-1.52.0/examples/07_event_timeline.py
--rwxrwxr-x   0 merzky    (1000) merzky    (1000)     5940 2021-09-24 08:24:17.000000 radical_analytics-1.52.0/examples/08_core_utilization_plot.py
--rwxrwxr-x   0 merzky    (1000) merzky    (1000)     8909 2021-09-24 08:24:17.000000 radical_analytics-1.52.0/examples/08c_core_utilization_plot.py
--rwxrwxr-x   0 merzky    (1000) merzky    (1000)     4990 2021-09-24 08:24:17.000000 radical_analytics-1.52.0/examples/09_session_plots.py
--rwxrwxr-x   0 merzky    (1000) merzky    (1000)     4717 2021-09-24 08:24:17.000000 radical_analytics-1.52.0/examples/10_durations.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)      126 2024-04-15 09:55:56.000000 radical_analytics-1.52.0/requirements-docs.txt
--rw-rw-r--   0 merzky    (1000) merzky    (1000)       71 2024-04-15 09:55:56.000000 radical_analytics-1.52.0/requirements-tests.txt
--rw-rw-r--   0 merzky    (1000) merzky    (1000)       70 2024-04-15 09:55:56.000000 radical_analytics-1.52.0/requirements.txt
--rw-rw-r--   0 merzky    (1000) merzky    (1000)       38 2024-04-15 09:56:04.017857 radical_analytics-1.52.0/setup.cfg
--rwxrwxr-x   0 merzky    (1000) merzky    (1000)    10959 2024-04-15 09:55:56.000000 radical_analytics-1.52.0/setup.py
-drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-04-15 09:56:04.013857 radical_analytics-1.52.0/src/
-drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-04-15 09:56:04.013857 radical_analytics-1.52.0/src/radical/
-drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-04-15 09:56:04.017857 radical_analytics-1.52.0/src/radical/analytics/
--rw-rw-r--   0 merzky    (1000) merzky    (1000)       32 2024-04-15 09:56:03.000000 radical_analytics-1.52.0/src/radical/analytics/SDIST
--rw-rw-r--   0 merzky    (1000) merzky    (1000)       29 2024-04-15 09:56:03.000000 radical_analytics-1.52.0/src/radical/analytics/VERSION
--rw-rw-r--   0 merzky    (1000) merzky    (1000)     1447 2024-04-15 09:55:56.000000 radical_analytics-1.52.0/src/radical/analytics/__init__.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)    17962 2024-04-15 09:55:56.000000 radical_analytics-1.52.0/src/radical/analytics/entity.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)     5158 2024-04-15 09:55:56.000000 radical_analytics-1.52.0/src/radical/analytics/experiment.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)     6514 2024-04-15 09:55:56.000000 radical_analytics-1.52.0/src/radical/analytics/plotter.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)    57418 2024-04-15 09:55:56.000000 radical_analytics-1.52.0/src/radical/analytics/session.py
-drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-04-15 09:56:04.017857 radical_analytics-1.52.0/src/radical/analytics/utils/
--rw-rw-r--   0 merzky    (1000) merzky    (1000)      639 2024-04-15 09:55:56.000000 radical_analytics-1.52.0/src/radical/analytics/utils/__init__.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)    17826 2024-04-15 09:55:56.000000 radical_analytics-1.52.0/src/radical/analytics/utils/plot.py
-drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-04-15 09:56:04.017857 radical_analytics-1.52.0/src/radical.analytics.egg-info/
--rw-r--r--   0 merzky    (1000) merzky    (1000)     2540 2024-04-15 09:56:03.000000 radical_analytics-1.52.0/src/radical.analytics.egg-info/PKG-INFO
--rw-rw-r--   0 merzky    (1000) merzky    (1000)     1601 2024-04-15 09:56:04.000000 radical_analytics-1.52.0/src/radical.analytics.egg-info/SOURCES.txt
--rw-rw-r--   0 merzky    (1000) merzky    (1000)        1 2024-04-15 09:56:03.000000 radical_analytics-1.52.0/src/radical.analytics.egg-info/dependency_links.txt
--rw-rw-r--   0 merzky    (1000) merzky    (1000)        1 2024-04-15 09:56:03.000000 radical_analytics-1.52.0/src/radical.analytics.egg-info/not-zip-safe
--rw-rw-r--   0 merzky    (1000) merzky    (1000)       71 2024-04-15 09:56:03.000000 radical_analytics-1.52.0/src/radical.analytics.egg-info/requires.txt
--rw-rw-r--   0 merzky    (1000) merzky    (1000)        8 2024-04-15 09:56:03.000000 radical_analytics-1.52.0/src/radical.analytics.egg-info/top_level.txt
-drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-04-15 09:56:04.017857 radical_analytics-1.52.0/styles/
--rw-rw-r--   0 merzky    (1000) merzky    (1000)     1682 2024-04-15 09:55:56.000000 radical_analytics-1.52.0/styles/radical_mpl.txt
-drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-04-15 09:56:04.017857 radical_analytics-1.52.0/tests/
--rw-rw-r--   0 merzky    (1000) merzky    (1000)     6185 2021-09-24 08:24:17.000000 radical_analytics-1.52.0/tests/test_duration_method.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)    26961 2024-04-15 09:55:56.000000 radical_analytics-1.52.0/tests/test_entity.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)      277 2021-09-24 08:24:17.000000 radical_analytics-1.52.0/tests/test_session.py
+drwxr-xr-x   0 mturilli   (501) staff       (20)        0 2021-07-08 08:08:44.969621 radical.analytics-1.6.7/
+-rw-r--r--   0 mturilli   (501) staff       (20)     5822 2021-07-08 08:06:17.000000 radical.analytics-1.6.7/CHANGES.md
+-rw-r--r--   0 mturilli   (501) staff       (20)     1093 2021-07-08 08:04:41.000000 radical.analytics-1.6.7/LICENSE
+-rw-r--r--   0 mturilli   (501) staff       (20)      115 2020-05-05 15:05:35.000000 radical.analytics-1.6.7/MANIFEST.in
+-rw-r--r--   0 mturilli   (501) staff       (20)      958 2021-07-08 08:08:44.969018 radical.analytics-1.6.7/PKG-INFO
+-rw-r--r--   0 mturilli   (501) staff       (20)     1139 2021-07-08 08:04:41.000000 radical.analytics-1.6.7/README.md
+-rw-r--r--   0 mturilli   (501) staff       (20)        6 2021-07-08 08:06:17.000000 radical.analytics-1.6.7/VERSION
+drwxr-xr-x   0 mturilli   (501) staff       (20)        0 2021-07-08 08:08:44.750461 radical.analytics-1.6.7/bin/
+-rwxr-xr-x   0 mturilli   (501) staff       (20)     4756 2021-07-08 08:04:41.000000 radical.analytics-1.6.7/bin/radical-analytics-check
+-rwxr-xr-x   0 mturilli   (501) staff       (20)     6006 2021-07-08 08:04:41.000000 radical.analytics-1.6.7/bin/radical-analytics-inspect
+-rwxr-xr-x   0 mturilli   (501) staff       (20)    10588 2021-07-08 08:04:41.000000 radical.analytics-1.6.7/bin/radical-analytics-plot.py
+-rwxr-xr-x   0 mturilli   (501) staff       (20)       88 2020-08-11 13:23:09.000000 radical.analytics-1.6.7/bin/radical-analytics-version
+-rwxr-xr-x   0 mturilli   (501) staff       (20)    36969 2020-05-05 15:05:35.000000 radical.analytics-1.6.7/bin/radical-analytics-wrangler.py
+drwxr-xr-x   0 mturilli   (501) staff       (20)        0 2021-07-08 08:08:44.753940 radical.analytics-1.6.7/bin/rp_inspect/
+-rwxr-xr-x   0 mturilli   (501) staff       (20)     3198 2021-07-08 08:04:41.000000 radical.analytics-1.6.7/bin/rp_inspect/plot_conc.py
+-rwxr-xr-x   0 mturilli   (501) staff       (20)     4937 2021-07-08 08:04:41.000000 radical.analytics-1.6.7/bin/rp_inspect/plot_dur.py
+-rwxr-xr-x   0 mturilli   (501) staff       (20)     2957 2021-07-08 08:04:41.000000 radical.analytics-1.6.7/bin/rp_inspect/plot_rate.py
+-rwxr-xr-x   0 mturilli   (501) staff       (20)     4824 2021-07-08 08:04:41.000000 radical.analytics-1.6.7/bin/rp_inspect/plot_state.py
+-rwxr-xr-x   0 mturilli   (501) staff       (20)     6903 2021-07-08 08:04:41.000000 radical.analytics-1.6.7/bin/rp_inspect/plot_util.py
+-rwxr-xr-x   0 mturilli   (501) staff       (20)     6785 2021-07-08 08:04:41.000000 radical.analytics-1.6.7/bin/rp_inspect/plot_util_2.py
+drwxr-xr-x   0 mturilli   (501) staff       (20)        0 2021-07-08 08:08:44.761312 radical.analytics-1.6.7/examples/
+-rwxr-xr-x   0 mturilli   (501) staff       (20)     3017 2020-05-05 15:05:35.000000 radical.analytics-1.6.7/examples/00_session_describe_rp.py
+-rwxr-xr-x   0 mturilli   (501) staff       (20)     2514 2020-05-05 15:05:35.000000 radical.analytics-1.6.7/examples/01_session_list_rp.py
+-rwxr-xr-x   0 mturilli   (501) staff       (20)     4166 2020-05-05 15:05:35.000000 radical.analytics-1.6.7/examples/02_session_get_rp.py
+-rwxr-xr-x   0 mturilli   (501) staff       (20)     3036 2020-05-05 15:05:35.000000 radical.analytics-1.6.7/examples/03_session_filter_rp.py
+-rwxr-xr-x   0 mturilli   (501) staff       (20)     4465 2020-05-05 15:05:35.000000 radical.analytics-1.6.7/examples/04_session_duration_rp.py
+-rwxr-xr-x   0 mturilli   (501) staff       (20)     1520 2020-05-05 15:05:35.000000 radical.analytics-1.6.7/examples/05_relationsships.py
+-rwxr-xr-x   0 mturilli   (501) staff       (20)     4856 2020-05-05 15:05:35.000000 radical.analytics-1.6.7/examples/06_events.py
+-rwxr-xr-x   0 mturilli   (501) staff       (20)     1289 2020-05-05 15:05:35.000000 radical.analytics-1.6.7/examples/06_ra_events.py
+-rwxr-xr-x   0 mturilli   (501) staff       (20)     4827 2020-05-05 15:05:35.000000 radical.analytics-1.6.7/examples/07_event_timeline.py
+-rwxr-xr-x   0 mturilli   (501) staff       (20)     5940 2020-05-05 15:05:35.000000 radical.analytics-1.6.7/examples/08_core_utilization_plot.py
+-rwxr-xr-x   0 mturilli   (501) staff       (20)     8909 2020-05-05 15:05:35.000000 radical.analytics-1.6.7/examples/08c_core_utilization_plot.py
+-rwxr-xr-x   0 mturilli   (501) staff       (20)     4990 2020-05-05 15:05:35.000000 radical.analytics-1.6.7/examples/09_session_plots.py
+-rwxr-xr-x   0 mturilli   (501) staff       (20)     4717 2020-05-05 15:05:35.000000 radical.analytics-1.6.7/examples/10_durations.py
+-rw-r--r--   0 mturilli   (501) staff       (20)       38 2021-07-08 08:08:44.969798 radical.analytics-1.6.7/setup.cfg
+-rwxr-xr-x   0 mturilli   (501) staff       (20)     9903 2021-07-08 08:06:17.000000 radical.analytics-1.6.7/setup.py
+drwxr-xr-x   0 mturilli   (501) staff       (20)        0 2021-07-08 08:08:44.742047 radical.analytics-1.6.7/src/
+drwxr-xr-x   0 mturilli   (501) staff       (20)        0 2021-07-08 08:08:44.742210 radical.analytics-1.6.7/src/radical/
+drwxr-xr-x   0 mturilli   (501) staff       (20)        0 2021-07-08 08:08:44.817963 radical.analytics-1.6.7/src/radical/analytics/
+-rw-r--r--   0 mturilli   (501) staff       (20)       47 2021-07-08 08:08:44.000000 radical.analytics-1.6.7/src/radical/analytics/SDIST
+-rw-r--r--   0 mturilli   (501) staff       (20)       22 2021-07-08 08:08:44.000000 radical.analytics-1.6.7/src/radical/analytics/VERSION
+-rw-r--r--   0 mturilli   (501) staff       (20)     1361 2021-07-08 08:04:41.000000 radical.analytics-1.6.7/src/radical/analytics/__init__.py
+-rw-r--r--   0 mturilli   (501) staff       (20)    17509 2021-07-08 08:04:41.000000 radical.analytics-1.6.7/src/radical/analytics/entity.py
+-rw-r--r--   0 mturilli   (501) staff       (20)     4631 2021-07-08 08:04:41.000000 radical.analytics-1.6.7/src/radical/analytics/experiment.py
+-rw-r--r--   0 mturilli   (501) staff       (20)     6514 2020-06-23 08:47:15.000000 radical.analytics-1.6.7/src/radical/analytics/plotter.py
+-rw-r--r--   0 mturilli   (501) staff       (20)    56570 2021-07-08 08:04:41.000000 radical.analytics-1.6.7/src/radical/analytics/session.py
+drwxr-xr-x   0 mturilli   (501) staff       (20)        0 2021-07-08 08:08:44.819208 radical.analytics-1.6.7/src/radical/analytics/utils/
+-rw-r--r--   0 mturilli   (501) staff       (20)      581 2021-07-08 08:04:41.000000 radical.analytics-1.6.7/src/radical/analytics/utils/__init__.py
+-rw-r--r--   0 mturilli   (501) staff       (20)    14771 2021-07-08 08:04:41.000000 radical.analytics-1.6.7/src/radical/analytics/utils/plot.py
+drwxr-xr-x   0 mturilli   (501) staff       (20)        0 2021-07-08 08:08:44.765025 radical.analytics-1.6.7/src/radical.analytics.egg-info/
+-rw-r--r--   0 mturilli   (501) staff       (20)      958 2021-07-08 08:08:44.000000 radical.analytics-1.6.7/src/radical.analytics.egg-info/PKG-INFO
+-rw-r--r--   0 mturilli   (501) staff       (20)     4376 2021-07-08 08:08:44.000000 radical.analytics-1.6.7/src/radical.analytics.egg-info/SOURCES.txt
+-rw-r--r--   0 mturilli   (501) staff       (20)        1 2021-07-08 08:08:44.000000 radical.analytics-1.6.7/src/radical.analytics.egg-info/dependency_links.txt
+-rw-r--r--   0 mturilli   (501) staff       (20)        8 2021-07-08 08:08:44.000000 radical.analytics-1.6.7/src/radical.analytics.egg-info/namespace_packages.txt
+-rw-r--r--   0 mturilli   (501) staff       (20)        1 2021-07-08 08:08:44.000000 radical.analytics-1.6.7/src/radical.analytics.egg-info/not-zip-safe
+-rw-r--r--   0 mturilli   (501) staff       (20)       83 2021-07-08 08:08:44.000000 radical.analytics-1.6.7/src/radical.analytics.egg-info/requires.txt
+-rw-r--r--   0 mturilli   (501) staff       (20)        8 2021-07-08 08:08:44.000000 radical.analytics-1.6.7/src/radical.analytics.egg-info/top_level.txt
+drwxr-xr-x   0 mturilli   (501) staff       (20)        0 2021-07-08 08:08:44.819699 radical.analytics-1.6.7/styles/
+-rw-r--r--   0 mturilli   (501) staff       (20)     1675 2021-07-08 08:04:41.000000 radical.analytics-1.6.7/styles/radical_mpl.txt
+drwxr-xr-x   0 mturilli   (501) staff       (20)        0 2021-07-08 08:08:44.821709 radical.analytics-1.6.7/tests/
+-rw-r--r--   0 mturilli   (501) staff       (20)        0 2020-05-05 15:05:35.000000 radical.analytics-1.6.7/tests/__init__.py
+drwxr-xr-x   0 mturilli   (501) staff       (20)        0 2021-07-08 08:08:44.822394 radical.analytics-1.6.7/tests/barrier_data/
+drwxr-xr-x   0 mturilli   (501) staff       (20)        0 2021-07-08 08:08:44.834169 radical.analytics-1.6.7/tests/barrier_data/rp.session.two.jdakka.017395.0000/
+-rw-r--r--   0 mturilli   (501) staff       (20)     1291 2020-05-05 15:05:35.000000 radical.analytics-1.6.7/tests/barrier_data/rp.session.two.jdakka.017395.0000/pmgr.0000.prof
+-rw-r--r--   0 mturilli   (501) staff       (20)        0 2020-05-05 15:05:35.000000 radical.analytics-1.6.7/tests/barrier_data/rp.session.two.jdakka.017395.0000/pmgr.launching.0.child.prof
+-rw-r--r--   0 mturilli   (501) staff       (20)      486 2020-05-05 15:05:35.000000 radical.analytics-1.6.7/tests/barrier_data/rp.session.two.jdakka.017395.0000/pmgr.launching.0.prof
+-rw-r--r--   0 mturilli   (501) staff       (20)      855 2020-05-05 15:05:35.000000 radical.analytics-1.6.7/tests/barrier_data/rp.session.two.jdakka.017395.0000/rp.session.two.jdakka.017395.0000.prof
+-rw-r--r--   0 mturilli   (501) staff       (20)   339968 2020-05-05 15:05:35.000000 radical.analytics-1.6.7/tests/barrier_data/rp.session.two.jdakka.017395.0000/umgr.0000.prof
+-rw-r--r--   0 mturilli   (501) staff       (20)    93001 2020-05-05 15:05:35.000000 radical.analytics-1.6.7/tests/barrier_data/rp.session.two.jdakka.017395.0000/umgr.scheduling.0.child.prof
+-rw-r--r--   0 mturilli   (501) staff       (20)      144 2020-05-05 15:05:35.000000 radical.analytics-1.6.7/tests/barrier_data/rp.session.two.jdakka.017395.0000/umgr.scheduling.0.prof
+-rw-r--r--   0 mturilli   (501) staff       (20)    83051 2020-05-05 15:05:35.000000 radical.analytics-1.6.7/tests/barrier_data/rp.session.two.jdakka.017395.0000/umgr.staging.input.0.child.prof
+-rw-r--r--   0 mturilli   (501) staff       (20)      148 2020-05-05 15:05:35.000000 radical.analytics-1.6.7/tests/barrier_data/rp.session.two.jdakka.017395.0000/umgr.staging.input.0.prof
+-rw-r--r--   0 mturilli   (501) staff       (20)    79361 2020-05-05 15:05:35.000000 radical.analytics-1.6.7/tests/barrier_data/rp.session.two.jdakka.017395.0000/umgr.staging.output.0.child.prof
+-rw-r--r--   0 mturilli   (501) staff       (20)      149 2020-05-05 15:05:35.000000 radical.analytics-1.6.7/tests/barrier_data/rp.session.two.jdakka.017395.0000/umgr.staging.output.0.prof
+-rw-r--r--   0 mturilli   (501) staff       (20)   647168 2020-05-05 15:05:35.000000 radical.analytics-1.6.7/tests/barrier_data/rp.session.two.jdakka.017395.0000/update.0.child.prof
+-rw-r--r--   0 mturilli   (501) staff       (20)      430 2020-05-05 15:05:35.000000 radical.analytics-1.6.7/tests/barrier_data/rp.session.two.jdakka.017395.0000/update.0.prof
+-rw-r--r--   0 mturilli   (501) staff       (20)   426921 2020-05-05 15:05:35.000000 radical.analytics-1.6.7/tests/barrier_data/rp.session.two.jdakka.017395.0000.json
+drwxr-xr-x   0 mturilli   (501) staff       (20)        0 2021-07-08 08:08:44.839229 radical.analytics-1.6.7/tests/example-data/
+-rw-r--r--   0 mturilli   (501) staff       (20)     7071 2020-05-05 15:05:35.000000 radical.analytics-1.6.7/tests/example-data/pilot-entity-example.json
+-rw-r--r--   0 mturilli   (501) staff       (20)     1503 2020-05-05 15:05:35.000000 radical.analytics-1.6.7/tests/example-data/pmgr-entity-example.json
+-rw-r--r--   0 mturilli   (501) staff       (20)     7057 2020-05-05 15:05:35.000000 radical.analytics-1.6.7/tests/example-data/range-testing-entity-example.json
+-rw-r--r--   0 mturilli   (501) staff       (20)    22261 2020-05-05 15:05:35.000000 radical.analytics-1.6.7/tests/example-data/rp-entity-example.json
+-rw-r--r--   0 mturilli   (501) staff       (20)     3543 2020-05-05 15:05:35.000000 radical.analytics-1.6.7/tests/example-data/umgr-entity-example.json
+-rw-r--r--   0 mturilli   (501) staff       (20)    13630 2021-07-08 08:04:41.000000 radical.analytics-1.6.7/tests/example-data/unit-entity-example.json
+drwxr-xr-x   0 mturilli   (501) staff       (20)        0 2021-07-08 08:08:44.913094 radical.analytics-1.6.7/tests/no_barrier_data/
+drwxr-xr-x   0 mturilli   (501) staff       (20)        0 2021-07-08 08:08:44.967522 radical.analytics-1.6.7/tests/no_barrier_data/rp.session.js-17-212.jetstream-cloud.org.vivek91.017401.0007/
+-rw-r--r--   0 mturilli   (501) staff       (20)     1208 2020-05-05 15:05:35.000000 radical.analytics-1.6.7/tests/no_barrier_data/rp.session.js-17-212.jetstream-cloud.org.vivek91.017401.0007/pmgr.0000.prof
+-rw-r--r--   0 mturilli   (501) staff       (20)        0 2020-05-05 15:05:35.000000 radical.analytics-1.6.7/tests/no_barrier_data/rp.session.js-17-212.jetstream-cloud.org.vivek91.017401.0007/pmgr.launching.0.child.prof
+-rw-r--r--   0 mturilli   (501) staff       (20)      492 2020-05-05 15:05:35.000000 radical.analytics-1.6.7/tests/no_barrier_data/rp.session.js-17-212.jetstream-cloud.org.vivek91.017401.0007/pmgr.launching.0.prof
+-rw-r--r--   0 mturilli   (501) staff       (20)     1207 2020-05-05 15:05:35.000000 radical.analytics-1.6.7/tests/no_barrier_data/rp.session.js-17-212.jetstream-cloud.org.vivek91.017401.0007/rp.session.js-17-212.jetstream-cloud.org.vivek91.017401.0007.prof
+-rw-r--r--   0 mturilli   (501) staff       (20)  3768320 2020-05-05 15:05:35.000000 radical.analytics-1.6.7/tests/no_barrier_data/rp.session.js-17-212.jetstream-cloud.org.vivek91.017401.0007/umgr.0000.prof
+-rw-r--r--   0 mturilli   (501) staff       (20)   847228 2020-05-05 15:05:35.000000 radical.analytics-1.6.7/tests/no_barrier_data/rp.session.js-17-212.jetstream-cloud.org.vivek91.017401.0007/umgr.scheduling.0.child.prof
+-rw-r--r--   0 mturilli   (501) staff       (20)      149 2020-05-05 15:05:35.000000 radical.analytics-1.6.7/tests/no_barrier_data/rp.session.js-17-212.jetstream-cloud.org.vivek91.017401.0007/umgr.scheduling.0.prof
+-rw-r--r--   0 mturilli   (501) staff       (20)   756110 2020-05-05 15:05:35.000000 radical.analytics-1.6.7/tests/no_barrier_data/rp.session.js-17-212.jetstream-cloud.org.vivek91.017401.0007/umgr.staging.input.0.child.prof
+-rw-r--r--   0 mturilli   (501) staff       (20)      150 2020-05-05 15:05:35.000000 radical.analytics-1.6.7/tests/no_barrier_data/rp.session.js-17-212.jetstream-cloud.org.vivek91.017401.0007/umgr.staging.input.0.prof
+-rw-r--r--   0 mturilli   (501) staff       (20)   722324 2020-05-05 15:05:35.000000 radical.analytics-1.6.7/tests/no_barrier_data/rp.session.js-17-212.jetstream-cloud.org.vivek91.017401.0007/umgr.staging.output.0.child.prof
+-rw-r--r--   0 mturilli   (501) staff       (20)      153 2020-05-05 15:05:35.000000 radical.analytics-1.6.7/tests/no_barrier_data/rp.session.js-17-212.jetstream-cloud.org.vivek91.017401.0007/umgr.staging.output.0.prof
+-rw-r--r--   0 mturilli   (501) staff       (20)  8548352 2020-05-05 15:05:35.000000 radical.analytics-1.6.7/tests/no_barrier_data/rp.session.js-17-212.jetstream-cloud.org.vivek91.017401.0007/update.0.child.prof
+-rw-r--r--   0 mturilli   (501) staff       (20)      436 2020-05-05 15:05:35.000000 radical.analytics-1.6.7/tests/no_barrier_data/rp.session.js-17-212.jetstream-cloud.org.vivek91.017401.0007/update.0.prof
+-rw-r--r--   0 mturilli   (501) staff       (20)  3762696 2020-05-05 15:05:35.000000 radical.analytics-1.6.7/tests/no_barrier_data/rp.session.js-17-212.jetstream-cloud.org.vivek91.017401.0007.json
+-rw-r--r--   0 mturilli   (501) staff       (20)     6185 2020-08-11 13:34:20.000000 radical.analytics-1.6.7/tests/test_duration_method.py
+-rw-r--r--   0 mturilli   (501) staff       (20)    28947 2020-08-11 13:34:20.000000 radical.analytics-1.6.7/tests/test_entity.py
+-rw-r--r--   0 mturilli   (501) staff       (20)      277 2020-05-05 15:05:35.000000 radical.analytics-1.6.7/tests/test_session.py
```

### Comparing `radical_analytics-1.52.0/README.md` & `radical.analytics-1.6.7/README.md`

 * *Files identical despite different names*

### Comparing `radical_analytics-1.52.0/bin/radical-analytics-check` & `radical.analytics-1.6.7/bin/radical-analytics-check`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 __copyright__ = 'Copyright 2013-2016, http://radical.rutgers.edu'
 __license__   = 'MIT'
 
 
 import os
 import sys
-import pprint
 
 import radical.utils     as ru
 import radical.analytics as ra
 
 
 # ------------------------------------------------------------------------------
 #
@@ -69,15 +68,15 @@
 
     print()
     print('-----------------------------------------------------------')
     print('  source  : %s' % base)
     print('  session : %s' % sid)
     setypes = dict()
     states  = dict()
-    for p in session.get(etype=['rp', 'pmgr', 'tmgr']):
+    for p in session.get(etype=['rp', 'pmgr', 'umgr']):
         for e in p.events:
             t = e[ru.EVENT]
             if t not in setypes: setypes[t]  = 1
             else               : setypes[t] += 1
     for t in sorted(setypes.keys()):
         print('            %9d : %s' % (setypes[t], t))
         n_events += setypes[t]
@@ -137,15 +136,14 @@
     print('  total   : %9d  (%d types)' % (n_events, n_types))
 
     found   = list(setypes.keys()) \
             + list(petypes.keys()) \
             + list(uetypes.keys())
     missing = list()
     allkeys = sorted(all_events.keys())
-    unknown = [e for e in found if e not in all_events]
     for e in allkeys:
         if e not in found:
             missing.append(e)
 
     print()
     print('  missing:  %9d' % len(missing))
     for e in sorted(missing):
@@ -156,24 +154,14 @@
         else:
             # missing mandatory event
             c    = '*'
             ret += 1
 
         print('                  %s  %-20s : %s' % (c, e, all_events[e]))
     print()
-
-  # pprint.pprint(unknown)
-  # pprint.pprint(all_events)
-
-    print()
-    print('  unknown:  %9d' % len(unknown))
-    for e in sorted(unknown):
-        print('                   ! %-20s' % e)
-
-    print()
     print('-----------------------------------------------------------')
     print()
 
     sys.exit(ret)
 
 
 # ------------------------------------------------------------------------------
```

### Comparing `radical_analytics-1.52.0/bin/radical-analytics-inspect` & `radical.analytics-1.6.7/bin/radical-analytics-inspect`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 
                       A second plot is written for this analysis, containing
                       a histogramm of the observed durations per metric (TODO).
 
          concurrency: (\$sid.conc.png / \$sid.conc_hist.png)
                       Plot a selection of concurrency measures to gauge the
                       efficiency of execution.  Specifically, we plot the
-                      concurrency of tasks waiting to be scheduled (pending)
+                      concurrency of units waiting to be scheduled (pending)
                       and concurrency of execution (execute).  The x-axis shows
                       time, the y-axis shows the number of tasks which were in
                       a specific state (between two specific events) at that
                       point in time.
 
                       A second plot is written for this analysis, containing
                       a histogramm of the observed durations per metric (TODO).
```

### Comparing `radical_analytics-1.52.0/bin/radical-analytics-plot.py` & `radical.analytics-1.6.7/bin/radical-analytics-plot.py`

 * *Files identical despite different names*

### Comparing `radical_analytics-1.52.0/bin/radical-analytics-wrangler.py` & `radical.analytics-1.6.7/bin/radical-analytics-wrangler.py`

 * *Files identical despite different names*

### Comparing `radical_analytics-1.52.0/bin/rp_inspect/plot_conc.py` & `radical.analytics-1.6.7/bin/rp_inspect/plot_conc.py`

 * *Files identical despite different names*

### Comparing `radical_analytics-1.52.0/bin/rp_inspect/plot_dur.py` & `radical.analytics-1.6.7/bin/rp_inspect/plot_dur.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,16 +21,16 @@
 
 
 # We look into individual contributions of sub-durations to a larger duration.
 # The event list below will describe the whole duration (first to last event),
 # and the durations between subsequential events are considered contributing
 # sub-durations.  For each entity, we plot the times derived that way.
 #
-event_entities = ['task', 'master', 'worker']
-event_list     = [
+event_entity = 'task'
+event_list   = [
     # {ru.STATE: 'NEW'                          , ru.EVENT: 'state'           },
     # {ru.STATE: 'TMGR_SCHEDULING_PENDING'      , ru.EVENT: 'state'           },
     # {ru.STATE: 'TMGR_SCHEDULING'              , ru.EVENT: 'state'           },
     # {ru.STATE: 'TMGR_STAGING_INPUT_PENDING'   , ru.EVENT: 'state'           },
     # {ru.STATE: 'TMGR_STAGING_INPUT'           , ru.EVENT: 'state'           },
     # {ru.STATE: 'AGENT_STAGING_INPUT_PENDING'  , ru.EVENT: 'state'           },
     # {ru.STATE: None                           , ru.EVENT: 'get'             },
@@ -61,15 +61,15 @@
         sys.exit(1)
 
     src     = sys.argv[1]
     stype   = 'radical.pilot'
     session = ra.Session.create(src, stype)
     data    = dict()
 
-    for thing in session.get(etype=event_entities):
+    for thing in session.get(etype=event_entity):
 
         tstamps = list()
 
         for event in event_list:
             times = thing.timestamps(event=event)
             if times: tstamps.append(times[0])
             else    : tstamps.append(np.nan)
```

### Comparing `radical_analytics-1.52.0/bin/rp_inspect/plot_rate.py` & `radical.analytics-1.6.7/bin/rp_inspect/plot_rate.py`

 * *Files identical despite different names*

### Comparing `radical_analytics-1.52.0/bin/rp_inspect/plot_state.py` & `radical.analytics-1.6.7/bin/rp_inspect/plot_state.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 plt.style.use(ra.get_mplstyle("radical_mpl"))
 
 
 # We plot timelines for all events listed in `event_list` for all entities of
 # type `event_entity`..  Before plotting, we sort those entities by the
 # timestamp of the first event in the event list
 
-event_entities = ['task', 'master', 'worker']
+event_entity = 'task'
 event_list   = [
     # {ru.STATE: rp.NEW                         , ru.EVENT: 'state'          },
     # {ru.STATE: rp.TMGR_SCHEDULING_PENDING     , ru.EVENT: 'state'          },
     # {ru.STATE: rp.TMGR_SCHEDULING             , ru.EVENT: 'state'          },
     # {ru.STATE: rp.TMGR_STAGING_INPUT_PENDING  , ru.EVENT: 'state'          },
     # {ru.STATE: rp.TMGR_STAGING_INPUT          , ru.EVENT: 'state'          },
     # {ru.STATE: rp.AGENT_STAGING_INPUT_PENDING , ru.EVENT: 'state'          },
@@ -38,19 +38,19 @@
       {ru.STATE: rp.AGENT_SCHEDULING_PENDING    , ru.EVENT: 'state'          },
       {ru.STATE: rp.AGENT_SCHEDULING            , ru.EVENT: 'state'          },
     # {ru.STATE: None                           , ru.EVENT: 'schedule_ok'    },
       {ru.STATE: rp.AGENT_EXECUTING_PENDING     , ru.EVENT: 'state'          },
       {ru.STATE: rp.AGENT_EXECUTING             , ru.EVENT: 'state'          },
     # {ru.STATE: None                           , ru.EVENT: 'exec_mkdir'     },
     # {ru.STATE: None                           , ru.EVENT: 'exec_mkdir_done'},
-      {ru.STATE: None                           , ru.EVENT: 'exec_start'     },
+    # {ru.STATE: None                           , ru.EVENT: 'exec_start'     },
     # {ru.STATE: None                           , ru.EVENT: 'app_start'      },
     # {ru.STATE: None                           , ru.EVENT: 'app_stop'       },
     # {ru.STATE: None                           , ru.EVENT: 'exec_ok'        },
-      {ru.STATE: None                           , ru.EVENT: 'exec_stop'      },
+    # {ru.STATE: None                           , ru.EVENT: 'exec_stop'      },
       {ru.STATE: rp.AGENT_STAGING_OUTPUT_PENDING, ru.EVENT: 'state'          },
       {ru.STATE: rp.AGENT_STAGING_OUTPUT        , ru.EVENT: 'state'          },
     # {ru.STATE: rp.TMGR_STAGING_OUTPUT_PENDING , ru.EVENT: 'state'          },
     # {ru.STATE: rp.TMGR_STAGING_OUTPUT         , ru.EVENT: 'state'          },
     # {ru.STATE: rp.DONE                        , ru.EVENT: 'state'          },
 ]
 
@@ -66,15 +66,15 @@
     src     = sys.argv[1]
     stype   = 'radical.pilot'
     session = ra.Session.create(src, stype)
 
     data = dict()
     pipe = dict()
 
-    for thing in session.get(etype=event_entities):
+    for thing in session.get(etype=event_entity):
 
         tstamps = list()
 
         for event in event_list:
             times = thing.timestamps(event=event)
             if times: tstamps.append(times[0])
             else    : tstamps.append(None)
@@ -91,17 +91,17 @@
   #     diffs.append(data[uid][-1] - data[uid][0])
   # print(sorted(diffs))
 
 
   # sort x-axis (task IDs) by
   #     'uid'  : task ID
   #     'get'  : time of ingest
-  #     'sched': time of scheduling
+  #     'sched': time of sccheduling
   #     'pipe' : pipeline ID (RE sessions only)
-    order = 'sched'
+    order = 'AGENT_EXECUTING state'
     index = 4
 
     if order == 'uid':
         sorted_uids = sorted(pipe.keys())
     else:
         sorted_uids = [x[0] for x in sorted(list(data.items()),
                                             key=lambda v: v[1][index])]
```

### Comparing `radical_analytics-1.52.0/bin/rp_inspect/plot_util.py` & `radical.analytics-1.6.7/bin/rp_inspect/plot_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,39 +124,37 @@
     session   = ra.Session(src, stype=stype)
 
     # this script only works for one pilot
     pilots = session.get(etype='pilot')
     assert(len(pilots) == 1), len(pilots)
 
     sid     = session.uid
-    pilot   = pilots[0]
-    rm_info = pilot.cfg['resource_details']['rm_info']
-    p_zero  = pilot.timestamps(event={ru.EVENT: 'bootstrap_0_start'})[0]
-    p_size  = pilot.description['cores']
-    n_nodes = int(p_size / rm_info['cores_per_node'])
+    p_zero  = pilots[0].timestamps(event={ru.EVENT: 'bootstrap_0_start'})[0]
+    p_size  = pilots[0].description['cores']
+    n_nodes = int(p_size / pilots[0].cfg['cores_per_node'])
     n_tasks = len(session.get(etype='task'))
 
     legend = None
     rtypes = ['cpu', 'gpu']
     for i, rtype in enumerate(rtypes):
 
         # get utilization information
         prov, consumed, stats_abs, stats_rel, info = session.utilization(metrics, rtype)
 
-        with ru.ru_open('%s.stats' % sid, 'w') as fout:
+        with open('%s.stats' % sid, 'w') as fout:
             fout.write('\n%s\n\n' % info)
 
       # import pprint
       # pprint.pprint(prov)
       # pprint.pprint(consumed)
       # pprint.pprint(stats_abs)
       # pprint.pprint(stats_rel)
 
         legend, patches, x, y = ra.get_plot_utilization(metrics,
-                {sid: consumed}, p_zero, sid)
+                {sid: consumed}, p_zero, sid, 'pilot.0000')
 
         for patch in patches:
             axes[i].add_patch(patch)
 
         # Format axes
         axes[i].set_xlim([x['min'], x['max']])
         axes[i].set_ylim([y['min'], y['max']])
@@ -173,15 +171,16 @@
         ax.label_outer()
 
     # Title of the plot. Facultative, requires info about session
     # (see RA Info Chapter)
     axes[0].set_title(to_latex('%s Tasks - %s Nodes' % (n_tasks, n_nodes)))
 
     # Add legend for both plots
-    fig.legend(legend, [m[0] for m in metrics], ncol=3,
+    fig.legend([to_latex(l) for l in legend],
+               [m[0] for m in metrics], ncol=3,
                loc='upper center', bbox_to_anchor=(0.5, 1.10))
 
 
   # plt.xticks(list(range(int(x_min)-1, int(x_max)+1)))
     fig.savefig('%s_util.png' % sid, bbox_inches="tight")
   # plt.show()
```

### Comparing `radical_analytics-1.52.0/examples/00_session_describe_rp.py` & `radical.analytics-1.6.7/examples/00_session_describe_rp.py`

 * *Files identical despite different names*

### Comparing `radical_analytics-1.52.0/examples/01_session_list_rp.py` & `radical.analytics-1.6.7/examples/01_session_list_rp.py`

 * *Files identical despite different names*

### Comparing `radical_analytics-1.52.0/examples/02_session_get_rp.py` & `radical.analytics-1.6.7/examples/02_session_get_rp.py`

 * *Files identical despite different names*

### Comparing `radical_analytics-1.52.0/examples/03_session_filter_rp.py` & `radical.analytics-1.6.7/examples/03_session_filter_rp.py`

 * *Files identical despite different names*

### Comparing `radical_analytics-1.52.0/examples/04_session_duration_rp.py` & `radical.analytics-1.6.7/examples/04_session_duration_rp.py`

 * *Files identical despite different names*

### Comparing `radical_analytics-1.52.0/examples/05_relationsships.py` & `radical.analytics-1.6.7/examples/05_relationsships.py`

 * *Files identical despite different names*

### Comparing `radical_analytics-1.52.0/examples/06_events.py` & `radical.analytics-1.6.7/examples/06_events.py`

 * *Files identical despite different names*

### Comparing `radical_analytics-1.52.0/examples/06_ra_events.py` & `radical.analytics-1.6.7/examples/06_ra_events.py`

 * *Files identical despite different names*

### Comparing `radical_analytics-1.52.0/examples/07_event_timeline.py` & `radical.analytics-1.6.7/examples/07_event_timeline.py`

 * *Files identical despite different names*

### Comparing `radical_analytics-1.52.0/examples/08_core_utilization_plot.py` & `radical.analytics-1.6.7/examples/08_core_utilization_plot.py`

 * *Files identical despite different names*

### Comparing `radical_analytics-1.52.0/examples/08c_core_utilization_plot.py` & `radical.analytics-1.6.7/examples/08c_core_utilization_plot.py`

 * *Files identical despite different names*

### Comparing `radical_analytics-1.52.0/examples/09_session_plots.py` & `radical.analytics-1.6.7/examples/09_session_plots.py`

 * *Files identical despite different names*

### Comparing `radical_analytics-1.52.0/examples/10_durations.py` & `radical.analytics-1.6.7/examples/10_durations.py`

 * *Files identical despite different names*

### Comparing `radical_analytics-1.52.0/src/radical/analytics/__init__.py` & `radical.analytics-1.6.7/src/radical/analytics/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,35 +11,33 @@
 from .plotter    import Plotter
 
 # ------------------------------------------------------------------------------
 #
 from .utils import get_plotsize, get_mplstyle, stack_transitions
 from .utils import get_pilot_series, get_plot_utilization, get_pilots_zeros
 from .utils import to_latex
-from .utils import tabulate_durations
 
 
 # ------------------------------------------------------------------------------
 #
 import os
 import radical.utils as ru
 
 pwd  = os.path.dirname (__file__)
 root = "%s" % pwd
 version_short, version_detail, version_base, \
         version_branch, sdist_name, sdist_path = ru.get_version(paths=[root])
 version = version_short
 
-logger = ru.Logger('radical.analytics', targets=['-'])
+logger = ru.Logger('radical.analytics')
 logger.info('radical.analytics    version: %s' % version_detail)
 
 
 # ------------------------------------------------------------------------------
 #
 __all__ = ('Experiment','Session','Entity','Plotter', 'get_plotsize',
            'get_mplstyle', 'stack_transitions', 'get_pilot_series',
-           'get_plot_utilization', 'get_pilots_zeros', 'to_latex',
-           'tabulate_durations')
+           'get_plot_utilization', 'get_pilots_zeros', 'to_latex')
 
 
 # ------------------------------------------------------------------------------
```

### Comparing `radical_analytics-1.52.0/src/radical/analytics/entity.py` & `radical.analytics-1.6.7/src/radical/analytics/entity.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,48 +5,38 @@
 import radical.utils as ru
 
 
 # ------------------------------------------------------------------------------
 #
 class Entity(object):
 
-    def __init__(self, _uid, _profile, _details):
+    def __init__(self, _uid, _etype, _profile, _details):
         """
         Args:
-            uid (`str`): an ID assumed to be unique in the scope of an RA
+            uid (:obj:str): an ID assumed to be unique in the scope of an RA
                 Session
-            profile: a list of profile events for this entity
-            details: a dictionary of complementary information on this entity
+            etype (:obj:str): the type of the entity. This defines, amongst
+                others, what event model the session will assume to be valid for
+                this entity.
+            profile: .
+            details: .
         """
 
-        assert _uid
-        assert _profile
+        assert(_uid)
+        assert(_profile)
 
         self._uid         = _uid
+        self._etype       = _etype
         self._details     = _details
-        self._etype       = self._details.get('etype')
         self._description = self._details.get('description', dict())
         self._cfg         = self._details.get('cfg',         dict())
         self._resources   = self._details.get('resources',   dict())
 
-        # if have no etype tree information, guess the etype from uid
-        if not self._etype:
-            self._etype = self._uid.split('.')[0]
-
-        # FIXME: this should be sorted out on RP level
-        self._cfg['hostid'] = self._details.get('hostid')
-
-        # entities for which we have no tree information are raptor tasks (they
-        # were created by the master and never saw the client side)
         # FIXME: this should be sorted out on RP level
-        if not self._etype:
-            if not self._details and 'task' in self._uid:
-                self._etype = 'raptor.task'
-            else:
-                self._etype = 'unknown'
+        self._cfg['hostid'] = self._details['hostid']
 
         self._states      = dict()
         self._events      = list()
         self._consistency = {'log'         : list(),
                              'state_model' : None,
                              'event_model' : None,
                              'timestamps'  : None}
@@ -169,16 +159,16 @@
 
 
     # --------------------------------------------------------------------------
     #
     def _initialize(self, profile):
 
         # only call once
-        assert not self._states
-        assert not self._events
+        assert (not self._states)
+        assert (not self._events)
 
         if profile:
             self._t_start = sys.float_info.max
             self._t_stop  = sys.float_info.min
 
         # we expect each event tuple to have `time` and `event`, and expect
         # 'advance' events to signify a state transition.
@@ -271,17 +261,17 @@
 
         if not ranges:
             ranges = self.ranges(state, event, time)
           # print 'get %5d ranges for %s' % (len(ranges), self.uid)
           # pprint.pprint(self.events)
 
         else:
-            assert not state
-            assert not event
-            assert not time
+            assert(not state)
+            assert(not event)
+            assert(not time)
 
             # make sure the ranges are collapsed (although they likely are
             # already...)
           # print 'use %5d ranges for %s' % (len(ranges), self.uid)
             ranges = ru.collapse_ranges(ranges)
 
         if not ranges:
@@ -405,16 +395,16 @@
         Setting 'collapse' to 'True' (default) will prompt the method to
         collapse the resulting set of ranges.
 
         The returned ranges are time-sorted
 
         Example::
 
-           task.ranges(state=[rp.NEW, rp.FINAL]))
-           task.ranges(event=[{ru.NAME : 'exec_start'},
+           unit.ranges(state=[rp.NEW, rp.FINAL]))
+           unit.ranges(event=[{ru.NAME : 'exec_start'},
                               {ru.NAME : 'exec_ok'}])
         """
 
         # NOTE: this method relies on all state changes (as events in
         #       `self.states`) to also be recorded as events (as events in in
         #       `self.events` with `ru.NAME == 'state'`).
```

### Comparing `radical_analytics-1.52.0/src/radical/analytics/experiment.py` & `radical.analytics-1.6.7/src/radical/analytics/experiment.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,54 +1,39 @@
 
 from .session import Session
 
-from typing import List, Union
-
 
 # ------------------------------------------------------------------------------
 #
 class Experiment(object):
 
     # --------------------------------------------------------------------------
     #
-    def __init__(self, sessions: List[Union[str, Session]],
-                       stype: str = None):
+    def __init__(self, sources, stype):
         '''
         This class represents an RCT experiment, i.e., a series of RA sessions
         which are collectively analyzed.
 
-        `sessions` is expected to be either (1) a list of session source paths
-        pointing to tarballs or session directories, or (b) a list of
-        `ra.Session` instances.  The order of entries in the list determines the
-        default order used in plots etc.
+        `sources` is expected to be a list of tuples of session source paths
+        pointing to tarballs or session directories.  The order of tuples in the
+        list determines the default order used in plots etc.
 
-        The session type `stype` will be uniformely applied when reading session
-        data from provided paths.
+        The session type `stype` will be uniformely applied to all sessions.
         '''
 
         # FIXME: this is missing an abstraction: `Run`: a collection of sessions
         #         which share the same parameters and thus can be statistically
         #         handled together (means, std-deviation, etc).  Right now we
         #         only use this `Experiment` abstraction for non-statistical
         #         analysis (event plots, utilization plots, etc.)
 
         self._sessions = list()
 
-        if not sessions:
-            raise ValueError('cannot create experiments w/o sessions')
-
-        if isinstance(sessions[0], str):
-            for src in sessions:
-                assert isinstance(src, str)
-                self._sessions.append(Session.create(src=src, stype=stype))
-
-        else:
-            for session in sessions:
-                assert isinstance(session, Session)
-                self._sessions.append(session)
+        for src in sources:
+            self._sessions.append(Session.create(src=src, stype=stype))
 
 
     # --------------------------------------------------------------------------
     #
     @property
     def sessions(self):
         return self._sessions
@@ -100,18 +85,18 @@
                         ...
                     },
                     ...
                 },
                 ...
             }
 
-        `float` is always in tasks of `resource * time`, (think `core-hours`),
+        `float` is always in units of `resource * time`, (think `core-hours`),
         `list` is a list of 4-tuples `[t0, t1, r0, r1]` which signify at what
         specific time interval (`t0 to t1`) what specific resources (`r0 to r1`)
-        have been used.  The task of the resources are here dependent on the
+        have been used.  The unit of the resources are here dependent on the
         session type: only RP sessions are supported at the moment where those
         resource values are indexes in to the list of cores used in that
         specific session (offset over multiple pilots, if needed).
         '''
 
         # FIXME: the data structure documented above is not yet implemented
```

### Comparing `radical_analytics-1.52.0/src/radical/analytics/plotter.py` & `radical.analytics-1.6.7/src/radical/analytics/plotter.py`

 * *Files identical despite different names*

### Comparing `radical_analytics-1.52.0/src/radical/analytics/session.py` & `radical.analytics-1.6.7/src/radical/analytics/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 # pylint: disable=W0102,W0212
 
-import re
 import os
 import sys
 import copy
 import tarfile
 
 import pickle as pickle
 
@@ -34,24 +33,19 @@
         directory name.
 
         '''
 
         if _init:
             # if no sid is given, derive it from the src path
             sid, src, tgt, ext = self._get_sid(sid, src)
-
         else:
             assert sid
             assert src
             tgt = None
 
-        self._sid   = sid
-        self._src   = src
-        self._stype = stype
-
         if tgt and not os.path.exists(tgt):
 
             # need to extract
             print(('extract tarball to %s' % tgt))
             try:
                 if ext in ['tbz', 'tar.bz', 'tbz2', 'tar.bz2']:
                     tf = tarfile.open(name=src, mode='r:bz2')
@@ -62,16 +56,17 @@
                 else:
                     raise ValueError('cannot handle extension %s' % ext)
 
             except Exception as e:
                 raise RuntimeError(
                     'Cannot extract tarball: %s' % repr(e)) from e
 
-        if tgt:
-            self._src = tgt
+        self._sid   = sid
+        self._src   = src
+        self._stype = stype
 
       # print 'sid: %s [%s]' % (sid, stype)
       # print 'src: %s'      % src
 
         if stype == 'radical':
 
             # src is expected to point either to a single profile, or to
@@ -105,18 +100,17 @@
             try:
                 import radical.pilot.utils as rpu
             except Exception as e:
                 raise RuntimeError('radical.analytics requires the '
                                    'radical.pilot module to analyze this '
                                    'session - please install it.') from e
 
-            self._profile, accuracy, hostmap = \
-                    rpu.get_session_profile(sid=sid, src=self._src)
-            self._description = \
-                    rpu.get_session_description(sid=sid, src=self._src)
+            self._profile, accuracy, hostmap \
+                              = rpu.get_session_profile    (sid=sid, src=self._src)
+            self._description = rpu.get_session_description(sid=sid, src=self._src)
 
             self._description['accuracy'] = accuracy
             self._description['hostmap']  = hostmap
 
 
         elif stype == 'radical.entk':
 
@@ -181,15 +175,15 @@
             raise ValueError('src [%s] does not exist' % src)
 
         if os.path.isdir(src):
             pass
 
         elif os.path.isfile(src):
 
-            # src is a file - we assume its a tarball and extract it
+            # src is afile - we assume its a tarball and extract it
             if  src.endswith('.prof'):
                 # use as is
                 tgt = src
 
             elif src.endswith('.tgz') or \
                  src.endswith('.tbz')    :
                 tgt = src[:-4]
@@ -283,26 +277,25 @@
             # no caching
             session = Session(src, stype, sid, _entities, _init)
 
         try:
             with open(cache, 'rb') as fin:
                 data = fin.read()
                 session = pickle.loads(data)
-                print(('using cache for %s' % sid))
          #      import pprint
          #      j = ru.read_json("%s/%s.json" % (src, sid))
          #      rd = j['pilot'][0]['resource_details']
          #      session.get(etype='pilot')[0].cfg['resource_details'] = rd
          #      pprint.pprint(session.get(etype='pilot')[0].cfg)
          #  with open(cache, 'wb') as fout:
          #    # session = Session(src, stype, sid, _entities, _init)
          #      fout.write(pickle.dumps(session, protocol=pickle.HIGHEST_PROTOCOL))
 
-        except Exception:
-            print(('no cache for %s' % sid))
+        except Exception as e:
+            print(('cache read failed: %s' % e))
             with open(cache, 'wb') as fout:
                 session = Session(src, stype, sid, _entities, _init)
                 fout.write(pickle.dumps(session, protocol=pickle.HIGHEST_PROTOCOL))
 
         return session
 
 
@@ -375,35 +368,29 @@
         first part of any dot-separated uid to signify an entity type.
         '''
 
         # create entities from the profile events:
         entity_events = dict()
 
         for event in profile:
-
-            if event[ru.TIME] < -1:  # allow fow 1sec rounding error
-                raise ValueError('invalid time stamp: %s' % event)
-
             uid = event[ru.UID]
+
             if uid not in entity_events:
                 entity_events[uid] = list()
             entity_events[uid].append(event)
 
         # for all uids found,  create and store an entity.  We look up the
         # entity type in one of the events (and assume it is consistent over
         # all events for that uid)
         for uid,events in list(entity_events.items()):
+            etype   = events[0][ru.ENTITY]
             details = self._description.get('tree', dict()).get(uid, dict())
-
-            # hostid should be handled on RP level
-            hostid  = self._description.get('hostmap', dict()).get(uid)
-            if hostid:
-                details['hostid'] = hostid
-
+            details['hostid'] = self._description.get('hostmap', dict()).get(uid)
             self._entities[uid] = Entity(_uid=uid,
+                                         _etype=etype,
                                          _profile=events,
                                          _details=details)
 
 
     # --------------------------------------------------------------------------
     #
     def _initialize_properties(self):
@@ -480,48 +467,32 @@
     #
     def _apply_filter(self, etype=None, uid=None, state=None,
                             event=None, time=None):
 
         # iterate through all self._entities and collect UIDs of all entities
         # which match the given set of filters (after removing all events which
         # are not in the given time ranges)
-        etype = ru.as_list(etype)
-        uids  = ru.as_list(uid)
-        state = ru.as_list(state)
-        event = ru.as_list(event)
-        time  = ru.as_list(time )
+        if not etype: etype = list()
+        if not uid  : uid   = list()
+        if not state: state = list()
+        if not event: event = list()
+        if not time : time  = list()
+
+        if etype and not isinstance(etype, list): etype = [etype]
+        if uid   and not isinstance(uid  , list): uid   = [uid  ]
+        if state and not isinstance(state, list): state = [state]
+        if event and not isinstance(event, list): event = [event]
+
+        if time and len(time) and not isinstance(time[0], list): time = [time]
 
         ret = list()
-        for eid, entity in list(self._entities.items()):
+        for eid,entity in list(self._entities.items()):
 
             if etype and entity.etype not in etype: continue
-
-            if uids:
-                try:
-                    re_pattern = re.Pattern
-                except AttributeError:
-                    re_pattern = None
-                    self._log.warn('re.Pattern is not supported within this '
-                                   'python version')
-
-                keep = False
-                for uid in uids:
-                    if re_pattern and isinstance(uid, re_pattern):
-                        # uid is actually a regex we use for matching
-                        if uid.match(entity.uid):
-                            keep = True
-                            break
-                    else:
-                        # uid is a specific string to look out for
-                        if entity.uid == uid:
-                            keep = True
-                            break
-
-                if not keep:
-                    continue
+            if uid   and entity.uid   not in uid  : continue
 
             if state:
                 match = False
                 for s,stuple in list(entity.states.items()):
                     if time and not ru.in_range(stuple[ru.TIME], time):
                         continue
                     if s in state:
@@ -777,39 +748,39 @@
         and will use the `ranges()` method to obtain a set of ranges.  It will
         return the sum of the durations for all resulting & collapsed ranges.
 
         Example::
 
            session.duration(state=[rp.NEW, rp.FINAL]))
 
-        where `rp.FINAL` is a list of final task states.
+        where `rp.FINAL` is a list of final unit states.
         '''
 
         if not ranges:
             ranges = self.ranges(state, event, time)
 
         else:
-            assert not state
-            assert not event
-            assert not time
+            assert(not state)
+            assert(not event)
+            assert(not time)
 
             # make sure the ranges are collapsed (although they likely are
             # already...)
             ranges = ru.collapse_ranges(ranges)
 
         return sum(r[1] - r[0] for r in ranges)
 
 
     # --------------------------------------------------------------------------
     #
     def concurrency(self, state=None, event=None, time=None, sampling=None):
         '''
         This method accepts the same set of parameters as the `ranges()` method,
         and will use the `ranges()` method to obtain a set of ranges.  It will
-        return a time series, counting the number of tasks which are
+        return a time series, counting the number of units which are
         concurrently matching the ranges filter at any point in time.
 
         The additional parameter `sampling` determines the exact points in time
         for which the concurrency is computed, and thus determines the sampling
         rate for the returned time series.  If not specified, the time series
         will contain all points at which the concurrency changed.  If specified,
         it is interpreted as second (float) interval at which, after the
@@ -823,15 +794,15 @@
               ...
               [time_n, concurrency_n] ]
 
         where `time_n` is represented as `float`, and `concurrency_n` as `int`.
 
         Example::
 
-            session.filter(etype='task').concurrency(state=[rp.AGENT_EXECUTING,
+            session.filter(etype='unit').concurrency(state=[rp.AGENT_EXECUTING,
                 rp.AGENT_STAGING_OUTPUT_PENDING])
 
         '''
 
         INC =  1  # increase concurrency
         DEC = -1  # decrease concurrency
 
@@ -877,27 +848,24 @@
         if not sampling:
             # return as is
             ret = collapsed
 
         else:
             # select data points according to sampling
             # get min time, and create timestamps at regular intervals
-            t   = times[0][0]
-            v   = collapsed[0][1]
-            ret = list()
+            t     = times[0][0]
+            ret   = list()
             for time, val in collapsed:
                 while time >= t:
-                    ret.append([t, v])
+                    ret.append([t, val])
                     t += sampling
-                # value is changed after reaching the next timestamp
-                v = val
 
             # append last time stamp if it is not appended, yet
-            if ret[-1] != [t, v]:
-                ret.append([t, v])
+            if ret[-1] != [t, val]:
+                ret.append([t, val])
 
         return ret
 
 
     # --------------------------------------------------------------------------
     #
     def rate(self, state=None, event=None, time=None, sampling=None,
@@ -931,15 +899,15 @@
         constrain the resulting time series.
 
         The 'first' is defined, only the first matching event fir the selected
         entities is considered viable.
 
         Example::
 
-           session.filter(etype='task').rate(state=[rp.AGENT_EXECUTING])
+           session.filter(etype='unit').rate(state=[rp.AGENT_EXECUTING])
         '''
 
         timestamps = self.timestamps(event=event, state=state, time=time,
                                      first=first)
 
         if not timestamps:
             # nothing to do
@@ -1026,15 +994,15 @@
         stats_rel = {'total': 100.0}
         total     = 0.0
 
         for pid in provided['total']:
             for box in provided['total'][pid]:
                 stats_abs['total'] += (box[1] - box[0]) * \
                                       (box[3] - box[2]  + 1)
-        total = (max(stats_abs['total'], 1))
+        total = stats_abs['total']
 
         for metric in metrics:
             if isinstance(metric, list):
                 name  = metric[0]
                 parts = metric[1]
             else:
                 name  = metric
@@ -1046,15 +1014,15 @@
             for part in parts:
                 for uid in consumed[part]:
                     for box in consumed[part][uid]:
                         stats_abs[name] += (box[1] - box[0]) * \
                                            (box[3] - box[2]  + 1)
 
         info  = ''
-        info += '%s [%d]\n' % (self.uid, len(self.get(etype='task')))
+        info += '%s [%d]\n' % (self.uid, len(self.get(etype='unit')))
 
         for metric in metrics + ['total']:
             if isinstance(metric, list):
                 name  = metric[0]
                 parts = metric[1]
             else:
                 name  = metric
@@ -1142,15 +1110,15 @@
     #     where `time_n` is represented as `float`, `resource_utilization_n` as
     #     `int`, and resource_size is the total resources the owner has.
 
 
     #     Example::
 
     #         s.utilization(owner          = 'pilot',
-    #                       consumer       = 'task',
+    #                       consumer       = 'unit',
     #                       resource       = 'cores',
     #                       owner_events   = [{ru.EVENT: 'bootstrap_0_start'},
     #                                         {ru.EVENT: 'bootstrap_0_stop' }])
     #                       consumer_events= [{ru.EVENT: 'exec_start'},
     #                                         {ru.EVENT: 'exec_stop' }])
     #     '''
     #     ret = dict()
@@ -1343,24 +1311,24 @@
             use_entity (Entity): :class:`Entity` instance which uses resources
             use_events (list): event tuples which specify usage time
 
         Example::
 
             usage('pilot', [{ru.STATE: None, ru.EVENT: 'bootstrap_0_start'},
                             {ru.STATE: None, ru.EVENT: 'bootstrap_0_stop' }],
-                  'task' , [{ru.STATE: None, ru.EVENT: 'schedule_ok'      },
+                  'unit' , [{ru.STATE: None, ru.EVENT: 'schedule_ok'      },
                             {ru.STATE: None, ru.EVENT: 'unschedule_stop'  }],
-                  'task' , [{ru.STATE: None, ru.EVENT: 'exec_start'       },
+                  'unit' , [{ru.STATE: None, ru.EVENT: 'exec_start'       },
                             {ru.STATE: None, ru.EVENT: 'exec_stop'        }])
         '''
 
         # this is currently only supported for RP sessions, as we only know for
-        # pilots and tasks how to dig resource information out of session and
+        # pilots and units how to dig resource information out of session and
         # entity metadata.
-        assert self.stype == 'radical.pilot', \
+        assert(self.stype == 'radical.pilot'), \
                'stype %s unsupported' % self._stype
 
         # for RP sessions, create resource indices which can be used to
         # determine the y-axis values for the rectangles.  This is basically
         # a dict of node_names for each alloc_entity which points to two indexes
         # for each node: one starting index for GPUs, and one for CPU cores
         res_idx = dict()
@@ -1398,15 +1366,15 @@
               # import pprint
               # pprint.pprint(res_idx[entity.uid])
 
                 # we assume min/max to cover CPU and GPU
                 return [[[res_idx[entity.uid]['_min'],
                           res_idx[entity.uid]['_max']]], []]
 
-            elif entity.etype == 'task':
+            elif entity.etype == 'unit':
 
                 # find owning pilot
                 pid = entity.cfg.get('pilot')
                 if not pid:
                     # no resources used
                     return [[],[]]
```

### Comparing `radical_analytics-1.52.0/src/radical/analytics/utils/plot.py` & `radical.analytics-1.6.7/src/radical/analytics/utils/plot.py`

 * *Files 13% similar despite different names*

```diff
@@ -166,33 +166,21 @@
              series['cpu']['term'] = [[0.0, 0.0], [302.4374113082886, 100.0],
              [304.6761999130249, 0.0]].
     x      : dict
              Mix and max value of the X-axes.
 
     """
 
-    # get total pilot resources and runtime,
+    # get total pilot resources and runtime
     p_resrc = {'cpu': pilot.cfg['cores'],
                'gpu': pilot.cfg['gpus' ]}
 
-    t_min = None
-    t_max = None
+    t_min = pilot.timestamps(event={1: 'bootstrap_0_start'})[0]
+    t_max = pilot.timestamps(event={1: 'bootstrap_0_stop'})[0]
 
-    try   : t_min = pilot.timestamps(event={1: 'bootstrap_0_start'})[0]
-    except: pass
-
-    try   : t_max = pilot.timestamps(event={1: 'bootstrap_0_stop'})[0]
-    except: pass
-
-    # fallback for missing bootstrap events
-    if t_min is None: t_min = pilot.timestamps(state='PMGR_ACTIVE')[0]
-    if t_max is None: t_max = pilot.events[-1][ru.TIME]
-
-    assert t_min is not None
-    assert t_max is not None
 
     t_span = t_max - t_min
     x_min  = 0
     x_max  = t_span + 0.05 * t_span
 
     # derive the pilot resource transition points from the metrics. Metrics
     # might be pulled from rp.utils but should be consistent with those used for
@@ -209,51 +197,40 @@
     contribs = {r: {
                 m: [[0.0, 0.0]]
                    for m in metrics}
                 for r in resrc}
 
     for entity in session.get():
 
-        td    = entity.description
-        etype = entity.etype
+        uid = entity.uid
+        td  = entity.description
 
-        transitions = tmap.get(etype)
-        if not transitions:
-          # print('no transitions for %s: etype %s' % (entity.uid, etype))
+        # filter out worker ranks
+        if uid.count('.') > 1:
             continue
 
-      # print('\n', entity.uid, etype, sorted(set([e[1] for e in entity.events])))
-      # print()
+        transitions = tmap.get(entity.etype, [])
+        if not transitions:
+            continue
 
         for trans in transitions:
 
             event  = trans[0]
             p_from = trans[1]
             p_to   = trans[2]
 
             try:
-                t_resrc = {'cpu': entity.resources.get('cpu'),
-                           'gpu': entity.resources.get('gpu')}
-
-                # raptor tasks which were created in the master may not have
-                # resources defined, or may not even have a task description
-                # (they don't get an entry on MongoDB).  We thus guess their
-                # resource consumption here.
-                # NOTE: this can lead to underutilization to be reported!
-                if not t_resrc['cpu'] and 'task' in entity.uid:
+                t_resrc = {'cpu': entity.resources['cpu'],
+                           'gpu': entity.resources['gpu']}
+                if 'task' in entity.uid:
                     td = entity.description
-                    if not td.get('cpu_processes'):
-                        # guess
-                        t_resrc = {'cpu': 1, 'gpu': 0}
-                    else:
-                        cores = td['cpu_processes'] * td['cpu_threads']
-                        gpus  = td['cpu_processes'] * td['gpu_processes']
-                        t_resrc = {'cpu': cores,
-                                   'gpu': gpus}
-              # print(entity.uid, p_from, p_to, t_resrc)
+                    cores = td['cpu_processes'] * td['cpu_threads']
+                    gpus  = td['cpu_processes'] * td['gpu_processes']
+                    t_resrc = {'cpu': cores,
+                            'gpu': gpus}
 
             except Exception as e:
                 # if 'request' not in entity.uid:
                 #     print('guess resources for %s' % entity.uid)
 
                 # if 'pilot' in entity.uid:
                 #     t_resrc = {'cpu': 1024 * 40,
@@ -270,26 +247,26 @@
             # resources of 1 node.  We take those data from the pilot.
             if 'agent' in str(event):
                 t_resrc = {'cpu': pilot.cfg['cores_per_node'],
                            'gpu': pilot.cfg['gpus_per_node' ]}
 
             ts = entity.timestamps(event=event)
             if not ts:
-              # print('%s: no event %s for %s' % (uid, event, etype))
                 continue
 
             for r in resrc:
-                amount = t_resrc[r]
-                if amount == 0:
-                    continue
-                t = (ts[0] - t_min)
-                contribs[r][p_from].append([t, -amount])
-                contribs[r][p_to  ].append([t, +amount])
-              # print('%6.3f : %-30s : %-25s : %-15s --> %-15s [%s]' %
-              #         (t, uid, event, p_from, p_to,   amount))
+                try:
+                    amount = t_resrc[r]
+                    if amount == 0:
+                        continue
+                    t = (ts[0] - t_min)
+                    contribs[r][p_from].append([t, -amount])
+                    contribs[r][p_to  ].append([t, +amount])
+                except Exception:
+                    pass
 
     # we now have, for all metrics, a list of resource changes, in the form of
     #
     #   [timestamp, change]
     #
     # where the change can be positive or negative.  From this, we now calculate
     # the continuous time series for the metrics: for each metric, sort the
@@ -306,29 +283,22 @@
 
             for c in sorted(contribs[r][m]):
                 value += c[1]
                 # normalize to pilot resources to obtain percent
                 if p_resrc[r]:
                     if percent:
                         rel = value / p_resrc[r] * 100
-                      # print('rel', rel)
                         series[r][m].append([c[0], rel])
                     else:
                         series[r][m].append([c[0], value])
-                      # print('val %6.3f %-15s: %3d' % (c[0], m, value))
                 else:
                     series[r][m].append([c[0], 0])
 
     x = {'min': x_min, 'max': x_max}
 
-  # import pprint
-  # pprint.pprint(p_resrc)
-  # pprint.pprint(series)
-  # pprint.pprint(x)
-
     return p_resrc, series, x
 
 
 # ------------------------------------------------------------------------------
 #
 def get_pilots_zeros(ra_exp_obj):
     """Calculates when a set of pilots become available.
@@ -450,86 +420,31 @@
     return legend, patches, x, y
 
 
 # ------------------------------------------------------------------------------
 #
 def to_latex(data):
     '''
-    Transforms the input string(s) so that it can be used as latex compiled plot
-    label, title etc. Escapes special characters with a slash.
+    Transform the input string(s) so that it can be used as latex compiled plot
+    label, title etc.  This method escapes special characters with `\\`.
 
     Parameters
     ----------
     data : list or str
-           An individual string or a list of strings to transform.
+           an individual string or a list of strings to transform
 
     Returns
     -------
-    data : list of str
-           Transformed data.
+    data : transformed string
     '''
 
     if isinstance(data, list):
         return [to_latex(x) for x in data]
 
-    if isinstance(data, str):
-        return data.replace('%',  '\\%') \
-                   .replace('#',  '\\#') \
-                   .replace('_',  '\\_') \
-                   .replace('$',  '\\$') \
-                   .replace('&',  '\\&') \
-                   .replace('~',  '\\~') \
-                   .replace('^',  '\\^') \
-                   .replace('{',  '\\{') \
-                   .replace('}',  '\\}')
-
-    return to_latex(str(data))
+    else:
+        assert(isinstance(data, str)), type(data)
+        return data.replace('%', '\\%') \
+                   .replace('#', '\\#') \
+                   .replace('_', '\\_')
 
 
 # ------------------------------------------------------------------------------
-#
-def tabulate_durations(durations):
-    '''
-    Takes a dict of durations as defined in rp.utils (e.g.,
-    `rp.utils.PILOT_DURATIONS_DEBUG`) and returns a list of durations with their
-    start and stop timestamps. That list can be directly converted to a
-    panda.df.
-
-    Parameters
-    ----------
-    durations : dict
-                Dict of lists of dicts/lists of dicts. It contains
-                details about states and events.
-
-    Returns
-    -------
-    data : list
-           List of dicts, each dict containing 'Duration Name',
-           'Start Timestamp' and 'Stop Timestamp'.
-    '''
-    table = []
-    for name in durations:
-        duration = {}
-        start = durations[name][0]
-        stop  = durations[name][1]
-
-        duration['Duration Name'] = name
-
-        if list(start.values())[0] == 'state':
-            duration['Start Timestamp'] = list(start.values())[1]
-        else:
-            duration['Start Timestamp'] = list(start.values())[0]
-
-        if isinstance(stop, list):
-            ds = []
-            for state in stop:
-                ds.append(list(state.values())[1])
-            duration['Stop Timestamp'] = ', '.join(map(str, ds))
-        else:
-            if list(stop.values())[0] == 'state':
-                duration['Stop Timestamp'] = list(stop.values())[1]
-            else:
-                duration['Stop Timestamp'] = list(stop.values())[0]
-
-        table.append(duration)
-
-    return table
```

### Comparing `radical_analytics-1.52.0/styles/radical_mpl.txt` & `radical.analytics-1.6.7/styles/radical_mpl.txt`

 * *Files 1% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 axes.edgecolor              : .15
 axes.facecolor              : white
 axes.formatter.use_mathtext : True
 axes.grid                   : False
 axes.labelcolor             : .15
 axes.labelsize              : 8
 axes.linewidth              : .5
-axes.prop_cycle             : cycler('color', ['1a80b2', 'ff801a', '339933', 'cc3333', '9966b2', '804c4c', 'e680cc', 'b2b21a', '1ab2cc', '4c4c4c', '808080', '99b2b2', 'b2cce6', 'ffb280', '99e680', 'ff9999', 'ccb2cc', 'cc9999', 'ffb2cc', 'e6e699', '99e6e6', '666666', '998080', 'cccccc'])
+axes.prop_cycle             : cycler('color', ['1a80b2', 'b2cce6', 'ff801a', 'ffb280', '339933', '99e680', 'cc3333', 'ff9999', '9966b2', 'ccb2cc', '804c4c', 'cc9999', 'e680cc', 'ffb2cc', 'b2b21a', 'e6e699', '1ab2cc', '99e6e6', '4c4c4c', '666666', '808080', '998080', '99b2b2', 'cccccc'])
 axes.spines.right           : False
 axes.spines.top             : False
 axes.titlesize              : 8
 
 errorbar.capsize            : 3
 
 figure.titlesize            : 8
 figure.dpi                  : 300
 
-font.family                 : [DeJavu serif]
+font.family                 : [serif]
 font.serif                  : [Times New Roman]
 font.size                   : 8
 
 grid.color                  : .8
 grid.linestyle              : -
 grid.linewidth              : .1
```

### Comparing `radical_analytics-1.52.0/tests/test_duration_method.py` & `radical.analytics-1.6.7/tests/test_duration_method.py`

 * *Files identical despite different names*

### Comparing `radical_analytics-1.52.0/tests/test_entity.py` & `radical.analytics-1.6.7/tests/test_entity.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,36 +3,36 @@
 import json
 import pytest
 import radical.utils as ru
 from radical.analytics.entity import Entity
 
 
 # Test Directory use to load example json files
-base = "%s/example-data" % os.path.dirname(__file__)
+directory = "%s/example-data" % os.path.dirname(__file__)
 
 
 # ------------------------------------------------------------------------------
 #
 @pytest.fixture
 def pilot_entity():
     """Fixture to get the example Pilot entity from example data"""
 
-    with ru.ru_open("%s/pilot-entity-example.json" % base, 'r') as f:
+    with open("%s/pilot-entity-example.json" % directory, 'r') as f:
         entity = json.load(f)
         entity['events'] = [tuple(event) for event in entity['events']]
         return entity
 
 
 # ------------------------------------------------------------------------------
 #
 @pytest.fixture
 def range_entity():
     """Fixture to get the example range-testing entity from example data"""
 
-    with ru.ru_open("%s/range-testing-entity-example.json" % base, 'r') as f:
+    with open("%s/range-testing-entity-example.json" % directory, 'r') as f:
         entity = json.load(f)
         entity['events'] = [tuple(event) for event in entity['events']]
         return entity
 
 
 # ------------------------------------------------------------------------------
 #
@@ -66,291 +66,307 @@
 class TestEntity(object):
 
     # --------------------------------------------------------------------------
     #
     def test_t_start(self, pilot_entity):
         """Test a valid t_start"""
         e = Entity(_uid=pilot_entity['uid'],
+                   _etype=pilot_entity['etype'],
                    _profile=pilot_entity['events'],
                    _details=pilot_entity['details']
                    )
         events = sort_events(pilot_entity['events'])
 
         # Should match the time in the first element after sorting
-        assert e.t_start == events[0][ru.TIME]
+        assert(e.t_start == events[0][ru.TIME])
 
 
     # --------------------------------------------------------------------------
     #
     def test_t_stop(self, pilot_entity):
         """Test a valid t_stop"""
         e = Entity(_uid=pilot_entity['uid'],
+                   _etype=pilot_entity['etype'],
                    _profile=pilot_entity['events'],
                    _details=pilot_entity['details']
                    )
         events = sort_events(pilot_entity['events'])
 
         # Should match the time in the last element after sorting
-        assert events[-1][ru.TIME] == e.t_stop
+        assert(events[-1][ru.TIME] == e.t_stop)
 
 
     # --------------------------------------------------------------------------
     #
     def test_ttc(self, pilot_entity):
         """Test a valid ttc"""
         e = Entity(_uid=pilot_entity['uid'],
+                   _etype=pilot_entity['etype'],
                    _profile=pilot_entity['events'],
                    _details=pilot_entity['details']
                    )
         events = sort_events(pilot_entity['events'])
 
         # Should match the difference in time between
         # first and last elements after sorting
-        assert e.ttc == float(events[-1][ru.TIME] - events[0][ru.TIME])
+        assert(e.ttc == float(events[-1][ru.TIME] - events[0][ru.TIME]))
 
 
     # --------------------------------------------------------------------------
     #
     def test_t_range(self, pilot_entity):
         """Test a valid t_range"""
         e = Entity(_uid=pilot_entity['uid'],
+                   _etype=pilot_entity['etype'],
                    _profile=pilot_entity['events'],
                    _details=pilot_entity['details']
                    )
         events = sort_events(pilot_entity['events'])
 
         # Should match exactly what was passed in...
-        assert [events[0][ru.TIME], events[-1][ru.TIME]] == e.t_range
+        assert[events[0][ru.TIME], events[-1][ru.TIME]] == e.t_range
 
 
     # --------------------------------------------------------------------------
     #
     def test_uid(self, pilot_entity):
         """Test a valid uid"""
         e = Entity(_uid=pilot_entity['uid'],
+                   _etype=pilot_entity['etype'],
                    _profile=pilot_entity['events'],
                    _details=pilot_entity['details']
                    )
 
         # Should match exactly what was passed in...
-        assert e.uid == pilot_entity['uid']
+        assert(e.uid == pilot_entity['uid'])
 
 
     # --------------------------------------------------------------------------
     #
     def test_etype(self, pilot_entity):
         """Test a valid etype"""
         e = Entity(_uid=pilot_entity['uid'],
+                   _etype=pilot_entity['etype'],
                    _profile=pilot_entity['events'],
                    _details=pilot_entity['details']
                    )
 
         # Should match exactly what was passed in...
-        assert e.etype == pilot_entity['etype']
+        assert(e.etype == pilot_entity['etype'])
 
 
     # --------------------------------------------------------------------------
     #
     def test_states(self, pilot_entity):
         """Test a valid states"""
         e = Entity(_uid=pilot_entity['uid'],
+                   _etype=pilot_entity['etype'],
                    _profile=pilot_entity['events'],
                    _details=pilot_entity['details']
                    )
         # Get all events in the example file and put them in a dictionary
         states = get_states(pilot_entity['events'])
 
         # Should match a list of events of type 'state'
         # extracted from the events passed in
-        assert e.states == states
+        assert(e.states == states)
 
 
     # --------------------------------------------------------------------------
     #
     def test_events(self, pilot_entity):
         """Test a valid events"""
         e = Entity(_uid=pilot_entity['uid'],
+                   _etype=pilot_entity['etype'],
                    _profile=pilot_entity['events'],
                    _details=pilot_entity['details']
                    )
         # Get all events in order by timestamp
         events = sort_events(pilot_entity['events'])
 
         # Should match a list of sorted events (by the time field)
         # generated from the list of events passed in
-        assert e.events == events
+        assert(e.events == events)
 
 
     # --------------------------------------------------------------------------
     #
     def test_description(self, pilot_entity):
         """Test a valid description"""
         e = Entity(_uid=pilot_entity['uid'],
+                   _etype=pilot_entity['etype'],
                    _profile=pilot_entity['events'],
                    _details=pilot_entity['details']
                    )
 
         # Should match exactly what was passed in...
-        assert type(e.description) is dict
-        assert e.description == pilot_entity['details']['description']
+        assert(type(e.description) is dict)
+        assert(e.description == pilot_entity['details']['description'])
 
 
     # --------------------------------------------------------------------------
     #
     def test_cfg(self, pilot_entity):
         """Test a valid cfg"""
         e = Entity(_uid=pilot_entity['uid'],
+                   _etype=pilot_entity['etype'],
                    _profile=pilot_entity['events'],
                    _details=pilot_entity['details']
                    )
 
         # Should match exactly what was passed in...
-        assert type(e.cfg) is dict
-        assert e.cfg == pilot_entity['details']['cfg']
+        assert(type(e.cfg) is dict)
+        assert(e.cfg == pilot_entity['details']['cfg'])
 
 
     # --------------------------------------------------------------------------
     #
     def test_consistency(self, pilot_entity):
         """Test a valid consistency"""
         e = Entity(_uid=pilot_entity['uid'],
+                   _etype=pilot_entity['etype'],
                    _profile=pilot_entity['events'],
                    _details=pilot_entity['details']
                    )
 
         # TODO: Better matching, for now we match just a dict()
-        assert type(e.consistency) is dict
+        assert(type(e.consistency) is dict)
 
 
     # --------------------------------------------------------------------------
     #
     def test_as_dict(self, pilot_entity):
         """Test a valid as_dict"""
         e = Entity(_uid=pilot_entity['uid'],
+                   _etype=pilot_entity['etype'],
                    _profile=pilot_entity['events'],
                    _details=pilot_entity['details']
                    )
         expected = {
             'uid': pilot_entity['uid'],
             'etype': pilot_entity['etype'],
             'states': get_states(pilot_entity['events']),
             'events': sort_events(pilot_entity['events'])
         }
 
         # Should match exactly what was passed in
         # as the order seen above...
         # don't match `cfg` and `description` as those are runtime dependent
         edict = e.as_dict()
-        del edict['cfg']
-        del edict['description']
-        del edict['resources']
-        assert edict == expected
+        del(edict['cfg'])
+        del(edict['description'])
+        assert(edict == expected)
 
 
     ##############################################################
     # Test Ranges Method: expand=False, collapse=True
     #
     # We match range values form the example data at:
     #   ./example-data/range-testing-entity-example.json
     ##############################################################
 
     # --------------------------------------------------------------------------
     #
     def test_ranges_one_state(self, range_entity):
         """Test a valid ranges result with one state start/finish"""
         e = Entity(_uid=range_entity['uid'],
+                   _etype=range_entity['etype'],
                    _profile=range_entity['events'],
                    _details=range_entity['details']
                    )
 
         # Only one range of one start/end
         ranges = e.ranges(state=['PMGR_ACTIVE_PENDING', 'FAILED'])
-        assert ranges == [[21.668299913406372, 50.227399826049805]]
+        assert(ranges == [[21.668299913406372, 50.227399826049805]])
 
 
     # --------------------------------------------------------------------------
     #
     def test_ranges_two_consecutive_state(self, range_entity):
         """Test a valid ranges result with two states start/finish"""
         e = Entity(_uid=range_entity['uid'],
+                   _etype=range_entity['etype'],
                    _profile=range_entity['events'],
                    _details=range_entity['details']
                    )
 
         # Two consecutive ranges which get collapsed to the spanning max
         ranges = e.ranges(state=[['NEW',            'PMGR_ACTIVE'     ],
                                  ['PMGR_LAUNCHING', 'PMGR_ACTIVE_PENDING']])
-        assert ranges == [[0.0, 4.449499845504761]]
+        assert(ranges == [[0.0, 4.449499845504761]])
 
 
     # --------------------------------------------------------------------------
     #
     def test_ranges_time_filter_exact_match(self, range_entity):
         """Test a valid ranges with time filter, exact matches"""
         e = Entity(_uid=range_entity['uid'],
+                   _etype=range_entity['etype'],
                    _profile=range_entity['events'],
                    _details=range_entity['details']
                    )
 
         # for state
         ranges = e.ranges(state=[
             ['PMGR_ACTIVE_PENDING'],
             ['FAILED']
         ], time=[
             [21.668299913406372, 50.227399826049805]
         ])
-        assert ranges == [
+        assert(ranges == [
             [21.668299913406372, 50.227399826049805]
-        ]
+        ])
 
         # for events
         ranges = e.ranges(event=[
             [{ru.EVENT: 'put'}],
             [{ru.EVENT: 'sync_rel'}]
         ], time=[
             [4.446699857711792, 29.150099992752075]
         ])
-        assert ranges == [
+        assert(ranges == [
             [4.446699857711792, 29.150099992752075]
-        ]
+        ])
 
 
     # --------------------------------------------------------------------------
     #
     def test_ranges_time_filter_no_match(self, range_entity):
         """Test a valid ranges with time filter, exact matches"""
         e = Entity(_uid=range_entity['uid'],
+                   _etype=range_entity['etype'],
                    _profile=range_entity['events'],
                    _details=range_entity['details']
                    )
 
         # for state
         ranges = e.ranges(state=[
             ['PMGR_ACTIVE_PENDING'],
             ['FAILED']
         ], time=[
             [60.0, 70.0]
         ])
-        assert ranges == []
+        assert(ranges == [])
 
         # for events
         ranges = e.ranges(event=[
             [{ru.EVENT: 'put'}],
             [{ru.EVENT: 'sync_rel'}]
         ], time=[
             [30.0, 40.0]
         ])
-        assert ranges == []
+        assert(ranges == [])
 
 
     # --------------------------------------------------------------------------
     #
     def test_ranges_time_filter_intersection_match(self, range_entity):
         """Test a valid ranges with time filter, one intersection match each"""
         e = Entity(_uid=range_entity['uid'],
+                   _etype=range_entity['etype'],
                    _profile=range_entity['events'],
                    _details=range_entity['details']
                    )
 
         # As you read the tests, here is what each symbol represents:
         #   [      ] --> matched range before time filtering
         #   {      } --> time filtering value
@@ -359,98 +375,99 @@
         # Inner intersection: [   {(  )}   ]
         ranges = e.ranges(state=[
             ['PMGR_ACTIVE_PENDING'],
             ['FAILED']
         ], time=[
             [25.0, 30.0]
         ])
-        assert ranges == [
+        assert(ranges == [
             [25.0, 30.0]
-        ]
+        ])
 
         ranges = e.ranges(event=[
             [{ru.EVENT: 'put'}],
             [{ru.EVENT: 'sync_rel'}]
         ], time=[
             [5.0, 25.0]
         ])
-        assert ranges == [
+        assert(ranges == [
             [5.0, 25.0]
-        ]
+        ])
 
         # Outter intersection: {   ([    ])   }
         ranges = e.ranges(state=[
             ['PMGR_ACTIVE_PENDING'],
             ['FAILED']
         ], time=[
             [10.0, 60.0]
         ])
-        assert ranges == [
+        assert(ranges == [
             [21.668299913406372, 50.227399826049805]
-        ]
+        ])
 
         ranges = e.ranges(event=[
             [{ru.EVENT: 'put'}],
             [{ru.EVENT: 'sync_rel'}]
         ], time=[
             [0.0, 50.0]
         ])
-        assert ranges == [
+        assert(ranges == [
             [4.446699857711792, 29.150099992752075]
-        ]
+        ])
 
         # Right-side intersection match: {   ([   )}   ]
         ranges = e.ranges(state=[
             ['PMGR_ACTIVE_PENDING'],
             ['FAILED']
         ], time=[
             [25.0, 100.00]
         ])
-        assert ranges == [
+        assert(ranges == [
             [25.0, 50.227399826049805]
-        ]
+        ])
 
         ranges = e.ranges(event=[
             [{ru.EVENT: 'put'}],
             [{ru.EVENT: 'sync_rel'}]
         ], time=[
             [5.0, 50.0]
         ])
-        assert ranges == [
+        assert(ranges == [
             [5.0, 29.150099992752075]
-        ]
+        ])
 
         # Left-side intersection match: [   {(   ])   }
         ranges = e.ranges(state=[
             ['PMGR_ACTIVE_PENDING'],
             ['FAILED']
         ], time=[
             [0, 30.0]
         ])
-        assert ranges == [
+        assert(ranges == [
             [21.668299913406372, 30.0]
-        ]
+        ])
 
         ranges = e.ranges(event=[
             [{ru.EVENT: 'put'}],
             [{ru.EVENT: 'sync_rel'}]
         ], time=[
             [0.0, 25.0]
         ])
-        assert ranges == [
+        assert(ranges == [
             [4.446699857711792, 25.0]
-        ]
+        ])
 
 
     # --------------------------------------------------------------------------
     #
     def test_ranges_multi_time_filter_exact_match(self, range_entity):
         """Test a valid ranges with multiple time filters,
         exact matches only"""
         e = Entity(_uid=range_entity['uid'],
+                   _etype=range_entity['etype'],
                    _profile=range_entity['events'],
                    _details=range_entity['details']
                    )
 
         # As you read the tests, here is what each symbol represents:
         #   [      ] --> matched range before time filtering
         #   {      } --> time filter #1
@@ -462,327 +479,354 @@
         ranges = e.ranges(state=[
             ['PMGR_ACTIVE_PENDING'],
             ['FAILED']
         ], time=[
             [21.668299913406372, 50.227399826049805],
             [60.0, 80.0]
         ])
-        assert ranges == [
+        assert(ranges == [
             [21.668299913406372, 50.227399826049805]
-        ]
+        ])
 
         ranges = e.ranges(event=[
             [{ru.EVENT: 'put'}],
             [{ru.EVENT: 'sync_rel'}]
         ], time=[
             [4.446699857711792, 29.150099992752075],
             [30.0, 40.0]
         ])
-        assert ranges == [
+        assert(ranges == [
             [4.446699857711792, 29.150099992752075]
-        ]
+        ])
 
         # Only one of the filters match: {   }   |<[   ]>|
         ranges = e.ranges(state=[
             ['PMGR_ACTIVE_PENDING'],
             ['FAILED']
         ], time=[
             [60.0, 80.0],
             [21.668299913406372, 50.227399826049805]
         ])
-        assert ranges == [
+        assert(ranges == [
             [21.668299913406372, 50.227399826049805]
-        ]
+        ])
 
         ranges = e.ranges(event=[
             [{ru.EVENT: 'put'}],
             [{ru.EVENT: 'sync_rel'}]
         ], time=[
             [30.0, 40.0],
             [4.446699857711792, 29.150099992752075]
         ])
-        assert ranges == [
+        assert(ranges == [
             [4.446699857711792, 29.150099992752075]
-        ]
+        ])
 
 
     # --------------------------------------------------------------------------
     #
     def test_ranges_multi_time_filter_intersection_match(
             self, range_entity):
         """Test a valid ranges with multiple time filters,
             intersection matches each"""
         e = Entity(_uid=range_entity['uid'],
+                   _etype=range_entity['etype'],
                    _profile=range_entity['events'],
                    _details=range_entity['details']
                    )
 
-        assert e.t_start       ==  0
-        assert e.t_stop        ==     50.507999897003174
-        assert e.ttc           ==     50.507999897003174
-        assert e.t_range       == [0, 50.507999897003174]
-        assert len(e.list_states()) ==  6
-        assert len(e.states       ) ==  6
-        assert len(e.events       ) == 22
+        assert(e.t_start       ==  0)
+        assert(e.t_stop        ==     50.507999897003174)
+        assert(e.ttc           ==     50.507999897003174)
+        assert(e.t_range       == [0, 50.507999897003174])
+        assert(len(e.list_states()) ==  6)
+        assert(len(e.states       ) ==  6)
+        assert(len(e.events       ) == 22)
         # TODO: Add more assertions as needed
 
         # As you read the tests, here is what each symbol represents:
         #   [      ] --> matched range before time filtering
         #   {      } --> time filter #1
         #   |      | --> time filter #2
         #   (      ) --> matched range #1 *after* time filtering
         #   <      > --> matched range #2 *after* time filtering
 
         # Non-overlaping filters, one matches:    {([   )}   ]   |   |
         ranges = e.ranges(state=['PMGR_ACTIVE_PENDING', 'FAILED'],
                           time=[[21.668299913406372, 25.0], [60.0, 70.0]])
-        assert ranges == [[21.668299913406372, 25.0]]
+        assert(ranges == [[21.668299913406372, 25.0]])
 
         ranges = e.ranges(event=[{ru.EVENT: 'put'}, {ru.EVENT: 'sync_rel'}],
                           time=[[4.446699857711792, 15.0], [30.0, 50.0]
         ])
-        assert ranges == [[4.446699857711792, 15.0]]
+        assert(ranges == [[4.446699857711792, 15.0]])
 
         # Non-overlaping filters, both match: {   ([   )}   |<   ]>   |
         ranges = e.ranges(state=['PMGR_ACTIVE_PENDING', 'FAILED'],
                           time=[[10, 25.0], [30.0, 70.0]])
-        assert ranges == [[21.668299913406372, 25.0],
-                           [30.0, 50.227399826049805]]
+        assert(ranges == [[21.668299913406372, 25.0],
+                           [30.0, 50.227399826049805]])
 
         ranges = e.ranges(event=[{ru.EVENT: 'put'}, {ru.EVENT: 'sync_rel'}],
                           time=[[0.0, 15.0], [20.0, 30.0]])
-        assert ranges == [[4.446699857711792, 15.0],
-                           [20.0, 29.150099992752075]]
+        assert(ranges == [[4.446699857711792, 15.0],
+                           [20.0, 29.150099992752075]])
 
         # semi-overlaping filters, one matches: [   {(   ])   |   }   |
         ranges = e.ranges(state=['PMGR_ACTIVE_PENDING', 'FAILED'],
                           time=[[25.0, 70.0], [60.0, 80.0]])
-        assert ranges == [[25.0, 50.227399826049805]]
+        assert(ranges == [[25.0, 50.227399826049805]])
 
         ranges = e.ranges(event=[{ru.EVENT: 'put'}, {ru.EVENT: 'sync_rel'}],
                           time=[[15.0, 40.0], [30.0, 50.0]])
-        assert ranges == [[15.0, 29.150099992752075]]
+        assert(ranges == [[15.0, 29.150099992752075]])
 
         # semi-overlaping filters, both match: {   ([   |<   )}   ]>   |
         ranges = e.ranges(state=['PMGR_ACTIVE_PENDING', 'FAILED'],
                           time=[[10, 30.0], [25.0, 70.0]])
-        assert ranges == [[21.668299913406372, 50.227399826049805]]
+        assert(ranges == [[21.668299913406372, 50.227399826049805]])
 
         ranges = e.ranges(event=[{ru.EVENT: 'put'}, {ru.EVENT: 'sync_rel'}],
                           time=[[0.0, 20.0], [15.0, 30.0]])
-        assert ranges == [[4.446699857711792, 29.150099992752075]]
+        assert(ranges == [[4.446699857711792, 29.150099992752075]])
 
         # complete-overlap filters, both match: |   <[   {(   )}   ]>   |
         ranges = e.ranges(state=['PMGR_ACTIVE_PENDING', 'FAILED'],
                           time=[[25.0, 35.0], [10.0, 70.0]])
-        assert ranges == [[21.668299913406372, 50.227399826049805]]
+        assert(ranges == [[21.668299913406372, 50.227399826049805]])
 
         ranges = e.ranges(event=[{ru.EVENT: 'put'}, {ru.EVENT: 'sync_rel'}],
                           time=[[10.0, 20.0], [0.0, 30.0]])
-        assert ranges == [[4.446699857711792, 29.150099992752075]]
+        assert(ranges == [[4.446699857711792, 29.150099992752075]])
 
 
     # --------------------------------------------------------------------------
     #
     def test_ranges_two_overlaping_state(self, range_entity):
         e = Entity(_uid=range_entity['uid'],
+                   _etype=range_entity['etype'],
                    _profile=range_entity['events'],
                    _details=range_entity['details']
                    )
 
         # Two overlaping ranges
         ranges = e.ranges(state=[['NEW', 'PMGR_ACTIVE_PENDING'],
                                  ['PMGR_LAUNCHING', 'PMGR_ACTIVE']])
-        assert ranges == [[4.433599948883057, 4.449499845504761]]
+        assert(ranges == [[4.433599948883057, 4.449499845504761]])
 
 
     # --------------------------------------------------------------------------
     #
     def test_ranges_one_event(self, range_entity):
         e = Entity(_uid=range_entity['uid'],
+                   _etype=range_entity['etype'],
                    _profile=range_entity['events'],
                    _details=range_entity['details']
                    )
 
         # Only one range of one start/end
         ranges = e.ranges(event=[
             ({ru.EVENT: 'put'}),
             ({ru.EVENT: 'cmd'})
         ])
-        assert ranges == [
+        assert(ranges == [
             [4.446699857711792, 50.507999897003174]
-        ]
+        ])
 
 
     # --------------------------------------------------------------------------
     #
     def test_ranges_one_event_multi_match(self, range_entity):
         e = Entity(_uid=range_entity['uid'],
+                   _etype=range_entity['etype'],
                    _profile=range_entity['events'],
                    _details=range_entity['details']
                    )
 
         # Only one range of one start/end
         ranges = e.ranges(event=[
             ({ru.EVENT: 'update_request'}),
             ({ru.EVENT: 'update_pushed'})
         ])
-        assert ranges == [
+        assert(ranges == [
             [4.447200059890747 , 4.457900047302246],
             [4.458099842071533 , 5.236199855804443],
             [21.666899919509888, 21.685499906539917],
             [29.752099990844727, 29.939599990844727],
             [30.722899913787842, 32.28690004348755 ],
             [50.22889995574951 , 50.240999937057495]
-        ]
+        ])
 
 
     # --------------------------------------------------------------------------
     #
     def test_ranges_two_consecutive_event(self, range_entity):
         e = Entity(_uid=range_entity['uid'],
+                   _etype=range_entity['etype'],
                    _profile=range_entity['events'],
                    _details=range_entity['details']
                    )
 
         # Two consecutive ranges
         ranges = e.ranges(event=[
             [{ru.EVENT: 'put'     }, {ru.EVENT: 'hostname'}],
             [{ru.EVENT: 'sync_rel'}, {ru.EVENT: 'cmd'     }]
         ])
         print(ranges)
-        assert ranges == [[4.446699857711792, 29.150099992752075],
-                          [29.760799884796143, 50.507999897003174]]
+        assert(ranges == [[4.446699857711792, 29.150099992752075],
+                          [29.760799884796143, 50.507999897003174]])
 
 
     # --------------------------------------------------------------------------
     #
     def test_ranges_two_overlaping_event(self, range_entity):
         e = Entity(_uid=range_entity['uid'],
+                   _etype=range_entity['etype'],
                    _profile=range_entity['events'],
                    _details=range_entity['details']
                    )
 
         # FIXME: this is the same test as above
 
         # Two overlaping ranges
         ranges = e.ranges(event=[
             [{ru.EVENT: 'put'     }, {ru.EVENT: 'hostname'}],
             [{ru.EVENT: 'sync_rel'}, {ru.EVENT: 'cmd'     }]
         ])
-        assert ranges == [
+        assert(ranges == [
             [4.446699857711792, 29.150099992752075],
             [29.760799884796143, 50.507999897003174]
-        ]
+        ])
 
 
     # --------------------------------------------------------------------------
     #
     def test_empty_profile(self, pilot_entity):
 
         with pytest.raises(Exception):
             Entity(_uid=pilot_entity['uid'],
+                   _etype=pilot_entity['etype'],
                    _profile=list(),
                    _details=pilot_entity['details'])
 
 
+    # --------------------------------------------------------------------------
+    #
+    def test_empty_details(self, pilot_entity):
+
+        with pytest.raises(Exception):
+            Entity(_uid=pilot_entity['uid'],
+                   _etype=pilot_entity['etype'],
+                   _profile=pilot_entity['events'],
+                   _details=dict())
+
+
+
     ##############################################################
     # Test invalid scenarios
     ##############################################################
 
     # --------------------------------------------------------------------------
     #
     def test_none_uid(self, pilot_entity):
 
         with pytest.raises(Exception):
             Entity(_uid=None,
+                   _etype=pilot_entity['etype'],
                    _profile=pilot_entity['events'],
                    _details=pilot_entity['details']
                    )
 
 
     # --------------------------------------------------------------------------
     #
     def test_none_etype(self, pilot_entity):
 
         Entity(_uid=pilot_entity['uid'],
+               _etype=None,
                _profile=pilot_entity['events'],
                _details=pilot_entity['details']
                )
 
 
     # --------------------------------------------------------------------------
     #
     def test_none_profile(self, pilot_entity):
         with pytest.raises(Exception):
             Entity(_uid=None,
+                   _etype=pilot_entity['etype'],
                    _profile=None,
                    _details=pilot_entity['details']
                    )
 
 
     # --------------------------------------------------------------------------
     #
     def test_none_details(self, pilot_entity):
         with pytest.raises(Exception):
             Entity(_uid=pilot_entity['uid'],
+                   _etype=pilot_entity['etype'],
                    _profile=pilot_entity['events'],
                    _details=None
                    )
 
 
     # --------------------------------------------------------------------------
     #
     def test_invalid_ranges_no_end_matched_state(self, range_entity):
         e = Entity(_uid=range_entity['uid'],
+                   _etype=range_entity['etype'],
                    _profile=range_entity['events'],
                    _details=range_entity['details']
                    )
 
         # Only one range of one start/end
         ranges = e.ranges(event=[({ru.EVENT: 'put'}), ({ru.EVENT: 'aaa'})
         ])
-        assert ranges == []
+        assert(ranges == [])
 
 
     # --------------------------------------------------------------------------
     #
     def test_invalid_ranges_no_end_matched_event(self, range_entity):
         e = Entity(_uid=range_entity['uid'],
+                   _etype=range_entity['etype'],
                    _profile=range_entity['events'],
                    _details=range_entity['details']
                    )
 
         # Only one range of one start/end
         ranges = e.ranges(event=[('NEW'), ('AAA') ])
-        assert ranges == []
+        assert(ranges == [])
 
 
     # --------------------------------------------------------------------------
     #
     def test_invalid_ranges_no_start_matched_event(self, range_entity):
         e = Entity(_uid=range_entity['uid'],
+                   _etype=range_entity['etype'],
                    _profile=range_entity['events'],
                    _details=range_entity['details']
                    )
 
         # Only one range of one start/end
         ranges = e.ranges(event=[({ru.EVENT: 'aaa'}), ({ru.EVENT: 'put'})
         ])
-        assert ranges == []
+        assert(ranges == [])
 
 
     # --------------------------------------------------------------------------
     #
     def test_invalid_ranges_no_start_matched_state(self, range_entity):
         e = Entity(_uid=range_entity['uid'],
+                   _etype=range_entity['etype'],
                    _profile=range_entity['events'],
                    _details=range_entity['details']
                    )
 
         # Only one range of one start/end
         ranges = e.ranges(event=[('AAA'), ('NEW')])
-        assert ranges == []
+        assert(ranges == [])
 
 
 # ------------------------------------------------------------------------------
```

