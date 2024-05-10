# Comparing `tmp/singlestoredb-1.2.0.tar.gz` & `tmp/singlestoredb-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "singlestoredb-1.2.0.tar", last modified: Thu Apr 25 18:57:34 2024, max compression
+gzip compressed data, was "singlestoredb-1.3.0.tar", last modified: Fri May 10 21:29:57 2024, max compression
```

## Comparing `singlestoredb-1.2.0.tar` & `singlestoredb-1.3.0.tar`

### file list

```diff
@@ -1,143 +1,143 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:57:34.074437 singlestoredb-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11341 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4896 2024-04-25 18:57:34.074437 singlestoredb-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4066 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)   161827 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/accel.c
--rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-04-25 18:57:34.078437 singlestoredb-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:57:34.062437 singlestoredb-1.2.0/singlestoredb/
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:57:34.062437 singlestoredb-1.2.0/singlestoredb/alchemy/
--rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/alchemy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7599 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    11822 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    44392 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    20681 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/converters.py
--rw-r--r--   0 runner    (1001) docker     (127)     3234 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:57:34.066437 singlestoredb-1.2.0/singlestoredb/functions/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5193 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/functions/decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)    31408 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/functions/dtypes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:57:34.066437 singlestoredb-1.2.0/singlestoredb/functions/ext/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/functions/ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9061 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/functions/ext/arrow.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    40088 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/functions/ext/asgi.py
--rw-r--r--   0 runner    (1001) docker     (127)    10404 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/functions/ext/json.py
--rw-r--r--   0 runner    (1001) docker     (127)    13711 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/functions/ext/mmap.py
--rw-r--r--   0 runner    (1001) docker     (127)    22306 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/functions/ext/rowdat_1.py
--rw-r--r--   0 runner    (1001) docker     (127)     5311 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/functions/ext/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    18866 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/functions/signature.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:57:34.066437 singlestoredb-1.2.0/singlestoredb/fusion/
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/fusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5207 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/fusion/graphql.py
--rw-r--r--   0 runner    (1001) docker     (127)    21581 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/fusion/handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:57:34.066437 singlestoredb-1.2.0/singlestoredb/fusion/handlers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/fusion/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13643 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/fusion/handlers/stage.py
--rw-r--r--   0 runner    (1001) docker     (127)     5109 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/fusion/handlers/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    25000 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/fusion/handlers/workspace.py
--rw-r--r--   0 runner    (1001) docker     (127)     6112 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/fusion/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)    11772 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/fusion/result.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:57:34.066437 singlestoredb-1.2.0/singlestoredb/http/
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    38818 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/http/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:57:34.066437 singlestoredb-1.2.0/singlestoredb/management/
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3735 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/management/billing_usage.py
--rw-r--r--   0 runner    (1001) docker     (127)    14362 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/management/cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     8810 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/management/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     4974 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/management/organization.py
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/management/region.py
--rw-r--r--   0 runner    (1001) docker     (127)     9197 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/management/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    61632 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/management/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:57:34.070437 singlestoredb-1.2.0/singlestoredb/mysql/
--rw-r--r--   0 runner    (1001) docker     (127)     4492 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/mysql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8043 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/mysql/_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    10510 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/mysql/charset.py
--rw-r--r--   0 runner    (1001) docker     (127)    67884 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/mysql/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:57:34.070437 singlestoredb-1.2.0/singlestoredb/mysql/constants/
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/mysql/constants/CLIENT.py
--rw-r--r--   0 runner    (1001) docker     (127)      679 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/mysql/constants/COMMAND.py
--rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/mysql/constants/CR.py
--rw-r--r--   0 runner    (1001) docker     (127)    12296 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/mysql/constants/ER.py
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/mysql/constants/EXTENDED_TYPE.py
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/mysql/constants/FIELD_TYPE.py
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/mysql/constants/FLAG.py
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/mysql/constants/SERVER_STATUS.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/mysql/constants/VECTOR_TYPE.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/mysql/constants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7500 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/mysql/converters.py
--rw-r--r--   0 runner    (1001) docker     (127)    26527 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/mysql/cursors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2388 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/mysql/err.py
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/mysql/optionfile.py
--rw-r--r--   0 runner    (1001) docker     (127)    14451 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/mysql/protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:57:34.070437 singlestoredb-1.2.0/singlestoredb/mysql/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/mysql/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4025 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/mysql/tests/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/mysql/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     4878 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/mysql/tests/test_DictCursor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4306 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/mysql/tests/test_SSCursor.py
--rw-r--r--   0 runner    (1001) docker     (127)    15465 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/mysql/tests/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (127)    32297 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/mysql/tests/test_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/mysql/tests/test_converters.py
--rw-r--r--   0 runner    (1001) docker     (127)     5045 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/mysql/tests/test_cursor.py
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/mysql/tests/test_err.py
--rw-r--r--   0 runner    (1001) docker     (127)    18965 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/mysql/tests/test_issues.py
--rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/mysql/tests/test_load_local.py
--rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/mysql/tests/test_nextset.py
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/mysql/tests/test_optionfile.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:57:34.070437 singlestoredb-1.2.0/singlestoredb/mysql/tests/thirdparty/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/mysql/tests/thirdparty/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:57:34.070437 singlestoredb-1.2.0/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10171 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/capabilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    31414 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/dbapi20.py
--rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_capabilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     8022 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_dbapi20.py
--rw-r--r--   0 runner    (1001) docker     (127)     2819 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_nonstandard.py
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/mysql/times.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:57:34.074437 singlestoredb-1.2.0/singlestoredb/notebook/
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/notebook/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7995 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/notebook/_objects.py
--rw-r--r--   0 runner    (1001) docker     (127)     9074 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/pytest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:57:34.074437 singlestoredb-1.2.0/singlestoredb/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/tests/empty.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:57:34.074437 singlestoredb-1.2.0/singlestoredb/tests/ext_funcs/
--rw-r--r--   0 runner    (1001) docker     (127)     9290 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/tests/ext_funcs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/tests/local_infile.csv
--rw-r--r--   0 runner    (1001) docker     (127)    17679 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/tests/test.sql
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/tests/test2.sql
--rwxr-xr-x   0 runner    (1001) docker     (127)    44180 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/tests/test_basics.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    11184 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/tests/test_config.py
--rwxr-xr-x   0 runner    (1001) docker     (127)   117405 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/tests/test_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/tests/test_dbapi.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1131 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/tests/test_exceptions.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    37357 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/tests/test_ext_func.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    47695 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/tests/test_ext_func_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    15100 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/tests/test_fusion.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8580 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/tests/test_http.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    28223 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/tests/test_management.py
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/tests/test_plugin.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6582 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/tests/test_results.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4500 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/tests/test_types.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    28075 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/tests/test_udf.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10408 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/tests/test_xdict.py
--rw-r--r--   0 runner    (1001) docker     (127)     4673 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9969 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:57:34.074437 singlestoredb-1.2.0/singlestoredb/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24503 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/utils/convert_rows.py
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/utils/debug.py
--rw-r--r--   0 runner    (1001) docker     (127)     5898 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/utils/dtypes.py
--rw-r--r--   0 runner    (1001) docker     (127)     4050 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/utils/mogrify.py
--rw-r--r--   0 runner    (1001) docker     (127)    15153 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/utils/results.py
--rw-r--r--   0 runner    (1001) docker     (127)    12896 2024-04-25 18:57:12.000000 singlestoredb-1.2.0/singlestoredb/utils/xdict.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:57:34.062437 singlestoredb-1.2.0/singlestoredb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4896 2024-04-25 18:57:34.000000 singlestoredb-1.2.0/singlestoredb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4462 2024-04-25 18:57:34.000000 singlestoredb-1.2.0/singlestoredb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 18:57:34.000000 singlestoredb-1.2.0/singlestoredb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-25 18:57:34.000000 singlestoredb-1.2.0/singlestoredb.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-25 18:57:34.000000 singlestoredb-1.2.0/singlestoredb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-25 18:57:34.000000 singlestoredb-1.2.0/singlestoredb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:29:57.152995 singlestoredb-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11341 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4896 2024-05-10 21:29:57.152995 singlestoredb-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4066 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)   161827 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/accel.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-05-10 21:29:57.152995 singlestoredb-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:29:57.136995 singlestoredb-1.3.0/singlestoredb/
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:29:57.136995 singlestoredb-1.3.0/singlestoredb/alchemy/
+-rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/alchemy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7599 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11822 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44958 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20681 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/converters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3234 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:29:57.140995 singlestoredb-1.3.0/singlestoredb/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5193 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/functions/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31408 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/functions/dtypes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:29:57.140995 singlestoredb-1.3.0/singlestoredb/functions/ext/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/functions/ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9061 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/functions/ext/arrow.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    40088 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/functions/ext/asgi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10404 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/functions/ext/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13711 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/functions/ext/mmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22306 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/functions/ext/rowdat_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5311 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/functions/ext/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18866 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/functions/signature.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:29:57.140995 singlestoredb-1.3.0/singlestoredb/fusion/
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/fusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5207 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/fusion/graphql.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21581 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/fusion/handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:29:57.140995 singlestoredb-1.3.0/singlestoredb/fusion/handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/fusion/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13643 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/fusion/handlers/stage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5109 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/fusion/handlers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25000 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/fusion/handlers/workspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6112 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/fusion/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11772 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/fusion/result.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:29:57.140995 singlestoredb-1.3.0/singlestoredb/http/
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39349 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/http/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:29:57.140995 singlestoredb-1.3.0/singlestoredb/management/
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3735 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/management/billing_usage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14362 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/management/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8810 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/management/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4974 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/management/organization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/management/region.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9197 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/management/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61632 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/management/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:29:57.144996 singlestoredb-1.3.0/singlestoredb/mysql/
+-rw-r--r--   0 runner    (1001) docker     (127)     4492 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/mysql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8043 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/mysql/_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10510 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/mysql/charset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    70301 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/mysql/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:29:57.144996 singlestoredb-1.3.0/singlestoredb/mysql/constants/
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/mysql/constants/CLIENT.py
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/mysql/constants/COMMAND.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/mysql/constants/CR.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12296 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/mysql/constants/ER.py
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/mysql/constants/EXTENDED_TYPE.py
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/mysql/constants/FIELD_TYPE.py
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/mysql/constants/FLAG.py
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/mysql/constants/SERVER_STATUS.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/mysql/constants/VECTOR_TYPE.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/mysql/constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7500 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/mysql/converters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26794 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/mysql/cursors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2388 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/mysql/err.py
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/mysql/optionfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14451 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/mysql/protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:29:57.144996 singlestoredb-1.3.0/singlestoredb/mysql/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/mysql/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4025 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/mysql/tests/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/mysql/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4878 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/mysql/tests/test_DictCursor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4306 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/mysql/tests/test_SSCursor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15465 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/mysql/tests/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32297 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/mysql/tests/test_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/mysql/tests/test_converters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5045 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/mysql/tests/test_cursor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/mysql/tests/test_err.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18965 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/mysql/tests/test_issues.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/mysql/tests/test_load_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/mysql/tests/test_nextset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/mysql/tests/test_optionfile.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:29:57.144996 singlestoredb-1.3.0/singlestoredb/mysql/tests/thirdparty/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/mysql/tests/thirdparty/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:29:57.148995 singlestoredb-1.3.0/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10171 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31414 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/dbapi20.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8022 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_dbapi20.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2819 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_nonstandard.py
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/mysql/times.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:29:57.148995 singlestoredb-1.3.0/singlestoredb/notebook/
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/notebook/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7995 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/notebook/_objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9074 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/pytest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:29:57.148995 singlestoredb-1.3.0/singlestoredb/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/tests/empty.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:29:57.148995 singlestoredb-1.3.0/singlestoredb/tests/ext_funcs/
+-rw-r--r--   0 runner    (1001) docker     (127)     9290 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/tests/ext_funcs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/tests/local_infile.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    17679 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/tests/test.sql
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/tests/test2.sql
+-rwxr-xr-x   0 runner    (1001) docker     (127)    44180 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/tests/test_basics.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11184 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/tests/test_config.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)   117405 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/tests/test_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/tests/test_dbapi.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1131 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/tests/test_exceptions.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    37357 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/tests/test_ext_func.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    47695 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/tests/test_ext_func_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15100 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/tests/test_fusion.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8580 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/tests/test_http.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    28223 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/tests/test_management.py
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/tests/test_plugin.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6582 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/tests/test_results.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4500 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/tests/test_types.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    28075 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/tests/test_udf.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10408 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/tests/test_xdict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4673 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9969 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:29:57.152995 singlestoredb-1.3.0/singlestoredb/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24503 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/utils/convert_rows.py
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/utils/debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5898 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/utils/dtypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4050 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/utils/mogrify.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15277 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/utils/results.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12896 2024-05-10 21:29:35.000000 singlestoredb-1.3.0/singlestoredb/utils/xdict.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:29:57.136995 singlestoredb-1.3.0/singlestoredb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4896 2024-05-10 21:29:57.000000 singlestoredb-1.3.0/singlestoredb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4462 2024-05-10 21:29:57.000000 singlestoredb-1.3.0/singlestoredb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 21:29:57.000000 singlestoredb-1.3.0/singlestoredb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-10 21:29:57.000000 singlestoredb-1.3.0/singlestoredb.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-10 21:29:57.000000 singlestoredb-1.3.0/singlestoredb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-10 21:29:57.000000 singlestoredb-1.3.0/singlestoredb.egg-info/top_level.txt
```

### Comparing `singlestoredb-1.2.0/LICENSE` & `singlestoredb-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.2.0/PKG-INFO` & `singlestoredb-1.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: singlestoredb
-Version: 1.2.0
+Version: 1.3.0
 Summary: Interface to the SingleStoreDB database and workspace management APIs
 Home-page: https://github.com/singlestore-labs/singlestoredb-python
 Author: SingleStore
 Author-email: support@singlestore.com
 License: Apache-2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `singlestoredb-1.2.0/README.md` & `singlestoredb-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.2.0/accel.c` & `singlestoredb-1.3.0/accel.c`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.2.0/setup.cfg` & `singlestoredb-1.3.0/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = singlestoredb
