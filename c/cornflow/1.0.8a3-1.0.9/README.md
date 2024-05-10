# Comparing `tmp/cornflow-1.0.8a3.tar.gz` & `tmp/cornflow-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cornflow-1.0.8a3.tar", last modified: Sun Oct 15 12:07:13 2023, max compression
+gzip compressed data, was "cornflow-1.0.9.tar", last modified: Wed Dec 27 10:12:58 2023, max compression
```

## Comparing `cornflow-1.0.8a3.tar` & `cornflow-1.0.9.tar`

### file list

```diff
@@ -1,200 +1,200 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-15 12:07:13.803501 cornflow-1.0.8a3/
--rw-r--r--   0 runner    (1001) docker     (127)      140 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    10048 2023-10-15 12:07:13.803501 cornflow-1.0.8a3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7775 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-15 12:07:13.783500 cornflow-1.0.8a3/airflow_config/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/airflow_config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      677 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/airflow_config/airflow_local_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-15 12:07:13.783500 cornflow-1.0.8a3/airflow_config/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-15 12:07:13.783500 cornflow-1.0.8a3/airflow_config/plugins/XCom/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/airflow_config/plugins/XCom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1795 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/airflow_config/plugins/XCom/gce_xcom_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/airflow_config/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2595 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/airflow_config/webserver_ldap.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-15 12:07:13.783500 cornflow-1.0.8a3/cornflow/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6997 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-15 12:07:13.787500 cornflow-1.0.8a3/cornflow/cli/
--rw-r--r--   0 runner    (1001) docker     (127)      742 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      424 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/cli/actions.py
--rw-r--r--   0 runner    (1001) docker     (127)      657 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/cli/arguments.py
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/cli/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/cli/migrations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/cli/permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/cli/roles.py
--rw-r--r--   0 runner    (1001) docker     (127)     6086 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/cli/schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)     9135 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/cli/service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-15 12:07:13.787500 cornflow-1.0.8a3/cornflow/cli/tools/
--rw-r--r--   0 runner    (1001) docker     (127)       19 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/cli/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16344 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/cli/tools/api_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)    12640 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/cli/tools/endpoint_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     5398 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/cli/tools/models_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     7557 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/cli/tools/schema_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2245 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/cli/tools/schemas_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)      929 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/cli/tools/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)      748 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/cli/users.py
--rw-r--r--   0 runner    (1001) docker     (127)      733 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/cli/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      636 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/cli/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-15 12:07:13.787500 cornflow-1.0.8a3/cornflow/commands/
--rw-r--r--   0 runner    (1001) docker     (127)      515 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      748 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/commands/access.py
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/commands/actions.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/commands/cleanup.py
--rw-r--r--   0 runner    (1001) docker     (127)     3715 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/commands/dag.py
--rw-r--r--   0 runner    (1001) docker     (127)     6627 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/commands/permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/commands/roles.py
--rw-r--r--   0 runner    (1001) docker     (127)      902 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/commands/schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)     2591 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/commands/users.py
--rw-r--r--   0 runner    (1001) docker     (127)     2276 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/commands/views.py
--rw-r--r--   0 runner    (1001) docker     (127)     4458 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-15 12:07:13.791500 cornflow-1.0.8a3/cornflow/endpoints/
--rw-r--r--   0 runner    (1001) docker     (127)     7168 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/endpoints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1359 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/endpoints/action.py
--rw-r--r--   0 runner    (1001) docker     (127)     1956 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/endpoints/alarms.py
--rw-r--r--   0 runner    (1001) docker     (127)     1370 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/endpoints/apiview.py
--rw-r--r--   0 runner    (1001) docker     (127)    18670 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/endpoints/case.py
--rw-r--r--   0 runner    (1001) docker     (127)    10390 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/endpoints/dag.py
--rw-r--r--   0 runner    (1001) docker     (127)    16496 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/endpoints/data_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     2441 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/endpoints/example_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    27951 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/endpoints/execution.py
--rw-r--r--   0 runner    (1001) docker     (127)     1610 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/endpoints/health.py
--rw-r--r--   0 runner    (1001) docker     (127)    11615 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/endpoints/instance.py
--rw-r--r--   0 runner    (1001) docker     (127)      873 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/endpoints/licenses.py
--rw-r--r--   0 runner    (1001) docker     (127)     7968 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/endpoints/login.py
--rw-r--r--   0 runner    (1001) docker     (127)     2006 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/endpoints/main_alarms.py
--rw-r--r--   0 runner    (1001) docker     (127)     8471 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/endpoints/meta_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     3751 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/endpoints/permission.py
--rw-r--r--   0 runner    (1001) docker     (127)     6105 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/endpoints/roles.py
--rw-r--r--   0 runner    (1001) docker     (127)     2933 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/endpoints/schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)     3513 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/endpoints/signup.py
--rw-r--r--   0 runner    (1001) docker     (127)     3071 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/endpoints/tables.py
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/endpoints/token.py
--rw-r--r--   0 runner    (1001) docker     (127)    11751 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/endpoints/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     6524 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/endpoints/user_role.py
--rw-r--r--   0 runner    (1001) docker     (127)      480 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/gunicorn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-15 12:07:13.791500 cornflow-1.0.8a3/cornflow/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/migrations/README
--rw-r--r--   0 runner    (1001) docker     (127)      857 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/migrations/alembic.ini
--rw-r--r--   0 runner    (1001) docker     (127)     2767 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/migrations/env.py
--rw-r--r--   0 runner    (1001) docker     (127)      494 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/migrations/script.py.mako
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-15 12:07:13.791500 cornflow-1.0.8a3/cornflow/migrations/versions/
--rw-r--r--   0 runner    (1001) docker     (127)     1370 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/migrations/versions/00757b557b02_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1926 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/migrations/versions/1af47a419bbd_.py
--rw-r--r--   0 runner    (1001) docker     (127)     2200 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/migrations/versions/4aac5e0c6e66_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1569 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/migrations/versions/7c3ea5ab5501_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1370 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/migrations/versions/a472b5ad50b7_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1812 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/migrations/versions/c2db9409cb5f_.py
--rw-r--r--   0 runner    (1001) docker     (127)     3574 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/migrations/versions/c8a6c762e818_.py
--rw-r--r--   0 runner    (1001) docker     (127)     2433 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/migrations/versions/ca449af8034c_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/migrations/versions/d0e0700dcd8e_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1607 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/migrations/versions/d1b5be1f0549_.py
--rw-r--r--   0 runner    (1001) docker     (127)     3555 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/migrations/versions/e1a50dae1ac9_.py
--rw-r--r--   0 runner    (1001) docker     (127)      710 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/migrations/versions/e937a5234ce4_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1848 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/migrations/versions/ebdd955fcc5e_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1782 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/migrations/versions/f3bee20314a2_.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-15 12:07:13.795500 cornflow-1.0.8a3/cornflow/models/
--rw-r--r--   0 runner    (1001) docker     (127)      500 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1200 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/models/action.py
--rw-r--r--   0 runner    (1001) docker     (127)     1682 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/models/alarms.py
--rw-r--r--   0 runner    (1001) docker     (127)     5467 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/models/base_data_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     7202 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/models/case.py
--rw-r--r--   0 runner    (1001) docker     (127)     2930 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/models/dag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1716 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/models/dag_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5974 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/models/execution.py
--rw-r--r--   0 runner    (1001) docker     (127)     3788 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/models/instance.py
--rw-r--r--   0 runner    (1001) docker     (127)     1748 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/models/main_alarms.py
--rw-r--r--   0 runner    (1001) docker     (127)    12000 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/models/meta_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2804 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/models/permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2052 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/models/role.py
--rw-r--r--   0 runner    (1001) docker     (127)     8560 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/models/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     4974 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/models/user_role.py
--rw-r--r--   0 runner    (1001) docker     (127)     2066 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/models/view.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-15 12:07:13.795500 cornflow-1.0.8a3/cornflow/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)      215 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      340 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/schemas/action.py
--rw-r--r--   0 runner    (1001) docker     (127)      541 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/schemas/alarms.py
--rw-r--r--   0 runner    (1001) docker     (127)     2909 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/schemas/case.py
--rw-r--r--   0 runner    (1001) docker     (127)      473 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/schemas/common.py
--rw-r--r--   0 runner    (1001) docker     (127)      901 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/schemas/dag.py
--rw-r--r--   0 runner    (1001) docker     (127)      146 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/schemas/example_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     4470 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/schemas/execution.py
--rw-r--r--   0 runner    (1001) docker     (127)      141 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/schemas/health.py
--rw-r--r--   0 runner    (1001) docker     (127)     1870 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/schemas/instance.py
--rw-r--r--   0 runner    (1001) docker     (127)      604 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/schemas/main_alarms.py
--rw-r--r--   0 runner    (1001) docker     (127)      202 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/schemas/model_json.py
--rw-r--r--   0 runner    (1001) docker     (127)      260 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/schemas/patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1270 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/schemas/permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)      984 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/schemas/query.py
--rw-r--r--   0 runner    (1001) docker     (127)      469 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/schemas/role.py
--rw-r--r--   0 runner    (1001) docker     (127)      433 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/schemas/schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)     2163 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/schemas/solution_log.py
--rw-r--r--   0 runner    (1001) docker     (127)      105 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/schemas/tables.py
--rw-r--r--   0 runner    (1001) docker     (127)     2045 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/schemas/user.py
--rw-r--r--   0 runner    (1001) docker     (127)      615 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/schemas/user_role.py
--rw-r--r--   0 runner    (1001) docker     (127)      429 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/schemas/view.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-15 12:07:13.799500 cornflow-1.0.8a3/cornflow/shared/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/shared/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-15 12:07:13.799500 cornflow-1.0.8a3/cornflow/shared/authentication/
--rw-r--r--   0 runner    (1001) docker     (127)      137 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/shared/authentication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16840 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/shared/authentication/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     1276 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/shared/authentication/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     4853 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/shared/authentication/ldap.py
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/shared/compress.py
--rw-r--r--   0 runner    (1001) docker     (127)     3440 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/shared/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     3437 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/shared/email.py
--rw-r--r--   0 runner    (1001) docker     (127)     6979 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/shared/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2235 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/shared/licenses.py
--rw-r--r--   0 runner    (1001) docker     (127)      621 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/shared/log_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1199 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/shared/query_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)      860 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/shared/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2236 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/shared/utils_tables.py
--rw-r--r--   0 runner    (1001) docker     (127)     4803 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/shared/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-15 12:07:13.799500 cornflow-1.0.8a3/cornflow/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2499 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/tests/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     3079 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/tests/custom_liveServer.py
--rw-r--r--   0 runner    (1001) docker     (127)    24773 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/tests/custom_test_case.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-15 12:07:13.799500 cornflow-1.0.8a3/cornflow/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      695 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/tests/integration/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)    20646 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/tests/integration/test_cornflowclient.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-15 12:07:13.799500 cornflow-1.0.8a3/cornflow/tests/ldap/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/tests/ldap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4286 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/tests/ldap/test_ldap_authentication.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-15 12:07:13.799500 cornflow-1.0.8a3/cornflow/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1755 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/tests/unit/test_actions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/tests/unit/test_alarms.py
--rw-r--r--   0 runner    (1001) docker     (127)     2107 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/tests/unit/test_apiview.py
--rw-r--r--   0 runner    (1001) docker     (127)    23985 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/tests/unit/test_cases.py
--rw-r--r--   0 runner    (1001) docker     (127)     9150 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/tests/unit/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     8776 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/tests/unit/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     9034 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/tests/unit/test_dags.py
--rw-r--r--   0 runner    (1001) docker     (127)     5471 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/tests/unit/test_data_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1518 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/tests/unit/test_example_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    15333 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/tests/unit/test_executions.py
--rw-r--r--   0 runner    (1001) docker     (127)    15376 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/tests/unit/test_generate_from_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/tests/unit/test_health.py
--rw-r--r--   0 runner    (1001) docker     (127)     9650 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/tests/unit/test_instances.py
--rw-r--r--   0 runner    (1001) docker     (127)     1986 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/tests/unit/test_instances_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/tests/unit/test_licenses.py
--rw-r--r--   0 runner    (1001) docker     (127)      979 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/tests/unit/test_log_in.py
--rw-r--r--   0 runner    (1001) docker     (127)     1970 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/tests/unit/test_main_alarms.py
--rw-r--r--   0 runner    (1001) docker     (127)     8782 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/tests/unit/test_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)    16581 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/tests/unit/test_roles.py
--rw-r--r--   0 runner    (1001) docker     (127)     4421 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/tests/unit/test_schema_from_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     7177 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/tests/unit/test_schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)     3481 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/tests/unit/test_sign_up.py
--rw-r--r--   0 runner    (1001) docker     (127)     8947 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/tests/unit/test_tables.py
--rw-r--r--   0 runner    (1001) docker     (127)     2068 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/tests/unit/test_token.py
--rw-r--r--   0 runner    (1001) docker     (127)    21677 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/tests/unit/test_users.py
--rw-r--r--   0 runner    (1001) docker     (127)      585 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/cornflow/tests/unit/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-15 12:07:13.783500 cornflow-1.0.8a3/cornflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10048 2023-10-15 12:07:13.000000 cornflow-1.0.8a3/cornflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5679 2023-10-15 12:07:13.000000 cornflow-1.0.8a3/cornflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-15 12:07:13.000000 cornflow-1.0.8a3/cornflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2023-10-15 12:07:13.000000 cornflow-1.0.8a3/cornflow.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      595 2023-10-15 12:07:13.000000 cornflow-1.0.8a3/cornflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2023-10-15 12:07:13.000000 cornflow-1.0.8a3/cornflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-15 12:07:13.803501 cornflow-1.0.8a3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2023-10-15 12:07:10.000000 cornflow-1.0.8a3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 10:12:58.053682 cornflow-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2023-12-27 10:12:56.000000 cornflow-1.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    10046 2023-12-27 10:12:58.053682 cornflow-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7775 2023-12-27 10:12:56.000000 cornflow-1.0.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 10:12:58.025682 cornflow-1.0.9/airflow_config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-27 10:12:56.000000 cornflow-1.0.9/airflow_config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2023-12-27 10:12:56.000000 cornflow-1.0.9/airflow_config/airflow_local_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 10:12:58.029682 cornflow-1.0.9/airflow_config/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 10:12:58.029682 cornflow-1.0.9/airflow_config/plugins/XCom/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-27 10:12:56.000000 cornflow-1.0.9/airflow_config/plugins/XCom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1795 2023-12-27 10:12:56.000000 cornflow-1.0.9/airflow_config/plugins/XCom/gce_xcom_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-27 10:12:56.000000 cornflow-1.0.9/airflow_config/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2595 2023-12-27 10:12:56.000000 cornflow-1.0.9/airflow_config/webserver_ldap.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 10:12:58.029682 cornflow-1.0.9/cornflow/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6997 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 10:12:58.029682 cornflow-1.0.9/cornflow/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/cli/actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/cli/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/cli/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/cli/migrations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/cli/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/cli/roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6086 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/cli/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9135 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/cli/service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 10:12:58.033682 cornflow-1.0.9/cornflow/cli/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/cli/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16344 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/cli/tools/api_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12640 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/cli/tools/endpoint_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5398 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/cli/tools/models_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7557 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/cli/tools/schema_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2245 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/cli/tools/schemas_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/cli/tools/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2104 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/cli/users.py
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/cli/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/cli/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 10:12:58.033682 cornflow-1.0.9/cornflow/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/commands/access.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/commands/actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/commands/cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3715 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/commands/dag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6627 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/commands/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/commands/roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/commands/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2591 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/commands/users.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2276 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/commands/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4556 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 10:12:58.037682 cornflow-1.0.9/cornflow/endpoints/
+-rw-r--r--   0 runner    (1001) docker     (127)     7168 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/endpoints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/endpoints/action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1956 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/endpoints/alarms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1370 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/endpoints/apiview.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18670 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/endpoints/case.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10390 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/endpoints/dag.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16496 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/endpoints/data_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2441 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/endpoints/example_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27951 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/endpoints/execution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1610 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/endpoints/health.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11615 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/endpoints/instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/endpoints/licenses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7968 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/endpoints/login.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2006 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/endpoints/main_alarms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8471 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/endpoints/meta_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3751 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/endpoints/permission.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6105 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/endpoints/roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2933 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/endpoints/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3513 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/endpoints/signup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3071 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/endpoints/tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/endpoints/token.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11751 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/endpoints/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6524 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/endpoints/user_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/gunicorn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 10:12:58.037682 cornflow-1.0.9/cornflow/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/migrations/README
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/migrations/alembic.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     2767 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/migrations/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/migrations/script.py.mako
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 10:12:58.041682 cornflow-1.0.9/cornflow/migrations/versions/
+-rw-r--r--   0 runner    (1001) docker     (127)     1370 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/migrations/versions/00757b557b02_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1926 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/migrations/versions/1af47a419bbd_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2200 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/migrations/versions/4aac5e0c6e66_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1569 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/migrations/versions/7c3ea5ab5501_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1370 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/migrations/versions/a472b5ad50b7_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/migrations/versions/c2db9409cb5f_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3574 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/migrations/versions/c8a6c762e818_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2433 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/migrations/versions/ca449af8034c_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/migrations/versions/d0e0700dcd8e_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1607 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/migrations/versions/d1b5be1f0549_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3555 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/migrations/versions/e1a50dae1ac9_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/migrations/versions/e937a5234ce4_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1848 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/migrations/versions/ebdd955fcc5e_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1782 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/migrations/versions/f3bee20314a2_.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 10:12:58.041682 cornflow-1.0.9/cornflow/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/models/action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/models/alarms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5467 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/models/base_data_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7202 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/models/case.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2930 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/models/dag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1716 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/models/dag_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5974 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/models/execution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3788 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/models/instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1748 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/models/main_alarms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12000 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/models/meta_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2804 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/models/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2052 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/models/role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8560 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/models/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4974 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/models/user_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2066 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/models/view.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 10:12:58.045682 cornflow-1.0.9/cornflow/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/schemas/action.py
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/schemas/alarms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2909 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/schemas/case.py
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/schemas/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/schemas/dag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/schemas/example_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4470 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/schemas/execution.py
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/schemas/health.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1870 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/schemas/instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/schemas/main_alarms.py
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/schemas/model_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/schemas/patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1270 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/schemas/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/schemas/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/schemas/role.py
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/schemas/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2163 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/schemas/solution_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/schemas/tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2045 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/schemas/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/schemas/user_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/schemas/view.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 10:12:58.049682 cornflow-1.0.9/cornflow/shared/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/shared/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 10:12:58.049682 cornflow-1.0.9/cornflow/shared/authentication/
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/shared/authentication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18621 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/shared/authentication/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1276 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/shared/authentication/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4853 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/shared/authentication/ldap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/shared/compress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3440 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/shared/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3437 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/shared/email.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6979 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/shared/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2235 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/shared/licenses.py
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/shared/log_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1199 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/shared/query_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/shared/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2236 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/shared/utils_tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4803 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/shared/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 10:12:58.049682 cornflow-1.0.9/cornflow/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2499 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/tests/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3079 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/tests/custom_liveServer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24777 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/tests/custom_test_case.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 10:12:58.049682 cornflow-1.0.9/cornflow/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/tests/integration/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20646 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/tests/integration/test_cornflowclient.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 10:12:58.049682 cornflow-1.0.9/cornflow/tests/ldap/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/tests/ldap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4286 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/tests/ldap/test_ldap_authentication.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 10:12:58.053682 cornflow-1.0.9/cornflow/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1755 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/tests/unit/test_actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/tests/unit/test_alarms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2107 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/tests/unit/test_apiview.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23985 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/tests/unit/test_cases.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12578 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/tests/unit/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8776 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/tests/unit/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9034 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/tests/unit/test_dags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5471 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/tests/unit/test_data_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1518 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/tests/unit/test_example_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15333 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/tests/unit/test_executions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15376 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/tests/unit/test_generate_from_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/tests/unit/test_health.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9650 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/tests/unit/test_instances.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1986 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/tests/unit/test_instances_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/tests/unit/test_licenses.py
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/tests/unit/test_log_in.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1970 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/tests/unit/test_main_alarms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8782 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/tests/unit/test_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16581 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/tests/unit/test_roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4421 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/tests/unit/test_schema_from_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7177 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/tests/unit/test_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3481 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/tests/unit/test_sign_up.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8947 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/tests/unit/test_tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3132 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/tests/unit/test_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21677 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/tests/unit/test_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2023-12-27 10:12:56.000000 cornflow-1.0.9/cornflow/tests/unit/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 10:12:58.029682 cornflow-1.0.9/cornflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10046 2023-12-27 10:12:57.000000 cornflow-1.0.9/cornflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5679 2023-12-27 10:12:58.000000 cornflow-1.0.9/cornflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-27 10:12:57.000000 cornflow-1.0.9/cornflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2023-12-27 10:12:57.000000 cornflow-1.0.9/cornflow.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2023-12-27 10:12:57.000000 cornflow-1.0.9/cornflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2023-12-27 10:12:57.000000 cornflow-1.0.9/cornflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-27 10:12:58.053682 cornflow-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2023-12-27 10:12:56.000000 cornflow-1.0.9/setup.py
```

### Comparing `cornflow-1.0.8a3/PKG-INFO` & `cornflow-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: cornflow
-Version: 1.0.8a3
+Version: 1.0.9
 Summary: Cornflow is an open source multi-solver optimization server with a REST API built using flask.
 Home-page: https://github.com/baobabsoluciones/cornflow
 Author: baobab soluciones
 Author-email: cornflow@baobabsoluciones.es
 License: UNKNOWN
 Description: Cornflow
         =========
