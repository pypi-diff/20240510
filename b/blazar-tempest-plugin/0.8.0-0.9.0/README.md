# Comparing `tmp/blazar_tempest_plugin-0.8.0.tar.gz` & `tmp/blazar_tempest_plugin-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blazar_tempest_plugin-0.8.0.tar", last modified: Mon Mar 14 14:53:46 2022, max compression
+gzip compressed data, was "blazar_tempest_plugin-0.9.0.tar", last modified: Tue Sep 20 09:01:56 2022, max compression
```

## Comparing `blazar_tempest_plugin-0.8.0.tar` & `blazar_tempest_plugin-0.9.0.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-14 14:53:46.107601 blazar_tempest_plugin-0.8.0/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       82 2022-03-14 14:52:59.000000 blazar_tempest_plugin-0.8.0/.coveragerc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       89 2022-03-14 14:52:59.000000 blazar_tempest_plugin-0.8.0/.mailmap
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       61 2022-03-14 14:52:59.000000 blazar_tempest_plugin-0.8.0/.stestr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2409 2022-03-14 14:52:59.000000 blazar_tempest_plugin-0.8.0/.zuul.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      911 2022-03-14 14:53:45.000000 blazar_tempest_plugin-0.8.0/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      650 2022-03-14 14:52:59.000000 blazar_tempest_plugin-0.8.0/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2593 2022-03-14 14:53:45.000000 blazar_tempest_plugin-0.8.0/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      159 2022-03-14 14:52:59.000000 blazar_tempest_plugin-0.8.0/HACKING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2022-03-14 14:52:59.000000 blazar_tempest_plugin-0.8.0/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1325 2022-03-14 14:53:46.107601 blazar_tempest_plugin-0.8.0/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      391 2022-03-14 14:52:59.000000 blazar_tempest_plugin-0.8.0/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2022-03-14 14:52:59.000000 blazar_tempest_plugin-0.8.0/babel.cfg
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-14 14:53:46.103601 blazar_tempest_plugin-0.8.0/blazar_tempest_plugin/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      193 2022-03-14 14:52:59.000000 blazar_tempest_plugin-0.8.0/blazar_tempest_plugin/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-14 14:52:59.000000 blazar_tempest_plugin-0.8.0/blazar_tempest_plugin/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1765 2022-03-14 14:52:59.000000 blazar_tempest_plugin-0.8.0/blazar_tempest_plugin/config.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1752 2022-03-14 14:52:59.000000 blazar_tempest_plugin-0.8.0/blazar_tempest_plugin/plugin.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-14 14:53:46.103601 blazar_tempest_plugin-0.8.0/blazar_tempest_plugin/services/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-14 14:52:59.000000 blazar_tempest_plugin-0.8.0/blazar_tempest_plugin/services/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-14 14:53:46.103601 blazar_tempest_plugin-0.8.0/blazar_tempest_plugin/services/reservation/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-14 14:52:59.000000 blazar_tempest_plugin-0.8.0/blazar_tempest_plugin/services/reservation/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3302 2022-03-14 14:52:59.000000 blazar_tempest_plugin-0.8.0/blazar_tempest_plugin/services/reservation/reservation_client.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-14 14:53:46.103601 blazar_tempest_plugin-0.8.0/blazar_tempest_plugin/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-14 14:52:59.000000 blazar_tempest_plugin-0.8.0/blazar_tempest_plugin/tests/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-14 14:53:46.103601 blazar_tempest_plugin-0.8.0/blazar_tempest_plugin/tests/api/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-14 14:52:59.000000 blazar_tempest_plugin-0.8.0/blazar_tempest_plugin/tests/api/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1040 2022-03-14 14:52:59.000000 blazar_tempest_plugin-0.8.0/blazar_tempest_plugin/tests/api/fixtures.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-14 14:53:46.103601 blazar_tempest_plugin-0.8.0/blazar_tempest_plugin/tests/api/gabbits/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1799 2022-03-14 14:52:59.000000 blazar_tempest_plugin-0.8.0/blazar_tempest_plugin/tests/api/gabbits/allocations.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1076 2022-03-14 14:52:59.000000 blazar_tempest_plugin-0.8.0/blazar_tempest_plugin/tests/api/gabbits/hosts.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1433 2022-03-14 14:52:59.000000 blazar_tempest_plugin-0.8.0/blazar_tempest_plugin/tests/api/gabbits/leases.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1099 2022-03-14 14:52:59.000000 blazar_tempest_plugin-0.8.0/blazar_tempest_plugin/tests/api/test_blazar_api.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-14 14:53:46.103601 blazar_tempest_plugin-0.8.0/blazar_tempest_plugin/tests/scenario/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-14 14:52:59.000000 blazar_tempest_plugin-0.8.0/blazar_tempest_plugin/tests/scenario/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    27112 2022-03-14 14:52:59.000000 blazar_tempest_plugin-0.8.0/blazar_tempest_plugin/tests/scenario/manager_freeze.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5945 2022-03-14 14:52:59.000000 blazar_tempest_plugin-0.8.0/blazar_tempest_plugin/tests/scenario/resource_reservation_scenario.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12154 2022-03-14 14:52:59.000000 blazar_tempest_plugin-0.8.0/blazar_tempest_plugin/tests/scenario/test_host_reservation.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8494 2022-03-14 14:52:59.000000 blazar_tempest_plugin-0.8.0/blazar_tempest_plugin/tests/scenario/test_instance_reservation.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1645 2022-03-14 14:52:59.000000 blazar_tempest_plugin-0.8.0/blazar_tempest_plugin/tests/scenario/test_reservation_concurrency.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-14 14:53:46.103601 blazar_tempest_plugin-0.8.0/blazar_tempest_plugin.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1325 2022-03-14 14:53:45.000000 blazar_tempest_plugin-0.8.0/blazar_tempest_plugin.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1916 2022-03-14 14:53:46.000000 blazar_tempest_plugin-0.8.0/blazar_tempest_plugin.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2022-03-14 14:53:45.000000 blazar_tempest_plugin-0.8.0/blazar_tempest_plugin.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       88 2022-03-14 14:53:45.000000 blazar_tempest_plugin-0.8.0/blazar_tempest_plugin.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2022-03-14 14:53:45.000000 blazar_tempest_plugin-0.8.0/blazar_tempest_plugin.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2022-03-14 14:53:45.000000 blazar_tempest_plugin-0.8.0/blazar_tempest_plugin.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2022-03-14 14:53:45.000000 blazar_tempest_plugin-0.8.0/blazar_tempest_plugin.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       22 2022-03-14 14:53:45.000000 blazar_tempest_plugin-0.8.0/blazar_tempest_plugin.egg-info/top_level.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-14 14:53:46.103601 blazar_tempest_plugin-0.8.0/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       92 2022-03-14 14:52:59.000000 blazar_tempest_plugin-0.8.0/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-14 14:53:46.103601 blazar_tempest_plugin-0.8.0/doc/source/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2873 2022-03-14 14:52:59.000000 blazar_tempest_plugin-0.8.0/doc/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       75 2022-03-14 14:52:59.000000 blazar_tempest_plugin-0.8.0/doc/source/contributing.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      567 2022-03-14 14:52:59.000000 blazar_tempest_plugin-0.8.0/doc/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      386 2022-03-14 14:52:59.000000 blazar_tempest_plugin-0.8.0/doc/source/installation.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       30 2022-03-14 14:52:59.000000 blazar_tempest_plugin-0.8.0/doc/source/readme.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      480 2022-03-14 14:52:59.000000 blazar_tempest_plugin-0.8.0/doc/source/usage.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-14 14:53:46.099601 blazar_tempest_plugin-0.8.0/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-14 14:53:46.107601 blazar_tempest_plugin-0.8.0/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-14 14:52:59.000000 blazar_tempest_plugin-0.8.0/releasenotes/notes/.placeholder
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-14 14:53:46.107601 blazar_tempest_plugin-0.8.0/releasenotes/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-14 14:53:46.107601 blazar_tempest_plugin-0.8.0/releasenotes/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-14 14:52:59.000000 blazar_tempest_plugin-0.8.0/releasenotes/source/_static/.placeholder
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-14 14:53:46.107601 blazar_tempest_plugin-0.8.0/releasenotes/source/_templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-14 14:52:59.000000 blazar_tempest_plugin-0.8.0/releasenotes/source/_templates/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9274 2022-03-14 14:52:59.000000 blazar_tempest_plugin-0.8.0/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      172 2022-03-14 14:52:59.000000 blazar_tempest_plugin-0.8.0/releasenotes/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2022-03-14 14:52:59.000000 blazar_tempest_plugin-0.8.0/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      460 2022-03-14 14:52:59.000000 blazar_tempest_plugin-0.8.0/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      872 2022-03-14 14:53:46.107601 blazar_tempest_plugin-0.8.0/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1030 2022-03-14 14:52:59.000000 blazar_tempest_plugin-0.8.0/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      409 2022-03-14 14:52:59.000000 blazar_tempest_plugin-0.8.0/test-requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1574 2022-03-14 14:52:59.000000 blazar_tempest_plugin-0.8.0/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-20 09:01:56.055389 blazar_tempest_plugin-0.9.0/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       82 2022-09-20 09:01:13.000000 blazar_tempest_plugin-0.9.0/.coveragerc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       89 2022-09-20 09:01:13.000000 blazar_tempest_plugin-0.9.0/.mailmap
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       61 2022-09-20 09:01:13.000000 blazar_tempest_plugin-0.9.0/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2191 2022-09-20 09:01:13.000000 blazar_tempest_plugin-0.9.0/.zuul.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      911 2022-09-20 09:01:55.000000 blazar_tempest_plugin-0.9.0/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      650 2022-09-20 09:01:13.000000 blazar_tempest_plugin-0.9.0/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3013 2022-09-20 09:01:55.000000 blazar_tempest_plugin-0.9.0/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      159 2022-09-20 09:01:13.000000 blazar_tempest_plugin-0.9.0/HACKING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2022-09-20 09:01:13.000000 blazar_tempest_plugin-0.9.0/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1325 2022-09-20 09:01:56.055389 blazar_tempest_plugin-0.9.0/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      391 2022-09-20 09:01:13.000000 blazar_tempest_plugin-0.9.0/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2022-09-20 09:01:13.000000 blazar_tempest_plugin-0.9.0/babel.cfg
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-20 09:01:56.047389 blazar_tempest_plugin-0.9.0/blazar_tempest_plugin/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      193 2022-09-20 09:01:13.000000 blazar_tempest_plugin-0.9.0/blazar_tempest_plugin/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-20 09:01:13.000000 blazar_tempest_plugin-0.9.0/blazar_tempest_plugin/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1765 2022-09-20 09:01:13.000000 blazar_tempest_plugin-0.9.0/blazar_tempest_plugin/config.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1752 2022-09-20 09:01:13.000000 blazar_tempest_plugin-0.9.0/blazar_tempest_plugin/plugin.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-20 09:01:56.051389 blazar_tempest_plugin-0.9.0/blazar_tempest_plugin/services/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-20 09:01:13.000000 blazar_tempest_plugin-0.9.0/blazar_tempest_plugin/services/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-20 09:01:56.051389 blazar_tempest_plugin-0.9.0/blazar_tempest_plugin/services/reservation/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-20 09:01:13.000000 blazar_tempest_plugin-0.9.0/blazar_tempest_plugin/services/reservation/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3302 2022-09-20 09:01:13.000000 blazar_tempest_plugin-0.9.0/blazar_tempest_plugin/services/reservation/reservation_client.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-20 09:01:56.051389 blazar_tempest_plugin-0.9.0/blazar_tempest_plugin/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-20 09:01:13.000000 blazar_tempest_plugin-0.9.0/blazar_tempest_plugin/tests/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-20 09:01:56.051389 blazar_tempest_plugin-0.9.0/blazar_tempest_plugin/tests/api/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-20 09:01:13.000000 blazar_tempest_plugin-0.9.0/blazar_tempest_plugin/tests/api/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1040 2022-09-20 09:01:13.000000 blazar_tempest_plugin-0.9.0/blazar_tempest_plugin/tests/api/fixtures.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-20 09:01:56.051389 blazar_tempest_plugin-0.9.0/blazar_tempest_plugin/tests/api/gabbits/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1799 2022-09-20 09:01:13.000000 blazar_tempest_plugin-0.9.0/blazar_tempest_plugin/tests/api/gabbits/allocations.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1076 2022-09-20 09:01:13.000000 blazar_tempest_plugin-0.9.0/blazar_tempest_plugin/tests/api/gabbits/hosts.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1433 2022-09-20 09:01:13.000000 blazar_tempest_plugin-0.9.0/blazar_tempest_plugin/tests/api/gabbits/leases.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1099 2022-09-20 09:01:13.000000 blazar_tempest_plugin-0.9.0/blazar_tempest_plugin/tests/api/test_blazar_api.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-20 09:01:56.055389 blazar_tempest_plugin-0.9.0/blazar_tempest_plugin/tests/scenario/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-20 09:01:13.000000 blazar_tempest_plugin-0.9.0/blazar_tempest_plugin/tests/scenario/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      916 2022-09-20 09:01:13.000000 blazar_tempest_plugin-0.9.0/blazar_tempest_plugin/tests/scenario/manager_freeze.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5945 2022-09-20 09:01:13.000000 blazar_tempest_plugin-0.9.0/blazar_tempest_plugin/tests/scenario/resource_reservation_scenario.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12154 2022-09-20 09:01:13.000000 blazar_tempest_plugin-0.9.0/blazar_tempest_plugin/tests/scenario/test_host_reservation.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8494 2022-09-20 09:01:13.000000 blazar_tempest_plugin-0.9.0/blazar_tempest_plugin/tests/scenario/test_instance_reservation.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1645 2022-09-20 09:01:13.000000 blazar_tempest_plugin-0.9.0/blazar_tempest_plugin/tests/scenario/test_reservation_concurrency.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-20 09:01:56.051389 blazar_tempest_plugin-0.9.0/blazar_tempest_plugin.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1325 2022-09-20 09:01:55.000000 blazar_tempest_plugin-0.9.0/blazar_tempest_plugin.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1916 2022-09-20 09:01:56.000000 blazar_tempest_plugin-0.9.0/blazar_tempest_plugin.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2022-09-20 09:01:55.000000 blazar_tempest_plugin-0.9.0/blazar_tempest_plugin.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       88 2022-09-20 09:01:55.000000 blazar_tempest_plugin-0.9.0/blazar_tempest_plugin.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2022-09-20 09:01:55.000000 blazar_tempest_plugin-0.9.0/blazar_tempest_plugin.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2022-09-20 09:01:55.000000 blazar_tempest_plugin-0.9.0/blazar_tempest_plugin.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2022-09-20 09:01:55.000000 blazar_tempest_plugin-0.9.0/blazar_tempest_plugin.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       22 2022-09-20 09:01:55.000000 blazar_tempest_plugin-0.9.0/blazar_tempest_plugin.egg-info/top_level.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-20 09:01:56.055389 blazar_tempest_plugin-0.9.0/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       92 2022-09-20 09:01:13.000000 blazar_tempest_plugin-0.9.0/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-20 09:01:56.055389 blazar_tempest_plugin-0.9.0/doc/source/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2873 2022-09-20 09:01:13.000000 blazar_tempest_plugin-0.9.0/doc/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       75 2022-09-20 09:01:13.000000 blazar_tempest_plugin-0.9.0/doc/source/contributing.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      567 2022-09-20 09:01:13.000000 blazar_tempest_plugin-0.9.0/doc/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      386 2022-09-20 09:01:13.000000 blazar_tempest_plugin-0.9.0/doc/source/installation.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       30 2022-09-20 09:01:13.000000 blazar_tempest_plugin-0.9.0/doc/source/readme.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      480 2022-09-20 09:01:13.000000 blazar_tempest_plugin-0.9.0/doc/source/usage.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-20 09:01:56.043389 blazar_tempest_plugin-0.9.0/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-20 09:01:56.055389 blazar_tempest_plugin-0.9.0/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-20 09:01:13.000000 blazar_tempest_plugin-0.9.0/releasenotes/notes/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-20 09:01:56.055389 blazar_tempest_plugin-0.9.0/releasenotes/source/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-20 09:01:56.055389 blazar_tempest_plugin-0.9.0/releasenotes/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-20 09:01:13.000000 blazar_tempest_plugin-0.9.0/releasenotes/source/_static/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-20 09:01:56.055389 blazar_tempest_plugin-0.9.0/releasenotes/source/_templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-20 09:01:13.000000 blazar_tempest_plugin-0.9.0/releasenotes/source/_templates/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9274 2022-09-20 09:01:13.000000 blazar_tempest_plugin-0.9.0/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      172 2022-09-20 09:01:13.000000 blazar_tempest_plugin-0.9.0/releasenotes/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2022-09-20 09:01:13.000000 blazar_tempest_plugin-0.9.0/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      460 2022-09-20 09:01:13.000000 blazar_tempest_plugin-0.9.0/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      872 2022-09-20 09:01:56.059389 blazar_tempest_plugin-0.9.0/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1030 2022-09-20 09:01:13.000000 blazar_tempest_plugin-0.9.0/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      409 2022-09-20 09:01:13.000000 blazar_tempest_plugin-0.9.0/test-requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1574 2022-09-20 09:01:13.000000 blazar_tempest_plugin-0.9.0/tox.ini
```

### Comparing `blazar_tempest_plugin-0.8.0/.zuul.yaml` & `blazar_tempest_plugin-0.9.0/.zuul.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 - project:
+    queue: blazar
     templates:
       - tempest-plugin-jobs
       - check-requirements
       - publish-openstack-docs-pti
     check:
       jobs:
         - blazar-tempest-plugin-base
         - blazar-tempest-plugin-ipv6-only
