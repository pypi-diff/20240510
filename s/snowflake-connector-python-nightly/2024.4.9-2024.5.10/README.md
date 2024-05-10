# Comparing `tmp/snowflake-connector-python-nightly-2024.4.9.tar.gz` & `tmp/snowflake_connector_python_nightly-2024.5.10.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snowflake-connector-python-nightly-2024.4.9.tar", last modified: Tue Apr  9 04:07:44 2024, max compression
+gzip compressed data, was "snowflake_connector_python_nightly-2024.5.10.tar", last modified: Fri May 10 04:06:44 2024, max compression
```

## Comparing `snowflake-connector-python-nightly-2024.4.9.tar` & `snowflake_connector_python_nightly-2024.5.10.tar`

### file list

```diff
@@ -1,257 +1,258 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:07:44.354408 snowflake-connector-python-nightly-2024.4.9/
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    58487 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/DESCRIPTION.md
--rw-r--r--   0 runner    (1001) docker     (127)    11365 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      926 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/NOTICE
--rw-r--r--   0 runner    (1001) docker     (127)     3588 2024-04-09 04:07:44.354408 snowflake-connector-python-nightly-2024.4.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3045 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/SECURITY.md
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-04-09 04:07:44.354408 snowflake-connector-python-nightly-2024.4.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     6919 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:07:44.306408 snowflake-connector-python-nightly-2024.4.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:07:44.306408 snowflake-connector-python-nightly-2024.4.9/src/snowflake/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:07:44.318408 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/
--rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11339 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/_query_context_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/_sql_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     5381 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/arrow_context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:07:44.322408 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/auth/
--rw-r--r--   0 runner    (1001) docker     (127)      991 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27978 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/auth/_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     7050 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/auth/by_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/auth/default.py
--rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/auth/idtoken.py
--rw-r--r--   0 runner    (1001) docker     (127)     6678 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/auth/keypair.py
--rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/auth/oauth.py
--rw-r--r--   0 runner    (1001) docker     (127)    11394 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/auth/okta.py
--rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/auth/usrpwdmfa.py
--rw-r--r--   0 runner    (1001) docker     (127)    17958 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/auth/webbrowser.py
--rw-r--r--   0 runner    (1001) docker     (127)     9913 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/azure_storage_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     4346 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/backoff_policies.py
--rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/bind_upload_agent.py
--rw-r--r--   0 runner    (1001) docker     (127)    23454 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     2894 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/compat.py
--rw-r--r--   0 runner    (1001) docker     (127)    19252 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/config_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    75785 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    32728 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/connection_diagnostic.py
--rw-r--r--   0 runner    (1001) docker     (127)    12971 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    27710 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/converter_issue23517.py
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/converter_null.py
--rw-r--r--   0 runner    (1001) docker     (127)     7633 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/converter_snowsql.py
--rw-r--r--   0 runner    (1001) docker     (127)    64707 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/cursor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/dbapi.py
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/description.py
--rw-r--r--   0 runner    (1001) docker     (127)     8018 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/encryption_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2708 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/errorcode.py
--rw-r--r--   0 runner    (1001) docker     (127)    20185 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/feature.py
--rw-r--r--   0 runner    (1001) docker     (127)     3246 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/file_compression_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    48252 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/file_transfer_agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     5011 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/file_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    16072 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/gcs_storage_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2802 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/gzip_decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3162 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/local_storage_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:07:44.306408 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:07:44.330408 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/
--rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/ArrayConverter.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/ArrayConverter.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/BinaryConverter.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/BinaryConverter.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/BooleanConverter.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/BooleanConverter.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    19180 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/CArrowChunkIterator.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2407 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/CArrowChunkIterator.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     4462 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/CArrowIterator.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4477 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/CArrowIterator.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    42047 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/CArrowTableIterator.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4892 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/CArrowTableIterator.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/DateConverter.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/DateConverter.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/DecimalConverter.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/DecimalConverter.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2739 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/FixedSizeListConverter.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/FixedSizeListConverter.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      991 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/FloatConverter.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/FloatConverter.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/IColumnConverter.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/IntConverter.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/IntConverter.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    11583 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/MapConverter.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/MapConverter.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/ObjectConverter.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/ObjectConverter.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:07:44.334408 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/Python/
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/Python/Common.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2522 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/Python/Common.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/Python/Helpers.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/Python/Helpers.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/SnowflakeType.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      933 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/SnowflakeType.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/StringConverter.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/StringConverter.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/TimeConverter.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/TimeConverter.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    13329 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/TimeStampConverter.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4114 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/TimeStampConverter.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:07:44.334408 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/Util/
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/Util/macros.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/Util/time.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2262 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/Util/time.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:07:44.334408 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/
--rw-r--r--   0 runner    (1001) docker     (127)     6007 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_accessors.h
--rw-r--r--   0 runner    (1001) docker     (127)     3515 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_alloc.h
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_assert.h
--rw-r--r--   0 runner    (1001) docker     (127)    79675 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_builder.h
--rw-r--r--   0 runner    (1001) docker     (127)     7437 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_emitter.h
--rw-r--r--   0 runner    (1001) docker     (127)     3998 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_endian.h
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_epilogue.h
--rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_flatbuffers.h
--rw-r--r--   0 runner    (1001) docker     (127)     4778 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_identifier.h
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_iov.h
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_prologue.h
--rw-r--r--   0 runner    (1001) docker     (127)     4826 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_refmap.h
--rw-r--r--   0 runner    (1001) docker     (127)     4917 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_rtconfig.h
--rw-r--r--   0 runner    (1001) docker     (127)     3091 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_types.h
--rw-r--r--   0 runner    (1001) docker     (127)    10913 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_verifier.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:07:44.338408 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/flatcc_portable.h
--rw-r--r--   0 runner    (1001) docker     (127)     5852 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/paligned_alloc.h
--rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pattributes.h
--rw-r--r--   0 runner    (1001) docker     (127)     2613 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pdiagnostic.h
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pdiagnostic_pop.h
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pdiagnostic_push.h
--rw-r--r--   0 runner    (1001) docker     (127)     5284 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pendian.h
--rw-r--r--   0 runner    (1001) docker     (127)     3719 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pendian_detect.h
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pinline.h
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pinttypes.h
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/portable.h
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/portable_basic.h
--rw-r--r--   0 runner    (1001) docker     (127)     1844 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pstatic_assert.h
--rw-r--r--   0 runner    (1001) docker     (127)     4295 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pstdalign.h
--rw-r--r--   0 runner    (1001) docker     (127)    31201 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pstdint.h
--rw-r--r--   0 runner    (1001) docker     (127)     8882 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/punaligned.h
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pversion.h
--rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pwarnings.h
--rw-r--r--   0 runner    (1001) docker     (127)   102952 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc.c
--rw-r--r--   0 runner    (1001) docker     (127)   107680 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/nanoarrow.c
--rw-r--r--   0 runner    (1001) docker     (127)   132283 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/nanoarrow.h
--rw-r--r--   0 runner    (1001) docker     (127)    12046 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/nanoarrow.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     8404 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/nanoarrow_arrow_iterator.pyx
--rw-r--r--   0 runner    (1001) docker     (127)    18580 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/nanoarrow_device.c
--rw-r--r--   0 runner    (1001) docker     (127)    14382 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/nanoarrow_device.h
--rw-r--r--   0 runner    (1001) docker     (127)  1616169 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/nanoarrow_ipc.c
--rw-r--r--   0 runner    (1001) docker     (127)    17533 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/nanoarrow_ipc.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:07:44.338408 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/Logging/
--rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/Logging/logging.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/Logging/logging.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    42377 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/network.py
--rw-r--r--   0 runner    (1001) docker     (127)    16575 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/ocsp_asn1crypto.py
--rw-r--r--   0 runner    (1001) docker     (127)    69704 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/ocsp_snowflake.py
--rw-r--r--   0 runner    (1001) docker     (127)     4782 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/options.py
--rw-r--r--   0 runner    (1001) docker     (127)    22495 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/pandas_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    26617 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/result_batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     9380 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/result_set.py
--rw-r--r--   0 runner    (1001) docker     (127)    21870 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/s3_storage_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     5343 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/secret_detector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/sf_dirs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/sfbinaryformat.py
--rw-r--r--   0 runner    (1001) docker     (127)    12449 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/sfdatetime.py
--rw-r--r--   0 runner    (1001) docker     (127)     4313 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/snow_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/sqlstate.py
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/ssd_internal_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)     4563 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/ssl_wrap_socket.py
--rw-r--r--   0 runner    (1001) docker     (127)    17583 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/storage_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     8861 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/telemetry.py
--rw-r--r--   0 runner    (1001) docker     (127)    19070 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/telemetry_oob.py
--rw-r--r--   0 runner    (1001) docker     (127)      982 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/test_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     5073 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/time_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:07:44.338408 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/tool/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/tool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/tool/dump_certs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4575 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/tool/dump_ocsp_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     6643 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/tool/dump_ocsp_response_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/tool/probe_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/url_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    10405 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/util_text.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:07:44.338408 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:07:44.342408 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/requests/
--rw-r--r--   0 runner    (1001) docker     (127)    10142 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/requests/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4742 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/requests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/requests/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/requests/_internal_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    19577 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/requests/adapters.py
--rw-r--r--   0 runner    (1001) docker     (127)     6449 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/requests/api.py
--rw-r--r--   0 runner    (1001) docker     (127)    10187 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/requests/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/requests/certs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/requests/compat.py
--rw-r--r--   0 runner    (1001) docker     (127)    18560 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/requests/cookies.py
--rw-r--r--   0 runner    (1001) docker     (127)     3813 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/requests/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3885 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/requests/help.py
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/requests/hooks.py
--rw-r--r--   0 runner    (1001) docker     (127)    35231 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/requests/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    30373 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/requests/sessions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4235 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/requests/status_codes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/requests/structures.py
--rw-r--r--   0 runner    (1001) docker     (127)    33450 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/requests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:07:44.346408 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2763 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11372 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/_collections.py
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    20300 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    40285 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/connectionpool.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:07:44.346408 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/contrib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/contrib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      957 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/contrib/_appengine_environ.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:07:44.346408 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17632 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/bindings.py
--rw-r--r--   0 runner    (1001) docker     (127)    13922 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/low_level.py
--rw-r--r--   0 runner    (1001) docker     (127)    11012 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/contrib/appengine.py
--rw-r--r--   0 runner    (1001) docker     (127)     4528 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/contrib/ntlmpool.py
--rw-r--r--   0 runner    (1001) docker     (127)    16772 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/contrib/pyopenssl.py
--rw-r--r--   0 runner    (1001) docker     (127)    34431 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/contrib/securetransport.py
--rw-r--r--   0 runner    (1001) docker     (127)     7097 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/contrib/socks.py
--rw-r--r--   0 runner    (1001) docker     (127)     8217 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     8579 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/filepost.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:07:44.346408 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/packages/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/packages/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:07:44.346408 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/packages/backports/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/packages/backports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/packages/backports/makefile.py
--rw-r--r--   0 runner    (1001) docker     (127)     5343 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/packages/backports/weakref_finalize.py
--rw-r--r--   0 runner    (1001) docker     (127)    34665 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/packages/six.py
--rw-r--r--   0 runner    (1001) docker     (127)    19990 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/poolmanager.py
--rw-r--r--   0 runner    (1001) docker     (127)     6691 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/request.py
--rw-r--r--   0 runner    (1001) docker     (127)    30760 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:07:44.350408 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/util/
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5376 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/util/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/util/proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/util/queue.py
--rw-r--r--   0 runner    (1001) docker     (127)     4225 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/util/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3510 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/util/response.py
--rw-r--r--   0 runner    (1001) docker     (127)    22013 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/util/retry.py
--rw-r--r--   0 runner    (1001) docker     (127)    17165 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/util/ssl_.py
--rw-r--r--   0 runner    (1001) docker     (127)     5758 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/util/ssl_match_hostname.py
--rw-r--r--   0 runner    (1001) docker     (127)     6895 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/util/ssltransport.py
--rw-r--r--   0 runner    (1001) docker     (127)    10168 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/util/timeout.py
--rw-r--r--   0 runner    (1001) docker     (127)    14279 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/util/url.py
--rw-r--r--   0 runner    (1001) docker     (127)     5403 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/util/wait.py
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-09 04:07:33.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 04:07:44.350408 snowflake-connector-python-nightly-2024.4.9/src/snowflake_connector_python_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3588 2024-04-09 04:07:44.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake_connector_python_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13274 2024-04-09 04:07:44.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake_connector_python_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 04:07:44.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake_connector_python_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-09 04:07:44.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake_connector_python_nightly.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 04:07:43.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake_connector_python_nightly.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-09 04:07:44.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake_connector_python_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-09 04:07:44.000000 snowflake-connector-python-nightly-2024.4.9/src/snowflake_connector_python_nightly.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 04:06:44.554083 snowflake_connector_python_nightly-2024.5.10/
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-05-10 04:06:37.000000 snowflake_connector_python_nightly-2024.5.10/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    59128 2024-05-10 04:06:37.000000 snowflake_connector_python_nightly-2024.5.10/DESCRIPTION.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11365 2024-05-10 04:06:37.000000 snowflake_connector_python_nightly-2024.5.10/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-05-10 04:06:37.000000 snowflake_connector_python_nightly-2024.5.10/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-10 04:06:37.000000 snowflake_connector_python_nightly-2024.5.10/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)     3589 2024-05-10 04:06:44.554083 snowflake_connector_python_nightly-2024.5.10/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3045 2024-05-10 04:06:37.000000 snowflake_connector_python_nightly-2024.5.10/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-10 04:06:37.000000 snowflake_connector_python_nightly-2024.5.10/SECURITY.md
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-10 04:06:37.000000 snowflake_connector_python_nightly-2024.5.10/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-05-10 04:06:44.558083 snowflake_connector_python_nightly-2024.5.10/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     6919 2024-05-10 04:06:37.000000 snowflake_connector_python_nightly-2024.5.10/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 04:06:44.502083 snowflake_connector_python_nightly-2024.5.10/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 04:06:44.502083 snowflake_connector_python_nightly-2024.5.10/src/snowflake/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 04:06:44.518083 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/
+-rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-05-10 04:06:37.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11339 2024-05-10 04:06:37.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/_query_context_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-05-10 04:06:37.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/_sql_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5381 2024-05-10 04:06:37.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/arrow_context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 04:06:44.518083 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-05-10 04:06:37.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27978 2024-05-10 04:06:37.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/auth/_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7050 2024-05-10 04:06:37.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/auth/by_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-10 04:06:37.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/auth/default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-05-10 04:06:37.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/auth/idtoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6678 2024-05-10 04:06:37.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/auth/keypair.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-05-10 04:06:37.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/auth/oauth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11394 2024-05-10 04:06:37.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/auth/okta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-05-10 04:06:37.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/auth/usrpwdmfa.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17958 2024-05-10 04:06:37.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/auth/webbrowser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9913 2024-05-10 04:06:37.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/azure_storage_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4346 2024-05-10 04:06:37.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/backoff_policies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-05-10 04:06:37.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/bind_upload_agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23454 2024-05-10 04:06:37.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2894 2024-05-10 04:06:37.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19252 2024-05-10 04:06:37.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/config_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    76329 2024-05-10 04:06:37.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32728 2024-05-10 04:06:37.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/connection_diagnostic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12971 2024-05-10 04:06:37.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27710 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-05-10 04:06:37.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/converter_issue23517.py
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-10 04:06:37.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/converter_null.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7633 2024-05-10 04:06:37.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/converter_snowsql.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65081 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/cursor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/dbapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/description.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8018 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/encryption_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2708 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/errorcode.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20185 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3246 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/file_compression_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48252 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/file_transfer_agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5011 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/file_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16072 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/gcs_storage_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2802 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/gzip_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3162 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/local_storage_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/log_configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 04:06:44.502083 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 04:06:44.530083 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/
+-rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/ArrayConverter.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/ArrayConverter.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/BinaryConverter.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/BinaryConverter.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/BooleanConverter.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/BooleanConverter.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    19180 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/CArrowChunkIterator.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2407 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/CArrowChunkIterator.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4462 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/CArrowIterator.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4477 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/CArrowIterator.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    42107 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/CArrowTableIterator.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4263 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/CArrowTableIterator.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/DateConverter.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/DateConverter.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/DecimalConverter.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/DecimalConverter.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2739 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/FixedSizeListConverter.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/FixedSizeListConverter.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/FloatConverter.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/FloatConverter.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/IColumnConverter.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/IntConverter.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/IntConverter.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    11583 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/MapConverter.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/MapConverter.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/ObjectConverter.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/ObjectConverter.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 04:06:44.530083 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/Python/
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/Python/Common.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2522 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/Python/Common.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/Python/Helpers.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/Python/Helpers.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/SnowflakeType.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/SnowflakeType.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/StringConverter.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/StringConverter.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/TimeConverter.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/TimeConverter.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    13329 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/TimeStampConverter.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4114 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/TimeStampConverter.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 04:06:44.530083 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/Util/
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/Util/macros.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/Util/time.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2262 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/Util/time.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 04:06:44.534083 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/
+-rw-r--r--   0 runner    (1001) docker     (127)     6007 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_accessors.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3515 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_alloc.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_assert.h
+-rw-r--r--   0 runner    (1001) docker     (127)    79675 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_builder.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7437 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_emitter.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3998 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_endian.h
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_epilogue.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_flatbuffers.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4778 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_identifier.h
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_iov.h
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_prologue.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4826 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_refmap.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4917 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_rtconfig.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3091 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_types.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10913 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_verifier.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 04:06:44.538083 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/flatcc_portable.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5852 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/paligned_alloc.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pattributes.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2613 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pdiagnostic.h
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pdiagnostic_pop.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pdiagnostic_push.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5284 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pendian.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3719 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pendian_detect.h
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pinline.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pinttypes.h
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/portable.h
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/portable_basic.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1844 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pstatic_assert.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4295 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pstdalign.h
+-rw-r--r--   0 runner    (1001) docker     (127)    31201 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pstdint.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8882 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/punaligned.h
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pversion.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pwarnings.h
+-rw-r--r--   0 runner    (1001) docker     (127)   102952 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc.c
+-rw-r--r--   0 runner    (1001) docker     (127)   107680 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/nanoarrow.c
+-rw-r--r--   0 runner    (1001) docker     (127)   132283 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/nanoarrow.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12046 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/nanoarrow.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8404 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/nanoarrow_arrow_iterator.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)    18580 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/nanoarrow_device.c
+-rw-r--r--   0 runner    (1001) docker     (127)    14382 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/nanoarrow_device.h
+-rw-r--r--   0 runner    (1001) docker     (127)  1616169 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/nanoarrow_ipc.c
+-rw-r--r--   0 runner    (1001) docker     (127)    17533 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/nanoarrow_ipc.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 04:06:44.538083 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/Logging/
+-rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/Logging/logging.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/Logging/logging.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    42377 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16575 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/ocsp_asn1crypto.py
+-rw-r--r--   0 runner    (1001) docker     (127)    69704 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/ocsp_snowflake.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4782 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22495 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/pandas_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    26617 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/result_batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9380 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/result_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22246 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/s3_storage_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5343 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/secret_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/sf_dirs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/sfbinaryformat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12449 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/sfdatetime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4313 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/snow_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/sqlstate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/ssd_internal_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4563 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/ssl_wrap_socket.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17583 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/storage_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8861 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/telemetry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19070 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/telemetry_oob.py
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5073 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/time_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 04:06:44.538083 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/tool/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/tool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/tool/dump_certs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4575 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/tool/dump_ocsp_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6643 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/tool/dump_ocsp_response_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/tool/probe_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/url_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10405 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/util_text.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 04:06:44.538083 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/vendored/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/vendored/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 04:06:44.542083 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/vendored/requests/
+-rw-r--r--   0 runner    (1001) docker     (127)    10142 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/vendored/requests/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4742 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/vendored/requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/vendored/requests/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/vendored/requests/_internal_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19577 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/vendored/requests/adapters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6449 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/vendored/requests/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10187 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/vendored/requests/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/vendored/requests/certs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/vendored/requests/compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18560 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/vendored/requests/cookies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3813 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/vendored/requests/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3885 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/vendored/requests/help.py
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/vendored/requests/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35231 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/vendored/requests/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30373 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/vendored/requests/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4235 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/vendored/requests/status_codes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/vendored/requests/structures.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33450 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/vendored/requests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 04:06:44.546083 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/vendored/urllib3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/vendored/urllib3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2763 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/vendored/urllib3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11372 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/vendored/urllib3/_collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/vendored/urllib3/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20300 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/vendored/urllib3/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40285 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/vendored/urllib3/connectionpool.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 04:06:44.546083 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/vendored/urllib3/contrib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/vendored/urllib3/contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/vendored/urllib3/contrib/_appengine_environ.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 04:06:44.546083 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17632 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/bindings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13922 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/low_level.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11012 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/vendored/urllib3/contrib/appengine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4528 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/vendored/urllib3/contrib/ntlmpool.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16772 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/vendored/urllib3/contrib/pyopenssl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34431 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/vendored/urllib3/contrib/securetransport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7097 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/vendored/urllib3/contrib/socks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8217 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/vendored/urllib3/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8579 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/vendored/urllib3/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/vendored/urllib3/filepost.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 04:06:44.546083 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/vendored/urllib3/packages/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/vendored/urllib3/packages/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 04:06:44.550083 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/vendored/urllib3/packages/backports/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/vendored/urllib3/packages/backports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/vendored/urllib3/packages/backports/makefile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5343 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/vendored/urllib3/packages/backports/weakref_finalize.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34665 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/vendored/urllib3/packages/six.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19990 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/vendored/urllib3/poolmanager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6691 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/vendored/urllib3/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30760 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/vendored/urllib3/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 04:06:44.550083 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/vendored/urllib3/util/
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/vendored/urllib3/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5376 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/vendored/urllib3/util/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/vendored/urllib3/util/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/vendored/urllib3/util/queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4225 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/vendored/urllib3/util/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3510 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/vendored/urllib3/util/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22013 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/vendored/urllib3/util/retry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17165 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/vendored/urllib3/util/ssl_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5758 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/vendored/urllib3/util/ssl_match_hostname.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6895 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/vendored/urllib3/util/ssltransport.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10168 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/vendored/urllib3/util/timeout.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14279 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/vendored/urllib3/util/url.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5403 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/vendored/urllib3/util/wait.py
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-10 04:06:38.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 04:06:44.554083 snowflake_connector_python_nightly-2024.5.10/src/snowflake_connector_python_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3589 2024-05-10 04:06:44.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake_connector_python_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13319 2024-05-10 04:06:44.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake_connector_python_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 04:06:44.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake_connector_python_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-10 04:06:44.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake_connector_python_nightly.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 04:06:44.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake_connector_python_nightly.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-10 04:06:44.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake_connector_python_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-10 04:06:44.000000 snowflake_connector_python_nightly-2024.5.10/src/snowflake_connector_python_nightly.egg-info/top_level.txt
```

### Comparing `snowflake-connector-python-nightly-2024.4.9/CONTRIBUTING.md` & `snowflake_connector_python_nightly-2024.5.10/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/DESCRIPTION.md` & `snowflake_connector_python_nightly-2024.5.10/DESCRIPTION.md`

 * *Files identical despite different names*

```diff
@@ -4,14 +4,32 @@
 Snowflake Documentation is available at:
 https://docs.snowflake.com/
 
 Source code is also available at: https://github.com/snowflakedb/snowflake-connector-python
 
 # Release Notes
 