-version = 1.2.0
+version = 1.3.0
 description = Interface to the SingleStoreDB database and workspace management APIs
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/singlestore-labs/singlestoredb-python
 author = SingleStore
 author_email = support@singlestore.com
 license = Apache-2.0
```

### Comparing `singlestoredb-1.2.0/setup.py` & `singlestoredb-1.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.2.0/singlestoredb/__init__.py` & `singlestoredb-1.3.0/singlestoredb/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 >>> cur = conn.cursor()
 >>> cur.execute('select * from customers')
 >>> for row in cur:
 ...     print(row)
 
 """
 
-__version__ = '1.2.0'
+__version__ = '1.3.0'
 
 from typing import Any
 
 from .config import options, get_option, set_option, describe_option
 from .connection import connect, apilevel, threadsafety, paramstyle
 from .exceptions import (
     Warning, Error, InterfaceError, DatabaseError, OperationalError,
```

### Comparing `singlestoredb-1.2.0/singlestoredb/alchemy/__init__.py` & `singlestoredb-1.3.0/singlestoredb/alchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.2.0/singlestoredb/auth.py` & `singlestoredb-1.3.0/singlestoredb/auth.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.2.0/singlestoredb/config.py` & `singlestoredb-1.3.0/singlestoredb/config.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.2.0/singlestoredb/connection.py` & `singlestoredb-1.3.0/singlestoredb/connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 #!/usr/bin/env python
 """SingleStoreDB connections and cursors."""
 import abc
 import inspect
+import io
+import queue
 import re
+import sys
 import warnings
 import weakref
 from collections.abc import Mapping
 from collections.abc import MutableMapping
 from typing import Any
 from typing import Callable
 from typing import Dict
@@ -29,14 +32,19 @@
 
 from . import auth
 from . import exceptions
 from .config import get_option
 from .utils.results import Description
 from .utils.results import Result
 
+if sys.version_info < (3, 10):
+    InfileQueue = queue.Queue
+else:
+    InfileQueue = queue.Queue[Union[bytes, str]]
+
 
 # DB-API settings
 apilevel = '2.0'
 threadsafety = 1
 paramstyle = map_paramstyle = 'pyformat'
 positional_paramstyle = 'format'
 
@@ -492,28 +500,38 @@
         """Close the cursor."""
         raise NotImplementedError
 
     @abc.abstractmethod
     def execute(
         self, query: str,
         args: Optional[Union[Sequence[Any], Dict[str, Any], Any]] = None,
+        infile_stream: Optional[  # type: ignore
+            Union[
+                io.RawIOBase,
+                io.TextIOBase,
+                Iterator[Union[bytes, str]],
+                InfileQueue,
+            ]
+        ] = None,
     ) -> int:
         """
         Execute a SQL statement.
 
         Queries can use the ``format``-style parameters (``%s``) when using a
         list of paramters or ``pyformat``-style parameters (``%(key)s``)
         when using a dictionary of parameters.
 
         Parameters
         ----------
         query : str
             The SQL statement to execute
         args : Sequence or dict, optional
             Parameters to substitute into the SQL code