+        - blazar-tempest-plugin-yoga
         - blazar-tempest-plugin-xena
         - blazar-tempest-plugin-wallaby
-        - blazar-tempest-plugin-victoria
-        - blazar-tempest-plugin-ussuri
     gate:
-      queue: blazar
       jobs:
         - blazar-tempest-plugin-base
 
 - job:
     name: blazar-tempest-plugin-base
     description: |
       This is a base devstack job for Blazar.
@@ -62,26 +61,20 @@
     vars: *blazar_base_vars
     irrelevant-files:
       - ^.*\.rst$
       - ^doc/.*$
       - ^releasenotes/.*$
 
 - job:
+    name: blazar-tempest-plugin-yoga
+    parent: blazar-tempest-plugin-base
+    override-checkout: stable/yoga
+
+- job:
     name: blazar-tempest-plugin-xena
     parent: blazar-tempest-plugin-base
     override-checkout: stable/xena
 
 - job:
     name: blazar-tempest-plugin-wallaby
     parent: blazar-tempest-plugin-base
     override-checkout: stable/wallaby
-
-- job:
-    name: blazar-tempest-plugin-victoria
-    parent: blazar-tempest-plugin-base
-    override-checkout: stable/victoria
-
-- job:
-    name: blazar-tempest-plugin-ussuri
-    parent: blazar-tempest-plugin-base
-    nodeset: openstack-single-node-bionic
-    override-checkout: stable/ussuri
```

### Comparing `blazar_tempest_plugin-0.8.0/AUTHORS` & `blazar_tempest_plugin-0.9.0/AUTHORS`

 * *Files identical despite different names*

### Comparing `blazar_tempest_plugin-0.8.0/CONTRIBUTING.rst` & `blazar_tempest_plugin-0.9.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `blazar_tempest_plugin-0.8.0/ChangeLog` & `blazar_tempest_plugin-0.9.0/ChangeLog`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,26 @@
 CHANGES
 =======
 
