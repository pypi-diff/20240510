# Comparing `tmp/pulumi_wavefront-3.2.0a1715229970.tar.gz` & `tmp/pulumi_wavefront-3.2.0a1715237486.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_wavefront-3.2.0a1715229970.tar", last modified: Thu May  9 04:50:02 2024, max compression
+gzip compressed data, was "pulumi_wavefront-3.2.0a1715237486.tar", last modified: Thu May  9 06:54:31 2024, max compression
```

## Comparing `pulumi_wavefront-3.2.0a1715229970.tar` & `pulumi_wavefront-3.2.0a1715237486.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 04:50:02.113978 pulumi_wavefront-3.2.0a1715229970/
--rw-r--r--   0 runner    (1001) docker     (127)     2890 2024-05-09 04:50:02.109978 pulumi_wavefront-3.2.0a1715229970/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-05-09 04:49:55.000000 pulumi_wavefront-3.2.0a1715229970/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 04:50:02.109978 pulumi_wavefront-3.2.0a1715229970/pulumi_wavefront/
--rw-r--r--   0 runner    (1001) docker     (127)     6689 2024-05-09 04:49:55.000000 pulumi_wavefront-3.2.0a1715229970/pulumi_wavefront/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    80836 2024-05-09 04:49:55.000000 pulumi_wavefront-3.2.0a1715229970/pulumi_wavefront/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-05-09 04:49:55.000000 pulumi_wavefront-3.2.0a1715229970/pulumi_wavefront/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    55260 2024-05-09 04:49:55.000000 pulumi_wavefront-3.2.0a1715229970/pulumi_wavefront/alert.py
--rw-r--r--   0 runner    (1001) docker     (127)    33237 2024-05-09 04:49:55.000000 pulumi_wavefront-3.2.0a1715229970/pulumi_wavefront/alert_target.py
--rw-r--r--   0 runner    (1001) docker     (127)    46881 2024-05-09 04:49:55.000000 pulumi_wavefront-3.2.0a1715229970/pulumi_wavefront/cloud_integration_app_dynamics.py
--rw-r--r--   0 runner    (1001) docker     (127)     4878 2024-05-09 04:49:55.000000 pulumi_wavefront-3.2.0a1715229970/pulumi_wavefront/cloud_integration_aws_external_id.py
--rw-r--r--   0 runner    (1001) docker     (127)    30693 2024-05-09 04:49:55.000000 pulumi_wavefront-3.2.0a1715229970/pulumi_wavefront/cloud_integration_azure.py
--rw-r--r--   0 runner    (1001) docker     (127)    26132 2024-05-09 04:49:55.000000 pulumi_wavefront-3.2.0a1715229970/pulumi_wavefront/cloud_integration_azure_activity_log.py
--rw-r--r--   0 runner    (1001) docker     (127)    28909 2024-05-09 04:49:55.000000 pulumi_wavefront-3.2.0a1715229970/pulumi_wavefront/cloud_integration_cloud_trail.py
--rw-r--r--   0 runner    (1001) docker     (127)    36675 2024-05-09 04:49:55.000000 pulumi_wavefront-3.2.0a1715229970/pulumi_wavefront/cloud_integration_cloud_watch.py
--rw-r--r--   0 runner    (1001) docker     (127)    24169 2024-05-09 04:49:55.000000 pulumi_wavefront-3.2.0a1715229970/pulumi_wavefront/cloud_integration_ec2.py
--rw-r--r--   0 runner    (1001) docker     (127)    29317 2024-05-09 04:49:55.000000 pulumi_wavefront-3.2.0a1715229970/pulumi_wavefront/cloud_integration_gcp.py
--rw-r--r--   0 runner    (1001) docker     (127)    23736 2024-05-09 04:49:55.000000 pulumi_wavefront-3.2.0a1715229970/pulumi_wavefront/cloud_integration_gcp_billing.py
--rw-r--r--   0 runner    (1001) docker     (127)    26312 2024-05-09 04:49:55.000000 pulumi_wavefront-3.2.0a1715229970/pulumi_wavefront/cloud_integration_new_relic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 04:50:02.109978 pulumi_wavefront-3.2.0a1715229970/pulumi_wavefront/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-09 04:49:55.000000 pulumi_wavefront-3.2.0a1715229970/pulumi_wavefront/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-09 04:49:55.000000 pulumi_wavefront-3.2.0a1715229970/pulumi_wavefront/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-09 04:49:55.000000 pulumi_wavefront-3.2.0a1715229970/pulumi_wavefront/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    31524 2024-05-09 04:49:55.000000 pulumi_wavefront-3.2.0a1715229970/pulumi_wavefront/dashboard.py
--rw-r--r--   0 runner    (1001) docker     (127)    16825 2024-05-09 04:49:55.000000 pulumi_wavefront-3.2.0a1715229970/pulumi_wavefront/dashboard_json.py
--rw-r--r--   0 runner    (1001) docker     (127)    15111 2024-05-09 04:49:55.000000 pulumi_wavefront-3.2.0a1715229970/pulumi_wavefront/derived_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)    14267 2024-05-09 04:49:55.000000 pulumi_wavefront-3.2.0a1715229970/pulumi_wavefront/event.py
--rw-r--r--   0 runner    (1001) docker     (127)    25046 2024-05-09 04:49:55.000000 pulumi_wavefront-3.2.0a1715229970/pulumi_wavefront/external_link.py
--rw-r--r--   0 runner    (1001) docker     (127)    17778 2024-05-09 04:49:55.000000 pulumi_wavefront-3.2.0a1715229970/pulumi_wavefront/get_alert.py
--rw-r--r--   0 runner    (1001) docker     (127)     4266 2024-05-09 04:49:55.000000 pulumi_wavefront-3.2.0a1715229970/pulumi_wavefront/get_alerts.py
--rw-r--r--   0 runner    (1001) docker     (127)    19876 2024-05-09 04:49:55.000000 pulumi_wavefront-3.2.0a1715229970/pulumi_wavefront/get_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     4439 2024-05-09 04:49:55.000000 pulumi_wavefront-3.2.0a1715229970/pulumi_wavefront/get_dashboards.py
--rw-r--r--   0 runner    (1001) docker     (127)     3065 2024-05-09 04:49:55.000000 pulumi_wavefront-3.2.0a1715229970/pulumi_wavefront/get_default_user_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    15959 2024-05-09 04:49:55.000000 pulumi_wavefront-3.2.0a1715229970/pulumi_wavefront/get_derived_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     4670 2024-05-09 04:49:55.000000 pulumi_wavefront-3.2.0a1715229970/pulumi_wavefront/get_derived_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     6727 2024-05-09 04:49:55.000000 pulumi_wavefront-3.2.0a1715229970/pulumi_wavefront/get_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     6874 2024-05-09 04:49:55.000000 pulumi_wavefront-3.2.0a1715229970/pulumi_wavefront/get_events.py
--rw-r--r--   0 runner    (1001) docker     (127)     9738 2024-05-09 04:49:55.000000 pulumi_wavefront-3.2.0a1715229970/pulumi_wavefront/get_external_link.py
--rw-r--r--   0 runner    (1001) docker     (127)     4625 2024-05-09 04:49:55.000000 pulumi_wavefront-3.2.0a1715229970/pulumi_wavefront/get_external_links.py
--rw-r--r--   0 runner    (1001) docker     (127)    13988 2024-05-09 04:49:55.000000 pulumi_wavefront-3.2.0a1715229970/pulumi_wavefront/get_maintenance_window.py
--rw-r--r--   0 runner    (1001) docker     (127)     3882 2024-05-09 04:49:55.000000 pulumi_wavefront-3.2.0a1715229970/pulumi_wavefront/get_maintenance_window_all.py
--rw-r--r--   0 runner    (1001) docker     (127)     3921 2024-05-09 04:49:55.000000 pulumi_wavefront-3.2.0a1715229970/pulumi_wavefront/get_metrics_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3902 2024-05-09 04:49:55.000000 pulumi_wavefront-3.2.0a1715229970/pulumi_wavefront/get_role.py
--rw-r--r--   0 runner    (1001) docker     (127)     4086 2024-05-09 04:49:55.000000 pulumi_wavefront-3.2.0a1715229970/pulumi_wavefront/get_roles.py
--rw-r--r--   0 runner    (1001) docker     (127)     5158 2024-05-09 04:49:55.000000 pulumi_wavefront-3.2.0a1715229970/pulumi_wavefront/get_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     4436 2024-05-09 04:49:55.000000 pulumi_wavefront-3.2.0a1715229970/pulumi_wavefront/get_user_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     4340 2024-05-09 04:49:55.000000 pulumi_wavefront-3.2.0a1715229970/pulumi_wavefront/get_user_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     2621 2024-05-09 04:49:55.000000 pulumi_wavefront-3.2.0a1715229970/pulumi_wavefront/get_users.py
--rw-r--r--   0 runner    (1001) docker     (127)    17169 2024-05-09 04:49:55.000000 pulumi_wavefront-3.2.0a1715229970/pulumi_wavefront/ingestion_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    34482 2024-05-09 04:49:55.000000 pulumi_wavefront-3.2.0a1715229970/pulumi_wavefront/maintenance_window.py
--rw-r--r--   0 runner    (1001) docker     (127)    12867 2024-05-09 04:49:55.000000 pulumi_wavefront-3.2.0a1715229970/pulumi_wavefront/metrics_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)   217687 2024-05-09 04:49:55.000000 pulumi_wavefront-3.2.0a1715229970/pulumi_wavefront/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5652 2024-05-09 04:49:55.000000 pulumi_wavefront-3.2.0a1715229970/pulumi_wavefront/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-09 04:49:55.000000 pulumi_wavefront-3.2.0a1715229970/pulumi_wavefront/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 04:49:55.000000 pulumi_wavefront-3.2.0a1715229970/pulumi_wavefront/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    14021 2024-05-09 04:49:55.000000 pulumi_wavefront-3.2.0a1715229970/pulumi_wavefront/role.py
--rw-r--r--   0 runner    (1001) docker     (127)    18954 2024-05-09 04:49:55.000000 pulumi_wavefront-3.2.0a1715229970/pulumi_wavefront/service_account.py
--rw-r--r--   0 runner    (1001) docker     (127)    14393 2024-05-09 04:49:55.000000 pulumi_wavefront-3.2.0a1715229970/pulumi_wavefront/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     8233 2024-05-09 04:49:55.000000 pulumi_wavefront-3.2.0a1715229970/pulumi_wavefront/user_group.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 04:50:02.109978 pulumi_wavefront-3.2.0a1715229970/pulumi_wavefront.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2890 2024-05-09 04:50:02.000000 pulumi_wavefront-3.2.0a1715229970/pulumi_wavefront.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-05-09 04:50:02.000000 pulumi_wavefront-3.2.0a1715229970/pulumi_wavefront.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 04:50:02.000000 pulumi_wavefront-3.2.0a1715229970/pulumi_wavefront.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-09 04:50:02.000000 pulumi_wavefront-3.2.0a1715229970/pulumi_wavefront.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-09 04:50:02.000000 pulumi_wavefront-3.2.0a1715229970/pulumi_wavefront.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-09 04:49:55.000000 pulumi_wavefront-3.2.0a1715229970/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 04:50:02.113978 pulumi_wavefront-3.2.0a1715229970/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:54:31.198515 pulumi_wavefront-3.2.0a1715237486/
+-rw-r--r--   0 runner    (1001) docker     (127)     2890 2024-05-09 06:54:31.198515 pulumi_wavefront-3.2.0a1715237486/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-05-09 06:54:25.000000 pulumi_wavefront-3.2.0a1715237486/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:54:31.198515 pulumi_wavefront-3.2.0a1715237486/pulumi_wavefront/
+-rw-r--r--   0 runner    (1001) docker     (127)     6689 2024-05-09 06:54:25.000000 pulumi_wavefront-3.2.0a1715237486/pulumi_wavefront/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    80836 2024-05-09 06:54:25.000000 pulumi_wavefront-3.2.0a1715237486/pulumi_wavefront/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-05-09 06:54:25.000000 pulumi_wavefront-3.2.0a1715237486/pulumi_wavefront/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55260 2024-05-09 06:54:25.000000 pulumi_wavefront-3.2.0a1715237486/pulumi_wavefront/alert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33237 2024-05-09 06:54:25.000000 pulumi_wavefront-3.2.0a1715237486/pulumi_wavefront/alert_target.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46881 2024-05-09 06:54:25.000000 pulumi_wavefront-3.2.0a1715237486/pulumi_wavefront/cloud_integration_app_dynamics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4878 2024-05-09 06:54:25.000000 pulumi_wavefront-3.2.0a1715237486/pulumi_wavefront/cloud_integration_aws_external_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30693 2024-05-09 06:54:25.000000 pulumi_wavefront-3.2.0a1715237486/pulumi_wavefront/cloud_integration_azure.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26132 2024-05-09 06:54:25.000000 pulumi_wavefront-3.2.0a1715237486/pulumi_wavefront/cloud_integration_azure_activity_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28909 2024-05-09 06:54:25.000000 pulumi_wavefront-3.2.0a1715237486/pulumi_wavefront/cloud_integration_cloud_trail.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36675 2024-05-09 06:54:25.000000 pulumi_wavefront-3.2.0a1715237486/pulumi_wavefront/cloud_integration_cloud_watch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24169 2024-05-09 06:54:25.000000 pulumi_wavefront-3.2.0a1715237486/pulumi_wavefront/cloud_integration_ec2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29317 2024-05-09 06:54:25.000000 pulumi_wavefront-3.2.0a1715237486/pulumi_wavefront/cloud_integration_gcp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23736 2024-05-09 06:54:25.000000 pulumi_wavefront-3.2.0a1715237486/pulumi_wavefront/cloud_integration_gcp_billing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26312 2024-05-09 06:54:25.000000 pulumi_wavefront-3.2.0a1715237486/pulumi_wavefront/cloud_integration_new_relic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:54:31.198515 pulumi_wavefront-3.2.0a1715237486/pulumi_wavefront/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-09 06:54:25.000000 pulumi_wavefront-3.2.0a1715237486/pulumi_wavefront/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-09 06:54:25.000000 pulumi_wavefront-3.2.0a1715237486/pulumi_wavefront/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-09 06:54:25.000000 pulumi_wavefront-3.2.0a1715237486/pulumi_wavefront/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31524 2024-05-09 06:54:25.000000 pulumi_wavefront-3.2.0a1715237486/pulumi_wavefront/dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16825 2024-05-09 06:54:25.000000 pulumi_wavefront-3.2.0a1715237486/pulumi_wavefront/dashboard_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15111 2024-05-09 06:54:25.000000 pulumi_wavefront-3.2.0a1715237486/pulumi_wavefront/derived_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14267 2024-05-09 06:54:25.000000 pulumi_wavefront-3.2.0a1715237486/pulumi_wavefront/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25046 2024-05-09 06:54:25.000000 pulumi_wavefront-3.2.0a1715237486/pulumi_wavefront/external_link.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17778 2024-05-09 06:54:25.000000 pulumi_wavefront-3.2.0a1715237486/pulumi_wavefront/get_alert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4266 2024-05-09 06:54:25.000000 pulumi_wavefront-3.2.0a1715237486/pulumi_wavefront/get_alerts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19876 2024-05-09 06:54:25.000000 pulumi_wavefront-3.2.0a1715237486/pulumi_wavefront/get_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4439 2024-05-09 06:54:25.000000 pulumi_wavefront-3.2.0a1715237486/pulumi_wavefront/get_dashboards.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3065 2024-05-09 06:54:25.000000 pulumi_wavefront-3.2.0a1715237486/pulumi_wavefront/get_default_user_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15959 2024-05-09 06:54:25.000000 pulumi_wavefront-3.2.0a1715237486/pulumi_wavefront/get_derived_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4670 2024-05-09 06:54:25.000000 pulumi_wavefront-3.2.0a1715237486/pulumi_wavefront/get_derived_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6727 2024-05-09 06:54:25.000000 pulumi_wavefront-3.2.0a1715237486/pulumi_wavefront/get_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6874 2024-05-09 06:54:25.000000 pulumi_wavefront-3.2.0a1715237486/pulumi_wavefront/get_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9738 2024-05-09 06:54:25.000000 pulumi_wavefront-3.2.0a1715237486/pulumi_wavefront/get_external_link.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4625 2024-05-09 06:54:25.000000 pulumi_wavefront-3.2.0a1715237486/pulumi_wavefront/get_external_links.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13988 2024-05-09 06:54:25.000000 pulumi_wavefront-3.2.0a1715237486/pulumi_wavefront/get_maintenance_window.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3882 2024-05-09 06:54:25.000000 pulumi_wavefront-3.2.0a1715237486/pulumi_wavefront/get_maintenance_window_all.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3921 2024-05-09 06:54:25.000000 pulumi_wavefront-3.2.0a1715237486/pulumi_wavefront/get_metrics_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3902 2024-05-09 06:54:25.000000 pulumi_wavefront-3.2.0a1715237486/pulumi_wavefront/get_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4086 2024-05-09 06:54:25.000000 pulumi_wavefront-3.2.0a1715237486/pulumi_wavefront/get_roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5158 2024-05-09 06:54:25.000000 pulumi_wavefront-3.2.0a1715237486/pulumi_wavefront/get_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4436 2024-05-09 06:54:25.000000 pulumi_wavefront-3.2.0a1715237486/pulumi_wavefront/get_user_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4340 2024-05-09 06:54:25.000000 pulumi_wavefront-3.2.0a1715237486/pulumi_wavefront/get_user_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2621 2024-05-09 06:54:25.000000 pulumi_wavefront-3.2.0a1715237486/pulumi_wavefront/get_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17169 2024-05-09 06:54:25.000000 pulumi_wavefront-3.2.0a1715237486/pulumi_wavefront/ingestion_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34482 2024-05-09 06:54:25.000000 pulumi_wavefront-3.2.0a1715237486/pulumi_wavefront/maintenance_window.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12867 2024-05-09 06:54:25.000000 pulumi_wavefront-3.2.0a1715237486/pulumi_wavefront/metrics_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)   217687 2024-05-09 06:54:25.000000 pulumi_wavefront-3.2.0a1715237486/pulumi_wavefront/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5652 2024-05-09 06:54:25.000000 pulumi_wavefront-3.2.0a1715237486/pulumi_wavefront/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-09 06:54:25.000000 pulumi_wavefront-3.2.0a1715237486/pulumi_wavefront/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 06:54:25.000000 pulumi_wavefront-3.2.0a1715237486/pulumi_wavefront/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    14021 2024-05-09 06:54:25.000000 pulumi_wavefront-3.2.0a1715237486/pulumi_wavefront/role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18954 2024-05-09 06:54:25.000000 pulumi_wavefront-3.2.0a1715237486/pulumi_wavefront/service_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14393 2024-05-09 06:54:25.000000 pulumi_wavefront-3.2.0a1715237486/pulumi_wavefront/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8233 2024-05-09 06:54:25.000000 pulumi_wavefront-3.2.0a1715237486/pulumi_wavefront/user_group.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:54:31.198515 pulumi_wavefront-3.2.0a1715237486/pulumi_wavefront.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2890 2024-05-09 06:54:31.000000 pulumi_wavefront-3.2.0a1715237486/pulumi_wavefront.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-05-09 06:54:31.000000 pulumi_wavefront-3.2.0a1715237486/pulumi_wavefront.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 06:54:31.000000 pulumi_wavefront-3.2.0a1715237486/pulumi_wavefront.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-09 06:54:31.000000 pulumi_wavefront-3.2.0a1715237486/pulumi_wavefront.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-09 06:54:31.000000 pulumi_wavefront-3.2.0a1715237486/pulumi_wavefront.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-09 06:54:25.000000 pulumi_wavefront-3.2.0a1715237486/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 06:54:31.198515 pulumi_wavefront-3.2.0a1715237486/setup.cfg
```

### Comparing `pulumi_wavefront-3.2.0a1715229970/PKG-INFO` & `pulumi_wavefront-3.2.0a1715237486/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_wavefront
-Version: 3.2.0a1715229970
+Version: 3.2.0a1715237486
 Summary: A Pulumi package for creating and managing wavefront cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-wavefront
 Keywords: pulumi,wavefront
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_wavefront-3.2.0a1715229970/README.md` & `pulumi_wavefront-3.2.0a1715237486/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-3.2.0a1715229970/pulumi_wavefront/__init__.py` & `pulumi_wavefront-3.2.0a1715237486/pulumi_wavefront/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-3.2.0a1715229970/pulumi_wavefront/_inputs.py` & `pulumi_wavefront-3.2.0a1715237486/pulumi_wavefront/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-3.2.0a1715229970/pulumi_wavefront/_utilities.py` & `pulumi_wavefront-3.2.0a1715237486/pulumi_wavefront/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-3.2.0a1715229970/pulumi_wavefront/alert.py` & `pulumi_wavefront-3.2.0a1715237486/pulumi_wavefront/alert.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-3.2.0a1715229970/pulumi_wavefront/alert_target.py` & `pulumi_wavefront-3.2.0a1715237486/pulumi_wavefront/alert_target.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-3.2.0a1715229970/pulumi_wavefront/cloud_integration_app_dynamics.py` & `pulumi_wavefront-3.2.0a1715237486/pulumi_wavefront/cloud_integration_app_dynamics.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-3.2.0a1715229970/pulumi_wavefront/cloud_integration_aws_external_id.py` & `pulumi_wavefront-3.2.0a1715237486/pulumi_wavefront/cloud_integration_aws_external_id.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-3.2.0a1715229970/pulumi_wavefront/cloud_integration_azure.py` & `pulumi_wavefront-3.2.0a1715237486/pulumi_wavefront/cloud_integration_azure.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-3.2.0a1715229970/pulumi_wavefront/cloud_integration_azure_activity_log.py` & `pulumi_wavefront-3.2.0a1715237486/pulumi_wavefront/cloud_integration_azure_activity_log.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-3.2.0a1715229970/pulumi_wavefront/cloud_integration_cloud_trail.py` & `pulumi_wavefront-3.2.0a1715237486/pulumi_wavefront/cloud_integration_cloud_trail.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-3.2.0a1715229970/pulumi_wavefront/cloud_integration_cloud_watch.py` & `pulumi_wavefront-3.2.0a1715237486/pulumi_wavefront/cloud_integration_cloud_watch.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-3.2.0a1715229970/pulumi_wavefront/cloud_integration_ec2.py` & `pulumi_wavefront-3.2.0a1715237486/pulumi_wavefront/cloud_integration_ec2.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-3.2.0a1715229970/pulumi_wavefront/cloud_integration_gcp.py` & `pulumi_wavefront-3.2.0a1715237486/pulumi_wavefront/cloud_integration_gcp.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-3.2.0a1715229970/pulumi_wavefront/cloud_integration_gcp_billing.py` & `pulumi_wavefront-3.2.0a1715237486/pulumi_wavefront/cloud_integration_gcp_billing.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-3.2.0a1715229970/pulumi_wavefront/cloud_integration_new_relic.py` & `pulumi_wavefront-3.2.0a1715237486/pulumi_wavefront/cloud_integration_new_relic.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-3.2.0a1715229970/pulumi_wavefront/config/vars.py` & `pulumi_wavefront-3.2.0a1715237486/pulumi_wavefront/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-3.2.0a1715229970/pulumi_wavefront/dashboard.py` & `pulumi_wavefront-3.2.0a1715237486/pulumi_wavefront/dashboard.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-3.2.0a1715229970/pulumi_wavefront/dashboard_json.py` & `pulumi_wavefront-3.2.0a1715237486/pulumi_wavefront/dashboard_json.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-3.2.0a1715229970/pulumi_wavefront/derived_metric.py` & `pulumi_wavefront-3.2.0a1715237486/pulumi_wavefront/derived_metric.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-3.2.0a1715229970/pulumi_wavefront/event.py` & `pulumi_wavefront-3.2.0a1715237486/pulumi_wavefront/event.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-3.2.0a1715229970/pulumi_wavefront/external_link.py` & `pulumi_wavefront-3.2.0a1715237486/pulumi_wavefront/external_link.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-3.2.0a1715229970/pulumi_wavefront/get_alert.py` & `pulumi_wavefront-3.2.0a1715237486/pulumi_wavefront/get_alert.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-3.2.0a1715229970/pulumi_wavefront/get_alerts.py` & `pulumi_wavefront-3.2.0a1715237486/pulumi_wavefront/get_alerts.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-3.2.0a1715229970/pulumi_wavefront/get_dashboard.py` & `pulumi_wavefront-3.2.0a1715237486/pulumi_wavefront/get_dashboard.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-3.2.0a1715229970/pulumi_wavefront/get_dashboards.py` & `pulumi_wavefront-3.2.0a1715237486/pulumi_wavefront/get_dashboards.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-3.2.0a1715229970/pulumi_wavefront/get_default_user_group.py` & `pulumi_wavefront-3.2.0a1715237486/pulumi_wavefront/get_default_user_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-3.2.0a1715229970/pulumi_wavefront/get_derived_metric.py` & `pulumi_wavefront-3.2.0a1715237486/pulumi_wavefront/get_derived_metric.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-3.2.0a1715229970/pulumi_wavefront/get_derived_metrics.py` & `pulumi_wavefront-3.2.0a1715237486/pulumi_wavefront/get_derived_metrics.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-3.2.0a1715229970/pulumi_wavefront/get_event.py` & `pulumi_wavefront-3.2.0a1715237486/pulumi_wavefront/get_event.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-3.2.0a1715229970/pulumi_wavefront/get_events.py` & `pulumi_wavefront-3.2.0a1715237486/pulumi_wavefront/get_events.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-3.2.0a1715229970/pulumi_wavefront/get_external_link.py` & `pulumi_wavefront-3.2.0a1715237486/pulumi_wavefront/get_external_link.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-3.2.0a1715229970/pulumi_wavefront/get_external_links.py` & `pulumi_wavefront-3.2.0a1715237486/pulumi_wavefront/get_external_links.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-3.2.0a1715229970/pulumi_wavefront/get_maintenance_window.py` & `pulumi_wavefront-3.2.0a1715237486/pulumi_wavefront/get_maintenance_window.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-3.2.0a1715229970/pulumi_wavefront/get_maintenance_window_all.py` & `pulumi_wavefront-3.2.0a1715237486/pulumi_wavefront/get_maintenance_window_all.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-3.2.0a1715229970/pulumi_wavefront/get_metrics_policy.py` & `pulumi_wavefront-3.2.0a1715237486/pulumi_wavefront/get_metrics_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-3.2.0a1715229970/pulumi_wavefront/get_role.py` & `pulumi_wavefront-3.2.0a1715237486/pulumi_wavefront/get_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-3.2.0a1715229970/pulumi_wavefront/get_roles.py` & `pulumi_wavefront-3.2.0a1715237486/pulumi_wavefront/get_roles.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-3.2.0a1715229970/pulumi_wavefront/get_user.py` & `pulumi_wavefront-3.2.0a1715237486/pulumi_wavefront/get_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-3.2.0a1715229970/pulumi_wavefront/get_user_group.py` & `pulumi_wavefront-3.2.0a1715237486/pulumi_wavefront/get_user_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-3.2.0a1715229970/pulumi_wavefront/get_user_groups.py` & `pulumi_wavefront-3.2.0a1715237486/pulumi_wavefront/get_user_groups.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-3.2.0a1715229970/pulumi_wavefront/get_users.py` & `pulumi_wavefront-3.2.0a1715237486/pulumi_wavefront/get_users.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-3.2.0a1715229970/pulumi_wavefront/ingestion_policy.py` & `pulumi_wavefront-3.2.0a1715237486/pulumi_wavefront/ingestion_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-3.2.0a1715229970/pulumi_wavefront/maintenance_window.py` & `pulumi_wavefront-3.2.0a1715237486/pulumi_wavefront/maintenance_window.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-3.2.0a1715229970/pulumi_wavefront/metrics_policy.py` & `pulumi_wavefront-3.2.0a1715237486/pulumi_wavefront/metrics_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-3.2.0a1715229970/pulumi_wavefront/outputs.py` & `pulumi_wavefront-3.2.0a1715237486/pulumi_wavefront/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-3.2.0a1715229970/pulumi_wavefront/provider.py` & `pulumi_wavefront-3.2.0a1715237486/pulumi_wavefront/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-3.2.0a1715229970/pulumi_wavefront/role.py` & `pulumi_wavefront-3.2.0a1715237486/pulumi_wavefront/role.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-3.2.0a1715229970/pulumi_wavefront/service_account.py` & `pulumi_wavefront-3.2.0a1715237486/pulumi_wavefront/service_account.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-3.2.0a1715229970/pulumi_wavefront/user.py` & `pulumi_wavefront-3.2.0a1715237486/pulumi_wavefront/user.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-3.2.0a1715229970/pulumi_wavefront/user_group.py` & `pulumi_wavefront-3.2.0a1715237486/pulumi_wavefront/user_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-3.2.0a1715229970/pulumi_wavefront.egg-info/PKG-INFO` & `pulumi_wavefront-3.2.0a1715237486/pulumi_wavefront.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_wavefront
-Version: 3.2.0a1715229970
+Version: 3.2.0a1715237486
 Summary: A Pulumi package for creating and managing wavefront cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-wavefront
 Keywords: pulumi,wavefront
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_wavefront-3.2.0a1715229970/pulumi_wavefront.egg-info/SOURCES.txt` & `pulumi_wavefront-3.2.0a1715237486/pulumi_wavefront.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-3.2.0a1715229970/pyproject.toml` & `pulumi_wavefront-3.2.0a1715237486/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_wavefront"
   description = "A Pulumi package for creating and managing wavefront cloud resources."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "wavefront"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "3.2.0a1715229970"
+  version = "3.2.0a1715237486"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://pulumi.io"
     Repository = "https://github.com/pulumi/pulumi-wavefront"
 
 [build-system]
```