+        infile_stream : io.RawIOBase or io.TextIOBase or Iterator[bytes|str], optional
+            Data stream for ``LOCAL INFILE`` statement
 
         Examples
         --------
         >>> cur.execute('select * from mytable')
 
         >>> cur.execute('select * from mytable where id < %s', [100])
 
@@ -1335,15 +1353,16 @@
     conv : dict[int, Callable], optional
         Dictionary of data conversion functions
     credential_type : str, optional
         Type of authentication to use: auth.PASSWORD, auth.JWT, or auth.BROWSER_SSO
     autocommit : bool, optional
         Enable autocommits
     results_type : str, optional
-        The form of the query results: tuples, namedtuples, dicts
+        The form of the query results: tuples, namedtuples, dicts,
+        numpy, polars, pandas, arrow
     results_format : str, optional
         Deprecated. This option has been renamed to results_type.
     program_name : str, optional
         Name of the program
     conn_attrs : dict, optional
         Additional connection attributes for telemetry. Example:
         {'program_version': "1.0.2", "_connector_name": "dbt connector"}
```

### Comparing `singlestoredb-1.2.0/singlestoredb/converters.py` & `singlestoredb-1.3.0/singlestoredb/converters.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.2.0/singlestoredb/exceptions.py` & `singlestoredb-1.3.0/singlestoredb/exceptions.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.2.0/singlestoredb/functions/decorator.py` & `singlestoredb-1.3.0/singlestoredb/functions/decorator.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.2.0/singlestoredb/functions/dtypes.py` & `singlestoredb-1.3.0/singlestoredb/functions/dtypes.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.2.0/singlestoredb/functions/ext/arrow.py` & `singlestoredb-1.3.0/singlestoredb/functions/ext/arrow.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.2.0/singlestoredb/functions/ext/asgi.py` & `singlestoredb-1.3.0/singlestoredb/functions/ext/asgi.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.2.0/singlestoredb/functions/ext/json.py` & `singlestoredb-1.3.0/singlestoredb/functions/ext/json.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.2.0/singlestoredb/functions/ext/mmap.py` & `singlestoredb-1.3.0/singlestoredb/functions/ext/mmap.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.2.0/singlestoredb/functions/ext/rowdat_1.py` & `singlestoredb-1.3.0/singlestoredb/functions/ext/rowdat_1.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.2.0/singlestoredb/functions/ext/utils.py` & `singlestoredb-1.3.0/singlestoredb/functions/ext/utils.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.2.0/singlestoredb/functions/signature.py` & `singlestoredb-1.3.0/singlestoredb/functions/signature.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.2.0/singlestoredb/fusion/graphql.py` & `singlestoredb-1.3.0/singlestoredb/fusion/graphql.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.2.0/singlestoredb/fusion/handler.py` & `singlestoredb-1.3.0/singlestoredb/fusion/handler.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.2.0/singlestoredb/fusion/handlers/stage.py` & `singlestoredb-1.3.0/singlestoredb/fusion/handlers/stage.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.2.0/singlestoredb/fusion/handlers/utils.py` & `singlestoredb-1.3.0/singlestoredb/fusion/handlers/utils.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.2.0/singlestoredb/fusion/handlers/workspace.py` & `singlestoredb-1.3.0/singlestoredb/fusion/handlers/workspace.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.2.0/singlestoredb/fusion/registry.py` & `singlestoredb-1.3.0/singlestoredb/fusion/registry.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.2.0/singlestoredb/fusion/result.py` & `singlestoredb-1.3.0/singlestoredb/fusion/result.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.2.0/singlestoredb/http/__init__.py` & `singlestoredb-1.3.0/singlestoredb/http/__init__.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.2.0/singlestoredb/http/connection.py` & `singlestoredb-1.3.0/singlestoredb/http/connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #!/usr/bin/env python
 """SingleStoreDB HTTP API interface."""
 import datetime
 import decimal
 import functools
