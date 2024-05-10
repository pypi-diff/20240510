# Comparing `tmp/redshift_client-5.1.0.tar.gz` & `tmp/redshift_client-5.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redshift_client-5.1.0.tar", last modified: Tue Jan  1 00:00:00 1980, max compression
+gzip compressed data, was "redshift_client-5.1.1.tar", last modified: Tue Jan  1 00:00:00 1980, max compression
```

## Comparing `redshift_client-5.1.0.tar` & `redshift_client-5.1.1.tar`

### file list

```diff
@@ -1,66 +1,66 @@
--rw-r--r--   0        0        0       84 1980-01-01 00:00:00.000000 redshift_client-5.1.0/.envrc
--rw-r--r--   0        0        0       47 1980-01-01 00:00:00.000000 redshift_client-5.1.0/.gitignore
--rw-r--r--   0        0        0     1798 1980-01-01 00:00:00.000000 redshift_client-5.1.0/.gitlab-ci.yml
--rw-r--r--   0        0        0      314 1980-01-01 00:00:00.000000 redshift_client-5.1.0/.pylintrc
--rw-r--r--   0        0        0      262 1980-01-01 00:00:00.000000 redshift_client-5.1.0/build/ci/check.nix
--rw-r--r--   0        0        0      191 1980-01-01 00:00:00.000000 redshift_client-5.1.0/build/ci/utils.sh
--rw-r--r--   0        0        0     1368 1980-01-01 00:00:00.000000 redshift_client-5.1.0/build/default.nix
--rw-r--r--   0        0        0      645 1980-01-01 00:00:00.000000 redshift_client-5.1.0/build/deps/arch_lint.nix
--rw-r--r--   0        0        0      345 1980-01-01 00:00:00.000000 redshift_client-5.1.0/build/deps/boto3/redshift-stubs.nix
--rw-r--r--   0        0        0      844 1980-01-01 00:00:00.000000 redshift_client-5.1.0/build/deps/boto3/stubs.nix
--rw-r--r--   0        0        0     1157 1980-01-01 00:00:00.000000 redshift_client-5.1.0/build/deps/default.nix
--rw-r--r--   0        0        0      653 1980-01-01 00:00:00.000000 redshift_client-5.1.0/build/deps/fa_purity.nix
--rw-r--r--   0        0        0      206 1980-01-01 00:00:00.000000 redshift_client-5.1.0/build/deps/psycopg2/stubs.nix
--rw-r--r--   0        0        0      182 1980-01-01 00:00:00.000000 redshift_client-5.1.0/build/dev_env/default.nix
--rwxr-xr-x   0        0        0      131 1980-01-01 00:00:00.000000 redshift_client-5.1.0/build/dev_env/hook.sh
--rw-r--r--   0        0        0     1482 1980-01-01 00:00:00.000000 redshift_client-5.1.0/build/dev_env/vs_settings.py
--rw-r--r--   0        0        0      310 1980-01-01 00:00:00.000000 redshift_client-5.1.0/build/filter.nix
--rw-r--r--   0        0        0     1913 1980-01-01 00:00:00.000000 redshift_client-5.1.0/flake.lock
--rw-r--r--   0        0        0     1140 1980-01-01 00:00:00.000000 redshift_client-5.1.0/flake.nix
--rw-r--r--   0        0        0      281 1980-01-01 00:00:00.000000 redshift_client-5.1.0/makes.lock.nix
--rw-r--r--   0        0        0      680 1980-01-01 00:00:00.000000 redshift_client-5.1.0/makes.nix
--rw-r--r--   0        0        0      714 1980-01-01 00:00:00.000000 redshift_client-5.1.0/mypy.ini
--rw-r--r--   0        0        0      260 1980-01-01 00:00:00.000000 redshift_client-5.1.0/nix.conf
--rw-r--r--   0        0        0      667 1980-01-01 00:00:00.000000 redshift_client-5.1.0/pyproject.toml
--rw-r--r--   0        0        0      112 1980-01-01 00:00:00.000000 redshift_client-5.1.0/redshift_client/__init__.py
--rw-r--r--   0        0        0     2996 1980-01-01 00:00:00.000000 redshift_client-5.1.0/redshift_client/_utils.py
--rw-r--r--   0        0        0      336 1980-01-01 00:00:00.000000 redshift_client-5.1.0/redshift_client/client/__init__.py
--rw-r--r--   0        0        0     6335 1980-01-01 00:00:00.000000 redshift_client-5.1.0/redshift_client/client/_core.py
--rw-r--r--   0        0        0      941 1980-01-01 00:00:00.000000 redshift_client-5.1.0/redshift_client/client/_factory.py
--rw-r--r--   0        0        0      864 1980-01-01 00:00:00.000000 redshift_client-5.1.0/redshift_client/client/_schema/__init__.py
--rw-r--r--   0        0        0     7451 1980-01-01 00:00:00.000000 redshift_client-5.1.0/redshift_client/client/_schema/_methods.py
--rw-r--r--   0        0        0     1120 1980-01-01 00:00:00.000000 redshift_client-5.1.0/redshift_client/client/_table/__init__.py
--rw-r--r--   0        0        0     2160 1980-01-01 00:00:00.000000 redshift_client-5.1.0/redshift_client/client/_table/_assert.py
--rw-r--r--   0        0        0      283 1980-01-01 00:00:00.000000 redshift_client-5.1.0/redshift_client/client/_table/_encode.py
--rw-r--r--   0        0        0    12271 1980-01-01 00:00:00.000000 redshift_client-5.1.0/redshift_client/client/_table/_methods.py
--rw-r--r--   0        0        0     1922 1980-01-01 00:00:00.000000 redshift_client-5.1.0/redshift_client/client/_table/_new.py
--rw-r--r--   0        0        0        0 1980-01-01 00:00:00.000000 redshift_client-5.1.0/redshift_client/core/__init__.py
--rw-r--r--   0        0        0      496 1980-01-01 00:00:00.000000 redshift_client-5.1.0/redshift_client/core/column.py
--rw-r--r--   0        0        0        0 1980-01-01 00:00:00.000000 redshift_client-5.1.0/redshift_client/core/data_type/__init__.py
--rw-r--r--   0        0        0     1589 1980-01-01 00:00:00.000000 redshift_client-5.1.0/redshift_client/core/data_type/alias.py
--rw-r--r--   0        0        0     1585 1980-01-01 00:00:00.000000 redshift_client-5.1.0/redshift_client/core/data_type/core.py
--rw-r--r--   0        0        0     1565 1980-01-01 00:00:00.000000 redshift_client-5.1.0/redshift_client/core/data_type/decode.py
--rw-r--r--   0        0        0      843 1980-01-01 00:00:00.000000 redshift_client-5.1.0/redshift_client/core/id_objs.py
--rw-r--r--   0        0        0      589 1980-01-01 00:00:00.000000 redshift_client-5.1.0/redshift_client/core/schema.py
--rw-r--r--   0        0        0     6793 1980-01-01 00:00:00.000000 redshift_client-5.1.0/redshift_client/core/table.py
--rw-r--r--   0        0        0        0 1980-01-01 00:00:00.000000 redshift_client-5.1.0/redshift_client/py.typed
--rw-r--r--   0        0        0      751 1980-01-01 00:00:00.000000 redshift_client-5.1.0/redshift_client/sql_client/__init__.py
--rw-r--r--   0        0        0     8811 1980-01-01 00:00:00.000000 redshift_client-5.1.0/redshift_client/sql_client/_client_1/__init__.py
--rw-r--r--   0        0        0     1295 1980-01-01 00:00:00.000000 redshift_client-5.1.0/redshift_client/sql_client/_client_1/_assert.py
--rw-r--r--   0        0        0        0 1980-01-01 00:00:00.000000 redshift_client-5.1.0/redshift_client/sql_client/_core/__init__.py
--rw-r--r--   0        0        0     1167 1980-01-01 00:00:00.000000 redshift_client-5.1.0/redshift_client/sql_client/_core/client.py
--rw-r--r--   0        0        0     3164 1980-01-01 00:00:00.000000 redshift_client-5.1.0/redshift_client/sql_client/_core/connection.py
--rw-r--r--   0        0        0      283 1980-01-01 00:00:00.000000 redshift_client-5.1.0/redshift_client/sql_client/_core/creds.py
--rw-r--r--   0        0        0     2624 1980-01-01 00:00:00.000000 redshift_client-5.1.0/redshift_client/sql_client/_core/primitive.py
--rw-r--r--   0        0        0     1029 1980-01-01 00:00:00.000000 redshift_client-5.1.0/redshift_client/sql_client/_core/query.py
--rw-r--r--   0        0        0      833 1980-01-01 00:00:00.000000 redshift_client-5.1.0/redshift_client/sql_client/_factory.py
--rw-r--r--   0        0        0     1801 1980-01-01 00:00:00.000000 redshift_client-5.1.0/redshift_client/sql_client/_temp_creds.py
--rw-r--r--   0        0        0        0 1980-01-01 00:00:00.000000 redshift_client-5.1.0/tests/__init__.py
--rw-r--r--   0        0        0        0 1980-01-01 00:00:00.000000 redshift_client-5.1.0/tests/arch/__init__.py
--rw-r--r--   0        0        0     1858 1980-01-01 00:00:00.000000 redshift_client-5.1.0/tests/arch/arch.py
--rw-r--r--   0        0        0     1055 1980-01-01 00:00:00.000000 redshift_client-5.1.0/tests/arch/test_arch.py
--rw-r--r--   0        0        0        0 1980-01-01 00:00:00.000000 redshift_client-5.1.0/tests/py.typed
--rw-r--r--   0        0        0      233 1980-01-01 00:00:00.000000 redshift_client-5.1.0/tests/test_column.py
--rw-r--r--   0        0        0     1618 1980-01-01 00:00:00.000000 redshift_client-5.1.0/tests/test_table.py
--rw-r--r--   0        0        0      462 1980-01-01 00:00:00.000000 redshift_client-5.1.0/tests/test_temp_creds.py
--rw-r--r--   0        0        0      579 1970-01-01 00:00:00.000000 redshift_client-5.1.0/PKG-INFO
+-rw-r--r--   0        0        0       84 1980-01-01 00:00:00.000000 redshift_client-5.1.1/.envrc
+-rw-r--r--   0        0        0       47 1980-01-01 00:00:00.000000 redshift_client-5.1.1/.gitignore
+-rw-r--r--   0        0        0     1798 1980-01-01 00:00:00.000000 redshift_client-5.1.1/.gitlab-ci.yml
+-rw-r--r--   0        0        0      314 1980-01-01 00:00:00.000000 redshift_client-5.1.1/.pylintrc
+-rw-r--r--   0        0        0      262 1980-01-01 00:00:00.000000 redshift_client-5.1.1/build/ci/check.nix
+-rw-r--r--   0        0        0      191 1980-01-01 00:00:00.000000 redshift_client-5.1.1/build/ci/utils.sh
+-rw-r--r--   0        0        0     1368 1980-01-01 00:00:00.000000 redshift_client-5.1.1/build/default.nix
+-rw-r--r--   0        0        0      645 1980-01-01 00:00:00.000000 redshift_client-5.1.1/build/deps/arch_lint.nix
+-rw-r--r--   0        0        0      345 1980-01-01 00:00:00.000000 redshift_client-5.1.1/build/deps/boto3/redshift-stubs.nix
+-rw-r--r--   0        0        0      844 1980-01-01 00:00:00.000000 redshift_client-5.1.1/build/deps/boto3/stubs.nix
+-rw-r--r--   0        0        0     1157 1980-01-01 00:00:00.000000 redshift_client-5.1.1/build/deps/default.nix
+-rw-r--r--   0        0        0      653 1980-01-01 00:00:00.000000 redshift_client-5.1.1/build/deps/fa_purity.nix
+-rw-r--r--   0        0        0      206 1980-01-01 00:00:00.000000 redshift_client-5.1.1/build/deps/psycopg2/stubs.nix
+-rw-r--r--   0        0        0      182 1980-01-01 00:00:00.000000 redshift_client-5.1.1/build/dev_env/default.nix
+-rwxr-xr-x   0        0        0      131 1980-01-01 00:00:00.000000 redshift_client-5.1.1/build/dev_env/hook.sh
+-rw-r--r--   0        0        0     1482 1980-01-01 00:00:00.000000 redshift_client-5.1.1/build/dev_env/vs_settings.py
+-rw-r--r--   0        0        0      310 1980-01-01 00:00:00.000000 redshift_client-5.1.1/build/filter.nix
+-rw-r--r--   0        0        0     1913 1980-01-01 00:00:00.000000 redshift_client-5.1.1/flake.lock
+-rw-r--r--   0        0        0     1140 1980-01-01 00:00:00.000000 redshift_client-5.1.1/flake.nix
+-rw-r--r--   0        0        0      281 1980-01-01 00:00:00.000000 redshift_client-5.1.1/makes.lock.nix
+-rw-r--r--   0        0        0      680 1980-01-01 00:00:00.000000 redshift_client-5.1.1/makes.nix
+-rw-r--r--   0        0        0      714 1980-01-01 00:00:00.000000 redshift_client-5.1.1/mypy.ini
+-rw-r--r--   0        0        0      260 1980-01-01 00:00:00.000000 redshift_client-5.1.1/nix.conf
+-rw-r--r--   0        0        0      667 1980-01-01 00:00:00.000000 redshift_client-5.1.1/pyproject.toml
+-rw-r--r--   0        0        0      112 1980-01-01 00:00:00.000000 redshift_client-5.1.1/redshift_client/__init__.py
+-rw-r--r--   0        0        0     2996 1980-01-01 00:00:00.000000 redshift_client-5.1.1/redshift_client/_utils.py
+-rw-r--r--   0        0        0      336 1980-01-01 00:00:00.000000 redshift_client-5.1.1/redshift_client/client/__init__.py
+-rw-r--r--   0        0        0     6335 1980-01-01 00:00:00.000000 redshift_client-5.1.1/redshift_client/client/_core.py
+-rw-r--r--   0        0        0      941 1980-01-01 00:00:00.000000 redshift_client-5.1.1/redshift_client/client/_factory.py
+-rw-r--r--   0        0        0      864 1980-01-01 00:00:00.000000 redshift_client-5.1.1/redshift_client/client/_schema/__init__.py
+-rw-r--r--   0        0        0     7451 1980-01-01 00:00:00.000000 redshift_client-5.1.1/redshift_client/client/_schema/_methods.py
+-rw-r--r--   0        0        0     1120 1980-01-01 00:00:00.000000 redshift_client-5.1.1/redshift_client/client/_table/__init__.py
+-rw-r--r--   0        0        0     2160 1980-01-01 00:00:00.000000 redshift_client-5.1.1/redshift_client/client/_table/_assert.py
+-rw-r--r--   0        0        0      283 1980-01-01 00:00:00.000000 redshift_client-5.1.1/redshift_client/client/_table/_encode.py
+-rw-r--r--   0        0        0    12271 1980-01-01 00:00:00.000000 redshift_client-5.1.1/redshift_client/client/_table/_methods.py
+-rw-r--r--   0        0        0     1922 1980-01-01 00:00:00.000000 redshift_client-5.1.1/redshift_client/client/_table/_new.py
+-rw-r--r--   0        0        0        0 1980-01-01 00:00:00.000000 redshift_client-5.1.1/redshift_client/core/__init__.py
+-rw-r--r--   0        0        0      496 1980-01-01 00:00:00.000000 redshift_client-5.1.1/redshift_client/core/column.py
+-rw-r--r--   0        0        0        0 1980-01-01 00:00:00.000000 redshift_client-5.1.1/redshift_client/core/data_type/__init__.py
+-rw-r--r--   0        0        0     1589 1980-01-01 00:00:00.000000 redshift_client-5.1.1/redshift_client/core/data_type/alias.py
+-rw-r--r--   0        0        0     1585 1980-01-01 00:00:00.000000 redshift_client-5.1.1/redshift_client/core/data_type/core.py
+-rw-r--r--   0        0        0     1565 1980-01-01 00:00:00.000000 redshift_client-5.1.1/redshift_client/core/data_type/decode.py
+-rw-r--r--   0        0        0      843 1980-01-01 00:00:00.000000 redshift_client-5.1.1/redshift_client/core/id_objs.py
+-rw-r--r--   0        0        0      589 1980-01-01 00:00:00.000000 redshift_client-5.1.1/redshift_client/core/schema.py
+-rw-r--r--   0        0        0     6793 1980-01-01 00:00:00.000000 redshift_client-5.1.1/redshift_client/core/table.py
+-rw-r--r--   0        0        0        0 1980-01-01 00:00:00.000000 redshift_client-5.1.1/redshift_client/py.typed
+-rw-r--r--   0        0        0      751 1980-01-01 00:00:00.000000 redshift_client-5.1.1/redshift_client/sql_client/__init__.py
+-rw-r--r--   0        0        0     8823 1980-01-01 00:00:00.000000 redshift_client-5.1.1/redshift_client/sql_client/_client_1/__init__.py
+-rw-r--r--   0        0        0     1295 1980-01-01 00:00:00.000000 redshift_client-5.1.1/redshift_client/sql_client/_client_1/_assert.py
+-rw-r--r--   0        0        0        0 1980-01-01 00:00:00.000000 redshift_client-5.1.1/redshift_client/sql_client/_core/__init__.py
+-rw-r--r--   0        0        0     1167 1980-01-01 00:00:00.000000 redshift_client-5.1.1/redshift_client/sql_client/_core/client.py
+-rw-r--r--   0        0        0     3164 1980-01-01 00:00:00.000000 redshift_client-5.1.1/redshift_client/sql_client/_core/connection.py
+-rw-r--r--   0        0        0      283 1980-01-01 00:00:00.000000 redshift_client-5.1.1/redshift_client/sql_client/_core/creds.py
+-rw-r--r--   0        0        0     2624 1980-01-01 00:00:00.000000 redshift_client-5.1.1/redshift_client/sql_client/_core/primitive.py
+-rw-r--r--   0        0        0     1029 1980-01-01 00:00:00.000000 redshift_client-5.1.1/redshift_client/sql_client/_core/query.py
+-rw-r--r--   0        0        0      833 1980-01-01 00:00:00.000000 redshift_client-5.1.1/redshift_client/sql_client/_factory.py
+-rw-r--r--   0        0        0     1801 1980-01-01 00:00:00.000000 redshift_client-5.1.1/redshift_client/sql_client/_temp_creds.py
+-rw-r--r--   0        0        0        0 1980-01-01 00:00:00.000000 redshift_client-5.1.1/tests/__init__.py
+-rw-r--r--   0        0        0        0 1980-01-01 00:00:00.000000 redshift_client-5.1.1/tests/arch/__init__.py
+-rw-r--r--   0        0        0     1858 1980-01-01 00:00:00.000000 redshift_client-5.1.1/tests/arch/arch.py
+-rw-r--r--   0        0        0     1055 1980-01-01 00:00:00.000000 redshift_client-5.1.1/tests/arch/test_arch.py
+-rw-r--r--   0        0        0        0 1980-01-01 00:00:00.000000 redshift_client-5.1.1/tests/py.typed
+-rw-r--r--   0        0        0      233 1980-01-01 00:00:00.000000 redshift_client-5.1.1/tests/test_column.py
+-rw-r--r--   0        0        0     1618 1980-01-01 00:00:00.000000 redshift_client-5.1.1/tests/test_table.py
+-rw-r--r--   0        0        0      462 1980-01-01 00:00:00.000000 redshift_client-5.1.1/tests/test_temp_creds.py
+-rw-r--r--   0        0        0      579 1970-01-01 00:00:00.000000 redshift_client-5.1.1/PKG-INFO
```

### Comparing `redshift_client-5.1.0/.gitlab-ci.yml` & `redshift_client-5.1.1/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `redshift_client-5.1.0/build/default.nix` & `redshift_client-5.1.1/build/default.nix`

 * *Files identical despite different names*