```

### Comparing `cornflow-1.0.8a3/README.rst` & `cornflow-1.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/airflow_config/airflow_local_settings.py` & `cornflow-1.0.9/airflow_config/airflow_local_settings.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/airflow_config/plugins/XCom/gce_xcom_backend.py` & `cornflow-1.0.9/airflow_config/plugins/XCom/gce_xcom_backend.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/airflow_config/webserver_ldap.py` & `cornflow-1.0.9/airflow_config/webserver_ldap.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow/app.py` & `cornflow-1.0.9/cornflow/app.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow/cli/__init__.py` & `cornflow-1.0.9/cornflow/cli/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 init file to have this as a module
 """
 
 import click
+
 from cornflow.cli.actions import actions
 from cornflow.cli.config import config
 from cornflow.cli.migrations import migrations
 from cornflow.cli.permissions import permissions
 from cornflow.cli.roles import roles
 from cornflow.cli.schemas import schemas
 from cornflow.cli.service import service
```

### Comparing `cornflow-1.0.8a3/cornflow/cli/arguments.py` & `cornflow-1.0.9/cornflow/cli/arguments.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow/cli/config.py` & `cornflow-1.0.9/cornflow/cli/config.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow/cli/migrations.py` & `cornflow-1.0.9/cornflow/cli/migrations.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow/cli/permissions.py` & `cornflow-1.0.9/cornflow/cli/permissions.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow/cli/schemas.py` & `cornflow-1.0.9/cornflow/cli/schemas.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow/cli/service.py` & `cornflow-1.0.9/cornflow/cli/service.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow/cli/tools/api_generator.py` & `cornflow-1.0.9/cornflow/cli/tools/api_generator.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow/cli/tools/endpoint_tools.py` & `cornflow-1.0.9/cornflow/cli/tools/endpoint_tools.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow/cli/tools/models_tools.py` & `cornflow-1.0.9/cornflow/cli/tools/models_tools.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow/cli/tools/schema_generator.py` & `cornflow-1.0.9/cornflow/cli/tools/schema_generator.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow/cli/tools/schemas_tools.py` & `cornflow-1.0.9/cornflow/cli/tools/schemas_tools.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow/cli/tools/tools.py` & `cornflow-1.0.9/cornflow/cli/tools/tools.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow/cli/utils.py` & `cornflow-1.0.9/cornflow/cli/utils.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow/cli/views.py` & `cornflow-1.0.9/cornflow/cli/views.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow/commands/__init__.py` & `cornflow-1.0.9/cornflow/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow/commands/access.py` & `cornflow-1.0.9/cornflow/commands/access.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow/commands/actions.py` & `cornflow-1.0.9/cornflow/commands/actions.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow/commands/dag.py` & `cornflow-1.0.9/cornflow/commands/dag.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow/commands/permissions.py` & `cornflow-1.0.9/cornflow/commands/permissions.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow/commands/roles.py` & `cornflow-1.0.9/cornflow/commands/roles.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow/commands/schemas.py` & `cornflow-1.0.9/cornflow/commands/schemas.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow/commands/users.py` & `cornflow-1.0.9/cornflow/commands/users.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow/commands/views.py` & `cornflow-1.0.9/cornflow/commands/views.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow/config.py` & `cornflow-1.0.9/cornflow/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 from .shared.const import AUTH_DB, PLANNER_ROLE
 from apispec import APISpec
 from apispec.ext.marshmallow import MarshmallowPlugin
 
 
 class DefaultConfig(object):
     SERVICE_NAME = os.getenv("SERVICE_NAME", "Cornflow")
-    SECRET_KEY = os.getenv("SECRET_KEY")
+    SECRET_TOKEN_KEY = os.getenv("SECRET_KEY")
+    SECRET_BI_KEY = os.getenv("SECRET_BI_KEY")
     SQLALCHEMY_DATABASE_URI = os.getenv("DATABASE_URL", "sqlite:///cornflow.db")
     AIRFLOW_URL = os.getenv("AIRFLOW_URL")
     AIRFLOW_USER = os.getenv("AIRFLOW_USER")
     AIRFLOW_PWD = os.getenv("AIRFLOW_PWD")
     AUTH_TYPE = int(os.getenv("AUTH_TYPE", AUTH_DB))
     DEFAULT_ROLE = int(os.getenv("DEFAULT_ROLE", PLANNER_ROLE))
     CORS_ORIGINS = os.getenv("CORS_ORIGINS", "*")
@@ -87,15 +88,16 @@
     """ """
 
     ENV = "testing"
     SQLALCHEMY_TRACK_MODIFICATIONS = False
     DEBUG = False
     TESTING = True
     PROPAGATE_EXCEPTIONS = True
-    SECRET_KEY = "TESTINGSECRETKEY"
+    SECRET_TOKEN_KEY = "TESTINGSECRETKEY"
+    SECRET_BI_KEY = "THISISANOTHERKEY"
     SQLALCHEMY_DATABASE_URI = os.getenv("DATABASE_URL", "sqlite:///cornflow_test.db")
     AIRFLOW_URL = os.getenv("AIRFLOW_URL", "http://localhost:8080")
     PRESERVE_CONTEXT_ON_EXCEPTION = False
     AIRFLOW_USER = os.getenv("AIRFLOW_USER", "admin")
     AIRFLOW_PWD = os.getenv("AIRFLOW_PWD", "admin")
     OPEN_DEPLOYMENT = 1
     LOG_LEVEL = int(os.getenv("LOG_LEVEL", 10))
```

### Comparing `cornflow-1.0.8a3/cornflow/endpoints/__init__.py` & `cornflow-1.0.9/cornflow/endpoints/__init__.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow/endpoints/action.py` & `cornflow-1.0.9/cornflow/endpoints/action.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow/endpoints/alarms.py` & `cornflow-1.0.9/cornflow/endpoints/alarms.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow/endpoints/apiview.py` & `cornflow-1.0.9/cornflow/endpoints/apiview.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow/endpoints/case.py` & `cornflow-1.0.9/cornflow/endpoints/case.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow/endpoints/dag.py` & `cornflow-1.0.9/cornflow/endpoints/dag.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow/endpoints/data_check.py` & `cornflow-1.0.9/cornflow/endpoints/data_check.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow/endpoints/example_data.py` & `cornflow-1.0.9/cornflow/endpoints/example_data.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow/endpoints/execution.py` & `cornflow-1.0.9/cornflow/endpoints/execution.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow/endpoints/health.py` & `cornflow-1.0.9/cornflow/endpoints/health.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow/endpoints/instance.py` & `cornflow-1.0.9/cornflow/endpoints/instance.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow/endpoints/licenses.py` & `cornflow-1.0.9/cornflow/endpoints/licenses.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow/endpoints/login.py` & `cornflow-1.0.9/cornflow/endpoints/login.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow/endpoints/main_alarms.py` & `cornflow-1.0.9/cornflow/endpoints/main_alarms.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow/endpoints/meta_resource.py` & `cornflow-1.0.9/cornflow/endpoints/meta_resource.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow/endpoints/permission.py` & `cornflow-1.0.9/cornflow/endpoints/permission.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow/endpoints/roles.py` & `cornflow-1.0.9/cornflow/endpoints/roles.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow/endpoints/schemas.py` & `cornflow-1.0.9/cornflow/endpoints/schemas.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow/endpoints/signup.py` & `cornflow-1.0.9/cornflow/endpoints/signup.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow/endpoints/tables.py` & `cornflow-1.0.9/cornflow/endpoints/tables.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow/endpoints/token.py` & `cornflow-1.0.9/cornflow/endpoints/token.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow/endpoints/user.py` & `cornflow-1.0.9/cornflow/endpoints/user.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow/endpoints/user_role.py` & `cornflow-1.0.9/cornflow/endpoints/user_role.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow/migrations/alembic.ini` & `cornflow-1.0.9/cornflow/migrations/alembic.ini`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow/migrations/env.py` & `cornflow-1.0.9/cornflow/migrations/env.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow/migrations/versions/00757b557b02_.py` & `cornflow-1.0.9/cornflow/migrations/versions/00757b557b02_.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow/migrations/versions/1af47a419bbd_.py` & `cornflow-1.0.9/cornflow/migrations/versions/1af47a419bbd_.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow/migrations/versions/4aac5e0c6e66_.py` & `cornflow-1.0.9/cornflow/migrations/versions/4aac5e0c6e66_.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow/migrations/versions/7c3ea5ab5501_.py` & `cornflow-1.0.9/cornflow/migrations/versions/7c3ea5ab5501_.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow/migrations/versions/a472b5ad50b7_.py` & `cornflow-1.0.9/cornflow/migrations/versions/a472b5ad50b7_.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow/migrations/versions/c2db9409cb5f_.py` & `cornflow-1.0.9/cornflow/migrations/versions/c2db9409cb5f_.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow/migrations/versions/c8a6c762e818_.py` & `cornflow-1.0.9/cornflow/migrations/versions/c8a6c762e818_.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow/migrations/versions/ca449af8034c_.py` & `cornflow-1.0.9/cornflow/migrations/versions/ca449af8034c_.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow/migrations/versions/d0e0700dcd8e_.py` & `cornflow-1.0.9/cornflow/migrations/versions/d0e0700dcd8e_.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow/migrations/versions/d1b5be1f0549_.py` & `cornflow-1.0.9/cornflow/migrations/versions/d1b5be1f0549_.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow/migrations/versions/e1a50dae1ac9_.py` & `cornflow-1.0.9/cornflow/migrations/versions/e1a50dae1ac9_.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow/migrations/versions/e937a5234ce4_.py` & `cornflow-1.0.9/cornflow/migrations/versions/e937a5234ce4_.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow/migrations/versions/ebdd955fcc5e_.py` & `cornflow-1.0.9/cornflow/migrations/versions/ebdd955fcc5e_.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow/migrations/versions/f3bee20314a2_.py` & `cornflow-1.0.9/cornflow/migrations/versions/f3bee20314a2_.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow/models/action.py` & `cornflow-1.0.9/cornflow/models/action.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow/models/alarms.py` & `cornflow-1.0.9/cornflow/models/alarms.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow/models/base_data_model.py` & `cornflow-1.0.9/cornflow/models/base_data_model.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow/models/case.py` & `cornflow-1.0.9/cornflow/models/case.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow/models/dag.py` & `cornflow-1.0.9/cornflow/models/dag.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow/models/dag_permissions.py` & `cornflow-1.0.9/cornflow/models/dag_permissions.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow/models/execution.py` & `cornflow-1.0.9/cornflow/models/execution.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow/models/instance.py` & `cornflow-1.0.9/cornflow/models/instance.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow/models/main_alarms.py` & `cornflow-1.0.9/cornflow/models/main_alarms.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow/models/meta_models.py` & `cornflow-1.0.9/cornflow/models/meta_models.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow/models/permissions.py` & `cornflow-1.0.9/cornflow/models/permissions.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow/models/role.py` & `cornflow-1.0.9/cornflow/models/role.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow/models/user.py` & `cornflow-1.0.9/cornflow/models/user.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow/models/user_role.py` & `cornflow-1.0.9/cornflow/models/user_role.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow/models/view.py` & `cornflow-1.0.9/cornflow/models/view.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow/schemas/alarms.py` & `cornflow-1.0.9/cornflow/schemas/alarms.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow/schemas/case.py` & `cornflow-1.0.9/cornflow/schemas/case.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow/schemas/dag.py` & `cornflow-1.0.9/cornflow/schemas/dag.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow/schemas/execution.py` & `cornflow-1.0.9/cornflow/schemas/execution.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow/schemas/instance.py` & `cornflow-1.0.9/cornflow/schemas/instance.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow/schemas/main_alarms.py` & `cornflow-1.0.9/cornflow/schemas/main_alarms.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow/schemas/permissions.py` & `cornflow-1.0.9/cornflow/schemas/permissions.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow/schemas/query.py` & `cornflow-1.0.9/cornflow/schemas/query.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow/schemas/solution_log.py` & `cornflow-1.0.9/cornflow/schemas/solution_log.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow/schemas/user.py` & `cornflow-1.0.9/cornflow/schemas/user.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow/schemas/user_role.py` & `cornflow-1.0.9/cornflow/schemas/user_role.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow/shared/authentication/auth.py` & `cornflow-1.0.9/cornflow/shared/authentication/auth.py`

 * *Files 4% similar despite different names*

```diff
@@ -95,59 +95,59 @@
         :param int user_id: user code to be encoded in the token to identify the user afterwards
         :return: the generated token
         :rtype: str
         """
         if user_id is None:
             err = "The user id passed to generate the token is not valid."
             raise InvalidUsage(
-                err,
-                log_txt="Error while trying to generate token. " + err
+                err, log_txt="Error while trying to generate token. " + err
             )
 
         payload = {
             "exp": datetime.utcnow() + timedelta(days=1),
             "iat": datetime.utcnow(),
             "sub": user_id,
         }
 