+import io
 import json
 import math
 import os
 import re
 import time
 from base64 import b64decode
 from typing import Any
@@ -416,27 +417,35 @@
     def close(self) -> None:
         """Close the cursor."""
         self._connection = None
 
     def execute(
         self, query: str,
         args: Optional[Union[Sequence[Any], Dict[str, Any]]] = None,
+        infile_stream: Optional[  # type: ignore
+            Union[
+                io.RawIOBase,
+                io.TextIOBase,
+                Iterable[Union[bytes, str]],
+                connection.InfileQueue,
+            ]
+        ] = None,
     ) -> int:
         """
         Execute a SQL statement.
 
         Parameters
         ----------
         query : str
             The SQL statement to execute
         args : iterable or dict, optional
             Parameters to substitute into the SQL code
 
         """
-        return self._execute(query, args)
+        return self._execute(query, args, infile_stream=infile_stream)
 
     def _validate_param_subs(
         self, query: str,
         args: Optional[Union[Sequence[Any], Dict[str, Any]]] = None,
     ) -> None:
         """Make sure the parameter substitions are valid."""
         if args:
@@ -492,14 +501,22 @@
 
         return self.rowcount
 
     def _execute(
         self, oper: str,
         params: Optional[Union[Sequence[Any], Dict[str, Any]]] = None,
         is_callproc: bool = False,
+        infile_stream: Optional[  # type: ignore
+            Union[
+                io.RawIOBase,
+                io.TextIOBase,
+                Iterable[Union[bytes, str]],
+                connection.InfileQueue,
+            ]
+        ] = None,
     ) -> int:
         self._descriptions = []
         self._schemas = []
         self._results = []
         self._pymy_results = []
         self._row_idx = -1
         self._result_idx = -1
