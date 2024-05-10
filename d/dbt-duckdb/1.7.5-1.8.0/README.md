# Comparing `tmp/dbt_duckdb-1.7.5.tar.gz` & `tmp/dbt_duckdb-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt_duckdb-1.7.5.tar", last modified: Wed May  8 05:42:52 2024, max compression
+gzip compressed data, was "dbt_duckdb-1.8.0.tar", last modified: Fri May 10 04:54:01 2024, max compression
```

## Comparing `dbt_duckdb-1.7.5.tar` & `dbt_duckdb-1.8.0.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 05:42:52.178551 dbt_duckdb-1.7.5/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-08 05:42:45.000000 dbt_duckdb-1.7.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-08 05:42:45.000000 dbt_duckdb-1.7.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    23723 2024-05-08 05:42:52.178551 dbt_duckdb-1.7.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    22716 2024-05-08 05:42:45.000000 dbt_duckdb-1.7.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 05:42:52.170551 dbt_duckdb-1.7.5/dbt/
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-08 05:42:45.000000 dbt_duckdb-1.7.5/dbt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 05:42:52.170551 dbt_duckdb-1.7.5/dbt/adapters/
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-08 05:42:45.000000 dbt_duckdb-1.7.5/dbt/adapters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 05:42:52.170551 dbt_duckdb-1.7.5/dbt/adapters/duckdb/
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-08 05:42:45.000000 dbt_duckdb-1.7.5/dbt/adapters/duckdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-08 05:42:45.000000 dbt_duckdb-1.7.5/dbt/adapters/duckdb/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-08 05:42:45.000000 dbt_duckdb-1.7.5/dbt/adapters/duckdb/column.py
--rw-r--r--   0 runner    (1001) docker     (127)     4078 2024-05-08 05:42:45.000000 dbt_duckdb-1.7.5/dbt/adapters/duckdb/connections.py
--rw-r--r--   0 runner    (1001) docker     (127)     9997 2024-05-08 05:42:45.000000 dbt_duckdb-1.7.5/dbt/adapters/duckdb/credentials.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 05:42:52.174551 dbt_duckdb-1.7.5/dbt/adapters/duckdb/environments/
--rw-r--r--   0 runner    (1001) docker     (127)     9912 2024-05-08 05:42:45.000000 dbt_duckdb-1.7.5/dbt/adapters/duckdb/environments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-05-08 05:42:45.000000 dbt_duckdb-1.7.5/dbt/adapters/duckdb/environments/buenavista.py
--rw-r--r--   0 runner    (1001) docker     (127)     5669 2024-05-08 05:42:45.000000 dbt_duckdb-1.7.5/dbt/adapters/duckdb/environments/local.py
--rw-r--r--   0 runner    (1001) docker     (127)    11305 2024-05-08 05:42:45.000000 dbt_duckdb-1.7.5/dbt/adapters/duckdb/impl.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 05:42:52.174551 dbt_duckdb-1.7.5/dbt/adapters/duckdb/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)     5039 2024-05-08 05:42:45.000000 dbt_duckdb-1.7.5/dbt/adapters/duckdb/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-05-08 05:42:45.000000 dbt_duckdb-1.7.5/dbt/adapters/duckdb/plugins/delta.py
--rw-r--r--   0 runner    (1001) docker     (127)     4951 2024-05-08 05:42:45.000000 dbt_duckdb-1.7.5/dbt/adapters/duckdb/plugins/excel.py
--rw-r--r--   0 runner    (1001) docker     (127)    12466 2024-05-08 05:42:45.000000 dbt_duckdb-1.7.5/dbt/adapters/duckdb/plugins/glue.py
--rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-05-08 05:42:45.000000 dbt_duckdb-1.7.5/dbt/adapters/duckdb/plugins/gsheet.py
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-05-08 05:42:45.000000 dbt_duckdb-1.7.5/dbt/adapters/duckdb/plugins/iceberg.py
--rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-05-08 05:42:45.000000 dbt_duckdb-1.7.5/dbt/adapters/duckdb/plugins/motherduck.py
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-05-08 05:42:45.000000 dbt_duckdb-1.7.5/dbt/adapters/duckdb/plugins/pd_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-05-08 05:42:45.000000 dbt_duckdb-1.7.5/dbt/adapters/duckdb/plugins/postgres.py
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-05-08 05:42:45.000000 dbt_duckdb-1.7.5/dbt/adapters/duckdb/plugins/sqlalchemy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3457 2024-05-08 05:42:45.000000 dbt_duckdb-1.7.5/dbt/adapters/duckdb/relation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2445 2024-05-08 05:42:45.000000 dbt_duckdb-1.7.5/dbt/adapters/duckdb/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 05:42:52.174551 dbt_duckdb-1.7.5/dbt/include/
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-08 05:42:45.000000 dbt_duckdb-1.7.5/dbt/include/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 05:42:52.174551 dbt_duckdb-1.7.5/dbt/include/duckdb/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-08 05:42:45.000000 dbt_duckdb-1.7.5/dbt/include/duckdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-08 05:42:45.000000 dbt_duckdb-1.7.5/dbt/include/duckdb/dbt_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 05:42:52.174551 dbt_duckdb-1.7.5/dbt/include/duckdb/macros/
--rw-r--r--   0 runner    (1001) docker     (127)     7949 2024-05-08 05:42:45.000000 dbt_duckdb-1.7.5/dbt/include/duckdb/macros/adapters.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-05-08 05:42:45.000000 dbt_duckdb-1.7.5/dbt/include/duckdb/macros/catalog.sql
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-08 05:42:45.000000 dbt_duckdb-1.7.5/dbt/include/duckdb/macros/columns.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-05-08 05:42:45.000000 dbt_duckdb-1.7.5/dbt/include/duckdb/macros/incremental_helper.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 05:42:52.178551 dbt_duckdb-1.7.5/dbt/include/duckdb/macros/materializations/
--rw-r--r--   0 runner    (1001) docker     (127)     4165 2024-05-08 05:42:45.000000 dbt_duckdb-1.7.5/dbt/include/duckdb/macros/materializations/external.sql
--rw-r--r--   0 runner    (1001) docker     (127)     5315 2024-05-08 05:42:45.000000 dbt_duckdb-1.7.5/dbt/include/duckdb/macros/materializations/incremental.sql
--rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-05-08 05:42:45.000000 dbt_duckdb-1.7.5/dbt/include/duckdb/macros/materializations/table.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-05-08 05:42:45.000000 dbt_duckdb-1.7.5/dbt/include/duckdb/macros/persist_docs.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-05-08 05:42:45.000000 dbt_duckdb-1.7.5/dbt/include/duckdb/macros/seed.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-05-08 05:42:45.000000 dbt_duckdb-1.7.5/dbt/include/duckdb/macros/snapshot_helper.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 05:42:52.178551 dbt_duckdb-1.7.5/dbt/include/duckdb/macros/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-08 05:42:45.000000 dbt_duckdb-1.7.5/dbt/include/duckdb/macros/utils/any_value.sql
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-08 05:42:45.000000 dbt_duckdb-1.7.5/dbt/include/duckdb/macros/utils/dateadd.sql
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-08 05:42:45.000000 dbt_duckdb-1.7.5/dbt/include/duckdb/macros/utils/datediff.sql
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-08 05:42:45.000000 dbt_duckdb-1.7.5/dbt/include/duckdb/macros/utils/external_location.sql
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-08 05:42:45.000000 dbt_duckdb-1.7.5/dbt/include/duckdb/macros/utils/lastday.sql
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-08 05:42:45.000000 dbt_duckdb-1.7.5/dbt/include/duckdb/macros/utils/listagg.sql
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-08 05:42:45.000000 dbt_duckdb-1.7.5/dbt/include/duckdb/macros/utils/splitpart.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-05-08 05:42:45.000000 dbt_duckdb-1.7.5/dbt/include/duckdb/macros/utils/upstream.sql
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-08 05:42:45.000000 dbt_duckdb-1.7.5/dbt/include/duckdb/sample_profiles.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 05:42:52.178551 dbt_duckdb-1.7.5/dbt_duckdb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    23723 2024-05-08 05:42:52.000000 dbt_duckdb-1.7.5/dbt_duckdb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-05-08 05:42:52.000000 dbt_duckdb-1.7.5/dbt_duckdb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 05:42:52.000000 dbt_duckdb-1.7.5/dbt_duckdb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-08 05:42:52.000000 dbt_duckdb-1.7.5/dbt_duckdb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-08 05:42:52.000000 dbt_duckdb-1.7.5/dbt_duckdb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 05:42:52.182551 dbt_duckdb-1.7.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-05-08 05:42:45.000000 dbt_duckdb-1.7.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 04:54:01.938098 dbt_duckdb-1.8.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-10 04:53:58.000000 dbt_duckdb-1.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-10 04:53:58.000000 dbt_duckdb-1.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    23789 2024-05-10 04:54:01.938098 dbt_duckdb-1.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    22716 2024-05-10 04:53:58.000000 dbt_duckdb-1.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 04:54:01.926098 dbt_duckdb-1.8.0/dbt/
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-10 04:53:58.000000 dbt_duckdb-1.8.0/dbt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 04:54:01.926098 dbt_duckdb-1.8.0/dbt/adapters/
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-10 04:53:58.000000 dbt_duckdb-1.8.0/dbt/adapters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 04:54:01.930098 dbt_duckdb-1.8.0/dbt/adapters/duckdb/
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-10 04:53:58.000000 dbt_duckdb-1.8.0/dbt/adapters/duckdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-10 04:53:58.000000 dbt_duckdb-1.8.0/dbt/adapters/duckdb/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-10 04:53:58.000000 dbt_duckdb-1.8.0/dbt/adapters/duckdb/column.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4256 2024-05-10 04:53:58.000000 dbt_duckdb-1.8.0/dbt/adapters/duckdb/connections.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10019 2024-05-10 04:53:58.000000 dbt_duckdb-1.8.0/dbt/adapters/duckdb/credentials.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 04:54:01.930098 dbt_duckdb-1.8.0/dbt/adapters/duckdb/environments/
+-rw-r--r--   0 runner    (1001) docker     (127)     9937 2024-05-10 04:53:58.000000 dbt_duckdb-1.8.0/dbt/adapters/duckdb/environments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2596 2024-05-10 04:53:58.000000 dbt_duckdb-1.8.0/dbt/adapters/duckdb/environments/buenavista.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5695 2024-05-10 04:53:58.000000 dbt_duckdb-1.8.0/dbt/adapters/duckdb/environments/local.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11292 2024-05-10 04:53:58.000000 dbt_duckdb-1.8.0/dbt/adapters/duckdb/impl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 04:54:01.930098 dbt_duckdb-1.8.0/dbt/adapters/duckdb/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)     5046 2024-05-10 04:53:58.000000 dbt_duckdb-1.8.0/dbt/adapters/duckdb/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-05-10 04:53:58.000000 dbt_duckdb-1.8.0/dbt/adapters/duckdb/plugins/delta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4951 2024-05-10 04:53:58.000000 dbt_duckdb-1.8.0/dbt/adapters/duckdb/plugins/excel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12466 2024-05-10 04:53:58.000000 dbt_duckdb-1.8.0/dbt/adapters/duckdb/plugins/glue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-05-10 04:53:58.000000 dbt_duckdb-1.8.0/dbt/adapters/duckdb/plugins/gsheet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-05-10 04:53:58.000000 dbt_duckdb-1.8.0/dbt/adapters/duckdb/plugins/iceberg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-05-10 04:53:58.000000 dbt_duckdb-1.8.0/dbt/adapters/duckdb/plugins/motherduck.py
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-05-10 04:53:58.000000 dbt_duckdb-1.8.0/dbt/adapters/duckdb/plugins/pd_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-05-10 04:53:58.000000 dbt_duckdb-1.8.0/dbt/adapters/duckdb/plugins/postgres.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-05-10 04:53:58.000000 dbt_duckdb-1.8.0/dbt/adapters/duckdb/plugins/sqlalchemy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3948 2024-05-10 04:53:58.000000 dbt_duckdb-1.8.0/dbt/adapters/duckdb/relation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2478 2024-05-10 04:53:58.000000 dbt_duckdb-1.8.0/dbt/adapters/duckdb/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 04:54:01.930098 dbt_duckdb-1.8.0/dbt/include/
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-10 04:53:58.000000 dbt_duckdb-1.8.0/dbt/include/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 04:54:01.930098 dbt_duckdb-1.8.0/dbt/include/duckdb/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-10 04:53:58.000000 dbt_duckdb-1.8.0/dbt/include/duckdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-10 04:53:58.000000 dbt_duckdb-1.8.0/dbt/include/duckdb/dbt_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 04:54:01.934098 dbt_duckdb-1.8.0/dbt/include/duckdb/macros/
+-rw-r--r--   0 runner    (1001) docker     (127)     7949 2024-05-10 04:53:58.000000 dbt_duckdb-1.8.0/dbt/include/duckdb/macros/adapters.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-05-10 04:53:58.000000 dbt_duckdb-1.8.0/dbt/include/duckdb/macros/catalog.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-10 04:53:58.000000 dbt_duckdb-1.8.0/dbt/include/duckdb/macros/columns.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-05-10 04:53:58.000000 dbt_duckdb-1.8.0/dbt/include/duckdb/macros/incremental_helper.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 04:54:01.934098 dbt_duckdb-1.8.0/dbt/include/duckdb/macros/materializations/
+-rw-r--r--   0 runner    (1001) docker     (127)     4165 2024-05-10 04:53:58.000000 dbt_duckdb-1.8.0/dbt/include/duckdb/macros/materializations/external.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     5315 2024-05-10 04:53:58.000000 dbt_duckdb-1.8.0/dbt/include/duckdb/macros/materializations/incremental.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-05-10 04:53:58.000000 dbt_duckdb-1.8.0/dbt/include/duckdb/macros/materializations/table.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-05-10 04:53:58.000000 dbt_duckdb-1.8.0/dbt/include/duckdb/macros/persist_docs.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-05-10 04:53:58.000000 dbt_duckdb-1.8.0/dbt/include/duckdb/macros/seed.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-05-10 04:53:58.000000 dbt_duckdb-1.8.0/dbt/include/duckdb/macros/snapshot_helper.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 04:54:01.934098 dbt_duckdb-1.8.0/dbt/include/duckdb/macros/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-10 04:53:58.000000 dbt_duckdb-1.8.0/dbt/include/duckdb/macros/utils/any_value.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-10 04:53:58.000000 dbt_duckdb-1.8.0/dbt/include/duckdb/macros/utils/dateadd.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-10 04:53:58.000000 dbt_duckdb-1.8.0/dbt/include/duckdb/macros/utils/datediff.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-10 04:53:58.000000 dbt_duckdb-1.8.0/dbt/include/duckdb/macros/utils/external_location.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-10 04:53:58.000000 dbt_duckdb-1.8.0/dbt/include/duckdb/macros/utils/lastday.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-10 04:53:58.000000 dbt_duckdb-1.8.0/dbt/include/duckdb/macros/utils/listagg.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-10 04:53:58.000000 dbt_duckdb-1.8.0/dbt/include/duckdb/macros/utils/splitpart.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-05-10 04:53:58.000000 dbt_duckdb-1.8.0/dbt/include/duckdb/macros/utils/upstream.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-10 04:53:58.000000 dbt_duckdb-1.8.0/dbt/include/duckdb/sample_profiles.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 04:54:01.934098 dbt_duckdb-1.8.0/dbt_duckdb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    23789 2024-05-10 04:54:01.000000 dbt_duckdb-1.8.0/dbt_duckdb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-05-10 04:54:01.000000 dbt_duckdb-1.8.0/dbt_duckdb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 04:54:01.000000 dbt_duckdb-1.8.0/dbt_duckdb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-10 04:54:01.000000 dbt_duckdb-1.8.0/dbt_duckdb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-10 04:54:01.000000 dbt_duckdb-1.8.0/dbt_duckdb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 04:54:01.938098 dbt_duckdb-1.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-05-10 04:53:58.000000 dbt_duckdb-1.8.0/setup.py
```

### Comparing `dbt_duckdb-1.7.5/LICENSE` & `dbt_duckdb-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt_duckdb-1.7.5/PKG-INFO` & `dbt_duckdb-1.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-duckdb
-Version: 1.7.5
+Version: 1.8.0
 Summary: The duckdb adapter plugin for dbt (data build tool)
 Home-page: https://github.com/jwills/dbt-duckdb
 Author: Josh Wills
 Author-email: joshwills+dbt@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
