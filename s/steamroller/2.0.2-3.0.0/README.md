# Comparing `tmp/SteamRoller-2.0.2.tar.gz` & `tmp/steamroller-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SteamRoller-2.0.2.tar", last modified: Fri Sep 29 23:39:34 2023, max compression
+gzip compressed data, was "steamroller-3.0.0.tar", last modified: Fri May 10 14:16:59 2024, max compression
```

## Comparing `SteamRoller-2.0.2.tar` & `steamroller-3.0.0.tar`

### file list

```diff
@@ -1,13 +1,32 @@
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-09-29 23:39:34.024002 SteamRoller-2.0.2/
--rw-r--r--   0 tom       (1000) tom       (1000)      286 2023-09-29 23:39:34.024002 SteamRoller-2.0.2/PKG-INFO
--rw-r--r--   0 tom       (1000) tom       (1000)     3243 2022-06-21 15:46:52.000000 SteamRoller-2.0.2/README.rst
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-09-29 23:39:34.024002 SteamRoller-2.0.2/SteamRoller.egg-info/
--rw-r--r--   0 tom       (1000) tom       (1000)      286 2023-09-29 23:39:33.000000 SteamRoller-2.0.2/SteamRoller.egg-info/PKG-INFO
--rw-r--r--   0 tom       (1000) tom       (1000)      217 2023-09-29 23:39:33.000000 SteamRoller-2.0.2/SteamRoller.egg-info/SOURCES.txt
--rw-r--r--   0 tom       (1000) tom       (1000)        1 2023-09-29 23:39:33.000000 SteamRoller-2.0.2/SteamRoller.egg-info/dependency_links.txt
--rw-r--r--   0 tom       (1000) tom       (1000)       13 2023-09-29 23:39:33.000000 SteamRoller-2.0.2/SteamRoller.egg-info/requires.txt
--rw-r--r--   0 tom       (1000) tom       (1000)       12 2023-09-29 23:39:33.000000 SteamRoller-2.0.2/SteamRoller.egg-info/top_level.txt
--rw-r--r--   0 tom       (1000) tom       (1000)       38 2023-09-29 23:39:34.024002 SteamRoller-2.0.2/setup.cfg
--rw-r--r--   0 tom       (1000) tom       (1000)      441 2023-09-29 23:38:31.000000 SteamRoller-2.0.2/setup.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-09-29 23:39:34.024002 SteamRoller-2.0.2/steamroller/
--rw-r--r--   0 tom       (1000) tom       (1000)     8181 2023-09-29 23:38:31.000000 SteamRoller-2.0.2/steamroller/__init__.py
+drwxrwsr-x   0 tlippin1  (3111) tlippin1  (1538)        0 2024-05-10 14:16:59.284511 steamroller-3.0.0/
+-rw-rw-r--   0 tlippin1  (3111) tlippin1  (1538)    35149 2024-03-28 14:35:18.000000 steamroller-3.0.0/LICENSE
+-rw-r--r--   0 tlippin1  (3111) tlippin1  (1538)     5041 2024-05-10 14:16:59.284094 steamroller-3.0.0/PKG-INFO
+-rw-rw-r--   0 tlippin1  (3111) tlippin1  (1538)     4248 2024-05-10 14:16:52.000000 steamroller-3.0.0/README.rst
+-rw-rw-r--   0 tlippin1  (3111) tlippin1  (1538)     1085 2024-05-09 15:44:31.000000 steamroller-3.0.0/pyproject.toml
+-rw-rw-r--   0 tlippin1  (3111) tlippin1  (1538)       38 2024-05-10 14:16:59.284576 steamroller-3.0.0/setup.cfg
+-rw-rw-r--   0 tlippin1  (3111) tlippin1  (1538)      451 2024-03-28 14:35:18.000000 steamroller-3.0.0/setup.py
+drwxrwsr-x   0 tlippin1  (3111) tlippin1  (1538)        0 2024-05-10 14:16:59.273139 steamroller-3.0.0/src/
+drwxrwsr-x   0 tlippin1  (3111) tlippin1  (1538)        0 2024-05-10 14:16:59.276736 steamroller-3.0.0/src/steamroller/
+-rw-rw-r--   0 tlippin1  (3111) tlippin1  (1538)    10430 2024-05-10 00:45:41.000000 steamroller-3.0.0/src/steamroller/__init__.py
+drwxrwsr-x   0 tlippin1  (3111) tlippin1  (1538)        0 2024-05-10 14:16:59.281601 steamroller-3.0.0/src/steamroller/data/
+-rw-rw-r--   0 tlippin1  (3111) tlippin1  (1538)      546 2024-05-09 15:44:55.000000 steamroller-3.0.0/src/steamroller/data/apply_model.py
+-rw-rw-r--   0 tlippin1  (3111) tlippin1  (1538)      546 2024-05-09 15:44:55.000000 steamroller-3.0.0/src/steamroller/data/generate_report.py
+-rw-rw-r--   0 tlippin1  (3111) tlippin1  (1538)      546 2024-05-09 15:44:55.000000 steamroller-3.0.0/src/steamroller/data/preprocess_data.py
+-rw-rw-r--   0 tlippin1  (3111) tlippin1  (1538)      546 2024-05-09 15:44:55.000000 steamroller-3.0.0/src/steamroller/data/shuffle_data.py
+-rw-rw-r--   0 tlippin1  (3111) tlippin1  (1538)      546 2024-05-09 15:44:55.000000 steamroller-3.0.0/src/steamroller/data/train_model.py
+drwxrwsr-x   0 tlippin1  (3111) tlippin1  (1538)        0 2024-05-10 14:16:59.283616 steamroller-3.0.0/src/steamroller/engines/
+-rw-rw-r--   0 tlippin1  (3111) tlippin1  (1538)      558 2024-03-28 14:35:18.000000 steamroller-3.0.0/src/steamroller/engines/__init__.py
+-rw-rw-r--   0 tlippin1  (3111) tlippin1  (1538)     5621 2024-05-05 22:54:22.000000 steamroller-3.0.0/src/steamroller/engines/grid_engine.py
+-rw-rw-r--   0 tlippin1  (3111) tlippin1  (1538)      355 2024-04-29 13:42:48.000000 steamroller-3.0.0/src/steamroller/engines/local_engine.py
+-rw-rw-r--   0 tlippin1  (3111) tlippin1  (1538)     1971 2024-04-27 16:29:27.000000 steamroller-3.0.0/src/steamroller/engines/slurm.py
+-rw-rw-r--   0 tlippin1  (3111) tlippin1  (1538)     1651 2024-05-05 15:46:37.000000 steamroller-3.0.0/src/steamroller/engines/slurm_engine.py
+-rw-rw-r--   0 tlippin1  (3111) tlippin1  (1538)     1434 2024-03-28 16:38:50.000000 steamroller-3.0.0/src/steamroller/engines/univa_engine.py
+-rw-rw-r--   0 tlippin1  (3111) tlippin1  (1538)     1755 2024-05-09 14:11:32.000000 steamroller-3.0.0/src/steamroller/environment.py
+-rw-rw-r--   0 tlippin1  (3111) tlippin1  (1538)     4099 2024-04-27 17:43:40.000000 steamroller-3.0.0/src/steamroller/util.py
+drwxrwsr-x   0 tlippin1  (3111) tlippin1  (1538)        0 2024-05-10 14:16:59.280191 steamroller-3.0.0/src/steamroller.egg-info/
+-rw-r--r--   0 tlippin1  (3111) tlippin1  (1538)     5041 2024-05-10 14:16:59.277489 steamroller-3.0.0/src/steamroller.egg-info/PKG-INFO
+-rw-rw-r--   0 tlippin1  (3111) tlippin1  (1538)      778 2024-05-10 14:16:59.277896 steamroller-3.0.0/src/steamroller.egg-info/SOURCES.txt
+-rw-rw-r--   0 tlippin1  (3111) tlippin1  (1538)        1 2024-05-10 14:16:59.278273 steamroller-3.0.0/src/steamroller.egg-info/dependency_links.txt
+-rw-rw-r--   0 tlippin1  (3111) tlippin1  (1538)       49 2024-05-10 14:16:59.278641 steamroller-3.0.0/src/steamroller.egg-info/entry_points.txt
+-rw-rw-r--   0 tlippin1  (3111) tlippin1  (1538)       13 2024-05-10 14:16:59.279858 steamroller-3.0.0/src/steamroller.egg-info/requires.txt
+-rw-rw-r--   0 tlippin1  (3111) tlippin1  (1538)       12 2024-05-10 14:16:59.280246 steamroller-3.0.0/src/steamroller.egg-info/top_level.txt
```