```

### Comparing `singlestoredb-1.2.0/singlestoredb/management/billing_usage.py` & `singlestoredb-1.3.0/singlestoredb/management/billing_usage.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.2.0/singlestoredb/management/cluster.py` & `singlestoredb-1.3.0/singlestoredb/management/cluster.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.2.0/singlestoredb/management/manager.py` & `singlestoredb-1.3.0/singlestoredb/management/manager.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.2.0/singlestoredb/management/organization.py` & `singlestoredb-1.3.0/singlestoredb/management/organization.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.2.0/singlestoredb/management/region.py` & `singlestoredb-1.3.0/singlestoredb/management/region.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.2.0/singlestoredb/management/utils.py` & `singlestoredb-1.3.0/singlestoredb/management/utils.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.2.0/singlestoredb/management/workspace.py` & `singlestoredb-1.3.0/singlestoredb/management/workspace.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.2.0/singlestoredb/mysql/__init__.py` & `singlestoredb-1.3.0/singlestoredb/mysql/__init__.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.2.0/singlestoredb/mysql/_auth.py` & `singlestoredb-1.3.0/singlestoredb/mysql/_auth.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.2.0/singlestoredb/mysql/charset.py` & `singlestoredb-1.3.0/singlestoredb/mysql/charset.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.2.0/singlestoredb/mysql/connection.py` & `singlestoredb-1.3.0/singlestoredb/mysql/connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 # type: ignore
 # Python implementation of the MySQL client-server protocol
 # http://dev.mysql.com/doc/internals/en/client-server-protocol.html
 # Error codes:
 # https://dev.mysql.com/doc/refman/5.5/en/error-handling.html
 import errno
 import functools
+import io
 import os
+import queue
 import socket
 import struct
 import sys
 import traceback
 import warnings
+from typing import Iterable
 
 try:
     import _singlestoredb_accel
 except (ImportError, ModuleNotFoundError):
     _singlestoredb_accel = None
 
 from . import _auth
@@ -349,14 +352,15 @@
 
         if compress or named_pipe:
             raise NotImplementedError(
                 'compress and named_pipe arguments are not supported',
             )
 
         self._local_infile = bool(local_infile)
+        self._local_infile_stream = None
         if self._local_infile:
             client_flag |= CLIENT.LOCAL_FILES
         if multi_statements:
             client_flag |= CLIENT.MULTI_STATEMENTS
 
         if read_default_group and not read_default_file:
             if sys.platform.startswith('win'):