+- v3.11.0(TBD)
+
+  - Added support for `token_file_path` connection parameter to read an OAuth token from a file when connecting to Snowflake.
+
+- v3.10.0(April 29,2024)
+
+  - Added support for structured types to fetch_pandas_all.
+  - Fixed an issue relating to incorrectly formed China S3 endpoints.
+
+- v3.9.1(April 22,2024)
+
+  - Fixed an issue that caused a HTTP 400 error when connecting to a China endpoint.
+
+- v3.9.0(April 20,2024)
+
+  - Added easy logging configuration so that users can easily generate log file by setup log config in `$SNOWFLAKE_HOME/config.toml`.
+  - Improved s3 acceleration logic when connecting to China endpoint.
+
 - v3.8.1(April 09, 2024)
 
   - Reverted the change "Updated `write_pandas` to skip TABLE IF NOT EXISTS in truncate mode." introduced in v3.8.0 (yanked) as it's a breaking change. `write_pandas` will be fixed in the future in a non-breaking way.
 
 - v3.8.0(April 04,2024)
 
   - Improved `externalbrowser` auth in containerized environments
```

### Comparing `snowflake-connector-python-nightly-2024.4.9/LICENSE.txt` & `snowflake_connector_python_nightly-2024.5.10/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/MANIFEST.in` & `snowflake_connector_python_nightly-2024.5.10/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/PKG-INFO` & `snowflake_connector_python_nightly-2024.5.10/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snowflake-connector-python-nightly
-Version: 2024.4.9
+Version: 2024.5.10
 Summary: Nigthly build of Snowflake Connector for Python
 Home-page: https://www.snowflake.com/
 Author: Snowflake, Inc
 Author-email: snowflake-python-libraries-dl@snowflake.com
 License: Apache-2.0
 Project-URL: Documentation, https://docs.snowflake.com/en/user-guide/python-connector.html
 Project-URL: Source, https://github.com/keller00/snowflake-connector-python-nightlies/