-        return jwt.encode(payload, current_app.config["SECRET_KEY"], algorithm="HS256")
+        return jwt.encode(
+            payload, current_app.config["SECRET_TOKEN_KEY"], algorithm="HS256"
+        )
 
     @staticmethod
     def decode_token(token: str = None) -> dict:
         """
         Decodes a given JSON Web token and extracts the sub from it to give it back.
 
         :param str token: the given JSON Web Token
         :return: the sub field of the token as the user_id
         :rtype: dict
         """
         if token is None:
             err = "The provided token is not valid."
             raise InvalidUsage(
-                err,
-                log_txt="Error while trying to decode token. " + err
+                err, log_txt="Error while trying to decode token. " + err
             )
         try:
             payload = jwt.decode(
-                token, current_app.config["SECRET_KEY"], algorithms="HS256"
+                token, current_app.config["SECRET_TOKEN_KEY"], algorithms="HS256"
             )
             return {"user_id": payload["sub"]}
         except jwt.ExpiredSignatureError:
             raise InvalidCredentials(
                 "The token has expired, please login again",
-                log_txt="Error while trying to decode token. The token has expired."
+                log_txt="Error while trying to decode token. The token has expired.",
             )
         except jwt.InvalidTokenError:
             raise InvalidCredentials(
                 "Invalid token, please try again with a new token",
-                log_txt="Error while trying to decode token. The token is invalid."
+                log_txt="Error while trying to decode token. The token is invalid.",
             )
 
     def validate_oid_token(
-            self, token: str, client_id: str, tenant_id: str, issuer: str, provider: int
+        self, token: str, client_id: str, tenant_id: str, issuer: str, provider: int
     ) -> dict:
         """
         This method takes a token issued by an OID provider, the relevant information about the OID provider
         and validates that the token was generated by such source, is valid and extracts the information
         in the token for its use during the login process
 
         :param str token: the received token
@@ -168,76 +168,75 @@
                 audience=[client_id],
                 issuer=issuer,
             )
             return decoded
         except jwt.ExpiredSignatureError:
             raise InvalidCredentials(
                 "The token has expired, please login again",
-                log_txt="Error while trying to validate a token. The token has expired. "
+                log_txt="Error while trying to validate a token. The token has expired.",
             )
         except jwt.InvalidTokenError:
             raise InvalidCredentials(
                 "Invalid token, please try again with a new token",
-                log_txt="Error while trying to validate a token. The token is not valid. "
+                log_txt="Error while trying to validate a token. The token is not valid.",
             )
 
     @staticmethod
     def get_token_from_header(headers: Headers = None) -> str:
         """
         Extracts the token given on the request from the Authorization headers.
 
         :param headers: the request headers
         :type headers: `Headers`
         :return: the extracted token
         :rtype: str
         """
         if headers is None:
-            raise InvalidUsage(log_txt="Error while trying to get a token from header. The header is invalid.")
+            raise InvalidUsage(
+                log_txt="Error while trying to get a token from header. The header is invalid."
+            )
 
         if "Authorization" not in headers:
             raise InvalidCredentials(
                 "Auth token is not available",
-                log_txt="Error while trying to get a token from header. The auth token is not available."
+                log_txt="Error while trying to get a token from header. The auth token is not available.",
             )
         auth_header = headers.get("Authorization")
         if not auth_header:
             return ""
         try:
             return auth_header.split(" ")[1]
         except Exception as e:
             err = f"The authorization header has a bad syntax: {e}"
             raise InvalidCredentials(
-                err,
-                log_txt=f"Error while trying to get a token from header. " + err
+                err, log_txt=f"Error while trying to get a token from header. " + err
             )
 
     def get_user_from_header(self, headers: Headers = None) -> UserModel:
         """
         Gets the user represented by the token that has to be in the request headers.
 
         :param headers: the request headers
         :type headers: `Headers`
         :return: the user object
         :rtype: `UserBaseModel`
         """
         if headers is None:
             err = "Headers are missing from the request. Authentication was not possible to perform."
             raise InvalidUsage(
-                err,
-                log_txt="Error while trying to get user from header. " + err
+                err, log_txt="Error while trying to get user from header. " + err
             )
         token = self.get_token_from_header(headers)
         data = self.decode_token(token)
         user_id = data["user_id"]
         user = self.user_model.get_one_user(user_id)
         if user is None:
             err = "User does not exist, invalid token."
             raise ObjectDoesNotExist(
-                err,
-                log_txt="Error while trying to get user from header. " + err
+                err, log_txt="Error while trying to get user from header. " + err
             )
         return user
 
     @staticmethod
     def return_user_from_token(token):
         """
         Function used for internal testing. Given a token gives back the user_id encoded in it.
