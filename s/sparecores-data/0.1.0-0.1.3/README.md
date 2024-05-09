# Comparing `tmp/sparecores-data-0.1.0.tar.gz` & `tmp/sparecores_data-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sparecores-data-0.1.0.tar", last modified: Mon Mar 25 13:55:13 2024, max compression
+gzip compressed data, was "sparecores_data-0.1.3.tar", last modified: Thu May  9 22:01:51 2024, max compression
```

## Comparing `sparecores-data-0.1.0.tar` & `sparecores_data-0.1.3.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 daroczig  (1000) daroczig  (1000)        0 2024-03-25 13:55:13.254927 sparecores-data-0.1.0/
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)    20131 2024-02-02 21:50:00.000000 sparecores-data-0.1.0/LICENSE
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)       26 2024-02-16 23:27:45.000000 sparecores-data-0.1.0/MANIFEST.in
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)     6781 2024-03-25 13:55:13.254927 sparecores-data-0.1.0/PKG-INFO
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)     5966 2024-03-25 13:52:23.000000 sparecores-data-0.1.0/README.md
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)     2672 2024-03-25 13:54:51.000000 sparecores-data-0.1.0/pyproject.toml
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)       38 2024-03-25 13:55:13.254927 sparecores-data-0.1.0/setup.cfg
-drwxr-xr-x   0 daroczig  (1000) daroczig  (1000)        0 2024-03-25 13:55:13.238260 sparecores-data-0.1.0/src/
-drwxr-xr-x   0 daroczig  (1000) daroczig  (1000)        0 2024-03-25 13:55:13.241593 sparecores-data-0.1.0/src/sc_data/
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)     1079 2024-03-15 13:42:54.000000 sparecores-data-0.1.0/src/sc_data/__init__.py
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)      474 2024-03-15 13:42:54.000000 sparecores-data-0.1.0/src/sc_data/constants.py
-drwxr-xr-x   0 daroczig  (1000) daroczig  (1000)        0 2024-03-25 13:55:13.241593 sparecores-data-0.1.0/src/sc_data/data/
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)       41 2024-02-23 08:46:40.000000 sparecores-data-0.1.0/src/sc_data/data/db_hash
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)  2113536 2024-02-23 08:46:40.000000 sparecores-data-0.1.0/src/sc_data/data/sc-data-all.db
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)     3189 2024-03-15 13:42:54.000000 sparecores-data-0.1.0/src/sc_data/data.py
-drwxr-xr-x   0 daroczig  (1000) daroczig  (1000)        0 2024-03-25 13:55:13.251593 sparecores-data-0.1.0/src/sparecores_data.egg-info/
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)     6781 2024-03-25 13:55:13.000000 sparecores-data-0.1.0/src/sparecores_data.egg-info/PKG-INFO
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)      403 2024-03-25 13:55:13.000000 sparecores-data-0.1.0/src/sparecores_data.egg-info/SOURCES.txt
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)        1 2024-03-25 13:55:13.000000 sparecores-data-0.1.0/src/sparecores_data.egg-info/dependency_links.txt
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)       80 2024-03-25 13:55:13.000000 sparecores-data-0.1.0/src/sparecores_data.egg-info/requires.txt
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)        8 2024-03-25 13:55:13.000000 sparecores-data-0.1.0/src/sparecores_data.egg-info/top_level.txt
-drwxr-xr-x   0 daroczig  (1000) daroczig  (1000)        0 2024-03-25 13:55:13.251593 sparecores-data-0.1.0/tests/
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)      544 2024-03-15 13:42:54.000000 sparecores-data-0.1.0/tests/test_data.py
+drwxr-xr-x   0 daroczig  (1000) daroczig  (1000)        0 2024-05-09 22:01:51.988234 sparecores_data-0.1.3/
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)    20131 2024-02-02 21:50:00.000000 sparecores_data-0.1.3/LICENSE
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)       26 2024-02-16 23:27:45.000000 sparecores_data-0.1.3/MANIFEST.in
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)     7137 2024-05-09 22:01:51.984901 sparecores_data-0.1.3/PKG-INFO
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)     6206 2024-03-25 23:54:50.000000 sparecores_data-0.1.3/README.md
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)     2798 2024-05-09 20:35:30.000000 sparecores_data-0.1.3/pyproject.toml
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)       38 2024-05-09 22:01:51.988234 sparecores_data-0.1.3/setup.cfg
+drwxr-xr-x   0 daroczig  (1000) daroczig  (1000)        0 2024-05-09 22:01:51.961567 sparecores_data-0.1.3/src/
+drwxr-xr-x   0 daroczig  (1000) daroczig  (1000)        0 2024-05-09 22:01:51.978234 sparecores_data-0.1.3/src/sc_data/
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)     1079 2024-03-15 13:42:54.000000 sparecores_data-0.1.3/src/sc_data/__init__.py
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)      480 2024-04-12 11:28:41.000000 sparecores_data-0.1.3/src/sc_data/constants.py
+drwxr-xr-x   0 daroczig  (1000) daroczig  (1000)        0 2024-05-09 22:01:51.981567 sparecores_data-0.1.3/src/sc_data/data/
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)      139 2024-04-12 17:08:12.000000 sparecores_data-0.1.3/src/sc_data/data/Pipfile
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)       41 2024-05-09 21:55:25.000000 sparecores_data-0.1.3/src/sc_data/data/db_hash
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)   487424 2024-05-09 19:49:14.000000 sparecores_data-0.1.3/src/sc_data/data/sc-data-priceless.db
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)     3325 2024-04-24 13:19:01.000000 sparecores_data-0.1.3/src/sc_data/data.py
+drwxr-xr-x   0 daroczig  (1000) daroczig  (1000)        0 2024-05-09 22:01:51.984901 sparecores_data-0.1.3/src/sparecores_data.egg-info/
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)     7137 2024-05-09 22:01:51.000000 sparecores_data-0.1.3/src/sparecores_data.egg-info/PKG-INFO
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)      434 2024-05-09 22:01:51.000000 sparecores_data-0.1.3/src/sparecores_data.egg-info/SOURCES.txt
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)        1 2024-05-09 22:01:51.000000 sparecores_data-0.1.3/src/sparecores_data.egg-info/dependency_links.txt
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)       80 2024-05-09 22:01:51.000000 sparecores_data-0.1.3/src/sparecores_data.egg-info/requires.txt
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)        8 2024-05-09 22:01:51.000000 sparecores_data-0.1.3/src/sparecores_data.egg-info/top_level.txt
+drwxr-xr-x   0 daroczig  (1000) daroczig  (1000)        0 2024-05-09 22:01:51.984901 sparecores_data-0.1.3/tests/
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)      544 2024-03-15 13:42:54.000000 sparecores_data-0.1.3/tests/test_data.py
```

### Comparing `sparecores-data-0.1.0/LICENSE` & `sparecores_data-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sparecores-data-0.1.0/PKG-INFO` & `sparecores_data-0.1.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: sparecores-data
-Version: 0.1.0
+Version: 0.1.3
 Summary: Structured data collected by sparecores-crawler.
 Author: Attila Nagy, Gergely Daroczi, Balazs Hodobay
 Maintainer-email: Spare Cores team <pkg@sparecores.com>