```

### Comparing `snowflake-connector-python-nightly-2024.4.9/README.md` & `snowflake_connector_python_nightly-2024.5.10/README.md`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/pyproject.toml` & `snowflake_connector_python_nightly-2024.5.10/pyproject.toml`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/setup.cfg` & `snowflake_connector_python_nightly-2024.5.10/setup.cfg`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/setup.py` & `snowflake_connector_python_nightly-2024.5.10/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -172,11 +172,11 @@
                 build_ext.build_extension(self, ext)
             finally:
                 self.compiler._compile = original__compile
 
     cmd_class = {"build_ext": MyBuildExt}
 
 setup(
-    version="2024.04.09",
+    version="2024.05.10",
     ext_modules=extensions,
     cmdclass=cmd_class,
 )
```

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/__init__.py` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,14 +40,15 @@
     InterfaceError,
     InternalError,
     NotSupportedError,
     OperationalError,
     ProgrammingError,
     _Warning,
 )
+from .log_configuration import EasyLoggingConfigPython
 from .version import VERSION
 
 logging.getLogger(__name__).addHandler(NullHandler())
 
 
 @wraps(SnowflakeConnection.__init__)
 def Connect(**kwargs) -> SnowflakeConnection:
@@ -88,8 +89,9 @@
     "TimestampFromTicks",
     "STRING",
     "BINARY",
     "NUMBER",
     "DATETIME",
     "ROWID",
     # Extended data type (experimental)
+    "EasyLoggingConfigPython",
 ]
```

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/_query_context_cache.py` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/_query_context_cache.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/_sql_util.py` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/_sql_util.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/arrow_context.py` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/arrow_context.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/auth/__init__.py` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/auth/_auth.py` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/auth/_auth.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/auth/by_plugin.py` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/auth/by_plugin.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/auth/default.py` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/auth/default.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/auth/idtoken.py` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/auth/idtoken.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/auth/keypair.py` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/auth/keypair.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/auth/oauth.py` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/auth/oauth.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/auth/okta.py` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/auth/okta.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/auth/usrpwdmfa.py` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/auth/usrpwdmfa.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/auth/webbrowser.py` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/auth/webbrowser.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/azure_storage_client.py` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/azure_storage_client.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/backoff_policies.py` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/backoff_policies.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/bind_upload_agent.py` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/bind_upload_agent.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/cache.py` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/cache.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/compat.py` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/compat.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/config_manager.py` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/config_manager.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/connection.py` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,14 +88,15 @@
     ER_NO_ACCOUNT_NAME,
     ER_NO_NUMPY,
     ER_NO_PASSWORD,
     ER_NO_USER,
     ER_NOT_IMPLICITY_SNOWFLAKE_DATATYPE,
 )
 from .errors import DatabaseError, Error, OperationalError, ProgrammingError
+from .log_configuration import EasyLoggingConfigPython
 from .network import (
     DEFAULT_AUTHENTICATOR,
     EXTERNAL_BROWSER_AUTHENTICATOR,
     KEY_PAIR_AUTHENTICATOR,
     OAUTH_AUTHENTICATOR,
     REQUEST_ID,
     USR_PWD_MFA_AUTHENTICATOR,
@@ -354,14 +355,15 @@
         connection_diag_whitelist_path: path to a whitelist.json file to test with enable_connection_diag - deprecated remove in future
         connection_diag_allowlist_path: path to a allowlist.json file to test with enable_connection_diag.
         json_result_force_utf8_decoding: When true, json result will be decoded in utf-8,
           when false, the encoding of the content is auto-detected. Default value is false.
           This parameter is only effective when the result format is JSON.
         server_session_keep_alive: When true, the connector does not destroy the session on the Snowflake server side
           before the connector shuts down. Default value is false.
+        token_file_path: The file path of the token file. If both token and token_file_path are provided, the token in token_file_path will be used.
     """
 
     OCSP_ENV_LOCK = Lock()
 
     def __init__(
         self,
         connection_name: str | None = None,
@@ -379,14 +381,17 @@
         When no arguments are given (other than connection_file_path) the
         default connection will be loaded first. Note that no overwriting is
         supported in this case.
 
         If overwriting values from the default connection is desirable, supply
         the name explicitly.
         """
+        # initiate easy logging during every connection
+        easy_logging = EasyLoggingConfigPython()
+        easy_logging.create_log()
         self._lock_sequence_counter = Lock()
         self.sequence_counter = 0
         self._errorhandler = Error.default_errorhandler
         self._lock_converter = Lock()
         self.messages = []
         self._async_sfqids: dict[str, None] = {}
         self._done_async_sfqids: dict[str, None] = {}
@@ -1174,14 +1179,20 @@
                 EXTERNAL_BROWSER_AUTHENTICATOR,
                 KEY_PAIR_AUTHENTICATOR,
                 OAUTH_AUTHENTICATOR,
                 USR_PWD_MFA_AUTHENTICATOR,
             ]:
                 self._authenticator = auth_tmp
 