+0.9.0
+-----
+
+* Update minimal tempest version to 27.0.0
+* Remove setup\_clients method
+* Remove unused methods
+* [CI] Move queue setting to project level
+* Remove stable/victoria job from master gate
+* Update 'Maintained' stable branch jobs on master gate
+* Remove \_log\_console\_output, ping\_ip\_address methods
+* Remove create\_server and rebuild\_server methods
+
 0.8.0
 -----
 
+* Remove \_create\_port and create\_keypair methods
 * Remove create\_server\_snapshot method
 * Updating python testing classifier as per Yoga testing runtime
 * Add stable/xena jobs on master gate
 
 0.7.0
 -----
```

### Comparing `blazar_tempest_plugin-0.8.0/LICENSE` & `blazar_tempest_plugin-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `blazar_tempest_plugin-0.8.0/PKG-INFO` & `blazar_tempest_plugin-0.9.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: blazar_tempest_plugin
-Version: 0.8.0
+Version: 0.9.0
 Summary: Tempest plugin for Blazar Project
 Home-page: https://docs.openstack.org/blazar/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: =====================
         Blazar Tempest Plugin
```

### Comparing `blazar_tempest_plugin-0.8.0/blazar_tempest_plugin/config.py` & `blazar_tempest_plugin-0.9.0/blazar_tempest_plugin/config.py`

 * *Files identical despite different names*