@@ -839,15 +843,15 @@
         return converters.escape_bytes(s)
 
     def cursor(self):
         """Create a new cursor to execute queries with."""
         return self.cursorclass(self)
 
     # The following methods are INTERNAL USE ONLY (called from Cursor)
-    def query(self, sql, unbuffered=False):
+    def query(self, sql, unbuffered=False, infile_stream=None):
         """
         Run a query on the server.
 
         Internal use only.
 
         """
         # if DEBUG:
@@ -855,16 +859,18 @@
         handler = fusion.get_handler(sql)
         if handler is not None:
             self._result = fusion.execute(self, sql, handler=handler)
             self._affected_rows = self._result.affected_rows
         else:
             if isinstance(sql, str):
                 sql = sql.encode(self.encoding, 'surrogateescape')
+            self._local_infile_stream = infile_stream
             self._execute_command(COMMAND.COM_QUERY, sql)
             self._affected_rows = self._read_query_result(unbuffered=unbuffered)
+            self._local_infile_stream = None
         return self._affected_rows
 
     def next_result(self, unbuffered=False):
         """
         Retrieve the next result set.
 
         Internal use only.
@@ -1867,29 +1873,87 @@
     def __init__(self, filename, connection):
         self.filename = filename
         self.connection = connection
 
     def send_data(self):
         """Send data packets from the local file to the server"""
         if not self.connection._sock:
-            raise err.InterfaceError(0, '')
+            raise err.InterfaceError(0, 'Connection is closed')
+
         conn = self.connection
+        infile = conn._local_infile_stream
+
+        # 16KB is efficient enough
+        packet_size = min(conn.max_allowed_packet, 16 * 1024)
 
         try:
-            with open(self.filename, 'rb') as open_file:
-                packet_size = min(
-                    conn.max_allowed_packet, 16 * 1024,
-                )  # 16KB is efficient enough
-                while True:
-                    chunk = open_file.read(packet_size)
-                    if not chunk:
-                        break
-                    conn.write_packet(chunk)
-        except OSError:
-            raise err.OperationalError(
-                ER.FILE_NOT_FOUND,
-                f"Can't find file '{self.filename}'",
-            )
+
+            if self.filename in [':stream:', b':stream:']:
+
+                if infile is None:
+                    raise err.OperationalError(
+                        ER.FILE_NOT_FOUND,
+                        ':stream: specified for LOCAL INFILE, but no stream was supplied',
+                    )
+
+                # Binary IO
+                elif isinstance(infile, io.RawIOBase):
+                    while True:
+                        chunk = infile.read(packet_size)
+                        if not chunk:
+                            break
+                        conn.write_packet(chunk)
+
+                # Text IO
+                elif isinstance(infile, io.TextIOBase):
+                    while True:
+                        chunk = infile.read(packet_size)
+                        if not chunk:
+                            break
+                        conn.write_packet(chunk.encode('utf8'))
+
+                # Iterable of bytes or str
+                elif isinstance(infile, Iterable):
+                    for chunk in infile:
+                        if not chunk:
+                            continue
+                        if isinstance(chunk, str):
+                            conn.write_packet(chunk.encode('utf8'))
+                        else:
+                            conn.write_packet(chunk)
+
+                # Queue (empty value ends the iteration)
+                elif isinstance(infile, queue.Queue):
+                    while True:
+                        chunk = infile.get()
+                        if not chunk:
+                            break
+                        if isinstance(chunk, str):
+                            conn.write_packet(chunk.encode('utf8'))
+                        else:
+                            conn.write_packet(chunk)
+
+                else:
+                    raise err.OperationalError(
+                        ER.FILE_NOT_FOUND,
+                        ':stream: specified for LOCAL INFILE, ' +
+                        f'but stream type is unrecognized: {infile}',
+                    )
+
+            else:
+                try:
+                    with open(self.filename, 'rb') as open_file:
+                        while True:
+                            chunk = open_file.read(packet_size)
+                            if not chunk:
+                                break
+                            conn.write_packet(chunk)
+                except OSError:
+                    raise err.OperationalError(
+                        ER.FILE_NOT_FOUND,
+                        f"Can't find file '{self.filename!s}'",
+                    )
+
         finally:
             if not conn._closed:
                 # send the empty packet to signify we are done sending data
                 conn.write_packet(b'')
```

### Comparing `singlestoredb-1.2.0/singlestoredb/mysql/constants/CLIENT.py` & `singlestoredb-1.3.0/singlestoredb/mysql/constants/CLIENT.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.2.0/singlestoredb/mysql/constants/COMMAND.py` & `singlestoredb-1.3.0/singlestoredb/mysql/constants/COMMAND.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.2.0/singlestoredb/mysql/constants/CR.py` & `singlestoredb-1.3.0/singlestoredb/mysql/constants/CR.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.2.0/singlestoredb/mysql/constants/ER.py` & `singlestoredb-1.3.0/singlestoredb/mysql/constants/ER.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.2.0/singlestoredb/mysql/constants/FIELD_TYPE.py` & `singlestoredb-1.3.0/singlestoredb/mysql/constants/FIELD_TYPE.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.2.0/singlestoredb/mysql/converters.py` & `singlestoredb-1.3.0/singlestoredb/mysql/converters.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.2.0/singlestoredb/mysql/cursors.py` & `singlestoredb-1.3.0/singlestoredb/mysql/cursors.py`

 * *Files 1% similar despite different names*

```diff
@@ -174,42 +174,44 @@
         conn = self._get_db()
 
         if args:
             query = query % self._escape_args(args, conn)
 
         return query
 
-    def execute(self, query, args=None):
+    def execute(self, query, args=None, infile_stream=None):
         """
         Execute a query.
 
         If args is a list or tuple, :1, :2, etc. can be used as a
         placeholder in the query.  If args is a dict, :name can be used
         as a placeholder in the query.
 
         Parameters
         ----------
         query : str
             Query to execute.
         args : Sequence[Any] or Dict[str, Any] or Any, optional
             Parameters used with query. (optional)