+        # read OAuth token from
+        token_file_path = kwargs.get("token_file_path")
+        if token_file_path:
+            with open(token_file_path) as f:
+                self._token = f.read()
+
         if not (self._master_token and self._session_token):
             if not self.user and self._authenticator != OAUTH_AUTHENTICATOR:
                 # OAuth Authentication does not require a username
                 Error.errorhandler_wrapper(
                     self,
                     None,
                     ProgrammingError,
```

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/connection_diagnostic.py` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/connection_diagnostic.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/constants.py` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/constants.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/converter.py` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/converter.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/converter_issue23517.py` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/converter_issue23517.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/converter_snowsql.py` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/converter_snowsql.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/cursor.py` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/cursor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1310,15 +1310,25 @@
             raise NotSupportedError
         self._log_telemetry_job_data(
             TelemetryField.PANDAS_FETCH_BATCHES, TelemetryData.TRUE
         )
         return self._result_set._fetch_pandas_batches(**kwargs)
 
     def fetch_pandas_all(self, **kwargs: Any) -> DataFrame:
-        """Fetch Pandas dataframes in batches, where 'batch' refers to Snowflake Chunk."""
+        """
+        Fetch Pandas dataframes in batches, where 'batch' refers to Snowflake Chunk.
+
+        Returns:
+            A pandas dataframe containing the cursors query results.
+
+        Note:
+            Timestamp types that are nested in structured types may not be accurately represented
+            due to a limitation in the pyarrow to pandas conversion.
+            See here for more information: https://github.com/apache/arrow/issues/4116
+        """
         self.check_can_use_pandas()
         if self._prefetch_hook is not None:
             self._prefetch_hook()
         if self._query_result_format != "arrow":
             raise NotSupportedError
         self._log_telemetry_job_data(
             TelemetryField.PANDAS_FETCH_ALL, TelemetryData.TRUE
```

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/dbapi.py` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/dbapi.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/description.py` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/description.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/encryption_util.py` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/encryption_util.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/errorcode.py` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/errorcode.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/errors.py` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/errors.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/file_compression_type.py` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/file_compression_type.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/file_transfer_agent.py` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/file_transfer_agent.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/file_util.py` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/file_util.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/gcs_storage_client.py` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/gcs_storage_client.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/gzip_decoder.py` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/gzip_decoder.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/local_storage_client.py` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/local_storage_client.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/ArrayConverter.cpp` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/ArrayConverter.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/ArrayConverter.hpp` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/ArrayConverter.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/BinaryConverter.cpp` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/BinaryConverter.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/BinaryConverter.hpp` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/BinaryConverter.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/CArrowChunkIterator.cpp` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/CArrowChunkIterator.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/CArrowChunkIterator.hpp` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/CArrowChunkIterator.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/CArrowIterator.cpp` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/CArrowIterator.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/CArrowIterator.hpp` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/CArrowIterator.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/CArrowTableIterator.cpp` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/CArrowTableIterator.cpp`

 * *Files 21% similar despite different names*

```diff
@@ -11,14 +11,277 @@
 
 #include "Python/Common.hpp"
 #include "SnowflakeType.hpp"
 #include "Util/time.hpp"
 
 namespace sf {
 
+void CArrowTableIterator::convertIfNeeded(ArrowSchema* columnSchema,
+                                          ArrowArrayView* columnArray) {
+  ArrowSchemaView columnSchemaView;
+  ArrowError error;
+  int returnCode;
+
+  returnCode = ArrowSchemaViewInit(&columnSchemaView, columnSchema, &error);
+  SF_CHECK_ARROW_RC(returnCode,
+                    "[Snowflake Exception] error initializing "
+                    "ArrowSchemaView : %s, error code: %d",
+                    ArrowErrorMessage(&error), returnCode);
+
+  ArrowStringView snowflakeLogicalType;
+  const char* metadata = columnSchema->metadata;
+  returnCode = ArrowMetadataGetValue(metadata, ArrowCharView("logicalType"),
+                                     &snowflakeLogicalType);
+  SF_CHECK_ARROW_RC(returnCode,
+                    "[Snowflake Exception] error getting 'logicalType' "
+                    "from Arrow metadata, error code: %d",
+                    returnCode);
+  SnowflakeType::Type st = SnowflakeType::snowflakeTypeFromString(
+      std::string(snowflakeLogicalType.data, snowflakeLogicalType.size_bytes));
+
+  // reconstruct columnArray in place
+  switch (st) {
+    case SnowflakeType::Type::FIXED: {
+      int scale = 0;
+      struct ArrowStringView scaleString = ArrowCharView(nullptr);
+      if (metadata != nullptr) {
+        returnCode = ArrowMetadataGetValue(metadata, ArrowCharView("scale"),
+                                           &scaleString);
+        SF_CHECK_ARROW_RC(returnCode,
+                          "[Snowflake Exception] error getting 'scale' "
+                          "from Arrow metadata, error code: %d",
+                          returnCode);
+        scale =
+            std::stoi(std::string(scaleString.data, scaleString.size_bytes));
+      }
+      if (scale > 0 &&
+          columnSchemaView.type != ArrowType::NANOARROW_TYPE_DECIMAL128) {
+        logger->debug(__FILE__, __func__, __LINE__,
+                      "Convert fixed number column to double column, "
+                      "column scale %d, column type id: %d",
+                      scale, columnSchemaView.type);
+        convertScaledFixedNumberColumn_nanoarrow(&columnSchemaView, columnArray,
+                                                 scale);
+      }
+      break;
+    }
+
+    case SnowflakeType::Type::ANY:
+    case SnowflakeType::Type::BINARY:
+    case SnowflakeType::Type::BOOLEAN:
+    case SnowflakeType::Type::CHAR:
+    case SnowflakeType::Type::DATE:
+    case SnowflakeType::Type::REAL:
+    case SnowflakeType::Type::TEXT:
+    case SnowflakeType::Type::VARIANT:
+    case SnowflakeType::Type::VECTOR: {
+      // Do not need to convert
+      break;
+    }
+
+    case SnowflakeType::Type::ARRAY: {
+      switch (columnSchemaView.type) {
+        case NANOARROW_TYPE_STRING: {
+          // No need to convert json encoded array
+          break;
+        }
+        case NANOARROW_TYPE_LIST: {
+          if (columnSchemaView.schema->n_children != 1) {
+            std::string errorInfo = Logger::formatString(
+                "[Snowflake Exception] invalid arrow schema for array items "
+                "expected 1 "
+                "schema child, but got %d",
+                columnSchemaView.schema->n_children);
+            logger->error(__FILE__, __func__, __LINE__, errorInfo.c_str());
+            PyErr_SetString(PyExc_Exception, errorInfo.c_str());
+            break;
+          }
+
+          ArrowSchema* item_schema = columnSchemaView.schema->children[0];
+          ArrowArrayView* item_array = columnArray->children[0];
+          convertIfNeeded(item_schema, item_array);
+          break;
+        }
+        default: {
+          std::string errorInfo = Logger::formatString(
+              "[Snowflake Exception] unknown arrow internal data type(%s) "
+              "for ARRAY data in %s",
+              NANOARROW_TYPE_ENUM_STRING[columnSchemaView.type],
+              columnSchemaView.schema->name);
+          logger->error(__FILE__, __func__, __LINE__, errorInfo.c_str());
+          PyErr_SetString(PyExc_Exception, errorInfo.c_str());
+          break;
+        }
+      }
+      break;
+    }
+    case SnowflakeType::Type::MAP: {
+      if (columnSchemaView.schema->n_children != 1) {
+        std::string errorInfo = Logger::formatString(
+            "[Snowflake Exception] invalid arrow schema for map entries "
+            "expected 1 "
+            "schema child, but got %d",
+            columnSchemaView.schema->n_children);
+        logger->error(__FILE__, __func__, __LINE__, errorInfo.c_str());
+        PyErr_SetString(PyExc_Exception, errorInfo.c_str());
+        break;
+      }
+
+      ArrowSchema* entries = columnSchemaView.schema->children[0];
+      if (entries->n_children != 2) {
+        std::string errorInfo = Logger::formatString(
+            "[Snowflake Exception] invalid arrow schema for map key/value "
+            "pair "
+            "expected 2 entries, but got %d",
+            entries->n_children);
+        logger->error(__FILE__, __func__, __LINE__, errorInfo.c_str());
+        PyErr_SetString(PyExc_Exception, errorInfo.c_str());
+        break;
+      }
+
+      ArrowSchema* key_schema = entries->children[0];
+      ArrowArrayView* key_array = columnArray->children[0]->children[0];
+      convertIfNeeded(key_schema, key_array);
+
+      ArrowSchema* value_schema = entries->children[1];
+      ArrowArrayView* value_array = columnArray->children[0]->children[1];
+      convertIfNeeded(value_schema, value_array);
+      break;
+    }
+
+    case SnowflakeType::Type::OBJECT: {
+      switch (columnSchemaView.type) {
+        case NANOARROW_TYPE_STRING: {
+          // No need to convert json encoded data
+          break;
+        }
+        case NANOARROW_TYPE_STRUCT: {
+          // Object field names are strings that do not need conversion
+          // Child values values may need conversion.
+          for (int i = 0; i < columnSchemaView.schema->n_children; i++) {
+            ArrowSchema* property_schema = columnSchemaView.schema->children[i];
+            ArrowArrayView* child_array = columnArray->children[i];
+            convertIfNeeded(property_schema, child_array);
+          }
+          break;
+        }
+        default: {
+          std::string errorInfo = Logger::formatString(
+              "[Snowflake Exception] unknown arrow internal data type(%s) "
+              "for OBJECT data in %s",
+              NANOARROW_TYPE_ENUM_STRING[columnSchemaView.type],
+              columnSchemaView.schema->name);
+          logger->error(__FILE__, __func__, __LINE__, errorInfo.c_str());
+          PyErr_SetString(PyExc_Exception, errorInfo.c_str());
+          break;
+        }
+      }
+      break;
+    }
+
+    case SnowflakeType::Type::TIME: {
+      int scale = 9;
+      if (metadata != nullptr) {
+        struct ArrowStringView scaleString = ArrowCharView(nullptr);
+        returnCode = ArrowMetadataGetValue(metadata, ArrowCharView("scale"),
+                                           &scaleString);
+        SF_CHECK_ARROW_RC(returnCode,
+                          "[Snowflake Exception] error getting 'scale' "
+                          "from Arrow metadata, error code: %d",
+                          returnCode);
+        scale =
+            std::stoi(std::string(scaleString.data, scaleString.size_bytes));
+      }
+
+      convertTimeColumn_nanoarrow(&columnSchemaView, columnArray, scale);
+      break;
+    }
+
+    case SnowflakeType::Type::TIMESTAMP_NTZ: {
+      int scale = 9;
+      if (metadata != nullptr) {
+        struct ArrowStringView scaleString = ArrowCharView(nullptr);
+        returnCode = ArrowMetadataGetValue(metadata, ArrowCharView("scale"),
+                                           &scaleString);
+        SF_CHECK_ARROW_RC(returnCode,
+                          "[Snowflake Exception] error getting 'scale' "
+                          "from Arrow metadata, error code: %d",
+                          returnCode);
+        scale =
+            std::stoi(std::string(scaleString.data, scaleString.size_bytes));
+      }
+      convertTimestampColumn_nanoarrow(&columnSchemaView, columnArray, scale);
+      break;
+    }
+
+    case SnowflakeType::Type::TIMESTAMP_LTZ: {
+      int scale = 9;
+      if (metadata != nullptr) {
+        struct ArrowStringView scaleString = ArrowCharView(nullptr);
+        returnCode = ArrowMetadataGetValue(metadata, ArrowCharView("scale"),
+                                           &scaleString);
+        SF_CHECK_ARROW_RC(returnCode,
+                          "[Snowflake Exception] error getting 'scale' "
+                          "from Arrow metadata, error code: %d",
+                          returnCode);
+        scale =
+            std::stoi(std::string(scaleString.data, scaleString.size_bytes));
+      }
+
+      logger->error(__FILE__, __func__, __LINE__, "scale: %d", scale);
+      convertTimestampColumn_nanoarrow(&columnSchemaView, columnArray, scale,
+                                       m_timezone);
+      break;
+    }
+
+    case SnowflakeType::Type::TIMESTAMP_TZ: {
+      struct ArrowStringView scaleString = ArrowCharView(nullptr);
+      struct ArrowStringView byteLengthString = ArrowCharView(nullptr);
+      int scale = 9;
+      int byteLength = 16;
+      if (metadata != nullptr) {
+        returnCode = ArrowMetadataGetValue(metadata, ArrowCharView("scale"),
+                                           &scaleString);
+        SF_CHECK_ARROW_RC(returnCode,
+                          "[Snowflake Exception] error getting 'scale' "
+                          "from Arrow metadata, error code: %d",
+                          returnCode);
+        returnCode = ArrowMetadataGetValue(
+            metadata, ArrowCharView("byteLength"), &byteLengthString);
+        SF_CHECK_ARROW_RC(
+            returnCode,
+            "[Snowflake Exception] error getting 'byteLength' from Arrow "
+            "metadata, error code: %d",
+            returnCode);
+        scale =
+            std::stoi(std::string(scaleString.data, scaleString.size_bytes));
+        // Data inside a structured type may not have bytelength metadata.
+        // Use default in this case.
+        if (byteLengthString.data != nullptr) {
+          byteLength = std::stoi(
+              std::string(byteLengthString.data, byteLengthString.size_bytes));
+        }
+      }
+
+      convertTimestampTZColumn_nanoarrow(&columnSchemaView, columnArray, scale,
+                                         byteLength, m_timezone);
+      break;
+    }
+
+    default: {
+      std::string errorInfo = Logger::formatString(
+          "[Snowflake Exception] unknown snowflake data type : %s",
+          snowflakeLogicalType.data);
+      logger->error(__FILE__, __func__, __LINE__, errorInfo.c_str());
+      PyErr_SetString(PyExc_Exception, errorInfo.c_str());
+      return;
+    }
+  }
+}
+
 /**
  * This function is to make sure the arrow table can be successfully converted
  * to pandas dataframe using arrow's to_pandas method. Since some Snowflake
  * arrow columns are not supported, this method can map those to supported ones.
  * Specifically,
  *    All Snowflake fixed number with scale > 0 (expect decimal) will be
  * converted to Arrow float64/double column All Snowflake time columns will be
@@ -32,196 +295,30 @@
  * small and large timestamps
  */
 void CArrowTableIterator::reconstructRecordBatches_nanoarrow() {
   int returnCode = 0;
   // Type conversion, the code needs to be optimized
   for (unsigned int batchIdx = 0; batchIdx < m_ipcArrowArrayViewVec.size();
        batchIdx++) {
-    // each record batch will have its own list of newly created array and
-    // schema
-    m_newArrays.push_back(std::vector<nanoarrow::UniqueArray>());
-    m_newSchemas.push_back(std::vector<nanoarrow::UniqueSchema>());
-
     nanoarrow::UniqueSchema copiedSchema;
     returnCode =
         ArrowSchemaDeepCopy(m_ipcArrowSchema.get(), copiedSchema.get());
     SF_CHECK_ARROW_RC(
         returnCode,
         "[Snowflake Exception] error copying arrow schema, error code: %d",
         returnCode);
     m_ipcSchemaArrayVec.push_back(std::move(copiedSchema));
 
-    ArrowError error;
-    int returnCode;
     for (int colIdx = 0; colIdx < m_ipcSchemaArrayVec[batchIdx]->n_children;
          colIdx++) {
       ArrowArrayView* columnArray =
           m_ipcArrowArrayViewVec[batchIdx]->children[colIdx];
       ArrowSchema* columnSchema =
           m_ipcSchemaArrayVec[batchIdx]->children[colIdx];
-      ArrowSchemaView columnSchemaView;
-
-      returnCode = ArrowSchemaViewInit(&columnSchemaView, columnSchema, &error);
-      SF_CHECK_ARROW_RC(returnCode,
-                        "[Snowflake Exception] error initializing "
-                        "ArrowSchemaView : %s, error code: %d",
-                        ArrowErrorMessage(&error), returnCode);
-
-      ArrowStringView snowflakeLogicalType;
-      const char* metadata =
-          m_ipcSchemaArrayVec[batchIdx]->children[colIdx]->metadata;
-      returnCode = ArrowMetadataGetValue(metadata, ArrowCharView("logicalType"),
-                                         &snowflakeLogicalType);
-      SF_CHECK_ARROW_RC(returnCode,
-                        "[Snowflake Exception] error getting 'logicalType' "
-                        "from Arrow metadata, error code: %d",
-                        returnCode);
-      SnowflakeType::Type st =
-          SnowflakeType::snowflakeTypeFromString(std::string(
-              snowflakeLogicalType.data, snowflakeLogicalType.size_bytes));
-
-      // reconstruct columnArray in place
-      switch (st) {
-        case SnowflakeType::Type::FIXED: {
-          int scale = 0;
-          struct ArrowStringView scaleString = ArrowCharView(nullptr);
-          if (metadata != nullptr) {
-            returnCode = ArrowMetadataGetValue(metadata, ArrowCharView("scale"),
-                                               &scaleString);
-            SF_CHECK_ARROW_RC(returnCode,
-                              "[Snowflake Exception] error getting 'scale' "
-                              "from Arrow metadata, error code: %d",
-                              returnCode);
-            scale = std::stoi(
-                std::string(scaleString.data, scaleString.size_bytes));
-          }
-          if (scale > 0 &&
-              columnSchemaView.type != ArrowType::NANOARROW_TYPE_DECIMAL128) {
-            logger->debug(__FILE__, __func__, __LINE__,
-                          "Convert fixed number column to double column, "
-                          "column scale %d, column type id: %d",
-                          scale, columnSchemaView.type);
-            convertScaledFixedNumberColumn_nanoarrow(
-                batchIdx, colIdx, &columnSchemaView, columnArray, scale);
-          }
-          break;
-        }
-
-        case SnowflakeType::Type::ANY:
-        case SnowflakeType::Type::ARRAY:
-        case SnowflakeType::Type::BINARY:
-        case SnowflakeType::Type::BOOLEAN:
-        case SnowflakeType::Type::CHAR:
-        case SnowflakeType::Type::DATE:
-        case SnowflakeType::Type::MAP:
-        case SnowflakeType::Type::OBJECT:
-        case SnowflakeType::Type::REAL:
-        case SnowflakeType::Type::TEXT:
-        case SnowflakeType::Type::VARIANT:
-        case SnowflakeType::Type::VECTOR: {
-          // Do not need to convert
-          break;
-        }
-
-        case SnowflakeType::Type::TIME: {
-          int scale = 9;
-          if (metadata != nullptr) {
-            struct ArrowStringView scaleString = ArrowCharView(nullptr);
-            returnCode = ArrowMetadataGetValue(metadata, ArrowCharView("scale"),
-                                               &scaleString);
-            SF_CHECK_ARROW_RC(returnCode,
-                              "[Snowflake Exception] error getting 'scale' "
-                              "from Arrow metadata, error code: %d",
-                              returnCode);
-            scale = std::stoi(
-                std::string(scaleString.data, scaleString.size_bytes));
-          }
-
-          convertTimeColumn_nanoarrow(batchIdx, colIdx, &columnSchemaView,
-                                      columnArray, scale);
-          break;
-        }
-
-        case SnowflakeType::Type::TIMESTAMP_NTZ: {
-          int scale = 9;
-          if (metadata != nullptr) {
-            struct ArrowStringView scaleString = ArrowCharView(nullptr);
-            returnCode = ArrowMetadataGetValue(metadata, ArrowCharView("scale"),
-                                               &scaleString);
-            SF_CHECK_ARROW_RC(returnCode,
-                              "[Snowflake Exception] error getting 'scale' "
-                              "from Arrow metadata, error code: %d",
-                              returnCode);
-            scale = std::stoi(
-                std::string(scaleString.data, scaleString.size_bytes));
-          }
-          convertTimestampColumn_nanoarrow(batchIdx, colIdx, &columnSchemaView,
-                                           columnArray, scale);
-          break;
-        }
-
-        case SnowflakeType::Type::TIMESTAMP_LTZ: {
-          int scale = 9;
-          if (metadata != nullptr) {
-            struct ArrowStringView scaleString = ArrowCharView(nullptr);
-            returnCode = ArrowMetadataGetValue(metadata, ArrowCharView("scale"),
-                                               &scaleString);
-            SF_CHECK_ARROW_RC(returnCode,
-                              "[Snowflake Exception] error getting 'scale' "
-                              "from Arrow metadata, error code: %d",
-                              returnCode);
-            scale = std::stoi(
-                std::string(scaleString.data, scaleString.size_bytes));
-          }
-
-          convertTimestampColumn_nanoarrow(batchIdx, colIdx, &columnSchemaView,
-                                           columnArray, scale, m_timezone);
-          break;
-        }
-
-        case SnowflakeType::Type::TIMESTAMP_TZ: {
-          struct ArrowStringView scaleString = ArrowCharView(nullptr);
-          struct ArrowStringView byteLengthString = ArrowCharView(nullptr);
-          int scale = 9;
-          int byteLength = 16;
-          if (metadata != nullptr) {
-            returnCode = ArrowMetadataGetValue(metadata, ArrowCharView("scale"),
-                                               &scaleString);
-            SF_CHECK_ARROW_RC(returnCode,
-                              "[Snowflake Exception] error getting 'scale' "
-                              "from Arrow metadata, error code: %d",
-                              returnCode);
-            returnCode = ArrowMetadataGetValue(
-                metadata, ArrowCharView("byteLength"), &byteLengthString);
-            SF_CHECK_ARROW_RC(
-                returnCode,
-                "[Snowflake Exception] error getting 'byteLength' from Arrow "
-                "metadata, error code: %d",
-                returnCode);
-            scale = std::stoi(
-                std::string(scaleString.data, scaleString.size_bytes));
-            byteLength = std::stoi(std::string(byteLengthString.data,
-                                               byteLengthString.size_bytes));
-          }
-
-          convertTimestampTZColumn_nanoarrow(batchIdx, colIdx,
-                                             &columnSchemaView, columnArray,
-                                             scale, byteLength, m_timezone);
-          break;
-        }
-
-        default: {
-          std::string errorInfo = Logger::formatString(
-              "[Snowflake Exception] unknown snowflake data type : %s",
-              snowflakeLogicalType.data);
-          logger->error(__FILE__, __func__, __LINE__, errorInfo.c_str());
-          PyErr_SetString(PyExc_Exception, errorInfo.c_str());
-          return;
-        }
-      }
+      convertIfNeeded(columnSchema, columnArray);
     }
     m_tableConverted = true;
   }
 }
 
 CArrowTableIterator::CArrowTableIterator(PyObject* context, char* arrow_bytes,
                                          int64_t arrow_bytes_size,
@@ -264,30 +361,30 @@
     valStr.insert(valStr.length() - scale, ".");
     std::size_t offset = 0;
     return std::stod(valStr, &offset);
   }
 }
 
 void CArrowTableIterator::convertScaledFixedNumberColumn_nanoarrow(
-    const unsigned int batchIdx, const int colIdx, ArrowSchemaView* field,
-    ArrowArrayView* columnArray, const unsigned int scale) {
+    ArrowSchemaView* field, ArrowArrayView* columnArray,
+    const unsigned int scale) {
   // Convert scaled fixed number to either Double, or Decimal based on setting
   if (m_convert_number_to_decimal) {
-    convertScaledFixedNumberColumnToDecimalColumn_nanoarrow(
-        batchIdx, colIdx, field, columnArray, scale);
+    convertScaledFixedNumberColumnToDecimalColumn_nanoarrow(field, columnArray,
+                                                            scale);
   } else {
-    convertScaledFixedNumberColumnToDoubleColumn_nanoarrow(
-        batchIdx, colIdx, field, columnArray, scale);
+    convertScaledFixedNumberColumnToDoubleColumn_nanoarrow(field, columnArray,
+                                                           scale);
   }
 }
 
 void CArrowTableIterator::
     convertScaledFixedNumberColumnToDecimalColumn_nanoarrow(
-        const unsigned int batchIdx, const int colIdx, ArrowSchemaView* field,
-        ArrowArrayView* columnArray, const unsigned int scale) {
+        ArrowSchemaView* field, ArrowArrayView* columnArray,
+        const unsigned int scale) {
   int returnCode = 0;
   // Convert to arrow double/float64 column
   nanoarrow::UniqueSchema newUniqueField;
   nanoarrow::UniqueArray newUniqueArray;
   ArrowSchema* newSchema = newUniqueField.get();
   ArrowArray* newArray = newUniqueArray.get();
 
@@ -340,28 +437,24 @@
     }
   }
   returnCode = ArrowArrayFinishBuildingDefault(newArray, &error);
   SF_CHECK_ARROW_RC(returnCode,
                     "[Snowflake Exception] error finishing building arrow "
                     "array: %s, error code: %d",
                     ArrowErrorMessage(&error), returnCode);