@@ -13,16 +13,18 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: dbt-core~=1.7.0
+Requires-Dist: dbt-common<2,>=1
+Requires-Dist: dbt-adapters<2,>=1
 Requires-Dist: duckdb>=0.7.0
+Requires-Dist: dbt-core>=1.8.0
 Provides-Extra: glue
 Requires-Dist: boto3; extra == "glue"
 Requires-Dist: mypy-boto3-glue; extra == "glue"
 Provides-Extra: md
 Requires-Dist: duckdb>=0.10.2; extra == "md"
 
 ## dbt-duckdb
```

### Comparing `dbt_duckdb-1.7.5/README.md` & `dbt_duckdb-1.8.0/README.md`

 * *Files identical despite different names*

### Comparing `dbt_duckdb-1.7.5/dbt/adapters/duckdb/column.py` & `dbt_duckdb-1.8.0/dbt/adapters/duckdb/column.py`

 * *Files identical despite different names*

### Comparing `dbt_duckdb-1.7.5/dbt/adapters/duckdb/connections.py` & `dbt_duckdb-1.8.0/dbt/adapters/duckdb/connections.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,38 @@
 import atexit
 import threading
 from contextlib import contextmanager
+from multiprocessing.context import SpawnContext
 from typing import Optional
 from typing import Tuple
 from typing import TYPE_CHECKING
 
 import dbt.exceptions
 from . import environments
