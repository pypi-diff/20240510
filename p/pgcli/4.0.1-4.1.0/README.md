# Comparing `tmp/pgcli-4.0.1.tar.gz` & `tmp/pgcli-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pgcli-4.0.1.tar", last modified: Tue Oct 31 03:34:21 2023, max compression
+gzip compressed data, was "pgcli-4.1.0.tar", last modified: Fri May 10 03:29:58 2024, max compression
```

## Comparing `pgcli-4.0.1.tar` & `pgcli-4.1.0.tar`

### file list

```diff
@@ -1,110 +1,111 @@
-drwxr-xr-x   0 jbennet    (501) staff       (20)        0 2023-10-31 03:34:21.238039 pgcli-4.0.1/
--rw-r--r--   0 jbennet    (501) staff       (20)     2974 2023-10-29 23:11:56.000000 pgcli-4.0.1/AUTHORS
--rw-r--r--   0 jbennet    (501) staff       (20)     1455 2023-09-27 04:14:56.000000 pgcli-4.0.1/LICENSE.txt
--rw-r--r--   0 jbennet    (501) staff       (20)       93 2023-09-27 04:14:56.000000 pgcli-4.0.1/MANIFEST.in
--rw-r--r--   0 jbennet    (501) staff       (20)    13672 2023-10-31 03:34:21.237588 pgcli-4.0.1/PKG-INFO
--rw-r--r--   0 jbennet    (501) staff       (20)    12165 2023-10-29 23:11:56.000000 pgcli-4.0.1/README.rst
--rw-r--r--   0 jbennet    (501) staff       (20)    47365 2023-10-31 03:33:23.000000 pgcli-4.0.1/changelog.rst
-drwxr-xr-x   0 jbennet    (501) staff       (20)        0 2023-10-31 03:34:21.205000 pgcli-4.0.1/pgcli/
--rw-r--r--   0 jbennet    (501) staff       (20)       22 2023-10-31 03:33:04.000000 pgcli-4.0.1/pgcli/__init__.py
--rw-r--r--   0 jbennet    (501) staff       (20)      101 2023-09-27 04:14:56.000000 pgcli-4.0.1/pgcli/__main__.py
--rw-r--r--   0 jbennet    (501) staff       (20)     1622 2023-09-27 04:14:56.000000 pgcli-4.0.1/pgcli/auth.py
--rw-r--r--   0 jbennet    (501) staff       (20)     5264 2023-10-11 17:48:27.000000 pgcli-4.0.1/pgcli/completion_refresher.py
--rw-r--r--   0 jbennet    (501) staff       (20)     2880 2023-09-27 04:14:56.000000 pgcli-4.0.1/pgcli/config.py
--rw-r--r--   0 jbennet    (501) staff       (20)      546 2023-09-27 04:14:56.000000 pgcli-4.0.1/pgcli/explain_output_formatter.py
--rw-r--r--   0 jbennet    (501) staff       (20)     4178 2023-09-27 04:14:56.000000 pgcli-4.0.1/pgcli/key_bindings.py
--rw-r--r--   0 jbennet    (501) staff       (20)     2262 2023-09-27 04:14:56.000000 pgcli-4.0.1/pgcli/magic.py
--rw-r--r--   0 jbennet    (501) staff       (20)    61900 2023-10-07 00:43:46.000000 pgcli-4.0.1/pgcli/main.py
-drwxr-xr-x   0 jbennet    (501) staff       (20)        0 2023-10-31 03:34:21.208852 pgcli-4.0.1/pgcli/packages/
--rw-r--r--   0 jbennet    (501) staff       (20)        0 2023-09-27 04:14:56.000000 pgcli-4.0.1/pgcli/packages/__init__.py
-drwxr-xr-x   0 jbennet    (501) staff       (20)        0 2023-10-31 03:34:21.210110 pgcli-4.0.1/pgcli/packages/formatter/
--rw-r--r--   0 jbennet    (501) staff       (20)       15 2023-09-27 04:14:56.000000 pgcli-4.0.1/pgcli/packages/formatter/__init__.py
--rw-r--r--   0 jbennet    (501) staff       (20)     2125 2023-09-27 04:14:56.000000 pgcli-4.0.1/pgcli/packages/formatter/sqlformatter.py
-drwxr-xr-x   0 jbennet    (501) staff       (20)        0 2023-10-31 03:34:21.212220 pgcli-4.0.1/pgcli/packages/parseutils/
--rw-r--r--   0 jbennet    (501) staff       (20)     1728 2023-09-27 04:14:56.000000 pgcli-4.0.1/pgcli/packages/parseutils/__init__.py
--rw-r--r--   0 jbennet    (501) staff       (20)     4776 2023-09-27 04:14:56.000000 pgcli-4.0.1/pgcli/packages/parseutils/ctes.py
--rw-r--r--   0 jbennet    (501) staff       (20)     5453 2023-09-27 04:14:56.000000 pgcli-4.0.1/pgcli/packages/parseutils/meta.py
--rw-r--r--   0 jbennet    (501) staff       (20)     6603 2023-09-27 04:14:56.000000 pgcli-4.0.1/pgcli/packages/parseutils/tables.py
--rw-r--r--   0 jbennet    (501) staff       (20)     4449 2023-09-27 04:14:56.000000 pgcli-4.0.1/pgcli/packages/parseutils/utils.py
-drwxr-xr-x   0 jbennet    (501) staff       (20)        0 2023-10-31 03:34:21.213302 pgcli-4.0.1/pgcli/packages/pgliterals/
--rw-r--r--   0 jbennet    (501) staff       (20)        0 2023-09-27 04:14:56.000000 pgcli-4.0.1/pgcli/packages/pgliterals/__init__.py
--rw-r--r--   0 jbennet    (501) staff       (20)      386 2023-09-27 04:14:56.000000 pgcli-4.0.1/pgcli/packages/pgliterals/main.py
--rw-r--r--   0 jbennet    (501) staff       (20)    12982 2023-09-27 04:14:56.000000 pgcli-4.0.1/pgcli/packages/pgliterals/pgliterals.json
--rw-r--r--   0 jbennet    (501) staff       (20)     1532 2023-09-27 04:14:56.000000 pgcli-4.0.1/pgcli/packages/prioritization.py
--rw-r--r--   0 jbennet    (501) staff       (20)     1125 2023-10-29 23:11:56.000000 pgcli-4.0.1/pgcli/packages/prompt_utils.py
--rw-r--r--   0 jbennet    (501) staff       (20)    22705 2023-09-27 04:14:56.000000 pgcli-4.0.1/pgcli/packages/sqlcompletion.py
--rw-r--r--   0 jbennet    (501) staff       (20)     2027 2023-09-27 04:14:56.000000 pgcli-4.0.1/pgcli/pgbuffer.py
--rw-r--r--   0 jbennet    (501) staff       (20)     8880 2023-10-07 00:33:55.000000 pgcli-4.0.1/pgcli/pgclirc
--rw-r--r--   0 jbennet    (501) staff       (20)    42591 2023-10-07 00:33:55.000000 pgcli-4.0.1/pgcli/pgcompleter.py
--rw-r--r--   0 jbennet    (501) staff       (20)    33530 2023-10-29 23:11:56.000000 pgcli-4.0.1/pgcli/pgexecute.py
--rw-r--r--   0 jbennet    (501) staff       (20)     4886 2023-09-27 04:14:56.000000 pgcli-4.0.1/pgcli/pgstyle.py
--rw-r--r--   0 jbennet    (501) staff       (20)     2409 2023-09-27 04:14:56.000000 pgcli-4.0.1/pgcli/pgtoolbar.py
--rw-r--r--   0 jbennet    (501) staff       (20)    15643 2023-09-27 04:14:56.000000 pgcli-4.0.1/pgcli/pyev.py
-drwxr-xr-x   0 jbennet    (501) staff       (20)        0 2023-10-31 03:34:21.207136 pgcli-4.0.1/pgcli.egg-info/
--rw-r--r--   0 jbennet    (501) staff       (20)    13672 2023-10-31 03:34:21.000000 pgcli-4.0.1/pgcli.egg-info/PKG-INFO
--rw-r--r--   0 jbennet    (501) staff       (20)     2684 2023-10-31 03:34:21.000000 pgcli-4.0.1/pgcli.egg-info/SOURCES.txt
--rw-r--r--   0 jbennet    (501) staff       (20)       65 2023-10-31 03:34:21.000000 pgcli-4.0.1/pgcli.egg-info/dependency_links.txt
--rw-r--r--   0 jbennet    (501) staff       (20)       41 2023-10-31 03:34:21.000000 pgcli-4.0.1/pgcli.egg-info/entry_points.txt
--rw-r--r--   0 jbennet    (501) staff       (20)      245 2023-10-31 03:34:21.000000 pgcli-4.0.1/pgcli.egg-info/requires.txt
--rw-r--r--   0 jbennet    (501) staff       (20)        6 2023-10-31 03:34:21.000000 pgcli-4.0.1/pgcli.egg-info/top_level.txt
--rw-r--r--   0 jbennet    (501) staff       (20)      257 2023-10-11 17:48:27.000000 pgcli-4.0.1/pyproject.toml
--rw-r--r--   0 jbennet    (501) staff       (20)       38 2023-10-31 03:34:21.238143 pgcli-4.0.1/setup.cfg
--rw-r--r--   0 jbennet    (501) staff       (20)     2645 2023-10-29 23:11:56.000000 pgcli-4.0.1/setup.py
-drwxr-xr-x   0 jbennet    (501) staff       (20)        0 2023-10-31 03:34:21.223727 pgcli-4.0.1/tests/
--rw-r--r--   0 jbennet    (501) staff       (20)     1104 2023-09-27 04:14:56.000000 pgcli-4.0.1/tests/conftest.py
-drwxr-xr-x   0 jbennet    (501) staff       (20)        0 2023-10-31 03:34:21.229776 pgcli-4.0.1/tests/features/
--rw-r--r--   0 jbennet    (501) staff       (20)        0 2023-09-27 04:14:56.000000 pgcli-4.0.1/tests/features/__init__.py
--rw-r--r--   0 jbennet    (501) staff       (20)      407 2023-09-27 04:14:56.000000 pgcli-4.0.1/tests/features/auto_vertical.feature
--rw-r--r--   0 jbennet    (501) staff       (20)     2296 2023-09-27 04:39:37.000000 pgcli-4.0.1/tests/features/basic_commands.feature
--rw-r--r--   0 jbennet    (501) staff       (20)      566 2023-09-27 04:14:56.000000 pgcli-4.0.1/tests/features/crud_database.feature
--rw-r--r--   0 jbennet    (501) staff       (20)     1608 2023-09-27 04:14:56.000000 pgcli-4.0.1/tests/features/crud_table.feature
--rw-r--r--   0 jbennet    (501) staff       (20)     2058 2023-09-27 04:14:56.000000 pgcli-4.0.1/tests/features/db_utils.py
--rw-r--r--   0 jbennet    (501) staff       (20)     7255 2023-10-11 17:48:27.000000 pgcli-4.0.1/tests/features/environment.py
--rw-r--r--   0 jbennet    (501) staff       (20)      852 2023-09-27 04:14:56.000000 pgcli-4.0.1/tests/features/expanded.feature
-drwxr-xr-x   0 jbennet    (501) staff       (20)        0 2023-10-31 03:34:21.230505 pgcli-4.0.1/tests/features/fixture_data/
--rw-r--r--   0 jbennet    (501) staff       (20)     1950 2023-09-27 04:14:56.000000 pgcli-4.0.1/tests/features/fixture_data/help.txt
--rw-r--r--   0 jbennet    (501) staff       (20)     1254 2023-09-27 04:14:56.000000 pgcli-4.0.1/tests/features/fixture_data/help_commands.txt
--rw-r--r--   0 jbennet    (501) staff       (20)      798 2023-09-27 04:14:56.000000 pgcli-4.0.1/tests/features/fixture_utils.py
--rw-r--r--   0 jbennet    (501) staff       (20)      513 2023-09-27 04:14:56.000000 pgcli-4.0.1/tests/features/iocommands.feature
--rw-r--r--   0 jbennet    (501) staff       (20)      334 2023-09-27 04:14:56.000000 pgcli-4.0.1/tests/features/named_queries.feature
--rw-r--r--   0 jbennet    (501) staff       (20)      280 2023-09-27 04:14:56.000000 pgcli-4.0.1/tests/features/pgbouncer.feature
--rw-r--r--   0 jbennet    (501) staff       (20)      167 2023-09-27 04:14:56.000000 pgcli-4.0.1/tests/features/specials.feature
-drwxr-xr-x   0 jbennet    (501) staff       (20)        0 2023-10-31 03:34:21.234692 pgcli-4.0.1/tests/features/steps/
--rw-r--r--   0 jbennet    (501) staff       (20)        0 2023-09-27 04:14:56.000000 pgcli-4.0.1/tests/features/steps/__init__.py
--rw-r--r--   0 jbennet    (501) staff       (20)     2276 2023-09-27 04:14:56.000000 pgcli-4.0.1/tests/features/steps/auto_vertical.py
--rw-r--r--   0 jbennet    (501) staff       (20)     6256 2023-10-29 23:11:56.000000 pgcli-4.0.1/tests/features/steps/basic_commands.py
--rw-r--r--   0 jbennet    (501) staff       (20)     2279 2023-09-27 04:14:56.000000 pgcli-4.0.1/tests/features/steps/crud_database.py
--rw-r--r--   0 jbennet    (501) staff       (20)     3958 2023-09-27 04:14:56.000000 pgcli-4.0.1/tests/features/steps/crud_table.py
--rw-r--r--   0 jbennet    (501) staff       (20)     2035 2023-10-29 23:11:56.000000 pgcli-4.0.1/tests/features/steps/expanded.py
--rw-r--r--   0 jbennet    (501) staff       (20)     2653 2023-09-27 04:14:56.000000 pgcli-4.0.1/tests/features/steps/iocommands.py
--rw-r--r--   0 jbennet    (501) staff       (20)     1293 2023-09-27 04:14:56.000000 pgcli-4.0.1/tests/features/steps/named_queries.py
--rw-r--r--   0 jbennet    (501) staff       (20)      558 2023-09-27 04:14:56.000000 pgcli-4.0.1/tests/features/steps/pgbouncer.py
--rw-r--r--   0 jbennet    (501) staff       (20)      724 2023-09-27 04:14:56.000000 pgcli-4.0.1/tests/features/steps/specials.py
--rw-r--r--   0 jbennet    (501) staff       (20)     2000 2023-10-08 00:06:24.000000 pgcli-4.0.1/tests/features/steps/wrappers.py
--rw-r--r--   0 jbennet    (501) staff       (20)      272 2023-09-27 04:14:56.000000 pgcli-4.0.1/tests/features/wrappager.py
-drwxr-xr-x   0 jbennet    (501) staff       (20)        0 2023-10-31 03:34:21.235557 pgcli-4.0.1/tests/formatter/
--rw-r--r--   0 jbennet    (501) staff       (20)       15 2023-09-27 04:14:56.000000 pgcli-4.0.1/tests/formatter/__init__.py
--rw-r--r--   0 jbennet    (501) staff       (20)     3563 2023-09-27 04:14:56.000000 pgcli-4.0.1/tests/formatter/test_sqlformatter.py
--rw-r--r--   0 jbennet    (501) staff       (20)     8896 2023-09-27 04:14:56.000000 pgcli-4.0.1/tests/metadata.py
-drwxr-xr-x   0 jbennet    (501) staff       (20)        0 2023-10-31 03:34:21.236580 pgcli-4.0.1/tests/parseutils/
--rw-r--r--   0 jbennet    (501) staff       (20)     3580 2023-09-27 04:14:56.000000 pgcli-4.0.1/tests/parseutils/test_ctes.py
--rw-r--r--   0 jbennet    (501) staff       (20)      596 2023-09-27 04:14:56.000000 pgcli-4.0.1/tests/parseutils/test_function_metadata.py
--rw-r--r--   0 jbennet    (501) staff       (20)     9939 2023-09-27 04:14:56.000000 pgcli-4.0.1/tests/parseutils/test_parseutils.py
--rw-r--r--   0 jbennet    (501) staff       (20)       43 2023-09-27 04:14:56.000000 pgcli-4.0.1/tests/pytest.ini
--rw-r--r--   0 jbennet    (501) staff       (20)     1481 2023-09-27 04:14:56.000000 pgcli-4.0.1/tests/test_auth.py
--rw-r--r--   0 jbennet    (501) staff       (20)     2633 2023-09-27 04:14:56.000000 pgcli-4.0.1/tests/test_completion_refresher.py
--rw-r--r--   0 jbennet    (501) staff       (20)      988 2023-09-27 04:14:56.000000 pgcli-4.0.1/tests/test_config.py
--rw-r--r--   0 jbennet    (501) staff       (20)     2823 2023-09-27 04:14:56.000000 pgcli-4.0.1/tests/test_fuzzy_completion.py
--rw-r--r--   0 jbennet    (501) staff       (20)    15956 2023-10-07 00:33:55.000000 pgcli-4.0.1/tests/test_main.py
--rw-r--r--   0 jbennet    (501) staff       (20)     4341 2023-09-27 04:14:56.000000 pgcli-4.0.1/tests/test_naive_completion.py
--rw-r--r--   0 jbennet    (501) staff       (20)     2081 2023-10-07 00:33:55.000000 pgcli-4.0.1/tests/test_pgcompleter.py
--rw-r--r--   0 jbennet    (501) staff       (20)    23369 2023-10-29 23:11:56.000000 pgcli-4.0.1/tests/test_pgexecute.py
--rw-r--r--   0 jbennet    (501) staff       (20)     2367 2023-09-27 04:14:56.000000 pgcli-4.0.1/tests/test_pgspecial.py
--rw-r--r--   0 jbennet    (501) staff       (20)      657 2023-09-27 04:14:56.000000 pgcli-4.0.1/tests/test_prioritization.py
--rw-r--r--   0 jbennet    (501) staff       (20)      523 2023-09-27 04:14:56.000000 pgcli-4.0.1/tests/test_prompt_utils.py
--rw-r--r--   0 jbennet    (501) staff       (20)     1964 2023-09-27 04:14:56.000000 pgcli-4.0.1/tests/test_rowlimit.py
--rw-r--r--   0 jbennet    (501) staff       (20)    24915 2023-09-27 04:14:56.000000 pgcli-4.0.1/tests/test_smart_completion_multiple_schemata.py
--rw-r--r--   0 jbennet    (501) staff       (20)    36355 2023-09-27 04:14:56.000000 pgcli-4.0.1/tests/test_smart_completion_public_schema_only.py
--rw-r--r--   0 jbennet    (501) staff       (20)    28885 2023-09-27 04:14:56.000000 pgcli-4.0.1/tests/test_sqlcompletion.py
--rw-r--r--   0 jbennet    (501) staff       (20)     6104 2023-09-27 04:14:56.000000 pgcli-4.0.1/tests/test_ssh_tunnel.py
--rw-r--r--   0 jbennet    (501) staff       (20)     2419 2023-09-27 04:14:56.000000 pgcli-4.0.1/tests/utils.py
+drwxr-xr-x   0 jbennet    (501) staff       (20)        0 2024-05-10 03:29:58.426921 pgcli-4.1.0/
+-rw-r--r--   0 jbennet    (501) staff       (20)     3086 2024-05-10 03:17:53.000000 pgcli-4.1.0/AUTHORS
+-rw-r--r--   0 jbennet    (501) staff       (20)     1455 2023-10-27 20:51:13.000000 pgcli-4.1.0/LICENSE.txt
+-rw-r--r--   0 jbennet    (501) staff       (20)       93 2023-10-27 20:51:13.000000 pgcli-4.1.0/MANIFEST.in
+-rw-r--r--   0 jbennet    (501) staff       (20)    13729 2024-05-10 03:29:58.426650 pgcli-4.1.0/PKG-INFO
+-rw-r--r--   0 jbennet    (501) staff       (20)    12165 2023-10-27 23:11:44.000000 pgcli-4.1.0/README.rst
+-rw-r--r--   0 jbennet    (501) staff       (20)    48497 2024-05-10 03:27:48.000000 pgcli-4.1.0/changelog.rst
+drwxr-xr-x   0 jbennet    (501) staff       (20)        0 2024-05-10 03:29:58.416504 pgcli-4.1.0/pgcli/
+-rw-r--r--   0 jbennet    (501) staff       (20)       22 2024-05-10 03:29:35.000000 pgcli-4.1.0/pgcli/__init__.py
+-rw-r--r--   0 jbennet    (501) staff       (20)      101 2023-10-27 20:51:13.000000 pgcli-4.1.0/pgcli/__main__.py
+-rw-r--r--   0 jbennet    (501) staff       (20)     1622 2023-10-27 20:51:13.000000 pgcli-4.1.0/pgcli/auth.py
+-rw-r--r--   0 jbennet    (501) staff       (20)     5264 2023-10-27 20:51:13.000000 pgcli-4.1.0/pgcli/completion_refresher.py
+-rw-r--r--   0 jbennet    (501) staff       (20)     2880 2023-10-27 20:51:13.000000 pgcli-4.1.0/pgcli/config.py
+-rw-r--r--   0 jbennet    (501) staff       (20)      546 2023-10-27 20:51:13.000000 pgcli-4.1.0/pgcli/explain_output_formatter.py
+-rw-r--r--   0 jbennet    (501) staff       (20)     4178 2023-10-27 20:51:13.000000 pgcli-4.1.0/pgcli/key_bindings.py
+-rw-r--r--   0 jbennet    (501) staff       (20)     2262 2023-10-27 20:51:13.000000 pgcli-4.1.0/pgcli/magic.py
+-rw-r--r--   0 jbennet    (501) staff       (20)    68648 2024-05-10 03:17:53.000000 pgcli-4.1.0/pgcli/main.py
+drwxr-xr-x   0 jbennet    (501) staff       (20)        0 2024-05-10 03:29:58.417761 pgcli-4.1.0/pgcli/packages/
+-rw-r--r--   0 jbennet    (501) staff       (20)        0 2023-10-27 20:51:13.000000 pgcli-4.1.0/pgcli/packages/__init__.py
+drwxr-xr-x   0 jbennet    (501) staff       (20)        0 2024-05-10 03:29:58.418034 pgcli-4.1.0/pgcli/packages/formatter/
+-rw-r--r--   0 jbennet    (501) staff       (20)       15 2023-10-27 20:51:13.000000 pgcli-4.1.0/pgcli/packages/formatter/__init__.py
+-rw-r--r--   0 jbennet    (501) staff       (20)     2125 2023-10-27 20:51:13.000000 pgcli-4.1.0/pgcli/packages/formatter/sqlformatter.py
+drwxr-xr-x   0 jbennet    (501) staff       (20)        0 2024-05-10 03:29:58.418791 pgcli-4.1.0/pgcli/packages/parseutils/
+-rw-r--r--   0 jbennet    (501) staff       (20)     1728 2023-10-27 20:51:13.000000 pgcli-4.1.0/pgcli/packages/parseutils/__init__.py
+-rw-r--r--   0 jbennet    (501) staff       (20)     4776 2023-10-27 20:51:13.000000 pgcli-4.1.0/pgcli/packages/parseutils/ctes.py
+-rw-r--r--   0 jbennet    (501) staff       (20)     5453 2023-10-27 20:51:13.000000 pgcli-4.1.0/pgcli/packages/parseutils/meta.py
+-rw-r--r--   0 jbennet    (501) staff       (20)     6603 2023-10-27 20:51:13.000000 pgcli-4.1.0/pgcli/packages/parseutils/tables.py
+-rw-r--r--   0 jbennet    (501) staff       (20)     4449 2023-10-27 20:51:13.000000 pgcli-4.1.0/pgcli/packages/parseutils/utils.py
+drwxr-xr-x   0 jbennet    (501) staff       (20)        0 2024-05-10 03:29:58.419159 pgcli-4.1.0/pgcli/packages/pgliterals/
+-rw-r--r--   0 jbennet    (501) staff       (20)        0 2023-10-27 20:51:13.000000 pgcli-4.1.0/pgcli/packages/pgliterals/__init__.py
+-rw-r--r--   0 jbennet    (501) staff       (20)      386 2023-10-27 20:51:13.000000 pgcli-4.1.0/pgcli/packages/pgliterals/main.py
+-rw-r--r--   0 jbennet    (501) staff       (20)    12982 2023-10-27 20:51:13.000000 pgcli-4.1.0/pgcli/packages/pgliterals/pgliterals.json
+-rw-r--r--   0 jbennet    (501) staff       (20)     1532 2023-10-27 20:51:13.000000 pgcli-4.1.0/pgcli/packages/prioritization.py
+-rw-r--r--   0 jbennet    (501) staff       (20)     1125 2023-10-27 20:51:13.000000 pgcli-4.1.0/pgcli/packages/prompt_utils.py
+-rw-r--r--   0 jbennet    (501) staff       (20)    22705 2023-10-27 20:51:13.000000 pgcli-4.1.0/pgcli/packages/sqlcompletion.py
+-rw-r--r--   0 jbennet    (501) staff       (20)     2027 2023-10-27 20:51:13.000000 pgcli-4.1.0/pgcli/pgbuffer.py
+-rw-r--r--   0 jbennet    (501) staff       (20)     9144 2024-05-10 03:17:53.000000 pgcli-4.1.0/pgcli/pgclirc
+-rw-r--r--   0 jbennet    (501) staff       (20)    42591 2023-10-27 20:51:13.000000 pgcli-4.1.0/pgcli/pgcompleter.py
+-rw-r--r--   0 jbennet    (501) staff       (20)    34024 2024-05-10 03:17:53.000000 pgcli-4.1.0/pgcli/pgexecute.py
+-rw-r--r--   0 jbennet    (501) staff       (20)     4886 2023-10-27 20:51:13.000000 pgcli-4.1.0/pgcli/pgstyle.py
+-rw-r--r--   0 jbennet    (501) staff       (20)     2409 2023-10-27 20:51:13.000000 pgcli-4.1.0/pgcli/pgtoolbar.py
+-rw-r--r--   0 jbennet    (501) staff       (20)    15643 2023-10-27 20:51:13.000000 pgcli-4.1.0/pgcli/pyev.py
+drwxr-xr-x   0 jbennet    (501) staff       (20)        0 2024-05-10 03:29:58.417253 pgcli-4.1.0/pgcli.egg-info/
+-rw-r--r--   0 jbennet    (501) staff       (20)    13729 2024-05-10 03:29:58.000000 pgcli-4.1.0/pgcli.egg-info/PKG-INFO
+-rw-r--r--   0 jbennet    (501) staff       (20)     2715 2024-05-10 03:29:58.000000 pgcli-4.1.0/pgcli.egg-info/SOURCES.txt
+-rw-r--r--   0 jbennet    (501) staff       (20)       65 2024-05-10 03:29:58.000000 pgcli-4.1.0/pgcli.egg-info/dependency_links.txt
+-rw-r--r--   0 jbennet    (501) staff       (20)       41 2024-05-10 03:29:58.000000 pgcli-4.1.0/pgcli.egg-info/entry_points.txt
+-rw-r--r--   0 jbennet    (501) staff       (20)      308 2024-05-10 03:29:58.000000 pgcli-4.1.0/pgcli.egg-info/requires.txt
+-rw-r--r--   0 jbennet    (501) staff       (20)        6 2024-05-10 03:29:58.000000 pgcli-4.1.0/pgcli.egg-info/top_level.txt
+-rw-r--r--   0 jbennet    (501) staff       (20)      257 2023-10-27 20:51:13.000000 pgcli-4.1.0/pyproject.toml
+-rw-r--r--   0 jbennet    (501) staff       (20)       38 2024-05-10 03:29:58.426972 pgcli-4.1.0/setup.cfg
+-rw-r--r--   0 jbennet    (501) staff       (20)     2552 2024-05-10 03:17:53.000000 pgcli-4.1.0/setup.py
+drwxr-xr-x   0 jbennet    (501) staff       (20)        0 2024-05-10 03:29:58.422052 pgcli-4.1.0/tests/
+-rw-r--r--   0 jbennet    (501) staff       (20)     1174 2024-05-10 03:17:53.000000 pgcli-4.1.0/tests/conftest.py
+drwxr-xr-x   0 jbennet    (501) staff       (20)        0 2024-05-10 03:29:58.423810 pgcli-4.1.0/tests/features/
+-rw-r--r--   0 jbennet    (501) staff       (20)        0 2023-10-27 20:51:13.000000 pgcli-4.1.0/tests/features/__init__.py
+-rw-r--r--   0 jbennet    (501) staff       (20)      407 2023-10-27 20:51:13.000000 pgcli-4.1.0/tests/features/auto_vertical.feature
+-rw-r--r--   0 jbennet    (501) staff       (20)     2296 2023-10-27 20:51:13.000000 pgcli-4.1.0/tests/features/basic_commands.feature
+-rw-r--r--   0 jbennet    (501) staff       (20)      566 2023-10-27 20:51:13.000000 pgcli-4.1.0/tests/features/crud_database.feature
+-rw-r--r--   0 jbennet    (501) staff       (20)     1608 2023-10-27 20:51:13.000000 pgcli-4.1.0/tests/features/crud_table.feature
+-rw-r--r--   0 jbennet    (501) staff       (20)     2058 2023-10-27 20:51:13.000000 pgcli-4.1.0/tests/features/db_utils.py
+-rw-r--r--   0 jbennet    (501) staff       (20)     7255 2023-10-27 20:51:13.000000 pgcli-4.1.0/tests/features/environment.py
+-rw-r--r--   0 jbennet    (501) staff       (20)      852 2023-10-27 20:51:13.000000 pgcli-4.1.0/tests/features/expanded.feature
+drwxr-xr-x   0 jbennet    (501) staff       (20)        0 2024-05-10 03:29:58.424094 pgcli-4.1.0/tests/features/fixture_data/
+-rw-r--r--   0 jbennet    (501) staff       (20)     1950 2023-10-27 20:51:13.000000 pgcli-4.1.0/tests/features/fixture_data/help.txt
+-rw-r--r--   0 jbennet    (501) staff       (20)     1254 2023-10-27 20:51:13.000000 pgcli-4.1.0/tests/features/fixture_data/help_commands.txt
+-rw-r--r--   0 jbennet    (501) staff       (20)      798 2023-10-27 20:51:13.000000 pgcli-4.1.0/tests/features/fixture_utils.py
+-rw-r--r--   0 jbennet    (501) staff       (20)      513 2023-10-27 20:51:13.000000 pgcli-4.1.0/tests/features/iocommands.feature
+-rw-r--r--   0 jbennet    (501) staff       (20)      334 2023-10-27 20:51:13.000000 pgcli-4.1.0/tests/features/named_queries.feature
+-rw-r--r--   0 jbennet    (501) staff       (20)      280 2023-10-27 20:51:13.000000 pgcli-4.1.0/tests/features/pgbouncer.feature
+-rw-r--r--   0 jbennet    (501) staff       (20)      167 2023-10-27 20:51:13.000000 pgcli-4.1.0/tests/features/specials.feature
+drwxr-xr-x   0 jbennet    (501) staff       (20)        0 2024-05-10 03:29:58.425542 pgcli-4.1.0/tests/features/steps/
+-rw-r--r--   0 jbennet    (501) staff       (20)        0 2023-10-27 20:51:13.000000 pgcli-4.1.0/tests/features/steps/__init__.py
+-rw-r--r--   0 jbennet    (501) staff       (20)     2276 2023-10-27 20:51:13.000000 pgcli-4.1.0/tests/features/steps/auto_vertical.py
+-rw-r--r--   0 jbennet    (501) staff       (20)     6256 2023-10-27 20:51:13.000000 pgcli-4.1.0/tests/features/steps/basic_commands.py
+-rw-r--r--   0 jbennet    (501) staff       (20)     2280 2024-05-10 03:17:53.000000 pgcli-4.1.0/tests/features/steps/crud_database.py
+-rw-r--r--   0 jbennet    (501) staff       (20)     3958 2023-10-27 20:51:13.000000 pgcli-4.1.0/tests/features/steps/crud_table.py
+-rw-r--r--   0 jbennet    (501) staff       (20)     2035 2023-10-27 20:51:13.000000 pgcli-4.1.0/tests/features/steps/expanded.py
+-rw-r--r--   0 jbennet    (501) staff       (20)     2653 2023-10-27 20:51:13.000000 pgcli-4.1.0/tests/features/steps/iocommands.py
+-rw-r--r--   0 jbennet    (501) staff       (20)     1293 2023-10-27 20:51:13.000000 pgcli-4.1.0/tests/features/steps/named_queries.py
+-rw-r--r--   0 jbennet    (501) staff       (20)      558 2023-10-27 20:51:13.000000 pgcli-4.1.0/tests/features/steps/pgbouncer.py
+-rw-r--r--   0 jbennet    (501) staff       (20)      724 2023-10-27 20:51:13.000000 pgcli-4.1.0/tests/features/steps/specials.py
+-rw-r--r--   0 jbennet    (501) staff       (20)     2000 2023-10-27 20:51:13.000000 pgcli-4.1.0/tests/features/steps/wrappers.py
+-rw-r--r--   0 jbennet    (501) staff       (20)      272 2023-10-27 20:51:13.000000 pgcli-4.1.0/tests/features/wrappager.py
+drwxr-xr-x   0 jbennet    (501) staff       (20)        0 2024-05-10 03:29:58.425794 pgcli-4.1.0/tests/formatter/
+-rw-r--r--   0 jbennet    (501) staff       (20)       15 2023-10-27 20:51:13.000000 pgcli-4.1.0/tests/formatter/__init__.py
+-rw-r--r--   0 jbennet    (501) staff       (20)     3563 2023-10-27 20:51:13.000000 pgcli-4.1.0/tests/formatter/test_sqlformatter.py
+-rw-r--r--   0 jbennet    (501) staff       (20)     8896 2023-10-27 20:51:13.000000 pgcli-4.1.0/tests/metadata.py
+drwxr-xr-x   0 jbennet    (501) staff       (20)        0 2024-05-10 03:29:58.426166 pgcli-4.1.0/tests/parseutils/
+-rw-r--r--   0 jbennet    (501) staff       (20)     3580 2023-10-27 20:51:13.000000 pgcli-4.1.0/tests/parseutils/test_ctes.py
+-rw-r--r--   0 jbennet    (501) staff       (20)      596 2023-10-27 20:51:13.000000 pgcli-4.1.0/tests/parseutils/test_function_metadata.py
+-rw-r--r--   0 jbennet    (501) staff       (20)     9939 2023-10-27 20:51:13.000000 pgcli-4.1.0/tests/parseutils/test_parseutils.py
+-rw-r--r--   0 jbennet    (501) staff       (20)       43 2023-10-27 20:51:13.000000 pgcli-4.1.0/tests/pytest.ini
+-rw-r--r--   0 jbennet    (501) staff       (20)      510 2024-05-10 03:17:53.000000 pgcli-4.1.0/tests/test_application_name.py
+-rw-r--r--   0 jbennet    (501) staff       (20)     1481 2023-10-27 20:51:13.000000 pgcli-4.1.0/tests/test_auth.py
+-rw-r--r--   0 jbennet    (501) staff       (20)     2633 2023-10-27 20:51:13.000000 pgcli-4.1.0/tests/test_completion_refresher.py
+-rw-r--r--   0 jbennet    (501) staff       (20)      988 2023-10-27 20:51:13.000000 pgcli-4.1.0/tests/test_config.py
+-rw-r--r--   0 jbennet    (501) staff       (20)     2823 2023-10-27 20:51:13.000000 pgcli-4.1.0/tests/test_fuzzy_completion.py
+-rw-r--r--   0 jbennet    (501) staff       (20)    18879 2024-05-10 03:17:53.000000 pgcli-4.1.0/tests/test_main.py
+-rw-r--r--   0 jbennet    (501) staff       (20)     4341 2023-10-27 20:51:13.000000 pgcli-4.1.0/tests/test_naive_completion.py
+-rw-r--r--   0 jbennet    (501) staff       (20)     2081 2023-10-27 20:51:13.000000 pgcli-4.1.0/tests/test_pgcompleter.py
+-rw-r--r--   0 jbennet    (501) staff       (20)    25102 2024-05-10 03:17:53.000000 pgcli-4.1.0/tests/test_pgexecute.py
+-rw-r--r--   0 jbennet    (501) staff       (20)     2367 2023-10-27 20:51:13.000000 pgcli-4.1.0/tests/test_pgspecial.py
+-rw-r--r--   0 jbennet    (501) staff       (20)      657 2023-10-27 20:51:13.000000 pgcli-4.1.0/tests/test_prioritization.py
+-rw-r--r--   0 jbennet    (501) staff       (20)      523 2023-10-27 20:51:13.000000 pgcli-4.1.0/tests/test_prompt_utils.py
+-rw-r--r--   0 jbennet    (501) staff       (20)     1964 2023-10-27 20:51:13.000000 pgcli-4.1.0/tests/test_rowlimit.py
+-rw-r--r--   0 jbennet    (501) staff       (20)    24915 2023-10-27 20:51:13.000000 pgcli-4.1.0/tests/test_smart_completion_multiple_schemata.py
+-rw-r--r--   0 jbennet    (501) staff       (20)    36355 2023-10-27 20:51:13.000000 pgcli-4.1.0/tests/test_smart_completion_public_schema_only.py
+-rw-r--r--   0 jbennet    (501) staff       (20)    28885 2023-10-27 20:51:13.000000 pgcli-4.1.0/tests/test_sqlcompletion.py
+-rw-r--r--   0 jbennet    (501) staff       (20)     6171 2024-05-10 03:17:53.000000 pgcli-4.1.0/tests/test_ssh_tunnel.py
+-rw-r--r--   0 jbennet    (501) staff       (20)     2419 2023-10-27 20:51:13.000000 pgcli-4.1.0/tests/utils.py
```

### Comparing `pgcli-4.0.1/AUTHORS` & `pgcli-4.1.0/AUTHORS`

 * *Files 2% similar despite different names*

```diff
@@ -126,11 +126,15 @@
     * Rigo Neri (rigoneri)
     * Anna Glasgall (annathyst)
     * Andy Schoenberger (andyscho)
     * Damien Baty (dbaty)
     * blag
     * Rob Berry (rob-b)
     * Sharon Yogev (sharonyogev)