### Comparing `redshift_client-5.1.0/build/deps/arch_lint.nix` & `redshift_client-5.1.1/build/deps/arch_lint.nix`

 * *Files identical despite different names*

### Comparing `redshift_client-5.1.0/build/deps/boto3/stubs.nix` & `redshift_client-5.1.1/build/deps/boto3/stubs.nix`

 * *Files identical despite different names*

### Comparing `redshift_client-5.1.0/build/deps/default.nix` & `redshift_client-5.1.1/build/deps/default.nix`

 * *Files identical despite different names*

### Comparing `redshift_client-5.1.0/build/deps/fa_purity.nix` & `redshift_client-5.1.1/build/deps/fa_purity.nix`

 * *Files identical despite different names*

### Comparing `redshift_client-5.1.0/build/dev_env/vs_settings.py` & `redshift_client-5.1.1/build/dev_env/vs_settings.py`

 * *Files identical despite different names*

### Comparing `redshift_client-5.1.0/flake.lock` & `redshift_client-5.1.1/flake.lock`

 * *Files identical despite different names*

### Comparing `redshift_client-5.1.0/flake.nix` & `redshift_client-5.1.1/flake.nix`

 * *Files identical despite different names*

### Comparing `redshift_client-5.1.0/makes.nix` & `redshift_client-5.1.1/makes.nix`

 * *Files identical despite different names*