+        infile_stream : io.BytesIO or Iterator[bytes], optional
+            Data stream for ``LOCAL INFILE`` statements
 
         Returns
         -------
         int : Number of affected rows.
 
         """
         while self.nextset():
             pass
 
         log_query(query, args)
 
         query = self.mogrify(query, args)
 
-        result = self._query(query)
+        result = self._query(query, infile_stream=infile_stream)
         self._executed = query
         return result
 
     def executemany(self, query, args=None):
         """
         Run several data against one query.
 
@@ -383,18 +385,18 @@
         else:
             raise err.ProgrammingError('unknown scroll mode %s' % mode)
 
         if not (0 <= r < len(self._rows)):
             raise IndexError('out of range')
         self._rownumber = r
 
-    def _query(self, q):
+    def _query(self, q, infile_stream=None):
         conn = self._get_db()
         self._clear_result()
-        conn.query(q)
+        conn.query(q, infile_stream=infile_stream)
         self._do_get_result()
         return self.rowcount
 
     def _clear_result(self):
         self._rownumber = 0
         self._result = None
 
@@ -676,18 +678,18 @@
             while self.nextset():
                 pass
         finally:
             self._connection = None
 
     __del__ = close
 
-    def _query(self, q):
+    def _query(self, q, infile_stream=None):
         conn = self._get_db()
         self._clear_result()
-        conn.query(q, unbuffered=True)
+        conn.query(q, unbuffered=True, infile_stream=infile_stream)
         self._do_get_result()
         return self.rowcount
 
     def nextset(self):
         return self._nextset(unbuffered=True)
 
     def read_next(self):