-  m_ipcSchemaArrayVec[batchIdx]->children[colIdx]->release(
-      m_ipcSchemaArrayVec[batchIdx]->children[colIdx]);
-  ArrowSchemaMove(newSchema, m_ipcSchemaArrayVec[batchIdx]->children[colIdx]);
-  m_ipcArrowArrayVec[batchIdx]->children[colIdx]->release(
-      m_ipcArrowArrayVec[batchIdx]->children[colIdx]);
-  ArrowArrayMove(newArray, m_ipcArrowArrayVec[batchIdx]->children[colIdx]);
-  m_newArrays[batchIdx].push_back(std::move(newUniqueArray));
-  m_newSchemas[batchIdx].push_back(std::move(newUniqueField));
+  field->schema->release(field->schema);
+  ArrowSchemaMove(newSchema, field->schema);
+  columnArray->array->release(columnArray->array);
+  ArrowArrayMove(newArray, columnArray->array);
 }
 
 void CArrowTableIterator::
     convertScaledFixedNumberColumnToDoubleColumn_nanoarrow(
-        const unsigned int batchIdx, const int colIdx, ArrowSchemaView* field,
-        ArrowArrayView* columnArray, const unsigned int scale) {
+        ArrowSchemaView* field, ArrowArrayView* columnArray,
+        const unsigned int scale) {
   int returnCode = 0;
   // Convert to arrow double/float64 column
   nanoarrow::UniqueSchema newUniqueField;
   nanoarrow::UniqueArray newUniqueArray;
   ArrowSchema* newSchema = newUniqueField.get();
   ArrowArray* newArray = newUniqueArray.get();
 
@@ -406,27 +499,22 @@
     }
   }
   returnCode = ArrowArrayFinishBuildingDefault(newArray, &error);
   SF_CHECK_ARROW_RC(returnCode,
                     "[Snowflake Exception] error finishing building arrow "
                     "array: %s, error code: %d",
                     ArrowErrorMessage(&error), returnCode);
