# Comparing `tmp/dbt-trino-1.8.0b2.tar.gz` & `tmp/dbt-trino-1.8.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-trino-1.8.0b2.tar", last modified: Mon Apr  8 18:32:24 2024, max compression
+gzip compressed data, was "dbt-trino-1.8.0b3.tar", last modified: Tue Apr 23 09:50:41 2024, max compression
```

## Comparing `dbt-trino-1.8.0b2.tar` & `dbt-trino-1.8.0b3.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:32:24.310373 dbt-trino-1.8.0b2/
--rw-r--r--   0 runner    (1001) docker     (127)    11350 2024-04-08 18:31:53.000000 dbt-trino-1.8.0b2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     7329 2024-04-08 18:32:24.310373 dbt-trino-1.8.0b2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6447 2024-04-08 18:31:53.000000 dbt-trino-1.8.0b2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:32:24.306373 dbt-trino-1.8.0b2/dbt/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:32:24.306373 dbt-trino-1.8.0b2/dbt/adapters/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:32:24.306373 dbt-trino-1.8.0b2/dbt/adapters/trino/
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-08 18:31:53.000000 dbt-trino-1.8.0b2/dbt/adapters/trino/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-08 18:31:53.000000 dbt-trino-1.8.0b2/dbt/adapters/trino/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3900 2024-04-08 18:31:53.000000 dbt-trino-1.8.0b2/dbt/adapters/trino/column.py
--rw-r--r--   0 runner    (1001) docker     (127)    17304 2024-04-08 18:31:53.000000 dbt-trino-1.8.0b2/dbt/adapters/trino/connections.py
--rw-r--r--   0 runner    (1001) docker     (127)     2642 2024-04-08 18:31:53.000000 dbt-trino-1.8.0b2/dbt/adapters/trino/impl.py
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-04-08 18:31:53.000000 dbt-trino-1.8.0b2/dbt/adapters/trino/relation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:32:24.306373 dbt-trino-1.8.0b2/dbt/include/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:32:24.306373 dbt-trino-1.8.0b2/dbt/include/trino/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-08 18:31:53.000000 dbt-trino-1.8.0b2/dbt/include/trino/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-08 18:31:53.000000 dbt-trino-1.8.0b2/dbt/include/trino/dbt_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:32:24.306373 dbt-trino-1.8.0b2/dbt/include/trino/macros/
--rw-r--r--   0 runner    (1001) docker     (127)    10767 2024-04-08 18:31:53.000000 dbt-trino-1.8.0b2/dbt/include/trino/macros/adapters.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-04-08 18:31:53.000000 dbt-trino-1.8.0b2/dbt/include/trino/macros/apply_grants.sql
--rw-r--r--   0 runner    (1001) docker     (127)     5484 2024-04-08 18:31:53.000000 dbt-trino-1.8.0b2/dbt/include/trino/macros/catalog.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:32:24.310373 dbt-trino-1.8.0b2/dbt/include/trino/macros/materializations/
--rw-r--r--   0 runner    (1001) docker     (127)     8740 2024-04-08 18:31:53.000000 dbt-trino-1.8.0b2/dbt/include/trino/macros/materializations/incremental.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-04-08 18:31:53.000000 dbt-trino-1.8.0b2/dbt/include/trino/macros/materializations/materialized_view.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:32:24.310373 dbt-trino-1.8.0b2/dbt/include/trino/macros/materializations/seeds/
--rw-r--r--   0 runner    (1001) docker     (127)     3547 2024-04-08 18:31:53.000000 dbt-trino-1.8.0b2/dbt/include/trino/macros/materializations/seeds/helpers.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-04-08 18:31:53.000000 dbt-trino-1.8.0b2/dbt/include/trino/macros/materializations/snapshot.sql
--rw-r--r--   0 runner    (1001) docker     (127)     3150 2024-04-08 18:31:53.000000 dbt-trino-1.8.0b2/dbt/include/trino/macros/materializations/table.sql
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-08 18:31:53.000000 dbt-trino-1.8.0b2/dbt/include/trino/macros/materializations/view.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:32:24.310373 dbt-trino-1.8.0b2/dbt/include/trino/macros/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-08 18:31:53.000000 dbt-trino-1.8.0b2/dbt/include/trino/macros/utils/any_value.sql
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-08 18:31:53.000000 dbt-trino-1.8.0b2/dbt/include/trino/macros/utils/array_append.sql
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-08 18:31:53.000000 dbt-trino-1.8.0b2/dbt/include/trino/macros/utils/array_concat.sql
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-08 18:31:53.000000 dbt-trino-1.8.0b2/dbt/include/trino/macros/utils/array_construct.sql
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-08 18:31:53.000000 dbt-trino-1.8.0b2/dbt/include/trino/macros/utils/bool_or.sql
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-08 18:31:53.000000 dbt-trino-1.8.0b2/dbt/include/trino/macros/utils/datatypes.sql
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-08 18:31:53.000000 dbt-trino-1.8.0b2/dbt/include/trino/macros/utils/date_spine.sql
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-08 18:31:53.000000 dbt-trino-1.8.0b2/dbt/include/trino/macros/utils/date_trunc.sql
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-08 18:31:53.000000 dbt-trino-1.8.0b2/dbt/include/trino/macros/utils/dateadd.sql
--rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-04-08 18:31:53.000000 dbt-trino-1.8.0b2/dbt/include/trino/macros/utils/datediff.sql
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-08 18:31:53.000000 dbt-trino-1.8.0b2/dbt/include/trino/macros/utils/hash.sql
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-08 18:31:53.000000 dbt-trino-1.8.0b2/dbt/include/trino/macros/utils/listagg.sql
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-08 18:31:53.000000 dbt-trino-1.8.0b2/dbt/include/trino/macros/utils/right.sql
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-08 18:31:53.000000 dbt-trino-1.8.0b2/dbt/include/trino/macros/utils/safe_cast.sql
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-08 18:31:53.000000 dbt-trino-1.8.0b2/dbt/include/trino/macros/utils/split_part.sql
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-08 18:31:53.000000 dbt-trino-1.8.0b2/dbt/include/trino/macros/utils/timestamps.sql
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-08 18:31:53.000000 dbt-trino-1.8.0b2/dbt/include/trino/sample_profiles.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:32:24.310373 dbt-trino-1.8.0b2/dbt_trino.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7329 2024-04-08 18:32:24.000000 dbt-trino-1.8.0b2/dbt_trino.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-04-08 18:32:24.000000 dbt-trino-1.8.0b2/dbt_trino.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 18:32:24.000000 dbt-trino-1.8.0b2/dbt_trino.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 18:32:24.000000 dbt-trino-1.8.0b2/dbt_trino.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-08 18:32:24.000000 dbt-trino-1.8.0b2/dbt_trino.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-08 18:32:24.000000 dbt-trino-1.8.0b2/dbt_trino.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 18:32:24.310373 dbt-trino-1.8.0b2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3402 2024-04-08 18:31:53.000000 dbt-trino-1.8.0b2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 09:50:41.344568 dbt-trino-1.8.0b3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11350 2024-04-23 09:50:11.000000 dbt-trino-1.8.0b3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     7329 2024-04-23 09:50:41.344568 dbt-trino-1.8.0b3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6447 2024-04-23 09:50:11.000000 dbt-trino-1.8.0b3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 09:50:41.336568 dbt-trino-1.8.0b3/dbt/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 09:50:41.336568 dbt-trino-1.8.0b3/dbt/adapters/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 09:50:41.340568 dbt-trino-1.8.0b3/dbt/adapters/trino/
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-23 09:50:11.000000 dbt-trino-1.8.0b3/dbt/adapters/trino/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-23 09:50:11.000000 dbt-trino-1.8.0b3/dbt/adapters/trino/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3900 2024-04-23 09:50:11.000000 dbt-trino-1.8.0b3/dbt/adapters/trino/column.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17304 2024-04-23 09:50:11.000000 dbt-trino-1.8.0b3/dbt/adapters/trino/connections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2775 2024-04-23 09:50:11.000000 dbt-trino-1.8.0b3/dbt/adapters/trino/impl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-04-23 09:50:11.000000 dbt-trino-1.8.0b3/dbt/adapters/trino/relation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 09:50:41.336568 dbt-trino-1.8.0b3/dbt/include/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 09:50:41.340568 dbt-trino-1.8.0b3/dbt/include/trino/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-23 09:50:11.000000 dbt-trino-1.8.0b3/dbt/include/trino/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-23 09:50:11.000000 dbt-trino-1.8.0b3/dbt/include/trino/dbt_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 09:50:41.340568 dbt-trino-1.8.0b3/dbt/include/trino/macros/
+-rw-r--r--   0 runner    (1001) docker     (127)    10767 2024-04-23 09:50:11.000000 dbt-trino-1.8.0b3/dbt/include/trino/macros/adapters.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-04-23 09:50:11.000000 dbt-trino-1.8.0b3/dbt/include/trino/macros/apply_grants.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     5484 2024-04-23 09:50:11.000000 dbt-trino-1.8.0b3/dbt/include/trino/macros/catalog.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 09:50:41.340568 dbt-trino-1.8.0b3/dbt/include/trino/macros/materializations/
+-rw-r--r--   0 runner    (1001) docker     (127)     8740 2024-04-23 09:50:11.000000 dbt-trino-1.8.0b3/dbt/include/trino/macros/materializations/incremental.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-04-23 09:50:11.000000 dbt-trino-1.8.0b3/dbt/include/trino/macros/materializations/materialized_view.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 09:50:41.340568 dbt-trino-1.8.0b3/dbt/include/trino/macros/materializations/seeds/
+-rw-r--r--   0 runner    (1001) docker     (127)     3547 2024-04-23 09:50:11.000000 dbt-trino-1.8.0b3/dbt/include/trino/macros/materializations/seeds/helpers.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-04-23 09:50:11.000000 dbt-trino-1.8.0b3/dbt/include/trino/macros/materializations/snapshot.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     3150 2024-04-23 09:50:11.000000 dbt-trino-1.8.0b3/dbt/include/trino/macros/materializations/table.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-23 09:50:11.000000 dbt-trino-1.8.0b3/dbt/include/trino/macros/materializations/view.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 09:50:41.344568 dbt-trino-1.8.0b3/dbt/include/trino/macros/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-23 09:50:11.000000 dbt-trino-1.8.0b3/dbt/include/trino/macros/utils/any_value.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-23 09:50:11.000000 dbt-trino-1.8.0b3/dbt/include/trino/macros/utils/array_append.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-23 09:50:11.000000 dbt-trino-1.8.0b3/dbt/include/trino/macros/utils/array_concat.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-23 09:50:11.000000 dbt-trino-1.8.0b3/dbt/include/trino/macros/utils/array_construct.sql
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-23 09:50:11.000000 dbt-trino-1.8.0b3/dbt/include/trino/macros/utils/bool_or.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-23 09:50:11.000000 dbt-trino-1.8.0b3/dbt/include/trino/macros/utils/datatypes.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-23 09:50:11.000000 dbt-trino-1.8.0b3/dbt/include/trino/macros/utils/date_spine.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-23 09:50:11.000000 dbt-trino-1.8.0b3/dbt/include/trino/macros/utils/date_trunc.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-23 09:50:11.000000 dbt-trino-1.8.0b3/dbt/include/trino/macros/utils/dateadd.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-04-23 09:50:11.000000 dbt-trino-1.8.0b3/dbt/include/trino/macros/utils/datediff.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-23 09:50:11.000000 dbt-trino-1.8.0b3/dbt/include/trino/macros/utils/hash.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-23 09:50:11.000000 dbt-trino-1.8.0b3/dbt/include/trino/macros/utils/listagg.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-23 09:50:11.000000 dbt-trino-1.8.0b3/dbt/include/trino/macros/utils/right.sql
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-23 09:50:11.000000 dbt-trino-1.8.0b3/dbt/include/trino/macros/utils/safe_cast.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-23 09:50:11.000000 dbt-trino-1.8.0b3/dbt/include/trino/macros/utils/split_part.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-23 09:50:11.000000 dbt-trino-1.8.0b3/dbt/include/trino/macros/utils/timestamps.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-23 09:50:11.000000 dbt-trino-1.8.0b3/dbt/include/trino/sample_profiles.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 09:50:41.344568 dbt-trino-1.8.0b3/dbt_trino.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7329 2024-04-23 09:50:41.000000 dbt-trino-1.8.0b3/dbt_trino.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-04-23 09:50:41.000000 dbt-trino-1.8.0b3/dbt_trino.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 09:50:41.000000 dbt-trino-1.8.0b3/dbt_trino.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 09:50:41.000000 dbt-trino-1.8.0b3/dbt_trino.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-23 09:50:41.000000 dbt-trino-1.8.0b3/dbt_trino.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-23 09:50:41.000000 dbt-trino-1.8.0b3/dbt_trino.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 09:50:41.344568 dbt-trino-1.8.0b3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3405 2024-04-23 09:50:11.000000 dbt-trino-1.8.0b3/setup.py
```

### Comparing `dbt-trino-1.8.0b2/LICENSE.txt` & `dbt-trino-1.8.0b3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dbt-trino-1.8.0b2/PKG-INFO` & `dbt-trino-1.8.0b3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-trino
-Version: 1.8.0b2
+Version: 1.8.0b3
 Summary: The trino adapter plugin for dbt (data build tool)
 Home-page: https://github.com/starburstdata/dbt-trino
 Author: Starburst Data
 Author-email: info@starburstdata.com
 License: Apache License 2.0
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
@@ -56,15 +56,15 @@
 
 `dbt-trino` adapter uses [Trino](https://trino.io/) as a underlying query engine to perform query federation across disperse data sources. Trino connects to multiple and diverse data sources ([available connectors](https://trino.io/docs/current/connector.html)) via one dbt connection and process SQL queries at scale. Transformations defined in dbt are passed to Trino which handles these SQL transformation queries and translates them to queries specific to the systems it connects to create tables or views and manipulate data.
 
 This repository represents a fork of the [dbt-presto](https://github.com/dbt-labs/dbt-presto) with adaptations to make it work with Trino.
 
 ## Compatibility
 
-This dbt plugin has been tested against `Trino` version `439`, `Starburst Enterprise` version `435-e.1` and `Starburst Galaxy`.
+This dbt plugin has been tested against `Trino` version `445`, `Starburst Enterprise` version `435-e.4` and `Starburst Galaxy`.
 
 ## Setup & Configuration
 
 For information on installing and configuring your profile to authenticate to Trino or Starburst, please refer to [Starburst and Trino Setup](https://docs.getdbt.com/reference/warehouse-setups/trino-setup) in the dbt docs.
 
 ### Trino- and Starburst-specific configuration
```

### Comparing `dbt-trino-1.8.0b2/README.md` & `dbt-trino-1.8.0b3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
 `dbt-trino` adapter uses [Trino](https://trino.io/) as a underlying query engine to perform query federation across disperse data sources. Trino connects to multiple and diverse data sources ([available connectors](https://trino.io/docs/current/connector.html)) via one dbt connection and process SQL queries at scale. Transformations defined in dbt are passed to Trino which handles these SQL transformation queries and translates them to queries specific to the systems it connects to create tables or views and manipulate data.
 
 This repository represents a fork of the [dbt-presto](https://github.com/dbt-labs/dbt-presto) with adaptations to make it work with Trino.
 
 ## Compatibility
 
-This dbt plugin has been tested against `Trino` version `439`, `Starburst Enterprise` version `435-e.1` and `Starburst Galaxy`.
+This dbt plugin has been tested against `Trino` version `445`, `Starburst Enterprise` version `435-e.4` and `Starburst Galaxy`.
 
 ## Setup & Configuration
 
 For information on installing and configuring your profile to authenticate to Trino or Starburst, please refer to [Starburst and Trino Setup](https://docs.getdbt.com/reference/warehouse-setups/trino-setup) in the dbt docs.
 
 ### Trino- and Starburst-specific configuration
```

### Comparing `dbt-trino-1.8.0b2/dbt/adapters/trino/__init__.py` & `dbt-trino-1.8.0b3/dbt/adapters/trino/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-trino-1.8.0b2/dbt/adapters/trino/column.py` & `dbt-trino-1.8.0b3/dbt/adapters/trino/column.py`

 * *Files identical despite different names*

### Comparing `dbt-trino-1.8.0b2/dbt/adapters/trino/connections.py` & `dbt-trino-1.8.0b3/dbt/adapters/trino/connections.py`

 * *Files identical despite different names*

### Comparing `dbt-trino-1.8.0b2/dbt/adapters/trino/impl.py` & `dbt-trino-1.8.0b3/dbt/adapters/trino/impl.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,14 +37,17 @@
     }
 
     _capabilities: CapabilityDict = CapabilityDict(
         {
             Capability.SchemaMetadataByRelations: CapabilitySupport(support=Support.Full),
             # No information about last table modification in information_schema.tables
             Capability.TableLastModifiedMetadata: CapabilitySupport(support=Support.Unsupported),
+            Capability.TableLastModifiedMetadataBatch: CapabilitySupport(
+                support=Support.Unsupported
+            ),
         }
     )
 
     @classmethod
     def date_function(cls):
         return "datenow()"
```

### Comparing `dbt-trino-1.8.0b2/dbt/adapters/trino/relation.py` & `dbt-trino-1.8.0b3/dbt/adapters/trino/relation.py`

 * *Files identical despite different names*

### Comparing `dbt-trino-1.8.0b2/dbt/include/trino/macros/adapters.sql` & `dbt-trino-1.8.0b3/dbt/include/trino/macros/adapters.sql`

 * *Files identical despite different names*

### Comparing `dbt-trino-1.8.0b2/dbt/include/trino/macros/apply_grants.sql` & `dbt-trino-1.8.0b3/dbt/include/trino/macros/apply_grants.sql`

 * *Files identical despite different names*

### Comparing `dbt-trino-1.8.0b2/dbt/include/trino/macros/catalog.sql` & `dbt-trino-1.8.0b3/dbt/include/trino/macros/catalog.sql`

 * *Files identical despite different names*

### Comparing `dbt-trino-1.8.0b2/dbt/include/trino/macros/materializations/incremental.sql` & `dbt-trino-1.8.0b3/dbt/include/trino/macros/materializations/incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt-trino-1.8.0b2/dbt/include/trino/macros/materializations/materialized_view.sql` & `dbt-trino-1.8.0b3/dbt/include/trino/macros/materializations/materialized_view.sql`

 * *Files identical despite different names*

### Comparing `dbt-trino-1.8.0b2/dbt/include/trino/macros/materializations/seeds/helpers.sql` & `dbt-trino-1.8.0b3/dbt/include/trino/macros/materializations/seeds/helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt-trino-1.8.0b2/dbt/include/trino/macros/materializations/snapshot.sql` & `dbt-trino-1.8.0b3/dbt/include/trino/macros/materializations/snapshot.sql`

 * *Files identical despite different names*

### Comparing `dbt-trino-1.8.0b2/dbt/include/trino/macros/materializations/table.sql` & `dbt-trino-1.8.0b3/dbt/include/trino/macros/materializations/table.sql`

 * *Files identical despite different names*

### Comparing `dbt-trino-1.8.0b2/dbt/include/trino/macros/utils/date_spine.sql` & `dbt-trino-1.8.0b3/dbt/include/trino/macros/utils/date_spine.sql`

 * *Files identical despite different names*

### Comparing `dbt-trino-1.8.0b2/dbt/include/trino/macros/utils/datediff.sql` & `dbt-trino-1.8.0b3/dbt/include/trino/macros/utils/datediff.sql`

 * *Files identical despite different names*

### Comparing `dbt-trino-1.8.0b2/dbt/include/trino/sample_profiles.yml` & `dbt-trino-1.8.0b3/dbt/include/trino/sample_profiles.yml`

 * *Files identical despite different names*

### Comparing `dbt-trino-1.8.0b2/dbt_trino.egg-info/PKG-INFO` & `dbt-trino-1.8.0b3/dbt_trino.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-trino
-Version: 1.8.0b2
+Version: 1.8.0b3
 Summary: The trino adapter plugin for dbt (data build tool)
 Home-page: https://github.com/starburstdata/dbt-trino
 Author: Starburst Data
 Author-email: info@starburstdata.com
 License: Apache License 2.0
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
@@ -56,15 +56,15 @@
 
 `dbt-trino` adapter uses [Trino](https://trino.io/) as a underlying query engine to perform query federation across disperse data sources. Trino connects to multiple and diverse data sources ([available connectors](https://trino.io/docs/current/connector.html)) via one dbt connection and process SQL queries at scale. Transformations defined in dbt are passed to Trino which handles these SQL transformation queries and translates them to queries specific to the systems it connects to create tables or views and manipulate data.
 
 This repository represents a fork of the [dbt-presto](https://github.com/dbt-labs/dbt-presto) with adaptations to make it work with Trino.
 
 ## Compatibility
 
-This dbt plugin has been tested against `Trino` version `439`, `Starburst Enterprise` version `435-e.1` and `Starburst Galaxy`.
+This dbt plugin has been tested against `Trino` version `445`, `Starburst Enterprise` version `435-e.4` and `Starburst Galaxy`.
 
 ## Setup & Configuration
 
 For information on installing and configuring your profile to authenticate to Trino or Starburst, please refer to [Starburst and Trino Setup](https://docs.getdbt.com/reference/warehouse-setups/trino-setup) in the dbt docs.
 
 ### Trino- and Starburst-specific configuration
```

### Comparing `dbt-trino-1.8.0b2/dbt_trino.egg-info/SOURCES.txt` & `dbt-trino-1.8.0b3/dbt_trino.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt-trino-1.8.0b2/setup.py` & `dbt-trino-1.8.0b3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -72,19 +72,19 @@
             "include/trino/sample_profiles.yml",
             "include/trino/macros/*.sql",
             "include/trino/macros/*/*.sql",
             "include/trino/macros/*/*/*.sql",
         ]
     },
     install_requires=[
-        "dbt-common>=1.0.0,<2.0",
-        "dbt-adapters>=1.0.0,<2.0",
+        "dbt-common>=1.0.1,<2.0",
+        "dbt-adapters>=1.1.0rc1,<2.0",
         "trino~=0.326",
         # add dbt-core to ensure backwards compatibility of installation, this is not a functional dependency
-        "dbt-core>=1.8.0b2",
+        "dbt-core>=1.8.0b3",
     ],
     zip_safe=False,
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: Microsoft :: Windows",
         "Operating System :: MacOS :: MacOS X",
```