+from dbt.adapters.contracts.connection import AdapterRequiredConfig
+from dbt.adapters.contracts.connection import AdapterResponse
+from dbt.adapters.contracts.connection import Connection
+from dbt.adapters.contracts.connection import ConnectionState
+from dbt.adapters.events.logging import AdapterLogger
 from dbt.adapters.sql import SQLConnectionManager
-from dbt.contracts.connection import AdapterRequiredConfig
-from dbt.contracts.connection import AdapterResponse
-from dbt.contracts.connection import Connection
-from dbt.contracts.connection import ConnectionState
-from dbt.logger import GLOBAL_LOGGER as logger
+
+logger = AdapterLogger("DuckDB")
 
 if TYPE_CHECKING:
     import agate
 
 
 class DuckDBConnectionManager(SQLConnectionManager):
     TYPE = "duckdb"
     _LOCK = threading.RLock()
     _ENV = None
 
-    def __init__(self, profile: AdapterRequiredConfig):
-        super().__init__(profile)
-        self.disable_transactions = profile.credentials.disable_transactions  # type: ignore
+    def __init__(self, config: AdapterRequiredConfig, mp_context: SpawnContext) -> None:
+        super().__init__(config, mp_context)
+        self.disable_transactions = config.credentials.disable_transactions  # type: ignore
 
     @classmethod
     def env(cls) -> environments.Environment:
         with cls._LOCK:
             if not cls._ENV:
                 raise Exception("DuckDBConnectionManager environment requested before creation!")
             return cls._ENV