-Project-URL: Homepage, https://github.com/SpareCores/sc-data
-Project-URL: Issues, https://github.com/SpareCores/sc-data/issues
+Project-URL: repository, https://github.com/SpareCores/sc-data
+Project-URL: issues, https://github.com/SpareCores/sc-data/issues
+Project-URL: homepage, https://sparecores.com
+Keywords: cloud,compute,etl,sqlite,spot-instances,cost-optimization
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
@@ -19,18 +21,19 @@
 Requires-Dist: sqlalchemy; extra == "testing"
 Provides-Extra: all
 Requires-Dist: sparecores-data[testing]; extra == "all"
 
 ## Spare Cores Data
 
 [![Build](https://img.shields.io/github/actions/workflow/status/SpareCores/sc-data/tests.yaml)](https://github.com/SpareCores/sc-data/actions/workflows/tests.yaml)
+[![Last Run](https://img.shields.io/endpoint?url=https%3A%2F%2Fsc-data-lastrun-mcjxzakwph52.runkit.sh)](https://github.com/SpareCores/sc-data/actions/workflows/crawl-spot.yaml)<!-- provided by https://runkit.com/daroczig/sc-data-lastrun -->
 <picture><source media="(prefers-color-scheme: dark)" srcset="https://img.shields.io/badge/status-alpha-blue"><source media="(prefers-color-scheme: light)" srcset="https://img.shields.io/badge/status-alpha-blue"><img alt="Project Status: Alpha" src="https://img.shields.io/badge/status-alpha-blue"></picture>
 <picture><source media="(prefers-color-scheme: dark)" srcset="https://img.shields.io/maintenance/yes/2024"><source media="(prefers-color-scheme: light)" srcset="https://img.shields.io/maintenance/yes/2024"><img alt="Maintenance Status: Active" src="https://img.shields.io/maintenance/yes/2024"></picture>
 [![CC-BY-SA 4.0 License](https://img.shields.io/github/license/SpareCores/sc-data)](https://github.com/SpareCores/sc-data/blob/main/LICENSE)
-[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/sc_data?logo=python&logoColor=ffdd54)](https://pypi.org/project/sparecores-data/)
+[![PyPI - Python Version](https://img.shields.io/pypi/v/sparecores-data?logo=python&logoColor=ffdd54)](https://pypi.org/project/sparecores-data/)
 [![NGI Search Open Call 3 beneficiary](https://img.shields.io/badge/NGI%20Search-Open%20Call%20%233-blue?logo=data:image/svg+xml;base64,PD94bWwgdmVyc2lvbj0iMS4wIiBlbmNvZGluZz0idXRmLTgiPz4NCjwhLS0gR2VuZXJhdG9yOiBBZG9iZSBJbGx1c3RyYXRvciAyMi4xLjAsIFNWRyBFeHBvcnQgUGx1Zy1JbiAuIFNWRyBWZXJzaW9uOiA2LjAwIEJ1aWxkIDApICAtLT4NCjxzdmcgdmVyc2lvbj0iMS4xIiBpZD0iTGF5ZXJfMSIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIiB4bWxuczp4bGluaz0iaHR0cDovL3d3dy53My5vcmcvMTk5OS94bGluayIgeD0iMHB4IiB5PSIwcHgiDQoJIHdpZHRoPSIxODBweCIgaGVpZ2h0PSIxODBweCIgdmlld0JveD0iMCAwIDE4MCAxODAiIHN0eWxlPSJlbmFibGUtYmFja2dyb3VuZDpuZXcgMCAwIDE4MCAxODA7IiB4bWw6c3BhY2U9InByZXNlcnZlIj4NCjxzdHlsZSB0eXBlPSJ0ZXh0L2NzcyI+DQoJLnN0MHtjbGlwLXBhdGg6dXJsKCNTVkdJRF8yXyk7fQ0KCS5zdDF7Y2xpcC1wYXRoOnVybCgjU1ZHSURfNF8pO2ZpbGw6dXJsKCNTVkdJRF81Xyk7fQ0KCS5zdDJ7ZmlsbDp1cmwoI1NWR0lEXzZfKTt9DQoJLnN0M3tmaWxsOiNGRkZGRkY7fQ0KPC9zdHlsZT4NCjxnPg0KCTxnPg0KCQk8ZGVmcz4NCgkJCTxwYXRoIGlkPSJTVkdJRF8xXyIgZD0iTTkwLDVDNDMuMiw1LDUsNDMuMiw1LDkwdjBjMCw0Ni43LDM4LjIsODUsODUsODVoMGM0Ni43LDAsODUtMzguMiw4NS04NXYwQzE3NSw0My4yLDEzNi44LDUsOTAsNUw5MCw1eiINCgkJCQkvPg0KCQk8L2RlZnM+DQoJCTxjbGlwUGF0aCBpZD0iU1ZHSURfMl8iPg0KCQkJPHVzZSB4bGluazpocmVmPSIjU1ZHSURfMV8iICBzdHlsZT0ib3ZlcmZsb3c6dmlzaWJsZTsiLz4NCgkJPC9jbGlwUGF0aD4NCgkJPGcgY2xhc3M9InN0MCI+DQoJCQk8Zz4NCgkJCQk8ZGVmcz4NCgkJCQkJPHJlY3QgaWQ9IlNWR0lEXzNfIiB3aWR0aD0iMTgwIiBoZWlnaHQ9IjE4MCIvPg0KCQkJCTwvZGVmcz4NCgkJCQk8Y2xpcFBhdGggaWQ9IlNWR0lEXzRfIj4NCgkJCQkJPHVzZSB4bGluazpocmVmPSIjU1ZHSURfM18iICBzdHlsZT0ib3ZlcmZsb3c6dmlzaWJsZTsiLz4NCgkJCQk8L2NsaXBQYXRoPg0KCQkJCQ0KCQkJCQk8bGluZWFyR3JhZGllbnQgaWQ9IlNWR0lEXzVfIiBncmFkaWVudFVuaXRzPSJ1c2VyU3BhY2VPblVzZSIgeDE9Ii0zMjQuNTY0MyIgeTE9IjIxMi4yNTg1IiB4Mj0iLTMyMy4zOTAzIiB5Mj0iMjEyLjI1ODUiIGdyYWRpZW50VHJhbnNmb3JtPSJtYXRyaXgoLTE1NS40ODE5IDE1MS4wOTY2IC0xNTEuMDk2NiAtMTU1LjQ4MTkgLTE4MjExLjA1ODYgODIwNDQuMjI2NikiPg0KCQkJCQk8c3RvcCAgb2Zmc2V0PSIwIiBzdHlsZT0ic3RvcC1jb2xvcjojRTUzNTAwIi8+DQoJCQkJCTxzdG9wICBvZmZzZXQ9IjEiIHN0eWxlPSJzdG9wLWNvbG9yOiM1MDAwMkQiLz4NCgkJCQk8L2xpbmVhckdyYWRpZW50Pg0KCQkJCTxwb2x5Z29uIGNsYXNzPSJzdDEiIHBvaW50cz0iMjcwLDkyLjYgODcuNCwyNzAgLTkwLDg3LjQgOTIuNiwtOTAgCQkJCSIvPg0KCQkJPC9nPg0KCQk8L2c+DQoJCTxnIGNsYXNzPSJzdDAiPg0KCQkJDQoJCQkJPGxpbmVhckdyYWRpZW50IGlkPSJTVkdJRF82XyIgZ3JhZGllbnRVbml0cz0idXNlclNwYWNlT25Vc2UiIHgxPSItMzM3Ljg2MDYiIHkxPSIxOTguNzY1NSIgeDI9Ii0zMzguMzY1MiIgeTI9IjE5OC43NzI3IiBncmFkaWVudFRyYW5zZm9ybT0ibWF0cml4KC0xMjEuNzc5NCAxMTguMzQ0NiAtMTE4LjM0NDYgLTEyMS43Nzk0IC0xNzU2MS45Mzc1IDY0MzA5LjgxMjUpIj4NCgkJCQk8c3RvcCAgb2Zmc2V0PSIwIiBzdHlsZT0ic3RvcC1jb2xvcjojNTAwMDJEIi8+DQoJCQkJPHN0b3AgIG9mZnNldD0iMSIgc3R5bGU9InN0b3AtY29sb3I6I0U1MzUwMCIvPg0KCQkJPC9saW5lYXJHcmFkaWVudD4NCgkJCTxwYXRoIGNsYXNzPSJzdDIiIGQ9Ik0xMDUuNiw4OC4yVjYzLjhjMC00LjMsMy41LTcuOCw3LjgtNy44aDBjNC4zLDAsNy44LDMuNSw3LjgsNy44djUyLjRjMCw0LjMtMy41LDcuOC03LjgsNy44aC0xLjUNCgkJCQljLTIuMywwLTQuNS0xLTYtMi44TDgwLjEsODkuN2MtMS45LTIuMy01LjctMS01LjcsMnYyNC41YzAsNC4zLTMuNSw3LjgtNy44LDcuOHMtNy44LTMuNS03LjgtNy44VjYzLjhjMC00LjMsMy41LTcuOCw3LjgtNy44DQoJCQkJaDEuNmMyLjMsMCw0LjUsMSw2LDIuOGwyNS43LDMxLjRDMTAxLjgsOTIuNiwxMDUuNiw5MS4zLDEwNS42LDg4LjJ6Ii8+DQoJCQk8cGF0aCBjbGFzcz0ic3QzIiBkPSJNNjguMiw1NmgtMS42Yy00LjMsMC03LjgsMy41LTcuOCw3Ljh2NTIuNGMwLDQuMywzLjUsNy44LDcuOCw3LjhzNy44LTMuNSw3LjgtNy44VjkxLjdjMC0zLDMuOC00LjQsNS43LTINCgkJCQlsMjUuOCwzMS41YzEuNSwxLjgsMy43LDIuOCw2LDIuOGgxLjVjNC4zLDAsNy44LTMuNSw3LjgtNy44VjYzLjhjMC00LjMtMy41LTcuOC03LjgtNy44aDBjLTQuMywwLTcuOCwzLjUtNy44LDcuOHYyNC41DQoJCQkJYzAsMy0zLjgsNC40LTUuNywyTDc0LjIsNTguOUM3Mi43LDU3LjEsNzAuNSw1Niw2OC4yLDU2eiIvPg0KCQk8L2c+DQoJPC9nPg0KPC9nPg0KPC9zdmc+DQo=)](https://www.ngisearch.eu/view/Events/OC3Searchers)
 
 SC Data is a Python package and related tools making use of
 [`sparecores-crawler`](https://github.com/SpareCores/sc-crawler) to pull and
 standardize data on cloud compute resources. This repository actually
 runs the crawler every 5 minutes to update spot prices, and every hour
 to update all cloud resources in an internal SCD table and public
```

### Comparing `sparecores-data-0.1.0/README.md` & `sparecores_data-0.1.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 ## Spare Cores Data
 
 [![Build](https://img.shields.io/github/actions/workflow/status/SpareCores/sc-data/tests.yaml)](https://github.com/SpareCores/sc-data/actions/workflows/tests.yaml)
+[![Last Run](https://img.shields.io/endpoint?url=https%3A%2F%2Fsc-data-lastrun-mcjxzakwph52.runkit.sh)](https://github.com/SpareCores/sc-data/actions/workflows/crawl-spot.yaml)<!-- provided by https://runkit.com/daroczig/sc-data-lastrun -->
 <picture><source media="(prefers-color-scheme: dark)" srcset="https://img.shields.io/badge/status-alpha-blue"><source media="(prefers-color-scheme: light)" srcset="https://img.shields.io/badge/status-alpha-blue"><img alt="Project Status: Alpha" src="https://img.shields.io/badge/status-alpha-blue"></picture>
 <picture><source media="(prefers-color-scheme: dark)" srcset="https://img.shields.io/maintenance/yes/2024"><source media="(prefers-color-scheme: light)" srcset="https://img.shields.io/maintenance/yes/2024"><img alt="Maintenance Status: Active" src="https://img.shields.io/maintenance/yes/2024"></picture>
 [![CC-BY-SA 4.0 License](https://img.shields.io/github/license/SpareCores/sc-data)](https://github.com/SpareCores/sc-data/blob/main/LICENSE)
-[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/sc_data?logo=python&logoColor=ffdd54)](https://pypi.org/project/sparecores-data/)
+[![PyPI - Python Version](https://img.shields.io/pypi/v/sparecores-data?logo=python&logoColor=ffdd54)](https://pypi.org/project/sparecores-data/)
 [![NGI Search Open Call 3 beneficiary](https://img.shields.io/badge/NGI%20Search-Open%20Call%20%233-blue?logo=data:image/svg+xml;base64,PD94bWwgdmVyc2lvbj0iMS4wIiBlbmNvZGluZz0idXRmLTgiPz4NCjwhLS0gR2VuZXJhdG9yOiBBZG9iZSBJbGx1c3RyYXRvciAyMi4xLjAsIFNWRyBFeHBvcnQgUGx1Zy1JbiAuIFNWRyBWZXJzaW9uOiA2LjAwIEJ1aWxkIDApICAtLT4NCjxzdmcgdmVyc2lvbj0iMS4xIiBpZD0iTGF5ZXJfMSIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIiB4bWxuczp4bGluaz0iaHR0cDovL3d3dy53My5vcmcvMTk5OS94bGluayIgeD0iMHB4IiB5PSIwcHgiDQoJIHdpZHRoPSIxODBweCIgaGVpZ2h0PSIxODBweCIgdmlld0JveD0iMCAwIDE4MCAxODAiIHN0eWxlPSJlbmFibGUtYmFja2dyb3VuZDpuZXcgMCAwIDE4MCAxODA7IiB4bWw6c3BhY2U9InByZXNlcnZlIj4NCjxzdHlsZSB0eXBlPSJ0ZXh0L2NzcyI+DQoJLnN0MHtjbGlwLXBhdGg6dXJsKCNTVkdJRF8yXyk7fQ0KCS5zdDF7Y2xpcC1wYXRoOnVybCgjU1ZHSURfNF8pO2ZpbGw6dXJsKCNTVkdJRF81Xyk7fQ0KCS5zdDJ7ZmlsbDp1cmwoI1NWR0lEXzZfKTt9DQoJLnN0M3tmaWxsOiNGRkZGRkY7fQ0KPC9zdHlsZT4NCjxnPg0KCTxnPg0KCQk8ZGVmcz4NCgkJCTxwYXRoIGlkPSJTVkdJRF8xXyIgZD0iTTkwLDVDNDMuMiw1LDUsNDMuMiw1LDkwdjBjMCw0Ni43LDM4LjIsODUsODUsODVoMGM0Ni43LDAsODUtMzguMiw4NS04NXYwQzE3NSw0My4yLDEzNi44LDUsOTAsNUw5MCw1eiINCgkJCQkvPg0KCQk8L2RlZnM+DQoJCTxjbGlwUGF0aCBpZD0iU1ZHSURfMl8iPg0KCQkJPHVzZSB4bGluazpocmVmPSIjU1ZHSURfMV8iICBzdHlsZT0ib3ZlcmZsb3c6dmlzaWJsZTsiLz4NCgkJPC9jbGlwUGF0aD4NCgkJPGcgY2xhc3M9InN0MCI+DQoJCQk8Zz4NCgkJCQk8ZGVmcz4NCgkJCQkJPHJlY3QgaWQ9IlNWR0lEXzNfIiB3aWR0aD0iMTgwIiBoZWlnaHQ9IjE4MCIvPg0KCQkJCTwvZGVmcz4NCgkJCQk8Y2xpcFBhdGggaWQ9IlNWR0lEXzRfIj4NCgkJCQkJPHVzZSB4bGluazpocmVmPSIjU1ZHSURfM18iICBzdHlsZT0ib3ZlcmZsb3c6dmlzaWJsZTsiLz4NCgkJCQk8L2NsaXBQYXRoPg0KCQkJCQ0KCQkJCQk8bGluZWFyR3JhZGllbnQgaWQ9IlNWR0lEXzVfIiBncmFkaWVudFVuaXRzPSJ1c2VyU3BhY2VPblVzZSIgeDE9Ii0zMjQuNTY0MyIgeTE9IjIxMi4yNTg1IiB4Mj0iLTMyMy4zOTAzIiB5Mj0iMjEyLjI1ODUiIGdyYWRpZW50VHJhbnNmb3JtPSJtYXRyaXgoLTE1NS40ODE5IDE1MS4wOTY2IC0xNTEuMDk2NiAtMTU1LjQ4MTkgLTE4MjExLjA1ODYgODIwNDQuMjI2NikiPg0KCQkJCQk8c3RvcCAgb2Zmc2V0PSIwIiBzdHlsZT0ic3RvcC1jb2xvcjojRTUzNTAwIi8+DQoJCQkJCTxzdG9wICBvZmZzZXQ9IjEiIHN0eWxlPSJzdG9wLWNvbG9yOiM1MDAwMkQiLz4NCgkJCQk8L2xpbmVhckdyYWRpZW50Pg0KCQkJCTxwb2x5Z29uIGNsYXNzPSJzdDEiIHBvaW50cz0iMjcwLDkyLjYgODcuNCwyNzAgLTkwLDg3LjQgOTIuNiwtOTAgCQkJCSIvPg0KCQkJPC9nPg0KCQk8L2c+DQoJCTxnIGNsYXNzPSJzdDAiPg0KCQkJDQoJCQkJPGxpbmVhckdyYWRpZW50IGlkPSJTVkdJRF82XyIgZ3JhZGllbnRVbml0cz0idXNlclNwYWNlT25Vc2UiIHgxPSItMzM3Ljg2MDYiIHkxPSIxOTguNzY1NSIgeDI9Ii0zMzguMzY1MiIgeTI9IjE5OC43NzI3IiBncmFkaWVudFRyYW5zZm9ybT0ibWF0cml4KC0xMjEuNzc5NCAxMTguMzQ0NiAtMTE4LjM0NDYgLTEyMS43Nzk0IC0xNzU2MS45Mzc1IDY0MzA5LjgxMjUpIj4NCgkJCQk8c3RvcCAgb2Zmc2V0PSIwIiBzdHlsZT0ic3RvcC1jb2xvcjojNTAwMDJEIi8+DQoJCQkJPHN0b3AgIG9mZnNldD0iMSIgc3R5bGU9InN0b3AtY29sb3I6I0U1MzUwMCIvPg0KCQkJPC9saW5lYXJHcmFkaWVudD4NCgkJCTxwYXRoIGNsYXNzPSJzdDIiIGQ9Ik0xMDUuNiw4OC4yVjYzLjhjMC00LjMsMy41LTcuOCw3LjgtNy44aDBjNC4zLDAsNy44LDMuNSw3LjgsNy44djUyLjRjMCw0LjMtMy41LDcuOC03LjgsNy44aC0xLjUNCgkJCQljLTIuMywwLTQuNS0xLTYtMi44TDgwLjEsODkuN2MtMS45LTIuMy01LjctMS01LjcsMnYyNC41YzAsNC4zLTMuNSw3LjgtNy44LDcuOHMtNy44LTMuNS03LjgtNy44VjYzLjhjMC00LjMsMy41LTcuOCw3LjgtNy44DQoJCQkJaDEuNmMyLjMsMCw0LjUsMSw2LDIuOGwyNS43LDMxLjRDMTAxLjgsOTIuNiwxMDUuNiw5MS4zLDEwNS42LDg4LjJ6Ii8+DQoJCQk8cGF0aCBjbGFzcz0ic3QzIiBkPSJNNjguMiw1NmgtMS42Yy00LjMsMC03LjgsMy41LTcuOCw3Ljh2NTIuNGMwLDQuMywzLjUsNy44LDcuOCw3LjhzNy44LTMuNSw3LjgtNy44VjkxLjdjMC0zLDMuOC00LjQsNS43LTINCgkJCQlsMjUuOCwzMS41YzEuNSwxLjgsMy43LDIuOCw2LDIuOGgxLjVjNC4zLDAsNy44LTMuNSw3LjgtNy44VjYzLjhjMC00LjMtMy41LTcuOC03LjgtNy44aDBjLTQuMywwLTcuOCwzLjUtNy44LDcuOHYyNC41DQoJCQkJYzAsMy0zLjgsNC40LTUuNywyTDc0LjIsNTguOUM3Mi43LDU3LjEsNzAuNSw1Niw2OC4yLDU2eiIvPg0KCQk8L2c+DQoJPC9nPg0KPC9nPg0KPC9zdmc+DQo=)](https://www.ngisearch.eu/view/Events/OC3Searchers)
 
 SC Data is a Python package and related tools making use of
 [`sparecores-crawler`](https://github.com/SpareCores/sc-crawler) to pull and
 standardize data on cloud compute resources. This repository actually
 runs the crawler every 5 minutes to update spot prices, and every hour
 to update all cloud resources in an internal SCD table and public
```

### Comparing `sparecores-data-0.1.0/pyproject.toml` & `sparecores_data-0.1.3/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "sparecores-data"
-version = "0.1.0"
+version = "0.1.3"
 description = "Structured data collected by sparecores-crawler."
 readme = "README.md"
 requires-python = ">=3.8"
 authors = [
   { name="Attila Nagy" },
   { name="Gergely Daroczi" },
   { name="Balazs Hodobay" },
@@ -12,23 +12,25 @@
 maintainers = [
   { name="Spare Cores team", email="pkg@sparecores.com" }
 ]
 dependencies = [
     "requests",
     "safe_exit",
 ]
+keywords = ["cloud", "compute", "etl", "sqlite", "spot-instances", "cost-optimization"]
 classifiers = [
   "Programming Language :: Python :: 3",
   "Operating System :: OS Independent",
   "Development Status :: 3 - Alpha",
 ]
 
 [project.urls]
-Homepage = "https://github.com/SpareCores/sc-data"
-Issues = "https://github.com/SpareCores/sc-data/issues"
+repository = "https://github.com/SpareCores/sc-data"
+issues = "https://github.com/SpareCores/sc-data/issues"
+homepage = "https://sparecores.com"
 
 [project.optional-dependencies]
 testing = ["pytest", "sqlalchemy"]
 all = ["sparecores-data[testing]"]
 
 [tool.setuptools]
 include-package-data = true  # see MANIFEST.in
```

### Comparing `sparecores-data-0.1.0/src/sc_data/__init__.py` & `sparecores_data-0.1.3/src/sc_data/__init__.py`

 * *Files identical despite different names*

### Comparing `sparecores-data-0.1.0/src/sc_data/data.py` & `sparecores_data-0.1.3/src/sc_data/data.py`

 * *Files 6% similar despite different names*

```diff
@@ -86,14 +86,17 @@
             shutil.copyfileobj(fh, tmpfile)
             tmpfile.flush()
             with self.lock:
                 self.actual_db_path = tmpfile.name
                 self.actual_db_hash = db_hash
             close_tmpfiles(self.tmpfiles)
             self.tmpfiles.append(tmpfile)
+            logging.debug("Updated database to hash %s", db_hash)
+        else:
+            logging.debug("No need to udpate database")
 
     def run(self):
         """Start the update thread if no_update is not set."""
         if get_parameter("no_update"):
             self.updated.set()
             return
         while True:
```

### Comparing `sparecores-data-0.1.0/src/sparecores_data.egg-info/PKG-INFO` & `sparecores_data-0.1.3/src/sparecores_data.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: sparecores-data
-Version: 0.1.0
+Version: 0.1.3
 Summary: Structured data collected by sparecores-crawler.
 Author: Attila Nagy, Gergely Daroczi, Balazs Hodobay
 Maintainer-email: Spare Cores team <pkg@sparecores.com>
-Project-URL: Homepage, https://github.com/SpareCores/sc-data
-Project-URL: Issues, https://github.com/SpareCores/sc-data/issues
+Project-URL: repository, https://github.com/SpareCores/sc-data
+Project-URL: issues, https://github.com/SpareCores/sc-data/issues
+Project-URL: homepage, https://sparecores.com
+Keywords: cloud,compute,etl,sqlite,spot-instances,cost-optimization
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
@@ -19,18 +21,19 @@
 Requires-Dist: sqlalchemy; extra == "testing"
 Provides-Extra: all
 Requires-Dist: sparecores-data[testing]; extra == "all"
 
 ## Spare Cores Data
 
 [![Build](https://img.shields.io/github/actions/workflow/status/SpareCores/sc-data/tests.yaml)](https://github.com/SpareCores/sc-data/actions/workflows/tests.yaml)
+[![Last Run](https://img.shields.io/endpoint?url=https%3A%2F%2Fsc-data-lastrun-mcjxzakwph52.runkit.sh)](https://github.com/SpareCores/sc-data/actions/workflows/crawl-spot.yaml)<!-- provided by https://runkit.com/daroczig/sc-data-lastrun -->
 <picture><source media="(prefers-color-scheme: dark)" srcset="https://img.shields.io/badge/status-alpha-blue"><source media="(prefers-color-scheme: light)" srcset="https://img.shields.io/badge/status-alpha-blue"><img alt="Project Status: Alpha" src="https://img.shields.io/badge/status-alpha-blue"></picture>
 <picture><source media="(prefers-color-scheme: dark)" srcset="https://img.shields.io/maintenance/yes/2024"><source media="(prefers-color-scheme: light)" srcset="https://img.shields.io/maintenance/yes/2024"><img alt="Maintenance Status: Active" src="https://img.shields.io/maintenance/yes/2024"></picture>
 [![CC-BY-SA 4.0 License](https://img.shields.io/github/license/SpareCores/sc-data)](https://github.com/SpareCores/sc-data/blob/main/LICENSE)
-[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/sc_data?logo=python&logoColor=ffdd54)](https://pypi.org/project/sparecores-data/)
+[![PyPI - Python Version](https://img.shields.io/pypi/v/sparecores-data?logo=python&logoColor=ffdd54)](https://pypi.org/project/sparecores-data/)
 [![NGI Search Open Call 3 beneficiary](https://img.shields.io/badge/NGI%20Search-Open%20Call%20%233-blue?logo=data:image/svg+xml;base64,PD94bWwgdmVyc2lvbj0iMS4wIiBlbmNvZGluZz0idXRmLTgiPz4NCjwhLS0gR2VuZXJhdG9yOiBBZG9iZSBJbGx1c3RyYXRvciAyMi4xLjAsIFNWRyBFeHBvcnQgUGx1Zy1JbiAuIFNWRyBWZXJzaW9uOiA2LjAwIEJ1aWxkIDApICAtLT4NCjxzdmcgdmVyc2lvbj0iMS4xIiBpZD0iTGF5ZXJfMSIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIiB4bWxuczp4bGluaz0iaHR0cDovL3d3dy53My5vcmcvMTk5OS94bGluayIgeD0iMHB4IiB5PSIwcHgiDQoJIHdpZHRoPSIxODBweCIgaGVpZ2h0PSIxODBweCIgdmlld0JveD0iMCAwIDE4MCAxODAiIHN0eWxlPSJlbmFibGUtYmFja2dyb3VuZDpuZXcgMCAwIDE4MCAxODA7IiB4bWw6c3BhY2U9InByZXNlcnZlIj4NCjxzdHlsZSB0eXBlPSJ0ZXh0L2NzcyI+DQoJLnN0MHtjbGlwLXBhdGg6dXJsKCNTVkdJRF8yXyk7fQ0KCS5zdDF7Y2xpcC1wYXRoOnVybCgjU1ZHSURfNF8pO2ZpbGw6dXJsKCNTVkdJRF81Xyk7fQ0KCS5zdDJ7ZmlsbDp1cmwoI1NWR0lEXzZfKTt9DQoJLnN0M3tmaWxsOiNGRkZGRkY7fQ0KPC9zdHlsZT4NCjxnPg0KCTxnPg0KCQk8ZGVmcz4NCgkJCTxwYXRoIGlkPSJTVkdJRF8xXyIgZD0iTTkwLDVDNDMuMiw1LDUsNDMuMiw1LDkwdjBjMCw0Ni43LDM4LjIsODUsODUsODVoMGM0Ni43LDAsODUtMzguMiw4NS04NXYwQzE3NSw0My4yLDEzNi44LDUsOTAsNUw5MCw1eiINCgkJCQkvPg0KCQk8L2RlZnM+DQoJCTxjbGlwUGF0aCBpZD0iU1ZHSURfMl8iPg0KCQkJPHVzZSB4bGluazpocmVmPSIjU1ZHSURfMV8iICBzdHlsZT0ib3ZlcmZsb3c6dmlzaWJsZTsiLz4NCgkJPC9jbGlwUGF0aD4NCgkJPGcgY2xhc3M9InN0MCI+DQoJCQk8Zz4NCgkJCQk8ZGVmcz4NCgkJCQkJPHJlY3QgaWQ9IlNWR0lEXzNfIiB3aWR0aD0iMTgwIiBoZWlnaHQ9IjE4MCIvPg0KCQkJCTwvZGVmcz4NCgkJCQk8Y2xpcFBhdGggaWQ9IlNWR0lEXzRfIj4NCgkJCQkJPHVzZSB4bGluazpocmVmPSIjU1ZHSURfM18iICBzdHlsZT0ib3ZlcmZsb3c6dmlzaWJsZTsiLz4NCgkJCQk8L2NsaXBQYXRoPg0KCQkJCQ0KCQkJCQk8bGluZWFyR3JhZGllbnQgaWQ9IlNWR0lEXzVfIiBncmFkaWVudFVuaXRzPSJ1c2VyU3BhY2VPblVzZSIgeDE9Ii0zMjQuNTY0MyIgeTE9IjIxMi4yNTg1IiB4Mj0iLTMyMy4zOTAzIiB5Mj0iMjEyLjI1ODUiIGdyYWRpZW50VHJhbnNmb3JtPSJtYXRyaXgoLTE1NS40ODE5IDE1MS4wOTY2IC0xNTEuMDk2NiAtMTU1LjQ4MTkgLTE4MjExLjA1ODYgODIwNDQuMjI2NikiPg0KCQkJCQk8c3RvcCAgb2Zmc2V0PSIwIiBzdHlsZT0ic3RvcC1jb2xvcjojRTUzNTAwIi8+DQoJCQkJCTxzdG9wICBvZmZzZXQ9IjEiIHN0eWxlPSJzdG9wLWNvbG9yOiM1MDAwMkQiLz4NCgkJCQk8L2xpbmVhckdyYWRpZW50Pg0KCQkJCTxwb2x5Z29uIGNsYXNzPSJzdDEiIHBvaW50cz0iMjcwLDkyLjYgODcuNCwyNzAgLTkwLDg3LjQgOTIuNiwtOTAgCQkJCSIvPg0KCQkJPC9nPg0KCQk8L2c+DQoJCTxnIGNsYXNzPSJzdDAiPg0KCQkJDQoJCQkJPGxpbmVhckdyYWRpZW50IGlkPSJTVkdJRF82XyIgZ3JhZGllbnRVbml0cz0idXNlclNwYWNlT25Vc2UiIHgxPSItMzM3Ljg2MDYiIHkxPSIxOTguNzY1NSIgeDI9Ii0zMzguMzY1MiIgeTI9IjE5OC43NzI3IiBncmFkaWVudFRyYW5zZm9ybT0ibWF0cml4KC0xMjEuNzc5NCAxMTguMzQ0NiAtMTE4LjM0NDYgLTEyMS43Nzk0IC0xNzU2MS45Mzc1IDY0MzA5LjgxMjUpIj4NCgkJCQk8c3RvcCAgb2Zmc2V0PSIwIiBzdHlsZT0ic3RvcC1jb2xvcjojNTAwMDJEIi8+DQoJCQkJPHN0b3AgIG9mZnNldD0iMSIgc3R5bGU9InN0b3AtY29sb3I6I0U1MzUwMCIvPg0KCQkJPC9saW5lYXJHcmFkaWVudD4NCgkJCTxwYXRoIGNsYXNzPSJzdDIiIGQ9Ik0xMDUuNiw4OC4yVjYzLjhjMC00LjMsMy41LTcuOCw3LjgtNy44aDBjNC4zLDAsNy44LDMuNSw3LjgsNy44djUyLjRjMCw0LjMtMy41LDcuOC03LjgsNy44aC0xLjUNCgkJCQljLTIuMywwLTQuNS0xLTYtMi44TDgwLjEsODkuN2MtMS45LTIuMy01LjctMS01LjcsMnYyNC41YzAsNC4zLTMuNSw3LjgtNy44LDcuOHMtNy44LTMuNS03LjgtNy44VjYzLjhjMC00LjMsMy41LTcuOCw3LjgtNy44DQoJCQkJaDEuNmMyLjMsMCw0LjUsMSw2LDIuOGwyNS43LDMxLjRDMTAxLjgsOTIuNiwxMDUuNiw5MS4zLDEwNS42LDg4LjJ6Ii8+DQoJCQk8cGF0aCBjbGFzcz0ic3QzIiBkPSJNNjguMiw1NmgtMS42Yy00LjMsMC03LjgsMy41LTcuOCw3Ljh2NTIuNGMwLDQuMywzLjUsNy44LDcuOCw3LjhzNy44LTMuNSw3LjgtNy44VjkxLjdjMC0zLDMuOC00LjQsNS43LTINCgkJCQlsMjUuOCwzMS41YzEuNSwxLjgsMy43LDIuOCw2LDIuOGgxLjVjNC4zLDAsNy44LTMuNSw3LjgtNy44VjYzLjhjMC00LjMtMy41LTcuOC03LjgtNy44aDBjLTQuMywwLTcuOCwzLjUtNy44LDcuOHYyNC41DQoJCQkJYzAsMy0zLjgsNC40LTUuNywyTDc0LjIsNTguOUM3Mi43LDU3LjEsNzAuNSw1Niw2OC4yLDU2eiIvPg0KCQk8L2c+DQoJPC9nPg0KPC9nPg0KPC9zdmc+DQo=)](https://www.ngisearch.eu/view/Events/OC3Searchers)
 
 SC Data is a Python package and related tools making use of
 [`sparecores-crawler`](https://github.com/SpareCores/sc-crawler) to pull and
 standardize data on cloud compute resources. This repository actually
 runs the crawler every 5 minutes to update spot prices, and every hour
 to update all cloud resources in an internal SCD table and public
```

### Comparing `sparecores-data-0.1.0/tests/test_data.py` & `sparecores_data-0.1.3/tests/test_data.py`

 * *Files identical despite different names*

