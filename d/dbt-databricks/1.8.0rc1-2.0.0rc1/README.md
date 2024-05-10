# Comparing `tmp/dbt-databricks-1.8.0rc1.tar.gz` & `tmp/dbt-databricks-2.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-databricks-1.8.0rc1.tar", last modified: Fri May 10 20:26:57 2024, max compression
+gzip compressed data, was "dbt-databricks-2.0.0rc1.tar", last modified: Wed May  8 19:39:36 2024, max compression
```

## Comparing `dbt-databricks-1.8.0rc1.tar` & `dbt-databricks-2.0.0rc1.tar`

### file list

```diff
@@ -1,112 +1,112 @@
-drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-05-10 20:26:57.862320 dbt-databricks-1.8.0rc1/
--rw-r--r--   0 ben.cassell   (502) staff       (20)       47 2024-05-10 19:26:33.000000 dbt-databricks-1.8.0rc1/MANIFEST.in
--rw-r--r--   0 ben.cassell   (502) staff       (20)     6131 2024-05-10 20:26:57.862125 dbt-databricks-1.8.0rc1/PKG-INFO
--rw-r--r--   0 ben.cassell   (502) staff       (20)     4624 2024-01-19 01:37:59.000000 dbt-databricks-1.8.0rc1/README.md
-drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-05-10 20:26:57.834407 dbt-databricks-1.8.0rc1/dbt/
--rw-r--r--   0 ben.cassell   (502) staff       (20)       76 2024-01-25 18:09:59.000000 dbt-databricks-1.8.0rc1/dbt/__init__.py
-drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-05-10 20:26:57.830064 dbt-databricks-1.8.0rc1/dbt/adapters/
-drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-05-10 20:26:57.838927 dbt-databricks-1.8.0rc1/dbt/adapters/databricks/
--rw-r--r--   0 ben.cassell   (502) staff       (20)      625 2024-05-10 19:26:33.000000 dbt-databricks-1.8.0rc1/dbt/adapters/databricks/__init__.py
--rw-r--r--   0 ben.cassell   (502) staff       (20)       26 2024-05-10 19:29:32.000000 dbt-databricks-1.8.0rc1/dbt/adapters/databricks/__version__.py
--rw-r--r--   0 ben.cassell   (502) staff       (20)     3513 2024-05-10 19:26:33.000000 dbt-databricks-1.8.0rc1/dbt/adapters/databricks/auth.py
--rw-r--r--   0 ben.cassell   (502) staff       (20)      707 2024-05-10 19:26:33.000000 dbt-databricks-1.8.0rc1/dbt/adapters/databricks/column.py
--rw-r--r--   0 ben.cassell   (502) staff       (20)    48111 2024-05-10 19:26:33.000000 dbt-databricks-1.8.0rc1/dbt/adapters/databricks/connections.py
--rw-r--r--   0 ben.cassell   (502) staff       (20)    15743 2024-05-10 19:26:33.000000 dbt-databricks-1.8.0rc1/dbt/adapters/databricks/credentials.py
-drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-05-10 20:26:57.840473 dbt-databricks-1.8.0rc1/dbt/adapters/databricks/events/
--rw-r--r--   0 ben.cassell   (502) staff       (20)      796 2024-05-10 19:26:33.000000 dbt-databricks-1.8.0rc1/dbt/adapters/databricks/events/base.py
--rw-r--r--   0 ben.cassell   (502) staff       (20)     3996 2024-05-10 19:26:33.000000 dbt-databricks-1.8.0rc1/dbt/adapters/databricks/events/connection_events.py
--rw-r--r--   0 ben.cassell   (502) staff       (20)      616 2024-05-10 19:26:33.000000 dbt-databricks-1.8.0rc1/dbt/adapters/databricks/events/credential_events.py
--rw-r--r--   0 ben.cassell   (502) staff       (20)     1826 2024-05-10 19:26:33.000000 dbt-databricks-1.8.0rc1/dbt/adapters/databricks/events/cursor_events.py
--rw-r--r--   0 ben.cassell   (502) staff       (20)      250 2024-05-10 19:26:33.000000 dbt-databricks-1.8.0rc1/dbt/adapters/databricks/events/other_events.py
--rw-r--r--   0 ben.cassell   (502) staff       (20)      842 2024-05-10 19:26:33.000000 dbt-databricks-1.8.0rc1/dbt/adapters/databricks/events/pipeline_events.py
--rw-r--r--   0 ben.cassell   (502) staff       (20)    30611 2024-05-10 19:26:33.000000 dbt-databricks-1.8.0rc1/dbt/adapters/databricks/impl.py
--rw-r--r--   0 ben.cassell   (502) staff       (20)      995 2024-05-10 19:26:33.000000 dbt-databricks-1.8.0rc1/dbt/adapters/databricks/logging.py
--rw-r--r--   0 ben.cassell   (502) staff       (20)    19165 2024-05-10 19:26:33.000000 dbt-databricks-1.8.0rc1/dbt/adapters/databricks/python_submissions.py
--rw-r--r--   0 ben.cassell   (502) staff       (20)     5313 2024-05-10 19:26:33.000000 dbt-databricks-1.8.0rc1/dbt/adapters/databricks/relation.py
-drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-05-10 20:26:57.843877 dbt-databricks-1.8.0rc1/dbt/adapters/databricks/relation_configs/
--rw-r--r--   0 ben.cassell   (502) staff       (20)     6157 2024-05-10 19:26:33.000000 dbt-databricks-1.8.0rc1/dbt/adapters/databricks/relation_configs/base.py
--rw-r--r--   0 ben.cassell   (502) staff       (20)     1085 2024-05-10 19:26:33.000000 dbt-databricks-1.8.0rc1/dbt/adapters/databricks/relation_configs/comment.py
--rw-r--r--   0 ben.cassell   (502) staff       (20)     1040 2024-05-10 19:26:33.000000 dbt-databricks-1.8.0rc1/dbt/adapters/databricks/relation_configs/incremental.py
--rw-r--r--   0 ben.cassell   (502) staff       (20)     1700 2024-05-10 19:26:33.000000 dbt-databricks-1.8.0rc1/dbt/adapters/databricks/relation_configs/materialized_view.py
--rw-r--r--   0 ben.cassell   (502) staff       (20)     1699 2024-05-10 19:26:33.000000 dbt-databricks-1.8.0rc1/dbt/adapters/databricks/relation_configs/partitioning.py
--rw-r--r--   0 ben.cassell   (502) staff       (20)     1182 2024-05-10 19:26:33.000000 dbt-databricks-1.8.0rc1/dbt/adapters/databricks/relation_configs/query.py
--rw-r--r--   0 ben.cassell   (502) staff       (20)     2955 2024-05-10 19:26:33.000000 dbt-databricks-1.8.0rc1/dbt/adapters/databricks/relation_configs/refresh.py
--rw-r--r--   0 ben.cassell   (502) staff       (20)     1802 2024-05-10 19:26:33.000000 dbt-databricks-1.8.0rc1/dbt/adapters/databricks/relation_configs/streaming_table.py
--rw-r--r--   0 ben.cassell   (502) staff       (20)     1850 2024-05-10 19:26:33.000000 dbt-databricks-1.8.0rc1/dbt/adapters/databricks/relation_configs/tags.py
--rw-r--r--   0 ben.cassell   (502) staff       (20)     2631 2024-05-10 19:26:33.000000 dbt-databricks-1.8.0rc1/dbt/adapters/databricks/relation_configs/tblproperties.py
--rw-r--r--   0 ben.cassell   (502) staff       (20)     2503 2024-05-10 19:26:33.000000 dbt-databricks-1.8.0rc1/dbt/adapters/databricks/utils.py
-drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-05-10 20:26:57.830875 dbt-databricks-1.8.0rc1/dbt/include/
-drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-05-10 20:26:57.844802 dbt-databricks-1.8.0rc1/dbt/include/databricks/
--rw-r--r--   0 ben.cassell   (502) staff       (20)       52 2023-05-30 21:40:46.000000 dbt-databricks-1.8.0rc1/dbt/include/databricks/__init__.py
--rw-r--r--   0 ben.cassell   (502) staff       (20)       77 2023-05-30 21:40:46.000000 dbt-databricks-1.8.0rc1/dbt/include/databricks/dbt_project.yml
-drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-05-10 20:26:57.833444 dbt-databricks-1.8.0rc1/dbt/include/databricks/macros/
-drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-05-10 20:26:57.846956 dbt-databricks-1.8.0rc1/dbt/include/databricks/macros/adapters/
--rw-r--r--   0 ben.cassell   (502) staff       (20)     3445 2024-05-10 19:26:33.000000 dbt-databricks-1.8.0rc1/dbt/include/databricks/macros/adapters/catalog.sql
--rw-r--r--   0 ben.cassell   (502) staff       (20)     2409 2024-03-26 16:27:09.000000 dbt-databricks-1.8.0rc1/dbt/include/databricks/macros/adapters/copy_into.sql
--rw-r--r--   0 ben.cassell   (502) staff       (20)      592 2024-05-10 19:26:33.000000 dbt-databricks-1.8.0rc1/dbt/include/databricks/macros/adapters/databricks_catalog.sql
--rw-r--r--   0 ben.cassell   (502) staff       (20)     5138 2024-05-10 19:26:33.000000 dbt-databricks-1.8.0rc1/dbt/include/databricks/macros/adapters/metadata.sql
--rw-r--r--   0 ben.cassell   (502) staff       (20)     1984 2024-05-10 19:26:33.000000 dbt-databricks-1.8.0rc1/dbt/include/databricks/macros/adapters/persist_docs.sql
--rw-r--r--   0 ben.cassell   (502) staff       (20)     3540 2024-05-10 19:26:33.000000 dbt-databricks-1.8.0rc1/dbt/include/databricks/macros/adapters/python.sql
--rw-r--r--   0 ben.cassell   (502) staff       (20)     1158 2024-05-10 19:26:33.000000 dbt-databricks-1.8.0rc1/dbt/include/databricks/macros/adapters/relation.sql
-drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-05-10 20:26:57.847182 dbt-databricks-1.8.0rc1/dbt/include/databricks/macros/etc/
--rw-r--r--   0 ben.cassell   (502) staff       (20)      648 2024-03-26 16:27:09.000000 dbt-databricks-1.8.0rc1/dbt/include/databricks/macros/etc/statement.sql
-drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-05-10 20:26:57.847513 dbt-databricks-1.8.0rc1/dbt/include/databricks/macros/get_custom_name/
--rw-r--r--   0 ben.cassell   (502) staff       (20)      458 2024-05-10 19:26:33.000000 dbt-databricks-1.8.0rc1/dbt/include/databricks/macros/get_custom_name/get_custom_database.sql
-drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-05-10 20:26:57.849717 dbt-databricks-1.8.0rc1/dbt/include/databricks/macros/materializations/
--rw-r--r--   0 ben.cassell   (502) staff       (20)     2803 2024-05-10 19:26:33.000000 dbt-databricks-1.8.0rc1/dbt/include/databricks/macros/materializations/clone.sql
-drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-05-10 20:26:57.850600 dbt-databricks-1.8.0rc1/dbt/include/databricks/macros/materializations/incremental/
--rw-r--r--   0 ben.cassell   (502) staff       (20)     4875 2024-05-10 19:26:33.000000 dbt-databricks-1.8.0rc1/dbt/include/databricks/macros/materializations/incremental/incremental.sql
--rw-r--r--   0 ben.cassell   (502) staff       (20)     5522 2024-05-10 19:26:33.000000 dbt-databricks-1.8.0rc1/dbt/include/databricks/macros/materializations/incremental/strategies.sql
--rw-r--r--   0 ben.cassell   (502) staff       (20)     1896 2024-05-10 19:17:14.000000 dbt-databricks-1.8.0rc1/dbt/include/databricks/macros/materializations/incremental/validate.sql
--rw-r--r--   0 ben.cassell   (502) staff       (20)     3657 2024-05-10 19:26:33.000000 dbt-databricks-1.8.0rc1/dbt/include/databricks/macros/materializations/materialized_view.sql
-drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-05-10 20:26:57.851284 dbt-databricks-1.8.0rc1/dbt/include/databricks/macros/materializations/seeds/
--rw-r--r--   0 ben.cassell   (502) staff       (20)     2849 2024-05-10 19:17:14.000000 dbt-databricks-1.8.0rc1/dbt/include/databricks/macros/materializations/seeds/helpers.sql
--rw-r--r--   0 ben.cassell   (502) staff       (20)     2477 2024-05-10 19:26:33.000000 dbt-databricks-1.8.0rc1/dbt/include/databricks/macros/materializations/seeds/seeds.sql
--rw-r--r--   0 ben.cassell   (502) staff       (20)     5397 2024-03-29 15:20:41.000000 dbt-databricks-1.8.0rc1/dbt/include/databricks/macros/materializations/snapshot.sql
--rw-r--r--   0 ben.cassell   (502) staff       (20)     3623 2024-05-10 19:26:33.000000 dbt-databricks-1.8.0rc1/dbt/include/databricks/macros/materializations/streaming_table.sql
--rw-r--r--   0 ben.cassell   (502) staff       (20)     1966 2024-05-10 19:26:33.000000 dbt-databricks-1.8.0rc1/dbt/include/databricks/macros/materializations/table.sql
--rw-r--r--   0 ben.cassell   (502) staff       (20)     1364 2024-05-10 19:26:33.000000 dbt-databricks-1.8.0rc1/dbt/include/databricks/macros/materializations/view.sql
-drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-05-10 20:26:57.854086 dbt-databricks-1.8.0rc1/dbt/include/databricks/macros/relations/
-drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-05-10 20:26:57.855284 dbt-databricks-1.8.0rc1/dbt/include/databricks/macros/relations/components/
--rw-r--r--   0 ben.cassell   (502) staff       (20)      131 2024-05-10 19:26:33.000000 dbt-databricks-1.8.0rc1/dbt/include/databricks/macros/relations/components/comment.sql
--rw-r--r--   0 ben.cassell   (502) staff       (20)      217 2024-05-10 19:26:33.000000 dbt-databricks-1.8.0rc1/dbt/include/databricks/macros/relations/components/partitioning.sql
--rw-r--r--   0 ben.cassell   (502) staff       (20)      670 2024-05-10 19:26:33.000000 dbt-databricks-1.8.0rc1/dbt/include/databricks/macros/relations/components/refresh_schedule.sql
--rw-r--r--   0 ben.cassell   (502) staff       (20)      310 2024-05-10 19:26:33.000000 dbt-databricks-1.8.0rc1/dbt/include/databricks/macros/relations/components/tblproperties.sql
--rw-r--r--   0 ben.cassell   (502) staff       (20)    10574 2024-05-10 19:26:33.000000 dbt-databricks-1.8.0rc1/dbt/include/databricks/macros/relations/constraints.sql
--rw-r--r--   0 ben.cassell   (502) staff       (20)      629 2024-05-10 19:26:33.000000 dbt-databricks-1.8.0rc1/dbt/include/databricks/macros/relations/create.sql
--rw-r--r--   0 ben.cassell   (502) staff       (20)      564 2024-05-10 19:26:33.000000 dbt-databricks-1.8.0rc1/dbt/include/databricks/macros/relations/drop.sql
--rw-r--r--   0 ben.cassell   (502) staff       (20)      147 2024-05-10 19:26:33.000000 dbt-databricks-1.8.0rc1/dbt/include/databricks/macros/relations/file_format.sql
--rw-r--r--   0 ben.cassell   (502) staff       (20)      615 2024-05-10 19:26:33.000000 dbt-databricks-1.8.0rc1/dbt/include/databricks/macros/relations/location.sql
-drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-05-10 20:26:57.856351 dbt-databricks-1.8.0rc1/dbt/include/databricks/macros/relations/materialized_view/
--rw-r--r--   0 ben.cassell   (502) staff       (20)     1801 2024-05-10 19:26:33.000000 dbt-databricks-1.8.0rc1/dbt/include/databricks/macros/relations/materialized_view/alter.sql
--rw-r--r--   0 ben.cassell   (502) staff       (20)      756 2024-05-10 19:26:33.000000 dbt-databricks-1.8.0rc1/dbt/include/databricks/macros/relations/materialized_view/create.sql
--rw-r--r--   0 ben.cassell   (502) staff       (20)      126 2024-05-10 19:26:33.000000 dbt-databricks-1.8.0rc1/dbt/include/databricks/macros/relations/materialized_view/drop.sql
--rw-r--r--   0 ben.cassell   (502) staff       (20)      119 2024-05-10 19:26:33.000000 dbt-databricks-1.8.0rc1/dbt/include/databricks/macros/relations/materialized_view/refresh.sql
--rw-r--r--   0 ben.cassell   (502) staff       (20)     1372 2024-05-10 19:26:33.000000 dbt-databricks-1.8.0rc1/dbt/include/databricks/macros/relations/optimize.sql
--rw-r--r--   0 ben.cassell   (502) staff       (20)     2273 2024-05-10 19:26:33.000000 dbt-databricks-1.8.0rc1/dbt/include/databricks/macros/relations/replace.sql
-drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-05-10 20:26:57.857639 dbt-databricks-1.8.0rc1/dbt/include/databricks/macros/relations/streaming_table/
--rw-r--r--   0 ben.cassell   (502) staff       (20)     3212 2024-05-10 19:26:33.000000 dbt-databricks-1.8.0rc1/dbt/include/databricks/macros/relations/streaming_table/alter.sql
--rw-r--r--   0 ben.cassell   (502) staff       (20)      904 2024-05-10 19:17:14.000000 dbt-databricks-1.8.0rc1/dbt/include/databricks/macros/relations/streaming_table/create.sql
--rw-r--r--   0 ben.cassell   (502) staff       (20)      246 2024-05-10 19:26:33.000000 dbt-databricks-1.8.0rc1/dbt/include/databricks/macros/relations/streaming_table/drop.sql
--rw-r--r--   0 ben.cassell   (502) staff       (20)      292 2024-05-10 19:17:14.000000 dbt-databricks-1.8.0rc1/dbt/include/databricks/macros/relations/streaming_table/refresh.sql
-drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-05-10 20:26:57.858296 dbt-databricks-1.8.0rc1/dbt/include/databricks/macros/relations/table/
--rw-r--r--   0 ben.cassell   (502) staff       (20)     3161 2024-05-10 19:26:33.000000 dbt-databricks-1.8.0rc1/dbt/include/databricks/macros/relations/table/create.sql
--rw-r--r--   0 ben.cassell   (502) staff       (20)      102 2024-05-10 19:26:33.000000 dbt-databricks-1.8.0rc1/dbt/include/databricks/macros/relations/table/drop.sql
--rw-r--r--   0 ben.cassell   (502) staff       (20)     1604 2024-05-10 19:26:33.000000 dbt-databricks-1.8.0rc1/dbt/include/databricks/macros/relations/tags.sql
--rw-r--r--   0 ben.cassell   (502) staff       (20)      764 2024-05-10 19:26:33.000000 dbt-databricks-1.8.0rc1/dbt/include/databricks/macros/relations/tblproperties.sql
-drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-05-10 20:26:57.858934 dbt-databricks-1.8.0rc1/dbt/include/databricks/macros/relations/view/
--rw-r--r--   0 ben.cassell   (502) staff       (20)      643 2024-05-10 19:26:33.000000 dbt-databricks-1.8.0rc1/dbt/include/databricks/macros/relations/view/create.sql
--rw-r--r--   0 ben.cassell   (502) staff       (20)      100 2024-05-10 19:26:33.000000 dbt-databricks-1.8.0rc1/dbt/include/databricks/macros/relations/view/drop.sql
-drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-05-10 20:26:57.859393 dbt-databricks-1.8.0rc1/dbt/include/databricks/macros/utils/
--rw-r--r--   0 ben.cassell   (502) staff       (20)      318 2023-05-30 21:40:46.000000 dbt-databricks-1.8.0rc1/dbt/include/databricks/macros/utils/dateadd.sql
--rw-r--r--   0 ben.cassell   (502) staff       (20)      338 2023-10-26 17:27:28.000000 dbt-databricks-1.8.0rc1/dbt/include/databricks/macros/utils/datediff.sql
--rw-r--r--   0 ben.cassell   (502) staff       (20)      535 2023-05-30 21:40:46.000000 dbt-databricks-1.8.0rc1/dbt/include/databricks/profile_template.yml
-drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-05-10 20:26:57.861662 dbt-databricks-1.8.0rc1/dbt_databricks.egg-info/
--rw-r--r--   0 ben.cassell   (502) staff       (20)     6131 2024-05-10 20:26:57.000000 dbt-databricks-1.8.0rc1/dbt_databricks.egg-info/PKG-INFO
--rw-r--r--   0 ben.cassell   (502) staff       (20)     4441 2024-05-10 20:26:57.000000 dbt-databricks-1.8.0rc1/dbt_databricks.egg-info/SOURCES.txt
--rw-r--r--   0 ben.cassell   (502) staff       (20)        1 2024-05-10 20:26:57.000000 dbt-databricks-1.8.0rc1/dbt_databricks.egg-info/dependency_links.txt
--rw-r--r--   0 ben.cassell   (502) staff       (20)        1 2024-05-08 19:39:36.000000 dbt-databricks-1.8.0rc1/dbt_databricks.egg-info/not-zip-safe
--rw-r--r--   0 ben.cassell   (502) staff       (20)      166 2024-05-10 20:26:57.000000 dbt-databricks-1.8.0rc1/dbt_databricks.egg-info/requires.txt
--rw-r--r--   0 ben.cassell   (502) staff       (20)        4 2024-05-10 20:26:57.000000 dbt-databricks-1.8.0rc1/dbt_databricks.egg-info/top_level.txt
--rw-r--r--   0 ben.cassell   (502) staff       (20)       38 2024-05-10 20:26:57.862392 dbt-databricks-1.8.0rc1/setup.cfg
--rw-r--r--   0 ben.cassell   (502) staff       (20)     2629 2024-05-10 19:26:33.000000 dbt-databricks-1.8.0rc1/setup.py
+drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-05-08 19:39:36.521535 dbt-databricks-2.0.0rc1/
+-rw-r--r--   0 ben.cassell   (502) staff       (20)       47 2024-05-08 18:44:23.000000 dbt-databricks-2.0.0rc1/MANIFEST.in
+-rw-r--r--   0 ben.cassell   (502) staff       (20)     5379 2024-05-08 19:39:36.521361 dbt-databricks-2.0.0rc1/PKG-INFO
+-rw-r--r--   0 ben.cassell   (502) staff       (20)     4624 2024-01-19 01:37:59.000000 dbt-databricks-2.0.0rc1/README.md
+drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-05-08 19:39:36.494981 dbt-databricks-2.0.0rc1/dbt/
+-rw-r--r--   0 ben.cassell   (502) staff       (20)       76 2024-01-25 18:09:59.000000 dbt-databricks-2.0.0rc1/dbt/__init__.py
+drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-05-08 19:39:36.491260 dbt-databricks-2.0.0rc1/dbt/adapters/
+drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-05-08 19:39:36.498675 dbt-databricks-2.0.0rc1/dbt/adapters/databricks/
+-rw-r--r--   0 ben.cassell   (502) staff       (20)      625 2024-05-08 18:44:23.000000 dbt-databricks-2.0.0rc1/dbt/adapters/databricks/__init__.py
+-rw-r--r--   0 ben.cassell   (502) staff       (20)       26 2024-05-08 18:44:23.000000 dbt-databricks-2.0.0rc1/dbt/adapters/databricks/__version__.py
+-rw-r--r--   0 ben.cassell   (502) staff       (20)     3513 2024-05-08 18:44:23.000000 dbt-databricks-2.0.0rc1/dbt/adapters/databricks/auth.py
+-rw-r--r--   0 ben.cassell   (502) staff       (20)      707 2024-05-08 18:44:23.000000 dbt-databricks-2.0.0rc1/dbt/adapters/databricks/column.py
+-rw-r--r--   0 ben.cassell   (502) staff       (20)    48111 2024-05-08 18:44:27.000000 dbt-databricks-2.0.0rc1/dbt/adapters/databricks/connections.py
+-rw-r--r--   0 ben.cassell   (502) staff       (20)    15743 2024-05-08 18:44:23.000000 dbt-databricks-2.0.0rc1/dbt/adapters/databricks/credentials.py
+drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-05-08 19:39:36.500789 dbt-databricks-2.0.0rc1/dbt/adapters/databricks/events/
+-rw-r--r--   0 ben.cassell   (502) staff       (20)      796 2024-05-02 16:13:11.000000 dbt-databricks-2.0.0rc1/dbt/adapters/databricks/events/base.py
+-rw-r--r--   0 ben.cassell   (502) staff       (20)     3996 2024-05-08 18:44:27.000000 dbt-databricks-2.0.0rc1/dbt/adapters/databricks/events/connection_events.py
+-rw-r--r--   0 ben.cassell   (502) staff       (20)      616 2024-05-02 16:13:11.000000 dbt-databricks-2.0.0rc1/dbt/adapters/databricks/events/credential_events.py
+-rw-r--r--   0 ben.cassell   (502) staff       (20)     1826 2024-05-02 16:13:11.000000 dbt-databricks-2.0.0rc1/dbt/adapters/databricks/events/cursor_events.py
+-rw-r--r--   0 ben.cassell   (502) staff       (20)      250 2024-05-02 16:13:11.000000 dbt-databricks-2.0.0rc1/dbt/adapters/databricks/events/other_events.py
+-rw-r--r--   0 ben.cassell   (502) staff       (20)      842 2024-05-02 16:13:11.000000 dbt-databricks-2.0.0rc1/dbt/adapters/databricks/events/pipeline_events.py
+-rw-r--r--   0 ben.cassell   (502) staff       (20)    33226 2024-05-08 18:44:23.000000 dbt-databricks-2.0.0rc1/dbt/adapters/databricks/impl.py
+-rw-r--r--   0 ben.cassell   (502) staff       (20)      995 2024-05-08 18:44:23.000000 dbt-databricks-2.0.0rc1/dbt/adapters/databricks/logging.py
+-rw-r--r--   0 ben.cassell   (502) staff       (20)    19165 2024-05-08 18:44:23.000000 dbt-databricks-2.0.0rc1/dbt/adapters/databricks/python_submissions.py
+-rw-r--r--   0 ben.cassell   (502) staff       (20)     5313 2024-05-08 18:44:23.000000 dbt-databricks-2.0.0rc1/dbt/adapters/databricks/relation.py
+drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-05-08 19:39:36.503801 dbt-databricks-2.0.0rc1/dbt/adapters/databricks/relation_configs/
+-rw-r--r--   0 ben.cassell   (502) staff       (20)     6157 2024-05-08 18:44:23.000000 dbt-databricks-2.0.0rc1/dbt/adapters/databricks/relation_configs/base.py
+-rw-r--r--   0 ben.cassell   (502) staff       (20)     1085 2024-05-08 18:44:23.000000 dbt-databricks-2.0.0rc1/dbt/adapters/databricks/relation_configs/comment.py
+-rw-r--r--   0 ben.cassell   (502) staff       (20)     1040 2024-05-08 18:44:23.000000 dbt-databricks-2.0.0rc1/dbt/adapters/databricks/relation_configs/incremental.py
+-rw-r--r--   0 ben.cassell   (502) staff       (20)     1700 2024-05-08 18:44:23.000000 dbt-databricks-2.0.0rc1/dbt/adapters/databricks/relation_configs/materialized_view.py
+-rw-r--r--   0 ben.cassell   (502) staff       (20)     1699 2024-05-08 18:44:23.000000 dbt-databricks-2.0.0rc1/dbt/adapters/databricks/relation_configs/partitioning.py
+-rw-r--r--   0 ben.cassell   (502) staff       (20)     1182 2024-05-08 18:44:23.000000 dbt-databricks-2.0.0rc1/dbt/adapters/databricks/relation_configs/query.py
+-rw-r--r--   0 ben.cassell   (502) staff       (20)     2955 2024-05-08 18:44:23.000000 dbt-databricks-2.0.0rc1/dbt/adapters/databricks/relation_configs/refresh.py
+-rw-r--r--   0 ben.cassell   (502) staff       (20)     1802 2024-05-08 18:44:23.000000 dbt-databricks-2.0.0rc1/dbt/adapters/databricks/relation_configs/streaming_table.py
+-rw-r--r--   0 ben.cassell   (502) staff       (20)     1850 2024-05-08 18:44:23.000000 dbt-databricks-2.0.0rc1/dbt/adapters/databricks/relation_configs/tags.py
+-rw-r--r--   0 ben.cassell   (502) staff       (20)     2631 2024-05-08 18:44:23.000000 dbt-databricks-2.0.0rc1/dbt/adapters/databricks/relation_configs/tblproperties.py
+-rw-r--r--   0 ben.cassell   (502) staff       (20)     2503 2024-05-08 18:44:23.000000 dbt-databricks-2.0.0rc1/dbt/adapters/databricks/utils.py
+drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-05-08 19:39:36.491927 dbt-databricks-2.0.0rc1/dbt/include/
+drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-05-08 19:39:36.504794 dbt-databricks-2.0.0rc1/dbt/include/databricks/
+-rw-r--r--   0 ben.cassell   (502) staff       (20)       52 2023-05-30 21:40:46.000000 dbt-databricks-2.0.0rc1/dbt/include/databricks/__init__.py
+-rw-r--r--   0 ben.cassell   (502) staff       (20)       77 2023-05-30 21:40:46.000000 dbt-databricks-2.0.0rc1/dbt/include/databricks/dbt_project.yml
+drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-05-08 19:39:36.493824 dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/
+drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-05-08 19:39:36.506895 dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/adapters/
+-rw-r--r--   0 ben.cassell   (502) staff       (20)     3445 2024-05-08 18:44:23.000000 dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/adapters/catalog.sql
+-rw-r--r--   0 ben.cassell   (502) staff       (20)     2409 2024-03-26 16:27:09.000000 dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/adapters/copy_into.sql
+-rw-r--r--   0 ben.cassell   (502) staff       (20)      592 2024-05-08 18:44:23.000000 dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/adapters/databricks_catalog.sql
+-rw-r--r--   0 ben.cassell   (502) staff       (20)     5153 2024-05-08 18:44:23.000000 dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/adapters/metadata.sql
+-rw-r--r--   0 ben.cassell   (502) staff       (20)     1984 2024-05-08 18:44:23.000000 dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/adapters/persist_docs.sql
+-rw-r--r--   0 ben.cassell   (502) staff       (20)     3540 2024-05-08 18:44:23.000000 dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/adapters/python.sql
+-rw-r--r--   0 ben.cassell   (502) staff       (20)     1158 2024-05-08 18:44:23.000000 dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/adapters/relation.sql
+drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-05-08 19:39:36.507117 dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/etc/
+-rw-r--r--   0 ben.cassell   (502) staff       (20)      648 2024-03-26 16:27:09.000000 dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/etc/statement.sql
+drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-05-08 19:39:36.507337 dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/get_custom_name/
+-rw-r--r--   0 ben.cassell   (502) staff       (20)      458 2024-05-08 18:44:23.000000 dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/get_custom_name/get_custom_database.sql
+drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-05-08 19:39:36.509359 dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/materializations/
+-rw-r--r--   0 ben.cassell   (502) staff       (20)     2803 2024-05-08 18:44:23.000000 dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/materializations/clone.sql
+drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-05-08 19:39:36.510259 dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/materializations/incremental/
+-rw-r--r--   0 ben.cassell   (502) staff       (20)     4875 2024-05-08 18:44:23.000000 dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/materializations/incremental/incremental.sql
+-rw-r--r--   0 ben.cassell   (502) staff       (20)     5522 2024-05-08 18:44:23.000000 dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/materializations/incremental/strategies.sql
+-rw-r--r--   0 ben.cassell   (502) staff       (20)     1896 2024-05-08 18:44:23.000000 dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/materializations/incremental/validate.sql
+-rw-r--r--   0 ben.cassell   (502) staff       (20)     3657 2024-05-08 18:44:23.000000 dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/materializations/materialized_view.sql
+drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-05-08 19:39:36.510888 dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/materializations/seeds/
+-rw-r--r--   0 ben.cassell   (502) staff       (20)     2849 2024-05-08 18:44:23.000000 dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/materializations/seeds/helpers.sql
+-rw-r--r--   0 ben.cassell   (502) staff       (20)     2477 2024-05-08 18:44:23.000000 dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/materializations/seeds/seeds.sql
+-rw-r--r--   0 ben.cassell   (502) staff       (20)     5397 2024-03-29 15:20:41.000000 dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/materializations/snapshot.sql
+-rw-r--r--   0 ben.cassell   (502) staff       (20)     3623 2024-05-08 18:44:23.000000 dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/materializations/streaming_table.sql
+-rw-r--r--   0 ben.cassell   (502) staff       (20)     1966 2024-05-08 18:44:23.000000 dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/materializations/table.sql
+-rw-r--r--   0 ben.cassell   (502) staff       (20)     1364 2024-05-08 18:44:23.000000 dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/materializations/view.sql
+drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-05-08 19:39:36.513975 dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/relations/
+drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-05-08 19:39:36.515305 dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/relations/components/
+-rw-r--r--   0 ben.cassell   (502) staff       (20)      131 2024-05-08 18:44:23.000000 dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/relations/components/comment.sql
+-rw-r--r--   0 ben.cassell   (502) staff       (20)      217 2024-05-08 18:44:23.000000 dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/relations/components/partitioning.sql
+-rw-r--r--   0 ben.cassell   (502) staff       (20)      670 2024-05-08 18:44:23.000000 dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/relations/components/refresh_schedule.sql
+-rw-r--r--   0 ben.cassell   (502) staff       (20)      310 2024-05-08 18:44:23.000000 dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/relations/components/tblproperties.sql
+-rw-r--r--   0 ben.cassell   (502) staff       (20)    10574 2024-05-08 18:44:23.000000 dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/relations/constraints.sql
+-rw-r--r--   0 ben.cassell   (502) staff       (20)      629 2024-05-08 18:44:23.000000 dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/relations/create.sql
+-rw-r--r--   0 ben.cassell   (502) staff       (20)      564 2024-05-08 18:44:23.000000 dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/relations/drop.sql
+-rw-r--r--   0 ben.cassell   (502) staff       (20)      147 2024-05-08 18:44:23.000000 dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/relations/file_format.sql
+-rw-r--r--   0 ben.cassell   (502) staff       (20)      615 2024-05-08 18:44:23.000000 dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/relations/location.sql
+drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-05-08 19:39:36.516644 dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/relations/materialized_view/
+-rw-r--r--   0 ben.cassell   (502) staff       (20)     1801 2024-05-08 18:44:23.000000 dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/relations/materialized_view/alter.sql
+-rw-r--r--   0 ben.cassell   (502) staff       (20)      756 2024-05-08 18:44:23.000000 dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/relations/materialized_view/create.sql
+-rw-r--r--   0 ben.cassell   (502) staff       (20)      126 2024-05-08 18:44:23.000000 dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/relations/materialized_view/drop.sql
+-rw-r--r--   0 ben.cassell   (502) staff       (20)      119 2024-05-08 18:44:23.000000 dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/relations/materialized_view/refresh.sql
+-rw-r--r--   0 ben.cassell   (502) staff       (20)     1372 2024-05-08 18:44:23.000000 dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/relations/optimize.sql
+-rw-r--r--   0 ben.cassell   (502) staff       (20)     2273 2024-05-08 18:44:23.000000 dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/relations/replace.sql
+drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-05-08 19:39:36.517490 dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/relations/streaming_table/
+-rw-r--r--   0 ben.cassell   (502) staff       (20)     3212 2024-05-08 18:44:23.000000 dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/relations/streaming_table/alter.sql
+-rw-r--r--   0 ben.cassell   (502) staff       (20)      904 2024-05-08 18:44:23.000000 dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/relations/streaming_table/create.sql
+-rw-r--r--   0 ben.cassell   (502) staff       (20)      246 2024-05-08 18:44:23.000000 dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/relations/streaming_table/drop.sql
+-rw-r--r--   0 ben.cassell   (502) staff       (20)      292 2024-05-08 18:44:23.000000 dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/relations/streaming_table/refresh.sql
+drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-05-08 19:39:36.518192 dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/relations/table/
+-rw-r--r--   0 ben.cassell   (502) staff       (20)     3161 2024-05-08 18:44:23.000000 dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/relations/table/create.sql
+-rw-r--r--   0 ben.cassell   (502) staff       (20)      102 2024-05-08 18:44:23.000000 dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/relations/table/drop.sql
+-rw-r--r--   0 ben.cassell   (502) staff       (20)     1604 2024-05-08 18:44:23.000000 dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/relations/tags.sql
+-rw-r--r--   0 ben.cassell   (502) staff       (20)      764 2024-05-01 20:15:21.000000 dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/relations/tblproperties.sql
+drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-05-08 19:39:36.518815 dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/relations/view/
+-rw-r--r--   0 ben.cassell   (502) staff       (20)      643 2024-05-08 18:44:23.000000 dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/relations/view/create.sql
+-rw-r--r--   0 ben.cassell   (502) staff       (20)      100 2024-05-08 18:44:23.000000 dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/relations/view/drop.sql
+drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-05-08 19:39:36.519299 dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/utils/
+-rw-r--r--   0 ben.cassell   (502) staff       (20)      318 2023-05-30 21:40:46.000000 dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/utils/dateadd.sql
+-rw-r--r--   0 ben.cassell   (502) staff       (20)      338 2023-10-26 17:27:28.000000 dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/utils/datediff.sql
+-rw-r--r--   0 ben.cassell   (502) staff       (20)      535 2023-05-30 21:40:46.000000 dbt-databricks-2.0.0rc1/dbt/include/databricks/profile_template.yml
+drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-05-08 19:39:36.520890 dbt-databricks-2.0.0rc1/dbt_databricks.egg-info/
+-rw-r--r--   0 ben.cassell   (502) staff       (20)     5379 2024-05-08 19:39:36.000000 dbt-databricks-2.0.0rc1/dbt_databricks.egg-info/PKG-INFO
+-rw-r--r--   0 ben.cassell   (502) staff       (20)     4441 2024-05-08 19:39:36.000000 dbt-databricks-2.0.0rc1/dbt_databricks.egg-info/SOURCES.txt
+-rw-r--r--   0 ben.cassell   (502) staff       (20)        1 2024-05-08 19:39:36.000000 dbt-databricks-2.0.0rc1/dbt_databricks.egg-info/dependency_links.txt
+-rw-r--r--   0 ben.cassell   (502) staff       (20)        1 2024-05-08 19:39:36.000000 dbt-databricks-2.0.0rc1/dbt_databricks.egg-info/not-zip-safe
+-rw-r--r--   0 ben.cassell   (502) staff       (20)      166 2024-05-08 19:39:36.000000 dbt-databricks-2.0.0rc1/dbt_databricks.egg-info/requires.txt
+-rw-r--r--   0 ben.cassell   (502) staff       (20)        4 2024-05-08 19:39:36.000000 dbt-databricks-2.0.0rc1/dbt_databricks.egg-info/top_level.txt
+-rw-r--r--   0 ben.cassell   (502) staff       (20)       38 2024-05-08 19:39:36.521583 dbt-databricks-2.0.0rc1/setup.cfg
+-rw-r--r--   0 ben.cassell   (502) staff       (20)     2629 2024-05-08 18:44:27.000000 dbt-databricks-2.0.0rc1/setup.py
```

### Comparing `dbt-databricks-1.8.0rc1/PKG-INFO` & `dbt-databricks-2.0.0rc1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,109 +1,107 @@
 Metadata-Version: 2.1
 Name: dbt-databricks