### Comparing `redshift_client-5.1.0/mypy.ini` & `redshift_client-5.1.1/mypy.ini`

 * *Files identical despite different names*

### Comparing `redshift_client-5.1.0/pyproject.toml` & `redshift_client-5.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `redshift_client-5.1.0/redshift_client/_utils.py` & `redshift_client-5.1.1/redshift_client/_utils.py`

 * *Files identical despite different names*

### Comparing `redshift_client-5.1.0/redshift_client/client/_core.py` & `redshift_client-5.1.1/redshift_client/client/_core.py`

 * *Files identical despite different names*

### Comparing `redshift_client-5.1.0/redshift_client/client/_factory.py` & `redshift_client-5.1.1/redshift_client/client/_factory.py`

 * *Files identical despite different names*

### Comparing `redshift_client-5.1.0/redshift_client/client/_schema/__init__.py` & `redshift_client-5.1.1/redshift_client/client/_schema/__init__.py`

 * *Files identical despite different names*

### Comparing `redshift_client-5.1.0/redshift_client/client/_schema/_methods.py` & `redshift_client-5.1.1/redshift_client/client/_schema/_methods.py`

 * *Files identical despite different names*

### Comparing `redshift_client-5.1.0/redshift_client/client/_table/__init__.py` & `redshift_client-5.1.1/redshift_client/client/_table/__init__.py`

 * *Files identical despite different names*