### Comparing `blazar_tempest_plugin-0.8.0/blazar_tempest_plugin/plugin.py` & `blazar_tempest_plugin-0.9.0/blazar_tempest_plugin/plugin.py`

 * *Files identical despite different names*

### Comparing `blazar_tempest_plugin-0.8.0/blazar_tempest_plugin/services/reservation/reservation_client.py` & `blazar_tempest_plugin-0.9.0/blazar_tempest_plugin/services/reservation/reservation_client.py`

 * *Files identical despite different names*

### Comparing `blazar_tempest_plugin-0.8.0/blazar_tempest_plugin/tests/api/fixtures.py` & `blazar_tempest_plugin-0.9.0/blazar_tempest_plugin/tests/api/fixtures.py`

 * *Files identical despite different names*

### Comparing `blazar_tempest_plugin-0.8.0/blazar_tempest_plugin/tests/api/gabbits/allocations.yaml` & `blazar_tempest_plugin-0.9.0/blazar_tempest_plugin/tests/api/gabbits/allocations.yaml`

 * *Files identical despite different names*

### Comparing `blazar_tempest_plugin-0.8.0/blazar_tempest_plugin/tests/api/gabbits/hosts.yaml` & `blazar_tempest_plugin-0.9.0/blazar_tempest_plugin/tests/api/gabbits/hosts.yaml`

 * *Files identical despite different names*