+    * Hollis Wu (holi0317)
+    * Antonio Aguilar (crazybolillo)
+    * Andrew M. MacFie (amacfie)
+    * saucoide
 
 Creator:
 --------
 Amjith Ramanujam
```

### Comparing `pgcli-4.0.1/LICENSE.txt` & `pgcli-4.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pgcli-4.0.1/PKG-INFO` & `pgcli-4.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pgcli
-Version: 4.0.1
+Version: 4.1.0
 Summary: CLI for Postgres Database. With auto-completion and syntax highlighting.
 Home-page: http://pgcli.com
 Author: Pgcli Core Team
 Author-email: pgcli-dev@googlegroups.com
 License: BSD
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
@@ -24,18 +24,18 @@
 Requires-Python: >=3.8
 License-File: LICENSE.txt
 License-File: AUTHORS
 Requires-Dist: pgspecial>=2.0.0
 Requires-Dist: click>=4.1
 Requires-Dist: Pygments>=2.0
 Requires-Dist: prompt_toolkit<4.0.0,>=2.0.6
-Requires-Dist: psycopg>=3.0.14
-Requires-Dist: sqlparse<0.5,>=0.3.0
+Requires-Dist: psycopg>=3.0.14; sys_platform != "win32"
+Requires-Dist: psycopg-binary>=3.0.14; sys_platform == "win32"
+Requires-Dist: sqlparse<0.6,>=0.3.0
 Requires-Dist: configobj>=5.0.6