-Version: 1.8.0rc1
+Version: 2.0.0rc1
 Summary: The Databricks adapter plugin for dbt
 Home-page: https://github.com/databricks/dbt-databricks
 Author: Databricks
 Author-email: feedback@databricks.com
-License: UNKNOWN
-Description: <p align="center">
-          <img src="https://bynder-public-us-west-2.s3.amazonaws.com/styleguide/ABB317701CA31CB7F29268E32B303CAE-pdf-column-1.png" alt="databricks logo" width="50%" />
-          <img src="https://raw.githubusercontent.com/dbt-labs/dbt/ec7dee39f793aa4f7dd3dae37282cc87664813e4/etc/dbt-logo-full.svg" alt="dbt logo" width="250"/>
-        </p>
-        <p align="center">
-          <a href="https://github.com/databricks/dbt-databricks/actions/workflows/main.yml">
-            <img src="https://github.com/databricks/dbt-databricks/actions/workflows/main.yml/badge.svg?event=push" alt="Unit Tests Badge"/>
-          </a>
-          <a href="https://github.com/databricks/dbt-databricks/actions/workflows/integration.yml">
-            <img src="https://github.com/databricks/dbt-databricks/actions/workflows/integration.yml/badge.svg?event=push" alt="Integration Tests Badge"/>
-          </a>
-        </p>
-        
-        **[dbt](https://www.getdbt.com/)** enables data analysts and engineers to transform their data using the same practices that software engineers use to build applications.
-        
-        The **[Databricks Lakehouse](https://www.databricks.com/)** provides one simple platform to unify all your data, analytics and AI workloads.
-        
-        # dbt-databricks
-        
-        The `dbt-databricks` adapter contains all of the code enabling dbt to work with Databricks. This adapter is based off the amazing work done in [dbt-spark](https://github.com/dbt-labs/dbt-spark). Some key features include:
-        
-        - **Easy setup**. No need to install an ODBC driver as the adapter uses pure Python APIs.
-        - **Open by default**. For example, it uses the the open and performant [Delta](https://delta.io/) table format by default. This has many benefits, including letting you use `MERGE` as the the default incremental materialization strategy.
-        - **Support for Unity Catalog**. dbt-databricks>=1.1.1 supports the 3-level namespace of Unity Catalog (catalog / schema / relations) so you can organize and secure your data the way you like.
-        - **Performance**. The adapter generates SQL expressions that are automatically accelerated by the native, vectorized [Photon](https://databricks.com/product/photon) execution engine.
-        
-        ## Choosing between dbt-databricks and dbt-spark
-        If you are developing a dbt project on Databricks, we recommend using `dbt-databricks` for the reasons noted above.
-        
-        `dbt-spark` is an actively developed adapter which works with Databricks as well as Apache Spark anywhere it is hosted e.g. on AWS EMR.
-        
-        ## Getting started
-        
-        ### Installation
-        
-        Install using pip:
-        ```nofmt
-        pip install dbt-databricks
-        ```
-        
-        Upgrade to the latest version
-        ```nofmt
-        pip install --upgrade dbt-databricks
-        ```
-        
-        ### Profile Setup
-        
-        ```nofmt
-        your_profile_name:
-          target: dev
-          outputs:
-            dev:
-              type: databricks
-              catalog: [optional catalog name, if you are using Unity Catalog, only available in dbt-databricks>=1.1.1]
-              schema: [database/schema name]
-              host: [your.databrickshost.com]
-              http_path: [/sql/your/http/path]
-              token: [dapiXXXXXXXXXXXXXXXXXXXXXXX]
-        ```
-        
-        ### Quick Starts
-        
-        These following quick starts will get you up and running with the `dbt-databricks` adapter:
-        - [Developing your first dbt project](https://github.com/databricks/dbt-databricks/blob/main/docs/local-dev.md)
-        - Using dbt Cloud with Databricks ([Azure](https://docs.microsoft.com/en-us/azure/databricks/integrations/prep/dbt-cloud) | [AWS](https://docs.databricks.com/integrations/prep/dbt-cloud.html))
-        - [Running dbt production jobs on Databricks Workflows](https://github.com/databricks/dbt-databricks/blob/main/docs/databricks-workflows.md)
-        - [Using Unity Catalog with dbt-databricks](https://github.com/databricks/dbt-databricks/blob/main/docs/uc.md)
-        - [Using GitHub Actions for dbt CI/CD on Databricks](https://github.com/databricks/dbt-databricks/blob/main/docs/github-actions.md)
-        - [Loading data from S3 into Delta using the databricks_copy_into macro](https://github.com/databricks/dbt-databricks/blob/main/docs/databricks-copy-into-macro-aws.md)
-        - [Contribute to this repository](CONTRIBUTING.MD)
-        
-        ### Compatibility
-        
-        The `dbt-databricks` adapter has been tested:
-        
-        - with Python 3.7 or above.
-        - against `Databricks SQL` and `Databricks runtime releases 9.1 LTS` and later.
-        
-        ### Tips and Tricks
-        ## Choosing compute for a Python model
-        You can override the compute used for a specific Python model by setting the `http_path` property in model configuration. This can be useful if, for example, you want to run a Python model on an All Purpose cluster, while running SQL models on a SQL Warehouse. Note that this capability is only available for Python models.
-        
-        ```
-        def model(dbt, session):
-            dbt.config(
-              http_path="sql/protocolv1/..."
-            )
-        ```
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+
+<p align="center">
+  <img src="https://bynder-public-us-west-2.s3.amazonaws.com/styleguide/ABB317701CA31CB7F29268E32B303CAE-pdf-column-1.png" alt="databricks logo" width="50%" />
+  <img src="https://raw.githubusercontent.com/dbt-labs/dbt/ec7dee39f793aa4f7dd3dae37282cc87664813e4/etc/dbt-logo-full.svg" alt="dbt logo" width="250"/>
+</p>
+<p align="center">
+  <a href="https://github.com/databricks/dbt-databricks/actions/workflows/main.yml">
+    <img src="https://github.com/databricks/dbt-databricks/actions/workflows/main.yml/badge.svg?event=push" alt="Unit Tests Badge"/>
+  </a>
+  <a href="https://github.com/databricks/dbt-databricks/actions/workflows/integration.yml">
+    <img src="https://github.com/databricks/dbt-databricks/actions/workflows/integration.yml/badge.svg?event=push" alt="Integration Tests Badge"/>
+  </a>
+</p>
+
+**[dbt](https://www.getdbt.com/)** enables data analysts and engineers to transform their data using the same practices that software engineers use to build applications.
+
+The **[Databricks Lakehouse](https://www.databricks.com/)** provides one simple platform to unify all your data, analytics and AI workloads.
+
+# dbt-databricks
+
+The `dbt-databricks` adapter contains all of the code enabling dbt to work with Databricks. This adapter is based off the amazing work done in [dbt-spark](https://github.com/dbt-labs/dbt-spark). Some key features include:
+
+- **Easy setup**. No need to install an ODBC driver as the adapter uses pure Python APIs.
+- **Open by default**. For example, it uses the the open and performant [Delta](https://delta.io/) table format by default. This has many benefits, including letting you use `MERGE` as the the default incremental materialization strategy.
+- **Support for Unity Catalog**. dbt-databricks>=1.1.1 supports the 3-level namespace of Unity Catalog (catalog / schema / relations) so you can organize and secure your data the way you like.
+- **Performance**. The adapter generates SQL expressions that are automatically accelerated by the native, vectorized [Photon](https://databricks.com/product/photon) execution engine.
+
+## Choosing between dbt-databricks and dbt-spark
+If you are developing a dbt project on Databricks, we recommend using `dbt-databricks` for the reasons noted above.
+
+`dbt-spark` is an actively developed adapter which works with Databricks as well as Apache Spark anywhere it is hosted e.g. on AWS EMR.
+
+## Getting started
+
+### Installation
+
+Install using pip:
+```nofmt
+pip install dbt-databricks
+```
+
+Upgrade to the latest version
+```nofmt
+pip install --upgrade dbt-databricks
+```
+
+### Profile Setup
+
+```nofmt
+your_profile_name:
+  target: dev
+  outputs:
+    dev:
+      type: databricks
+      catalog: [optional catalog name, if you are using Unity Catalog, only available in dbt-databricks>=1.1.1]
+      schema: [database/schema name]
+      host: [your.databrickshost.com]
+      http_path: [/sql/your/http/path]
+      token: [dapiXXXXXXXXXXXXXXXXXXXXXXX]
+```
+
+### Quick Starts
+
+These following quick starts will get you up and running with the `dbt-databricks` adapter:
+- [Developing your first dbt project](https://github.com/databricks/dbt-databricks/blob/main/docs/local-dev.md)
+- Using dbt Cloud with Databricks ([Azure](https://docs.microsoft.com/en-us/azure/databricks/integrations/prep/dbt-cloud) | [AWS](https://docs.databricks.com/integrations/prep/dbt-cloud.html))
+- [Running dbt production jobs on Databricks Workflows](https://github.com/databricks/dbt-databricks/blob/main/docs/databricks-workflows.md)
+- [Using Unity Catalog with dbt-databricks](https://github.com/databricks/dbt-databricks/blob/main/docs/uc.md)
+- [Using GitHub Actions for dbt CI/CD on Databricks](https://github.com/databricks/dbt-databricks/blob/main/docs/github-actions.md)
+- [Loading data from S3 into Delta using the databricks_copy_into macro](https://github.com/databricks/dbt-databricks/blob/main/docs/databricks-copy-into-macro-aws.md)
+- [Contribute to this repository](CONTRIBUTING.MD)
+
+### Compatibility
+
+The `dbt-databricks` adapter has been tested:
+
+- with Python 3.7 or above.
+- against `Databricks SQL` and `Databricks runtime releases 9.1 LTS` and later.
+
+### Tips and Tricks
+## Choosing compute for a Python model
+You can override the compute used for a specific Python model by setting the `http_path` property in model configuration. This can be useful if, for example, you want to run a Python model on an All Purpose cluster, while running SQL models on a SQL Warehouse. Note that this capability is only available for Python models.
+
+```
+def model(dbt, session):
+    dbt.config(
+      http_path="sql/protocolv1/..."
+    )
+```
```

### Comparing `dbt-databricks-1.8.0rc1/README.md` & `dbt-databricks-2.0.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.0rc1/dbt/adapters/databricks/__init__.py` & `dbt-databricks-2.0.0rc1/dbt/adapters/databricks/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.0rc1/dbt/adapters/databricks/auth.py` & `dbt-databricks-2.0.0rc1/dbt/adapters/databricks/auth.py`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.0rc1/dbt/adapters/databricks/column.py` & `dbt-databricks-2.0.0rc1/dbt/adapters/databricks/column.py`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.0rc1/dbt/adapters/databricks/connections.py` & `dbt-databricks-2.0.0rc1/dbt/adapters/databricks/connections.py`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.0rc1/dbt/adapters/databricks/credentials.py` & `dbt-databricks-2.0.0rc1/dbt/adapters/databricks/credentials.py`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.0rc1/dbt/adapters/databricks/events/base.py` & `dbt-databricks-2.0.0rc1/dbt/adapters/databricks/events/base.py`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.0rc1/dbt/adapters/databricks/events/connection_events.py` & `dbt-databricks-2.0.0rc1/dbt/adapters/databricks/events/connection_events.py`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.0rc1/dbt/adapters/databricks/events/credential_events.py` & `dbt-databricks-2.0.0rc1/dbt/adapters/databricks/events/credential_events.py`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.0rc1/dbt/adapters/databricks/events/cursor_events.py` & `dbt-databricks-2.0.0rc1/dbt/adapters/databricks/events/cursor_events.py`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.0rc1/dbt/adapters/databricks/events/pipeline_events.py` & `dbt-databricks-2.0.0rc1/dbt/adapters/databricks/events/pipeline_events.py`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.0rc1/dbt/adapters/databricks/impl.py` & `dbt-databricks-2.0.0rc1/dbt/adapters/databricks/impl.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,57 +3,59 @@
 from abc import ABC
 from abc import abstractmethod
 from collections import defaultdict
 from concurrent.futures import Future
 from contextlib import contextmanager
 from dataclasses import dataclass
 from typing import Any
-from typing import Callable
 from typing import ClassVar
 from typing import Dict
 from typing import FrozenSet
 from typing import Generic
 from typing import Iterable
 from typing import Iterator
 from typing import List
 from typing import Optional
 from typing import Set
 from typing import Tuple
 from typing import Type
-from typing import TypeVar
 from typing import Union
 
 from agate import Row
 from agate import Table
 from agate import Text
 from dbt.adapters.base import AdapterConfig
 from dbt.adapters.base import PythonJobHelper
 from dbt.adapters.base.impl import catch_as_completed
 from dbt.adapters.base.meta import available
 from dbt.adapters.base.relation import BaseRelation
+from dbt.adapters.base.relation import InformationSchema
 from dbt.adapters.capability import Capability
 from dbt.adapters.capability import CapabilityDict
 from dbt.adapters.capability import CapabilitySupport
 from dbt.adapters.capability import Support
 from dbt.adapters.contracts.connection import AdapterResponse
 from dbt.adapters.contracts.connection import Connection
 from dbt.adapters.contracts.relation import RelationConfig
 from dbt.adapters.contracts.relation import RelationType
 from dbt.adapters.databricks.column import DatabricksColumn
 from dbt.adapters.databricks.connections import DatabricksConnectionManager
 from dbt.adapters.databricks.connections import ExtendedSessionConnectionManager
 from dbt.adapters.databricks.connections import USE_LONG_SESSIONS
+from dbt.adapters.databricks.logging import logger
 from dbt.adapters.databricks.python_submissions import (
     DbtDatabricksAllPurposeClusterPythonJobHelper,
 )
 from dbt.adapters.databricks.python_submissions import (
     DbtDatabricksJobClusterPythonJobHelper,
 )
 from dbt.adapters.databricks.relation import DatabricksRelation
 from dbt.adapters.databricks.relation import DatabricksRelationType
+from dbt.adapters.databricks.relation import extract_identifiers
+from dbt.adapters.databricks.relation import is_hive_metastore
 from dbt.adapters.databricks.relation_configs.base import DatabricksRelationConfig
 from dbt.adapters.databricks.relation_configs.base import DatabricksRelationConfigBase
 from dbt.adapters.databricks.relation_configs.incremental import IncrementalTableConfig
 from dbt.adapters.databricks.relation_configs.materialized_view import (
     MaterializedViewConfig,
 )
 from dbt.adapters.databricks.relation_configs.streaming_table import (
@@ -69,15 +71,14 @@
 from dbt.adapters.spark.impl import KEY_TABLE_STATISTICS
 from dbt.adapters.spark.impl import LIST_SCHEMAS_MACRO_NAME
 from dbt.adapters.spark.impl import SparkAdapter
 from dbt.adapters.spark.impl import TABLE_OR_VIEW_NOT_FOUND_MESSAGES
 from dbt_common.clients.agate_helper import DEFAULT_TYPE_TESTER
 from dbt_common.exceptions import DbtRuntimeError
 from dbt_common.utils import executor
-from dbt_common.utils.dict import AttrDict
 
 CURRENT_CATALOG_MACRO_NAME = "current_catalog"
 USE_CATALOG_MACRO_NAME = "use_catalog"
 GET_CATALOG_MACRO_NAME = "get_catalog"
 SHOW_TABLE_EXTENDED_MACRO_NAME = "show_table_extended"
 SHOW_TABLES_MACRO_NAME = "show_tables"
 SHOW_VIEWS_MACRO_NAME = "show_views"
@@ -98,29 +99,15 @@
     tblproperties: Optional[Dict[str, str]] = None
     zorder: Optional[Union[List[str], str]] = None
 
 
 def check_not_found_error(errmsg: str) -> bool:
     new_error = "[SCHEMA_NOT_FOUND]" in errmsg
     old_error = re.match(r".*(Database).*(not found).*", errmsg, re.DOTALL)
-    found_msgs = (msg in errmsg for msg in TABLE_OR_VIEW_NOT_FOUND_MESSAGES)
-    return new_error or old_error is not None or any(found_msgs)
-
-
-T = TypeVar("T")
-
-
-def handle_missing_objects(exec: Callable[[], T], default: T) -> T:
-    try:
-        return exec()
-    except DbtRuntimeError as e:
-        errmsg = getattr(e, "msg", "")
-        if check_not_found_error(errmsg):
-            return default
-        raise e
+    return new_error or old_error is not None
 
 
 def get_identifier_list_string(table_names: Set[str]) -> str:
     """Returns `"|".join(table_names)` by default.
 
     Returns `"*"` if `DBT_DESCRIBE_TABLE_2048_CHAR_BYPASS` == `"true"`
     and the joined string exceeds 2048 characters
@@ -150,15 +137,15 @@
     connections: DatabricksConnectionManager
 
     AdapterSpecificConfigs = DatabricksConfig
 
     _capabilities = CapabilityDict(
         {
             Capability.TableLastModifiedMetadata: CapabilitySupport(support=Support.Full),
-            Capability.SchemaMetadataByRelations: CapabilitySupport(support=Support.Full),
+            Capability.SchemaMetadataByRelations: CapabilitySupport(support=Support.NotImplemented),
         }
     )
 
     # override/overload
     def acquire_connection(
         self, name: Optional[str] = None, query_header_context: Any = None
     ) -> Connection:
@@ -221,45 +208,91 @@
         finally:
             if staging_table is not None:
                 self.drop_relation(staging_table)
 
     def list_relations_without_caching(  # type: ignore[override]
         self, schema_relation: DatabricksRelation
     ) -> List[DatabricksRelation]:
-        results = handle_missing_objects(
-            lambda: self.get_relations_without_caching(schema_relation),
-            Table([], ["name", "kind", "file_format", "owner"]),
-        )
+        try:
+            results = self.get_relations_without_caching(schema_relation)
+        except DbtRuntimeError as e:
+            errmsg = getattr(e, "msg", "")
+            if check_not_found_error(errmsg):
+                return []
+            else:
+                description = "Error while retrieving information about"
+                logger.debug(f"{description} {schema_relation}: {e.msg}")
+                raise e
 
         return [
             self.Relation.create(
                 database=schema_relation.database,
                 schema=schema_relation.schema,
                 identifier=name,
                 type=self.Relation.get_relation_type(kind),
+                comment=comment if comment != "" else None,
                 file_format=file_format,
                 owner=owner,
             )
-            for name, kind, file_format, owner in results.select(
-                ["name", "kind", "file_format", "owner"]
+            for name, comment, kind, file_format, owner in results.select(
+                ["name", "comment", "kind", "file_format", "owner"]
             )
         ]
 
+    def _list_relations_with_information(
+        self, schema_relation: DatabricksRelation
+    ) -> List[Tuple[DatabricksRelation, str]]:
+        results: List[Row]
+        kwargs = {"schema_relation": schema_relation}
+        try:
+            # The catalog for `show table extended` needs to match the current catalog.
+            with self._catalog(schema_relation.database):
+                results = list(self.execute_macro(SHOW_TABLE_EXTENDED_MACRO_NAME, kwargs=kwargs))
+        except DbtRuntimeError as e:
+            errmsg = getattr(e, "msg", "")
+            if check_not_found_error(errmsg):
+                results = []
+            else:
+                description = "Error while retrieving information about"
+                logger.debug(f"{description} {schema_relation.without_identifier()}: {e.msg}")
+                raise e
+
+        relations: List[Tuple[DatabricksRelation, str]] = []
+        for row in results:
+            if len(row) != 4:
+                raise DbtRuntimeError(
+                    f'Invalid value from "show table extended ...", '
+                    f"got {len(row)} values, expected 4"
+                )
+            _schema, name, _, information = row
+            rel_type = RelationType.View if "Type: VIEW" in information else RelationType.Table
+            relation = self.Relation.create(
+                database=schema_relation.database,
+                # Use `_schema` retrieved from the cluster to avoid mismatched case
+                # between the profile and the cluster.
+                schema=_schema,
+                identifier=name,
+                type=rel_type,
+            )
+            relations.append((relation, information))
+
+        return relations
+
     def get_relations_without_caching(self, relation: DatabricksRelation) -> Table:
         if relation.is_hive_metastore():
             return self._get_hive_relations(relation)
         return self._get_uc_relations(relation)
 
     def _get_uc_relations(self, relation: DatabricksRelation) -> Table:
         kwargs = {"relation": relation}
         tables = self.execute_macro("get_uc_tables", kwargs=kwargs)
         return Table(
             tables,
-            column_names=["name", "kind", "file_format", "owner"],
-            column_types=[Text(), Text(), Text(), Text()],
+            column_names=["name", "comment", "kind", "file_format", "owner"],
+            column_types=[Text(), Text(), Text(), Text(), Text()],
         )
 
     def _get_hive_relations(self, relation: DatabricksRelation) -> Table:
         kwargs = {"relation": relation}
 
         new_rows: List[Tuple[str, Optional[str]]]
         if all([relation.database, relation.schema]):
@@ -286,17 +319,17 @@
                 view_names = set(views.columns["viewName"].values())  # type: ignore[attr-defined]
                 new_rows = [
                     (row[0], str(RelationType.View if row[0] in view_names else RelationType.Table))
                     for row in new_rows
                 ]
 
         return Table(
-            [(row[0], row[1], None, None) for row in new_rows],
-            column_names=["name", "kind", "file_format", "owner"],
-            column_types=[Text(), Text(), Text(), Text()],
+            [(row[0], None, row[1], None, None) for row in new_rows],
+            column_names=["name", "comment", "kind", "file_format", "owner"],
+            column_types=[Text(), Text(), Text(), Text(), Text()],
         )
 
     def get_relation(
         self,
         database: Optional[str],
         schema: str,
         identifier: str,
@@ -316,14 +349,15 @@
         self, relation: DatabricksRelation, raw_rows: List[Row]
     ) -> Tuple[Dict[str, Any], List[DatabricksColumn]]:
         # Convert the Row to a dict
         dict_rows = [dict(zip(row._keys, row._values)) for row in raw_rows]
         # Find the separator between the rows and the metadata provided
         # by the DESCRIBE TABLE EXTENDED statement
         pos = self.find_table_information_separator(dict_rows)
+
         # Remove rows that start with a hash, they are comments
         rows = [row for row in raw_rows[0:pos] if not row["col_name"].startswith("#")]
         metadata = {col["col_name"]: col["data_type"] for col in raw_rows[pos + 1 :]}
 
         raw_table_stats = metadata.get(KEY_TABLE_STATISTICS)
         table_stats = DatabricksColumn.convert_table_stats(raw_table_stats)
         return metadata, [
@@ -342,48 +376,60 @@
             )
             for idx, column in enumerate(rows)
         ]
 
     def get_columns_in_relation(  # type: ignore[override]
         self, relation: DatabricksRelation
     ) -> List[DatabricksColumn]:
-        rows = list(
-            handle_missing_objects(
-                lambda: self.execute_macro(
-                    GET_COLUMNS_COMMENTS_MACRO_NAME, kwargs={"relation": relation}
-                ),
-                AttrDict(),
+        try:
+            rows: List[Row] = list(
+                self.execute_macro(GET_COLUMNS_COMMENTS_MACRO_NAME, kwargs={"relation": relation})
             )
-        )
-
-        columns = []
-        for row in rows:
-            if row["col_name"].startswith("#"):
-                break
-            columns.append(
-                DatabricksColumn(
-                    column=row["col_name"], dtype=row["data_type"], comment=row["comment"]
+            columns = []
+            for row in rows:
+                if row["col_name"].startswith("#"):
+                    break
+                columns.append(
+                    DatabricksColumn(
+                        column=row["col_name"], dtype=row["data_type"], comment=row["comment"]
+                    )
                 )
-            )
+        except DbtRuntimeError as e:
+            # spark would throw error when table doesn't exist, where other
+            # CDW would just return and empty list, normalizing the behavior here
+            errmsg = getattr(e, "msg", "")
+            found_msgs = (msg in errmsg for msg in TABLE_OR_VIEW_NOT_FOUND_MESSAGES)
+            if any(found_msgs):
+                columns = []
+            else:
+                raise e
 
         return columns
 
     def _get_updated_relation(
         self, relation: DatabricksRelation
     ) -> Tuple[DatabricksRelation, List[DatabricksColumn]]:
-        rows = list(
-            handle_missing_objects(
-                lambda: self.execute_macro(
+        try:
+            rows: List[Row] = list(
+                self.execute_macro(
                     GET_COLUMNS_IN_RELATION_RAW_MACRO_NAME,
                     kwargs={"relation": relation},
-                ),
-                AttrDict(),
+                )
             )
-        )
-        metadata, columns = self.parse_describe_extended(relation, rows)
+            metadata, columns = self.parse_describe_extended(relation, rows)
+        except DbtRuntimeError as e:
+            # spark would throw error when table doesn't exist, where other
+            # CDW would just return and empty list, normalizing the behavior here
+            errmsg = getattr(e, "msg", "")
+            found_msgs = (msg in errmsg for msg in TABLE_OR_VIEW_NOT_FOUND_MESSAGES)
+            if any(found_msgs):
+                metadata = None
+                columns = []
+            else:
+                raise e
 
         # strip hudi metadata columns.
         columns = [x for x in columns if x.name not in self.HUDI_METADATA_COLUMNS]
 
         return (
             self.Relation.create(
                 database=relation.database,
@@ -403,24 +449,24 @@
         return self._get_updated_relation(relation)[0]
 
     def parse_columns_from_information(  # type: ignore[override]
         self, relation: DatabricksRelation, information: str
     ) -> List[DatabricksColumn]:
         owner_match = re.findall(self.INFORMATION_OWNER_REGEX, information)
         owner = owner_match[0] if owner_match else None
-        matches = re.finditer(self.INFORMATION_COLUMNS_REGEX, information)
         comment_match = re.findall(self.INFORMATION_COMMENT_REGEX, information)
         table_comment = comment_match[0] if comment_match else None
+        matches = re.finditer(self.INFORMATION_COLUMNS_REGEX, information)
         columns = []
         stats_match = re.findall(self.INFORMATION_STATISTICS_REGEX, information)
         raw_table_stats = stats_match[0] if stats_match else None
         table_stats = DatabricksColumn.convert_table_stats(raw_table_stats)
 
         for match_num, match in enumerate(matches):
-            column_name, column_type, _ = match.groups()
+            column_name, column_type, nullable = match.groups()
             column = DatabricksColumn(
                 table_database=relation.database,
                 table_schema=relation.schema,
                 table_name=relation.table,
                 table_type=relation.type,
                 table_comment=table_comment,
                 column_index=match_num,
@@ -428,99 +474,101 @@
                 column=column_name,
                 dtype=DatabricksColumn.translate_type(column_type),
                 table_stats=table_stats,
             )
             columns.append(column)
         return columns
 
-    def get_catalog_by_relations(
-        self, used_schemas: FrozenSet[Tuple[str, str]], relations: Set[BaseRelation]
-    ) -> Tuple[Table, List[Exception]]:
-        relation_map: Dict[Tuple[str, str], Set[str]] = defaultdict(set)
-        for relation in relations:
-            if relation.identifier:
-                relation_map[
-                    (relation.database or "hive_metastore", relation.schema or "schema")
-                ].add(relation.identifier)
-
-        return self._get_catalog_for_relation_map(relation_map, used_schemas)
-
     def get_catalog(
         self,
         relation_configs: Iterable[RelationConfig],
         used_schemas: FrozenSet[Tuple[str, str]],
-    ) -> Tuple[Table, List[Exception]]:
-        relation_map: Dict[Tuple[str, str], Set[str]] = defaultdict(set)
-        for relation in relation_configs:
-            relation_map[(relation.database or "hive_metastore", relation.schema or "default")].add(
-                relation.identifier
-            )
+    ) -> Tuple[Table, List[Exception]]:  # type: ignore
+        schema_map = self._get_catalog_schemas(relation_configs)
 
-        return self._get_catalog_for_relation_map(relation_map, used_schemas)
-
-    def _get_catalog_for_relation_map(
-        self,
-        relation_map: Dict[Tuple[str, str], Set[str]],
-        used_schemas: FrozenSet[Tuple[str, str]],
-    ) -> Tuple[Table, List[Exception]]:
         with executor(self.config) as tpe:
             futures: List[Future[Table]] = []
-            for schema, relations in relation_map.items():
-                if schema in used_schemas:
-                    identifier = get_identifier_list_string(relations)
-                    if identifier:
+            for info, schemas in schema_map.items():
+                if is_hive_metastore(info.database):
+                    for schema in schemas:
                         futures.append(
                             tpe.submit_connected(
                                 self,
-                                str(schema),
-                                self._get_schema_for_catalog,
-                                schema[0],
-                                schema[1],
-                                identifier,
+                                "hive_metastore",
+                                self._get_hive_catalog,
+                                schema,
+                                "*",
                             )
                         )
+                else:
+                    name = ".".join([str(info.database), "information_schema"])
+                    fut = tpe.submit_connected(
+                        self, name, self._get_one_unity_catalog, info, used_schemas
+                    )
+                    futures.append(fut)
             catalogs, exceptions = catch_as_completed(futures)
         return catalogs, exceptions
 
-    def _list_relations_with_information(
-        self, schema_relation: DatabricksRelation
-    ) -> List[Tuple[DatabricksRelation, str]]:
-        results = self._show_table_extended(schema_relation)
+    def _get_one_unity_catalog(
+        self, info: InformationSchema, schemas: FrozenSet[Tuple[str, str]]
+    ) -> Table:
+        kwargs = {
+            "information_schema": info,
+            "schemas": schemas,
+        }
+        table = self.execute_macro(GET_CATALOG_MACRO_NAME, kwargs=kwargs)
 
-        relations: List[Tuple[DatabricksRelation, str]] = []
-        for name, information in results.select(["tableName", "information"]):
-            rel_type = RelationType.View if "Type: VIEW" in information else RelationType.Table
-            relation = self.Relation.create(
-                database=schema_relation.database.lower() if schema_relation.database else None,
-                schema=schema_relation.schema.lower() if schema_relation.schema else None,
-                identifier=name,
-                type=rel_type,
-            )
-            relations.append((relation, information))
+        results = self._catalog_filter_table(table, schemas)
+        return results
 
-        return relations
+    def get_catalog_by_relations(
+        self, used_schemas: FrozenSet[Tuple[str, str]], relations: Set[BaseRelation]
+    ) -> Tuple[Table, List[Exception]]:
+        with executor(self.config) as tpe:
+            relations_by_catalog = self._get_catalog_relations_by_info_schema(relations)
+            futures: List[Future[Table]] = []
 
-    def _show_table_extended(self, schema_relation: DatabricksRelation) -> Table:
-        kwargs = {"schema_relation": schema_relation}
+            for info_schema, catalog_relations in relations_by_catalog.items():
+                if is_hive_metastore(info_schema.database):
+                    schema_map = defaultdict(list)
+                    for relation in catalog_relations:
+                        schema_map[relation.schema].append(relation)
 
-        def exec() -> AttrDict:
-            with self._catalog(schema_relation.database):
-                return self.execute_macro(SHOW_TABLE_EXTENDED_MACRO_NAME, kwargs=kwargs)
+                    for schema, schema_relations in schema_map.items():
+                        table_names = extract_identifiers(schema_relations)
+                        futures.append(
+                            tpe.submit_connected(
+                                self,
+                                "hive_metastore",
+                                self._get_hive_catalog,
+                                schema,
+                                get_identifier_list_string(table_names),
+                            )
+                        )
+                else:
+                    name = ".".join([str(info_schema.database), "information_schema"])
+                    fut = tpe.submit_connected(
+                        self,
+                        name,
+                        self._get_one_catalog_by_relations,
+                        info_schema,
+                        catalog_relations,
+                        used_schemas,
+                    )
+                    futures.append(fut)
 
-        return Table(
-            handle_missing_objects(exec, AttrDict()),
-            column_names=["schema", "tableName", "isTemporary", "information"],
-        )
+            catalogs, exceptions = catch_as_completed(futures)
+        return catalogs, exceptions
 
-    def _get_schema_for_catalog(self, catalog: str, schema: str, identifier: str) -> Table:
+    def _get_hive_catalog(self, schema: str, identifier: str) -> Table:
         columns: List[Dict[str, Any]] = []
 
         if identifier:
             schema_relation = self.Relation.create(
-                database=catalog or "hive_metastore",
+                database="hive_metastore",
                 schema=schema,
                 identifier=identifier,
                 quote_policy=self.config.quoting,
             )
             for relation, information in self._list_relations_with_information(schema_relation):
                 columns.extend(self._get_columns_for_catalog(relation, information))
         return Table.from_object(columns, column_types=DEFAULT_TYPE_TESTER)
```

### Comparing `dbt-databricks-1.8.0rc1/dbt/adapters/databricks/logging.py` & `dbt-databricks-2.0.0rc1/dbt/adapters/databricks/logging.py`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.0rc1/dbt/adapters/databricks/python_submissions.py` & `dbt-databricks-2.0.0rc1/dbt/adapters/databricks/python_submissions.py`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.0rc1/dbt/adapters/databricks/relation.py` & `dbt-databricks-2.0.0rc1/dbt/adapters/databricks/relation.py`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.0rc1/dbt/adapters/databricks/relation_configs/base.py` & `dbt-databricks-2.0.0rc1/dbt/adapters/databricks/relation_configs/base.py`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.0rc1/dbt/adapters/databricks/relation_configs/comment.py` & `dbt-databricks-2.0.0rc1/dbt/adapters/databricks/relation_configs/comment.py`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.0rc1/dbt/adapters/databricks/relation_configs/incremental.py` & `dbt-databricks-2.0.0rc1/dbt/adapters/databricks/relation_configs/incremental.py`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.0rc1/dbt/adapters/databricks/relation_configs/materialized_view.py` & `dbt-databricks-2.0.0rc1/dbt/adapters/databricks/relation_configs/materialized_view.py`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.0rc1/dbt/adapters/databricks/relation_configs/partitioning.py` & `dbt-databricks-2.0.0rc1/dbt/adapters/databricks/relation_configs/partitioning.py`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.0rc1/dbt/adapters/databricks/relation_configs/query.py` & `dbt-databricks-2.0.0rc1/dbt/adapters/databricks/relation_configs/query.py`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.0rc1/dbt/adapters/databricks/relation_configs/refresh.py` & `dbt-databricks-2.0.0rc1/dbt/adapters/databricks/relation_configs/refresh.py`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.0rc1/dbt/adapters/databricks/relation_configs/streaming_table.py` & `dbt-databricks-2.0.0rc1/dbt/adapters/databricks/relation_configs/streaming_table.py`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.0rc1/dbt/adapters/databricks/relation_configs/tags.py` & `dbt-databricks-2.0.0rc1/dbt/adapters/databricks/relation_configs/tags.py`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.0rc1/dbt/adapters/databricks/relation_configs/tblproperties.py` & `dbt-databricks-2.0.0rc1/dbt/adapters/databricks/relation_configs/tblproperties.py`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.0rc1/dbt/adapters/databricks/utils.py` & `dbt-databricks-2.0.0rc1/dbt/adapters/databricks/utils.py`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.0rc1/dbt/include/databricks/macros/adapters/catalog.sql` & `dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/adapters/catalog.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.0rc1/dbt/include/databricks/macros/adapters/copy_into.sql` & `dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/adapters/copy_into.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.0rc1/dbt/include/databricks/macros/adapters/databricks_catalog.sql` & `dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/adapters/databricks_catalog.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.0rc1/dbt/include/databricks/macros/adapters/metadata.sql` & `dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/adapters/metadata.sql`

 * *Files 0% similar despite different names*

```diff
@@ -131,14 +131,15 @@
   {% do return(load_result('get_uc_tables_with_columns').table) %}
 {% endmacro %}
 
 {% macro get_uc_tables(relation) %}
   {% call statement('get_uc_tables', fetch_result=True) -%}
     select
       table_name,
+      comment,
       if(table_type = 'EXTERNAL' or table_type = 'MANAGED', 'table', lower(table_type)) as table_type,
       lower(data_source_format) as file_format,
       table_owner
     from `{{ relation.database }}`.`information_schema`.`tables`
     where table_schema = '{{ relation.schema }}'
     {% if relation.identifier %}
       and table_name = '{{ relation.identifier }}'
```

### Comparing `dbt-databricks-1.8.0rc1/dbt/include/databricks/macros/adapters/persist_docs.sql` & `dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/adapters/persist_docs.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.0rc1/dbt/include/databricks/macros/adapters/python.sql` & `dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/adapters/python.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.0rc1/dbt/include/databricks/macros/adapters/relation.sql` & `dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/adapters/relation.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.0rc1/dbt/include/databricks/macros/etc/statement.sql` & `dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/etc/statement.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.0rc1/dbt/include/databricks/macros/materializations/clone.sql` & `dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/materializations/clone.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.0rc1/dbt/include/databricks/macros/materializations/incremental/incremental.sql` & `dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/materializations/incremental/incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.0rc1/dbt/include/databricks/macros/materializations/incremental/strategies.sql` & `dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/materializations/incremental/strategies.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.0rc1/dbt/include/databricks/macros/materializations/incremental/validate.sql` & `dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/materializations/incremental/validate.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.0rc1/dbt/include/databricks/macros/materializations/materialized_view.sql` & `dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/materializations/materialized_view.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.0rc1/dbt/include/databricks/macros/materializations/seeds/helpers.sql` & `dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/materializations/seeds/helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.0rc1/dbt/include/databricks/macros/materializations/seeds/seeds.sql` & `dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/materializations/seeds/seeds.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.0rc1/dbt/include/databricks/macros/materializations/snapshot.sql` & `dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/materializations/snapshot.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.0rc1/dbt/include/databricks/macros/materializations/streaming_table.sql` & `dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/materializations/streaming_table.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.0rc1/dbt/include/databricks/macros/materializations/table.sql` & `dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/materializations/table.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.0rc1/dbt/include/databricks/macros/materializations/view.sql` & `dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/materializations/view.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.0rc1/dbt/include/databricks/macros/relations/components/refresh_schedule.sql` & `dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/relations/components/refresh_schedule.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.0rc1/dbt/include/databricks/macros/relations/constraints.sql` & `dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/relations/constraints.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.0rc1/dbt/include/databricks/macros/relations/create.sql` & `dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/relations/create.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.0rc1/dbt/include/databricks/macros/relations/drop.sql` & `dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/relations/drop.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.0rc1/dbt/include/databricks/macros/relations/location.sql` & `dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/relations/location.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.0rc1/dbt/include/databricks/macros/relations/materialized_view/alter.sql` & `dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/relations/materialized_view/alter.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.0rc1/dbt/include/databricks/macros/relations/materialized_view/create.sql` & `dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/relations/materialized_view/create.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.0rc1/dbt/include/databricks/macros/relations/optimize.sql` & `dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/relations/optimize.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.0rc1/dbt/include/databricks/macros/relations/replace.sql` & `dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/relations/replace.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.0rc1/dbt/include/databricks/macros/relations/streaming_table/alter.sql` & `dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/relations/streaming_table/alter.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.0rc1/dbt/include/databricks/macros/relations/streaming_table/create.sql` & `dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/relations/streaming_table/create.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.0rc1/dbt/include/databricks/macros/relations/table/create.sql` & `dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/relations/table/create.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.0rc1/dbt/include/databricks/macros/relations/tags.sql` & `dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/relations/tags.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.0rc1/dbt/include/databricks/macros/relations/tblproperties.sql` & `dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/relations/tblproperties.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.0rc1/dbt/include/databricks/macros/relations/view/create.sql` & `dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/relations/view/create.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.0rc1/dbt/include/databricks/profile_template.yml` & `dbt-databricks-2.0.0rc1/dbt/include/databricks/profile_template.yml`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.0rc1/dbt_databricks.egg-info/PKG-INFO` & `dbt-databricks-2.0.0rc1/dbt_databricks.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,109 +1,107 @@
 Metadata-Version: 2.1
 Name: dbt-databricks
-Version: 1.8.0rc1
+Version: 2.0.0rc1
 Summary: The Databricks adapter plugin for dbt
 Home-page: https://github.com/databricks/dbt-databricks
 Author: Databricks
 Author-email: feedback@databricks.com
-License: UNKNOWN
-Description: <p align="center">
-          <img src="https://bynder-public-us-west-2.s3.amazonaws.com/styleguide/ABB317701CA31CB7F29268E32B303CAE-pdf-column-1.png" alt="databricks logo" width="50%" />
-          <img src="https://raw.githubusercontent.com/dbt-labs/dbt/ec7dee39f793aa4f7dd3dae37282cc87664813e4/etc/dbt-logo-full.svg" alt="dbt logo" width="250"/>
-        </p>
-        <p align="center">
-          <a href="https://github.com/databricks/dbt-databricks/actions/workflows/main.yml">
-            <img src="https://github.com/databricks/dbt-databricks/actions/workflows/main.yml/badge.svg?event=push" alt="Unit Tests Badge"/>
-          </a>
-          <a href="https://github.com/databricks/dbt-databricks/actions/workflows/integration.yml">
-            <img src="https://github.com/databricks/dbt-databricks/actions/workflows/integration.yml/badge.svg?event=push" alt="Integration Tests Badge"/>
-          </a>
-        </p>
-        
-        **[dbt](https://www.getdbt.com/)** enables data analysts and engineers to transform their data using the same practices that software engineers use to build applications.
-        
-        The **[Databricks Lakehouse](https://www.databricks.com/)** provides one simple platform to unify all your data, analytics and AI workloads.
-        
-        # dbt-databricks
-        
-        The `dbt-databricks` adapter contains all of the code enabling dbt to work with Databricks. This adapter is based off the amazing work done in [dbt-spark](https://github.com/dbt-labs/dbt-spark). Some key features include:
-        
-        - **Easy setup**. No need to install an ODBC driver as the adapter uses pure Python APIs.
-        - **Open by default**. For example, it uses the the open and performant [Delta](https://delta.io/) table format by default. This has many benefits, including letting you use `MERGE` as the the default incremental materialization strategy.
-        - **Support for Unity Catalog**. dbt-databricks>=1.1.1 supports the 3-level namespace of Unity Catalog (catalog / schema / relations) so you can organize and secure your data the way you like.
-        - **Performance**. The adapter generates SQL expressions that are automatically accelerated by the native, vectorized [Photon](https://databricks.com/product/photon) execution engine.
-        
-        ## Choosing between dbt-databricks and dbt-spark
-        If you are developing a dbt project on Databricks, we recommend using `dbt-databricks` for the reasons noted above.
-        
-        `dbt-spark` is an actively developed adapter which works with Databricks as well as Apache Spark anywhere it is hosted e.g. on AWS EMR.
-        
-        ## Getting started
-        
-        ### Installation
-        
-        Install using pip:
-        ```nofmt
-        pip install dbt-databricks
-        ```
-        
-        Upgrade to the latest version
-        ```nofmt
-        pip install --upgrade dbt-databricks
-        ```
-        
-        ### Profile Setup
-        
-        ```nofmt
-        your_profile_name:
-          target: dev
-          outputs:
-            dev:
-              type: databricks
-              catalog: [optional catalog name, if you are using Unity Catalog, only available in dbt-databricks>=1.1.1]
-              schema: [database/schema name]
-              host: [your.databrickshost.com]
-              http_path: [/sql/your/http/path]
-              token: [dapiXXXXXXXXXXXXXXXXXXXXXXX]
-        ```
-        
-        ### Quick Starts
-        
-        These following quick starts will get you up and running with the `dbt-databricks` adapter:
-        - [Developing your first dbt project](https://github.com/databricks/dbt-databricks/blob/main/docs/local-dev.md)
-        - Using dbt Cloud with Databricks ([Azure](https://docs.microsoft.com/en-us/azure/databricks/integrations/prep/dbt-cloud) | [AWS](https://docs.databricks.com/integrations/prep/dbt-cloud.html))
-        - [Running dbt production jobs on Databricks Workflows](https://github.com/databricks/dbt-databricks/blob/main/docs/databricks-workflows.md)
-        - [Using Unity Catalog with dbt-databricks](https://github.com/databricks/dbt-databricks/blob/main/docs/uc.md)
-        - [Using GitHub Actions for dbt CI/CD on Databricks](https://github.com/databricks/dbt-databricks/blob/main/docs/github-actions.md)
-        - [Loading data from S3 into Delta using the databricks_copy_into macro](https://github.com/databricks/dbt-databricks/blob/main/docs/databricks-copy-into-macro-aws.md)
-        - [Contribute to this repository](CONTRIBUTING.MD)
-        
-        ### Compatibility
-        
-        The `dbt-databricks` adapter has been tested:
-        
-        - with Python 3.7 or above.
-        - against `Databricks SQL` and `Databricks runtime releases 9.1 LTS` and later.
-        
-        ### Tips and Tricks
-        ## Choosing compute for a Python model
-        You can override the compute used for a specific Python model by setting the `http_path` property in model configuration. This can be useful if, for example, you want to run a Python model on an All Purpose cluster, while running SQL models on a SQL Warehouse. Note that this capability is only available for Python models.
-        
-        ```
-        def model(dbt, session):
-            dbt.config(
-              http_path="sql/protocolv1/..."
-            )
-        ```
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+
+<p align="center">
+  <img src="https://bynder-public-us-west-2.s3.amazonaws.com/styleguide/ABB317701CA31CB7F29268E32B303CAE-pdf-column-1.png" alt="databricks logo" width="50%" />
+  <img src="https://raw.githubusercontent.com/dbt-labs/dbt/ec7dee39f793aa4f7dd3dae37282cc87664813e4/etc/dbt-logo-full.svg" alt="dbt logo" width="250"/>
+</p>
+<p align="center">
+  <a href="https://github.com/databricks/dbt-databricks/actions/workflows/main.yml">
+    <img src="https://github.com/databricks/dbt-databricks/actions/workflows/main.yml/badge.svg?event=push" alt="Unit Tests Badge"/>
+  </a>
+  <a href="https://github.com/databricks/dbt-databricks/actions/workflows/integration.yml">
+    <img src="https://github.com/databricks/dbt-databricks/actions/workflows/integration.yml/badge.svg?event=push" alt="Integration Tests Badge"/>
+  </a>
+</p>
+
+**[dbt](https://www.getdbt.com/)** enables data analysts and engineers to transform their data using the same practices that software engineers use to build applications.
+
+The **[Databricks Lakehouse](https://www.databricks.com/)** provides one simple platform to unify all your data, analytics and AI workloads.
+
+# dbt-databricks
+
+The `dbt-databricks` adapter contains all of the code enabling dbt to work with Databricks. This adapter is based off the amazing work done in [dbt-spark](https://github.com/dbt-labs/dbt-spark). Some key features include:
+
+- **Easy setup**. No need to install an ODBC driver as the adapter uses pure Python APIs.
+- **Open by default**. For example, it uses the the open and performant [Delta](https://delta.io/) table format by default. This has many benefits, including letting you use `MERGE` as the the default incremental materialization strategy.
+- **Support for Unity Catalog**. dbt-databricks>=1.1.1 supports the 3-level namespace of Unity Catalog (catalog / schema / relations) so you can organize and secure your data the way you like.
+- **Performance**. The adapter generates SQL expressions that are automatically accelerated by the native, vectorized [Photon](https://databricks.com/product/photon) execution engine.
+
+## Choosing between dbt-databricks and dbt-spark
+If you are developing a dbt project on Databricks, we recommend using `dbt-databricks` for the reasons noted above.
+
+`dbt-spark` is an actively developed adapter which works with Databricks as well as Apache Spark anywhere it is hosted e.g. on AWS EMR.
+
+## Getting started
+
+### Installation
+
+Install using pip:
+```nofmt
+pip install dbt-databricks
+```
+
+Upgrade to the latest version
+```nofmt
+pip install --upgrade dbt-databricks
+```
+
+### Profile Setup
+
+```nofmt
+your_profile_name:
+  target: dev
+  outputs:
+    dev:
+      type: databricks
+      catalog: [optional catalog name, if you are using Unity Catalog, only available in dbt-databricks>=1.1.1]
+      schema: [database/schema name]
+      host: [your.databrickshost.com]
+      http_path: [/sql/your/http/path]
+      token: [dapiXXXXXXXXXXXXXXXXXXXXXXX]
+```
+
+### Quick Starts
+
+These following quick starts will get you up and running with the `dbt-databricks` adapter:
+- [Developing your first dbt project](https://github.com/databricks/dbt-databricks/blob/main/docs/local-dev.md)
+- Using dbt Cloud with Databricks ([Azure](https://docs.microsoft.com/en-us/azure/databricks/integrations/prep/dbt-cloud) | [AWS](https://docs.databricks.com/integrations/prep/dbt-cloud.html))
+- [Running dbt production jobs on Databricks Workflows](https://github.com/databricks/dbt-databricks/blob/main/docs/databricks-workflows.md)
+- [Using Unity Catalog with dbt-databricks](https://github.com/databricks/dbt-databricks/blob/main/docs/uc.md)
+- [Using GitHub Actions for dbt CI/CD on Databricks](https://github.com/databricks/dbt-databricks/blob/main/docs/github-actions.md)
+- [Loading data from S3 into Delta using the databricks_copy_into macro](https://github.com/databricks/dbt-databricks/blob/main/docs/databricks-copy-into-macro-aws.md)
+- [Contribute to this repository](CONTRIBUTING.MD)
+
+### Compatibility
+
+The `dbt-databricks` adapter has been tested:
+
+- with Python 3.7 or above.
+- against `Databricks SQL` and `Databricks runtime releases 9.1 LTS` and later.
+
+### Tips and Tricks
+## Choosing compute for a Python model
+You can override the compute used for a specific Python model by setting the `http_path` property in model configuration. This can be useful if, for example, you want to run a Python model on an All Purpose cluster, while running SQL models on a SQL Warehouse. Note that this capability is only available for Python models.
+
+```
+def model(dbt, session):
+    dbt.config(
+      http_path="sql/protocolv1/..."
+    )
+```
```

### Comparing `dbt-databricks-1.8.0rc1/dbt_databricks.egg-info/SOURCES.txt` & `dbt-databricks-2.0.0rc1/dbt_databricks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.0rc1/setup.py` & `dbt-databricks-2.0.0rc1/setup.py`

 * *Files identical despite different names*