-  m_ipcSchemaArrayVec[batchIdx]->children[colIdx]->release(
-      m_ipcSchemaArrayVec[batchIdx]->children[colIdx]);
-  ArrowSchemaMove(newSchema, m_ipcSchemaArrayVec[batchIdx]->children[colIdx]);
-  m_ipcArrowArrayVec[batchIdx]->children[colIdx]->release(
-      m_ipcArrowArrayVec[batchIdx]->children[colIdx]);
-  ArrowArrayMove(newArray, m_ipcArrowArrayVec[batchIdx]->children[colIdx]);
-  m_newArrays[batchIdx].push_back(std::move(newUniqueArray));
-  m_newSchemas[batchIdx].push_back(std::move(newUniqueField));
+  field->schema->release(field->schema);
+  ArrowSchemaMove(newSchema, field->schema);
+  columnArray->array->release(columnArray->array);
+  ArrowArrayMove(newArray, columnArray->array);
 }
 
 void CArrowTableIterator::convertTimeColumn_nanoarrow(
-    const unsigned int batchIdx, const int colIdx, ArrowSchemaView* field,
-    ArrowArrayView* columnArray, const int scale) {
+    ArrowSchemaView* field, ArrowArrayView* columnArray, const int scale) {
   int returnCode = 0;
   nanoarrow::UniqueSchema newUniqueField;
   nanoarrow::UniqueArray newUniqueArray;
   ArrowSchema* newSchema = newUniqueField.get();
   ArrowArray* newArray = newUniqueArray.get();
   ArrowError error;
 
@@ -508,27 +596,23 @@
   }
 
   returnCode = ArrowArrayFinishBuildingDefault(newArray, &error);
   SF_CHECK_ARROW_RC(returnCode,
                     "[Snowflake Exception] error finishing building arrow "
                     "array: %s, error code: %d",
                     ArrowErrorMessage(&error), returnCode);
-  m_ipcSchemaArrayVec[batchIdx]->children[colIdx]->release(
-      m_ipcSchemaArrayVec[batchIdx]->children[colIdx]);
-  ArrowSchemaMove(newSchema, m_ipcSchemaArrayVec[batchIdx]->children[colIdx]);
-  m_ipcArrowArrayVec[batchIdx]->children[colIdx]->release(
-      m_ipcArrowArrayVec[batchIdx]->children[colIdx]);
-  ArrowArrayMove(newArray, m_ipcArrowArrayVec[batchIdx]->children[colIdx]);
-  m_newArrays[batchIdx].push_back(std::move(newUniqueArray));
-  m_newSchemas[batchIdx].push_back(std::move(newUniqueField));
+  field->schema->release(field->schema);
+  ArrowSchemaMove(newSchema, field->schema);
+  columnArray->array->release(columnArray->array);
+  ArrowArrayMove(newArray, columnArray->array);
 }
 
 void CArrowTableIterator::convertTimestampColumn_nanoarrow(
-    const unsigned int batchIdx, const int colIdx, ArrowSchemaView* field,
-    ArrowArrayView* columnArray, const int scale, const std::string timezone) {
+    ArrowSchemaView* field, ArrowArrayView* columnArray, const int scale,
+    const std::string timezone) {
   int returnCode = 0;
   nanoarrow::UniqueSchema newUniqueField;
   nanoarrow::UniqueArray newUniqueArray;
   ArrowSchema* newSchema = newUniqueField.get();
   ArrowArray* newArray = newUniqueArray.get();
   ArrowError error;
 
@@ -755,28 +839,23 @@
   }
 
   returnCode = ArrowArrayFinishBuildingDefault(newArray, &error);
   SF_CHECK_ARROW_RC(returnCode,
                     "[Snowflake Exception] error finishing building arrow "
                     "array: %s, error code: %d",
                     ArrowErrorMessage(&error), returnCode);