-Requires-Dist: pendulum>=2.1.0
 Requires-Dist: cli_helpers[styles]>=2.2.1
 Requires-Dist: setproctitle>=1.1.9
 Provides-Extra: keyring
 Requires-Dist: keyring>=12.2.0; extra == "keyring"
 Provides-Extra: sshtunnel
 Requires-Dist: sshtunnel>=0.4.0; extra == "sshtunnel"
```

### Comparing `pgcli-4.0.1/README.rst` & `pgcli-4.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `pgcli-4.0.1/changelog.rst` & `pgcli-4.1.0/changelog.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,38 @@
+4.1.0 (2024-03-09)
 ==================
-4.0.1 (2023-11-30)
+
+Features:
+---------
+* Support `PGAPPNAME` as an environment variable and `--application-name` as a command line argument.
+* Add `verbose_errors` config and `\v` special command which enable the
+  displaying of all Postgres error fields received.
+* Show Postgres notifications.
+* Support sqlparse 0.5.x
+* Add `--log-file [filename]` cli argument and `\log-file [filename]` special commands to
+  log to an external file in addition to the normal output
+
+Bug fixes:
+----------
+
+* Fix display of "short host" in prompt (with `\h`) for IPv4 addresses ([issue 964](https://github.com/dbcli/pgcli/issues/964)).
+* Fix backwards display of NOTICEs from a Function ([issue 1443](https://github.com/dbcli/pgcli/issues/1443))
+* Fix psycopg errors when installing on Windows.  ([issue 1413](https://https://github.com/dbcli/pgcli/issues/1413))
+* Use a home-made function to display query duration instead of relying on a third-party library (the general behaviour does not change), which fixes the installation of `pgcli` on 32-bit architectures ([issue 1451](https://github.com/dbcli/pgcli/issues/1451))
+
+==================
+4.0.1 (2023-10-30)
 ==================
 
 Internal:
 ---------
 * Allow stable version of pendulum.
 
 ==================
-4.0.0 (2023-11-27)
+4.0.0 (2023-10-27)
 ==================
 
 Features:
 ---------
 
 * Ask for confirmation when quitting cli while a transaction is ongoing.
 * New `destructive_statements_require_transaction` config option to refuse to execute a
```