@@ -48,15 +51,15 @@
                 connection.handle = cls._ENV.handle()
                 connection.state = ConnectionState.OPEN
 
             except RuntimeError as e:
                 logger.debug("Got an error when attempting to connect to DuckDB: '{}'".format(e))
                 connection.handle = None
                 connection.state = ConnectionState.FAIL
-                raise dbt.exceptions.FailedToConnectError(str(e))
+                raise dbt.adapters.exceptions.FailedToConnectError(str(e))
 
             return connection
 
     @classmethod
     def close(cls, connection: Connection) -> Connection:
         # if the connection is in closed or init, there's nothing to do
         if connection.state in {ConnectionState.CLOSED, ConnectionState.INIT}:
```

### Comparing `dbt_duckdb-1.7.5/dbt/adapters/duckdb/credentials.py` & `dbt_duckdb-1.8.0/dbt/adapters/duckdb/credentials.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,17 +6,18 @@
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Tuple
 from urllib.parse import urlparse
 
-import dbt.exceptions
-from dbt.adapters.base import Credentials
-from dbt.dataclass_schema import dbtClassMixin
+from dbt_common.dataclass_schema import dbtClassMixin
+from dbt_common.exceptions import DbtRuntimeError
+
+from dbt.adapters.contracts.connection import Credentials
 
 
 @dataclass
 class Attachment(dbtClassMixin):
     # The path to the database to be attached (may be a URL)
     path: str
 