### Comparing `blazar_tempest_plugin-0.8.0/blazar_tempest_plugin/tests/api/gabbits/leases.yaml` & `blazar_tempest_plugin-0.9.0/blazar_tempest_plugin/tests/api/gabbits/leases.yaml`

 * *Files identical despite different names*

### Comparing `blazar_tempest_plugin-0.8.0/blazar_tempest_plugin/tests/api/test_blazar_api.py` & `blazar_tempest_plugin-0.9.0/blazar_tempest_plugin/tests/api/test_blazar_api.py`

 * *Files identical despite different names*

### Comparing `blazar_tempest_plugin-0.8.0/blazar_tempest_plugin/tests/scenario/resource_reservation_scenario.py` & `blazar_tempest_plugin-0.9.0/blazar_tempest_plugin/tests/scenario/resource_reservation_scenario.py`

 * *Files identical despite different names*

### Comparing `blazar_tempest_plugin-0.8.0/blazar_tempest_plugin/tests/scenario/test_host_reservation.py` & `blazar_tempest_plugin-0.9.0/blazar_tempest_plugin/tests/scenario/test_host_reservation.py`

 * *Files identical despite different names*

### Comparing `blazar_tempest_plugin-0.8.0/blazar_tempest_plugin/tests/scenario/test_instance_reservation.py` & `blazar_tempest_plugin-0.9.0/blazar_tempest_plugin/tests/scenario/test_instance_reservation.py`

 * *Files identical despite different names*