### Comparing `pgcli-4.0.1/pgcli/auth.py` & `pgcli-4.1.0/pgcli/auth.py`

 * *Files identical despite different names*

### Comparing `pgcli-4.0.1/pgcli/completion_refresher.py` & `pgcli-4.1.0/pgcli/completion_refresher.py`

 * *Files identical despite different names*

### Comparing `pgcli-4.0.1/pgcli/config.py` & `pgcli-4.1.0/pgcli/config.py`

 * *Files identical despite different names*

### Comparing `pgcli-4.0.1/pgcli/explain_output_formatter.py` & `pgcli-4.1.0/pgcli/explain_output_formatter.py`

 * *Files identical despite different names*

### Comparing `pgcli-4.0.1/pgcli/key_bindings.py` & `pgcli-4.1.0/pgcli/key_bindings.py`

 * *Files identical despite different names*

### Comparing `pgcli-4.0.1/pgcli/magic.py` & `pgcli-4.1.0/pgcli/magic.py`

 * *Files identical despite different names*

### Comparing `pgcli-4.0.1/pgcli/main.py` & `pgcli-4.1.0/pgcli/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 import re
 import sys
 import traceback
 import logging
 import threading
 import shutil
 import functools
-import pendulum
 import datetime as dt
 import itertools
+import pathlib
 import platform
 from time import time, sleep
 from typing import Optional
 
 from cli_helpers.tabular_output import TabularOutputFormatter
 from cli_helpers.tabular_output.preprocessors import align_decimals, format_numbers
 from cli_helpers.utils import strip_ansi
@@ -70,16 +70,17 @@
 
 click.disable_unicode_literals_warning = True
 
 from urllib.parse import urlparse
 
 from getpass import getuser
 
-from psycopg import OperationalError, InterfaceError
+from psycopg import OperationalError, InterfaceError, Notify
 from psycopg.conninfo import make_conninfo, conninfo_to_dict
+from psycopg.errors import Diagnostic
 
 from collections import namedtuple
 
 try:
     import sshtunnel
 
     SSH_TUNNEL_SUPPORT = True
@@ -125,14 +126,23 @@
 )
 
 
 class PgCliQuitError(Exception):
     pass
 
 
+def notify_callback(notify: Notify):
+    click.secho(
+        'Notification received on channel "{}" (PID {}):\n{}'.format(
+            notify.channel, notify.pid, notify.payload
+        ),
+        fg="green",
+    )
+
+
 class PGCli:
     default_prompt = "\\u@\\h:\\d> "
     max_len_prompt = 30
 
     def set_default_pager(self, config):
         configured_pager = config["main"].get("pager")
         os_environ_pager = os.environ.get("PAGER")
@@ -161,21 +171,23 @@
     def __init__(
         self,
         force_passwd_prompt=False,
         never_passwd_prompt=False,
         pgexecute=None,
         pgclirc_file=None,
         row_limit=None,
+        application_name="pgcli",
         single_connection=False,
         less_chatty=None,
         prompt=None,
         prompt_dsn=None,
         auto_vertical_output=False,
         warn=None,
         ssh_tunnel_url: Optional[str] = None,
+        log_file: Optional[str] = None,
     ):
         self.force_passwd_prompt = force_passwd_prompt
         self.never_passwd_prompt = never_passwd_prompt
         self.pgexecute = pgexecute
         self.dsn_alias = None
         self.watch_command = None
 
@@ -206,14 +218,16 @@
         self.expanded_output = c["main"].as_bool("expand")
         self.pgspecial.timing_enabled = c["main"].as_bool("timing")
         if row_limit is not None:
             self.row_limit = row_limit
         else:
             self.row_limit = c["main"].as_int("row_limit")
 