@@ -183,20 +184,20 @@
                 if path_db == "":
                     path_db = "my_db"
 
         if path_db and "database" not in data:
             data["database"] = path_db
         elif path_db and data["database"] != path_db:
             if not data.get("remote"):
-                raise dbt.exceptions.DbtRuntimeError(
+                raise DbtRuntimeError(
                     "Inconsistency detected between 'path' and 'database' fields in profile; "
                     f"the 'database' property must be set to '{path_db}' to match the 'path'"
                 )
         elif not path_db:
-            raise dbt.exceptions.DbtRuntimeError(
+            raise DbtRuntimeError(
                 "Unable to determine target database name from 'path' field in profile"
             )
         return data
 
     @property
     def unique_field(self) -> str:
         """
```

### Comparing `dbt_duckdb-1.7.5/dbt/adapters/duckdb/environments/__init__.py` & `dbt_duckdb-1.8.0/dbt/adapters/duckdb/environments/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,22 +5,22 @@
 import tempfile
 import time
 from typing import Dict
 from typing import List
 from typing import Optional
 
 import duckdb
+from dbt_common.exceptions import DbtRuntimeError
 
 from ..credentials import DuckDBCredentials
 from ..plugins import BasePlugin
 from ..utils import SourceConfig
 from ..utils import TargetConfig
-from dbt.contracts.connection import AdapterResponse
-from dbt.contracts.connection import Connection
-from dbt.exceptions import DbtRuntimeError
+from dbt.adapters.contracts.connection import AdapterResponse
+from dbt.adapters.contracts.connection import Connection
 
 
 def _ensure_event_loop():
     """
     Ensures the current thread has an event loop defined, and creates one if necessary.
     """
     import asyncio
```

### Comparing `dbt_duckdb-1.7.5/dbt/adapters/duckdb/environments/buenavista.py` & `dbt_duckdb-1.8.0/dbt/adapters/duckdb/environments/buenavista.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import json
 
 import psycopg2
 
 from . import Environment
 from .. import credentials
 from .. import utils
-from dbt.contracts.connection import AdapterResponse
-from dbt.contracts.connection import Connection
+from dbt.adapters.contracts.connection import AdapterResponse
+from dbt.adapters.contracts.connection import Connection
 
 
 class BVEnvironment(Environment):
     @classmethod
     def _get_conn(cls, dbname: str, remote: credentials.Remote):
         return psycopg2.connect(
             dbname=dbname,
```

### Comparing `dbt_duckdb-1.7.5/dbt/adapters/duckdb/environments/local.py` & `dbt_duckdb-1.8.0/dbt/adapters/duckdb/environments/local.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import threading
 
+from dbt_common.exceptions import DbtRuntimeError
+
 from . import Environment
 from .. import credentials
 from .. import utils
-from dbt.contracts.connection import AdapterResponse
-from dbt.contracts.connection import Connection
-from dbt.exceptions import DbtRuntimeError
+from dbt.adapters.contracts.connection import AdapterResponse
+from dbt.adapters.contracts.connection import Connection
 
 
 class DuckDBCursorWrapper:
     def __init__(self, cursor):
         self._cursor = cursor
 
     # forward along all non-execute() methods/attribute look-ups
```

### Comparing `dbt_duckdb-1.7.5/dbt/adapters/duckdb/impl.py` & `dbt_duckdb-1.8.0/dbt/adapters/duckdb/impl.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 import os
 from typing import Any
 from typing import List
 from typing import Optional
 from typing import Sequence
 from typing import TYPE_CHECKING
 
+from dbt_common.contracts.constraints import ColumnLevelConstraint
+from dbt_common.contracts.constraints import ConstraintType
+from dbt_common.exceptions import DbtInternalError
+from dbt_common.exceptions import DbtRuntimeError
+
 from dbt.adapters.base import BaseRelation
 from dbt.adapters.base.column import Column as BaseColumn
 from dbt.adapters.base.impl import ConstraintSupport
 from dbt.adapters.base.meta import available
+from dbt.adapters.contracts.connection import AdapterResponse
+from dbt.adapters.contracts.relation import Path
+from dbt.adapters.contracts.relation import RelationType
 from dbt.adapters.duckdb.column import DuckDBColumn
 from dbt.adapters.duckdb.connections import DuckDBConnectionManager
 from dbt.adapters.duckdb.relation import DuckDBRelation
 from dbt.adapters.duckdb.utils import TargetConfig
 from dbt.adapters.duckdb.utils import TargetLocation
 from dbt.adapters.sql import SQLAdapter
-from dbt.context.providers import RuntimeConfigObject
-from dbt.contracts.connection import AdapterResponse
-from dbt.contracts.graph.nodes import ColumnLevelConstraint
-from dbt.contracts.graph.nodes import ConstraintType
-from dbt.contracts.relation import Path
-from dbt.contracts.relation import RelationType
-from dbt.exceptions import DbtInternalError
-from dbt.exceptions import DbtRuntimeError
+
 
 TEMP_SCHEMA_NAME = "temp_schema_name"
 DEFAULT_TEMP_SCHEMA_NAME = "dbt_temp"
 
 if TYPE_CHECKING:
     import agate
 
@@ -99,15 +100,15 @@
     def store_relation(
         self,
         plugin_name: str,
         relation: DuckDBRelation,
         column_list: Sequence[BaseColumn],
         path: str,
         format: str,
-        config: RuntimeConfigObject,
+        config: Any,
     ) -> None:
         target_config = TargetConfig(
             relation=relation,
             column_list=column_list,
             config=config,
             location=TargetLocation(path=path, format=format),
         )
```

### Comparing `dbt_duckdb-1.7.5/dbt/adapters/duckdb/plugins/__init__.py` & `dbt_duckdb-1.8.0/dbt/adapters/duckdb/plugins/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import importlib
 import os
 from typing import Any
 from typing import Dict
 from typing import Optional
 
+from dbt_common.dataclass_schema import dbtClassMixin
 from duckdb import DuckDBPyConnection
 
 from ..credentials import DuckDBCredentials
 from ..utils import SourceConfig
 from ..utils import TargetConfig
-from dbt.dataclass_schema import dbtClassMixin
 
 
 class PluginConfig(dbtClassMixin):
     """A helper class for defining the configuration settings a particular plugin uses."""
 
     pass
```

### Comparing `dbt_duckdb-1.7.5/dbt/adapters/duckdb/plugins/delta.py` & `dbt_duckdb-1.8.0/dbt/adapters/duckdb/plugins/delta.py`

 * *Files identical despite different names*

### Comparing `dbt_duckdb-1.7.5/dbt/adapters/duckdb/plugins/excel.py` & `dbt_duckdb-1.8.0/dbt/adapters/duckdb/plugins/excel.py`

 * *Files identical despite different names*

### Comparing `dbt_duckdb-1.7.5/dbt/adapters/duckdb/plugins/glue.py` & `dbt_duckdb-1.8.0/dbt/adapters/duckdb/plugins/glue.py`

 * *Files identical despite different names*

### Comparing `dbt_duckdb-1.7.5/dbt/adapters/duckdb/plugins/gsheet.py` & `dbt_duckdb-1.8.0/dbt/adapters/duckdb/plugins/gsheet.py`

 * *Files identical despite different names*

### Comparing `dbt_duckdb-1.7.5/dbt/adapters/duckdb/plugins/iceberg.py` & `dbt_duckdb-1.8.0/dbt/adapters/duckdb/plugins/iceberg.py`

 * *Files identical despite different names*

### Comparing `dbt_duckdb-1.7.5/dbt/adapters/duckdb/plugins/motherduck.py` & `dbt_duckdb-1.8.0/dbt/adapters/duckdb/plugins/motherduck.py`

 * *Files identical despite different names*

### Comparing `dbt_duckdb-1.7.5/dbt/adapters/duckdb/plugins/pd_utils.py` & `dbt_duckdb-1.8.0/dbt/adapters/duckdb/plugins/pd_utils.py`

 * *Files identical despite different names*

### Comparing `dbt_duckdb-1.7.5/dbt/adapters/duckdb/plugins/postgres.py` & `dbt_duckdb-1.8.0/dbt/adapters/duckdb/plugins/postgres.py`

 * *Files identical despite different names*

### Comparing `dbt_duckdb-1.7.5/dbt/adapters/duckdb/plugins/sqlalchemy.py` & `dbt_duckdb-1.8.0/dbt/adapters/duckdb/plugins/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `dbt_duckdb-1.7.5/dbt/adapters/duckdb/relation.py` & `dbt_duckdb-1.8.0/dbt/adapters/duckdb/relation.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,24 +3,38 @@
 from typing import Any
 from typing import Optional
 from typing import Type
 
 from .connections import DuckDBConnectionManager
 from .utils import SourceConfig
 from dbt.adapters.base.relation import BaseRelation
-from dbt.adapters.base.relation import Self
-from dbt.contracts.graph.nodes import SourceDefinition
+from dbt.adapters.contracts.relation import HasQuoting
+from dbt.adapters.contracts.relation import RelationConfig
 
 
 @dataclass(frozen=True, eq=False, repr=False)
 class DuckDBRelation(BaseRelation):
     external: Optional[str] = None
 
     @classmethod
-    def create_from_source(cls: Type[Self], source: SourceDefinition, **kwargs: Any) -> Self:
+    def create_from(
+        cls: Type["DuckDBRelation"],
+        quoting: HasQuoting,
+        relation_config: RelationConfig,
+        **kwargs: Any,
+    ) -> "DuckDBRelation":
+        if relation_config.resource_type == "source":
+            return cls.create_from_source(quoting, relation_config, **kwargs)
+        else:
+            return super().create_from(quoting, relation_config, **kwargs)
+
+    @classmethod
+    def create_from_source(
+        cls: Type["DuckDBRelation"], quoting: HasQuoting, source: RelationConfig, **kwargs: Any
+    ) -> "DuckDBRelation":
         """
         This method creates a new DuckDBRelation instance from a source definition.
         It first checks if a 'plugin' is defined in the meta argument for the source or its parent configuration.
         If a 'plugin' is defined, it uses the environment associated with this run to get the name of the source that we should reference in the compiled model.
         If an 'external_location' is defined, it formats the location based on the 'formatter' defined in the source configuration.
         If the 'formatter' is not recognized, it raises a ValueError.
         Finally, it calls the parent class's create_from_source method to create the DuckDBRelation instance.
@@ -55,14 +69,14 @@
                 )
 
             # If it's a function call or already has single quotes, don't add them
             if "(" not in ext_location and not ext_location.startswith("'"):
                 ext_location = f"'{ext_location}'"
             kwargs["external"] = ext_location
 
-        return super().create_from_source(source, **kwargs)  # type: ignore
+        return super().create_from(quoting, source, **kwargs)  # type: ignore
 
     def render(self) -> str:
         if self.external:
             return self.external
         else:
             return super().render()
```

### Comparing `dbt_duckdb-1.7.5/dbt/adapters/duckdb/utils.py` & `dbt_duckdb-1.8.0/dbt/adapters/duckdb/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,16 +3,17 @@
 from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Sequence
 
 from dbt.adapters.base.column import Column
 from dbt.adapters.base.relation import BaseRelation
-from dbt.context.providers import RuntimeConfigObject
-from dbt.contracts.graph.nodes import SourceDefinition
+from dbt.adapters.contracts.relation import RelationConfig
+# TODO
+# from dbt.context.providers import RuntimeConfigObject
 
 
 @dataclass
 class SourceConfig:
     name: str
     identifier: str
     schema: str
@@ -43,19 +44,19 @@
             "database": self.database,
             "tags": self.tags,
         }
         base.update(self.meta)
         return base
 
     @classmethod