### Comparing `redshift_client-5.1.0/redshift_client/client/_table/_assert.py` & `redshift_client-5.1.1/redshift_client/client/_table/_assert.py`

 * *Files identical despite different names*

### Comparing `redshift_client-5.1.0/redshift_client/client/_table/_methods.py` & `redshift_client-5.1.1/redshift_client/client/_table/_methods.py`

 * *Files identical despite different names*

### Comparing `redshift_client-5.1.0/redshift_client/client/_table/_new.py` & `redshift_client-5.1.1/redshift_client/client/_table/_new.py`

 * *Files identical despite different names*

### Comparing `redshift_client-5.1.0/redshift_client/core/data_type/alias.py` & `redshift_client-5.1.1/redshift_client/core/data_type/alias.py`

 * *Files identical despite different names*

### Comparing `redshift_client-5.1.0/redshift_client/core/data_type/core.py` & `redshift_client-5.1.1/redshift_client/core/data_type/core.py`

 * *Files identical despite different names*

### Comparing `redshift_client-5.1.0/redshift_client/core/data_type/decode.py` & `redshift_client-5.1.1/redshift_client/core/data_type/decode.py`

 * *Files identical despite different names*

### Comparing `redshift_client-5.1.0/redshift_client/core/id_objs.py` & `redshift_client-5.1.1/redshift_client/core/id_objs.py`

 * *Files identical despite different names*