+        self.application_name = application_name
+
         # if not specified, set to DEFAULT_MAX_FIELD_WIDTH
         # if specified but empty, set to None to disable truncation
         # ellipsis will take at least 3 symbols, so this can't be less than 3 if specified and > 0
         max_field_width = c["main"].get("max_field_width", DEFAULT_MAX_FIELD_WIDTH)
         if max_field_width and max_field_width.lower() != "none":
             max_field_width = max(3, abs(int(max_field_width)))
         else:
@@ -233,14 +247,17 @@
             "destructive_warning_restarts_connection"
         )
         self.destructive_statements_require_transaction = c["main"].as_bool(
             "destructive_statements_require_transaction"
         )
 
         self.less_chatty = bool(less_chatty) or c["main"].as_bool("less_chatty")
+        self.verbose_errors = "verbose_errors" in c["main"] and c["main"].as_bool(
+            "verbose_errors"
+        )
         self.null_string = c["main"].get("null_string", "<null>")
         self.prompt_format = (
             prompt
             if prompt is not None
             else c["main"].get("prompt", self.default_prompt)
         )
         self.prompt_dsn_format = prompt_dsn
@@ -291,14 +308,19 @@
 
         self.prompt_app = None
 
         self.ssh_tunnel_config = c.get("ssh tunnels")
         self.ssh_tunnel_url = ssh_tunnel_url
         self.ssh_tunnel = None
 
+        if log_file:
+            with open(log_file, "a+"):
+                pass  # ensure writeable
+        self.log_file = log_file
+
         # formatter setup
         self.formatter = TabularOutputFormatter(format_name=c["main"]["table_format"])
         register_new_formatter(self.formatter)
 
     def quit(self):
         raise PgCliQuitError
 
@@ -351,14 +373,20 @@
         self.pgspecial.register(
             self.write_to_file,
             "\\o",
             "\\o [filename]",
             "Send all query results to file.",
         )
         self.pgspecial.register(
+            self.write_to_logfile,
+            "\\log-file",
+            "\\log-file [filename]",
+            "Log all query results to a logfile, in addition to the normal output destination.",
+        )
+        self.pgspecial.register(
             self.info_connection, "\\conninfo", "\\conninfo", "Get connection details"
         )
         self.pgspecial.register(
             self.change_table_format,
             "\\T",
             "\\T [format]",
             "Change the table format used to output results",
@@ -374,14 +402,34 @@
         self.pgspecial.register(
             self.echo,
             "\\qecho",
             "\\qecho [string]",
             "Echo a string to the query output channel.",
         )
 
+        self.pgspecial.register(
+            self.toggle_verbose_errors,
+            "\\v",
+            "\\v [on|off]",
+            "Toggle verbose errors.",
+        )
+
+    def toggle_verbose_errors(self, pattern, **_):
+        flag = pattern.strip()
+
+        if flag == "on":
+            self.verbose_errors = True
+        elif flag == "off":
+            self.verbose_errors = False
+        else:
+            self.verbose_errors = not self.verbose_errors
+
+        message = "Verbose errors " + "on." if self.verbose_errors else "off."
+        return [(None, None, None, message)]
+
     def echo(self, pattern, **_):
         return [(None, None, None, pattern)]
 
     def change_table_format(self, pattern, **_):
         try:
             if pattern not in TabularOutputFormatter().supported_formats:
                 raise ValueError()
@@ -469,14 +517,34 @@
         return self.pgexecute.run(
             query,
             self.pgspecial,
             on_error_resume=on_error_resume,
             explain_mode=self.explain_mode,
         )
 
+    def write_to_logfile(self, pattern, **_):
+        if not pattern:
+            self.log_file = None
+            message = "Logfile capture disabled"
+            return [(None, None, None, message, "", True, True)]
+
+        log_file = pathlib.Path(pattern).expanduser().absolute()
+
+        try:
+            with open(log_file, "a+"):
+                pass  # ensure writeable
+        except OSError as e:
+            self.log_file = None
+            message = str(e) + "\nLogfile capture disabled"
+            return [(None, None, None, message, "", False, True)]
+
+        self.log_file = str(log_file)
+        message = 'Writing to file "%s"' % self.log_file
+        return [(None, None, None, message, "", True, True)]
+
     def write_to_file(self, pattern, **_):
         if not pattern:
             self.output_file = None
             message = "File output disabled"
             return [(None, None, None, message, "", True, True)]
         filename = os.path.abspath(os.path.expanduser(pattern))
         if not os.path.isfile(filename):
@@ -564,15 +632,15 @@
 
         if not user:
             user = getuser()
 
         if not database:
             database = user
 
-        kwargs.setdefault("application_name", "pgcli")
+        kwargs.setdefault("application_name", self.application_name)
 
         # If password prompt is not forced but no password is provided, try
         # getting it from environment variable.
         if not self.force_passwd_prompt and not passwd:
             passwd = os.environ.get("PGPASSWORD", "")
 
         # Prompt for a password immediately if requested via the -W flag. This
@@ -654,25 +722,41 @@
 
         # Attempt to connect to the database.
         # Note that passwd may be empty on the first attempt. If connection
         # fails because of a missing or incorrect password, but we're allowed to
         # prompt for a password (no -w flag), prompt for a passwd and try again.
         try:
             try:
-                pgexecute = PGExecute(database, user, passwd, host, port, dsn, **kwargs)
+                pgexecute = PGExecute(
+                    database,
+                    user,
+                    passwd,
+                    host,
+                    port,
+                    dsn,
+                    notify_callback,
+                    **kwargs,
+                )
             except (OperationalError, InterfaceError) as e:
                 if should_ask_for_password(e):
                     passwd = click.prompt(
                         "Password for %s" % user,
                         hide_input=True,
                         show_default=False,
                         type=str,
                     )
                     pgexecute = PGExecute(
-                        database, user, passwd, host, port, dsn, **kwargs
+                        database,
+                        user,
+                        passwd,
+                        host,
+                        port,
+                        dsn,
+                        notify_callback,
+                        **kwargs,
                     )
                 else:
                     raise e
             if passwd and auth.keyring:
                 auth.keyring_set_password(key, passwd)
 
         except Exception as e:  # Connecting to a database could fail.
@@ -771,39 +855,56 @@
         except Exception as e:
             logger.error("sql: %r, error: %r", text, e)
             logger.error("traceback: %r", traceback.format_exc())
             click.secho(str(e), err=True, fg="red")
         else:
             try:
                 if self.output_file and not text.startswith(
-                    ("\\o ", "\\? ", "\\echo ")
+                    ("\\o ", "\\log-file", "\\? ", "\\echo ")
                 ):
                     try:
                         with open(self.output_file, "a", encoding="utf-8") as f:
                             click.echo(text, file=f)
                             click.echo("\n".join(output), file=f)
                             click.echo("", file=f)  # extra newline
                     except OSError as e:
                         click.secho(str(e), err=True, fg="red")
                 else:
                     if output:
                         self.echo_via_pager("\n".join(output))
+
+                # Log to file in addition to normal output
+                if (
+                    self.log_file
+                    and not text.startswith(("\\o ", "\\log-file", "\\? ", "\\echo "))
+                    and not text.strip() == ""
+                ):
+                    try:
+                        with open(self.log_file, "a", encoding="utf-8") as f:
+                            click.echo(
+                                dt.datetime.now().isoformat(), file=f
+                            )  # timestamp log
+                            click.echo(text, file=f)
+                            click.echo("\n".join(output), file=f)
+                            click.echo("", file=f)  # extra newline
+                    except OSError as e:
+                        click.secho(str(e), err=True, fg="red")
             except KeyboardInterrupt:
                 pass
 
             if self.pgspecial.timing_enabled:
                 # Only add humanized time display if > 1 second
                 if query.total_time > 1:
                     print(
                         "Time: %0.03fs (%s), executed in: %0.03fs (%s)"
                         % (
                             query.total_time,
-                            pendulum.Duration(seconds=query.total_time).in_words(),
+                            duration_in_words(query.total_time),
                             query.execution_time,
-                            pendulum.Duration(seconds=query.execution_time).in_words(),
+                            duration_in_words(query.execution_time),
                         )
                     )
                 else:
                     print("Time: %0.03fs" % query.total_time)
 
             # Check if we need to update completions, in order of most
             # to least drastic changes
@@ -1049,15 +1150,15 @@
 
         # Run the query.
         start = time()
         on_error_resume = self.on_error == "RESUME"
         res = self.pgexecute.run(
             text,
             self.pgspecial,
-            exception_formatter,
+            lambda x: exception_formatter(x, self.verbose_errors),
             on_error_resume,
             explain_mode=self.explain_mode,
         )
 
         is_special = None
 
         for title, cur, headers, status, sql, success, is_special in res:
@@ -1334,14 +1435,20 @@
     "--row-limit",
     default=None,
     envvar="PGROWLIMIT",
     type=click.INT,
     help="Set threshold for row limit prompt. Use 0 to disable prompt.",
 )
 @click.option(
+    "--application-name",
+    default="pgcli",
+    envvar="PGAPPNAME",
+    help="Application name for the connection.",
+)
+@click.option(
     "--less-chatty",
     "less_chatty",
     is_flag=True,
     default=False,
     help="Skip intro on startup and goodbye on exit.",
 )
 @click.option("--prompt", help='Prompt format (Default: "\\u@\\h:\\d> ").')
@@ -1367,14 +1474,19 @@
     help="Warn before running a destructive query.",
 )
 @click.option(
     "--ssh-tunnel",
     default=None,
     help="Open an SSH tunnel to the given address and connect to the database from it.",
 )
+@click.option(
+    "--log-file",
+    default=None,
+    help="Write all queries & output into a file, in addition to the normal output destination.",
+)
 @click.argument("dbname", default=lambda: None, envvar="PGDATABASE", nargs=1)
 @click.argument("username", default=lambda: None, envvar="PGUSER", nargs=1)
 def cli(
     dbname,
     username_opt,
     host,
     port,
@@ -1383,22 +1495,24 @@
     single_connection,
     dbname_opt,
     username,
     version,
     pgclirc,
     dsn,
     row_limit,
+    application_name,
     less_chatty,
     prompt,
     prompt_dsn,
     list_databases,
     auto_vertical_output,
     list_dsn,
     warn,
     ssh_tunnel: str,
+    log_file: str,
 ):
     if version:
         print("Version:", __version__)
         sys.exit(0)
 
     config_dir = os.path.dirname(config_location())
     if not os.path.exists(config_dir):
@@ -1441,21 +1555,23 @@
         exit(1)
 
     pgcli = PGCli(
         prompt_passwd,
         never_prompt,
         pgclirc_file=pgclirc,
         row_limit=row_limit,
+        application_name=application_name,
         single_connection=single_connection,
         less_chatty=less_chatty,
         prompt=prompt,
         prompt_dsn=prompt_dsn,
         auto_vertical_output=auto_vertical_output,
         warn=warn,
         ssh_tunnel_url=ssh_tunnel,
+        log_file=log_file,
     )
 
     # Choose which ever one has a valid value.
     if dbname_opt and dbname:
         # work as psql: when database is given as option and argument use the argument as user
         username = dbname
     database = dbname_opt or dbname or ""
@@ -1579,16 +1695,79 @@
 def is_select(status):
     """Returns true if the first word in status is 'select'."""
     if not status:
         return False
     return status.split(None, 1)[0].lower() == "select"
 
 