-    def create_from_source(cls, source: SourceDefinition) -> "SourceConfig":
-        meta = source.source_meta.copy()
-        meta.update(source.meta)
+    def create_from_source(cls, source: RelationConfig) -> "SourceConfig":
+        meta = source.meta.copy()
         # Use the config properties as well if they are present
-        meta.update(source.config._extra)
+        config_properties = source.config.extra if source.config else {}
+        meta.update(config_properties)
         return SourceConfig(
             name=source.name,
             identifier=source.identifier,
             schema=source.schema,
             database=source.database,
             meta=meta,
             tags=source.tags or [],
@@ -71,15 +72,15 @@
         return {"path": self.path, "format": self.format}
 
 
 @dataclass
 class TargetConfig:
     relation: BaseRelation
     column_list: Sequence[Column]
-    config: RuntimeConfigObject
+    config: Any  # TODO
     location: Optional[TargetLocation] = None
 
     def as_dict(self) -> Dict[str, Any]:
         base = {
             "relation": self.relation.to_dict(),
             "column_list": [{"column": c.column, "dtype": c.dtype} for c in self.column_list],
             "config": self.config,
```

### Comparing `dbt_duckdb-1.7.5/dbt/include/duckdb/macros/adapters.sql` & `dbt_duckdb-1.8.0/dbt/include/duckdb/macros/adapters.sql`

 * *Files identical despite different names*

### Comparing `dbt_duckdb-1.7.5/dbt/include/duckdb/macros/catalog.sql` & `dbt_duckdb-1.8.0/dbt/include/duckdb/macros/catalog.sql`

 * *Files identical despite different names*

### Comparing `dbt_duckdb-1.7.5/dbt/include/duckdb/macros/columns.sql` & `dbt_duckdb-1.8.0/dbt/include/duckdb/macros/columns.sql`

 * *Files identical despite different names*

### Comparing `dbt_duckdb-1.7.5/dbt/include/duckdb/macros/incremental_helper.sql` & `dbt_duckdb-1.8.0/dbt/include/duckdb/macros/incremental_helper.sql`

 * *Files identical despite different names*

### Comparing `dbt_duckdb-1.7.5/dbt/include/duckdb/macros/materializations/external.sql` & `dbt_duckdb-1.8.0/dbt/include/duckdb/macros/materializations/external.sql`

 * *Files identical despite different names*

### Comparing `dbt_duckdb-1.7.5/dbt/include/duckdb/macros/materializations/incremental.sql` & `dbt_duckdb-1.8.0/dbt/include/duckdb/macros/materializations/incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt_duckdb-1.7.5/dbt/include/duckdb/macros/materializations/table.sql` & `dbt_duckdb-1.8.0/dbt/include/duckdb/macros/materializations/table.sql`

 * *Files identical despite different names*

### Comparing `dbt_duckdb-1.7.5/dbt/include/duckdb/macros/persist_docs.sql` & `dbt_duckdb-1.8.0/dbt/include/duckdb/macros/persist_docs.sql`

 * *Files identical despite different names*

### Comparing `dbt_duckdb-1.7.5/dbt/include/duckdb/macros/seed.sql` & `dbt_duckdb-1.8.0/dbt/include/duckdb/macros/seed.sql`

 * *Files identical despite different names*

### Comparing `dbt_duckdb-1.7.5/dbt/include/duckdb/macros/snapshot_helper.sql` & `dbt_duckdb-1.8.0/dbt/include/duckdb/macros/snapshot_helper.sql`

 * *Files identical despite different names*

### Comparing `dbt_duckdb-1.7.5/dbt/include/duckdb/macros/utils/listagg.sql` & `dbt_duckdb-1.8.0/dbt/include/duckdb/macros/utils/listagg.sql`

 * *Files identical despite different names*

### Comparing `dbt_duckdb-1.7.5/dbt/include/duckdb/macros/utils/upstream.sql` & `dbt_duckdb-1.8.0/dbt/include/duckdb/macros/utils/upstream.sql`

 * *Files identical despite different names*

### Comparing `dbt_duckdb-1.7.5/dbt_duckdb.egg-info/PKG-INFO` & `dbt_duckdb-1.8.0/dbt_duckdb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-duckdb
-Version: 1.7.5
+Version: 1.8.0
 Summary: The duckdb adapter plugin for dbt (data build tool)
 Home-page: https://github.com/jwills/dbt-duckdb
 Author: Josh Wills
 Author-email: joshwills+dbt@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
@@ -13,16 +13,18 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: dbt-core~=1.7.0
+Requires-Dist: dbt-common<2,>=1
+Requires-Dist: dbt-adapters<2,>=1
 Requires-Dist: duckdb>=0.7.0
+Requires-Dist: dbt-core>=1.8.0
 Provides-Extra: glue
 Requires-Dist: boto3; extra == "glue"
 Requires-Dist: mypy-boto3-glue; extra == "glue"
 Provides-Extra: md
 Requires-Dist: duckdb>=0.10.2; extra == "md"
 
 ## dbt-duckdb
```

### Comparing `dbt_duckdb-1.7.5/dbt_duckdb.egg-info/SOURCES.txt` & `dbt_duckdb-1.8.0/dbt_duckdb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt_duckdb-1.7.5/setup.py` & `dbt_duckdb-1.8.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -33,16 +33,19 @@
     long_description_content_type="text/markdown",
     author="Josh Wills",
     author_email="joshwills+dbt@gmail.com",
     url="https://github.com/jwills/dbt-duckdb",
     packages=find_namespace_packages(include=["dbt", "dbt.*"]),
     include_package_data=True,
     install_requires=[
-        "dbt-core~=1.7.0",
+        "dbt-common>=1,<2",
+        "dbt-adapters>=1,<2",
         "duckdb>=0.7.0",
+        # add dbt-core to ensure backwards compatibility of installation, this is not a functional dependency
+        "dbt-core>=1.8.0",
     ],
     extras_require={"glue": ["boto3", "mypy-boto3-glue"], "md": ["duckdb>=0.10.2"]},
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: Microsoft :: Windows",
         "Operating System :: MacOS :: MacOS X",
```

