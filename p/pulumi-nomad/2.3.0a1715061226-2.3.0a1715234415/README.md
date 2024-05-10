# Comparing `tmp/pulumi_nomad-2.3.0a1715061226.tar.gz` & `tmp/pulumi_nomad-2.3.0a1715234415.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_nomad-2.3.0a1715061226.tar", last modified: Tue May  7 06:01:12 2024, max compression
+gzip compressed data, was "pulumi_nomad-2.3.0a1715234415.tar", last modified: Thu May  9 06:07:57 2024, max compression
```

## Comparing `pulumi_nomad-2.3.0a1715061226.tar` & `pulumi_nomad-2.3.0a1715234415.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 06:01:12.627031 pulumi_nomad-2.3.0a1715061226/
--rw-r--r--   0 runner    (1001) docker     (127)     4727 2024-05-07 06:01:12.627031 pulumi_nomad-2.3.0a1715061226/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4279 2024-05-07 06:01:06.000000 pulumi_nomad-2.3.0a1715061226/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 06:01:12.627031 pulumi_nomad-2.3.0a1715061226/pulumi_nomad/
--rw-r--r--   0 runner    (1001) docker     (127)     4332 2024-05-07 06:01:06.000000 pulumi_nomad-2.3.0a1715061226/pulumi_nomad/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    68669 2024-05-07 06:01:06.000000 pulumi_nomad-2.3.0a1715061226/pulumi_nomad/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-05-07 06:01:06.000000 pulumi_nomad-2.3.0a1715061226/pulumi_nomad/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    23774 2024-05-07 06:01:06.000000 pulumi_nomad-2.3.0a1715061226/pulumi_nomad/acl_auth_method.py
--rw-r--r--   0 runner    (1001) docker     (127)    16396 2024-05-07 06:01:06.000000 pulumi_nomad-2.3.0a1715061226/pulumi_nomad/acl_binding_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    12176 2024-05-07 06:01:06.000000 pulumi_nomad-2.3.0a1715061226/pulumi_nomad/acl_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    10526 2024-05-07 06:01:06.000000 pulumi_nomad-2.3.0a1715061226/pulumi_nomad/acl_role.py
--rw-r--r--   0 runner    (1001) docker     (127)    28727 2024-05-07 06:01:06.000000 pulumi_nomad-2.3.0a1715061226/pulumi_nomad/acl_token.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 06:01:12.627031 pulumi_nomad-2.3.0a1715061226/pulumi_nomad/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-07 06:01:06.000000 pulumi_nomad-2.3.0a1715061226/pulumi_nomad/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-05-07 06:01:06.000000 pulumi_nomad-2.3.0a1715061226/pulumi_nomad/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-05-07 06:01:06.000000 pulumi_nomad-2.3.0a1715061226/pulumi_nomad/config/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3432 2024-05-07 06:01:06.000000 pulumi_nomad-2.3.0a1715061226/pulumi_nomad/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    48598 2024-05-07 06:01:06.000000 pulumi_nomad-2.3.0a1715061226/pulumi_nomad/csi_volume.py
--rw-r--r--   0 runner    (1001) docker     (127)    50513 2024-05-07 06:01:06.000000 pulumi_nomad-2.3.0a1715061226/pulumi_nomad/csi_volume_registration.py
--rw-r--r--   0 runner    (1001) docker     (127)    50425 2024-05-07 06:01:06.000000 pulumi_nomad-2.3.0a1715061226/pulumi_nomad/external_volume.py
--rw-r--r--   0 runner    (1001) docker     (127)     3550 2024-05-07 06:01:06.000000 pulumi_nomad-2.3.0a1715061226/pulumi_nomad/get_acl_policies.py
--rw-r--r--   0 runner    (1001) docker     (127)     3800 2024-05-07 06:01:06.000000 pulumi_nomad-2.3.0a1715061226/pulumi_nomad/get_acl_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3873 2024-05-07 06:01:06.000000 pulumi_nomad-2.3.0a1715061226/pulumi_nomad/get_acl_role.py
--rw-r--r--   0 runner    (1001) docker     (127)     3446 2024-05-07 06:01:06.000000 pulumi_nomad-2.3.0a1715061226/pulumi_nomad/get_acl_roles.py
--rw-r--r--   0 runner    (1001) docker     (127)     7630 2024-05-07 06:01:06.000000 pulumi_nomad-2.3.0a1715061226/pulumi_nomad/get_acl_token.py
--rw-r--r--   0 runner    (1001) docker     (127)     3419 2024-05-07 06:01:06.000000 pulumi_nomad-2.3.0a1715061226/pulumi_nomad/get_acl_tokens.py
--rw-r--r--   0 runner    (1001) docker     (127)     5350 2024-05-07 06:01:06.000000 pulumi_nomad-2.3.0a1715061226/pulumi_nomad/get_allocations.py
--rw-r--r--   0 runner    (1001) docker     (127)     4647 2024-05-07 06:01:06.000000 pulumi_nomad-2.3.0a1715061226/pulumi_nomad/get_datacenters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-05-07 06:01:06.000000 pulumi_nomad-2.3.0a1715061226/pulumi_nomad/get_deployments.py
--rw-r--r--   0 runner    (1001) docker     (127)    13404 2024-05-07 06:01:06.000000 pulumi_nomad-2.3.0a1715061226/pulumi_nomad/get_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     4001 2024-05-07 06:01:06.000000 pulumi_nomad-2.3.0a1715061226/pulumi_nomad/get_job_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     5344 2024-05-07 06:01:06.000000 pulumi_nomad-2.3.0a1715061226/pulumi_nomad/get_namespace.py
--rw-r--r--   0 runner    (1001) docker     (127)     3561 2024-05-07 06:01:06.000000 pulumi_nomad-2.3.0a1715061226/pulumi_nomad/get_namespaces.py
--rw-r--r--   0 runner    (1001) docker     (127)     4427 2024-05-07 06:01:06.000000 pulumi_nomad-2.3.0a1715061226/pulumi_nomad/get_node_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)     4370 2024-05-07 06:01:06.000000 pulumi_nomad-2.3.0a1715061226/pulumi_nomad/get_node_pools.py
--rw-r--r--   0 runner    (1001) docker     (127)    10732 2024-05-07 06:01:06.000000 pulumi_nomad-2.3.0a1715061226/pulumi_nomad/get_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-05-07 06:01:06.000000 pulumi_nomad-2.3.0a1715061226/pulumi_nomad/get_plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)     3286 2024-05-07 06:01:06.000000 pulumi_nomad-2.3.0a1715061226/pulumi_nomad/get_regions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4658 2024-05-07 06:01:06.000000 pulumi_nomad-2.3.0a1715061226/pulumi_nomad/get_scaling_policies.py
--rw-r--r--   0 runner    (1001) docker     (127)     5116 2024-05-07 06:01:06.000000 pulumi_nomad-2.3.0a1715061226/pulumi_nomad/get_scaling_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-05-07 06:01:06.000000 pulumi_nomad-2.3.0a1715061226/pulumi_nomad/get_scheduler_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     4113 2024-05-07 06:01:06.000000 pulumi_nomad-2.3.0a1715061226/pulumi_nomad/get_variable.py
--rw-r--r--   0 runner    (1001) docker     (127)     5420 2024-05-07 06:01:06.000000 pulumi_nomad-2.3.0a1715061226/pulumi_nomad/get_volumes.py
--rw-r--r--   0 runner    (1001) docker     (127)    51951 2024-05-07 06:01:06.000000 pulumi_nomad-2.3.0a1715061226/pulumi_nomad/job.py
--rw-r--r--   0 runner    (1001) docker     (127)    20505 2024-05-07 06:01:06.000000 pulumi_nomad-2.3.0a1715061226/pulumi_nomad/namespace.py
--rw-r--r--   0 runner    (1001) docker     (127)    13126 2024-05-07 06:01:06.000000 pulumi_nomad-2.3.0a1715061226/pulumi_nomad/node_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)    95392 2024-05-07 06:01:06.000000 pulumi_nomad-2.3.0a1715061226/pulumi_nomad/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    21549 2024-05-07 06:01:06.000000 pulumi_nomad-2.3.0a1715061226/pulumi_nomad/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-07 06:01:06.000000 pulumi_nomad-2.3.0a1715061226/pulumi_nomad/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 06:01:06.000000 pulumi_nomad-2.3.0a1715061226/pulumi_nomad/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    12113 2024-05-07 06:01:06.000000 pulumi_nomad-2.3.0a1715061226/pulumi_nomad/quote_specification.py
--rw-r--r--   0 runner    (1001) docker     (127)    14110 2024-05-07 06:01:06.000000 pulumi_nomad-2.3.0a1715061226/pulumi_nomad/scheduler_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    17058 2024-05-07 06:01:06.000000 pulumi_nomad-2.3.0a1715061226/pulumi_nomad/sentinel_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    11529 2024-05-07 06:01:06.000000 pulumi_nomad-2.3.0a1715061226/pulumi_nomad/variable.py
--rw-r--r--   0 runner    (1001) docker     (127)    55456 2024-05-07 06:01:06.000000 pulumi_nomad-2.3.0a1715061226/pulumi_nomad/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 06:01:12.627031 pulumi_nomad-2.3.0a1715061226/pulumi_nomad.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4727 2024-05-07 06:01:12.000000 pulumi_nomad-2.3.0a1715061226/pulumi_nomad.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-05-07 06:01:12.000000 pulumi_nomad-2.3.0a1715061226/pulumi_nomad.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 06:01:12.000000 pulumi_nomad-2.3.0a1715061226/pulumi_nomad.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-07 06:01:12.000000 pulumi_nomad-2.3.0a1715061226/pulumi_nomad.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-07 06:01:12.000000 pulumi_nomad-2.3.0a1715061226/pulumi_nomad.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-05-07 06:01:06.000000 pulumi_nomad-2.3.0a1715061226/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 06:01:12.627031 pulumi_nomad-2.3.0a1715061226/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:07:57.651249 pulumi_nomad-2.3.0a1715234415/
+-rw-r--r--   0 runner    (1001) docker     (127)     4727 2024-05-09 06:07:57.651249 pulumi_nomad-2.3.0a1715234415/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4279 2024-05-09 06:07:51.000000 pulumi_nomad-2.3.0a1715234415/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:07:57.651249 pulumi_nomad-2.3.0a1715234415/pulumi_nomad/
+-rw-r--r--   0 runner    (1001) docker     (127)     4332 2024-05-09 06:07:51.000000 pulumi_nomad-2.3.0a1715234415/pulumi_nomad/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68669 2024-05-09 06:07:51.000000 pulumi_nomad-2.3.0a1715234415/pulumi_nomad/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-05-09 06:07:51.000000 pulumi_nomad-2.3.0a1715234415/pulumi_nomad/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23774 2024-05-09 06:07:51.000000 pulumi_nomad-2.3.0a1715234415/pulumi_nomad/acl_auth_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16396 2024-05-09 06:07:51.000000 pulumi_nomad-2.3.0a1715234415/pulumi_nomad/acl_binding_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12176 2024-05-09 06:07:51.000000 pulumi_nomad-2.3.0a1715234415/pulumi_nomad/acl_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10526 2024-05-09 06:07:51.000000 pulumi_nomad-2.3.0a1715234415/pulumi_nomad/acl_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28727 2024-05-09 06:07:51.000000 pulumi_nomad-2.3.0a1715234415/pulumi_nomad/acl_token.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:07:57.651249 pulumi_nomad-2.3.0a1715234415/pulumi_nomad/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-09 06:07:51.000000 pulumi_nomad-2.3.0a1715234415/pulumi_nomad/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-05-09 06:07:51.000000 pulumi_nomad-2.3.0a1715234415/pulumi_nomad/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-05-09 06:07:51.000000 pulumi_nomad-2.3.0a1715234415/pulumi_nomad/config/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3432 2024-05-09 06:07:51.000000 pulumi_nomad-2.3.0a1715234415/pulumi_nomad/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48598 2024-05-09 06:07:51.000000 pulumi_nomad-2.3.0a1715234415/pulumi_nomad/csi_volume.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50513 2024-05-09 06:07:51.000000 pulumi_nomad-2.3.0a1715234415/pulumi_nomad/csi_volume_registration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50425 2024-05-09 06:07:51.000000 pulumi_nomad-2.3.0a1715234415/pulumi_nomad/external_volume.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3550 2024-05-09 06:07:51.000000 pulumi_nomad-2.3.0a1715234415/pulumi_nomad/get_acl_policies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3800 2024-05-09 06:07:51.000000 pulumi_nomad-2.3.0a1715234415/pulumi_nomad/get_acl_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3873 2024-05-09 06:07:51.000000 pulumi_nomad-2.3.0a1715234415/pulumi_nomad/get_acl_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3446 2024-05-09 06:07:51.000000 pulumi_nomad-2.3.0a1715234415/pulumi_nomad/get_acl_roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7630 2024-05-09 06:07:51.000000 pulumi_nomad-2.3.0a1715234415/pulumi_nomad/get_acl_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3419 2024-05-09 06:07:51.000000 pulumi_nomad-2.3.0a1715234415/pulumi_nomad/get_acl_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5350 2024-05-09 06:07:51.000000 pulumi_nomad-2.3.0a1715234415/pulumi_nomad/get_allocations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4647 2024-05-09 06:07:51.000000 pulumi_nomad-2.3.0a1715234415/pulumi_nomad/get_datacenters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-05-09 06:07:51.000000 pulumi_nomad-2.3.0a1715234415/pulumi_nomad/get_deployments.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13404 2024-05-09 06:07:51.000000 pulumi_nomad-2.3.0a1715234415/pulumi_nomad/get_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4001 2024-05-09 06:07:51.000000 pulumi_nomad-2.3.0a1715234415/pulumi_nomad/get_job_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5344 2024-05-09 06:07:51.000000 pulumi_nomad-2.3.0a1715234415/pulumi_nomad/get_namespace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3561 2024-05-09 06:07:51.000000 pulumi_nomad-2.3.0a1715234415/pulumi_nomad/get_namespaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4427 2024-05-09 06:07:51.000000 pulumi_nomad-2.3.0a1715234415/pulumi_nomad/get_node_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4370 2024-05-09 06:07:51.000000 pulumi_nomad-2.3.0a1715234415/pulumi_nomad/get_node_pools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10732 2024-05-09 06:07:51.000000 pulumi_nomad-2.3.0a1715234415/pulumi_nomad/get_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-05-09 06:07:51.000000 pulumi_nomad-2.3.0a1715234415/pulumi_nomad/get_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3286 2024-05-09 06:07:51.000000 pulumi_nomad-2.3.0a1715234415/pulumi_nomad/get_regions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4658 2024-05-09 06:07:51.000000 pulumi_nomad-2.3.0a1715234415/pulumi_nomad/get_scaling_policies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5116 2024-05-09 06:07:51.000000 pulumi_nomad-2.3.0a1715234415/pulumi_nomad/get_scaling_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-05-09 06:07:51.000000 pulumi_nomad-2.3.0a1715234415/pulumi_nomad/get_scheduler_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4113 2024-05-09 06:07:51.000000 pulumi_nomad-2.3.0a1715234415/pulumi_nomad/get_variable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5420 2024-05-09 06:07:51.000000 pulumi_nomad-2.3.0a1715234415/pulumi_nomad/get_volumes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51951 2024-05-09 06:07:51.000000 pulumi_nomad-2.3.0a1715234415/pulumi_nomad/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20505 2024-05-09 06:07:51.000000 pulumi_nomad-2.3.0a1715234415/pulumi_nomad/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13126 2024-05-09 06:07:51.000000 pulumi_nomad-2.3.0a1715234415/pulumi_nomad/node_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)    95392 2024-05-09 06:07:51.000000 pulumi_nomad-2.3.0a1715234415/pulumi_nomad/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21549 2024-05-09 06:07:51.000000 pulumi_nomad-2.3.0a1715234415/pulumi_nomad/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-09 06:07:51.000000 pulumi_nomad-2.3.0a1715234415/pulumi_nomad/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 06:07:51.000000 pulumi_nomad-2.3.0a1715234415/pulumi_nomad/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    12113 2024-05-09 06:07:51.000000 pulumi_nomad-2.3.0a1715234415/pulumi_nomad/quote_specification.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14110 2024-05-09 06:07:51.000000 pulumi_nomad-2.3.0a1715234415/pulumi_nomad/scheduler_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17058 2024-05-09 06:07:51.000000 pulumi_nomad-2.3.0a1715234415/pulumi_nomad/sentinel_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11529 2024-05-09 06:07:51.000000 pulumi_nomad-2.3.0a1715234415/pulumi_nomad/variable.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55456 2024-05-09 06:07:51.000000 pulumi_nomad-2.3.0a1715234415/pulumi_nomad/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:07:57.651249 pulumi_nomad-2.3.0a1715234415/pulumi_nomad.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4727 2024-05-09 06:07:57.000000 pulumi_nomad-2.3.0a1715234415/pulumi_nomad.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-05-09 06:07:57.000000 pulumi_nomad-2.3.0a1715234415/pulumi_nomad.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 06:07:57.000000 pulumi_nomad-2.3.0a1715234415/pulumi_nomad.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-09 06:07:57.000000 pulumi_nomad-2.3.0a1715234415/pulumi_nomad.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-09 06:07:57.000000 pulumi_nomad-2.3.0a1715234415/pulumi_nomad.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-05-09 06:07:51.000000 pulumi_nomad-2.3.0a1715234415/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 06:07:57.651249 pulumi_nomad-2.3.0a1715234415/setup.cfg
```

### Comparing `pulumi_nomad-2.3.0a1715061226/PKG-INFO` & `pulumi_nomad-2.3.0a1715234415/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_nomad
-Version: 2.3.0a1715061226
+Version: 2.3.0a1715234415
 Summary: A Pulumi package for creating and managing nomad cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-nomad
 Keywords: pulumi,nomad
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_nomad-2.3.0a1715061226/README.md` & `pulumi_nomad-2.3.0a1715234415/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-2.3.0a1715061226/pulumi_nomad/__init__.py` & `pulumi_nomad-2.3.0a1715234415/pulumi_nomad/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-2.3.0a1715061226/pulumi_nomad/_inputs.py` & `pulumi_nomad-2.3.0a1715234415/pulumi_nomad/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-2.3.0a1715061226/pulumi_nomad/_utilities.py` & `pulumi_nomad-2.3.0a1715234415/pulumi_nomad/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-2.3.0a1715061226/pulumi_nomad/acl_auth_method.py` & `pulumi_nomad-2.3.0a1715234415/pulumi_nomad/acl_auth_method.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-2.3.0a1715061226/pulumi_nomad/acl_binding_rule.py` & `pulumi_nomad-2.3.0a1715234415/pulumi_nomad/acl_binding_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-2.3.0a1715061226/pulumi_nomad/acl_policy.py` & `pulumi_nomad-2.3.0a1715234415/pulumi_nomad/acl_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-2.3.0a1715061226/pulumi_nomad/acl_role.py` & `pulumi_nomad-2.3.0a1715234415/pulumi_nomad/acl_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-2.3.0a1715061226/pulumi_nomad/acl_token.py` & `pulumi_nomad-2.3.0a1715234415/pulumi_nomad/acl_token.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-2.3.0a1715061226/pulumi_nomad/config/__init__.pyi` & `pulumi_nomad-2.3.0a1715234415/pulumi_nomad/config/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-2.3.0a1715061226/pulumi_nomad/config/outputs.py` & `pulumi_nomad-2.3.0a1715234415/pulumi_nomad/config/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-2.3.0a1715061226/pulumi_nomad/config/vars.py` & `pulumi_nomad-2.3.0a1715234415/pulumi_nomad/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-2.3.0a1715061226/pulumi_nomad/csi_volume.py` & `pulumi_nomad-2.3.0a1715234415/pulumi_nomad/csi_volume.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-2.3.0a1715061226/pulumi_nomad/csi_volume_registration.py` & `pulumi_nomad-2.3.0a1715234415/pulumi_nomad/csi_volume_registration.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-2.3.0a1715061226/pulumi_nomad/external_volume.py` & `pulumi_nomad-2.3.0a1715234415/pulumi_nomad/external_volume.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-2.3.0a1715061226/pulumi_nomad/get_acl_policies.py` & `pulumi_nomad-2.3.0a1715234415/pulumi_nomad/get_acl_policies.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-2.3.0a1715061226/pulumi_nomad/get_acl_policy.py` & `pulumi_nomad-2.3.0a1715234415/pulumi_nomad/get_acl_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-2.3.0a1715061226/pulumi_nomad/get_acl_role.py` & `pulumi_nomad-2.3.0a1715234415/pulumi_nomad/get_acl_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-2.3.0a1715061226/pulumi_nomad/get_acl_roles.py` & `pulumi_nomad-2.3.0a1715234415/pulumi_nomad/get_acl_roles.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-2.3.0a1715061226/pulumi_nomad/get_acl_token.py` & `pulumi_nomad-2.3.0a1715234415/pulumi_nomad/get_acl_token.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-2.3.0a1715061226/pulumi_nomad/get_acl_tokens.py` & `pulumi_nomad-2.3.0a1715234415/pulumi_nomad/get_acl_tokens.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-2.3.0a1715061226/pulumi_nomad/get_allocations.py` & `pulumi_nomad-2.3.0a1715234415/pulumi_nomad/get_allocations.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-2.3.0a1715061226/pulumi_nomad/get_datacenters.py` & `pulumi_nomad-2.3.0a1715234415/pulumi_nomad/get_datacenters.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-2.3.0a1715061226/pulumi_nomad/get_deployments.py` & `pulumi_nomad-2.3.0a1715234415/pulumi_nomad/get_deployments.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-2.3.0a1715061226/pulumi_nomad/get_job.py` & `pulumi_nomad-2.3.0a1715234415/pulumi_nomad/get_job.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-2.3.0a1715061226/pulumi_nomad/get_job_parser.py` & `pulumi_nomad-2.3.0a1715234415/pulumi_nomad/get_job_parser.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-2.3.0a1715061226/pulumi_nomad/get_namespace.py` & `pulumi_nomad-2.3.0a1715234415/pulumi_nomad/get_namespace.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-2.3.0a1715061226/pulumi_nomad/get_namespaces.py` & `pulumi_nomad-2.3.0a1715234415/pulumi_nomad/get_namespaces.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-2.3.0a1715061226/pulumi_nomad/get_node_pool.py` & `pulumi_nomad-2.3.0a1715234415/pulumi_nomad/get_node_pool.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-2.3.0a1715061226/pulumi_nomad/get_node_pools.py` & `pulumi_nomad-2.3.0a1715234415/pulumi_nomad/get_node_pools.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-2.3.0a1715061226/pulumi_nomad/get_plugin.py` & `pulumi_nomad-2.3.0a1715234415/pulumi_nomad/get_plugin.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-2.3.0a1715061226/pulumi_nomad/get_plugins.py` & `pulumi_nomad-2.3.0a1715234415/pulumi_nomad/get_plugins.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-2.3.0a1715061226/pulumi_nomad/get_regions.py` & `pulumi_nomad-2.3.0a1715234415/pulumi_nomad/get_regions.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-2.3.0a1715061226/pulumi_nomad/get_scaling_policies.py` & `pulumi_nomad-2.3.0a1715234415/pulumi_nomad/get_scaling_policies.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-2.3.0a1715061226/pulumi_nomad/get_scaling_policy.py` & `pulumi_nomad-2.3.0a1715234415/pulumi_nomad/get_scaling_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-2.3.0a1715061226/pulumi_nomad/get_scheduler_policy.py` & `pulumi_nomad-2.3.0a1715234415/pulumi_nomad/get_scheduler_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-2.3.0a1715061226/pulumi_nomad/get_variable.py` & `pulumi_nomad-2.3.0a1715234415/pulumi_nomad/get_variable.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-2.3.0a1715061226/pulumi_nomad/get_volumes.py` & `pulumi_nomad-2.3.0a1715234415/pulumi_nomad/get_volumes.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-2.3.0a1715061226/pulumi_nomad/job.py` & `pulumi_nomad-2.3.0a1715234415/pulumi_nomad/job.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-2.3.0a1715061226/pulumi_nomad/namespace.py` & `pulumi_nomad-2.3.0a1715234415/pulumi_nomad/namespace.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-2.3.0a1715061226/pulumi_nomad/node_pool.py` & `pulumi_nomad-2.3.0a1715234415/pulumi_nomad/node_pool.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-2.3.0a1715061226/pulumi_nomad/outputs.py` & `pulumi_nomad-2.3.0a1715234415/pulumi_nomad/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-2.3.0a1715061226/pulumi_nomad/provider.py` & `pulumi_nomad-2.3.0a1715234415/pulumi_nomad/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-2.3.0a1715061226/pulumi_nomad/quote_specification.py` & `pulumi_nomad-2.3.0a1715234415/pulumi_nomad/quote_specification.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-2.3.0a1715061226/pulumi_nomad/scheduler_config.py` & `pulumi_nomad-2.3.0a1715234415/pulumi_nomad/scheduler_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-2.3.0a1715061226/pulumi_nomad/sentinel_policy.py` & `pulumi_nomad-2.3.0a1715234415/pulumi_nomad/sentinel_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-2.3.0a1715061226/pulumi_nomad/variable.py` & `pulumi_nomad-2.3.0a1715234415/pulumi_nomad/variable.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-2.3.0a1715061226/pulumi_nomad/volume.py` & `pulumi_nomad-2.3.0a1715234415/pulumi_nomad/volume.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-2.3.0a1715061226/pulumi_nomad.egg-info/PKG-INFO` & `pulumi_nomad-2.3.0a1715234415/pulumi_nomad.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_nomad
-Version: 2.3.0a1715061226
+Version: 2.3.0a1715234415
 Summary: A Pulumi package for creating and managing nomad cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-nomad
 Keywords: pulumi,nomad
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_nomad-2.3.0a1715061226/pulumi_nomad.egg-info/SOURCES.txt` & `pulumi_nomad-2.3.0a1715234415/pulumi_nomad.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-2.3.0a1715061226/pyproject.toml` & `pulumi_nomad-2.3.0a1715234415/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_nomad"
   description = "A Pulumi package for creating and managing nomad cloud resources."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "nomad"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "2.3.0a1715061226"
+  version = "2.3.0a1715234415"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://pulumi.io"
     Repository = "https://github.com/pulumi/pulumi-nomad"
 
 [build-system]
```