-def exception_formatter(e):
-    return click.style(str(e), fg="red")
+def diagnostic_output(diagnostic: Diagnostic) -> str:
+    fields = []
+
+    if diagnostic.severity is not None:
+        fields.append("Severity: " + diagnostic.severity)
+
+    if diagnostic.severity_nonlocalized is not None:
+        fields.append("Severity (non-localized): " + diagnostic.severity_nonlocalized)
+
+    if diagnostic.sqlstate is not None:
+        fields.append("SQLSTATE code: " + diagnostic.sqlstate)
+
+    if diagnostic.message_primary is not None:
+        fields.append("Message: " + diagnostic.message_primary)
+
+    if diagnostic.message_detail is not None:
+        fields.append("Detail: " + diagnostic.message_detail)
+
+    if diagnostic.message_hint is not None:
+        fields.append("Hint: " + diagnostic.message_hint)
+
+    if diagnostic.statement_position is not None:
+        fields.append("Position: " + diagnostic.statement_position)
+
+    if diagnostic.internal_position is not None:
+        fields.append("Internal position: " + diagnostic.internal_position)
+
+    if diagnostic.internal_query is not None:
+        fields.append("Internal query: " + diagnostic.internal_query)
+
+    if diagnostic.context is not None:
+        fields.append("Where: " + diagnostic.context)
+
+    if diagnostic.schema_name is not None:
+        fields.append("Schema name: " + diagnostic.schema_name)
+
+    if diagnostic.table_name is not None:
+        fields.append("Table name: " + diagnostic.table_name)
+
+    if diagnostic.column_name is not None:
+        fields.append("Column name: " + diagnostic.column_name)
+
+    if diagnostic.datatype_name is not None:
+        fields.append("Data type name: " + diagnostic.datatype_name)
+
+    if diagnostic.constraint_name is not None:
+        fields.append("Constraint name: " + diagnostic.constraint_name)
+
+    if diagnostic.source_file is not None:
+        fields.append("File: " + diagnostic.source_file)
+
+    if diagnostic.source_line is not None:
+        fields.append("Line: " + diagnostic.source_line)
+
+    if diagnostic.source_function is not None:
+        fields.append("Routine: " + diagnostic.source_function)
+
+    return "\n".join(fields)
+
+
+def exception_formatter(e, verbose_errors: bool = False):
+    s = str(e)
+    if verbose_errors:
+        s += "\n" + diagnostic_output(e.diag)
+    return click.style(s, fg="red")
 
 
 def format_output(title, cur, headers, status, settings, explain_mode=False):
     output = []
     expanded = settings.expanded or settings.table_format == "vertical"
     table_format = "vertical" if settings.expanded else settings.table_format
     max_width = settings.max_width
@@ -1720,9 +1899,32 @@
             raise err
     if service not in service_file_config:
         return None, service_file
     service_conf = service_file_config.get(service)
     return service_conf, service_file
 
 
+def duration_in_words(duration_in_seconds: float) -> str:
+    if not duration_in_seconds:
+        return "0 seconds"
+    components = []
+    hours, remainder = divmod(duration_in_seconds, 3600)
+    if hours > 1:
+        components.append(f"{hours} hours")
+    elif hours == 1:
+        components.append("1 hour")
+    minutes, seconds = divmod(remainder, 60)
+    if minutes > 1:
+        components.append(f"{minutes} minutes")
+    elif minutes == 1:
+        components.append("1 minute")
+    if seconds >= 2:
+        components.append(f"{int(seconds)} seconds")
+    elif seconds >= 1:
+        components.append("1 second")
+    elif seconds:
+        components.append(f"{round(seconds, 3)} second")
+    return " ".join(components)
+
+
 if __name__ == "__main__":
     cli()
```

### Comparing `pgcli-4.0.1/pgcli/packages/formatter/sqlformatter.py` & `pgcli-4.1.0/pgcli/packages/formatter/sqlformatter.py`

 * *Files identical despite different names*

### Comparing `pgcli-4.0.1/pgcli/packages/parseutils/__init__.py` & `pgcli-4.1.0/pgcli/packages/parseutils/__init__.py`

 * *Files identical despite different names*

### Comparing `pgcli-4.0.1/pgcli/packages/parseutils/ctes.py` & `pgcli-4.1.0/pgcli/packages/parseutils/ctes.py`

 * *Files identical despite different names*

### Comparing `pgcli-4.0.1/pgcli/packages/parseutils/meta.py` & `pgcli-4.1.0/pgcli/packages/parseutils/meta.py`

 * *Files identical despite different names*

### Comparing `pgcli-4.0.1/pgcli/packages/parseutils/tables.py` & `pgcli-4.1.0/pgcli/packages/parseutils/tables.py`

 * *Files identical despite different names*

### Comparing `pgcli-4.0.1/pgcli/packages/parseutils/utils.py` & `pgcli-4.1.0/pgcli/packages/parseutils/utils.py`

 * *Files identical despite different names*

### Comparing `pgcli-4.0.1/pgcli/packages/pgliterals/pgliterals.json` & `pgcli-4.1.0/pgcli/packages/pgliterals/pgliterals.json`

 * *Files identical despite different names*

### Comparing `pgcli-4.0.1/pgcli/packages/prioritization.py` & `pgcli-4.1.0/pgcli/packages/prioritization.py`

 * *Files identical despite different names*

### Comparing `pgcli-4.0.1/pgcli/packages/prompt_utils.py` & `pgcli-4.1.0/pgcli/packages/prompt_utils.py`

 * *Files identical despite different names*

### Comparing `pgcli-4.0.1/pgcli/packages/sqlcompletion.py` & `pgcli-4.1.0/pgcli/packages/sqlcompletion.py`

 * *Files identical despite different names*

### Comparing `pgcli-4.0.1/pgcli/pgbuffer.py` & `pgcli-4.1.0/pgcli/pgbuffer.py`

 * *Files identical despite different names*

### Comparing `pgcli-4.0.1/pgcli/pgclirc` & `pgcli-4.1.0/pgcli/pgclirc`

 * *Files 2% similar despite different names*

```diff
@@ -29,18 +29,19 @@
 # Destructive warning will alert you before executing a sql statement
 # that may cause harm to the database such as "drop table", "drop database",
 # "shutdown", "delete", or "update".
 # You can pass a list of destructive commands or leave it empty if you want to skip all warnings.
 # "unconditional_update" will warn you of update statements that don't have a where clause
 destructive_warning = drop, shutdown, delete, truncate, alter, update, unconditional_update
 
-# Destructive warning can restart the connection if this is enabled and the
-# user declines. This means that any current uncommitted transaction can be
-# aborted if the user doesn't want to proceed with a destructive_warning
-# statement.
+# When `destructive_warning` is on and the user declines to proceed with a
+# destructive statement, the current transaction (if any) is left untouched,
+# by default. When setting `destructive_warning_restarts_connection` to
+# "True", the connection to the server is restarted. In that case, the
+# transaction (if any) is rolled back.
 destructive_warning_restarts_connection = False
 
 # When this option is on (and if `destructive_warning` is not empty),
 # destructive statements are not executed when outside of a transaction.
 destructive_statements_require_transaction = False
 
 # Enables expand mode, which is similar to `\x` in psql.
@@ -151,14 +152,19 @@
 # Be aware that formatting might get slow with values larger than 500 and tables with
 # lots of records.
 max_field_width = 500
 
 # Skip intro on startup and goodbye on exit
 less_chatty = False
 
+# Show all Postgres error fields (as listed in
+# https://www.postgresql.org/docs/current/protocol-error-fields.html).
+# Can be toggled with \v.
+verbose_errors = False
+
 # Postgres prompt
 # \t - Current date and time
 # \u - Username
 # \h - Short hostname of the server (up to first '.')
 # \H - Hostname of the server
 # \d - Database name
 # \p - Database port
```

### Comparing `pgcli-4.0.1/pgcli/pgcompleter.py` & `pgcli-4.1.0/pgcli/pgcompleter.py`

 * *Files identical despite different names*

### Comparing `pgcli-4.0.1/pgcli/pgexecute.py` & `pgcli-4.1.0/pgcli/pgexecute.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import ipaddress
 import logging
 import traceback
 from collections import namedtuple
 import re
 import pgspecial as special
 import psycopg
 import psycopg.sql
@@ -162,26 +163,28 @@
         self,
         database=None,
         user=None,
         password=None,
         host=None,
         port=None,
         dsn=None,
+        notify_callback=None,
         **kwargs,
     ):
         self._conn_params = {}
         self._is_virtual_database = None
         self.conn = None
         self.dbname = None
         self.user = None
         self.password = None
         self.host = None
         self.port = None
         self.server_version = None
         self.extra_args = None
+        self.notify_callback = notify_callback
         self.connect(database, user, password, host, port, dsn, **kwargs)
         self.reset_expanded = None
 
     def is_virtual_database(self):
         if self._is_virtual_database is None:
             self._is_virtual_database = self.is_protocol_error()
         return self._is_virtual_database
@@ -232,14 +235,17 @@
 
         self._conn_params = conn_params
         if self.conn:
             self.conn.close()
         self.conn = conn
         self.conn.autocommit = True
 
+        if self.notify_callback is not None:
+            self.conn.add_notify_handler(self.notify_callback)
+
         # When we connect using a DSN, we don't really know what db,
         # user, etc. we connected to. Let's read it.
         # Note: moved this after setting autocommit because of #664.
         dsn_parameters = conn.info.get_parameters()
 
         if dsn_parameters:
             self.dbname = dsn_parameters.get("dbname")
@@ -269,14 +275,19 @@
         # _set_wait_callback(self.is_virtual_database())
 
         if not self.is_virtual_database():
             register_typecasters(conn)
 
     @property
     def short_host(self):
+        try:
+            ipaddress.ip_address(self.host)
+            return self.host
+        except ValueError:
+            pass
         if "," in self.host:
             host, _, _ = self.host.partition(",")
         else:
             host = self.host
         short_host, _, _ = host.partition(".")
         return short_host
 
@@ -427,15 +438,19 @@
         """Returns tuple (title, rows, headers, status)"""
         _logger.debug("Regular sql statement. sql: %r", split_sql)
 
         title = ""
 
         def handle_notices(n):
             nonlocal title
-            title = f"{n.message_primary}\n{n.message_detail}\n{title}"
+            title = f"{title}"
+            if n.message_primary is not None:
+                title = f"{title}\n{n.message_primary}"
+            if n.message_detail is not None:
+                title = f"{title}\n{n.message_detail}"
 
         self.conn.add_notice_handler(handle_notices)
 
         if self.is_virtual_database() and "show help" in split_sql.lower():
             # see https://github.com/psycopg/psycopg/issues/303
             # special case "show help" in pgbouncer
             res = self.conn.pgconn.exec_(split_sql.encode())
```

### Comparing `pgcli-4.0.1/pgcli/pgstyle.py` & `pgcli-4.1.0/pgcli/pgstyle.py`

 * *Files identical despite different names*

### Comparing `pgcli-4.0.1/pgcli/pgtoolbar.py` & `pgcli-4.1.0/pgcli/pgtoolbar.py`

 * *Files identical despite different names*

### Comparing `pgcli-4.0.1/pgcli/pyev.py` & `pgcli-4.1.0/pgcli/pyev.py`

 * *Files identical despite different names*

### Comparing `pgcli-4.0.1/pgcli.egg-info/PKG-INFO` & `pgcli-4.1.0/pgcli.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pgcli
-Version: 4.0.1
+Version: 4.1.0
 Summary: CLI for Postgres Database. With auto-completion and syntax highlighting.
 Home-page: http://pgcli.com
 Author: Pgcli Core Team
 Author-email: pgcli-dev@googlegroups.com
 License: BSD
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
@@ -24,18 +24,18 @@
 Requires-Python: >=3.8
 License-File: LICENSE.txt
 License-File: AUTHORS
 Requires-Dist: pgspecial>=2.0.0
 Requires-Dist: click>=4.1
 Requires-Dist: Pygments>=2.0
 Requires-Dist: prompt_toolkit<4.0.0,>=2.0.6
