# Comparing `tmp/frequenz-api-microgrid-0.16.1.tar.gz` & `tmp/frequenz-api-microgrid-0.17.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frequenz-api-microgrid-0.16.1.tar", last modified: Mon Mar 25 17:13:45 2024, max compression
+gzip compressed data, was "frequenz-api-microgrid-0.17.0.tar", last modified: Fri May 10 15:08:04 2024, max compression
```

## Comparing `frequenz-api-microgrid-0.16.1.tar` & `frequenz-api-microgrid-0.17.0.tar`

### file list

```diff
@@ -1,128 +1,139 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 17:13:45.120935 frequenz-api-microgrid-0.16.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-03-25 17:13:26.000000 frequenz-api-microgrid-0.16.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-03-25 17:13:26.000000 frequenz-api-microgrid-0.16.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6468 2024-03-25 17:13:45.120935 frequenz-api-microgrid-0.16.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5198 2024-03-25 17:13:26.000000 frequenz-api-microgrid-0.16.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-03-25 17:13:26.000000 frequenz-api-microgrid-0.16.1/RELEASE_NOTES.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 17:13:45.104935 frequenz-api-microgrid-0.16.1/proto/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 17:13:45.104935 frequenz-api-microgrid-0.16.1/proto/frequenz/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 17:13:45.104935 frequenz-api-microgrid-0.16.1/proto/frequenz/api/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 17:13:45.104935 frequenz-api-microgrid-0.16.1/proto/frequenz/api/microgrid/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 17:13:45.108935 frequenz-api-microgrid-0.16.1/proto/frequenz/api/microgrid/v1/
--rw-r--r--   0 runner    (1001) docker     (127)    23818 2024-03-25 17:13:26.000000 frequenz-api-microgrid-0.16.1/proto/frequenz/api/microgrid/v1/microgrid.proto
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 17:13:45.108935 frequenz-api-microgrid-0.16.1/py/
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-03-25 17:13:26.000000 frequenz-api-microgrid-0.16.1/py/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 17:13:45.104935 frequenz-api-microgrid-0.16.1/py/frequenz/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 17:13:45.104935 frequenz-api-microgrid-0.16.1/py/frequenz/api/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 17:13:45.108935 frequenz-api-microgrid-0.16.1/py/frequenz/api/microgrid/
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-03-25 17:13:26.000000 frequenz-api-microgrid-0.16.1/py/frequenz/api/microgrid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 17:13:26.000000 frequenz-api-microgrid-0.16.1/py/frequenz/api/microgrid/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 17:13:45.108935 frequenz-api-microgrid-0.16.1/py/frequenz/api/microgrid/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-03-25 17:13:26.000000 frequenz-api-microgrid-0.16.1/py/frequenz/api/microgrid/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 17:13:45.108935 frequenz-api-microgrid-0.16.1/py/frequenz_api_microgrid.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6468 2024-03-25 17:13:45.000000 frequenz-api-microgrid-0.16.1/py/frequenz_api_microgrid.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5075 2024-03-25 17:13:45.000000 frequenz-api-microgrid-0.16.1/py/frequenz_api_microgrid.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 17:13:45.000000 frequenz-api-microgrid-0.16.1/py/frequenz_api_microgrid.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-03-25 17:13:45.000000 frequenz-api-microgrid-0.16.1/py/frequenz_api_microgrid.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-25 17:13:45.000000 frequenz-api-microgrid-0.16.1/py/frequenz_api_microgrid.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4587 2024-03-25 17:13:26.000000 frequenz-api-microgrid-0.16.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-25 17:13:45.120935 frequenz-api-microgrid-0.16.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 17:13:45.108935 frequenz-api-microgrid-0.16.1/submodules/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 17:13:45.104935 frequenz-api-microgrid-0.16.1/submodules/api-common-protos/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 17:13:45.108935 frequenz-api-microgrid-0.16.1/submodules/api-common-protos/google/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 17:13:45.116935 frequenz-api-microgrid-0.16.1/submodules/api-common-protos/google/api/
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-03-25 17:13:27.000000 frequenz-api-microgrid-0.16.1/submodules/api-common-protos/google/api/annotations.proto
--rw-r--r--   0 runner    (1001) docker     (127)     7374 2024-03-25 17:13:27.000000 frequenz-api-microgrid-0.16.1/submodules/api-common-protos/google/api/auth.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-03-25 17:13:27.000000 frequenz-api-microgrid-0.16.1/submodules/api-common-protos/google/api/backend.proto
--rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-03-25 17:13:27.000000 frequenz-api-microgrid-0.16.1/submodules/api-common-protos/google/api/billing.proto
--rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-03-25 17:13:27.000000 frequenz-api-microgrid-0.16.1/submodules/api-common-protos/google/api/client.proto
--rw-r--r--   0 runner    (1001) docker     (127)     3169 2024-03-25 17:13:27.000000 frequenz-api-microgrid-0.16.1/submodules/api-common-protos/google/api/config_change.proto
--rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-03-25 17:13:27.000000 frequenz-api-microgrid-0.16.1/submodules/api-common-protos/google/api/consumer.proto
--rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-03-25 17:13:27.000000 frequenz-api-microgrid-0.16.1/submodules/api-common-protos/google/api/context.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-03-25 17:13:27.000000 frequenz-api-microgrid-0.16.1/submodules/api-common-protos/google/api/control.proto
--rw-r--r--   0 runner    (1001) docker     (127)     8657 2024-03-25 17:13:27.000000 frequenz-api-microgrid-0.16.1/submodules/api-common-protos/google/api/distribution.proto
--rw-r--r--   0 runner    (1001) docker     (127)     6132 2024-03-25 17:13:27.000000 frequenz-api-microgrid-0.16.1/submodules/api-common-protos/google/api/documentation.proto
--rw-r--r--   0 runner    (1001) docker     (127)     2824 2024-03-25 17:13:27.000000 frequenz-api-microgrid-0.16.1/submodules/api-common-protos/google/api/endpoint.proto
--rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-03-25 17:13:27.000000 frequenz-api-microgrid-0.16.1/submodules/api-common-protos/google/api/field_behavior.proto
--rw-r--r--   0 runner    (1001) docker     (127)    12099 2024-03-25 17:13:27.000000 frequenz-api-microgrid-0.16.1/submodules/api-common-protos/google/api/http.proto
--rw-r--r--   0 runner    (1001) docker     (127)     2605 2024-03-25 17:13:27.000000 frequenz-api-microgrid-0.16.1/submodules/api-common-protos/google/api/httpbody.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-03-25 17:13:27.000000 frequenz-api-microgrid-0.16.1/submodules/api-common-protos/google/api/label.proto
--rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-03-25 17:13:27.000000 frequenz-api-microgrid-0.16.1/submodules/api-common-protos/google/api/launch_stage.proto
--rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-03-25 17:13:27.000000 frequenz-api-microgrid-0.16.1/submodules/api-common-protos/google/api/log.proto
--rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-03-25 17:13:27.000000 frequenz-api-microgrid-0.16.1/submodules/api-common-protos/google/api/logging.proto
--rw-r--r--   0 runner    (1001) docker     (127)     6628 2024-03-25 17:13:27.000000 frequenz-api-microgrid-0.16.1/submodules/api-common-protos/google/api/metric.proto
--rw-r--r--   0 runner    (1001) docker     (127)     5512 2024-03-25 17:13:27.000000 frequenz-api-microgrid-0.16.1/submodules/api-common-protos/google/api/monitored_resource.proto
--rw-r--r--   0 runner    (1001) docker     (127)     3524 2024-03-25 17:13:27.000000 frequenz-api-microgrid-0.16.1/submodules/api-common-protos/google/api/monitoring.proto
--rw-r--r--   0 runner    (1001) docker     (127)    10854 2024-03-25 17:13:27.000000 frequenz-api-microgrid-0.16.1/submodules/api-common-protos/google/api/quota.proto
--rw-r--r--   0 runner    (1001) docker     (127)    11347 2024-03-25 17:13:27.000000 frequenz-api-microgrid-0.16.1/submodules/api-common-protos/google/api/resource.proto
--rw-r--r--   0 runner    (1001) docker     (127)    14929 2024-03-25 17:13:27.000000 frequenz-api-microgrid-0.16.1/submodules/api-common-protos/google/api/routing.proto
--rw-r--r--   0 runner    (1001) docker     (127)     6099 2024-03-25 17:13:27.000000 frequenz-api-microgrid-0.16.1/submodules/api-common-protos/google/api/service.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-03-25 17:13:27.000000 frequenz-api-microgrid-0.16.1/submodules/api-common-protos/google/api/source_info.proto
--rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-03-25 17:13:27.000000 frequenz-api-microgrid-0.16.1/submodules/api-common-protos/google/api/system_parameter.proto
--rw-r--r--   0 runner    (1001) docker     (127)     3513 2024-03-25 17:13:27.000000 frequenz-api-microgrid-0.16.1/submodules/api-common-protos/google/api/usage.proto
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 17:13:45.116935 frequenz-api-microgrid-0.16.1/submodules/api-common-protos/google/cloud/
--rw-r--r--   0 runner    (1001) docker     (127)     6308 2024-03-25 17:13:27.000000 frequenz-api-microgrid-0.16.1/submodules/api-common-protos/google/cloud/extended_operations.proto
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 17:13:45.104935 frequenz-api-microgrid-0.16.1/submodules/api-common-protos/google/iam/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 17:13:45.104935 frequenz-api-microgrid-0.16.1/submodules/api-common-protos/google/iam/admin/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 17:13:45.116935 frequenz-api-microgrid-0.16.1/submodules/api-common-protos/google/iam/admin/v1/
--rw-r--r--   0 runner    (1001) docker     (127)    41483 2024-03-25 17:13:27.000000 frequenz-api-microgrid-0.16.1/submodules/api-common-protos/google/iam/admin/v1/iam.proto
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 17:13:45.116935 frequenz-api-microgrid-0.16.1/submodules/api-common-protos/google/iam/v1/
--rw-r--r--   0 runner    (1001) docker     (127)     5482 2024-03-25 17:13:27.000000 frequenz-api-microgrid-0.16.1/submodules/api-common-protos/google/iam/v1/iam_policy.proto
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 17:13:45.116935 frequenz-api-microgrid-0.16.1/submodules/api-common-protos/google/iam/v1/logging/
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-03-25 17:13:27.000000 frequenz-api-microgrid-0.16.1/submodules/api-common-protos/google/iam/v1/logging/audit_data.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-03-25 17:13:27.000000 frequenz-api-microgrid-0.16.1/submodules/api-common-protos/google/iam/v1/options.proto
--rw-r--r--   0 runner    (1001) docker     (127)     8659 2024-03-25 17:13:27.000000 frequenz-api-microgrid-0.16.1/submodules/api-common-protos/google/iam/v1/policy.proto
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 17:13:45.108935 frequenz-api-microgrid-0.16.1/submodules/api-common-protos/google/logging/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 17:13:45.116935 frequenz-api-microgrid-0.16.1/submodules/api-common-protos/google/logging/type/
--rw-r--r--   0 runner    (1001) docker     (127)     3389 2024-03-25 17:13:27.000000 frequenz-api-microgrid-0.16.1/submodules/api-common-protos/google/logging/type/http_request.proto
--rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-03-25 17:13:27.000000 frequenz-api-microgrid-0.16.1/submodules/api-common-protos/google/logging/type/log_severity.proto
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 17:13:45.116935 frequenz-api-microgrid-0.16.1/submodules/api-common-protos/google/longrunning/
--rw-r--r--   0 runner    (1001) docker     (127)    10515 2024-03-25 17:13:27.000000 frequenz-api-microgrid-0.16.1/submodules/api-common-protos/google/longrunning/operations.proto
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 17:13:45.116935 frequenz-api-microgrid-0.16.1/submodules/api-common-protos/google/rpc/
--rw-r--r--   0 runner    (1001) docker     (127)     7125 2024-03-25 17:13:27.000000 frequenz-api-microgrid-0.16.1/submodules/api-common-protos/google/rpc/code.proto
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 17:13:45.116935 frequenz-api-microgrid-0.16.1/submodules/api-common-protos/google/rpc/context/
--rw-r--r--   0 runner    (1001) docker     (127)    12015 2024-03-25 17:13:27.000000 frequenz-api-microgrid-0.16.1/submodules/api-common-protos/google/rpc/context/attribute_context.proto
--rw-r--r--   0 runner    (1001) docker     (127)     9504 2024-03-25 17:13:27.000000 frequenz-api-microgrid-0.16.1/submodules/api-common-protos/google/rpc/error_details.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-03-25 17:13:27.000000 frequenz-api-microgrid-0.16.1/submodules/api-common-protos/google/rpc/status.proto
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 17:13:45.120935 frequenz-api-microgrid-0.16.1/submodules/api-common-protos/google/type/
--rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-03-25 17:13:27.000000 frequenz-api-microgrid-0.16.1/submodules/api-common-protos/google/type/calendar_period.proto
--rw-r--r--   0 runner    (1001) docker     (127)     6193 2024-03-25 17:13:27.000000 frequenz-api-microgrid-0.16.1/submodules/api-common-protos/google/type/color.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-03-25 17:13:27.000000 frequenz-api-microgrid-0.16.1/submodules/api-common-protos/google/type/date.proto
--rw-r--r--   0 runner    (1001) docker     (127)     3508 2024-03-25 17:13:27.000000 frequenz-api-microgrid-0.16.1/submodules/api-common-protos/google/type/datetime.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-03-25 17:13:27.000000 frequenz-api-microgrid-0.16.1/submodules/api-common-protos/google/type/dayofweek.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-03-25 17:13:27.000000 frequenz-api-microgrid-0.16.1/submodules/api-common-protos/google/type/expr.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-03-25 17:13:27.000000 frequenz-api-microgrid-0.16.1/submodules/api-common-protos/google/type/fraction.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-03-25 17:13:27.000000 frequenz-api-microgrid-0.16.1/submodules/api-common-protos/google/type/latlng.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-03-25 17:13:27.000000 frequenz-api-microgrid-0.16.1/submodules/api-common-protos/google/type/money.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-03-25 17:13:27.000000 frequenz-api-microgrid-0.16.1/submodules/api-common-protos/google/type/month.proto
--rw-r--r--   0 runner    (1001) docker     (127)     6239 2024-03-25 17:13:27.000000 frequenz-api-microgrid-0.16.1/submodules/api-common-protos/google/type/postal_address.proto
--rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-03-25 17:13:27.000000 frequenz-api-microgrid-0.16.1/submodules/api-common-protos/google/type/quaternion.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-03-25 17:13:27.000000 frequenz-api-microgrid-0.16.1/submodules/api-common-protos/google/type/timeofday.proto
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 17:13:45.108935 frequenz-api-microgrid-0.16.1/submodules/frequenz-api-common/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 17:13:45.108935 frequenz-api-microgrid-0.16.1/submodules/frequenz-api-common/proto/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 17:13:45.108935 frequenz-api-microgrid-0.16.1/submodules/frequenz-api-common/proto/frequenz/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 17:13:45.108935 frequenz-api-microgrid-0.16.1/submodules/frequenz-api-common/proto/frequenz/api/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 17:13:45.108935 frequenz-api-microgrid-0.16.1/submodules/frequenz-api-common/proto/frequenz/api/common/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 17:13:45.120935 frequenz-api-microgrid-0.16.1/submodules/frequenz-api-common/proto/frequenz/api/common/v1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 17:13:45.120935 frequenz-api-microgrid-0.16.1/submodules/frequenz-api-common/proto/frequenz/api/common/v1/grid/
--rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-03-25 17:13:27.000000 frequenz-api-microgrid-0.16.1/submodules/frequenz-api-common/proto/frequenz/api/common/v1/grid/delivery_area.proto
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-03-25 17:13:27.000000 frequenz-api-microgrid-0.16.1/submodules/frequenz-api-common/proto/frequenz/api/common/v1/location.proto
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 17:13:45.120935 frequenz-api-microgrid-0.16.1/submodules/frequenz-api-common/proto/frequenz/api/common/v1/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-03-25 17:13:27.000000 frequenz-api-microgrid-0.16.1/submodules/frequenz-api-common/proto/frequenz/api/common/v1/metrics/bounds.proto
--rw-r--r--   0 runner    (1001) docker     (127)     6989 2024-03-25 17:13:27.000000 frequenz-api-microgrid-0.16.1/submodules/frequenz-api-common/proto/frequenz/api/common/v1/metrics/metric_sample.proto
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 17:13:45.120935 frequenz-api-microgrid-0.16.1/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 17:13:45.120935 frequenz-api-microgrid-0.16.1/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-03-25 17:13:27.000000 frequenz-api-microgrid-0.16.1/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/battery.proto
--rw-r--r--   0 runner    (1001) docker     (127)    16612 2024-03-25 17:13:27.000000 frequenz-api-microgrid-0.16.1/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/components.proto
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-03-25 17:13:27.000000 frequenz-api-microgrid-0.16.1/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/ev_charger.proto
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-03-25 17:13:27.000000 frequenz-api-microgrid-0.16.1/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/fuse.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-03-25 17:13:27.000000 frequenz-api-microgrid-0.16.1/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/grid.proto
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-03-25 17:13:27.000000 frequenz-api-microgrid-0.16.1/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/inverter.proto
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-03-25 17:13:27.000000 frequenz-api-microgrid-0.16.1/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/transformer.proto
--rw-r--r--   0 runner    (1001) docker     (127)      966 2024-03-25 17:13:27.000000 frequenz-api-microgrid-0.16.1/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/lifetime.proto
--rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-03-25 17:13:27.000000 frequenz-api-microgrid-0.16.1/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/microgrid.proto
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 17:13:45.120935 frequenz-api-microgrid-0.16.1/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/sensors/
--rw-r--r--   0 runner    (1001) docker     (127)     5595 2024-03-25 17:13:27.000000 frequenz-api-microgrid-0.16.1/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/sensors/sensors.proto
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 17:13:45.120935 frequenz-api-microgrid-0.16.1/submodules/frequenz-api-common/proto/frequenz/api/common/v1/pagination/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-03-25 17:13:27.000000 frequenz-api-microgrid-0.16.1/submodules/frequenz-api-common/proto/frequenz/api/common/v1/pagination/pagination_info.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-03-25 17:13:27.000000 frequenz-api-microgrid-0.16.1/submodules/frequenz-api-common/proto/frequenz/api/common/v1/pagination/pagination_params.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:08:04.297415 frequenz-api-microgrid-0.17.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-10 15:07:53.000000 frequenz-api-microgrid-0.17.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-10 15:07:53.000000 frequenz-api-microgrid-0.17.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6468 2024-05-10 15:08:04.297415 frequenz-api-microgrid-0.17.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5198 2024-05-10 15:07:53.000000 frequenz-api-microgrid-0.17.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-05-10 15:07:53.000000 frequenz-api-microgrid-0.17.0/RELEASE_NOTES.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:08:04.277415 frequenz-api-microgrid-0.17.0/proto/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:08:04.277415 frequenz-api-microgrid-0.17.0/proto/frequenz/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:08:04.277415 frequenz-api-microgrid-0.17.0/proto/frequenz/api/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:08:04.277415 frequenz-api-microgrid-0.17.0/proto/frequenz/api/microgrid/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:08:04.281415 frequenz-api-microgrid-0.17.0/proto/frequenz/api/microgrid/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)    21575 2024-05-10 15:07:53.000000 frequenz-api-microgrid-0.17.0/proto/frequenz/api/microgrid/v1/microgrid.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:08:04.281415 frequenz-api-microgrid-0.17.0/py/
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-10 15:07:53.000000 frequenz-api-microgrid-0.17.0/py/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:08:04.277415 frequenz-api-microgrid-0.17.0/py/frequenz/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:08:04.277415 frequenz-api-microgrid-0.17.0/py/frequenz/api/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:08:04.281415 frequenz-api-microgrid-0.17.0/py/frequenz/api/microgrid/
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-10 15:07:53.000000 frequenz-api-microgrid-0.17.0/py/frequenz/api/microgrid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 15:07:53.000000 frequenz-api-microgrid-0.17.0/py/frequenz/api/microgrid/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:08:04.281415 frequenz-api-microgrid-0.17.0/py/frequenz/api/microgrid/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-10 15:07:53.000000 frequenz-api-microgrid-0.17.0/py/frequenz/api/microgrid/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:08:04.285415 frequenz-api-microgrid-0.17.0/py/frequenz_api_microgrid.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6468 2024-05-10 15:08:04.000000 frequenz-api-microgrid-0.17.0/py/frequenz_api_microgrid.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5702 2024-05-10 15:08:04.000000 frequenz-api-microgrid-0.17.0/py/frequenz_api_microgrid.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 15:08:04.000000 frequenz-api-microgrid-0.17.0/py/frequenz_api_microgrid.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-05-10 15:08:04.000000 frequenz-api-microgrid-0.17.0/py/frequenz_api_microgrid.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-10 15:08:04.000000 frequenz-api-microgrid-0.17.0/py/frequenz_api_microgrid.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4589 2024-05-10 15:07:53.000000 frequenz-api-microgrid-0.17.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 15:08:04.297415 frequenz-api-microgrid-0.17.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:08:04.281415 frequenz-api-microgrid-0.17.0/submodules/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:08:04.277415 frequenz-api-microgrid-0.17.0/submodules/api-common-protos/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:08:04.281415 frequenz-api-microgrid-0.17.0/submodules/api-common-protos/google/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:08:04.289415 frequenz-api-microgrid-0.17.0/submodules/api-common-protos/google/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-10 15:07:53.000000 frequenz-api-microgrid-0.17.0/submodules/api-common-protos/google/api/annotations.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     7374 2024-05-10 15:07:53.000000 frequenz-api-microgrid-0.17.0/submodules/api-common-protos/google/api/auth.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-05-10 15:07:53.000000 frequenz-api-microgrid-0.17.0/submodules/api-common-protos/google/api/backend.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-05-10 15:07:53.000000 frequenz-api-microgrid-0.17.0/submodules/api-common-protos/google/api/billing.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-05-10 15:07:53.000000 frequenz-api-microgrid-0.17.0/submodules/api-common-protos/google/api/client.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     3169 2024-05-10 15:07:53.000000 frequenz-api-microgrid-0.17.0/submodules/api-common-protos/google/api/config_change.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-05-10 15:07:53.000000 frequenz-api-microgrid-0.17.0/submodules/api-common-protos/google/api/consumer.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-05-10 15:07:53.000000 frequenz-api-microgrid-0.17.0/submodules/api-common-protos/google/api/context.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-05-10 15:07:53.000000 frequenz-api-microgrid-0.17.0/submodules/api-common-protos/google/api/control.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     8657 2024-05-10 15:07:53.000000 frequenz-api-microgrid-0.17.0/submodules/api-common-protos/google/api/distribution.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     6132 2024-05-10 15:07:53.000000 frequenz-api-microgrid-0.17.0/submodules/api-common-protos/google/api/documentation.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     2824 2024-05-10 15:07:53.000000 frequenz-api-microgrid-0.17.0/submodules/api-common-protos/google/api/endpoint.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-05-10 15:07:53.000000 frequenz-api-microgrid-0.17.0/submodules/api-common-protos/google/api/field_behavior.proto
+-rw-r--r--   0 runner    (1001) docker     (127)    12099 2024-05-10 15:07:53.000000 frequenz-api-microgrid-0.17.0/submodules/api-common-protos/google/api/http.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     2605 2024-05-10 15:07:53.000000 frequenz-api-microgrid-0.17.0/submodules/api-common-protos/google/api/httpbody.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-05-10 15:07:53.000000 frequenz-api-microgrid-0.17.0/submodules/api-common-protos/google/api/label.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-05-10 15:07:53.000000 frequenz-api-microgrid-0.17.0/submodules/api-common-protos/google/api/launch_stage.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-05-10 15:07:53.000000 frequenz-api-microgrid-0.17.0/submodules/api-common-protos/google/api/log.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-05-10 15:07:53.000000 frequenz-api-microgrid-0.17.0/submodules/api-common-protos/google/api/logging.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     6628 2024-05-10 15:07:53.000000 frequenz-api-microgrid-0.17.0/submodules/api-common-protos/google/api/metric.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     5512 2024-05-10 15:07:53.000000 frequenz-api-microgrid-0.17.0/submodules/api-common-protos/google/api/monitored_resource.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     3524 2024-05-10 15:07:53.000000 frequenz-api-microgrid-0.17.0/submodules/api-common-protos/google/api/monitoring.proto
+-rw-r--r--   0 runner    (1001) docker     (127)    10854 2024-05-10 15:07:53.000000 frequenz-api-microgrid-0.17.0/submodules/api-common-protos/google/api/quota.proto
+-rw-r--r--   0 runner    (1001) docker     (127)    11347 2024-05-10 15:07:53.000000 frequenz-api-microgrid-0.17.0/submodules/api-common-protos/google/api/resource.proto
+-rw-r--r--   0 runner    (1001) docker     (127)    14929 2024-05-10 15:07:53.000000 frequenz-api-microgrid-0.17.0/submodules/api-common-protos/google/api/routing.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     6099 2024-05-10 15:07:53.000000 frequenz-api-microgrid-0.17.0/submodules/api-common-protos/google/api/service.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-05-10 15:07:53.000000 frequenz-api-microgrid-0.17.0/submodules/api-common-protos/google/api/source_info.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-05-10 15:07:53.000000 frequenz-api-microgrid-0.17.0/submodules/api-common-protos/google/api/system_parameter.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     3513 2024-05-10 15:07:53.000000 frequenz-api-microgrid-0.17.0/submodules/api-common-protos/google/api/usage.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:08:04.289415 frequenz-api-microgrid-0.17.0/submodules/api-common-protos/google/cloud/
+-rw-r--r--   0 runner    (1001) docker     (127)     6308 2024-05-10 15:07:53.000000 frequenz-api-microgrid-0.17.0/submodules/api-common-protos/google/cloud/extended_operations.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:08:04.281415 frequenz-api-microgrid-0.17.0/submodules/api-common-protos/google/iam/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:08:04.281415 frequenz-api-microgrid-0.17.0/submodules/api-common-protos/google/iam/admin/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:08:04.289415 frequenz-api-microgrid-0.17.0/submodules/api-common-protos/google/iam/admin/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)    41483 2024-05-10 15:07:53.000000 frequenz-api-microgrid-0.17.0/submodules/api-common-protos/google/iam/admin/v1/iam.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:08:04.289415 frequenz-api-microgrid-0.17.0/submodules/api-common-protos/google/iam/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)     5482 2024-05-10 15:07:53.000000 frequenz-api-microgrid-0.17.0/submodules/api-common-protos/google/iam/v1/iam_policy.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:08:04.289415 frequenz-api-microgrid-0.17.0/submodules/api-common-protos/google/iam/v1/logging/
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-05-10 15:07:53.000000 frequenz-api-microgrid-0.17.0/submodules/api-common-protos/google/iam/v1/logging/audit_data.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-05-10 15:07:53.000000 frequenz-api-microgrid-0.17.0/submodules/api-common-protos/google/iam/v1/options.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     8659 2024-05-10 15:07:53.000000 frequenz-api-microgrid-0.17.0/submodules/api-common-protos/google/iam/v1/policy.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:08:04.281415 frequenz-api-microgrid-0.17.0/submodules/api-common-protos/google/logging/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:08:04.289415 frequenz-api-microgrid-0.17.0/submodules/api-common-protos/google/logging/type/
+-rw-r--r--   0 runner    (1001) docker     (127)     3389 2024-05-10 15:07:53.000000 frequenz-api-microgrid-0.17.0/submodules/api-common-protos/google/logging/type/http_request.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-05-10 15:07:53.000000 frequenz-api-microgrid-0.17.0/submodules/api-common-protos/google/logging/type/log_severity.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:08:04.289415 frequenz-api-microgrid-0.17.0/submodules/api-common-protos/google/longrunning/
+-rw-r--r--   0 runner    (1001) docker     (127)    10515 2024-05-10 15:07:53.000000 frequenz-api-microgrid-0.17.0/submodules/api-common-protos/google/longrunning/operations.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:08:04.289415 frequenz-api-microgrid-0.17.0/submodules/api-common-protos/google/rpc/
+-rw-r--r--   0 runner    (1001) docker     (127)     7125 2024-05-10 15:07:53.000000 frequenz-api-microgrid-0.17.0/submodules/api-common-protos/google/rpc/code.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:08:04.289415 frequenz-api-microgrid-0.17.0/submodules/api-common-protos/google/rpc/context/
+-rw-r--r--   0 runner    (1001) docker     (127)    12015 2024-05-10 15:07:53.000000 frequenz-api-microgrid-0.17.0/submodules/api-common-protos/google/rpc/context/attribute_context.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     9504 2024-05-10 15:07:53.000000 frequenz-api-microgrid-0.17.0/submodules/api-common-protos/google/rpc/error_details.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-05-10 15:07:53.000000 frequenz-api-microgrid-0.17.0/submodules/api-common-protos/google/rpc/status.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:08:04.293415 frequenz-api-microgrid-0.17.0/submodules/api-common-protos/google/type/
+-rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-05-10 15:07:53.000000 frequenz-api-microgrid-0.17.0/submodules/api-common-protos/google/type/calendar_period.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     6193 2024-05-10 15:07:53.000000 frequenz-api-microgrid-0.17.0/submodules/api-common-protos/google/type/color.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-05-10 15:07:53.000000 frequenz-api-microgrid-0.17.0/submodules/api-common-protos/google/type/date.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     3508 2024-05-10 15:07:53.000000 frequenz-api-microgrid-0.17.0/submodules/api-common-protos/google/type/datetime.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-05-10 15:07:53.000000 frequenz-api-microgrid-0.17.0/submodules/api-common-protos/google/type/dayofweek.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-05-10 15:07:53.000000 frequenz-api-microgrid-0.17.0/submodules/api-common-protos/google/type/expr.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-10 15:07:53.000000 frequenz-api-microgrid-0.17.0/submodules/api-common-protos/google/type/fraction.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-05-10 15:07:53.000000 frequenz-api-microgrid-0.17.0/submodules/api-common-protos/google/type/latlng.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-05-10 15:07:53.000000 frequenz-api-microgrid-0.17.0/submodules/api-common-protos/google/type/money.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-05-10 15:07:53.000000 frequenz-api-microgrid-0.17.0/submodules/api-common-protos/google/type/month.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     6239 2024-05-10 15:07:53.000000 frequenz-api-microgrid-0.17.0/submodules/api-common-protos/google/type/postal_address.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-05-10 15:07:53.000000 frequenz-api-microgrid-0.17.0/submodules/api-common-protos/google/type/quaternion.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-05-10 15:07:53.000000 frequenz-api-microgrid-0.17.0/submodules/api-common-protos/google/type/timeofday.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:08:04.281415 frequenz-api-microgrid-0.17.0/submodules/frequenz-api-common/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:08:04.281415 frequenz-api-microgrid-0.17.0/submodules/frequenz-api-common/proto/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:08:04.281415 frequenz-api-microgrid-0.17.0/submodules/frequenz-api-common/proto/frequenz/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:08:04.281415 frequenz-api-microgrid-0.17.0/submodules/frequenz-api-common/proto/frequenz/api/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:08:04.293415 frequenz-api-microgrid-0.17.0/submodules/frequenz-api-common/proto/frequenz/api/common/
+-rw-r--r--   0 runner    (1001) docker     (127)     3557 2024-05-10 15:07:53.000000 frequenz-api-microgrid-0.17.0/submodules/frequenz-api-common/proto/frequenz/api/common/components.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-10 15:07:53.000000 frequenz-api-microgrid-0.17.0/submodules/frequenz-api-common/proto/frequenz/api/common/location.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:08:04.293415 frequenz-api-microgrid-0.17.0/submodules/frequenz-api-common/proto/frequenz/api/common/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)     6191 2024-05-10 15:07:53.000000 frequenz-api-microgrid-0.17.0/submodules/frequenz-api-common/proto/frequenz/api/common/metrics/electrical.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     7405 2024-05-10 15:07:53.000000 frequenz-api-microgrid-0.17.0/submodules/frequenz-api-common/proto/frequenz/api/common/metrics.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:08:04.293415 frequenz-api-microgrid-0.17.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:08:04.293415 frequenz-api-microgrid-0.17.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/grid/
+-rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-05-10 15:07:53.000000 frequenz-api-microgrid-0.17.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/grid/delivery_area.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-05-10 15:07:53.000000 frequenz-api-microgrid-0.17.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/grid/delivery_duration.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-10 15:07:53.000000 frequenz-api-microgrid-0.17.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/location.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:08:04.293415 frequenz-api-microgrid-0.17.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/market/
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-05-10 15:07:53.000000 frequenz-api-microgrid-0.17.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/market/energy.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-05-10 15:07:53.000000 frequenz-api-microgrid-0.17.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/market/price.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:08:04.293415 frequenz-api-microgrid-0.17.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-10 15:07:53.000000 frequenz-api-microgrid-0.17.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/metrics/bounds.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     8186 2024-05-10 15:07:53.000000 frequenz-api-microgrid-0.17.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/metrics/metric_sample.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:08:04.293415 frequenz-api-microgrid-0.17.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:08:04.293415 frequenz-api-microgrid-0.17.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-10 15:07:53.000000 frequenz-api-microgrid-0.17.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/battery.proto
+-rw-r--r--   0 runner    (1001) docker     (127)    17610 2024-05-10 15:07:53.000000 frequenz-api-microgrid-0.17.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/components.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-10 15:07:53.000000 frequenz-api-microgrid-0.17.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/ev_charger.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-10 15:07:53.000000 frequenz-api-microgrid-0.17.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/fuse.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-05-10 15:07:53.000000 frequenz-api-microgrid-0.17.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/grid.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-05-10 15:07:53.000000 frequenz-api-microgrid-0.17.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/inverter.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-10 15:07:53.000000 frequenz-api-microgrid-0.17.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/transformer.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-05-10 15:07:53.000000 frequenz-api-microgrid-0.17.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/lifetime.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-05-10 15:07:53.000000 frequenz-api-microgrid-0.17.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/microgrid.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:08:04.293415 frequenz-api-microgrid-0.17.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/sensors/
+-rw-r--r--   0 runner    (1001) docker     (127)     5691 2024-05-10 15:07:53.000000 frequenz-api-microgrid-0.17.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/sensors/sensors.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:08:04.297415 frequenz-api-microgrid-0.17.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/pagination/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-10 15:07:53.000000 frequenz-api-microgrid-0.17.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/pagination/pagination_info.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-05-10 15:07:53.000000 frequenz-api-microgrid-0.17.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/pagination/pagination_params.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:08:04.297415 frequenz-api-microgrid-0.17.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/types/
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-05-10 15:07:53.000000 frequenz-api-microgrid-0.17.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/types/decimal.proto
```

### Comparing `frequenz-api-microgrid-0.16.1/LICENSE` & `frequenz-api-microgrid-0.17.0/LICENSE`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.16.1/PKG-INFO` & `frequenz-api-microgrid-0.17.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frequenz-api-microgrid
-Version: 0.16.1
+Version: 0.17.0
 Summary: Frequenz gRPC API for monitoring and control of microgrids
 Author-email: Frequenz Energy-as-a-Service GmbH <floss@frequenz.com>
 License: MIT
 Project-URL: Changelog, https://github.com/frequenz-floss/frequenz-api-microgrid/releases
 Project-URL: Issues, https://github.com/frequenz-floss/frequenz-api-microgrid/issues
 Project-URL: Repository, https://github.com/frequenz-floss/frequenz-api-microgrid
 Project-URL: Support, https://github.com/frequenz-floss/frequenz-api-microgrid/discussions/categories/support
```