@@ -456,7 +455,61 @@
         :param int provider: the token provider information
         :return: the public key in the token or it raises an error
         :rtype: str
         """
         kid = self._get_key_id(token)
         jwk = self._get_jwk(kid, tenant_id, provider)
         return self._rsa_pem_from_jwk(jwk)
+
+
+class BIAuth(Auth):
+    def __init__(self, user_model=UserModel):
+        super().__init__(user_model)
+
+    @staticmethod
+    def decode_token(token: str = None) -> dict:
+        """
+        Decodes a given JSON Web token and extracts the sub from it to give it back.
+
+        :param str token: the given JSON Web Token
+        :return: the sub field of the token as the user_id
+        :rtype: dict
+        """
+        if token is None:
+            err = "The provided token is not valid."
+            raise InvalidUsage(
+                err, log_txt="Error while trying to decode token. " + err
+            )
+        try:
+            payload = jwt.decode(
+                token, current_app.config["SECRET_BI_KEY"], algorithms="HS256"
+            )
+            return {"user_id": payload["sub"]}
+        except jwt.InvalidTokenError:
+            raise InvalidCredentials(
+                "Invalid token, please try again with a new token",
+                log_txt="Error while trying to decode token. The token is invalid.",
+            )
+
+    @staticmethod
+    def generate_token(user_id: int = None) -> str:
+        """
+        Generates a token given a user_id with a duration of one day
+
+        :param int user_id: user code to be encoded in the token to identify the user afterward.
+        :return: the generated token
+        :rtype: str
+        """
+        if user_id is None:
+            err = "The user id passed to generate the token is not valid."
+            raise InvalidUsage(
+                err, log_txt="Error while trying to generate token. " + err
+            )
+
+        payload = {
+            "iat": datetime.utcnow(),
+            "sub": user_id,
+        }
+
+        return jwt.encode(
+            payload, current_app.config["SECRET_BI_KEY"], algorithm="HS256"
+        )
```

### Comparing `cornflow-1.0.8a3/cornflow/shared/authentication/decorators.py` & `cornflow-1.0.9/cornflow/shared/authentication/decorators.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow/shared/authentication/ldap.py` & `cornflow-1.0.9/cornflow/shared/authentication/ldap.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow/shared/compress.py` & `cornflow-1.0.9/cornflow/shared/compress.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow/shared/const.py` & `cornflow-1.0.9/cornflow/shared/const.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow/shared/email.py` & `cornflow-1.0.9/cornflow/shared/email.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow/shared/exceptions.py` & `cornflow-1.0.9/cornflow/shared/exceptions.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow/shared/licenses.py` & `cornflow-1.0.9/cornflow/shared/licenses.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow/shared/log_config.py` & `cornflow-1.0.9/cornflow/shared/log_config.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow/shared/query_tools.py` & `cornflow-1.0.9/cornflow/shared/query_tools.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow/shared/utils.py` & `cornflow-1.0.9/cornflow/shared/utils.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow/shared/utils_tables.py` & `cornflow-1.0.9/cornflow/shared/utils_tables.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow/shared/validators.py` & `cornflow-1.0.9/cornflow/shared/validators.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow/tests/const.py` & `cornflow-1.0.9/cornflow/tests/const.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow/tests/custom_liveServer.py` & `cornflow-1.0.9/cornflow/tests/custom_liveServer.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow/tests/custom_test_case.py` & `cornflow-1.0.9/cornflow/tests/custom_test_case.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,15 +97,14 @@
             data=json.dumps(data),
             follow_redirects=True,
             headers={"Content-Type": "application/json"},
         )
 
     @staticmethod
     def assign_role(user_id, role_id):
-
         if UserRoleModel.check_if_role_assigned(user_id, role_id):
             user_role = UserRoleModel.query.filter_by(
                 user_id=user_id, role_id=role_id
             ).first()
         else:
             user_role = UserRoleModel({"user_id": user_id, "role_id": role_id})
             user_role.save()
@@ -284,15 +283,14 @@
         )
 
         self.assertEqual(expected_status, row.status_code)
         self.assertEqual(payload_to_check["data"], row.json["data"])
         self.assertEqual(payload_to_check["solution"], row.json["solution"])
 
     def delete_row(self, url):
-
         response = self.client.delete(
             url, follow_redirects=True, headers=self.get_header_with_auth(self.token)
         )
         self.assertEqual(200, response.status_code)
 
         response = self.client.get(
             url, follow_redirects=True, headers=self.get_header_with_auth(self.token)
@@ -729,15 +727,15 @@
                 headers={"Content-Type": "application/json"},
             )
 
             self.assertEqual(200, self.response.status_code)
             self.assertEqual(str, type(self.response.json["token"]))
             decoded_token = jwt.decode(
                 self.response.json["token"],
-                current_app.config["SECRET_KEY"],
+                current_app.config["SECRET_TOKEN_KEY"],
                 algorithms="HS256",
             )
 
             self.assertAlmostEqual(
                 datetime.utcnow(),
                 datetime.utcfromtimestamp(decoded_token["iat"]),
                 delta=timedelta(seconds=2),
```

### Comparing `cornflow-1.0.8a3/cornflow/tests/integration/test_commands.py` & `cornflow-1.0.9/cornflow/tests/integration/test_commands.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow/tests/integration/test_cornflowclient.py` & `cornflow-1.0.9/cornflow/tests/integration/test_cornflowclient.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow/tests/ldap/test_ldap_authentication.py` & `cornflow-1.0.9/cornflow/tests/ldap/test_ldap_authentication.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow/tests/unit/test_actions.py` & `cornflow-1.0.9/cornflow/tests/unit/test_actions.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow/tests/unit/test_alarms.py` & `cornflow-1.0.9/cornflow/tests/unit/test_alarms.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow/tests/unit/test_apiview.py` & `cornflow-1.0.9/cornflow/tests/unit/test_apiview.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow/tests/unit/test_cases.py` & `cornflow-1.0.9/cornflow/tests/unit/test_cases.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow/tests/unit/test_cli.py` & `cornflow-1.0.9/cornflow/tests/unit/test_cli.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 import configparser
 import os
 
 from click.testing import CliRunner
+from flask_testing import TestCase
+
 from cornflow.app import create_app
 from cornflow.cli import cli
-from cornflow.models import UserModel
 from cornflow.models import (
     ActionModel,
     RoleModel,
     ViewModel,
     PermissionViewRoleModel,
 )
+from cornflow.models import UserModel
 from cornflow.shared import db
-from flask_testing import TestCase
+from cornflow.shared.exceptions import NoPermission, ObjectDoesNotExist
 
 
 class CLITests(TestCase):
     def setUp(self):
         db.create_all()
 
     def tearDown(self):
@@ -204,25 +206,163 @@
         self.assertIn("The password of the user", result.output)
         self.assertIn("password", result.output)
         self.assertIn("The email of the user", result.output)
         self.assertIn("email", result.output)
 
     def test_service_user_command(self):
         runner = CliRunner()
+        self.test_roles_init_command()
         result = runner.invoke(
             cli,
             [
                 "users",
                 "create",
                 "service",
                 "-u",
                 "test",
                 "-p",
                 "testPassword1!",
                 "-e",
                 "test@test.org",
             ],
         )
-        self.assertEqual(result.exit_code, 1)
+        self.assertEqual(result.exit_code, 0)
         user = UserModel.get_one_user_by_email("test@test.org")
         self.assertEqual(user.username, "test")
         self.assertEqual(user.email, "test@test.org")
+        self.assertEqual(user.roles, {4: "service"})
+        self.assertTrue(user.is_service_user())
+
+    def test_viewer_user_command(self):
+        runner = CliRunner()
+        self.test_roles_init_command()
+        result = runner.invoke(
+            cli,
+            [
+                "users",
+                "create",
+                "viewer",
+                "-u",
+                "test",
+                "-p",
+                "testPassword1!",
+                "-e",
+                "test@test.org",
+            ],
+        )
+
+        self.assertEqual(result.exit_code, 0)
+        user = UserModel.get_one_user_by_email("test@test.org")
+        self.assertEqual(user.username, "test")
+        self.assertEqual(user.email, "test@test.org")
+        self.assertEqual(user.roles, {1: "viewer"})
+        self.assertFalse(user.is_service_user())
+
+    def test_generate_token(self):
+        runner = CliRunner()
+
+        self.test_roles_init_command()
+
+        result = runner.invoke(
+            cli,
+            [
+                "users",
+                "create",
+                "viewer",
+                "-u",
+                "viewer_user",
+                "-p",
+                "testPassword1!",
+                "-e",
+                "viewer@test.org",
+            ],
+        )
+
+        self.assertEqual(result.exit_code, 0)
+
+        user_id = UserModel.get_one_user_by_username("viewer_user").id
+
+        result = runner.invoke(
+            cli,
+            [
+                "users",
+                "create",
+                "service",
+                "-u",
+                "test",
+                "-p",
+                "testPassword1!",
+                "-e",
+                "test@test.org",
+            ],
+        )
+
+        self.assertEqual(result.exit_code, 0)
+
+        result = runner.invoke(
+            cli,
+            [
+                "users",
+                "create",
+                "token",
+                "-i",
+                user_id,
+                "-u",
+                "test",
+                "-p",
+                "testPassword1!",
+            ],
+        )
+
+        self.assertIn("ey", result.output)
+
+        result = runner.invoke(
+            cli,
+            [
+                "users",
+                "create",
+                "token",
+                "-i",
+                user_id,
+                "-u",
+                "test",
+                "-p",
+                "Otherpassword",
+            ],
+        )
+
+        self.assertEqual(result.exit_code, 1)
+        self.assertIsInstance(result.exception, NoPermission)
+
+        result = runner.invoke(
+            cli,
+            [
+                "users",
+                "create",
+                "token",
+                "-i",
+                user_id,
+                "-u",
+                "viewer_user",
+                "-p",
+                "testPassword1!",
+            ],
+        )
+
+        self.assertIsInstance(result.exception, NoPermission)
+
+        result = runner.invoke(
+            cli,
+            [
+                "users",
+                "create",
+                "token",
+                "-i",
+                100,
+                "-u",
+                "test",
+                "-p",
+                "testPassword1!",
+            ],
+        )
+
+        self.assertIsInstance(result.exception, ObjectDoesNotExist)
```

### Comparing `cornflow-1.0.8a3/cornflow/tests/unit/test_commands.py` & `cornflow-1.0.9/cornflow/tests/unit/test_commands.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow/tests/unit/test_dags.py` & `cornflow-1.0.9/cornflow/tests/unit/test_dags.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow/tests/unit/test_data_checks.py` & `cornflow-1.0.9/cornflow/tests/unit/test_data_checks.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow/tests/unit/test_example_data.py` & `cornflow-1.0.9/cornflow/tests/unit/test_example_data.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow/tests/unit/test_executions.py` & `cornflow-1.0.9/cornflow/tests/unit/test_executions.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow/tests/unit/test_generate_from_schema.py` & `cornflow-1.0.9/cornflow/tests/unit/test_generate_from_schema.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow/tests/unit/test_health.py` & `cornflow-1.0.9/cornflow/tests/unit/test_health.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow/tests/unit/test_instances.py` & `cornflow-1.0.9/cornflow/tests/unit/test_instances.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow/tests/unit/test_instances_file.py` & `cornflow-1.0.9/cornflow/tests/unit/test_instances_file.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow/tests/unit/test_licenses.py` & `cornflow-1.0.9/cornflow/tests/unit/test_licenses.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow/tests/unit/test_log_in.py` & `cornflow-1.0.9/cornflow/tests/unit/test_log_in.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow/tests/unit/test_main_alarms.py` & `cornflow-1.0.9/cornflow/tests/unit/test_main_alarms.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow/tests/unit/test_permissions.py` & `cornflow-1.0.9/cornflow/tests/unit/test_permissions.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow/tests/unit/test_roles.py` & `cornflow-1.0.9/cornflow/tests/unit/test_roles.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow/tests/unit/test_schema_from_models.py` & `cornflow-1.0.9/cornflow/tests/unit/test_schema_from_models.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow/tests/unit/test_schemas.py` & `cornflow-1.0.9/cornflow/tests/unit/test_schemas.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow/tests/unit/test_sign_up.py` & `cornflow-1.0.9/cornflow/tests/unit/test_sign_up.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow/tests/unit/test_tables.py` & `cornflow-1.0.9/cornflow/tests/unit/test_tables.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow/tests/unit/test_token.py` & `cornflow-1.0.9/cornflow/tests/unit/test_token.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """
 Unit test for the token endpoint
 """
+import json
 
-# Import from libraries
 from flask import current_app
-import json
 
-# Import from internal modules
 from cornflow.models import UserModel
 from cornflow.shared import db
-from cornflow.tests.custom_test_case import CheckTokenTestCase
+from cornflow.shared.authentication.auth import BIAuth, Auth
+from cornflow.shared.exceptions import InvalidUsage
 from cornflow.tests.const import LOGIN_URL
+from cornflow.tests.custom_test_case import CheckTokenTestCase, CustomTestCase
 
 
 class TestCheckToken(CheckTokenTestCase.TokenEndpoint):
     def setUp(self):
         super().setUp()
         db.create_all()
         self.AUTH_TYPE = current_app.config["AUTH_TYPE"]
@@ -60,7 +60,38 @@
             "eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJleHAiOjE2MTA1MzYwNjUsImlhdCI6MTYxMDQ0OTY2NSwic3ViIjoxfQ"
             ".QEfmO-hh55PjtecnJ1RJT3aW2brGLadkg5ClH9yrRnc "
         )
 
         self.get_check_token()
         self.assertEqual(200, self.response.status_code)
         self.assertEqual(0, self.response.json["valid"])
+
+
+class TestUnexpiringToken(CustomTestCase):
+    def test_token_unexpiring(self):
+        auth = BIAuth()
+
+        token = auth.generate_token(1)
+
+        response = auth.decode_token(token)
+        self.assertEqual(response, {"user_id": 1})
+
+        token = "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpYXQiOjE3MDM1OTI1OTIsInN1YiI6MX0.Plvmi02FMfZOTn6bxArELEmDeyuP-2X794c5VtAFgCg"
+
+        response = auth.decode_token(token)
+        self.assertEqual(response, {"user_id": 1})
+
+    def test_user_not_valid(self):
+        auth = BIAuth()
+        self.assertRaises(InvalidUsage, auth.generate_token, None)
+
+        auth = Auth()
+        self.assertRaises(InvalidUsage, auth.generate_token, None)
+
+    def test_token_not_valid(self):
+        auth = BIAuth()
+        self.assertRaises(InvalidUsage, auth.decode_token, None)
+        token = ""
+        self.assertRaises(InvalidUsage, auth.decode_token, token)
+
+        auth = Auth()
+        self.assertRaises(InvalidUsage, auth.decode_token, None)
```

### Comparing `cornflow-1.0.8a3/cornflow/tests/unit/test_users.py` & `cornflow-1.0.9/cornflow/tests/unit/test_users.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow/tests/unit/tools.py` & `cornflow-1.0.9/cornflow/tests/unit/tools.py`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow.egg-info/PKG-INFO` & `cornflow-1.0.9/cornflow.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: cornflow
-Version: 1.0.8a3
+Version: 1.0.9
 Summary: Cornflow is an open source multi-solver optimization server with a REST API built using flask.
 Home-page: https://github.com/baobabsoluciones/cornflow
 Author: baobab soluciones
 Author-email: cornflow@baobabsoluciones.es
 License: UNKNOWN
 Description: Cornflow
         =========
```

### Comparing `cornflow-1.0.8a3/cornflow.egg-info/SOURCES.txt` & `cornflow-1.0.9/cornflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cornflow-1.0.8a3/cornflow.egg-info/requires.txt` & `cornflow-1.0.9/cornflow.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 alembic==1.9.2
 apispec<=6.2.0
 click<=8.1.3
-cornflow-client==1.0.16a2
+cornflow-client<=1.0.16
 cryptography<=39.0.2
 disposable-email-domains>=0.0.86
 Flask==2.3.2
 flask-apispec<=0.11.4
 Flask-Bcrypt<=1.0.1
 Flask-Compress<=1.13
 flask-cors<=3.0.10
```

### Comparing `cornflow-1.0.8a3/setup.py` & `cornflow-1.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 required = []
 with open("requirements.txt", "r") as fh:
     required.append(fh.read().splitlines())
 
 setuptools.setup(
     name="cornflow",
-    version="1.0.8a3",
+    version="1.0.9",
     author="baobab soluciones",
     author_email="cornflow@baobabsoluciones.es",
     description="Cornflow is an open source multi-solver optimization server with a REST API built using flask.",
     long_description=long_description,
     url="https://github.com/baobabsoluciones/cornflow",
     packages=setuptools.find_packages(),
     install_requires=required,
```