-Requires-Dist: psycopg>=3.0.14
-Requires-Dist: sqlparse<0.5,>=0.3.0
+Requires-Dist: psycopg>=3.0.14; sys_platform != "win32"
+Requires-Dist: psycopg-binary>=3.0.14; sys_platform == "win32"
+Requires-Dist: sqlparse<0.6,>=0.3.0
 Requires-Dist: configobj>=5.0.6
-Requires-Dist: pendulum>=2.1.0
 Requires-Dist: cli_helpers[styles]>=2.2.1
 Requires-Dist: setproctitle>=1.1.9
 Provides-Extra: keyring
 Requires-Dist: keyring>=12.2.0; extra == "keyring"
 Provides-Extra: sshtunnel
 Requires-Dist: sshtunnel>=0.4.0; extra == "sshtunnel"
```

### Comparing `pgcli-4.0.1/pgcli.egg-info/SOURCES.txt` & `pgcli-4.1.0/pgcli.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 pgcli/packages/parseutils/utils.py
 pgcli/packages/pgliterals/__init__.py
 pgcli/packages/pgliterals/main.py
 pgcli/packages/pgliterals/pgliterals.json
 tests/conftest.py
 tests/metadata.py
 tests/pytest.ini
+tests/test_application_name.py
 tests/test_auth.py
 tests/test_completion_refresher.py
 tests/test_config.py
 tests/test_fuzzy_completion.py
 tests/test_main.py
 tests/test_naive_completion.py
 tests/test_pgcompleter.py
```

### Comparing `pgcli-4.0.1/setup.py` & `pgcli-4.1.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,34 +8,29 @@
 install_requirements = [
     "pgspecial>=2.0.0",
     "click >= 4.1",
     "Pygments>=2.0",  # Pygments has to be Capitalcased. WTF?
     # We still need to use pt-2 unless pt-3 released on Fedora32
     # see: https://github.com/dbcli/pgcli/pull/1197
     "prompt_toolkit>=2.0.6,<4.0.0",
-    "psycopg >= 3.0.14",
-    "sqlparse >=0.3.0,<0.5",
+    "psycopg >= 3.0.14; sys_platform != 'win32'",
+    "psycopg-binary >= 3.0.14; sys_platform == 'win32'",
+    "sqlparse >=0.3.0,<0.6",
     "configobj >= 5.0.6",
-    "pendulum>=2.1.0",
     "cli_helpers[styles] >= 2.2.1",
 ]
 
 
 # setproctitle is used to mask the password when running `ps` in command line.
 # But this is not necessary in Windows since the password is never shown in the
 # task manager. Also setproctitle is a hard dependency to install in Windows,
 # so we'll only install it if we're not in Windows.
 if platform.system() != "Windows" and not platform.system().startswith("CYGWIN"):
     install_requirements.append("setproctitle >= 1.1.9")
 
-# Windows will require the binary psycopg to run pgcli
-if platform.system() == "Windows":
-    install_requirements.append("psycopg-binary >= 3.0.14")
-
-
 setup(
     name="pgcli",
     author="Pgcli Core Team",
     author_email="pgcli-dev@googlegroups.com",
     version=__version__,
     license="BSD",
     url="http://pgcli.com",
```

### Comparing `pgcli-4.0.1/tests/conftest.py` & `pgcli-4.1.0/tests/conftest.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,14 +5,15 @@
     POSTGRES_PORT,
     POSTGRES_USER,
     POSTGRES_PASSWORD,
     create_db,
     db_connection,
     drop_tables,
 )
+import pgcli.main
 import pgcli.pgexecute
 
 
 @pytest.fixture(scope="function")
 def connection():
     create_db("_test_db")
     connection = db_connection("_test_db")
@@ -33,14 +34,15 @@
     return pgcli.pgexecute.PGExecute(
         database="_test_db",
         user=POSTGRES_USER,
         host=POSTGRES_HOST,
         password=POSTGRES_PASSWORD,
         port=POSTGRES_PORT,
         dsn=None,
+        notify_callback=pgcli.main.notify_callback,
     )
 
 
 @pytest.fixture
 def exception_formatter():
     return lambda e: str(e)
```

### Comparing `pgcli-4.0.1/tests/features/basic_commands.feature` & `pgcli-4.1.0/tests/features/basic_commands.feature`

 * *Files identical despite different names*

### Comparing `pgcli-4.0.1/tests/features/crud_database.feature` & `pgcli-4.1.0/tests/features/crud_database.feature`

 * *Files identical despite different names*

### Comparing `pgcli-4.0.1/tests/features/crud_table.feature` & `pgcli-4.1.0/tests/features/crud_table.feature`

 * *Files identical despite different names*

### Comparing `pgcli-4.0.1/tests/features/db_utils.py` & `pgcli-4.1.0/tests/features/db_utils.py`

 * *Files identical despite different names*

### Comparing `pgcli-4.0.1/tests/features/environment.py` & `pgcli-4.1.0/tests/features/environment.py`

 * *Files identical despite different names*

### Comparing `pgcli-4.0.1/tests/features/expanded.feature` & `pgcli-4.1.0/tests/features/expanded.feature`

 * *Files identical despite different names*

### Comparing `pgcli-4.0.1/tests/features/fixture_data/help.txt` & `pgcli-4.1.0/tests/features/fixture_data/help.txt`

 * *Files identical despite different names*

### Comparing `pgcli-4.0.1/tests/features/fixture_data/help_commands.txt` & `pgcli-4.1.0/tests/features/fixture_data/help_commands.txt`

 * *Files identical despite different names*

### Comparing `pgcli-4.0.1/tests/features/fixture_utils.py` & `pgcli-4.1.0/tests/features/fixture_utils.py`

 * *Files identical despite different names*

### Comparing `pgcli-4.0.1/tests/features/iocommands.feature` & `pgcli-4.1.0/tests/features/iocommands.feature`

 * *Files identical despite different names*

### Comparing `pgcli-4.0.1/tests/features/steps/auto_vertical.py` & `pgcli-4.1.0/tests/features/steps/auto_vertical.py`

 * *Files identical despite different names*

### Comparing `pgcli-4.0.1/tests/features/steps/basic_commands.py` & `pgcli-4.1.0/tests/features/steps/basic_commands.py`

 * *Files identical despite different names*

### Comparing `pgcli-4.0.1/tests/features/steps/crud_database.py` & `pgcli-4.1.0/tests/features/steps/crud_database.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Steps for behavioral style tests are defined in this module.
 Each step is defined by the string decorating it.
 This string is used to call the step in "*.feature" file.
 """
+
 import pexpect
 
 from behave import when, then
 import wrappers
 
 
 @when("we create database")
```

### Comparing `pgcli-4.0.1/tests/features/steps/crud_table.py` & `pgcli-4.1.0/tests/features/steps/crud_table.py`

 * *Files identical despite different names*

### Comparing `pgcli-4.0.1/tests/features/steps/expanded.py` & `pgcli-4.1.0/tests/features/steps/expanded.py`

 * *Files identical despite different names*

### Comparing `pgcli-4.0.1/tests/features/steps/iocommands.py` & `pgcli-4.1.0/tests/features/steps/iocommands.py`

 * *Files identical despite different names*

### Comparing `pgcli-4.0.1/tests/features/steps/named_queries.py` & `pgcli-4.1.0/tests/features/steps/named_queries.py`

 * *Files identical despite different names*

### Comparing `pgcli-4.0.1/tests/features/steps/pgbouncer.py` & `pgcli-4.1.0/tests/features/steps/pgbouncer.py`

 * *Files identical despite different names*

### Comparing `pgcli-4.0.1/tests/features/steps/specials.py` & `pgcli-4.1.0/tests/features/steps/specials.py`

 * *Files identical despite different names*

### Comparing `pgcli-4.0.1/tests/features/steps/wrappers.py` & `pgcli-4.1.0/tests/features/steps/wrappers.py`

 * *Files identical despite different names*

### Comparing `pgcli-4.0.1/tests/formatter/test_sqlformatter.py` & `pgcli-4.1.0/tests/formatter/test_sqlformatter.py`

 * *Files identical despite different names*

### Comparing `pgcli-4.0.1/tests/metadata.py` & `pgcli-4.1.0/tests/metadata.py`

 * *Files identical despite different names*

### Comparing `pgcli-4.0.1/tests/parseutils/test_ctes.py` & `pgcli-4.1.0/tests/parseutils/test_ctes.py`

 * *Files identical despite different names*

### Comparing `pgcli-4.0.1/tests/parseutils/test_function_metadata.py` & `pgcli-4.1.0/tests/parseutils/test_function_metadata.py`

 * *Files identical despite different names*

### Comparing `pgcli-4.0.1/tests/parseutils/test_parseutils.py` & `pgcli-4.1.0/tests/parseutils/test_parseutils.py`

 * *Files identical despite different names*

### Comparing `pgcli-4.0.1/tests/test_auth.py` & `pgcli-4.1.0/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `pgcli-4.0.1/tests/test_completion_refresher.py` & `pgcli-4.1.0/tests/test_completion_refresher.py`

 * *Files identical despite different names*

### Comparing `pgcli-4.0.1/tests/test_config.py` & `pgcli-4.1.0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `pgcli-4.0.1/tests/test_fuzzy_completion.py` & `pgcli-4.1.0/tests/test_fuzzy_completion.py`

 * *Files identical despite different names*

### Comparing `pgcli-4.0.1/tests/test_main.py` & `pgcli-4.1.0/tests/test_main.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 import os
 import platform
+import re
+import tempfile
+import datetime
 from unittest import mock
 
 import pytest
 
 try:
     import setproctitle
 except ImportError:
     setproctitle = None
 
 from pgcli.main import (
     obfuscate_process_password,
+    duration_in_words,
     format_output,
+    notify_callback,
     PGCli,
     OutputSettings,
     COLOR_CODE_REGEX,
 )
 from pgcli.pgexecute import PGExecute
 from pgspecial.main import PAGER_OFF, PAGER_LONG_OUTPUT, PAGER_ALWAYS
 from utils import dbtest, run
@@ -293,14 +298,32 @@
     rcfile = str(tmpdir.join("rcfile"))
     cli = PGCli(pgexecute=executor, pgclirc_file=rcfile)
     statement = r"\i {0}".format(sqlfile)
     run(executor, statement, pgspecial=cli.pgspecial)
 
 
 @dbtest
+def test_toggle_verbose_errors(executor):
+    cli = PGCli(pgexecute=executor)
+
+    cli._evaluate_command("\\v on")
+    assert cli.verbose_errors
+    output, _ = cli._evaluate_command("SELECT 1/0")
+    assert "SQLSTATE" in output[0]
+
+    cli._evaluate_command("\\v off")
+    assert not cli.verbose_errors
+    output, _ = cli._evaluate_command("SELECT 1/0")
+    assert "SQLSTATE" not in output[0]
+
+    cli._evaluate_command("\\v")
+    assert cli.verbose_errors
+
+
+@dbtest
 def test_echo_works(executor):
     cli = PGCli(pgexecute=executor)
     statement = r"\echo asdf"
     result = run(executor, statement, pgspecial=cli.pgspecial)
     assert result == ["asdf"]
 
 
@@ -309,14 +332,42 @@
     cli = PGCli(pgexecute=executor)
     statement = r"\qecho asdf"
     result = run(executor, statement, pgspecial=cli.pgspecial)
     assert result == ["asdf"]
 
 
 @dbtest
+def test_logfile_works(executor):
+    with tempfile.TemporaryDirectory() as tmpdir:
+        log_file = f"{tmpdir}/tempfile.log"
+        cli = PGCli(pgexecute=executor, log_file=log_file)
+        statement = r"\qecho hello!"
+        cli.execute_command(statement)
+        with open(log_file, "r") as f:
+            log_contents = f.readlines()
+        assert datetime.datetime.fromisoformat(log_contents[0].strip())
+        assert log_contents[1].strip() == r"\qecho hello!"
+        assert log_contents[2].strip() == "hello!"
+
+
+@dbtest
+def test_logfile_unwriteable_file(executor):
+    cli = PGCli(pgexecute=executor)
+    statement = r"\log-file forbidden.log"
+    with mock.patch("builtins.open") as mock_open:
+        mock_open.side_effect = PermissionError(
+            "[Errno 13] Permission denied: 'forbidden.log'"
+        )
+        result = run(executor, statement, pgspecial=cli.pgspecial)
+    assert result == [
+        "[Errno 13] Permission denied: 'forbidden.log'\nLogfile capture disabled"
+    ]
+
+
+@dbtest
 def test_watch_works(executor):
     cli = PGCli(pgexecute=executor)
 
     def run_with_watch(
         query, target_call_count=1, expected_output="", expected_timing=None
     ):
         """