### Comparing `redshift_client-5.1.0/redshift_client/core/schema.py` & `redshift_client-5.1.1/redshift_client/core/schema.py`

 * *Files identical despite different names*

### Comparing `redshift_client-5.1.0/redshift_client/core/table.py` & `redshift_client-5.1.1/redshift_client/core/table.py`

 * *Files identical despite different names*

### Comparing `redshift_client-5.1.0/redshift_client/sql_client/__init__.py` & `redshift_client-5.1.1/redshift_client/sql_client/__init__.py`

 * *Files identical despite different names*

### Comparing `redshift_client-5.1.0/redshift_client/sql_client/_client_1/__init__.py` & `redshift_client-5.1.1/redshift_client/sql_client/_client_1/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -237,15 +237,15 @@
                 lambda q: _to_raw(q.values)
             )
             return _handle_psycopg_errors(
                 lambda: extras.execute_values(  # type: ignore[misc]
                     self._cursor,
                     query.statement,
                     _args,
-                    template=",".join(template.keys),
+                    template="(" + ",".join(template.keys) + ")",
                 )
             )
 
         return Cmd.from_cmd(_action)
 
     def fetch_one(self) -> Cmd[ResultE[Maybe[RowData]]]:
         def _action() -> ResultE[Maybe[RowData]]:
