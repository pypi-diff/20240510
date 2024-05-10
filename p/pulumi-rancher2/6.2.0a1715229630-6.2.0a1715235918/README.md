# Comparing `tmp/pulumi_rancher2-6.2.0a1715229630.tar.gz` & `tmp/pulumi_rancher2-6.2.0a1715235918.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_rancher2-6.2.0a1715229630.tar", last modified: Thu May  9 04:47:25 2024, max compression
+gzip compressed data, was "pulumi_rancher2-6.2.0a1715235918.tar", last modified: Thu May  9 06:37:15 2024, max compression
```

## Comparing `pulumi_rancher2-6.2.0a1715229630.tar` & `pulumi_rancher2-6.2.0a1715235918.tar`

### file list

```diff
@@ -1,113 +1,113 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 04:47:25.248287 pulumi_rancher2-6.2.0a1715229630/
--rw-r--r--   0 runner    (1001) docker     (127)     3763 2024-05-09 04:47:25.248287 pulumi_rancher2-6.2.0a1715229630/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-05-09 04:47:19.000000 pulumi_rancher2-6.2.0a1715229630/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 04:47:25.248287 pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/
--rw-r--r--   0 runner    (1001) docker     (127)    12750 2024-05-09 04:47:19.000000 pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)  1231524 2024-05-09 04:47:19.000000 pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-05-09 04:47:19.000000 pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    40997 2024-05-09 04:47:19.000000 pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/app.py
--rw-r--r--   0 runner    (1001) docker     (127)    42135 2024-05-09 04:47:19.000000 pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/app_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    81707 2024-05-09 04:47:19.000000 pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/auth_config_active_directory.py
--rw-r--r--   0 runner    (1001) docker     (127)    35228 2024-05-09 04:47:19.000000 pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/auth_config_adfs.py
--rw-r--r--   0 runner    (1001) docker     (127)    34916 2024-05-09 04:47:19.000000 pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/auth_config_azure_ad.py
--rw-r--r--   0 runner    (1001) docker     (127)    79388 2024-05-09 04:47:19.000000 pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/auth_config_free_ipa.py
--rw-r--r--   0 runner    (1001) docker     (127)    26284 2024-05-09 04:47:19.000000 pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/auth_config_github.py
--rw-r--r--   0 runner    (1001) docker     (127)    37428 2024-05-09 04:47:19.000000 pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/auth_config_keycloak.py
--rw-r--r--   0 runner    (1001) docker     (127)    35228 2024-05-09 04:47:19.000000 pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/auth_config_okta.py
--rw-r--r--   0 runner    (1001) docker     (127)    79475 2024-05-09 04:47:19.000000 pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/auth_config_open_ldap.py
--rw-r--r--   0 runner    (1001) docker     (127)    37231 2024-05-09 04:47:19.000000 pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/auth_config_ping.py
--rw-r--r--   0 runner    (1001) docker     (127)    26466 2024-05-09 04:47:19.000000 pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (127)    32946 2024-05-09 04:47:19.000000 pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)    34833 2024-05-09 04:47:19.000000 pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/catalog_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    19683 2024-05-09 04:47:19.000000 pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/certificate.py
--rw-r--r--   0 runner    (1001) docker     (127)    45398 2024-05-09 04:47:19.000000 pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/cloud_credential.py
--rw-r--r--   0 runner    (1001) docker     (127)   165840 2024-05-09 04:47:19.000000 pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)    24984 2024-05-09 04:47:19.000000 pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/cluster_alert_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    39406 2024-05-09 04:47:19.000000 pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/cluster_alert_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    24090 2024-05-09 04:47:19.000000 pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/cluster_driver.py
--rw-r--r--   0 runner    (1001) docker     (127)    25533 2024-05-09 04:47:19.000000 pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/cluster_role_template_binding.py
--rw-r--r--   0 runner    (1001) docker     (127)    31474 2024-05-09 04:47:19.000000 pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/cluster_sync.py
--rw-r--r--   0 runner    (1001) docker     (127)    25124 2024-05-09 04:47:19.000000 pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/cluster_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    62895 2024-05-09 04:47:19.000000 pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/cluster_v2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 04:47:25.248287 pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-09 04:47:19.000000 pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-05-09 04:47:19.000000 pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-05-09 04:47:19.000000 pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    20013 2024-05-09 04:47:19.000000 pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/config_map_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    32339 2024-05-09 04:47:19.000000 pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/custom_user_token.py
--rw-r--r--   0 runner    (1001) docker     (127)    22233 2024-05-09 04:47:19.000000 pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/etcd_backup.py
--rw-r--r--   0 runner    (1001) docker     (127)    13050 2024-05-09 04:47:19.000000 pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/feature.py
--rw-r--r--   0 runner    (1001) docker     (127)    10022 2024-05-09 04:47:19.000000 pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/get_app.py
--rw-r--r--   0 runner    (1001) docker     (127)     8774 2024-05-09 04:47:19.000000 pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/get_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)    10474 2024-05-09 04:47:19.000000 pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/get_catalog_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     7568 2024-05-09 04:47:19.000000 pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/get_certificate.py
--rw-r--r--   0 runner    (1001) docker     (127)     3968 2024-05-09 04:47:19.000000 pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/get_cloud_credential.py
--rw-r--r--   0 runner    (1001) docker     (127)    25468 2024-05-09 04:47:19.000000 pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/get_cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     8053 2024-05-09 04:47:19.000000 pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/get_cluster_alert_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    11563 2024-05-09 04:47:19.000000 pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/get_cluster_alert_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     7688 2024-05-09 04:47:19.000000 pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/get_cluster_driver.py
--rw-r--r--   0 runner    (1001) docker     (127)     8388 2024-05-09 04:47:19.000000 pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/get_cluster_role_template_binding.py
--rw-r--r--   0 runner    (1001) docker     (127)     7346 2024-05-09 04:47:19.000000 pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/get_cluster_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    13468 2024-05-09 04:47:19.000000 pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/get_cluster_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6850 2024-05-09 04:47:19.000000 pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/get_config_map_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6766 2024-05-09 04:47:19.000000 pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/get_etcd_backup.py
--rw-r--r--   0 runner    (1001) docker     (127)     6776 2024-05-09 04:47:19.000000 pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/get_global_dns_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     7338 2024-05-09 04:47:19.000000 pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/get_global_role.py
--rw-r--r--   0 runner    (1001) docker     (127)     6076 2024-05-09 04:47:19.000000 pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/get_global_role_binding.py
--rw-r--r--   0 runner    (1001) docker     (127)    10228 2024-05-09 04:47:19.000000 pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/get_multi_cluster_app.py
--rw-r--r--   0 runner    (1001) docker     (127)     6599 2024-05-09 04:47:19.000000 pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/get_namespace.py
--rw-r--r--   0 runner    (1001) docker     (127)     8092 2024-05-09 04:47:19.000000 pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/get_node_driver.py
--rw-r--r--   0 runner    (1001) docker     (127)     9339 2024-05-09 04:47:19.000000 pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/get_node_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)    11657 2024-05-09 04:47:19.000000 pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/get_node_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    10488 2024-05-09 04:47:19.000000 pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/get_notifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     5826 2024-05-09 04:47:19.000000 pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/get_pod_security_admission_configuration_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    29295 2024-05-09 04:47:19.000000 pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/get_pod_security_policy_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     3653 2024-05-09 04:47:19.000000 pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/get_principal.py
--rw-r--r--   0 runner    (1001) docker     (127)     7956 2024-05-09 04:47:19.000000 pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/get_project.py
--rw-r--r--   0 runner    (1001) docker     (127)     8053 2024-05-09 04:47:19.000000 pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/get_project_alert_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    10768 2024-05-09 04:47:19.000000 pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/get_project_alert_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     8388 2024-05-09 04:47:19.000000 pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/get_project_role_template_binding.py
--rw-r--r--   0 runner    (1001) docker     (127)     7583 2024-05-09 04:47:19.000000 pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/get_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     9189 2024-05-09 04:47:19.000000 pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/get_role_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     7362 2024-05-09 04:47:19.000000 pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/get_secret.py
--rw-r--r--   0 runner    (1001) docker     (127)     7340 2024-05-09 04:47:19.000000 pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/get_secret_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3198 2024-05-09 04:47:19.000000 pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/get_setting.py
--rw-r--r--   0 runner    (1001) docker     (127)     8732 2024-05-09 04:47:19.000000 pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/get_storage_class_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6246 2024-05-09 04:47:19.000000 pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/get_user.py
--rw-r--r--   0 runner    (1001) docker     (127)    23658 2024-05-09 04:47:19.000000 pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/global_dns.py
--rw-r--r--   0 runner    (1001) docker     (127)    22371 2024-05-09 04:47:19.000000 pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/global_dns_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)    21535 2024-05-09 04:47:19.000000 pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/global_role.py
--rw-r--r--   0 runner    (1001) docker     (127)    19056 2024-05-09 04:47:19.000000 pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/global_role_binding.py
--rw-r--r--   0 runner    (1001) docker     (127)    47117 2024-05-09 04:47:19.000000 pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/machine_config_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    41596 2024-05-09 04:47:19.000000 pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/multi_cluster_app.py
--rw-r--r--   0 runner    (1001) docker     (127)    27977 2024-05-09 04:47:19.000000 pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/namespace.py
--rw-r--r--   0 runner    (1001) docker     (127)    26635 2024-05-09 04:47:19.000000 pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/node_driver.py
--rw-r--r--   0 runner    (1001) docker     (127)    31706 2024-05-09 04:47:19.000000 pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/node_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)    83435 2024-05-09 04:47:19.000000 pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/node_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    34476 2024-05-09 04:47:19.000000 pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/notifier.py
--rw-r--r--   0 runner    (1001) docker     (127)  1667240 2024-05-09 04:47:19.000000 pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    18319 2024-05-09 04:47:19.000000 pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/pod_security_admission_configuration_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    69311 2024-05-09 04:47:19.000000 pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/pod_security_policy_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    37721 2024-05-09 04:47:19.000000 pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/project.py
--rw-r--r--   0 runner    (1001) docker     (127)    24984 2024-05-09 04:47:19.000000 pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/project_alert_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    37740 2024-05-09 04:47:19.000000 pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/project_alert_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    25638 2024-05-09 04:47:19.000000 pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/project_role_template_binding.py
--rw-r--r--   0 runner    (1001) docker     (127)    14405 2024-05-09 04:47:19.000000 pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-09 04:47:19.000000 pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 04:47:19.000000 pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    21460 2024-05-09 04:47:19.000000 pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)    31723 2024-05-09 04:47:19.000000 pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/role_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    21070 2024-05-09 04:47:19.000000 pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/secret.py
--rw-r--r--   0 runner    (1001) docker     (127)    23036 2024-05-09 04:47:19.000000 pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/secret_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    12440 2024-05-09 04:47:19.000000 pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/setting.py
--rw-r--r--   0 runner    (1001) docker     (127)    28123 2024-05-09 04:47:19.000000 pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/storage_class_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    23952 2024-05-09 04:47:19.000000 pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/token.py
--rw-r--r--   0 runner    (1001) docker     (127)    17201 2024-05-09 04:47:19.000000 pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 04:47:25.248287 pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3763 2024-05-09 04:47:25.000000 pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3753 2024-05-09 04:47:25.000000 pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 04:47:25.000000 pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-09 04:47:25.000000 pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-09 04:47:25.000000 pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-09 04:47:19.000000 pulumi_rancher2-6.2.0a1715229630/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 04:47:25.248287 pulumi_rancher2-6.2.0a1715229630/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:37:15.421433 pulumi_rancher2-6.2.0a1715235918/
+-rw-r--r--   0 runner    (1001) docker     (127)     3763 2024-05-09 06:37:15.421433 pulumi_rancher2-6.2.0a1715235918/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-05-09 06:37:09.000000 pulumi_rancher2-6.2.0a1715235918/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:37:15.421433 pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/
+-rw-r--r--   0 runner    (1001) docker     (127)    12750 2024-05-09 06:37:09.000000 pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1231524 2024-05-09 06:37:09.000000 pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-05-09 06:37:09.000000 pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40997 2024-05-09 06:37:09.000000 pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42135 2024-05-09 06:37:09.000000 pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/app_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    81707 2024-05-09 06:37:09.000000 pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/auth_config_active_directory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35228 2024-05-09 06:37:09.000000 pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/auth_config_adfs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34916 2024-05-09 06:37:09.000000 pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/auth_config_azure_ad.py
+-rw-r--r--   0 runner    (1001) docker     (127)    79388 2024-05-09 06:37:09.000000 pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/auth_config_free_ipa.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26284 2024-05-09 06:37:09.000000 pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/auth_config_github.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37428 2024-05-09 06:37:09.000000 pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/auth_config_keycloak.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35228 2024-05-09 06:37:09.000000 pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/auth_config_okta.py
+-rw-r--r--   0 runner    (1001) docker     (127)    79475 2024-05-09 06:37:09.000000 pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/auth_config_open_ldap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37231 2024-05-09 06:37:09.000000 pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/auth_config_ping.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26466 2024-05-09 06:37:09.000000 pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32946 2024-05-09 06:37:09.000000 pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34833 2024-05-09 06:37:09.000000 pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/catalog_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19683 2024-05-09 06:37:09.000000 pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/certificate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45398 2024-05-09 06:37:09.000000 pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/cloud_credential.py
+-rw-r--r--   0 runner    (1001) docker     (127)   165840 2024-05-09 06:37:09.000000 pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24984 2024-05-09 06:37:09.000000 pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/cluster_alert_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39406 2024-05-09 06:37:09.000000 pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/cluster_alert_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24090 2024-05-09 06:37:09.000000 pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/cluster_driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25533 2024-05-09 06:37:09.000000 pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/cluster_role_template_binding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31474 2024-05-09 06:37:09.000000 pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/cluster_sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25124 2024-05-09 06:37:09.000000 pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/cluster_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62895 2024-05-09 06:37:09.000000 pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/cluster_v2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:37:15.421433 pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-09 06:37:09.000000 pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-05-09 06:37:09.000000 pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-05-09 06:37:09.000000 pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20013 2024-05-09 06:37:09.000000 pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/config_map_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32339 2024-05-09 06:37:09.000000 pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/custom_user_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22233 2024-05-09 06:37:09.000000 pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/etcd_backup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13050 2024-05-09 06:37:09.000000 pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10022 2024-05-09 06:37:09.000000 pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/get_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8774 2024-05-09 06:37:09.000000 pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/get_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10474 2024-05-09 06:37:09.000000 pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/get_catalog_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7568 2024-05-09 06:37:09.000000 pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/get_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3968 2024-05-09 06:37:09.000000 pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/get_cloud_credential.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25468 2024-05-09 06:37:09.000000 pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/get_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8053 2024-05-09 06:37:09.000000 pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/get_cluster_alert_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11563 2024-05-09 06:37:09.000000 pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/get_cluster_alert_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7688 2024-05-09 06:37:09.000000 pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/get_cluster_driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8388 2024-05-09 06:37:09.000000 pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/get_cluster_role_template_binding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7346 2024-05-09 06:37:09.000000 pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/get_cluster_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13468 2024-05-09 06:37:09.000000 pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/get_cluster_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6850 2024-05-09 06:37:09.000000 pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/get_config_map_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6766 2024-05-09 06:37:09.000000 pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/get_etcd_backup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6776 2024-05-09 06:37:09.000000 pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/get_global_dns_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7338 2024-05-09 06:37:09.000000 pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/get_global_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6076 2024-05-09 06:37:09.000000 pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/get_global_role_binding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10228 2024-05-09 06:37:09.000000 pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/get_multi_cluster_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6599 2024-05-09 06:37:09.000000 pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/get_namespace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8092 2024-05-09 06:37:09.000000 pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/get_node_driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9339 2024-05-09 06:37:09.000000 pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/get_node_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11657 2024-05-09 06:37:09.000000 pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/get_node_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10488 2024-05-09 06:37:09.000000 pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/get_notifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5826 2024-05-09 06:37:09.000000 pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/get_pod_security_admission_configuration_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29295 2024-05-09 06:37:09.000000 pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/get_pod_security_policy_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3653 2024-05-09 06:37:09.000000 pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/get_principal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7956 2024-05-09 06:37:09.000000 pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/get_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8053 2024-05-09 06:37:09.000000 pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/get_project_alert_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10768 2024-05-09 06:37:09.000000 pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/get_project_alert_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8388 2024-05-09 06:37:09.000000 pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/get_project_role_template_binding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7583 2024-05-09 06:37:09.000000 pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/get_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9189 2024-05-09 06:37:09.000000 pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/get_role_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7362 2024-05-09 06:37:09.000000 pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/get_secret.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7340 2024-05-09 06:37:09.000000 pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/get_secret_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3198 2024-05-09 06:37:09.000000 pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/get_setting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8732 2024-05-09 06:37:09.000000 pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/get_storage_class_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6246 2024-05-09 06:37:09.000000 pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/get_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23658 2024-05-09 06:37:09.000000 pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/global_dns.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22371 2024-05-09 06:37:09.000000 pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/global_dns_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21535 2024-05-09 06:37:09.000000 pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/global_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19056 2024-05-09 06:37:09.000000 pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/global_role_binding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47117 2024-05-09 06:37:09.000000 pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/machine_config_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41596 2024-05-09 06:37:09.000000 pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/multi_cluster_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27977 2024-05-09 06:37:09.000000 pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26635 2024-05-09 06:37:09.000000 pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/node_driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31706 2024-05-09 06:37:09.000000 pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/node_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)    83435 2024-05-09 06:37:09.000000 pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/node_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34476 2024-05-09 06:37:09.000000 pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/notifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1667240 2024-05-09 06:37:09.000000 pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18319 2024-05-09 06:37:09.000000 pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/pod_security_admission_configuration_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    69311 2024-05-09 06:37:09.000000 pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/pod_security_policy_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37721 2024-05-09 06:37:09.000000 pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24984 2024-05-09 06:37:09.000000 pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/project_alert_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37740 2024-05-09 06:37:09.000000 pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/project_alert_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25638 2024-05-09 06:37:09.000000 pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/project_role_template_binding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14405 2024-05-09 06:37:09.000000 pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-09 06:37:09.000000 pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 06:37:09.000000 pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    21460 2024-05-09 06:37:09.000000 pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31723 2024-05-09 06:37:09.000000 pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/role_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21070 2024-05-09 06:37:09.000000 pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/secret.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23036 2024-05-09 06:37:09.000000 pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/secret_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12440 2024-05-09 06:37:09.000000 pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/setting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28123 2024-05-09 06:37:09.000000 pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/storage_class_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23952 2024-05-09 06:37:09.000000 pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/token.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17201 2024-05-09 06:37:09.000000 pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:37:15.421433 pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3763 2024-05-09 06:37:15.000000 pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3753 2024-05-09 06:37:15.000000 pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 06:37:15.000000 pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-09 06:37:15.000000 pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-09 06:37:15.000000 pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-09 06:37:09.000000 pulumi_rancher2-6.2.0a1715235918/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 06:37:15.421433 pulumi_rancher2-6.2.0a1715235918/setup.cfg
```

### Comparing `pulumi_rancher2-6.2.0a1715229630/PKG-INFO` & `pulumi_rancher2-6.2.0a1715235918/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_rancher2
-Version: 6.2.0a1715229630
+Version: 6.2.0a1715235918
 Summary: A Pulumi package for creating and managing rancher2 resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-rancher2
 Keywords: pulumi,rancher2
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_rancher2-6.2.0a1715229630/README.md` & `pulumi_rancher2-6.2.0a1715235918/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/__init__.py` & `pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/_inputs.py` & `pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/_utilities.py` & `pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/app.py` & `pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/app.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/app_v2.py` & `pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/app_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/auth_config_active_directory.py` & `pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/auth_config_active_directory.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/auth_config_adfs.py` & `pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/auth_config_adfs.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/auth_config_azure_ad.py` & `pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/auth_config_azure_ad.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/auth_config_free_ipa.py` & `pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/auth_config_free_ipa.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/auth_config_github.py` & `pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/auth_config_github.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/auth_config_keycloak.py` & `pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/auth_config_keycloak.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/auth_config_okta.py` & `pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/auth_config_okta.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/auth_config_open_ldap.py` & `pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/auth_config_open_ldap.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/auth_config_ping.py` & `pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/auth_config_ping.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/bootstrap.py` & `pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/bootstrap.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/catalog.py` & `pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/catalog.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/catalog_v2.py` & `pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/catalog_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/certificate.py` & `pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/cloud_credential.py` & `pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/cloud_credential.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/cluster.py` & `pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/cluster_alert_group.py` & `pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/cluster_alert_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/cluster_alert_rule.py` & `pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/cluster_alert_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/cluster_driver.py` & `pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/cluster_driver.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/cluster_role_template_binding.py` & `pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/cluster_role_template_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/cluster_sync.py` & `pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/cluster_sync.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/cluster_template.py` & `pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/cluster_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/cluster_v2.py` & `pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/cluster_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/config/__init__.pyi` & `pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/config/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/config/vars.py` & `pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/config_map_v2.py` & `pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/config_map_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/custom_user_token.py` & `pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/custom_user_token.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/etcd_backup.py` & `pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/etcd_backup.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/feature.py` & `pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/feature.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/get_app.py` & `pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/get_app.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/get_catalog.py` & `pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/get_catalog.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/get_catalog_v2.py` & `pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/get_catalog_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/get_certificate.py` & `pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/get_certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/get_cloud_credential.py` & `pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/get_cloud_credential.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/get_cluster.py` & `pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/get_cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/get_cluster_alert_group.py` & `pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/get_cluster_alert_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/get_cluster_alert_rule.py` & `pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/get_cluster_alert_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/get_cluster_driver.py` & `pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/get_cluster_driver.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/get_cluster_role_template_binding.py` & `pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/get_cluster_role_template_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/get_cluster_template.py` & `pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/get_cluster_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/get_cluster_v2.py` & `pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/get_cluster_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/get_config_map_v2.py` & `pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/get_config_map_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/get_etcd_backup.py` & `pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/get_etcd_backup.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/get_global_dns_provider.py` & `pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/get_global_dns_provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/get_global_role.py` & `pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/get_global_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/get_global_role_binding.py` & `pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/get_global_role_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/get_multi_cluster_app.py` & `pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/get_multi_cluster_app.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/get_namespace.py` & `pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/get_namespace.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/get_node_driver.py` & `pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/get_node_driver.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/get_node_pool.py` & `pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/get_node_pool.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/get_node_template.py` & `pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/get_node_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/get_notifier.py` & `pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/get_notifier.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/get_pod_security_admission_configuration_template.py` & `pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/get_pod_security_admission_configuration_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/get_pod_security_policy_template.py` & `pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/get_pod_security_policy_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/get_principal.py` & `pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/get_principal.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/get_project.py` & `pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/get_project.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/get_project_alert_group.py` & `pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/get_project_alert_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/get_project_alert_rule.py` & `pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/get_project_alert_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/get_project_role_template_binding.py` & `pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/get_project_role_template_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/get_registry.py` & `pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/get_registry.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/get_role_template.py` & `pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/get_role_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/get_secret.py` & `pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/get_secret.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/get_secret_v2.py` & `pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/get_secret_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/get_setting.py` & `pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/get_setting.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/get_storage_class_v2.py` & `pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/get_storage_class_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/get_user.py` & `pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/get_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/global_dns.py` & `pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/global_dns.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/global_dns_provider.py` & `pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/global_dns_provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/global_role.py` & `pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/global_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/global_role_binding.py` & `pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/global_role_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/machine_config_v2.py` & `pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/machine_config_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/multi_cluster_app.py` & `pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/multi_cluster_app.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/namespace.py` & `pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/namespace.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/node_driver.py` & `pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/node_driver.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/node_pool.py` & `pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/node_pool.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/node_template.py` & `pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/node_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/notifier.py` & `pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/notifier.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/outputs.py` & `pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/pod_security_admission_configuration_template.py` & `pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/pod_security_admission_configuration_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/pod_security_policy_template.py` & `pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/pod_security_policy_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/project.py` & `pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/project.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/project_alert_group.py` & `pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/project_alert_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/project_alert_rule.py` & `pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/project_alert_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/project_role_template_binding.py` & `pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/project_role_template_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/provider.py` & `pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/registry.py` & `pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/registry.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/role_template.py` & `pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/role_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/secret.py` & `pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/secret.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/secret_v2.py` & `pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/secret_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/setting.py` & `pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/setting.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/storage_class_v2.py` & `pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/storage_class_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/token.py` & `pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/token.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2/user.py` & `pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2/user.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2.egg-info/PKG-INFO` & `pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_rancher2
-Version: 6.2.0a1715229630
+Version: 6.2.0a1715235918
 Summary: A Pulumi package for creating and managing rancher2 resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-rancher2
 Keywords: pulumi,rancher2
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_rancher2-6.2.0a1715229630/pulumi_rancher2.egg-info/SOURCES.txt` & `pulumi_rancher2-6.2.0a1715235918/pulumi_rancher2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1715229630/pyproject.toml` & `pulumi_rancher2-6.2.0a1715235918/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_rancher2"
   description = "A Pulumi package for creating and managing rancher2 resources."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "rancher2"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "6.2.0a1715229630"
+  version = "6.2.0a1715235918"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://pulumi.io"
     Repository = "https://github.com/pulumi/pulumi-rancher2"
 
 [build-system]
```