### Comparing `frequenz-api-microgrid-0.16.1/README.md` & `frequenz-api-microgrid-0.17.0/README.md`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.16.1/proto/frequenz/api/microgrid/v1/microgrid.proto` & `frequenz-api-microgrid-0.17.0/proto/frequenz/api/microgrid/v1/microgrid.proto`

 * *Files 6% similar despite different names*

```diff
@@ -126,100 +126,49 @@
   rpc ReceiveSensorDataStream(ReceiveSensorDataStreamRequest)
     returns (stream ReceiveSensorDataStreamResponse) {
     option (google.api.http) = {
       get : "/v1/sensors/{sensor_id}/data"
     };
   }
 
-  // Adds exclusion bounds for a given metric of a given component, and returns
-  // the UTC timestamp until which the given exclusion bounds will stay in
-  // effect.
-  //
-  // Exclusion bounds refer to the range of values that are disallowed for the
-  // metric. If these bounds for a metric are [`lower`, `upper`], then this
-  // metric's `value` needs to comply with the constraints
-  // `value <= lower` OR `upper <= value`.
-  //
-  // Exclusion bounds are a useful tool for enhancing the performance of a
-  // system. They can be used to restrict the acceptance of commands that fall
-  // below a certain threshold, which can help ensure the smooth functioning of
-  // the system.
-  // E.g., exclusion bounds can be set to limit the minimum charging power to a
-  // sufficiently high level, preventing a peak-shaver client from sending
-  // charge powers that are too low when a DC heater client is executing a
-  // charge pulse. This can significantly improve the overall performance of the
-  // DC heating mechanism.
-  //
-  //
-  // If multiple exclusion bounds have been provided bor a metric, then the
-  // aggregated lower and upper exclusion bounds are calculated as follows:
-  // lower: the minimum of all lower exclusion bounds
-  // upper: the maximum of all upper exclusion bounds
-  //
-  // It is important to note that these bounds work together with
-  // `system_inclusion_bounds`.
-  //
-  // E.g., for the system to accept a charge command,
-  // clients need to request power values within the bounds
-  // `[system_inclusion_bounds.lower, system_exclusion_bounds.lower]`.
-  // This means that clients can only request charge commands with values that
-  // are within the `system_inclusion_bounds`, but not within
-  // `system_exclusion_bounds`.
-  // Similarly, for the system to accept a discharge command,
-  // clients need to request power values within the bounds
-  // `[system_exclusion_bounds.upper, system_inclusion_bounds.upper]`.
+  // Adds inclusion bounds for a given metric of a given component. Returns the
+  // time at which the bounds will expire (as a timestamp (UTC)).
   //
-  // The following diagram illustrates the relationship between the bounds.
-  // ```
-  //   inclusion.lower                              inclusion.upper
-  // <-------|============|------------------|============|--------->
-  //                exclusion.lower    exclusion.upper
-  // ```
-  // ---- values here are disallowed and will be rejected
-  // ==== vales here are allowed and will be accepted
-  rpc AddComponentExclusionBounds(AddComponentExclusionBoundsRequest)
-    returns (AddComponentExclusionBoundsResponse);
-
-  // Adds inclusion bounds for a given metric of a given component, and returns
-  // the UTC timestamp until which the given inclusion bounds will stay in
-  // effect.
-  //
-  // Inclusion bounds refer to the range of values that are allowed for the
-  // metric. If these bounds for a metric are [`lower`, `upper`], then this
-  // metric's `value` needs to comply with the constraint
-  // `lower <= value <= upper`.
-  //
-  // If multiple inclusion bounds have been provided bor a metric, then the
-  // aggregated lower and upper inclusion bounds are calculated as follows:
-  // lower: the maximum of all lower inclusion bounds
-  // upper: the minimum of all upper inclusion bounds
-  //
-  // It is important to note that these bounds work together with
-  // `system_exclusion_bounds`.
-  //
-  // E.g., for the system to accept a charge command,
-  // clients need to request power values within the bounds
-  // `[system_inclusion_bounds.lower, system_exclusion_bounds.lower]`.
-  // This means that clients can only request charge commands with values that
-  // are within the `system_inclusion_bounds`, but not within
-  // `system_exclusion_bounds`.
-  // Similarly, for the system to accept a discharge command,
-  // clients need to request power values within the bounds
-  // `[system_exclusion_bounds.upper, system_inclusion_bounds.upper]`.
+  // The request parameters allows users to select a duration until
+  // which the bounds will stay in effect. If no duration is provided, then the
+  // bounds will be removed after a default duration of 5 seconds.
+  //
+  // Inclusion bounds give the range that the system will try to keep the
+  // metric within. If the metric goes outside of these bounds, the system will
+  // try to bring it back within the bounds.
+  // If the bounds for a metric are [[`lower_1`, `upper_1`],
+  // [`lower_2`, `upper_2`]], then this metric's `value` needs to comply with
+  // the constraints
+  // `lower_1 <= value <= upper_1` OR `lower_2 <= value <= upper_2`.
+  //
+  // If multiple inclusion bounds have been provided for a metric, then the
+  // overlapping bounds are merged into a single bound, and non-overlapping
+  // bounds are kept separate.
+  // E.g. if the bounds are [[0, 10], [5, 15], [20, 30]], then the resulting
+  // bounds will be [[0, 15], [20, 30]].
   //