```

### Comparing `redshift_client-5.1.0/redshift_client/sql_client/_client_1/_assert.py` & `redshift_client-5.1.1/redshift_client/sql_client/_client_1/_assert.py`

 * *Files identical despite different names*

### Comparing `redshift_client-5.1.0/redshift_client/sql_client/_core/client.py` & `redshift_client-5.1.1/redshift_client/sql_client/_core/client.py`

 * *Files identical despite different names*

### Comparing `redshift_client-5.1.0/redshift_client/sql_client/_core/connection.py` & `redshift_client-5.1.1/redshift_client/sql_client/_core/connection.py`

 * *Files identical despite different names*

### Comparing `redshift_client-5.1.0/redshift_client/sql_client/_core/primitive.py` & `redshift_client-5.1.1/redshift_client/sql_client/_core/primitive.py`

 * *Files identical despite different names*

### Comparing `redshift_client-5.1.0/redshift_client/sql_client/_core/query.py` & `redshift_client-5.1.1/redshift_client/sql_client/_core/query.py`

 * *Files identical despite different names*

### Comparing `redshift_client-5.1.0/redshift_client/sql_client/_factory.py` & `redshift_client-5.1.1/redshift_client/sql_client/_factory.py`

 * *Files identical despite different names*

### Comparing `redshift_client-5.1.0/redshift_client/sql_client/_temp_creds.py` & `redshift_client-5.1.1/redshift_client/sql_client/_temp_creds.py`

 * *Files identical despite different names*

### Comparing `redshift_client-5.1.0/tests/arch/arch.py` & `redshift_client-5.1.1/tests/arch/arch.py`

 * *Files identical despite different names*

### Comparing `redshift_client-5.1.0/tests/arch/test_arch.py` & `redshift_client-5.1.1/tests/arch/test_arch.py`

 * *Files identical despite different names*

### Comparing `redshift_client-5.1.0/tests/test_table.py` & `redshift_client-5.1.1/tests/test_table.py`

 * *Files identical despite different names*

### Comparing `redshift_client-5.1.0/PKG-INFO` & `redshift_client-5.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redshift_client
-Version: 5.1.0
+Version: 5.1.1
 Summary: Redshift client-SDK
 Author-email: Product Team <development@fluidattacks.com>
 Requires-Python: >=3.11
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: boto3 >=1.28.57, <2.0.0
 Requires-Dist: Deprecated >=1.2.12, <2.0.0
 Requires-Dist: psycopg2 >=2.8.6, <3.0.0
```