-  m_ipcSchemaArrayVec[batchIdx]->children[colIdx]->release(
-      m_ipcSchemaArrayVec[batchIdx]->children[colIdx]);
-  ArrowSchemaMove(newSchema, m_ipcSchemaArrayVec[batchIdx]->children[colIdx]);
-  m_ipcArrowArrayVec[batchIdx]->children[colIdx]->release(
-      m_ipcArrowArrayVec[batchIdx]->children[colIdx]);
-  ArrowArrayMove(newArray, m_ipcArrowArrayVec[batchIdx]->children[colIdx]);
-  m_newArrays[batchIdx].push_back(std::move(newUniqueArray));
-  m_newSchemas[batchIdx].push_back(std::move(newUniqueField));
+  field->schema->release(field->schema);
+  ArrowSchemaMove(newSchema, field->schema);
+  columnArray->array->release(columnArray->array);
+  ArrowArrayMove(newArray, columnArray->array);
 }
 
 void CArrowTableIterator::convertTimestampTZColumn_nanoarrow(
-    const unsigned int batchIdx, const int colIdx, ArrowSchemaView* field,
-    ArrowArrayView* columnArray, const int scale, const int byteLength,
-    const std::string timezone) {
+    ArrowSchemaView* field, ArrowArrayView* columnArray, const int scale,
+    const int byteLength, const std::string timezone) {
   int returnCode = 0;
   nanoarrow::UniqueSchema newUniqueField;
   nanoarrow::UniqueArray newUniqueArray;
   ArrowSchema* newSchema = newUniqueField.get();
   ArrowArray* newArray = newUniqueArray.get();
   ArrowError error;
   ArrowSchemaInit(newSchema);
@@ -836,73 +915,49 @@
 
   for (int64_t rowIdx = 0; rowIdx < columnArray->array->length; rowIdx++) {
     if (!ArrowArrayViewIsNull(columnArray, rowIdx)) {
       if (byteLength == 8) {
         int64_t epoch = ArrowArrayViewGetIntUnsafe(epochArray, rowIdx);
         if (scale == 0) {
           returnCode = ArrowArrayAppendInt(newArray, epoch);
-          SF_CHECK_ARROW_RC(returnCode,
-                            "[Snowflake Exception] error appending int to "
-                            "arrow array, error code: %d",
-                            returnCode);
         } else if (scale <= 3) {
           returnCode = ArrowArrayAppendInt(
               newArray, epoch * sf::internal::powTenSB4[3 - scale]);
-          SF_CHECK_ARROW_RC(returnCode,
-                            "[Snowflake Exception] error appending int to "
-                            "arrow array, error code: %d",
-                            returnCode);
         } else if (scale <= 6) {
           returnCode = ArrowArrayAppendInt(
               newArray, epoch * sf::internal::powTenSB4[6 - scale]);
-          SF_CHECK_ARROW_RC(returnCode,
-                            "[Snowflake Exception] error appending int to "
-                            "arrow array, error code: %d",
-                            returnCode);
         } else {
           returnCode = ArrowArrayAppendInt(
               newArray, epoch * sf::internal::powTenSB4[9 - scale]);
-          SF_CHECK_ARROW_RC(returnCode,
-                            "[Snowflake Exception] error appending int to "
-                            "arrow array, error code: %d",
-                            returnCode);
         }
+        SF_CHECK_ARROW_RC(returnCode,
+                          "[Snowflake Exception] error appending int to "
+                          "arrow array, error code: %d",
+                          returnCode);
       } else if (byteLength == 16) {
         int64_t epoch = ArrowArrayViewGetIntUnsafe(epochArray, rowIdx);
         int64_t fraction = ArrowArrayViewGetIntUnsafe(fractionArray, rowIdx);
         if (scale == 0) {
           returnCode = ArrowArrayAppendInt(newArray, epoch);
-          SF_CHECK_ARROW_RC(returnCode,
-                            "[Snowflake Exception] error appending int to "
-                            "arrow array, error code: %d",
-                            returnCode);
         } else if (scale <= 3) {
           returnCode = ArrowArrayAppendInt(
               newArray, epoch * sf::internal::powTenSB4[3 - scale] +
                             fraction / sf::internal::powTenSB4[6]);
-          SF_CHECK_ARROW_RC(returnCode,
-                            "[Snowflake Exception] error appending int to "
-                            "arrow array, error code: %d",
-                            returnCode);
         } else if (scale <= 6) {
           returnCode = ArrowArrayAppendInt(
               newArray, epoch * sf::internal::powTenSB4[6] +
                             fraction / sf::internal::powTenSB4[3]);
-          SF_CHECK_ARROW_RC(returnCode,
-                            "[Snowflake Exception] error appending int to "
-                            "arrow array, error code: %d",
-                            returnCode);
         } else {
           returnCode = ArrowArrayAppendInt(
               newArray, epoch * sf::internal::powTenSB4[9] + fraction);
-          SF_CHECK_ARROW_RC(returnCode,
-                            "[Snowflake Exception] error appending int to "
-                            "arrow array, error code: %d",
-                            returnCode);
         }
+        SF_CHECK_ARROW_RC(returnCode,
+                          "[Snowflake Exception] error appending int to "
+                          "arrow array, error code: %d",
+                          returnCode);
       } else {
         std::string errorInfo = Logger::formatString(
             "[Snowflake Exception] unknown arrow internal data type(%d) "
             "for TIMESTAMP_TZ data",
             NANOARROW_TYPE_ENUM_STRING[field->type]);
         logger->error(__FILE__, __func__, __LINE__, errorInfo.c_str());
         PyErr_SetString(PyExc_Exception, errorInfo.c_str());
@@ -918,22 +973,18 @@
   }
 
   returnCode = ArrowArrayFinishBuildingDefault(newArray, &error);
   SF_CHECK_ARROW_RC(returnCode,
                     "[Snowflake Exception] error finishing building arrow "
                     "array: %s, error code: %d",
                     ArrowErrorMessage(&error), returnCode);
-  m_ipcSchemaArrayVec[batchIdx]->children[colIdx]->release(
-      m_ipcSchemaArrayVec[batchIdx]->children[colIdx]);
-  ArrowSchemaMove(newSchema, m_ipcSchemaArrayVec[batchIdx]->children[colIdx]);
-  m_ipcArrowArrayVec[batchIdx]->children[colIdx]->release(
-      m_ipcArrowArrayVec[batchIdx]->children[colIdx]);
-  ArrowArrayMove(newArray, m_ipcArrowArrayVec[batchIdx]->children[colIdx]);
-  m_newArrays[batchIdx].push_back(std::move(newUniqueArray));
-  m_newSchemas[batchIdx].push_back(std::move(newUniqueField));
+  field->schema->release(field->schema);
+  ArrowSchemaMove(newSchema, field->schema);
+  columnArray->array->release(columnArray->array);
+  ArrowArrayMove(newArray, columnArray->array);
 }
 
 bool CArrowTableIterator::convertRecordBatchesToTable_nanoarrow() {
   // only do conversion once and there exist some record batches
   if (!m_tableConverted && m_ipcArrowArrayViewVec.size() > 0) {
     reconstructRecordBatches_nanoarrow();
     return true;
```

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/CArrowTableIterator.hpp` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/CArrowTableIterator.hpp`

 * *Files 17% similar despite different names*

```diff
@@ -22,15 +22,14 @@
  * record batches and build a new table.
  */
 class CArrowTableIterator : public CArrowIterator {
  public:
   /**
    * Constructor
    */
-
   CArrowTableIterator(PyObject* context, char* arrow_bytes,
                       int64_t arrow_bytes_size, bool number_to_decimal);
 
   /**
    * Destructor
    */
   ~CArrowTableIterator() = default;
@@ -40,16 +39,14 @@
    */
   ReturnVal next() override;
   std::vector<uintptr_t> getArrowArrayPtrs() override;
   std::vector<uintptr_t> getArrowSchemaPtrs() override;
 
  private:
   // nanoarrow data
-  std::vector<std::vector<nanoarrow::UniqueArray>> m_newArrays;
-  std::vector<std::vector<nanoarrow::UniqueSchema>> m_newSchemas;
   std::vector<nanoarrow::UniqueSchema> m_ipcSchemaArrayVec;
 
   bool m_tableConverted = false;
 
   /** arrow format convert context for the current session */
   PyObject* m_context;
 
@@ -57,76 +54,69 @@
   char* m_timezone;
   const bool m_convert_number_to_decimal;
 
   /**
    * Reconstruct record batches with type conversion in place
    */
   void reconstructRecordBatches();
-
+  void convertIfNeeded(ArrowSchema* columnSchema, ArrowArrayView* columnArray);
   void reconstructRecordBatches_nanoarrow();
 
   /**
    * Convert all current RecordBatches to Arrow Table
    * @return if conversion is executed at first time and successfully
    */
   bool convertRecordBatchesToTable_nanoarrow();
 
   /**
    * convert scaled fixed number column to Decimal, or Double column based on
    * setting
    */
-  void convertScaledFixedNumberColumn_nanoarrow(const unsigned int batchIdx,
-                                                const int colIdx,
-                                                ArrowSchemaView* field,
+  void convertScaledFixedNumberColumn_nanoarrow(ArrowSchemaView* field,
                                                 ArrowArrayView* columnArray,
                                                 const unsigned int scale);
 
   /**
    * convert scaled fixed number column to Decimal column
    */
   void convertScaledFixedNumberColumnToDecimalColumn_nanoarrow(
-      const unsigned int batchIdx, const int colIdx, ArrowSchemaView* field,
-      ArrowArrayView* columnArray, const unsigned int scale);
+      ArrowSchemaView* field, ArrowArrayView* columnArray,
+      const unsigned int scale);
 
   /**
    * convert scaled fixed number column to Double column
    */
   void convertScaledFixedNumberColumnToDoubleColumn_nanoarrow(
-      const unsigned int batchIdx, const int colIdx, ArrowSchemaView* field,
-      ArrowArrayView* columnArray, const unsigned int scale);
+      ArrowSchemaView* field, ArrowArrayView* columnArray,
+      const unsigned int scale);
 
   /**
    * convert Snowflake Time column (Arrow int32/int64) to Arrow Time column
    * Since Python/Pandas Time does not support nanoseconds, this function
    * truncates values to microseconds if necessary
    */
-  void convertTimeColumn_nanoarrow(const unsigned int batchIdx,
-                                   const int colIdx, ArrowSchemaView* field,
+  void convertTimeColumn_nanoarrow(ArrowSchemaView* field,
                                    ArrowArrayView* columnArray,
                                    const int scale);
 
   /**
    * convert Snowflake TimestampNTZ/TimestampLTZ column to Arrow Timestamp
    * column
    */
-  void convertTimestampColumn_nanoarrow(const unsigned int batchIdx,
-                                        const int colIdx,
-                                        ArrowSchemaView* field,
+  void convertTimestampColumn_nanoarrow(ArrowSchemaView* field,
                                         ArrowArrayView* columnArray,
                                         const int scale,
                                         const std::string timezone = "");
 
   /**
    * convert Snowflake TimestampTZ column to Arrow Timestamp column in UTC
    * Arrow Timestamp does not support time zone info in each value, so this
    * method convert TimestampTZ to Arrow timestamp with UTC timezone
    */
-  void convertTimestampTZColumn_nanoarrow(const unsigned int batchIdx,
-                                          const int colIdx,
-                                          ArrowSchemaView* field,
+  void convertTimestampTZColumn_nanoarrow(ArrowSchemaView* field,
                                           ArrowArrayView* columnArray,
                                           const int scale, const int byteLength,
                                           const std::string timezone);
 
   /**
    * convert scaled fixed number to double
    * if scale is small, then just divide based on the scale; otherwise, convert
```

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/DateConverter.cpp` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/DateConverter.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/DateConverter.hpp` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/DateConverter.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/DecimalConverter.cpp` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/DecimalConverter.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/DecimalConverter.hpp` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/DecimalConverter.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/FixedSizeListConverter.cpp` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/FixedSizeListConverter.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/FixedSizeListConverter.hpp` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/FixedSizeListConverter.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/FloatConverter.cpp` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/FloatConverter.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/FloatConverter.hpp` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/FloatConverter.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/IntConverter.cpp` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/IntConverter.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/IntConverter.hpp` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/IntConverter.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/LICENSE.txt` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/MapConverter.cpp` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/MapConverter.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/MapConverter.hpp` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/MapConverter.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/ObjectConverter.cpp` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/ObjectConverter.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/ObjectConverter.hpp` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/ObjectConverter.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/Python/Common.hpp` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/Python/Common.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/Python/Helpers.cpp` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/Python/Helpers.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/Python/Helpers.hpp` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/Python/Helpers.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/SnowflakeType.cpp` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/SnowflakeType.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/SnowflakeType.hpp` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/SnowflakeType.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/StringConverter.cpp` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/StringConverter.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/StringConverter.hpp` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/StringConverter.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/TimeConverter.cpp` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/TimeConverter.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/TimeConverter.hpp` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/TimeConverter.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/TimeStampConverter.cpp` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/TimeStampConverter.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/TimeStampConverter.hpp` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/TimeStampConverter.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/Util/time.cpp` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/Util/time.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/Util/time.hpp` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/Util/time.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_accessors.h` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_accessors.h`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_alloc.h` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_alloc.h`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_assert.h` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_assert.h`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_builder.h` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_builder.h`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_emitter.h` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_emitter.h`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_endian.h` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_endian.h`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_flatbuffers.h` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_flatbuffers.h`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_identifier.h` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_identifier.h`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_iov.h` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_iov.h`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_refmap.h` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_refmap.h`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_rtconfig.h` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_rtconfig.h`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_types.h` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_types.h`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_verifier.h` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/flatcc_verifier.h`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/paligned_alloc.h` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/paligned_alloc.h`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pattributes.h` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pattributes.h`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pdiagnostic.h` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pdiagnostic.h`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pdiagnostic_pop.h` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pdiagnostic_pop.h`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pdiagnostic_push.h` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pdiagnostic_push.h`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pendian.h` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pendian.h`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pendian_detect.h` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pendian_detect.h`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pinttypes.h` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pinttypes.h`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/portable_basic.h` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/portable_basic.h`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pstatic_assert.h` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pstatic_assert.h`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pstdalign.h` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pstdalign.h`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pstdint.h` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pstdint.h`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/punaligned.h` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/punaligned.h`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pwarnings.h` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc/portable/pwarnings.h`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc.c` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/flatcc.c`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/nanoarrow.c` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/nanoarrow.c`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/nanoarrow.h` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/nanoarrow.h`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/nanoarrow.hpp` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/nanoarrow.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/nanoarrow_arrow_iterator.pyx` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/nanoarrow_arrow_iterator.pyx`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/nanoarrow_device.c` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/nanoarrow_device.c`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/nanoarrow_device.h` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/nanoarrow_device.h`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/nanoarrow_ipc.c` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/nanoarrow_ipc.c`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/nanoarrow_ipc.h` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/ArrowIterator/nanoarrow_ipc.h`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/Logging/logging.cpp` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/Logging/logging.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/nanoarrow_cpp/Logging/logging.hpp` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/nanoarrow_cpp/Logging/logging.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/network.py` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/network.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/ocsp_asn1crypto.py` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/ocsp_asn1crypto.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/ocsp_snowflake.py` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/ocsp_snowflake.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/options.py` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/options.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/pandas_tools.py` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/pandas_tools.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/proxy.py` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/proxy.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/result_batch.py` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/result_batch.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/result_set.py` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/result_set.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/s3_storage_client.py` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/s3_storage_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,26 +76,34 @@
         self.etags: list[str] | None = None
         self.s3location: S3Location = (
             SnowflakeS3RestClient._extract_bucket_name_and_path(
                 self.stage_info["location"]
             )
         )
         self.use_s3_regional_url = use_s3_regional_url
+        self.location_type = stage_info.get("locationType")
 
         # if GS sends us an endpoint, it's likely for FIPS. Use it.
         self.endpoint: str | None = None
         if stage_info["endPoint"]:
             self.endpoint = (
                 f"https://{self.s3location.bucket_name}." + stage_info["endPoint"]
             )
         self.transfer_accelerate_config(use_accelerate_endpoint)
 
     def transfer_accelerate_config(
         self, use_accelerate_endpoint: bool | None = None
     ) -> bool:
+        # accelerate cannot be used in China and us government
+        if self.region_name and self.region_name.startswith("cn-"):
+            self.endpoint = (
+                f"https://{self.s3location.bucket_name}."
+                f"s3.{self.region_name}.amazonaws.com.cn"
+            )
+            return False
         # if self.endpoint has been set, e.g. by metadata, no more config is needed.
         if self.endpoint is not None:
             return self.endpoint.find("s3-accelerate.amazonaws.com") >= 0
         if self.use_s3_regional_url:
             self.endpoint = (
                 f"https://{self.s3location.bucket_name}."
                 f"s3.{self.region_name}.amazonaws.com"
```

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/secret_detector.py` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/secret_detector.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/sf_dirs.py` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/sf_dirs.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/sfbinaryformat.py` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/sfbinaryformat.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/sfdatetime.py` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/sfdatetime.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/snow_logging.py` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/snow_logging.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/ssd_internal_keys.py` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/ssd_internal_keys.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/ssl_wrap_socket.py` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/ssl_wrap_socket.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/storage_client.py` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/storage_client.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/telemetry.py` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/telemetry.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/telemetry_oob.py` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/telemetry_oob.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/test_util.py` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/test_util.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/time_util.py` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/time_util.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/tool/dump_certs.py` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/tool/dump_certs.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/tool/dump_ocsp_response.py` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/tool/dump_ocsp_response.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/tool/dump_ocsp_response_cache.py` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/tool/dump_ocsp_response_cache.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/tool/probe_connection.py` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/tool/probe_connection.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/url_util.py` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/url_util.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/util_text.py` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/util_text.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/requests/LICENSE` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/vendored/requests/LICENSE`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/requests/__init__.py` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/vendored/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/requests/_internal_utils.py` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/vendored/requests/_internal_utils.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/requests/adapters.py` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/vendored/requests/adapters.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/requests/api.py` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/vendored/requests/api.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/requests/auth.py` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/vendored/requests/auth.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/requests/compat.py` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/vendored/requests/compat.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/requests/cookies.py` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/vendored/requests/cookies.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/requests/exceptions.py` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/vendored/requests/exceptions.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/requests/help.py` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/vendored/requests/help.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/requests/hooks.py` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/vendored/requests/hooks.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/requests/models.py` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/vendored/requests/models.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/requests/sessions.py` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/vendored/requests/sessions.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/requests/status_codes.py` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/vendored/requests/status_codes.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/requests/structures.py` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/vendored/requests/structures.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/requests/utils.py` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/vendored/requests/utils.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/LICENSE.txt` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/vendored/urllib3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/__init__.py` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/vendored/urllib3/__init__.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/_collections.py` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/vendored/urllib3/_collections.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/connection.py` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/vendored/urllib3/connection.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/connectionpool.py` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/vendored/urllib3/connectionpool.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/contrib/_appengine_environ.py` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/vendored/urllib3/contrib/_appengine_environ.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/bindings.py` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/bindings.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/low_level.py` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/low_level.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/contrib/appengine.py` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/vendored/urllib3/contrib/appengine.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/contrib/ntlmpool.py` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/vendored/urllib3/contrib/ntlmpool.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/contrib/pyopenssl.py` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/vendored/urllib3/contrib/pyopenssl.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/contrib/securetransport.py` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/vendored/urllib3/contrib/securetransport.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/contrib/socks.py` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/vendored/urllib3/contrib/socks.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/exceptions.py` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/vendored/urllib3/exceptions.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/fields.py` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/vendored/urllib3/fields.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/filepost.py` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/vendored/urllib3/filepost.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/packages/backports/makefile.py` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/vendored/urllib3/packages/backports/makefile.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/packages/backports/weakref_finalize.py` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/vendored/urllib3/packages/backports/weakref_finalize.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/packages/six.py` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/vendored/urllib3/packages/six.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/poolmanager.py` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/vendored/urllib3/poolmanager.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/request.py` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/vendored/urllib3/request.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/response.py` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/vendored/urllib3/response.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/util/__init__.py` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/vendored/urllib3/util/__init__.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/util/connection.py` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/vendored/urllib3/util/connection.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/util/proxy.py` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/vendored/urllib3/util/proxy.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/util/request.py` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/vendored/urllib3/util/request.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/util/response.py` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/vendored/urllib3/util/response.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/util/retry.py` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/vendored/urllib3/util/retry.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/util/ssl_.py` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/vendored/urllib3/util/ssl_.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/util/ssl_match_hostname.py` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/vendored/urllib3/util/ssl_match_hostname.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/util/ssltransport.py` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/vendored/urllib3/util/ssltransport.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/util/timeout.py` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/vendored/urllib3/util/timeout.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/util/url.py` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/vendored/urllib3/util/url.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake/connector/vendored/urllib3/util/wait.py` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake/connector/vendored/urllib3/util/wait.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake_connector_python_nightly.egg-info/PKG-INFO` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake_connector_python_nightly.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snowflake-connector-python-nightly
-Version: 2024.4.9
+Version: 2024.5.10
 Summary: Nigthly build of Snowflake Connector for Python
 Home-page: https://www.snowflake.com/
 Author: Snowflake, Inc
 Author-email: snowflake-python-libraries-dl@snowflake.com
 License: Apache-2.0
 Project-URL: Documentation, https://docs.snowflake.com/en/user-guide/python-connector.html
 Project-URL: Source, https://github.com/keller00/snowflake-connector-python-nightlies/
```

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake_connector_python_nightly.egg-info/SOURCES.txt` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake_connector_python_nightly.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 src/snowflake/connector/feature.py
 src/snowflake/connector/file_compression_type.py
 src/snowflake/connector/file_transfer_agent.py
 src/snowflake/connector/file_util.py
 src/snowflake/connector/gcs_storage_client.py
 src/snowflake/connector/gzip_decoder.py
 src/snowflake/connector/local_storage_client.py
+src/snowflake/connector/log_configuration.py
 src/snowflake/connector/network.py
 src/snowflake/connector/ocsp_asn1crypto.py
 src/snowflake/connector/ocsp_snowflake.py
 src/snowflake/connector/options.py
 src/snowflake/connector/pandas_tools.py
 src/snowflake/connector/proxy.py
 src/snowflake/connector/py.typed
```

### Comparing `snowflake-connector-python-nightly-2024.4.9/src/snowflake_connector_python_nightly.egg-info/requires.txt` & `snowflake_connector_python_nightly-2024.5.10/src/snowflake_connector_python_nightly.egg-info/requires.txt`

 * *Files identical despite different names*