-  // The following diagram illustrates the relationship between the bounds.
+  // The following diagram illustrates how bounds are applied:
   // ```
-  //   inclusion.lower                              inclusion.upper
-  // <-------|============|------------------|============|--------->
-  //                exclusion.lower    exclusion.upper
+  //   lower_1  upper_1
+  // <----|========|--------|========|-------->
+  //                     lower_2  upper_2
   // ```
-  // ---- values here are disallowed and will be rejected
-  // ==== vales here are allowed and will be accepted
-  rpc AddComponentInclusionBounds(AddComponentInclusionBoundsRequest)
-    returns (AddComponentInclusionBoundsResponse);
+  // The bounds in this example are `[[lower_1, upper_1], [lower_2, upper_2]]`.
+  // ---- values here are considered out of range.
+  // ==== values here are considered within range.
+  //
+  // Note that for power metrics, regardless of the bounds, 0W is always
+  // allowed.
+  rpc AddComponentBounds(AddComponentBoundsRequest)
+    returns (AddComponentBoundsResponse);
 
   // Sets the active power output of a component with a given ID, provided the
   // component supports it. The power output is specified in watts.
   //
   // The power output can be -ve or +ve, depending on whether the component is
   // supposed to be discharging or charging, respectively.
   //
@@ -244,16 +193,18 @@
       get : "/v1/components/{component_id}/setPowerActive/{power}"
     };
   }
 
   // Sets the reactive power output of a component with a given ID, provided the
   // component supports it. The power output is specified in VAr.
   //