@@ -427,14 +478,15 @@
     mock_pgexecute.assert_called_with(
         "b_dbname",
         "b_user",
         "very_secure",
         "b_host",
         "5435",
         "",
+        notify_callback,
         application_name="pgcli",
     )
     del os.environ["PGPASSWORD"]
     del os.environ["PGSERVICEFILE"]
 
 
 def test_ssl_db_uri(tmpdir):
@@ -482,9 +534,54 @@
 
 def test_application_name_db_uri(tmpdir):
     with mock.patch.object(PGExecute, "__init__") as mock_pgexecute:
         mock_pgexecute.return_value = None
         cli = PGCli(pgclirc_file=str(tmpdir.join("rcfile")))
         cli.connect_uri("postgres://bar@baz.com/?application_name=cow")
     mock_pgexecute.assert_called_with(
-        "bar", "bar", "", "baz.com", "", "", application_name="cow"
+        "bar", "bar", "", "baz.com", "", "", notify_callback, application_name="cow"
     )
+
+
+@pytest.mark.parametrize(
+    "duration_in_seconds,words",
+    [
+        (0, "0 seconds"),
+        (0.0009, "0.001 second"),
+        (0.0005, "0.001 second"),
+        (0.0004, "0.0 second"),  # not perfect, but will do
+        (0.2, "0.2 second"),
+        (1, "1 second"),
+        (1.4, "1 second"),
+        (2, "2 seconds"),
+        (3.4, "3 seconds"),
+        (60, "1 minute"),
+        (61, "1 minute 1 second"),
+        (123, "2 minutes 3 seconds"),
+        (3600, "1 hour"),
+        (7235, "2 hours 35 seconds"),
+        (9005, "2 hours 30 minutes 5 seconds"),
+        (86401, "24 hours 1 second"),
+    ],
+)
+def test_duration_in_words(duration_in_seconds, words):
+    assert duration_in_words(duration_in_seconds) == words
+
+
+@dbtest
+def test_notifications(executor):
+    run(executor, "listen chan1")
+
+    with mock.patch("pgcli.main.click.secho") as mock_secho:
+        run(executor, "notify chan1, 'testing1'")
+        mock_secho.assert_called()
+        arg = mock_secho.call_args_list[0].args[0]
+    assert re.match(
+        r'Notification received on channel "chan1" \(PID \d+\):\ntesting1',
+        arg,
+    )
+
+    run(executor, "unlisten chan1")
+
+    with mock.patch("pgcli.main.click.secho") as mock_secho:
+        run(executor, "notify chan1, 'testing2'")
+        mock_secho.assert_not_called()
```

### Comparing `pgcli-4.0.1/tests/test_naive_completion.py` & `pgcli-4.1.0/tests/test_naive_completion.py`

 * *Files identical despite different names*

### Comparing `pgcli-4.0.1/tests/test_pgcompleter.py` & `pgcli-4.1.0/tests/test_pgcompleter.py`

 * *Files identical despite different names*

### Comparing `pgcli-4.0.1/tests/test_pgexecute.py` & `pgcli-4.1.0/tests/test_pgexecute.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,17 @@
+import re
 from textwrap import dedent
 
 import psycopg
 import pytest
 from unittest.mock import patch, MagicMock
 from pgspecial.main import PGSpecial, NO_QUERY
 from utils import run, dbtest, requires_json, requires_jsonb
 
-from pgcli.main import PGCli
+from pgcli.main import PGCli, exception_formatter as main_exception_formatter
 from pgcli.packages.parseutils.meta import FunctionMetadata
 
 
 def function_meta_data(
     func_name,
     schema_name="public",
     arg_names=None,
@@ -215,16 +216,41 @@
 def test_database_list(executor):
     databases = executor.databases()
     assert "_test_db" in databases
 
 
 @dbtest
 def test_invalid_syntax(executor, exception_formatter):
-    result = run(executor, "invalid syntax!", exception_formatter=exception_formatter)
+    result = run(
+        executor,
+        "invalid syntax!",
+        exception_formatter=lambda x: main_exception_formatter(x, verbose_errors=False),
+    )
     assert 'syntax error at or near "invalid"' in result[0]
+    assert "SQLSTATE" not in result[0]
+
+
+@dbtest
+def test_invalid_syntax_verbose(executor):
+    result = run(
+        executor,
+        "invalid syntax!",
+        exception_formatter=lambda x: main_exception_formatter(x, verbose_errors=True),
+    )
+    fields = r"""
+Severity: ERROR
+Severity \(non-localized\): ERROR
+SQLSTATE code: 42601
+Message: syntax error at or near "invalid"
+Position: 1
+File: scan\.l
+Line: \d+
+Routine: scanner_yyerror
+    """.strip()
+    assert re.search(fields, result[0])
 
 
 @dbtest
 def test_invalid_column_name(executor, exception_formatter):
     result = run(
         executor, "select invalid command", exception_formatter=exception_formatter
     )
@@ -687,14 +713,46 @@
             $function$
     """,
     )
     result = executor.function_definition("the_number_three")
 
 
 @dbtest
+def test_function_notice_order(executor):
+    run(
+        executor,
+        """
+        CREATE OR REPLACE FUNCTION demo_order() RETURNS VOID AS
+        $$
+        BEGIN
+            RAISE NOTICE 'first';
+            RAISE NOTICE 'second';
+            RAISE NOTICE 'third';
+            RAISE NOTICE 'fourth';
+            RAISE NOTICE 'fifth';
+            RAISE NOTICE 'sixth';
+        END;
+        $$
+        LANGUAGE plpgsql;
+    """,
+    )
+
+    executor.function_definition("demo_order")
+
+    result = run(executor, "select demo_order()")
+    assert "first\nsecond\nthird\nfourth\nfifth\nsixth" in result[0]
+    assert "+------------+" in result[1]
+    assert "| demo_order |" in result[2]
+    assert "|------------|" in result[3]
+    assert "|            |" in result[4]
+    assert "+------------+" in result[5]
+    assert "SELECT 1" in result[6]
+
+
+@dbtest
 def test_view_definition(executor):
     run(executor, "create table tbl1 (a text, b numeric)")
     run(executor, "create view vw1 AS SELECT * FROM tbl1")
     run(executor, "create materialized view mvw1 AS SELECT * FROM tbl1")
     result = executor.view_definition("vw1")
     assert 'VIEW "public"."vw1" AS' in result
     assert "FROM tbl1" in result
@@ -717,14 +775,18 @@
         assert executor.short_host == "localhost"
     with patch.object(executor, "host", "localhost.example.org"):
         assert executor.short_host == "localhost"
     with patch.object(
         executor, "host", "localhost1.example.org,localhost2.example.org"
     ):
         assert executor.short_host == "localhost1"
+    with patch.object(executor, "host", "ec2-11-222-333-444.compute-1.amazonaws.com"):
+        assert executor.short_host == "ec2-11-222-333-444"
+    with patch.object(executor, "host", "1.2.3.4"):
+        assert executor.short_host == "1.2.3.4"
 
 
 class VirtualCursor:
     """Mock a cursor to virtual database like pgbouncer."""
 
     def __init__(self):
         self.protocol_error = False
```

### Comparing `pgcli-4.0.1/tests/test_pgspecial.py` & `pgcli-4.1.0/tests/test_pgspecial.py`

 * *Files identical despite different names*

### Comparing `pgcli-4.0.1/tests/test_prioritization.py` & `pgcli-4.1.0/tests/test_prioritization.py`

 * *Files identical despite different names*

### Comparing `pgcli-4.0.1/tests/test_prompt_utils.py` & `pgcli-4.1.0/tests/test_prompt_utils.py`

 * *Files identical despite different names*

### Comparing `pgcli-4.0.1/tests/test_rowlimit.py` & `pgcli-4.1.0/tests/test_rowlimit.py`

 * *Files identical despite different names*

### Comparing `pgcli-4.0.1/tests/test_smart_completion_multiple_schemata.py` & `pgcli-4.1.0/tests/test_smart_completion_multiple_schemata.py`

 * *Files identical despite different names*

### Comparing `pgcli-4.0.1/tests/test_smart_completion_public_schema_only.py` & `pgcli-4.1.0/tests/test_smart_completion_public_schema_only.py`

 * *Files identical despite different names*

### Comparing `pgcli-4.0.1/tests/test_sqlcompletion.py` & `pgcli-4.1.0/tests/test_sqlcompletion.py`

 * *Files identical despite different names*

### Comparing `pgcli-4.0.1/tests/test_ssh_tunnel.py` & `pgcli-4.1.0/tests/test_ssh_tunnel.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from unittest.mock import patch, MagicMock, ANY
 
 import pytest
 from configobj import ConfigObj
 from click.testing import CliRunner
 from sshtunnel import SSHTunnelForwarder
 
-from pgcli.main import cli, PGCli
+from pgcli.main import cli, notify_callback, PGCli
 from pgcli.pgexecute import PGExecute
 
 
 @pytest.fixture
 def mock_ssh_tunnel_forwarder() -> MagicMock:
     mock_ssh_tunnel_forwarder = MagicMock(
         SSHTunnelForwarder, local_bind_ports=[1111], autospec=True
@@ -57,14 +57,15 @@
     assert call_args == (
         db_params["database"],
         db_params["user"],
         db_params["passwd"],
         "127.0.0.1",
         pgcli.ssh_tunnel.local_bind_ports[0],
         "",
+        notify_callback,
     )
     mock_ssh_tunnel_forwarder.reset_mock()
     mock_pgexecute.reset_mock()
 
     # Test with a full url and with a specific db port
     tunnel_user = "tunnel_user"
     tunnel_passwd = "tunnel_pass"
@@ -92,14 +93,15 @@
     assert call_args == (
         db_params["database"],
         db_params["user"],
         db_params["passwd"],
         "127.0.0.1",
         pgcli.ssh_tunnel.local_bind_ports[0],
         "",
+        notify_callback,
     )
     mock_ssh_tunnel_forwarder.reset_mock()
     mock_pgexecute.reset_mock()
 
     # Test with DSN
     dsn = (
         f"user={db_params['user']} password={db_params['passwd']} "
```

### Comparing `pgcli-4.0.1/tests/utils.py` & `pgcli-4.1.0/tests/utils.py`

 * *Files identical despite different names*