### Comparing `blazar_tempest_plugin-0.8.0/blazar_tempest_plugin/tests/scenario/test_reservation_concurrency.py` & `blazar_tempest_plugin-0.9.0/blazar_tempest_plugin/tests/scenario/test_reservation_concurrency.py`

 * *Files identical despite different names*

### Comparing `blazar_tempest_plugin-0.8.0/blazar_tempest_plugin.egg-info/PKG-INFO` & `blazar_tempest_plugin-0.9.0/blazar_tempest_plugin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: blazar-tempest-plugin
-Version: 0.8.0
+Version: 0.9.0
 Summary: Tempest plugin for Blazar Project
 Home-page: https://docs.openstack.org/blazar/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: =====================
         Blazar Tempest Plugin
```

### Comparing `blazar_tempest_plugin-0.8.0/blazar_tempest_plugin.egg-info/SOURCES.txt` & `blazar_tempest_plugin-0.9.0/blazar_tempest_plugin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `blazar_tempest_plugin-0.8.0/doc/source/conf.py` & `blazar_tempest_plugin-0.9.0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `blazar_tempest_plugin-0.8.0/doc/source/index.rst` & `blazar_tempest_plugin-0.9.0/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `blazar_tempest_plugin-0.8.0/releasenotes/source/conf.py` & `blazar_tempest_plugin-0.9.0/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `blazar_tempest_plugin-0.8.0/setup.cfg` & `blazar_tempest_plugin-0.9.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `blazar_tempest_plugin-0.8.0/setup.py` & `blazar_tempest_plugin-0.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `blazar_tempest_plugin-0.8.0/tox.ini` & `blazar_tempest_plugin-0.9.0/tox.ini`

 * *Files identical despite different names*