-  // The power output can be -ve or +ve, depending on whether the component is
-  // supposed to be delivering inductive or capacitive power, respectively.
+  // We follow the polarity specified in the IEEE 1459-2010 standard
+  // definitions, where
+  //- positive reactive is inductive (current is lagging the voltage)
+  //- negative reactive is capacitive (current is leading the voltage)
   //
   // The return value is the timestamp until which the given power command will
   // stay in effect. After this timestamp, the component's reactive power will
   // be set to 0, if the API receives no further command to change it before
   // then.
   // By default, this timestamp will be set to the current time plus 60 seconds.
   //
@@ -491,70 +442,63 @@
 
 // A data sample from a sensor in the microgrid.
 message ReceiveSensorDataStreamResponse {
   // The sensor data.
   frequenz.api.common.v1.microgrid.sensors.SensorData data = 1;
 }
 
-// An enumerated list of metrics whose bounds can be set using the RPCs
-// `AddComponentExclusionBounds` and `AddComponentInclusionBounds`.
-enum ComponentBoundsTargetMetric {
-  COMPONENT_BOUNDS_TARGET_METRIC_UNSPECIFIED = 0;
-  COMPONENT_BOUNDS_TARGET_METRIC_POWER_ACTIVE = 1;
-  COMPONENT_BOUNDS_TARGET_METRIC_CURRENT = 2;
-  COMPONENT_BOUNDS_TARGET_METRIC_CURRENT_PHASE_1 = 3;
-  COMPONENT_BOUNDS_TARGET_METRIC_CURRENT_PHASE_2 = 4;
-  COMPONENT_BOUNDS_TARGET_METRIC_CURRENT_PHASE_3 = 5;
-  COMPONENT_BOUNDS_TARGET_METRIC_POWER_REACTIVE = 6;
-}
-
-// Request parameters for the RPC `AddComponentExclusionBounds`.
-message AddComponentExclusionBoundsRequest {
-  // The ID of the target component.
-  uint64 component_id = 1;
-
-  // The target metric whose bounds have to be set.
-  ComponentBoundsTargetMetric target_metric = 2;
-
-  // The bounds for the target metric.
-  frequenz.api.common.v1.metrics.Bounds bounds = 3;
-}
-
-// Response message for the RPC `AddComponentExclusionBounds`.
-message AddComponentExclusionBoundsResponse {
-  // The timestamp until which the given exclusion bounds will stay in effect.
-  google.protobuf.Timestamp ts = 1;
+// The duration for which a given list of bounds will stay in effect.
+enum ComponentBoundsValidityDuration {
+  COMPONENT_BOUNDS_VALIDITY_DURATION_UNSPECIFIED = 0;
+  COMPONENT_BOUNDS_VALIDITY_DURATION_5_SECONDS = 1;
+  COMPONENT_BOUNDS_VALIDITY_DURATION_1_MINUTE = 2;
+  COMPONENT_BOUNDS_VALIDITY_DURATION_5_MINUTES = 3;
+  COMPONENT_BOUNDS_VALIDITY_DURATION_15_MINUTES = 4;
 }
 
-// Request parameters for the RPC `AddComponentInclusionBounds`.
-message AddComponentInclusionBoundsRequest {
+// Request parameters for the RPC `AddComponentBounds`.
+message AddComponentBoundsRequest {
   // The ID of the target component.
   uint64 component_id = 1;
 
   // The target metric whose bounds have to be set.
-  ComponentBoundsTargetMetric target_metric = 2;
+  frequenz.api.common.v1.metrics.Metric target_metric = 2;
 
-  // The bounds for the target metric.
-  frequenz.api.common.v1.metrics.Bounds bounds = 3;
-}
-
-// Response message for the RPC `AddComponentInclusionBounds`.
-message AddComponentInclusionBoundsResponse {
-  // The timestamp until which the given inclusion bounds will stay in effect.
+  // A list of bounds for the target metric.
+  // While incorporating these bounds, the API will ensure that overlapping
+  // pairs of bounds are merged into a single pair of bounds, and
+  // non-overlapping ones are kept separated.
+  repeated frequenz.api.common.v1.metrics.Bounds bounds = 3;
+
+  // The duration for which the given bounds will stay in effect.
+  // If this field is not provided, then the bounds will be removed after a
+  // default duration of 5 seconds.
+  ComponentBoundsValidityDuration validity_duration = 4;
+}
+
+// Response message for the RPC `AddComponentBounds`.
+message AddComponentBoundsResponse {
+  // The timestamp until which the given bounds will stay in effect.
   google.protobuf.Timestamp ts = 1;
 }
 
 // Request parameters for the RPC `SetComponentPowerActive`.
 message SetComponentPowerActiveRequest {
   // The ID of the component to set the output active power of.
   uint64 component_id = 1;
 
   // The output active power level, in watts.
   // -ve values are for discharging, and +ve values are for charging.
   float power = 2;
+
+  // The duration, in seconds, until which the request will stay in effect.
+  // This duration has to be between 10 seconds and 15 minutes (including both
+  // limits), otherwise the request will be rejected.
+  // If not provided, it defaults to 60s.
+  optional uint64 request_lifetime = 3;
 }
 
 // Response message for the RPC `SetComponentPowerActive`.
 message SetComponentPowerActiveResponse {
   // The timestamp until which the given power command will stay in effect.
   // After this timestamp, the component power will be set to 0, if the API
   // receives no further power commands. By default, this timestamp will be set
@@ -564,17 +508,26 @@
 
 // Request parameters for the RPC `SetComponentPowerReactive`.
 message SetComponentPowerReactiveRequest {
   // The ID of the component to set the output reactive power of.
   uint64 component_id = 1;
 
   // The output reactive power level, in VAr.
-  // -ve values are for inductive (lagging) power , and +ve values are for
-  //  capacitive (leading) power.
+  //
+  // The standard of polarity is as per the IEEE 1459-2010 standard
+  // definitions:
+  // - positive reactive is inductive (current is lagging the voltage)
+  // - negative reactive is capacitive (current is leading the voltage)
   float power = 2;
+
+  // The duration, in seconds, until which the request will stay in effect.
+  // This duration has to be between 10 seconds and 15 minutes (including both
+  // limits), otherwise the request will be rejected.
+  // If not provided, it defaults to 60s.
+  optional uint64 request_lifetime = 3;
 }
 
 // Response message for the RPC `SetComponentPowerReactive`.
 message SetComponentPowerReactiveResponse {
   // The timestamp until which the given power command will stay in effect.
   // After this timestamp, the component power will be set to 0, if the API
   // receives no further power commands. By default, this timestamp will be set
```

### Comparing `frequenz-api-microgrid-0.16.1/py/frequenz_api_microgrid.egg-info/PKG-INFO` & `frequenz-api-microgrid-0.17.0/py/frequenz_api_microgrid.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frequenz-api-microgrid
-Version: 0.16.1
+Version: 0.17.0
 Summary: Frequenz gRPC API for monitoring and control of microgrids
 Author-email: Frequenz Energy-as-a-Service GmbH <floss@frequenz.com>
 License: MIT
 Project-URL: Changelog, https://github.com/frequenz-floss/frequenz-api-microgrid/releases
 Project-URL: Issues, https://github.com/frequenz-floss/frequenz-api-microgrid/issues
 Project-URL: Repository, https://github.com/frequenz-floss/frequenz-api-microgrid
 Project-URL: Support, https://github.com/frequenz-floss/frequenz-api-microgrid/discussions/categories/support
```

### Comparing `frequenz-api-microgrid-0.16.1/py/frequenz_api_microgrid.egg-info/SOURCES.txt` & `frequenz-api-microgrid-0.17.0/py/frequenz_api_microgrid.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -64,23 +64,31 @@
 submodules/api-common-protos/google/type/fraction.proto
 submodules/api-common-protos/google/type/latlng.proto
 submodules/api-common-protos/google/type/money.proto
 submodules/api-common-protos/google/type/month.proto
 submodules/api-common-protos/google/type/postal_address.proto
 submodules/api-common-protos/google/type/quaternion.proto
 submodules/api-common-protos/google/type/timeofday.proto
+submodules/frequenz-api-common/proto/frequenz/api/common/components.proto
+submodules/frequenz-api-common/proto/frequenz/api/common/location.proto
+submodules/frequenz-api-common/proto/frequenz/api/common/metrics.proto
+submodules/frequenz-api-common/proto/frequenz/api/common/metrics/electrical.proto
 submodules/frequenz-api-common/proto/frequenz/api/common/v1/location.proto
 submodules/frequenz-api-common/proto/frequenz/api/common/v1/grid/delivery_area.proto
+submodules/frequenz-api-common/proto/frequenz/api/common/v1/grid/delivery_duration.proto
+submodules/frequenz-api-common/proto/frequenz/api/common/v1/market/energy.proto
+submodules/frequenz-api-common/proto/frequenz/api/common/v1/market/price.proto
 submodules/frequenz-api-common/proto/frequenz/api/common/v1/metrics/bounds.proto
 submodules/frequenz-api-common/proto/frequenz/api/common/v1/metrics/metric_sample.proto
 submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/lifetime.proto
 submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/microgrid.proto
 submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/battery.proto
 submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/components.proto
 submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/ev_charger.proto
 submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/fuse.proto
 submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/grid.proto
 submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/inverter.proto
 submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/transformer.proto
 submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/sensors/sensors.proto
 submodules/frequenz-api-common/proto/frequenz/api/common/v1/pagination/pagination_info.proto
-submodules/frequenz-api-common/proto/frequenz/api/common/v1/pagination/pagination_params.proto
+submodules/frequenz-api-common/proto/frequenz/api/common/v1/pagination/pagination_params.proto
+submodules/frequenz-api-common/proto/frequenz/api/common/v1/types/decimal.proto
```

### Comparing `frequenz-api-microgrid-0.16.1/py/frequenz_api_microgrid.egg-info/requires.txt` & `frequenz-api-microgrid-0.17.0/py/frequenz_api_microgrid.egg-info/requires.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-frequenz-api-common<0.6,>=0.5.0
-googleapis-common-protos<2,>=1.56.2
+frequenz-api-common<0.7,>=0.6.1
+googleapis-common-protos<2,>=1.56.4
 grpcio<2,>=1.51.1
 
 [dev]
 frequenz-api-microgrid[dev-flake8,dev-formatting,dev-mkdocs,dev-mypy,dev-noxfile,dev-pylint,dev-pytest]
 
 [dev-flake8]
 flake8==7.0.0
 flake8-docstrings==1.7.0
 flake8-pyproject==1.2.3
 pydoclint==0.4.1
 pydocstyle==6.3.0
 
 [dev-formatting]
-black==24.3.0
+black==24.4.2
 isort==5.13.2
 
 [dev-mkdocs]
 mike==1.1.2
 mkdocs-gen-files==0.5.0
 mkdocs-literate-nav==0.6.1
-mkdocs-material==9.5.15
+mkdocs-material==9.5.20
 mkdocstrings[python]==0.23.0
 frequenz-repo-config[api]==0.9.1
 
 [dev-mypy]
-mypy==1.9.0
+mypy==1.10.0
 grpc-stubs==1.53.0.5
 frequenz-api-microgrid[dev-mkdocs,dev-noxfile,dev-pytest]
 
 [dev-noxfile]
-nox==2024.3.2
+nox==2024.4.15
 frequenz-repo-config[api]==0.9.1
 
 [dev-pylint]
 pylint==3.1.0
 frequenz-api-microgrid[dev-mkdocs,dev-noxfile,dev-pytest]
 
 [dev-pytest]
-pytest==8.1.1
+pytest==8.2.0
 frequenz-repo-config[extra-lint-examples]==0.9.1
```

### Comparing `frequenz-api-microgrid-0.16.1/pyproject.toml` & `frequenz-api-microgrid-0.17.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -22,16 +22,16 @@
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3 :: Only",
   "Topic :: Software Development :: Libraries",
   "Typing :: Typed",
 ]
 requires-python = ">= 3.11, < 4"
 dependencies = [
-  "frequenz-api-common >= 0.5.0, < 0.6",
-  "googleapis-common-protos >= 1.56.2, < 2",
+  "frequenz-api-common >= 0.6.1, < 0.7",
+  "googleapis-common-protos >= 1.56.4, < 2",
   "grpcio >= 1.51.1, < 2",
 ]
 dynamic = ["version"]
 
 [[project.authors]]
 name = "Frequenz Energy-as-a-Service GmbH"
 email = "floss@frequenz.com"
@@ -40,40 +40,40 @@
 dev-flake8 = [
   "flake8 == 7.0.0",
   "flake8-docstrings == 1.7.0",
   "flake8-pyproject == 1.2.3",  # For reading the flake8 config from pyproject.toml
   "pydoclint == 0.4.1",
   "pydocstyle == 6.3.0",
 ]
-dev-formatting = ["black == 24.3.0", "isort == 5.13.2"]
+dev-formatting = ["black == 24.4.2", "isort == 5.13.2"]
 dev-mkdocs = [
   "mike == 1.1.2",
   "mkdocs-gen-files == 0.5.0",
   "mkdocs-literate-nav == 0.6.1",
-  "mkdocs-material == 9.5.15",
+  "mkdocs-material == 9.5.20",
   "mkdocstrings[python] == 0.23.0",
   "frequenz-repo-config[api] == 0.9.1",
 ]
 dev-mypy = [
-  "mypy == 1.9.0",
+  "mypy == 1.10.0",
   "grpc-stubs == 1.53.0.5",
   # For checking the noxfile, docs/ script, and tests
   "frequenz-api-microgrid[dev-mkdocs,dev-noxfile,dev-pytest]",
 ]
 dev-noxfile = [
-  "nox == 2024.3.2",
+  "nox == 2024.4.15",
   "frequenz-repo-config[api] == 0.9.1",
 ]
 dev-pylint = [
   "pylint == 3.1.0",
   # For checking the noxfile, docs/ script, and tests
   "frequenz-api-microgrid[dev-mkdocs,dev-noxfile,dev-pytest]",
 ]
 dev-pytest = [
-  "pytest == 8.1.1",
+  "pytest == 8.2.0",
   "frequenz-repo-config[extra-lint-examples] == 0.9.1",
 ]
 dev = [
   "frequenz-api-microgrid[dev-mkdocs,dev-flake8,dev-formatting,dev-mkdocs,dev-mypy,dev-noxfile,dev-pylint,dev-pytest]",
 ]
 
 [project.urls]
```

### Comparing `frequenz-api-microgrid-0.16.1/submodules/api-common-protos/google/api/annotations.proto` & `frequenz-api-microgrid-0.17.0/submodules/api-common-protos/google/api/annotations.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.16.1/submodules/api-common-protos/google/api/auth.proto` & `frequenz-api-microgrid-0.17.0/submodules/api-common-protos/google/api/auth.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.16.1/submodules/api-common-protos/google/api/backend.proto` & `frequenz-api-microgrid-0.17.0/submodules/api-common-protos/google/api/backend.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.16.1/submodules/api-common-protos/google/api/billing.proto` & `frequenz-api-microgrid-0.17.0/submodules/api-common-protos/google/api/billing.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.16.1/submodules/api-common-protos/google/api/client.proto` & `frequenz-api-microgrid-0.17.0/submodules/api-common-protos/google/api/client.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.16.1/submodules/api-common-protos/google/api/config_change.proto` & `frequenz-api-microgrid-0.17.0/submodules/api-common-protos/google/api/config_change.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.16.1/submodules/api-common-protos/google/api/consumer.proto` & `frequenz-api-microgrid-0.17.0/submodules/api-common-protos/google/api/consumer.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.16.1/submodules/api-common-protos/google/api/context.proto` & `frequenz-api-microgrid-0.17.0/submodules/api-common-protos/google/api/context.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.16.1/submodules/api-common-protos/google/api/control.proto` & `frequenz-api-microgrid-0.17.0/submodules/api-common-protos/google/api/control.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.16.1/submodules/api-common-protos/google/api/distribution.proto` & `frequenz-api-microgrid-0.17.0/submodules/api-common-protos/google/api/distribution.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.16.1/submodules/api-common-protos/google/api/documentation.proto` & `frequenz-api-microgrid-0.17.0/submodules/api-common-protos/google/api/documentation.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.16.1/submodules/api-common-protos/google/api/endpoint.proto` & `frequenz-api-microgrid-0.17.0/submodules/api-common-protos/google/api/endpoint.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.16.1/submodules/api-common-protos/google/api/field_behavior.proto` & `frequenz-api-microgrid-0.17.0/submodules/api-common-protos/google/api/field_behavior.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.16.1/submodules/api-common-protos/google/api/http.proto` & `frequenz-api-microgrid-0.17.0/submodules/api-common-protos/google/api/http.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.16.1/submodules/api-common-protos/google/api/httpbody.proto` & `frequenz-api-microgrid-0.17.0/submodules/api-common-protos/google/api/httpbody.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.16.1/submodules/api-common-protos/google/api/label.proto` & `frequenz-api-microgrid-0.17.0/submodules/api-common-protos/google/api/label.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.16.1/submodules/api-common-protos/google/api/launch_stage.proto` & `frequenz-api-microgrid-0.17.0/submodules/api-common-protos/google/api/launch_stage.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.16.1/submodules/api-common-protos/google/api/log.proto` & `frequenz-api-microgrid-0.17.0/submodules/api-common-protos/google/api/log.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.16.1/submodules/api-common-protos/google/api/logging.proto` & `frequenz-api-microgrid-0.17.0/submodules/api-common-protos/google/api/logging.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.16.1/submodules/api-common-protos/google/api/metric.proto` & `frequenz-api-microgrid-0.17.0/submodules/api-common-protos/google/api/metric.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.16.1/submodules/api-common-protos/google/api/monitored_resource.proto` & `frequenz-api-microgrid-0.17.0/submodules/api-common-protos/google/api/monitored_resource.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.16.1/submodules/api-common-protos/google/api/monitoring.proto` & `frequenz-api-microgrid-0.17.0/submodules/api-common-protos/google/api/monitoring.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.16.1/submodules/api-common-protos/google/api/quota.proto` & `frequenz-api-microgrid-0.17.0/submodules/api-common-protos/google/api/quota.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.16.1/submodules/api-common-protos/google/api/resource.proto` & `frequenz-api-microgrid-0.17.0/submodules/api-common-protos/google/api/resource.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.16.1/submodules/api-common-protos/google/api/routing.proto` & `frequenz-api-microgrid-0.17.0/submodules/api-common-protos/google/api/routing.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.16.1/submodules/api-common-protos/google/api/service.proto` & `frequenz-api-microgrid-0.17.0/submodules/api-common-protos/google/api/service.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.16.1/submodules/api-common-protos/google/api/source_info.proto` & `frequenz-api-microgrid-0.17.0/submodules/api-common-protos/google/api/source_info.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.16.1/submodules/api-common-protos/google/api/system_parameter.proto` & `frequenz-api-microgrid-0.17.0/submodules/api-common-protos/google/api/system_parameter.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.16.1/submodules/api-common-protos/google/api/usage.proto` & `frequenz-api-microgrid-0.17.0/submodules/api-common-protos/google/api/usage.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.16.1/submodules/api-common-protos/google/cloud/extended_operations.proto` & `frequenz-api-microgrid-0.17.0/submodules/api-common-protos/google/cloud/extended_operations.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.16.1/submodules/api-common-protos/google/iam/admin/v1/iam.proto` & `frequenz-api-microgrid-0.17.0/submodules/api-common-protos/google/iam/admin/v1/iam.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.16.1/submodules/api-common-protos/google/iam/v1/iam_policy.proto` & `frequenz-api-microgrid-0.17.0/submodules/api-common-protos/google/iam/v1/iam_policy.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.16.1/submodules/api-common-protos/google/iam/v1/logging/audit_data.proto` & `frequenz-api-microgrid-0.17.0/submodules/api-common-protos/google/iam/v1/logging/audit_data.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.16.1/submodules/api-common-protos/google/iam/v1/options.proto` & `frequenz-api-microgrid-0.17.0/submodules/api-common-protos/google/iam/v1/options.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.16.1/submodules/api-common-protos/google/iam/v1/policy.proto` & `frequenz-api-microgrid-0.17.0/submodules/api-common-protos/google/iam/v1/policy.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.16.1/submodules/api-common-protos/google/logging/type/http_request.proto` & `frequenz-api-microgrid-0.17.0/submodules/api-common-protos/google/logging/type/http_request.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.16.1/submodules/api-common-protos/google/logging/type/log_severity.proto` & `frequenz-api-microgrid-0.17.0/submodules/api-common-protos/google/logging/type/log_severity.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.16.1/submodules/api-common-protos/google/longrunning/operations.proto` & `frequenz-api-microgrid-0.17.0/submodules/api-common-protos/google/longrunning/operations.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.16.1/submodules/api-common-protos/google/rpc/code.proto` & `frequenz-api-microgrid-0.17.0/submodules/api-common-protos/google/rpc/code.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.16.1/submodules/api-common-protos/google/rpc/context/attribute_context.proto` & `frequenz-api-microgrid-0.17.0/submodules/api-common-protos/google/rpc/context/attribute_context.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.16.1/submodules/api-common-protos/google/rpc/error_details.proto` & `frequenz-api-microgrid-0.17.0/submodules/api-common-protos/google/rpc/error_details.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.16.1/submodules/api-common-protos/google/rpc/status.proto` & `frequenz-api-microgrid-0.17.0/submodules/api-common-protos/google/rpc/status.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.16.1/submodules/api-common-protos/google/type/calendar_period.proto` & `frequenz-api-microgrid-0.17.0/submodules/api-common-protos/google/type/calendar_period.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.16.1/submodules/api-common-protos/google/type/color.proto` & `frequenz-api-microgrid-0.17.0/submodules/api-common-protos/google/type/color.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.16.1/submodules/api-common-protos/google/type/date.proto` & `frequenz-api-microgrid-0.17.0/submodules/api-common-protos/google/type/date.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.16.1/submodules/api-common-protos/google/type/datetime.proto` & `frequenz-api-microgrid-0.17.0/submodules/api-common-protos/google/type/datetime.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.16.1/submodules/api-common-protos/google/type/dayofweek.proto` & `frequenz-api-microgrid-0.17.0/submodules/api-common-protos/google/type/dayofweek.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.16.1/submodules/api-common-protos/google/type/expr.proto` & `frequenz-api-microgrid-0.17.0/submodules/api-common-protos/google/type/expr.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.16.1/submodules/api-common-protos/google/type/fraction.proto` & `frequenz-api-microgrid-0.17.0/submodules/api-common-protos/google/type/fraction.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.16.1/submodules/api-common-protos/google/type/latlng.proto` & `frequenz-api-microgrid-0.17.0/submodules/api-common-protos/google/type/latlng.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.16.1/submodules/api-common-protos/google/type/money.proto` & `frequenz-api-microgrid-0.17.0/submodules/api-common-protos/google/type/money.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.16.1/submodules/api-common-protos/google/type/month.proto` & `frequenz-api-microgrid-0.17.0/submodules/api-common-protos/google/type/month.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.16.1/submodules/api-common-protos/google/type/postal_address.proto` & `frequenz-api-microgrid-0.17.0/submodules/api-common-protos/google/type/postal_address.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.16.1/submodules/api-common-protos/google/type/quaternion.proto` & `frequenz-api-microgrid-0.17.0/submodules/api-common-protos/google/type/quaternion.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.16.1/submodules/api-common-protos/google/type/timeofday.proto` & `frequenz-api-microgrid-0.17.0/submodules/api-common-protos/google/type/timeofday.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.16.1/submodules/frequenz-api-common/proto/frequenz/api/common/v1/grid/delivery_area.proto` & `frequenz-api-microgrid-0.17.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/grid/delivery_area.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.16.1/submodules/frequenz-api-common/proto/frequenz/api/common/v1/location.proto` & `frequenz-api-microgrid-0.17.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/location.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.16.1/submodules/frequenz-api-common/proto/frequenz/api/common/v1/metrics/metric_sample.proto` & `frequenz-api-microgrid-0.17.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/metrics/metric_sample.proto`

 * *Files 16% similar despite different names*

```diff
@@ -12,57 +12,57 @@
 
 import "frequenz/api/common/v1/metrics/bounds.proto";
 
 import "google/protobuf/timestamp.proto";
 
 // Represents a single sample of a specific metric, the value of which is either
 // measured or derived at a particular time.
-message SimpleMetricSample {
+message SimpleMetricValue {
   // The value of the metric, which could be either measured or derived.
   float value = 2;
 }
 
 // Encapsulates derived statistical summaries of a single metric.
 //
 // The message allows for the reporting of statistical summaries — minimum,
 // maximum, and average values - as well as the complete list of individual
 // samples if available.
 //
 // This message represents derived metrics and contains fields for statistical
 // summaries—minimum, maximum, and average values. Individual measurements are
 // are optional, accommodating scenarios where only subsets of this information
 // are available.
-message AggregatedMetricSample {
+message AggregatedMetricValue {
   // The derived average value of the metric.
   float avg_value = 2;
 
   // The minimum measured value of the metric.
   optional float min_value = 3;
 
   // The maximum measured value of the metric.
   optional float max_value = 4;
 
   // Optional array of all the raw individual values.
   repeated float raw_values = 5;
 }
 
-// MetricSampleVariant serves as a union type that can encapsulate either a
-// `SimpleMetricSample` or an `AggregatedMetricSample`.
+// `MetricValueVariant` serves as a union type that can encapsulate either a
+// `SimpleMetricValue` or an `AggregatedMetricValue`.
 //
 // This message is designed to offer flexibility in capturing different
 // granularities of metric samples—either a simple single-point measurement
 // or an aggregated set of measurements for a metric.
 //
-// A `MetricSampleVariant` can hold either a `SimpleMetricSample` or an
-// `AggregatedMetricSample`, but not both simultaneously. Setting one will
+// A `MetricValueVariant` can hold either a `SimpleMetricValue` or an
+// `AggregatedMetricValue`, but not both simultaneously. Setting one will
 // nullify the other.
-message MetricSampleVariant {
-  oneof metric_sample_type {
-    SimpleMetricSample simple_metric = 1;
-    AggregatedMetricSample aggregated_metric = 2;
+message MetricValueVariant {
+  oneof metric_value_variant {
+    SimpleMetricValue simple_metric = 1;
+    AggregatedMetricValue aggregated_metric = 2;
   }
 }
 
 // List of supported metrics.
 enum Metric {
   // Default value.
   METRIC_UNSPECIFIED = 0;
@@ -71,35 +71,38 @@
   METRIC_DC_VOLTAGE = 1;
   METRIC_DC_CURRENT = 2;
   METRIC_DC_POWER = 3;
 
   // General AC electricity metrics
   METRIC_AC_FREQUENCY = 10;
   METRIC_AC_VOLTAGE = 11;
-  METRIC_AC_VOLTAGE_PHASE_1 = 12;
-  METRIC_AC_VOLTAGE_PHASE_2 = 13;
-  METRIC_AC_VOLTAGE_PHASE_3 = 14;
-  METRIC_AC_APPARENT_CURRENT = 15;
-  METRIC_AC_APPARENT_CURRENT_PHASE_1 = 16;
-  METRIC_AC_APPARENT_CURRENT_PHASE_2 = 17;
-  METRIC_AC_APPARENT_CURRENT_PHASE_3 = 18;
+  METRIC_AC_VOLTAGE_PHASE_1_N = 12;
+  METRIC_AC_VOLTAGE_PHASE_2_N = 13;
+  METRIC_AC_VOLTAGE_PHASE_3_N = 14;
+  METRIC_AC_VOLTAGE_PHASE_1_PHASE_2 = 15;
+  METRIC_AC_VOLTAGE_PHASE_2_PHASE_3 = 16;
+  METRIC_AC_VOLTAGE_PHASE_3_PHASE_1 = 17;
+  METRIC_AC_CURRENT = 18;
+  METRIC_AC_CURRENT_PHASE_1 = 19;
+  METRIC_AC_CURRENT_PHASE_2 = 20;
+  METRIC_AC_CURRENT_PHASE_3 = 21;
 
   // AC power metrics
-  METRIC_AC_APPARENT_POWER = 20;
-  METRIC_AC_APPARENT_POWER_PHASE_1 = 21;
-  METRIC_AC_APPARENT_POWER_PHASE_2 = 22;
-  METRIC_AC_APPARENT_POWER_PHASE_3 = 23;
-  METRIC_AC_ACTIVE_POWER = 24;
-  METRIC_AC_ACTIVE_POWER_PHASE_1 = 25;
-  METRIC_AC_ACTIVE_POWER_PHASE_2 = 26;
-  METRIC_AC_ACTIVE_POWER_PHASE_3 = 27;
-  METRIC_AC_REACTIVE_POWER = 28;
-  METRIC_AC_REACTIVE_POWER_PHASE_1 = 29;
-  METRIC_AC_REACTIVE_POWER_PHASE_2 = 30;
-  METRIC_AC_REACTIVE_POWER_PHASE_3 = 31;
+  METRIC_AC_APPARENT_POWER = 22;
+  METRIC_AC_APPARENT_POWER_PHASE_1 = 23;
+  METRIC_AC_APPARENT_POWER_PHASE_2 = 24;
+  METRIC_AC_APPARENT_POWER_PHASE_3 = 25;
+  METRIC_AC_ACTIVE_POWER = 26;
+  METRIC_AC_ACTIVE_POWER_PHASE_1 = 27;
+  METRIC_AC_ACTIVE_POWER_PHASE_2 = 28;
+  METRIC_AC_ACTIVE_POWER_PHASE_3 = 29;
+  METRIC_AC_REACTIVE_POWER = 30;
+  METRIC_AC_REACTIVE_POWER_PHASE_1 = 31;
+  METRIC_AC_REACTIVE_POWER_PHASE_2 = 32;
+  METRIC_AC_REACTIVE_POWER_PHASE_3 = 33;
 
   // AC Power factor
   METRIC_AC_POWER_FACTOR = 40;
   METRIC_AC_POWER_FACTOR_PHASE_1 = 41;
   METRIC_AC_POWER_FACTOR_PHASE_2 = 42;
   METRIC_AC_POWER_FACTOR_PHASE_3 = 43;
 
@@ -122,26 +125,29 @@
   METRIC_AC_ACTIVE_ENERGY_DELIVERED_PHASE_3 = 65;
   METRIC_AC_REACTIVE_ENERGY = 66;
   METRIC_AC_REACTIVE_ENERGY_PHASE_1 = 67;
   METRIC_AC_REACTIVE_ENERGY_PHASE_2 = 69;
   METRIC_AC_REACTIVE_ENERGY_PHASE_3 = 70;
 
   // AC harmonics
-  METRIC_AC_THD_CURRENT = 80;
-  METRIC_AC_THD_CURRENT_PHASE_1 = 81;
-  METRIC_AC_THD_CURRENT_PHASE_2 = 82;
-  METRIC_AC_THD_CURRENT_PHASE_3 = 83;
+  METRIC_AC_TOTAL_HARMONIC_DISTORTION_CURRENT = 80;
+  METRIC_AC_TOTAL_HARMONIC_DISTORTION_CURRENT_PHASE_1 = 81;
+  METRIC_AC_TOTAL_HARMONIC_DISTORTION_CURRENT_PHASE_2 = 82;
+  METRIC_AC_TOTAL_HARMONIC_DISTORTION_CURRENT_PHASE_3 = 83;
 
   // General BMS metrics.
   METRIC_BATTERY_CAPACITY = 101;
   METRIC_BATTERY_SOC_PCT = 102;
   METRIC_BATTERY_TEMPERATURE = 103;
 
   // General inverter metrics.
   METRIC_INVERTER_TEMPERATURE = 120;
+  METRIC_INVERTER_TEMPERATURE_CABINET = 121;
+  METRIC_INVERTER_TEMPERATURE_HEATSINK = 122;
+  METRIC_INVERTER_TEMPERATURE_TRANSFORMER = 123;
 
   // EV charging station metrics.
   METRIC_EV_CHARGER_TEMPERATURE = 140;
 
   // General sensor metrics
   METRIC_SENSOR_WIND_SPEED = 160;
   METRIC_SENSOR_WIND_DIRECTION = 162;
@@ -168,15 +174,15 @@
   // The UTC timestamp of when the metric was sampled.
   google.protobuf.Timestamp sampled_at = 1;
 
   // The metric that was sampled.
   Metric metric = 2;
 
   // The value of the sampled metric.
-  MetricSampleVariant sample = 3;
+  MetricValueVariant value = 3;
 
   // List of bounds that apply to the metric sample.
   //
   // These bounds adapt in real-time to reflect the operating conditions at the
   // time of aggregation or derivation.
   //
   // #### Multiple Bounds
@@ -197,8 +203,24 @@
   //      bound[0].lower                         bound[1].upper
   // <-------|============|------------------|============|--------->
   //                bound[0].upper      bound[1].lower
   // ```
   // ---- values here are disallowed and will be rejected
   // ==== values here are allowed and will be accepted
   repeated Bounds bounds = 4;
+
+  // An optional string that can be used to identify the source of the metric.
+  //
+  // This is expected to be populated when the same `Metric` variant can be
+  // obtained from multiple sensors in the component. Knowing the source of the
+  // metric can help in certain control and monitoring applications.
+  //
+  // E.g., a hybrid inverter can have a DC string for a battery and another DC
+  // string for a PV array. The source names could resemble, say,
+  // `dc_battery_0` and ``dc_pv_0`. A metric like DC voltage can be obtained
+  // from both sources. For an application to determine the SoC of the battery
+  // using the battery voltage, the source of the voltage metric is important.
+  //
+  // In cases where the component has just one source for a metric, then this
+  // field is not expected to be present, because the source is implicit.
+  optional string source = 5;
 }
```

### Comparing `frequenz-api-microgrid-0.16.1/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/battery.proto` & `frequenz-api-microgrid-0.17.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/battery.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.16.1/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/components.proto` & `frequenz-api-microgrid-0.17.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/components.proto`

 * *Files 5% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 // License:
 // MIT
 
 syntax = "proto3";
 
 package frequenz.api.common.v1.microgrid.components;
 
+import "frequenz/api/common/v1/metrics/bounds.proto";
 import "frequenz/api/common/v1/metrics/metric_sample.proto";
 import "frequenz/api/common/v1/microgrid/components/battery.proto";
 import "frequenz/api/common/v1/microgrid/components/ev_charger.proto";
 import "frequenz/api/common/v1/microgrid/components/fuse.proto";
 import "frequenz/api/common/v1/microgrid/components/grid.proto";
 import "frequenz/api/common/v1/microgrid/components/inverter.proto";
 import "frequenz/api/common/v1/microgrid/components/transformer.proto";
@@ -76,14 +77,17 @@
   // A voltage transformer.
   // Voltage transformers are used to step up or step down the voltage, keeping
   // the power somewhat constant by increasing or decreasing the current.
   // If voltage is stepped up, current is stepped down, and vice versa.
   // Note that voltage transformers have efficiency losses, so the output power
   // is always less than the input power.
   COMPONENT_CATEGORY_VOLTAGE_TRANSFORMER = 14;
+
+  // An HVAC (Heating, Ventilation, and Air Conditioning) system.
+  COMPONENT_CATEGORY_HVAC = 15;
 }
 
 // Metadata specific to a microgrid component.
 message ComponentCategoryMetadataVariant {
   oneof metadata {
     frequenz.api.common.v1.microgrid.components.Battery battery = 1;
     frequenz.api.common.v1.microgrid.components.EvCharger ev_charger = 2;
@@ -137,14 +141,34 @@
   string model_name = 7;
 
   // The status of the component.
   ComponentStatus status = 8;
 
   // The operational lifetime of the component.
   frequenz.api.common.v1.microgrid.Lifetime operational_lifetime = 9;
+
+  // List of rated bounds present for the component identified by Metric.
+  repeated MetricConfigBounds metric_config_bounds = 10;
+}
+
+// MetricConfigBounds describes a set of limits for a specific metric consisting
+// of a lower and upper bound for said metric.
+//
+// This can be used for example to specify an allowed range of power output
+// for a component.
+message MetricConfigBounds {
+  // Metric type the config bounds are for
+  frequenz.api.common.v1.metrics.Metric metric = 1;
+
+  // The set of bounds for the specified metric.
+  //
+  // This contains the lower and upper bounds for said metric.
+  // Sources these may be derived from include the component configuration,
+  // manufacturers limits, and limits of other devices.
+  frequenz.api.common.v1.metrics.Bounds config_bounds = 2;
 }
 
 // ComponentConnection describes a single electrical link between two components
 // within a microgrid, effectively representing the physical wiring as viewed
 // from the grid connection point, if one exists, or from the islanding point,
 // in case of an islanded microgrids.
 //
@@ -189,34 +213,36 @@
 //    {
 //      component_id: 13,
 //      metric_samples: [
 //        /* list of metrics for multiple timestamps */
 //        {
 //          sampled_at: "2023-10-01T00:00:00Z",
 //          metric: "DC_VOLTAGE_V",
-//          sample: {},
+//          value: {},
 //          bounds: {},
 //        },
 //        {
 //          sampled_at: "2023-10-01T00:00:00Z",
 //          metric: "DC_VOLTAGE_V",
-//          sample: {},
+//          value: {},
 //          bounds: {},
 //        }
 //      ],
 //      states: [
 //        /* list of states for multiple timestamps */
 //        {
 //          sampled_at: "2023-10-01T00:00:00Z",
 //          states: [],
+//          warnings: [],
 //          errors: [],
 //        },
 //        {
 //          sampled_at: "2023-10-01T00:00:00Z",
 //          states: [],
+//          warnings: [],
 //          errors: [],
 //        },
 //      ]
 //    }
 //  ```
 message ComponentData {
   // The ID of the microgrid component.
```

### Comparing `frequenz-api-microgrid-0.16.1/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/ev_charger.proto` & `frequenz-api-microgrid-0.17.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/ev_charger.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.16.1/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/fuse.proto` & `frequenz-api-microgrid-0.17.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/fuse.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.16.1/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/grid.proto` & `frequenz-api-microgrid-0.17.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/grid.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.16.1/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/inverter.proto` & `frequenz-api-microgrid-0.17.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/inverter.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.16.1/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/transformer.proto` & `frequenz-api-microgrid-0.17.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/transformer.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.16.1/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/lifetime.proto` & `frequenz-api-microgrid-0.17.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/lifetime.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.16.1/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/microgrid.proto` & `frequenz-api-microgrid-0.17.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/microgrid.proto`

 * *Files 4% similar despite different names*

```diff
@@ -58,7 +58,16 @@
 
   // The current status of the microgrid.
   MicrogridStatus status = 6;
 
   // The UTC timestamp indicating when the microgrid was initially created.
   google.protobuf.Timestamp create_timestamp = 7;
 }
+
+// A message to link component IDs with their respective microgrid ID.
+message MicrogridComponentIDs {
+  // The ID of the microgrid.
+  uint64 microgrid_id = 1;
+
+  // List of component IDs belonging to this microgrid.
+  repeated uint64 component_ids = 2;
+}
```

### Comparing `frequenz-api-microgrid-0.16.1/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/sensors/sensors.proto` & `frequenz-api-microgrid-0.17.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/sensors/sensors.proto`

 * *Files 8% similar despite different names*

```diff
@@ -103,37 +103,43 @@
   // Dew point.
   // The temperature at which the air becomes saturated with water vapor.
   //
   // In Celsius (°C).
   SENSOR_METRIC_DEW_POINT = 8;
 }
 
-// ComponentData message aggregates multiple metrics, operational states, and
-// errors, related to a specific microgrid component.
+// SensorData message aggregates multiple metrics, operational states, and
+// errors, related to a specific microgrid sensor.
 //
 // !!! example
 //   Example output of a component data message:
 //   ```
 //    {
-//      component_id: 13,
+//      sensor_id: 13,
 //      metric_samples: [
 //        /* list of metrics for multiple timestamps */
 //        {
 //          sampled_at: "2023-10-01T00:00:00Z",
 //          metric: "METRIC_SENSOR_TEMPERATURE",
-//          sample: metric_sample_type: {simple_metric: {value: 23.5},
-//          bounds: {},
+//          value: metric_value_variant: {simple_metric: {value: 23.5},
 //        },
 //        {
 //          sampled_at: "2023-10-01T00:00:00Z",
 //          metric: "METRIC_SENSOR_RELATIVE_HUMIDITY",
-//          sample: metric_sample_type: {simple_metric: {value: 23.5},
-//          bounds: {},
+//          value: metric_value_variant: {simple_metric: {value: 23.5},
 //        }
+//      ],
+//      states: [
+//        {
+//          sampled_at: "2023-10-01T00:00:00Z",
+//          states: [],
+//          errors: [],
+//        },
 //      ]
+//
 //    }
 //  ```
 message SensorData {
   // The ID of the microgrid sensors.
   uint64 sensor_id = 1;
 
   // List of measurements for a metric of the specific microgrid sensor.
@@ -199,9 +205,9 @@
   // The UTC timestamp of when the metric was sampled.
   google.protobuf.Timestamp sampled_at = 1;
 
   // The metric that was sampled.
   frequenz.api.common.v1.metrics.Metric metric = 2;
 
   // The value of the sampled metric.
-  frequenz.api.common.v1.metrics.MetricSampleVariant sample = 3;
+  frequenz.api.common.v1.metrics.MetricValueVariant value = 3;
 }
```

### Comparing `frequenz-api-microgrid-0.16.1/submodules/frequenz-api-common/proto/frequenz/api/common/v1/pagination/pagination_info.proto` & `frequenz-api-microgrid-0.17.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/pagination/pagination_info.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.16.1/submodules/frequenz-api-common/proto/frequenz/api/common/v1/pagination/pagination_params.proto` & `frequenz-api-microgrid-0.17.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/pagination/pagination_params.proto`

 * *Files identical despite different names*