```

### Comparing `singlestoredb-1.2.0/singlestoredb/mysql/err.py` & `singlestoredb-1.3.0/singlestoredb/mysql/err.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.2.0/singlestoredb/mysql/optionfile.py` & `singlestoredb-1.3.0/singlestoredb/mysql/optionfile.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.2.0/singlestoredb/mysql/protocol.py` & `singlestoredb-1.3.0/singlestoredb/mysql/protocol.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.2.0/singlestoredb/mysql/tests/__init__.py` & `singlestoredb-1.3.0/singlestoredb/mysql/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.2.0/singlestoredb/mysql/tests/base.py` & `singlestoredb-1.3.0/singlestoredb/mysql/tests/base.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.2.0/singlestoredb/mysql/tests/conftest.py` & `singlestoredb-1.3.0/singlestoredb/mysql/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.2.0/singlestoredb/mysql/tests/test_DictCursor.py` & `singlestoredb-1.3.0/singlestoredb/mysql/tests/test_DictCursor.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.2.0/singlestoredb/mysql/tests/test_SSCursor.py` & `singlestoredb-1.3.0/singlestoredb/mysql/tests/test_SSCursor.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.2.0/singlestoredb/mysql/tests/test_basic.py` & `singlestoredb-1.3.0/singlestoredb/mysql/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.2.0/singlestoredb/mysql/tests/test_connection.py` & `singlestoredb-1.3.0/singlestoredb/mysql/tests/test_connection.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.2.0/singlestoredb/mysql/tests/test_converters.py` & `singlestoredb-1.3.0/singlestoredb/mysql/tests/test_converters.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.2.0/singlestoredb/mysql/tests/test_cursor.py` & `singlestoredb-1.3.0/singlestoredb/mysql/tests/test_cursor.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.2.0/singlestoredb/mysql/tests/test_issues.py` & `singlestoredb-1.3.0/singlestoredb/mysql/tests/test_issues.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.2.0/singlestoredb/mysql/tests/test_load_local.py` & `singlestoredb-1.3.0/singlestoredb/mysql/tests/test_load_local.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.2.0/singlestoredb/mysql/tests/test_nextset.py` & `singlestoredb-1.3.0/singlestoredb/mysql/tests/test_nextset.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.2.0/singlestoredb/mysql/tests/test_optionfile.py` & `singlestoredb-1.3.0/singlestoredb/mysql/tests/test_optionfile.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.2.0/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/capabilities.py` & `singlestoredb-1.3.0/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/capabilities.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.2.0/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/dbapi20.py` & `singlestoredb-1.3.0/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/dbapi20.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.2.0/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_capabilities.py` & `singlestoredb-1.3.0/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_capabilities.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.2.0/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_dbapi20.py` & `singlestoredb-1.3.0/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_dbapi20.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.2.0/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_nonstandard.py` & `singlestoredb-1.3.0/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_nonstandard.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.2.0/singlestoredb/notebook/_objects.py` & `singlestoredb-1.3.0/singlestoredb/notebook/_objects.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.2.0/singlestoredb/pytest.py` & `singlestoredb-1.3.0/singlestoredb/pytest.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.2.0/singlestoredb/tests/ext_funcs/__init__.py` & `singlestoredb-1.3.0/singlestoredb/tests/ext_funcs/__init__.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.2.0/singlestoredb/tests/test.sql` & `singlestoredb-1.3.0/singlestoredb/tests/test.sql`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.2.0/singlestoredb/tests/test_basics.py` & `singlestoredb-1.3.0/singlestoredb/tests/test_basics.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.2.0/singlestoredb/tests/test_config.py` & `singlestoredb-1.3.0/singlestoredb/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.2.0/singlestoredb/tests/test_connection.py` & `singlestoredb-1.3.0/singlestoredb/tests/test_connection.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.2.0/singlestoredb/tests/test_dbapi.py` & `singlestoredb-1.3.0/singlestoredb/tests/test_dbapi.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.2.0/singlestoredb/tests/test_exceptions.py` & `singlestoredb-1.3.0/singlestoredb/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.2.0/singlestoredb/tests/test_ext_func.py` & `singlestoredb-1.3.0/singlestoredb/tests/test_ext_func.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.2.0/singlestoredb/tests/test_ext_func_data.py` & `singlestoredb-1.3.0/singlestoredb/tests/test_ext_func_data.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.2.0/singlestoredb/tests/test_fusion.py` & `singlestoredb-1.3.0/singlestoredb/tests/test_fusion.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.2.0/singlestoredb/tests/test_http.py` & `singlestoredb-1.3.0/singlestoredb/tests/test_http.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.2.0/singlestoredb/tests/test_management.py` & `singlestoredb-1.3.0/singlestoredb/tests/test_management.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.2.0/singlestoredb/tests/test_plugin.py` & `singlestoredb-1.3.0/singlestoredb/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.2.0/singlestoredb/tests/test_results.py` & `singlestoredb-1.3.0/singlestoredb/tests/test_results.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.2.0/singlestoredb/tests/test_types.py` & `singlestoredb-1.3.0/singlestoredb/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.2.0/singlestoredb/tests/test_udf.py` & `singlestoredb-1.3.0/singlestoredb/tests/test_udf.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.2.0/singlestoredb/tests/test_xdict.py` & `singlestoredb-1.3.0/singlestoredb/tests/test_xdict.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.2.0/singlestoredb/tests/utils.py` & `singlestoredb-1.3.0/singlestoredb/tests/utils.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.2.0/singlestoredb/types.py` & `singlestoredb-1.3.0/singlestoredb/types.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.2.0/singlestoredb/utils/config.py` & `singlestoredb-1.3.0/singlestoredb/utils/config.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.2.0/singlestoredb/utils/convert_rows.py` & `singlestoredb-1.3.0/singlestoredb/utils/convert_rows.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.2.0/singlestoredb/utils/dtypes.py` & `singlestoredb-1.3.0/singlestoredb/utils/dtypes.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.2.0/singlestoredb/utils/mogrify.py` & `singlestoredb-1.3.0/singlestoredb/utils/mogrify.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.2.0/singlestoredb/utils/results.py` & `singlestoredb-1.3.0/singlestoredb/utils/results.py`

 * *Files 1% similar despite different names*

```diff
@@ -511,14 +511,16 @@
 ] = {
     'tuple': _no_schema,
     'tuples': _no_schema,
     'namedtuple': _no_schema,
     'namedtuples': _no_schema,
     'dict': _no_schema,
     'dicts': _no_schema,
+    'structsequence': _no_schema,
+    'structsequences': _no_schema,
     'numpy': _description_to_numpy_schema,
     'pandas': _description_to_numpy_schema,
     'polars': _description_to_polars_schema,
     'arrow': _description_to_arrow_schema,
     'pyarrow': _description_to_arrow_schema,
 }
 
@@ -574,8 +576,10 @@
     Returns
     -------
     Dict[str, Any]
         A dictionary of function parameters containing schema information
         for the given format type
 
     """
-    return _schema_converters[format](desc) or {}
+    if format in _schema_converters:
+        return _schema_converters[format](desc) or {}
+    return {}
```

### Comparing `singlestoredb-1.2.0/singlestoredb/utils/xdict.py` & `singlestoredb-1.3.0/singlestoredb/utils/xdict.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.2.0/singlestoredb.egg-info/PKG-INFO` & `singlestoredb-1.3.0/singlestoredb.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: singlestoredb
-Version: 1.2.0
+Version: 1.3.0
 Summary: Interface to the SingleStoreDB database and workspace management APIs
 Home-page: https://github.com/singlestore-labs/singlestoredb-python
 Author: SingleStore
 Author-email: support@singlestore.com
 License: Apache-2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `singlestoredb-1.2.0/singlestoredb.egg-info/SOURCES.txt` & `singlestoredb-1.3.0/singlestoredb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

