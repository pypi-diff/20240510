# Comparing `tmp/seeq-65.0.1.tar.gz` & `tmp/seeq-65.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seeq-65.0.1.tar", last modified: Wed May  1 22:02:36 2024, max compression
+gzip compressed data, was "seeq-65.0.2.tar", last modified: Thu May  9 22:12:11 2024, max compression
```

## Comparing `seeq-65.0.1.tar` & `seeq-65.0.2.tar`

### file list

```diff
@@ -1,456 +1,456 @@
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-01 22:02:36.345995 seeq-65.0.1/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    33136 2024-05-01 20:37:56.000000 seeq-65.0.1/LICENSE
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       18 2024-05-01 20:37:56.000000 seeq-65.0.1/MANIFEST.in
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3869 2024-05-01 22:02:36.345995 seeq-65.0.1/PKG-INFO
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3317 2024-05-01 20:37:56.000000 seeq-65.0.1/README.md
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-01 20:37:57.000000 seeq-65.0.1/pyproject.toml
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-01 22:02:36.293992 seeq-65.0.1/seeq/
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-01 22:02:36.293992 seeq-65.0.1/seeq/sdk/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    27471 2024-05-01 20:46:29.000000 seeq-65.0.1/seeq/sdk/__init__.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-01 22:02:36.301993 seeq-65.0.1/seeq/sdk/api/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2117 2024-05-01 20:46:29.000000 seeq-65.0.1/seeq/sdk/api/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15396 2024-05-01 20:46:28.000000 seeq-65.0.1/seeq/sdk/api/access_keys_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    29293 2024-05-01 20:46:28.000000 seeq-65.0.1/seeq/sdk/api/add_ons_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)   139189 2024-05-01 20:46:28.000000 seeq-65.0.1/seeq/sdk/api/agents_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    54975 2024-05-01 20:46:28.000000 seeq-65.0.1/seeq/sdk/api/annotations_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    24078 2024-05-01 20:46:28.000000 seeq-65.0.1/seeq/sdk/api/assets_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8202 2024-05-01 20:46:28.000000 seeq-65.0.1/seeq/sdk/api/audit_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    21842 2024-05-01 20:46:28.000000 seeq-65.0.1/seeq/sdk/api/auth_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    27275 2024-05-01 20:46:28.000000 seeq-65.0.1/seeq/sdk/api/condition_monitors_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    52130 2024-05-01 20:46:28.000000 seeq-65.0.1/seeq/sdk/api/conditions_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)   126123 2024-05-01 20:46:28.000000 seeq-65.0.1/seeq/sdk/api/content_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    84129 2024-05-01 20:46:28.000000 seeq-65.0.1/seeq/sdk/api/context_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    34507 2024-05-01 20:46:28.000000 seeq-65.0.1/seeq/sdk/api/datafiles_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    50775 2024-05-01 20:46:28.000000 seeq-65.0.1/seeq/sdk/api/datasources_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    25032 2024-05-01 20:46:28.000000 seeq-65.0.1/seeq/sdk/api/display_templates_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    24305 2024-05-01 20:46:28.000000 seeq-65.0.1/seeq/sdk/api/displays_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    30080 2024-05-01 20:46:28.000000 seeq-65.0.1/seeq/sdk/api/export_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    50560 2024-05-01 20:46:28.000000 seeq-65.0.1/seeq/sdk/api/folders_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)   107375 2024-05-01 20:46:28.000000 seeq-65.0.1/seeq/sdk/api/formulas_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5495 2024-05-01 20:46:28.000000 seeq-65.0.1/seeq/sdk/api/graph_ql_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)   195259 2024-05-01 20:46:28.000000 seeq-65.0.1/seeq/sdk/api/items_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    35736 2024-05-01 20:46:28.000000 seeq-65.0.1/seeq/sdk/api/jobs_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    21471 2024-05-01 20:46:28.000000 seeq-65.0.1/seeq/sdk/api/logs_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    24612 2024-05-01 20:46:28.000000 seeq-65.0.1/seeq/sdk/api/metrics_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    32019 2024-05-01 20:46:28.000000 seeq-65.0.1/seeq/sdk/api/monitors_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5962 2024-05-01 20:46:28.000000 seeq-65.0.1/seeq/sdk/api/networks_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    33687 2024-05-01 20:46:28.000000 seeq-65.0.1/seeq/sdk/api/notification_configurations_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10156 2024-05-01 20:46:28.000000 seeq-65.0.1/seeq/sdk/api/notifier_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    21444 2024-05-01 20:46:28.000000 seeq-65.0.1/seeq/sdk/api/plugins_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    35456 2024-05-01 20:46:28.000000 seeq-65.0.1/seeq/sdk/api/projects_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    24605 2024-05-01 20:46:28.000000 seeq-65.0.1/seeq/sdk/api/report_templates_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5758 2024-05-01 20:46:28.000000 seeq-65.0.1/seeq/sdk/api/reports_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    38193 2024-05-01 20:46:28.000000 seeq-65.0.1/seeq/sdk/api/requests_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    28492 2024-05-01 20:46:28.000000 seeq-65.0.1/seeq/sdk/api/scalars_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    17482 2024-05-01 20:46:28.000000 seeq-65.0.1/seeq/sdk/api/scim_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)   110312 2024-05-01 20:46:29.000000 seeq-65.0.1/seeq/sdk/api/signals_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    20586 2024-05-01 20:46:29.000000 seeq-65.0.1/seeq/sdk/api/subscriptions_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)   104888 2024-05-01 20:46:29.000000 seeq-65.0.1/seeq/sdk/api/system_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    51967 2024-05-01 20:46:29.000000 seeq-65.0.1/seeq/sdk/api/table_definitions_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    66306 2024-05-01 20:46:29.000000 seeq-65.0.1/seeq/sdk/api/trees_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8652 2024-05-01 20:46:29.000000 seeq-65.0.1/seeq/sdk/api/unstable_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12944 2024-05-01 20:46:29.000000 seeq-65.0.1/seeq/sdk/api/usage_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    52327 2024-05-01 20:46:29.000000 seeq-65.0.1/seeq/sdk/api/user_groups_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    49735 2024-05-01 20:46:29.000000 seeq-65.0.1/seeq/sdk/api/users_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    94800 2024-05-01 20:46:29.000000 seeq-65.0.1/seeq/sdk/api/workbooks_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    32200 2024-05-01 20:46:29.000000 seeq-65.0.1/seeq/sdk/api_client.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9343 2024-05-01 20:46:29.000000 seeq-65.0.1/seeq/sdk/configuration.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-01 22:02:36.345995 seeq-65.0.1/seeq/sdk/models/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    22725 2024-05-01 20:46:29.000000 seeq-65.0.1/seeq/sdk/models/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4286 2024-05-01 20:46:22.000000 seeq-65.0.1/seeq/sdk/models/access_key_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7328 2024-05-01 20:46:22.000000 seeq-65.0.1/seeq/sdk/models/access_key_output_list_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14440 2024-05-01 20:46:22.000000 seeq-65.0.1/seeq/sdk/models/access_key_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4107 2024-05-01 20:46:22.000000 seeq-65.0.1/seeq/sdk/models/ace_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5730 2024-05-01 20:46:22.000000 seeq-65.0.1/seeq/sdk/models/ace_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6786 2024-05-01 20:46:22.000000 seeq-65.0.1/seeq/sdk/models/acl_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6589 2024-05-01 20:46:22.000000 seeq-65.0.1/seeq/sdk/models/acl_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3601 2024-05-01 20:46:22.000000 seeq-65.0.1/seeq/sdk/models/activity_graph_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7375 2024-05-01 20:46:22.000000 seeq-65.0.1/seeq/sdk/models/activity_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8578 2024-05-01 20:46:22.000000 seeq-65.0.1/seeq/sdk/models/add_on_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7271 2024-05-01 20:46:22.000000 seeq-65.0.1/seeq/sdk/models/add_on_output_list_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15975 2024-05-01 20:46:23.000000 seeq-65.0.1/seeq/sdk/models/add_on_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7513 2024-05-01 20:46:23.000000 seeq-65.0.1/seeq/sdk/models/add_on_preview_output_list_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6530 2024-05-01 20:46:23.000000 seeq-65.0.1/seeq/sdk/models/add_on_preview_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11088 2024-05-01 20:46:23.000000 seeq-65.0.1/seeq/sdk/models/add_on_tool_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    17343 2024-05-01 20:46:23.000000 seeq-65.0.1/seeq/sdk/models/add_on_tool_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4143 2024-05-01 20:46:23.000000 seeq-65.0.1/seeq/sdk/models/administrator_contact_information_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4853 2024-05-01 20:46:23.000000 seeq-65.0.1/seeq/sdk/models/agent_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3128 2024-05-01 20:46:23.000000 seeq-65.0.1/seeq/sdk/models/agent_key_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7460 2024-05-01 20:46:23.000000 seeq-65.0.1/seeq/sdk/models/agent_orchestrator_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13856 2024-05-01 20:46:23.000000 seeq-65.0.1/seeq/sdk/models/agent_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8806 2024-05-01 20:46:23.000000 seeq-65.0.1/seeq/sdk/models/agent_status_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7833 2024-05-01 20:46:23.000000 seeq-65.0.1/seeq/sdk/models/agent_status_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4282 2024-05-01 20:46:23.000000 seeq-65.0.1/seeq/sdk/models/annotation_image_link_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11035 2024-05-01 20:46:23.000000 seeq-65.0.1/seeq/sdk/models/annotation_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4225 2024-05-01 20:46:23.000000 seeq-65.0.1/seeq/sdk/models/annotation_interest_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3750 2024-05-01 20:46:23.000000 seeq-65.0.1/seeq/sdk/models/annotation_interest_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7392 2024-05-01 20:46:23.000000 seeq-65.0.1/seeq/sdk/models/annotation_list_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    34976 2024-05-01 20:46:23.000000 seeq-65.0.1/seeq/sdk/models/annotation_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4433 2024-05-01 20:46:23.000000 seeq-65.0.1/seeq/sdk/models/archive_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4176 2024-05-01 20:46:23.000000 seeq-65.0.1/seeq/sdk/models/asset_batch_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4667 2024-05-01 20:46:23.000000 seeq-65.0.1/seeq/sdk/models/asset_error.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14717 2024-05-01 20:46:23.000000 seeq-65.0.1/seeq/sdk/models/asset_group_asset_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4038 2024-05-01 20:46:23.000000 seeq-65.0.1/seeq/sdk/models/asset_group_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3969 2024-05-01 20:46:23.000000 seeq-65.0.1/seeq/sdk/models/asset_group_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13792 2024-05-01 20:46:23.000000 seeq-65.0.1/seeq/sdk/models/asset_group_root_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6462 2024-05-01 20:46:23.000000 seeq-65.0.1/seeq/sdk/models/asset_group_tree_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11760 2024-05-01 20:46:23.000000 seeq-65.0.1/seeq/sdk/models/asset_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    17564 2024-05-01 20:46:23.000000 seeq-65.0.1/seeq/sdk/models/asset_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8465 2024-05-01 20:46:23.000000 seeq-65.0.1/seeq/sdk/models/asset_selection_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13114 2024-05-01 20:46:23.000000 seeq-65.0.1/seeq/sdk/models/asset_selection_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7086 2024-05-01 20:46:23.000000 seeq-65.0.1/seeq/sdk/models/asset_tree_batch_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11209 2024-05-01 20:46:23.000000 seeq-65.0.1/seeq/sdk/models/asset_tree_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4432 2024-05-01 20:46:23.000000 seeq-65.0.1/seeq/sdk/models/asset_tree_single_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4866 2024-05-01 20:46:23.000000 seeq-65.0.1/seeq/sdk/models/attachment_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8190 2024-05-01 20:46:23.000000 seeq-65.0.1/seeq/sdk/models/audit_output_list_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9644 2024-05-01 20:46:23.000000 seeq-65.0.1/seeq/sdk/models/audit_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7075 2024-05-01 20:46:23.000000 seeq-65.0.1/seeq/sdk/models/auth_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3442 2024-05-01 20:46:23.000000 seeq-65.0.1/seeq/sdk/models/auth_providers_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4444 2024-05-01 20:46:23.000000 seeq-65.0.1/seeq/sdk/models/authoritative_region_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2455 2024-05-01 20:46:23.000000 seeq-65.0.1/seeq/sdk/models/boolean_configuration_field_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9542 2024-05-01 20:46:23.000000 seeq-65.0.1/seeq/sdk/models/cache_block.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4089 2024-05-01 20:46:23.000000 seeq-65.0.1/seeq/sdk/models/cache_info_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    20746 2024-05-01 20:46:23.000000 seeq-65.0.1/seeq/sdk/models/calculated_item_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5332 2024-05-01 20:46:23.000000 seeq-65.0.1/seeq/sdk/models/capsule_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4348 2024-05-01 20:46:23.000000 seeq-65.0.1/seeq/sdk/models/capsule_property_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4161 2024-05-01 20:46:23.000000 seeq-65.0.1/seeq/sdk/models/capsule_property_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7480 2024-05-01 20:46:23.000000 seeq-65.0.1/seeq/sdk/models/capsule_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3259 2024-05-01 20:46:23.000000 seeq-65.0.1/seeq/sdk/models/capsules_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10294 2024-05-01 20:46:23.000000 seeq-65.0.1/seeq/sdk/models/capsules_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4020 2024-05-01 20:46:23.000000 seeq-65.0.1/seeq/sdk/models/capsules_overwrite_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7228 2024-05-01 20:46:23.000000 seeq-65.0.1/seeq/sdk/models/channel_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4181 2024-05-01 20:46:23.000000 seeq-65.0.1/seeq/sdk/models/column_definition_input_list_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8308 2024-05-01 20:46:23.000000 seeq-65.0.1/seeq/sdk/models/column_definition_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3797 2024-05-01 20:46:23.000000 seeq-65.0.1/seeq/sdk/models/column_definition_order_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7934 2024-05-01 20:46:23.000000 seeq-65.0.1/seeq/sdk/models/column_definition_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4700 2024-05-01 20:46:23.000000 seeq-65.0.1/seeq/sdk/models/column_rule_ancestor_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10419 2024-05-01 20:46:23.000000 seeq-65.0.1/seeq/sdk/models/column_rule_asset_creator_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3561 2024-05-01 20:46:23.000000 seeq-65.0.1/seeq/sdk/models/column_rule_concat_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3577 2024-05-01 20:46:23.000000 seeq-65.0.1/seeq/sdk/models/column_rule_constant_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8932 2024-05-01 20:46:23.000000 seeq-65.0.1/seeq/sdk/models/column_rule_descendant_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3634 2024-05-01 20:46:23.000000 seeq-65.0.1/seeq/sdk/models/column_rule_event_property_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12681 2024-05-01 20:46:23.000000 seeq-65.0.1/seeq/sdk/models/column_rule_formula_creator_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10334 2024-05-01 20:46:23.000000 seeq-65.0.1/seeq/sdk/models/column_rule_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4507 2024-05-01 20:46:23.000000 seeq-65.0.1/seeq/sdk/models/column_rule_item_property_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4782 2024-05-01 20:46:23.000000 seeq-65.0.1/seeq/sdk/models/column_rule_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5241 2024-05-01 20:46:23.000000 seeq-65.0.1/seeq/sdk/models/column_rule_path_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4525 2024-05-01 20:46:23.000000 seeq-65.0.1/seeq/sdk/models/column_rule_tree_path_creator_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3409 2024-05-01 20:46:23.000000 seeq-65.0.1/seeq/sdk/models/condition_batch_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    20503 2024-05-01 20:46:23.000000 seeq-65.0.1/seeq/sdk/models/condition_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12557 2024-05-01 20:46:23.000000 seeq-65.0.1/seeq/sdk/models/condition_monitor_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11211 2024-05-01 20:46:23.000000 seeq-65.0.1/seeq/sdk/models/condition_monitor_notification_configuration_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    22784 2024-05-01 20:46:23.000000 seeq-65.0.1/seeq/sdk/models/condition_monitor_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9233 2024-05-01 20:46:23.000000 seeq-65.0.1/seeq/sdk/models/condition_notification_output_list_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6660 2024-05-01 20:46:23.000000 seeq-65.0.1/seeq/sdk/models/condition_notification_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    24440 2024-05-01 20:46:23.000000 seeq-65.0.1/seeq/sdk/models/condition_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    23781 2024-05-01 20:46:23.000000 seeq-65.0.1/seeq/sdk/models/condition_update_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7675 2024-05-01 20:46:23.000000 seeq-65.0.1/seeq/sdk/models/configuration_field_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4064 2024-05-01 20:46:23.000000 seeq-65.0.1/seeq/sdk/models/configuration_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4276 2024-05-01 20:46:23.000000 seeq-65.0.1/seeq/sdk/models/configuration_option_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3748 2024-05-01 20:46:24.000000 seeq-65.0.1/seeq/sdk/models/configuration_option_output_simple_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12329 2024-05-01 20:46:24.000000 seeq-65.0.1/seeq/sdk/models/configuration_option_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8813 2024-05-01 20:46:24.000000 seeq-65.0.1/seeq/sdk/models/configuration_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4959 2024-05-01 20:46:24.000000 seeq-65.0.1/seeq/sdk/models/configured_directives_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8527 2024-05-01 20:46:24.000000 seeq-65.0.1/seeq/sdk/models/connection_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    27327 2024-05-01 20:46:24.000000 seeq-65.0.1/seeq/sdk/models/connection_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    18799 2024-05-01 20:46:24.000000 seeq-65.0.1/seeq/sdk/models/connection_status_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    16922 2024-05-01 20:46:24.000000 seeq-65.0.1/seeq/sdk/models/connection_status_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3253 2024-05-01 20:46:24.000000 seeq-65.0.1/seeq/sdk/models/connections_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4941 2024-05-01 20:46:24.000000 seeq-65.0.1/seeq/sdk/models/connector_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14854 2024-05-01 20:46:24.000000 seeq-65.0.1/seeq/sdk/models/connector_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3273 2024-05-01 20:46:24.000000 seeq-65.0.1/seeq/sdk/models/connectors_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15681 2024-05-01 20:46:24.000000 seeq-65.0.1/seeq/sdk/models/content_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    22574 2024-05-01 20:46:24.000000 seeq-65.0.1/seeq/sdk/models/content_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5298 2024-05-01 20:46:24.000000 seeq-65.0.1/seeq/sdk/models/content_with_metadata_list_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    28438 2024-05-01 20:46:24.000000 seeq-65.0.1/seeq/sdk/models/content_with_metadata_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5888 2024-05-01 20:46:24.000000 seeq-65.0.1/seeq/sdk/models/context_comment_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11939 2024-05-01 20:46:24.000000 seeq-65.0.1/seeq/sdk/models/context_comment_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5849 2024-05-01 20:46:24.000000 seeq-65.0.1/seeq/sdk/models/context_label_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12837 2024-05-01 20:46:24.000000 seeq-65.0.1/seeq/sdk/models/context_label_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6788 2024-05-01 20:46:24.000000 seeq-65.0.1/seeq/sdk/models/context_opaque_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12675 2024-05-01 20:46:24.000000 seeq-65.0.1/seeq/sdk/models/context_opaque_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3446 2024-05-01 20:46:24.000000 seeq-65.0.1/seeq/sdk/models/csv_datafile_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    50145 2024-05-01 20:46:24.000000 seeq-65.0.1/seeq/sdk/models/datafile_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    53738 2024-05-01 20:46:24.000000 seeq-65.0.1/seeq/sdk/models/datafile_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3115 2024-05-01 20:46:24.000000 seeq-65.0.1/seeq/sdk/models/datafiles_csv_body.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9607 2024-05-01 20:46:24.000000 seeq-65.0.1/seeq/sdk/models/datasource_clean_up_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4283 2024-05-01 20:46:24.000000 seeq-65.0.1/seeq/sdk/models/datasource_clean_up_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13268 2024-05-01 20:46:24.000000 seeq-65.0.1/seeq/sdk/models/datasource_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7504 2024-05-01 20:46:24.000000 seeq-65.0.1/seeq/sdk/models/datasource_output_list_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    20088 2024-05-01 20:46:24.000000 seeq-65.0.1/seeq/sdk/models/datasource_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8806 2024-05-01 20:46:24.000000 seeq-65.0.1/seeq/sdk/models/datasource_preview_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15846 2024-05-01 20:46:24.000000 seeq-65.0.1/seeq/sdk/models/datasource_statistics_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8689 2024-05-01 20:46:24.000000 seeq-65.0.1/seeq/sdk/models/datasource_status_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9118 2024-05-01 20:46:24.000000 seeq-65.0.1/seeq/sdk/models/datasource_status_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    28984 2024-05-01 20:46:24.000000 seeq-65.0.1/seeq/sdk/models/datasource_summary_status_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11225 2024-05-01 20:46:24.000000 seeq-65.0.1/seeq/sdk/models/datasources_status_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9723 2024-05-01 20:46:24.000000 seeq-65.0.1/seeq/sdk/models/date_range_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    16890 2024-05-01 20:46:24.000000 seeq-65.0.1/seeq/sdk/models/date_range_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4111 2024-05-01 20:46:24.000000 seeq-65.0.1/seeq/sdk/models/debug_cache_block_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4868 2024-05-01 20:46:24.000000 seeq-65.0.1/seeq/sdk/models/detailed_meter_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5727 2024-05-01 20:46:24.000000 seeq-65.0.1/seeq/sdk/models/detailed_timer_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5047 2024-05-01 20:46:24.000000 seeq-65.0.1/seeq/sdk/models/directive_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5244 2024-05-01 20:46:24.000000 seeq-65.0.1/seeq/sdk/models/display_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7354 2024-05-01 20:46:24.000000 seeq-65.0.1/seeq/sdk/models/display_output_list_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14727 2024-05-01 20:46:24.000000 seeq-65.0.1/seeq/sdk/models/display_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9431 2024-05-01 20:46:24.000000 seeq-65.0.1/seeq/sdk/models/display_template_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7791 2024-05-01 20:46:24.000000 seeq-65.0.1/seeq/sdk/models/display_template_output_list_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15926 2024-05-01 20:46:24.000000 seeq-65.0.1/seeq/sdk/models/display_template_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4899 2024-05-01 20:46:24.000000 seeq-65.0.1/seeq/sdk/models/document_backup_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4138 2024-05-01 20:46:24.000000 seeq-65.0.1/seeq/sdk/models/double_configuration_field_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5405 2024-05-01 20:46:24.000000 seeq-65.0.1/seeq/sdk/models/email_notification_recipient_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6366 2024-05-01 20:46:24.000000 seeq-65.0.1/seeq/sdk/models/emailer_configuration_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5314 2024-05-01 20:46:24.000000 seeq-65.0.1/seeq/sdk/models/export_item_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    22645 2024-05-01 20:46:24.000000 seeq-65.0.1/seeq/sdk/models/export_items_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    18512 2024-05-01 20:46:24.000000 seeq-65.0.1/seeq/sdk/models/export_items_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7286 2024-05-01 20:46:24.000000 seeq-65.0.1/seeq/sdk/models/export_preview_list_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10723 2024-05-01 20:46:24.000000 seeq-65.0.1/seeq/sdk/models/export_preview_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5909 2024-05-01 20:46:24.000000 seeq-65.0.1/seeq/sdk/models/fixed_list_search_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6490 2024-05-01 20:46:24.000000 seeq-65.0.1/seeq/sdk/models/folded_stack_node_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7686 2024-05-01 20:46:24.000000 seeq-65.0.1/seeq/sdk/models/folder_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5698 2024-05-01 20:46:24.000000 seeq-65.0.1/seeq/sdk/models/folder_navigation_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15863 2024-05-01 20:46:24.000000 seeq-65.0.1/seeq/sdk/models/folder_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4035 2024-05-01 20:46:24.000000 seeq-65.0.1/seeq/sdk/models/formula_compile_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6875 2024-05-01 20:46:24.000000 seeq-65.0.1/seeq/sdk/models/formula_compile_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8113 2024-05-01 20:46:24.000000 seeq-65.0.1/seeq/sdk/models/formula_compiler_error_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4330 2024-05-01 20:46:24.000000 seeq-65.0.1/seeq/sdk/models/formula_dependency_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4006 2024-05-01 20:46:24.000000 seeq-65.0.1/seeq/sdk/models/formula_doc_example_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3464 2024-05-01 20:46:24.000000 seeq-65.0.1/seeq/sdk/models/formula_doc_example_list_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7389 2024-05-01 20:46:24.000000 seeq-65.0.1/seeq/sdk/models/formula_doc_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3415 2024-05-01 20:46:24.000000 seeq-65.0.1/seeq/sdk/models/formula_doc_keyword_list_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    21607 2024-05-01 20:46:24.000000 seeq-65.0.1/seeq/sdk/models/formula_doc_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3228 2024-05-01 20:46:24.000000 seeq-65.0.1/seeq/sdk/models/formula_doc_summaries_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8265 2024-05-01 20:46:24.000000 seeq-65.0.1/seeq/sdk/models/formula_doc_summary_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8265 2024-05-01 20:46:24.000000 seeq-65.0.1/seeq/sdk/models/formula_error_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3952 2024-05-01 20:46:24.000000 seeq-65.0.1/seeq/sdk/models/formula_example_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    18896 2024-05-01 20:46:24.000000 seeq-65.0.1/seeq/sdk/models/formula_item_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    20492 2024-05-01 20:46:24.000000 seeq-65.0.1/seeq/sdk/models/formula_item_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3933 2024-05-01 20:46:24.000000 seeq-65.0.1/seeq/sdk/models/formula_log_entry.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3718 2024-05-01 20:46:24.000000 seeq-65.0.1/seeq/sdk/models/formula_log_entry_details.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4453 2024-05-01 20:46:24.000000 seeq-65.0.1/seeq/sdk/models/formula_log_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6771 2024-05-01 20:46:24.000000 seeq-65.0.1/seeq/sdk/models/formula_package_import_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6060 2024-05-01 20:46:24.000000 seeq-65.0.1/seeq/sdk/models/formula_package_import_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9360 2024-05-01 20:46:24.000000 seeq-65.0.1/seeq/sdk/models/formula_package_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    17867 2024-05-01 20:46:24.000000 seeq-65.0.1/seeq/sdk/models/formula_package_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6189 2024-05-01 20:46:24.000000 seeq-65.0.1/seeq/sdk/models/formula_parameter_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5572 2024-05-01 20:46:24.000000 seeq-65.0.1/seeq/sdk/models/formula_parameter_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12942 2024-05-01 20:46:24.000000 seeq-65.0.1/seeq/sdk/models/formula_run_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12280 2024-05-01 20:46:24.000000 seeq-65.0.1/seeq/sdk/models/formula_run_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4077 2024-05-01 20:46:24.000000 seeq-65.0.1/seeq/sdk/models/formula_token.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4064 2024-05-01 20:46:24.000000 seeq-65.0.1/seeq/sdk/models/formula_update_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4108 2024-05-01 20:46:25.000000 seeq-65.0.1/seeq/sdk/models/formula_upgrade_change_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4932 2024-05-01 20:46:25.000000 seeq-65.0.1/seeq/sdk/models/formula_upgrade_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13617 2024-05-01 20:46:25.000000 seeq-65.0.1/seeq/sdk/models/function_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4594 2024-05-01 20:46:25.000000 seeq-65.0.1/seeq/sdk/models/function_parameter_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6327 2024-05-01 20:46:25.000000 seeq-65.0.1/seeq/sdk/models/function_variant_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4834 2024-05-01 20:46:25.000000 seeq-65.0.1/seeq/sdk/models/gauge_datum_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4157 2024-05-01 20:46:25.000000 seeq-65.0.1/seeq/sdk/models/generic_table_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3286 2024-05-01 20:46:25.000000 seeq-65.0.1/seeq/sdk/models/get_add_on_tools_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7344 2024-05-01 20:46:25.000000 seeq-65.0.1/seeq/sdk/models/get_channels_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9186 2024-05-01 20:46:25.000000 seeq-65.0.1/seeq/sdk/models/get_condition_monitor_items_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7561 2024-05-01 20:46:25.000000 seeq-65.0.1/seeq/sdk/models/get_content_items_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7469 2024-05-01 20:46:25.000000 seeq-65.0.1/seeq/sdk/models/get_date_ranges_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7136 2024-05-01 20:46:25.000000 seeq-65.0.1/seeq/sdk/models/get_jobs_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7319 2024-05-01 20:46:25.000000 seeq-65.0.1/seeq/sdk/models/get_metrics_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7348 2024-05-01 20:46:25.000000 seeq-65.0.1/seeq/sdk/models/get_projects_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4191 2024-05-01 20:46:25.000000 seeq-65.0.1/seeq/sdk/models/get_request_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3122 2024-05-01 20:46:25.000000 seeq-65.0.1/seeq/sdk/models/get_requests_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6221 2024-05-01 20:46:25.000000 seeq-65.0.1/seeq/sdk/models/get_sample_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11225 2024-05-01 20:46:25.000000 seeq-65.0.1/seeq/sdk/models/get_samples_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7292 2024-05-01 20:46:25.000000 seeq-65.0.1/seeq/sdk/models/get_signals_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3806 2024-05-01 20:46:25.000000 seeq-65.0.1/seeq/sdk/models/graph_ql_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3765 2024-05-01 20:46:25.000000 seeq-65.0.1/seeq/sdk/models/graph_ql_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3087 2024-05-01 20:46:25.000000 seeq-65.0.1/seeq/sdk/models/id_images_body.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3541 2024-05-01 20:46:25.000000 seeq-65.0.1/seeq/sdk/models/identity_mapping_list_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6253 2024-05-01 20:46:25.000000 seeq-65.0.1/seeq/sdk/models/identity_mapping_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8348 2024-05-01 20:46:25.000000 seeq-65.0.1/seeq/sdk/models/identity_preview_list_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12927 2024-05-01 20:46:25.000000 seeq-65.0.1/seeq/sdk/models/identity_preview_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4212 2024-05-01 20:46:25.000000 seeq-65.0.1/seeq/sdk/models/indexing_parameters_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4947 2024-05-01 20:46:25.000000 seeq-65.0.1/seeq/sdk/models/installer_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4136 2024-05-01 20:46:25.000000 seeq-65.0.1/seeq/sdk/models/interval_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2997 2024-05-01 20:46:25.000000 seeq-65.0.1/seeq/sdk/models/invalid_swap_out_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5360 2024-05-01 20:46:25.000000 seeq-65.0.1/seeq/sdk/models/item_batch_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11549 2024-05-01 20:46:25.000000 seeq-65.0.1/seeq/sdk/models/item_dependency_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11046 2024-05-01 20:46:25.000000 seeq-65.0.1/seeq/sdk/models/item_finder_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7639 2024-05-01 20:46:25.000000 seeq-65.0.1/seeq/sdk/models/item_finder_output_list_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    16822 2024-05-01 20:46:25.000000 seeq-65.0.1/seeq/sdk/models/item_finder_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5509 2024-05-01 20:46:25.000000 seeq-65.0.1/seeq/sdk/models/item_finder_searches_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4132 2024-05-01 20:46:25.000000 seeq-65.0.1/seeq/sdk/models/item_finder_searches_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3168 2024-05-01 20:46:25.000000 seeq-65.0.1/seeq/sdk/models/item_id_list_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14649 2024-05-01 20:46:25.000000 seeq-65.0.1/seeq/sdk/models/item_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11275 2024-05-01 20:46:25.000000 seeq-65.0.1/seeq/sdk/models/item_parameter_of_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8178 2024-05-01 20:46:25.000000 seeq-65.0.1/seeq/sdk/models/item_preview_list_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6934 2024-05-01 20:46:25.000000 seeq-65.0.1/seeq/sdk/models/item_preview_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9485 2024-05-01 20:46:25.000000 seeq-65.0.1/seeq/sdk/models/item_preview_with_assets_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4196 2024-05-01 20:46:25.000000 seeq-65.0.1/seeq/sdk/models/item_search_preview_list_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8661 2024-05-01 20:46:25.000000 seeq-65.0.1/seeq/sdk/models/item_search_preview_paginated_list_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    16178 2024-05-01 20:46:25.000000 seeq-65.0.1/seeq/sdk/models/item_search_preview_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4708 2024-05-01 20:46:25.000000 seeq-65.0.1/seeq/sdk/models/item_swap_result_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6537 2024-05-01 20:46:25.000000 seeq-65.0.1/seeq/sdk/models/item_update_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4220 2024-05-01 20:46:25.000000 seeq-65.0.1/seeq/sdk/models/item_user_attributes_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5888 2024-05-01 20:46:25.000000 seeq-65.0.1/seeq/sdk/models/item_user_attributes_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5144 2024-05-01 20:46:25.000000 seeq-65.0.1/seeq/sdk/models/item_with_swap_pairs_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4395 2024-05-01 20:46:25.000000 seeq-65.0.1/seeq/sdk/models/jira_attachment.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6025 2024-05-01 20:46:25.000000 seeq-65.0.1/seeq/sdk/models/jira_attachment_media_type.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6230 2024-05-01 20:46:25.000000 seeq-65.0.1/seeq/sdk/models/job_accepted_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14001 2024-05-01 20:46:25.000000 seeq-65.0.1/seeq/sdk/models/job_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4845 2024-05-01 20:46:25.000000 seeq-65.0.1/seeq/sdk/models/json_backup_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4626 2024-05-01 20:46:25.000000 seeq-65.0.1/seeq/sdk/models/label_category_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3222 2024-05-01 20:46:25.000000 seeq-65.0.1/seeq/sdk/models/label_category_output_list_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5274 2024-05-01 20:46:25.000000 seeq-65.0.1/seeq/sdk/models/label_category_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4773 2024-05-01 20:46:25.000000 seeq-65.0.1/seeq/sdk/models/label_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3062 2024-05-01 20:46:25.000000 seeq-65.0.1/seeq/sdk/models/label_output_list_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5063 2024-05-01 20:46:25.000000 seeq-65.0.1/seeq/sdk/models/label_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4381 2024-05-01 20:46:25.000000 seeq-65.0.1/seeq/sdk/models/license_importer_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13507 2024-05-01 20:46:25.000000 seeq-65.0.1/seeq/sdk/models/license_status_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6191 2024-05-01 20:46:25.000000 seeq-65.0.1/seeq/sdk/models/licensed_feature_status_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4668 2024-05-01 20:46:25.000000 seeq-65.0.1/seeq/sdk/models/log_message.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4136 2024-05-01 20:46:25.000000 seeq-65.0.1/seeq/sdk/models/long_configuration_field_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4693 2024-05-01 20:46:25.000000 seeq-65.0.1/seeq/sdk/models/meter_datum_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3177 2024-05-01 20:46:25.000000 seeq-65.0.1/seeq/sdk/models/migrate_editor_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4779 2024-05-01 20:46:25.000000 seeq-65.0.1/seeq/sdk/models/monitor_definition_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3420 2024-05-01 20:46:25.000000 seeq-65.0.1/seeq/sdk/models/monitor_definitions_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4520 2024-05-01 20:46:25.000000 seeq-65.0.1/seeq/sdk/models/monitor_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3189 2024-05-01 20:46:25.000000 seeq-65.0.1/seeq/sdk/models/monitor_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13074 2024-05-01 20:46:26.000000 seeq-65.0.1/seeq/sdk/models/monitor_values.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3164 2024-05-01 20:46:26.000000 seeq-65.0.1/seeq/sdk/models/monitors_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8926 2024-05-01 20:46:26.000000 seeq-65.0.1/seeq/sdk/models/notifiable_report_output_list_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8081 2024-05-01 20:46:26.000000 seeq-65.0.1/seeq/sdk/models/notifiable_report_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12021 2024-05-01 20:46:26.000000 seeq-65.0.1/seeq/sdk/models/notification_configuration_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6065 2024-05-01 20:46:26.000000 seeq-65.0.1/seeq/sdk/models/optional_report_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6206 2024-05-01 20:46:26.000000 seeq-65.0.1/seeq/sdk/models/parameter_doc_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4124 2024-05-01 20:46:26.000000 seeq-65.0.1/seeq/sdk/models/permissions_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8236 2024-05-01 20:46:26.000000 seeq-65.0.1/seeq/sdk/models/plugin_output_list_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    16602 2024-05-01 20:46:26.000000 seeq-65.0.1/seeq/sdk/models/plugin_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3084 2024-05-01 20:46:26.000000 seeq-65.0.1/seeq/sdk/models/plugins_body.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6354 2024-05-01 20:46:26.000000 seeq-65.0.1/seeq/sdk/models/pre_provision_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3980 2024-05-01 20:46:26.000000 seeq-65.0.1/seeq/sdk/models/pre_provision_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4929 2024-05-01 20:46:26.000000 seeq-65.0.1/seeq/sdk/models/priority_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4011 2024-05-01 20:46:26.000000 seeq-65.0.1/seeq/sdk/models/progress_information_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10158 2024-05-01 20:46:26.000000 seeq-65.0.1/seeq/sdk/models/project_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    20788 2024-05-01 20:46:26.000000 seeq-65.0.1/seeq/sdk/models/project_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5624 2024-05-01 20:46:26.000000 seeq-65.0.1/seeq/sdk/models/property_filter_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4255 2024-05-01 20:46:26.000000 seeq-65.0.1/seeq/sdk/models/property_href_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4582 2024-05-01 20:46:26.000000 seeq-65.0.1/seeq/sdk/models/property_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6492 2024-05-01 20:46:26.000000 seeq-65.0.1/seeq/sdk/models/property_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8130 2024-05-01 20:46:26.000000 seeq-65.0.1/seeq/sdk/models/property_search_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5041 2024-05-01 20:46:26.000000 seeq-65.0.1/seeq/sdk/models/provision_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13320 2024-05-01 20:46:26.000000 seeq-65.0.1/seeq/sdk/models/put_asset_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    19360 2024-05-01 20:46:26.000000 seeq-65.0.1/seeq/sdk/models/put_scalar_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7198 2024-05-01 20:46:26.000000 seeq-65.0.1/seeq/sdk/models/put_scalars_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3288 2024-05-01 20:46:26.000000 seeq-65.0.1/seeq/sdk/models/put_signals_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3413 2024-05-01 20:46:26.000000 seeq-65.0.1/seeq/sdk/models/put_user_groups_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3276 2024-05-01 20:46:26.000000 seeq-65.0.1/seeq/sdk/models/referenced_items_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11239 2024-05-01 20:46:26.000000 seeq-65.0.1/seeq/sdk/models/regression_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4575 2024-05-01 20:46:26.000000 seeq-65.0.1/seeq/sdk/models/remote_agent_directives_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    16599 2024-05-01 20:46:26.000000 seeq-65.0.1/seeq/sdk/models/remote_agent_status_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    16708 2024-05-01 20:46:26.000000 seeq-65.0.1/seeq/sdk/models/remote_agent_status_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5135 2024-05-01 20:46:26.000000 seeq-65.0.1/seeq/sdk/models/report_input_item_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4810 2024-05-01 20:46:26.000000 seeq-65.0.1/seeq/sdk/models/report_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8329 2024-05-01 20:46:26.000000 seeq-65.0.1/seeq/sdk/models/report_notification_configuration_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6225 2024-05-01 20:46:26.000000 seeq-65.0.1/seeq/sdk/models/report_template_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15217 2024-05-01 20:46:26.000000 seeq-65.0.1/seeq/sdk/models/report_template_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15198 2024-05-01 20:46:26.000000 seeq-65.0.1/seeq/sdk/models/request_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4385 2024-05-01 20:46:26.000000 seeq-65.0.1/seeq/sdk/models/sample_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4453 2024-05-01 20:46:26.000000 seeq-65.0.1/seeq/sdk/models/sample_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3237 2024-05-01 20:46:26.000000 seeq-65.0.1/seeq/sdk/models/samples_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3501 2024-05-01 20:46:26.000000 seeq-65.0.1/seeq/sdk/models/samples_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3994 2024-05-01 20:46:26.000000 seeq-65.0.1/seeq/sdk/models/samples_overwrite_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11225 2024-05-01 20:46:26.000000 seeq-65.0.1/seeq/sdk/models/scalar_evaluate_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    17724 2024-05-01 20:46:26.000000 seeq-65.0.1/seeq/sdk/models/scalar_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5290 2024-05-01 20:46:26.000000 seeq-65.0.1/seeq/sdk/models/scalar_property_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4748 2024-05-01 20:46:26.000000 seeq-65.0.1/seeq/sdk/models/scalar_value_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4542 2024-05-01 20:46:26.000000 seeq-65.0.1/seeq/sdk/models/scale_across_tree_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8516 2024-05-01 20:46:26.000000 seeq-65.0.1/seeq/sdk/models/schedulable_admin_list_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    16074 2024-05-01 20:46:26.000000 seeq-65.0.1/seeq/sdk/models/schedulable_admin_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4210 2024-05-01 20:46:26.000000 seeq-65.0.1/seeq/sdk/models/schedulable_summary_day_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3331 2024-05-01 20:46:26.000000 seeq-65.0.1/seeq/sdk/models/schedulable_summary_week_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4216 2024-05-01 20:46:26.000000 seeq-65.0.1/seeq/sdk/models/schedule_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4974 2024-05-01 20:46:26.000000 seeq-65.0.1/seeq/sdk/models/schedule_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9394 2024-05-01 20:46:26.000000 seeq-65.0.1/seeq/sdk/models/scheduled_notebook_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4611 2024-05-01 20:46:26.000000 seeq-65.0.1/seeq/sdk/models/scheduled_notebook_list_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    20126 2024-05-01 20:46:26.000000 seeq-65.0.1/seeq/sdk/models/scheduled_notebook_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4186 2024-05-01 20:46:26.000000 seeq-65.0.1/seeq/sdk/models/scim_token_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4325 2024-05-01 20:46:26.000000 seeq-65.0.1/seeq/sdk/models/screenshot_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4142 2024-05-01 20:46:26.000000 seeq-65.0.1/seeq/sdk/models/secret_configuration_field_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5699 2024-05-01 20:46:26.000000 seeq-65.0.1/seeq/sdk/models/see_also_doc_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4926 2024-05-01 20:46:26.000000 seeq-65.0.1/seeq/sdk/models/send_email_attachment_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3804 2024-05-01 20:46:26.000000 seeq-65.0.1/seeq/sdk/models/send_email_contact_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7956 2024-05-01 20:46:26.000000 seeq-65.0.1/seeq/sdk/models/send_email_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5175 2024-05-01 20:46:26.000000 seeq-65.0.1/seeq/sdk/models/sent_email_attachment_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12471 2024-05-01 20:46:26.000000 seeq-65.0.1/seeq/sdk/models/sent_email_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3347 2024-05-01 20:46:26.000000 seeq-65.0.1/seeq/sdk/models/sent_emails_list_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3349 2024-05-01 20:46:26.000000 seeq-65.0.1/seeq/sdk/models/server_build_info_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4641 2024-05-01 20:46:26.000000 seeq-65.0.1/seeq/sdk/models/server_load_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6420 2024-05-01 20:46:26.000000 seeq-65.0.1/seeq/sdk/models/server_spec_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11947 2024-05-01 20:46:26.000000 seeq-65.0.1/seeq/sdk/models/server_status_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    18077 2024-05-01 20:46:26.000000 seeq-65.0.1/seeq/sdk/models/signal_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    27764 2024-05-01 20:46:26.000000 seeq-65.0.1/seeq/sdk/models/signal_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    23062 2024-05-01 20:46:26.000000 seeq-65.0.1/seeq/sdk/models/signal_with_id_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3267 2024-05-01 20:46:26.000000 seeq-65.0.1/seeq/sdk/models/status_message.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3515 2024-05-01 20:46:26.000000 seeq-65.0.1/seeq/sdk/models/status_message_base.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3788 2024-05-01 20:46:26.000000 seeq-65.0.1/seeq/sdk/models/store_secret_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4142 2024-05-01 20:46:26.000000 seeq-65.0.1/seeq/sdk/models/string_configuration_field_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4368 2024-05-01 20:46:26.000000 seeq-65.0.1/seeq/sdk/models/subscription_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4908 2024-05-01 20:46:26.000000 seeq-65.0.1/seeq/sdk/models/subscription_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3389 2024-05-01 20:46:26.000000 seeq-65.0.1/seeq/sdk/models/subscription_update_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10912 2024-05-01 20:46:26.000000 seeq-65.0.1/seeq/sdk/models/support_request_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4180 2024-05-01 20:46:26.000000 seeq-65.0.1/seeq/sdk/models/support_request_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4302 2024-05-01 20:46:26.000000 seeq-65.0.1/seeq/sdk/models/supported_units_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7054 2024-05-01 20:46:26.000000 seeq-65.0.1/seeq/sdk/models/swap_across_assets_search_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4209 2024-05-01 20:46:26.000000 seeq-65.0.1/seeq/sdk/models/swap_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3559 2024-05-01 20:46:26.000000 seeq-65.0.1/seeq/sdk/models/swap_option_list_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5575 2024-05-01 20:46:26.000000 seeq-65.0.1/seeq/sdk/models/swap_option_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3784 2024-05-01 20:46:26.000000 seeq-65.0.1/seeq/sdk/models/swap_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11724 2024-05-01 20:46:26.000000 seeq-65.0.1/seeq/sdk/models/sync_progress.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    18924 2024-05-01 20:46:26.000000 seeq-65.0.1/seeq/sdk/models/sync_progress_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3122 2024-05-01 20:46:26.000000 seeq-65.0.1/seeq/sdk/models/system_license_body.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4800 2024-05-01 20:46:26.000000 seeq-65.0.1/seeq/sdk/models/table_column_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10804 2024-05-01 20:46:27.000000 seeq-65.0.1/seeq/sdk/models/table_definition_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7909 2024-05-01 20:46:27.000000 seeq-65.0.1/seeq/sdk/models/table_definition_output_list_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    16936 2024-05-01 20:46:27.000000 seeq-65.0.1/seeq/sdk/models/table_definition_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5426 2024-05-01 20:46:27.000000 seeq-65.0.1/seeq/sdk/models/table_definition_update_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    19125 2024-05-01 20:46:27.000000 seeq-65.0.1/seeq/sdk/models/threshold_metric_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    28187 2024-05-01 20:46:27.000000 seeq-65.0.1/seeq/sdk/models/threshold_metric_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5042 2024-05-01 20:46:27.000000 seeq-65.0.1/seeq/sdk/models/threshold_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4793 2024-05-01 20:46:27.000000 seeq-65.0.1/seeq/sdk/models/timer_datum_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    20067 2024-05-01 20:46:27.000000 seeq-65.0.1/seeq/sdk/models/tree_item_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7244 2024-05-01 20:46:27.000000 seeq-65.0.1/seeq/sdk/models/treemap_item_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10190 2024-05-01 20:46:27.000000 seeq-65.0.1/seeq/sdk/models/treemap_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3553 2024-05-01 20:46:27.000000 seeq-65.0.1/seeq/sdk/models/units_of_measure_batch_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4051 2024-05-01 20:46:27.000000 seeq-65.0.1/seeq/sdk/models/units_of_measure_item_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3472 2024-05-01 20:46:27.000000 seeq-65.0.1/seeq/sdk/models/units_of_measure_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11015 2024-05-01 20:46:27.000000 seeq-65.0.1/seeq/sdk/models/unsubscribe_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4193 2024-05-01 20:46:27.000000 seeq-65.0.1/seeq/sdk/models/usage_output_list_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11083 2024-05-01 20:46:27.000000 seeq-65.0.1/seeq/sdk/models/usage_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3055 2024-05-01 20:46:27.000000 seeq-65.0.1/seeq/sdk/models/usage_types_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9888 2024-05-01 20:46:27.000000 seeq-65.0.1/seeq/sdk/models/user_group_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    19622 2024-05-01 20:46:27.000000 seeq-65.0.1/seeq/sdk/models/user_group_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13170 2024-05-01 20:46:27.000000 seeq-65.0.1/seeq/sdk/models/user_group_with_id_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    19192 2024-05-01 20:46:27.000000 seeq-65.0.1/seeq/sdk/models/user_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8124 2024-05-01 20:46:27.000000 seeq-65.0.1/seeq/sdk/models/user_output_list_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    30572 2024-05-01 20:46:27.000000 seeq-65.0.1/seeq/sdk/models/user_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4241 2024-05-01 20:46:27.000000 seeq-65.0.1/seeq/sdk/models/user_password_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5463 2024-05-01 20:46:27.000000 seeq-65.0.1/seeq/sdk/models/validate_cron_list_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3332 2024-05-01 20:46:27.000000 seeq-65.0.1/seeq/sdk/models/validate_cron_list_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7088 2024-05-01 20:46:27.000000 seeq-65.0.1/seeq/sdk/models/validate_cron_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9328 2024-05-01 20:46:27.000000 seeq-65.0.1/seeq/sdk/models/workbench_item_output_list_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    20603 2024-05-01 20:46:27.000000 seeq-65.0.1/seeq/sdk/models/workbench_search_result_preview_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8268 2024-05-01 20:46:27.000000 seeq-65.0.1/seeq/sdk/models/workbook_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7400 2024-05-01 20:46:27.000000 seeq-65.0.1/seeq/sdk/models/workbook_output_list_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    16804 2024-05-01 20:46:27.000000 seeq-65.0.1/seeq/sdk/models/workbook_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6769 2024-05-01 20:46:27.000000 seeq-65.0.1/seeq/sdk/models/worksheet_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7452 2024-05-01 20:46:27.000000 seeq-65.0.1/seeq/sdk/models/worksheet_output_list_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14268 2024-05-01 20:46:27.000000 seeq-65.0.1/seeq/sdk/models/worksheet_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3232 2024-05-01 20:46:27.000000 seeq-65.0.1/seeq/sdk/models/workstep_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13818 2024-05-01 20:46:27.000000 seeq-65.0.1/seeq/sdk/models/workstep_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13450 2024-05-01 20:46:29.000000 seeq-65.0.1/seeq/sdk/rest.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-01 22:02:36.293992 seeq-65.0.1/seeq.egg-info/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3869 2024-05-01 22:02:36.000000 seeq-65.0.1/seeq.egg-info/PKG-INFO
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    18230 2024-05-01 22:02:36.000000 seeq-65.0.1/seeq.egg-info/SOURCES.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-05-01 22:02:36.000000 seeq-65.0.1/seeq.egg-info/dependency_links.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-05-01 22:02:36.000000 seeq-65.0.1/seeq.egg-info/not-zip-safe
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       86 2024-05-01 22:02:36.000000 seeq-65.0.1/seeq.egg-info/requires.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        5 2024-05-01 22:02:36.000000 seeq-65.0.1/seeq.egg-info/top_level.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-05-01 22:02:36.345995 seeq-65.0.1/setup.cfg
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1192 2024-05-01 20:42:29.000000 seeq-65.0.1/setup.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-09 22:12:11.931960 seeq-65.0.2/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    33136 2024-05-09 20:53:29.000000 seeq-65.0.2/LICENSE
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       18 2024-05-09 20:53:29.000000 seeq-65.0.2/MANIFEST.in
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3869 2024-05-09 22:12:11.931960 seeq-65.0.2/PKG-INFO
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3317 2024-05-09 20:53:29.000000 seeq-65.0.2/README.md
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-09 20:53:29.000000 seeq-65.0.2/pyproject.toml
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-09 22:12:11.867959 seeq-65.0.2/seeq/
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-09 22:12:11.871959 seeq-65.0.2/seeq/sdk/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    27471 2024-05-09 20:58:04.000000 seeq-65.0.2/seeq/sdk/__init__.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-09 22:12:11.879959 seeq-65.0.2/seeq/sdk/api/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2117 2024-05-09 20:58:04.000000 seeq-65.0.2/seeq/sdk/api/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15396 2024-05-09 20:58:03.000000 seeq-65.0.2/seeq/sdk/api/access_keys_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    29293 2024-05-09 20:58:03.000000 seeq-65.0.2/seeq/sdk/api/add_ons_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)   139189 2024-05-09 20:58:03.000000 seeq-65.0.2/seeq/sdk/api/agents_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    54975 2024-05-09 20:58:03.000000 seeq-65.0.2/seeq/sdk/api/annotations_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    24078 2024-05-09 20:58:03.000000 seeq-65.0.2/seeq/sdk/api/assets_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8202 2024-05-09 20:58:03.000000 seeq-65.0.2/seeq/sdk/api/audit_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    21842 2024-05-09 20:58:03.000000 seeq-65.0.2/seeq/sdk/api/auth_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    27275 2024-05-09 20:58:03.000000 seeq-65.0.2/seeq/sdk/api/condition_monitors_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    52130 2024-05-09 20:58:03.000000 seeq-65.0.2/seeq/sdk/api/conditions_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)   126123 2024-05-09 20:58:03.000000 seeq-65.0.2/seeq/sdk/api/content_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    84129 2024-05-09 20:58:03.000000 seeq-65.0.2/seeq/sdk/api/context_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    34507 2024-05-09 20:58:03.000000 seeq-65.0.2/seeq/sdk/api/datafiles_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    50775 2024-05-09 20:58:03.000000 seeq-65.0.2/seeq/sdk/api/datasources_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    25032 2024-05-09 20:58:03.000000 seeq-65.0.2/seeq/sdk/api/display_templates_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    24305 2024-05-09 20:58:03.000000 seeq-65.0.2/seeq/sdk/api/displays_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    30080 2024-05-09 20:58:03.000000 seeq-65.0.2/seeq/sdk/api/export_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    50560 2024-05-09 20:58:03.000000 seeq-65.0.2/seeq/sdk/api/folders_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)   107375 2024-05-09 20:58:03.000000 seeq-65.0.2/seeq/sdk/api/formulas_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5495 2024-05-09 20:58:03.000000 seeq-65.0.2/seeq/sdk/api/graph_ql_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)   195259 2024-05-09 20:58:03.000000 seeq-65.0.2/seeq/sdk/api/items_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    35736 2024-05-09 20:58:04.000000 seeq-65.0.2/seeq/sdk/api/jobs_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    21471 2024-05-09 20:58:04.000000 seeq-65.0.2/seeq/sdk/api/logs_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    24612 2024-05-09 20:58:04.000000 seeq-65.0.2/seeq/sdk/api/metrics_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    32019 2024-05-09 20:58:04.000000 seeq-65.0.2/seeq/sdk/api/monitors_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5962 2024-05-09 20:58:04.000000 seeq-65.0.2/seeq/sdk/api/networks_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    33687 2024-05-09 20:58:04.000000 seeq-65.0.2/seeq/sdk/api/notification_configurations_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10156 2024-05-09 20:58:04.000000 seeq-65.0.2/seeq/sdk/api/notifier_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    21444 2024-05-09 20:58:04.000000 seeq-65.0.2/seeq/sdk/api/plugins_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    35456 2024-05-09 20:58:04.000000 seeq-65.0.2/seeq/sdk/api/projects_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    24605 2024-05-09 20:58:04.000000 seeq-65.0.2/seeq/sdk/api/report_templates_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5758 2024-05-09 20:58:04.000000 seeq-65.0.2/seeq/sdk/api/reports_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    38193 2024-05-09 20:58:04.000000 seeq-65.0.2/seeq/sdk/api/requests_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    28492 2024-05-09 20:58:04.000000 seeq-65.0.2/seeq/sdk/api/scalars_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    17482 2024-05-09 20:58:04.000000 seeq-65.0.2/seeq/sdk/api/scim_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)   110312 2024-05-09 20:58:04.000000 seeq-65.0.2/seeq/sdk/api/signals_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    20586 2024-05-09 20:58:04.000000 seeq-65.0.2/seeq/sdk/api/subscriptions_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)   104888 2024-05-09 20:58:04.000000 seeq-65.0.2/seeq/sdk/api/system_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    51967 2024-05-09 20:58:04.000000 seeq-65.0.2/seeq/sdk/api/table_definitions_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    66306 2024-05-09 20:58:04.000000 seeq-65.0.2/seeq/sdk/api/trees_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8652 2024-05-09 20:58:04.000000 seeq-65.0.2/seeq/sdk/api/unstable_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12944 2024-05-09 20:58:04.000000 seeq-65.0.2/seeq/sdk/api/usage_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    52327 2024-05-09 20:58:04.000000 seeq-65.0.2/seeq/sdk/api/user_groups_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    49735 2024-05-09 20:58:04.000000 seeq-65.0.2/seeq/sdk/api/users_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    94800 2024-05-09 20:58:04.000000 seeq-65.0.2/seeq/sdk/api/workbooks_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    32200 2024-05-09 20:58:04.000000 seeq-65.0.2/seeq/sdk/api_client.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9343 2024-05-09 20:58:04.000000 seeq-65.0.2/seeq/sdk/configuration.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-09 22:12:11.931960 seeq-65.0.2/seeq/sdk/models/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    22725 2024-05-09 20:58:04.000000 seeq-65.0.2/seeq/sdk/models/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4286 2024-05-09 20:57:55.000000 seeq-65.0.2/seeq/sdk/models/access_key_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7328 2024-05-09 20:57:55.000000 seeq-65.0.2/seeq/sdk/models/access_key_output_list_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14440 2024-05-09 20:57:55.000000 seeq-65.0.2/seeq/sdk/models/access_key_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4107 2024-05-09 20:57:55.000000 seeq-65.0.2/seeq/sdk/models/ace_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5730 2024-05-09 20:57:55.000000 seeq-65.0.2/seeq/sdk/models/ace_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6786 2024-05-09 20:57:56.000000 seeq-65.0.2/seeq/sdk/models/acl_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6589 2024-05-09 20:57:56.000000 seeq-65.0.2/seeq/sdk/models/acl_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3601 2024-05-09 20:57:56.000000 seeq-65.0.2/seeq/sdk/models/activity_graph_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7375 2024-05-09 20:57:56.000000 seeq-65.0.2/seeq/sdk/models/activity_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8578 2024-05-09 20:57:56.000000 seeq-65.0.2/seeq/sdk/models/add_on_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7271 2024-05-09 20:57:56.000000 seeq-65.0.2/seeq/sdk/models/add_on_output_list_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15975 2024-05-09 20:57:56.000000 seeq-65.0.2/seeq/sdk/models/add_on_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7513 2024-05-09 20:57:56.000000 seeq-65.0.2/seeq/sdk/models/add_on_preview_output_list_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6530 2024-05-09 20:57:56.000000 seeq-65.0.2/seeq/sdk/models/add_on_preview_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11088 2024-05-09 20:57:56.000000 seeq-65.0.2/seeq/sdk/models/add_on_tool_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    17343 2024-05-09 20:57:56.000000 seeq-65.0.2/seeq/sdk/models/add_on_tool_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4143 2024-05-09 20:57:56.000000 seeq-65.0.2/seeq/sdk/models/administrator_contact_information_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4853 2024-05-09 20:57:56.000000 seeq-65.0.2/seeq/sdk/models/agent_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3128 2024-05-09 20:57:56.000000 seeq-65.0.2/seeq/sdk/models/agent_key_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7460 2024-05-09 20:57:56.000000 seeq-65.0.2/seeq/sdk/models/agent_orchestrator_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13856 2024-05-09 20:57:56.000000 seeq-65.0.2/seeq/sdk/models/agent_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8806 2024-05-09 20:57:56.000000 seeq-65.0.2/seeq/sdk/models/agent_status_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7833 2024-05-09 20:57:56.000000 seeq-65.0.2/seeq/sdk/models/agent_status_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4282 2024-05-09 20:57:56.000000 seeq-65.0.2/seeq/sdk/models/annotation_image_link_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11035 2024-05-09 20:57:56.000000 seeq-65.0.2/seeq/sdk/models/annotation_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4225 2024-05-09 20:57:56.000000 seeq-65.0.2/seeq/sdk/models/annotation_interest_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3750 2024-05-09 20:57:56.000000 seeq-65.0.2/seeq/sdk/models/annotation_interest_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7392 2024-05-09 20:57:56.000000 seeq-65.0.2/seeq/sdk/models/annotation_list_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    34976 2024-05-09 20:57:56.000000 seeq-65.0.2/seeq/sdk/models/annotation_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4433 2024-05-09 20:57:56.000000 seeq-65.0.2/seeq/sdk/models/archive_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4176 2024-05-09 20:57:56.000000 seeq-65.0.2/seeq/sdk/models/asset_batch_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4667 2024-05-09 20:57:56.000000 seeq-65.0.2/seeq/sdk/models/asset_error.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14717 2024-05-09 20:57:56.000000 seeq-65.0.2/seeq/sdk/models/asset_group_asset_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4038 2024-05-09 20:57:56.000000 seeq-65.0.2/seeq/sdk/models/asset_group_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3969 2024-05-09 20:57:56.000000 seeq-65.0.2/seeq/sdk/models/asset_group_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13792 2024-05-09 20:57:56.000000 seeq-65.0.2/seeq/sdk/models/asset_group_root_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6462 2024-05-09 20:57:56.000000 seeq-65.0.2/seeq/sdk/models/asset_group_tree_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11760 2024-05-09 20:57:56.000000 seeq-65.0.2/seeq/sdk/models/asset_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    17564 2024-05-09 20:57:57.000000 seeq-65.0.2/seeq/sdk/models/asset_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8465 2024-05-09 20:57:57.000000 seeq-65.0.2/seeq/sdk/models/asset_selection_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13114 2024-05-09 20:57:57.000000 seeq-65.0.2/seeq/sdk/models/asset_selection_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7086 2024-05-09 20:57:57.000000 seeq-65.0.2/seeq/sdk/models/asset_tree_batch_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11209 2024-05-09 20:57:57.000000 seeq-65.0.2/seeq/sdk/models/asset_tree_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4432 2024-05-09 20:57:57.000000 seeq-65.0.2/seeq/sdk/models/asset_tree_single_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4866 2024-05-09 20:57:57.000000 seeq-65.0.2/seeq/sdk/models/attachment_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8190 2024-05-09 20:57:57.000000 seeq-65.0.2/seeq/sdk/models/audit_output_list_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9644 2024-05-09 20:57:57.000000 seeq-65.0.2/seeq/sdk/models/audit_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7075 2024-05-09 20:57:57.000000 seeq-65.0.2/seeq/sdk/models/auth_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3442 2024-05-09 20:57:57.000000 seeq-65.0.2/seeq/sdk/models/auth_providers_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4444 2024-05-09 20:57:57.000000 seeq-65.0.2/seeq/sdk/models/authoritative_region_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2455 2024-05-09 20:57:57.000000 seeq-65.0.2/seeq/sdk/models/boolean_configuration_field_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9542 2024-05-09 20:57:57.000000 seeq-65.0.2/seeq/sdk/models/cache_block.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4089 2024-05-09 20:57:57.000000 seeq-65.0.2/seeq/sdk/models/cache_info_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    20746 2024-05-09 20:57:57.000000 seeq-65.0.2/seeq/sdk/models/calculated_item_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5332 2024-05-09 20:57:57.000000 seeq-65.0.2/seeq/sdk/models/capsule_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4348 2024-05-09 20:57:57.000000 seeq-65.0.2/seeq/sdk/models/capsule_property_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4161 2024-05-09 20:57:57.000000 seeq-65.0.2/seeq/sdk/models/capsule_property_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7480 2024-05-09 20:57:57.000000 seeq-65.0.2/seeq/sdk/models/capsule_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3259 2024-05-09 20:57:57.000000 seeq-65.0.2/seeq/sdk/models/capsules_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10294 2024-05-09 20:57:57.000000 seeq-65.0.2/seeq/sdk/models/capsules_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4020 2024-05-09 20:57:57.000000 seeq-65.0.2/seeq/sdk/models/capsules_overwrite_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7228 2024-05-09 20:57:57.000000 seeq-65.0.2/seeq/sdk/models/channel_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4181 2024-05-09 20:57:57.000000 seeq-65.0.2/seeq/sdk/models/column_definition_input_list_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8308 2024-05-09 20:57:57.000000 seeq-65.0.2/seeq/sdk/models/column_definition_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3797 2024-05-09 20:57:57.000000 seeq-65.0.2/seeq/sdk/models/column_definition_order_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7934 2024-05-09 20:57:57.000000 seeq-65.0.2/seeq/sdk/models/column_definition_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4700 2024-05-09 20:57:57.000000 seeq-65.0.2/seeq/sdk/models/column_rule_ancestor_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10419 2024-05-09 20:57:57.000000 seeq-65.0.2/seeq/sdk/models/column_rule_asset_creator_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3561 2024-05-09 20:57:57.000000 seeq-65.0.2/seeq/sdk/models/column_rule_concat_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3577 2024-05-09 20:57:57.000000 seeq-65.0.2/seeq/sdk/models/column_rule_constant_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8932 2024-05-09 20:57:57.000000 seeq-65.0.2/seeq/sdk/models/column_rule_descendant_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3634 2024-05-09 20:57:57.000000 seeq-65.0.2/seeq/sdk/models/column_rule_event_property_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12681 2024-05-09 20:57:57.000000 seeq-65.0.2/seeq/sdk/models/column_rule_formula_creator_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10334 2024-05-09 20:57:57.000000 seeq-65.0.2/seeq/sdk/models/column_rule_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4507 2024-05-09 20:57:57.000000 seeq-65.0.2/seeq/sdk/models/column_rule_item_property_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4782 2024-05-09 20:57:57.000000 seeq-65.0.2/seeq/sdk/models/column_rule_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5241 2024-05-09 20:57:57.000000 seeq-65.0.2/seeq/sdk/models/column_rule_path_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4525 2024-05-09 20:57:57.000000 seeq-65.0.2/seeq/sdk/models/column_rule_tree_path_creator_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3409 2024-05-09 20:57:57.000000 seeq-65.0.2/seeq/sdk/models/condition_batch_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    20503 2024-05-09 20:57:57.000000 seeq-65.0.2/seeq/sdk/models/condition_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12557 2024-05-09 20:57:57.000000 seeq-65.0.2/seeq/sdk/models/condition_monitor_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11211 2024-05-09 20:57:57.000000 seeq-65.0.2/seeq/sdk/models/condition_monitor_notification_configuration_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    22784 2024-05-09 20:57:57.000000 seeq-65.0.2/seeq/sdk/models/condition_monitor_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9233 2024-05-09 20:57:57.000000 seeq-65.0.2/seeq/sdk/models/condition_notification_output_list_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6660 2024-05-09 20:57:57.000000 seeq-65.0.2/seeq/sdk/models/condition_notification_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    24440 2024-05-09 20:57:57.000000 seeq-65.0.2/seeq/sdk/models/condition_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    23781 2024-05-09 20:57:57.000000 seeq-65.0.2/seeq/sdk/models/condition_update_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7675 2024-05-09 20:57:57.000000 seeq-65.0.2/seeq/sdk/models/configuration_field_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4064 2024-05-09 20:57:57.000000 seeq-65.0.2/seeq/sdk/models/configuration_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4276 2024-05-09 20:57:57.000000 seeq-65.0.2/seeq/sdk/models/configuration_option_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3748 2024-05-09 20:57:57.000000 seeq-65.0.2/seeq/sdk/models/configuration_option_output_simple_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12329 2024-05-09 20:57:57.000000 seeq-65.0.2/seeq/sdk/models/configuration_option_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8813 2024-05-09 20:57:57.000000 seeq-65.0.2/seeq/sdk/models/configuration_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4959 2024-05-09 20:57:57.000000 seeq-65.0.2/seeq/sdk/models/configured_directives_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8527 2024-05-09 20:57:57.000000 seeq-65.0.2/seeq/sdk/models/connection_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    27327 2024-05-09 20:57:57.000000 seeq-65.0.2/seeq/sdk/models/connection_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    18799 2024-05-09 20:57:57.000000 seeq-65.0.2/seeq/sdk/models/connection_status_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    16922 2024-05-09 20:57:57.000000 seeq-65.0.2/seeq/sdk/models/connection_status_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3253 2024-05-09 20:57:57.000000 seeq-65.0.2/seeq/sdk/models/connections_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4941 2024-05-09 20:57:58.000000 seeq-65.0.2/seeq/sdk/models/connector_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14854 2024-05-09 20:57:58.000000 seeq-65.0.2/seeq/sdk/models/connector_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3273 2024-05-09 20:57:58.000000 seeq-65.0.2/seeq/sdk/models/connectors_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15681 2024-05-09 20:57:58.000000 seeq-65.0.2/seeq/sdk/models/content_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    22574 2024-05-09 20:57:58.000000 seeq-65.0.2/seeq/sdk/models/content_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5298 2024-05-09 20:57:58.000000 seeq-65.0.2/seeq/sdk/models/content_with_metadata_list_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    28438 2024-05-09 20:57:58.000000 seeq-65.0.2/seeq/sdk/models/content_with_metadata_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5888 2024-05-09 20:57:58.000000 seeq-65.0.2/seeq/sdk/models/context_comment_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11939 2024-05-09 20:57:58.000000 seeq-65.0.2/seeq/sdk/models/context_comment_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5849 2024-05-09 20:57:58.000000 seeq-65.0.2/seeq/sdk/models/context_label_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12837 2024-05-09 20:57:58.000000 seeq-65.0.2/seeq/sdk/models/context_label_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6788 2024-05-09 20:57:58.000000 seeq-65.0.2/seeq/sdk/models/context_opaque_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12675 2024-05-09 20:57:58.000000 seeq-65.0.2/seeq/sdk/models/context_opaque_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3446 2024-05-09 20:57:58.000000 seeq-65.0.2/seeq/sdk/models/csv_datafile_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    50145 2024-05-09 20:57:58.000000 seeq-65.0.2/seeq/sdk/models/datafile_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    53738 2024-05-09 20:57:58.000000 seeq-65.0.2/seeq/sdk/models/datafile_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3115 2024-05-09 20:57:58.000000 seeq-65.0.2/seeq/sdk/models/datafiles_csv_body.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9607 2024-05-09 20:57:58.000000 seeq-65.0.2/seeq/sdk/models/datasource_clean_up_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4283 2024-05-09 20:57:58.000000 seeq-65.0.2/seeq/sdk/models/datasource_clean_up_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13268 2024-05-09 20:57:58.000000 seeq-65.0.2/seeq/sdk/models/datasource_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7504 2024-05-09 20:57:58.000000 seeq-65.0.2/seeq/sdk/models/datasource_output_list_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    20088 2024-05-09 20:57:58.000000 seeq-65.0.2/seeq/sdk/models/datasource_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8806 2024-05-09 20:57:58.000000 seeq-65.0.2/seeq/sdk/models/datasource_preview_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15846 2024-05-09 20:57:58.000000 seeq-65.0.2/seeq/sdk/models/datasource_statistics_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8689 2024-05-09 20:57:58.000000 seeq-65.0.2/seeq/sdk/models/datasource_status_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9118 2024-05-09 20:57:58.000000 seeq-65.0.2/seeq/sdk/models/datasource_status_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    28984 2024-05-09 20:57:58.000000 seeq-65.0.2/seeq/sdk/models/datasource_summary_status_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11225 2024-05-09 20:57:58.000000 seeq-65.0.2/seeq/sdk/models/datasources_status_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9723 2024-05-09 20:57:58.000000 seeq-65.0.2/seeq/sdk/models/date_range_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    16890 2024-05-09 20:57:58.000000 seeq-65.0.2/seeq/sdk/models/date_range_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4111 2024-05-09 20:57:58.000000 seeq-65.0.2/seeq/sdk/models/debug_cache_block_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4868 2024-05-09 20:57:58.000000 seeq-65.0.2/seeq/sdk/models/detailed_meter_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5727 2024-05-09 20:57:58.000000 seeq-65.0.2/seeq/sdk/models/detailed_timer_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5047 2024-05-09 20:57:58.000000 seeq-65.0.2/seeq/sdk/models/directive_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5244 2024-05-09 20:57:58.000000 seeq-65.0.2/seeq/sdk/models/display_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7354 2024-05-09 20:57:58.000000 seeq-65.0.2/seeq/sdk/models/display_output_list_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14727 2024-05-09 20:57:58.000000 seeq-65.0.2/seeq/sdk/models/display_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9431 2024-05-09 20:57:58.000000 seeq-65.0.2/seeq/sdk/models/display_template_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7791 2024-05-09 20:57:58.000000 seeq-65.0.2/seeq/sdk/models/display_template_output_list_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15926 2024-05-09 20:57:58.000000 seeq-65.0.2/seeq/sdk/models/display_template_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4899 2024-05-09 20:57:58.000000 seeq-65.0.2/seeq/sdk/models/document_backup_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4138 2024-05-09 20:57:58.000000 seeq-65.0.2/seeq/sdk/models/double_configuration_field_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5405 2024-05-09 20:57:58.000000 seeq-65.0.2/seeq/sdk/models/email_notification_recipient_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6366 2024-05-09 20:57:58.000000 seeq-65.0.2/seeq/sdk/models/emailer_configuration_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5314 2024-05-09 20:57:58.000000 seeq-65.0.2/seeq/sdk/models/export_item_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    22645 2024-05-09 20:57:58.000000 seeq-65.0.2/seeq/sdk/models/export_items_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    18512 2024-05-09 20:57:58.000000 seeq-65.0.2/seeq/sdk/models/export_items_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7286 2024-05-09 20:57:58.000000 seeq-65.0.2/seeq/sdk/models/export_preview_list_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10723 2024-05-09 20:57:58.000000 seeq-65.0.2/seeq/sdk/models/export_preview_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5909 2024-05-09 20:57:58.000000 seeq-65.0.2/seeq/sdk/models/fixed_list_search_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6490 2024-05-09 20:57:58.000000 seeq-65.0.2/seeq/sdk/models/folded_stack_node_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7686 2024-05-09 20:57:58.000000 seeq-65.0.2/seeq/sdk/models/folder_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5698 2024-05-09 20:57:58.000000 seeq-65.0.2/seeq/sdk/models/folder_navigation_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15863 2024-05-09 20:57:58.000000 seeq-65.0.2/seeq/sdk/models/folder_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4035 2024-05-09 20:57:58.000000 seeq-65.0.2/seeq/sdk/models/formula_compile_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6875 2024-05-09 20:57:58.000000 seeq-65.0.2/seeq/sdk/models/formula_compile_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8113 2024-05-09 20:57:58.000000 seeq-65.0.2/seeq/sdk/models/formula_compiler_error_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4330 2024-05-09 20:57:58.000000 seeq-65.0.2/seeq/sdk/models/formula_dependency_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4006 2024-05-09 20:57:58.000000 seeq-65.0.2/seeq/sdk/models/formula_doc_example_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3464 2024-05-09 20:57:58.000000 seeq-65.0.2/seeq/sdk/models/formula_doc_example_list_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7389 2024-05-09 20:57:58.000000 seeq-65.0.2/seeq/sdk/models/formula_doc_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3415 2024-05-09 20:57:58.000000 seeq-65.0.2/seeq/sdk/models/formula_doc_keyword_list_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    21607 2024-05-09 20:57:58.000000 seeq-65.0.2/seeq/sdk/models/formula_doc_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3228 2024-05-09 20:57:59.000000 seeq-65.0.2/seeq/sdk/models/formula_doc_summaries_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8265 2024-05-09 20:57:59.000000 seeq-65.0.2/seeq/sdk/models/formula_doc_summary_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8265 2024-05-09 20:57:59.000000 seeq-65.0.2/seeq/sdk/models/formula_error_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3952 2024-05-09 20:57:59.000000 seeq-65.0.2/seeq/sdk/models/formula_example_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    18896 2024-05-09 20:57:59.000000 seeq-65.0.2/seeq/sdk/models/formula_item_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    20492 2024-05-09 20:57:59.000000 seeq-65.0.2/seeq/sdk/models/formula_item_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3933 2024-05-09 20:57:59.000000 seeq-65.0.2/seeq/sdk/models/formula_log_entry.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3718 2024-05-09 20:57:59.000000 seeq-65.0.2/seeq/sdk/models/formula_log_entry_details.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4453 2024-05-09 20:57:59.000000 seeq-65.0.2/seeq/sdk/models/formula_log_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6771 2024-05-09 20:57:59.000000 seeq-65.0.2/seeq/sdk/models/formula_package_import_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6060 2024-05-09 20:57:59.000000 seeq-65.0.2/seeq/sdk/models/formula_package_import_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9360 2024-05-09 20:57:59.000000 seeq-65.0.2/seeq/sdk/models/formula_package_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    17867 2024-05-09 20:57:59.000000 seeq-65.0.2/seeq/sdk/models/formula_package_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6189 2024-05-09 20:57:59.000000 seeq-65.0.2/seeq/sdk/models/formula_parameter_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5572 2024-05-09 20:57:59.000000 seeq-65.0.2/seeq/sdk/models/formula_parameter_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12942 2024-05-09 20:57:59.000000 seeq-65.0.2/seeq/sdk/models/formula_run_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12280 2024-05-09 20:57:59.000000 seeq-65.0.2/seeq/sdk/models/formula_run_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4077 2024-05-09 20:57:59.000000 seeq-65.0.2/seeq/sdk/models/formula_token.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4064 2024-05-09 20:57:59.000000 seeq-65.0.2/seeq/sdk/models/formula_update_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4108 2024-05-09 20:57:59.000000 seeq-65.0.2/seeq/sdk/models/formula_upgrade_change_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4932 2024-05-09 20:57:59.000000 seeq-65.0.2/seeq/sdk/models/formula_upgrade_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13617 2024-05-09 20:57:59.000000 seeq-65.0.2/seeq/sdk/models/function_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4594 2024-05-09 20:57:59.000000 seeq-65.0.2/seeq/sdk/models/function_parameter_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6327 2024-05-09 20:57:59.000000 seeq-65.0.2/seeq/sdk/models/function_variant_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4834 2024-05-09 20:57:59.000000 seeq-65.0.2/seeq/sdk/models/gauge_datum_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4157 2024-05-09 20:57:59.000000 seeq-65.0.2/seeq/sdk/models/generic_table_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3286 2024-05-09 20:57:59.000000 seeq-65.0.2/seeq/sdk/models/get_add_on_tools_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7344 2024-05-09 20:57:59.000000 seeq-65.0.2/seeq/sdk/models/get_channels_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9186 2024-05-09 20:57:59.000000 seeq-65.0.2/seeq/sdk/models/get_condition_monitor_items_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7561 2024-05-09 20:57:59.000000 seeq-65.0.2/seeq/sdk/models/get_content_items_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7469 2024-05-09 20:57:59.000000 seeq-65.0.2/seeq/sdk/models/get_date_ranges_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7136 2024-05-09 20:57:59.000000 seeq-65.0.2/seeq/sdk/models/get_jobs_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7319 2024-05-09 20:57:59.000000 seeq-65.0.2/seeq/sdk/models/get_metrics_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7348 2024-05-09 20:57:59.000000 seeq-65.0.2/seeq/sdk/models/get_projects_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4191 2024-05-09 20:57:59.000000 seeq-65.0.2/seeq/sdk/models/get_request_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3122 2024-05-09 20:57:59.000000 seeq-65.0.2/seeq/sdk/models/get_requests_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6221 2024-05-09 20:57:59.000000 seeq-65.0.2/seeq/sdk/models/get_sample_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11225 2024-05-09 20:57:59.000000 seeq-65.0.2/seeq/sdk/models/get_samples_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7292 2024-05-09 20:57:59.000000 seeq-65.0.2/seeq/sdk/models/get_signals_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3806 2024-05-09 20:57:59.000000 seeq-65.0.2/seeq/sdk/models/graph_ql_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3765 2024-05-09 20:57:59.000000 seeq-65.0.2/seeq/sdk/models/graph_ql_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3087 2024-05-09 20:57:59.000000 seeq-65.0.2/seeq/sdk/models/id_images_body.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3541 2024-05-09 20:57:59.000000 seeq-65.0.2/seeq/sdk/models/identity_mapping_list_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6253 2024-05-09 20:57:59.000000 seeq-65.0.2/seeq/sdk/models/identity_mapping_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8348 2024-05-09 20:57:59.000000 seeq-65.0.2/seeq/sdk/models/identity_preview_list_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12927 2024-05-09 20:57:59.000000 seeq-65.0.2/seeq/sdk/models/identity_preview_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4212 2024-05-09 20:57:59.000000 seeq-65.0.2/seeq/sdk/models/indexing_parameters_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4947 2024-05-09 20:57:59.000000 seeq-65.0.2/seeq/sdk/models/installer_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4136 2024-05-09 20:57:59.000000 seeq-65.0.2/seeq/sdk/models/interval_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2997 2024-05-09 20:57:59.000000 seeq-65.0.2/seeq/sdk/models/invalid_swap_out_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5360 2024-05-09 20:57:59.000000 seeq-65.0.2/seeq/sdk/models/item_batch_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11549 2024-05-09 20:57:59.000000 seeq-65.0.2/seeq/sdk/models/item_dependency_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11046 2024-05-09 20:57:59.000000 seeq-65.0.2/seeq/sdk/models/item_finder_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7639 2024-05-09 20:57:59.000000 seeq-65.0.2/seeq/sdk/models/item_finder_output_list_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    17929 2024-05-09 20:57:59.000000 seeq-65.0.2/seeq/sdk/models/item_finder_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5509 2024-05-09 20:58:00.000000 seeq-65.0.2/seeq/sdk/models/item_finder_searches_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4132 2024-05-09 20:58:00.000000 seeq-65.0.2/seeq/sdk/models/item_finder_searches_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3168 2024-05-09 20:58:00.000000 seeq-65.0.2/seeq/sdk/models/item_id_list_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14649 2024-05-09 20:58:00.000000 seeq-65.0.2/seeq/sdk/models/item_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11275 2024-05-09 20:58:00.000000 seeq-65.0.2/seeq/sdk/models/item_parameter_of_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8178 2024-05-09 20:58:00.000000 seeq-65.0.2/seeq/sdk/models/item_preview_list_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6934 2024-05-09 20:58:00.000000 seeq-65.0.2/seeq/sdk/models/item_preview_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9485 2024-05-09 20:58:00.000000 seeq-65.0.2/seeq/sdk/models/item_preview_with_assets_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4196 2024-05-09 20:58:00.000000 seeq-65.0.2/seeq/sdk/models/item_search_preview_list_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8661 2024-05-09 20:58:00.000000 seeq-65.0.2/seeq/sdk/models/item_search_preview_paginated_list_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    16178 2024-05-09 20:58:00.000000 seeq-65.0.2/seeq/sdk/models/item_search_preview_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4708 2024-05-09 20:58:00.000000 seeq-65.0.2/seeq/sdk/models/item_swap_result_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6537 2024-05-09 20:58:00.000000 seeq-65.0.2/seeq/sdk/models/item_update_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4220 2024-05-09 20:58:00.000000 seeq-65.0.2/seeq/sdk/models/item_user_attributes_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5888 2024-05-09 20:58:00.000000 seeq-65.0.2/seeq/sdk/models/item_user_attributes_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5144 2024-05-09 20:58:00.000000 seeq-65.0.2/seeq/sdk/models/item_with_swap_pairs_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4395 2024-05-09 20:58:00.000000 seeq-65.0.2/seeq/sdk/models/jira_attachment.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6025 2024-05-09 20:58:00.000000 seeq-65.0.2/seeq/sdk/models/jira_attachment_media_type.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6230 2024-05-09 20:58:00.000000 seeq-65.0.2/seeq/sdk/models/job_accepted_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14001 2024-05-09 20:58:00.000000 seeq-65.0.2/seeq/sdk/models/job_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4845 2024-05-09 20:58:00.000000 seeq-65.0.2/seeq/sdk/models/json_backup_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4626 2024-05-09 20:58:00.000000 seeq-65.0.2/seeq/sdk/models/label_category_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3222 2024-05-09 20:58:00.000000 seeq-65.0.2/seeq/sdk/models/label_category_output_list_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5274 2024-05-09 20:58:00.000000 seeq-65.0.2/seeq/sdk/models/label_category_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4773 2024-05-09 20:58:00.000000 seeq-65.0.2/seeq/sdk/models/label_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3062 2024-05-09 20:58:00.000000 seeq-65.0.2/seeq/sdk/models/label_output_list_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5063 2024-05-09 20:58:00.000000 seeq-65.0.2/seeq/sdk/models/label_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4381 2024-05-09 20:58:00.000000 seeq-65.0.2/seeq/sdk/models/license_importer_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13507 2024-05-09 20:58:00.000000 seeq-65.0.2/seeq/sdk/models/license_status_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6191 2024-05-09 20:58:00.000000 seeq-65.0.2/seeq/sdk/models/licensed_feature_status_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4668 2024-05-09 20:58:00.000000 seeq-65.0.2/seeq/sdk/models/log_message.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4136 2024-05-09 20:58:00.000000 seeq-65.0.2/seeq/sdk/models/long_configuration_field_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4693 2024-05-09 20:58:00.000000 seeq-65.0.2/seeq/sdk/models/meter_datum_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3177 2024-05-09 20:58:00.000000 seeq-65.0.2/seeq/sdk/models/migrate_editor_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4779 2024-05-09 20:58:00.000000 seeq-65.0.2/seeq/sdk/models/monitor_definition_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3420 2024-05-09 20:58:00.000000 seeq-65.0.2/seeq/sdk/models/monitor_definitions_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4520 2024-05-09 20:58:00.000000 seeq-65.0.2/seeq/sdk/models/monitor_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3189 2024-05-09 20:58:00.000000 seeq-65.0.2/seeq/sdk/models/monitor_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13074 2024-05-09 20:58:00.000000 seeq-65.0.2/seeq/sdk/models/monitor_values.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3164 2024-05-09 20:58:00.000000 seeq-65.0.2/seeq/sdk/models/monitors_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8926 2024-05-09 20:58:00.000000 seeq-65.0.2/seeq/sdk/models/notifiable_report_output_list_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8081 2024-05-09 20:58:00.000000 seeq-65.0.2/seeq/sdk/models/notifiable_report_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12021 2024-05-09 20:58:00.000000 seeq-65.0.2/seeq/sdk/models/notification_configuration_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6065 2024-05-09 20:58:00.000000 seeq-65.0.2/seeq/sdk/models/optional_report_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6206 2024-05-09 20:58:00.000000 seeq-65.0.2/seeq/sdk/models/parameter_doc_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4124 2024-05-09 20:58:00.000000 seeq-65.0.2/seeq/sdk/models/permissions_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8236 2024-05-09 20:58:00.000000 seeq-65.0.2/seeq/sdk/models/plugin_output_list_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    16602 2024-05-09 20:58:00.000000 seeq-65.0.2/seeq/sdk/models/plugin_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3084 2024-05-09 20:58:00.000000 seeq-65.0.2/seeq/sdk/models/plugins_body.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6354 2024-05-09 20:58:00.000000 seeq-65.0.2/seeq/sdk/models/pre_provision_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3980 2024-05-09 20:58:00.000000 seeq-65.0.2/seeq/sdk/models/pre_provision_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4929 2024-05-09 20:58:00.000000 seeq-65.0.2/seeq/sdk/models/priority_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4011 2024-05-09 20:58:00.000000 seeq-65.0.2/seeq/sdk/models/progress_information_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10158 2024-05-09 20:58:00.000000 seeq-65.0.2/seeq/sdk/models/project_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    20788 2024-05-09 20:58:00.000000 seeq-65.0.2/seeq/sdk/models/project_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5624 2024-05-09 20:58:00.000000 seeq-65.0.2/seeq/sdk/models/property_filter_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4255 2024-05-09 20:58:00.000000 seeq-65.0.2/seeq/sdk/models/property_href_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4582 2024-05-09 20:58:00.000000 seeq-65.0.2/seeq/sdk/models/property_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6492 2024-05-09 20:58:00.000000 seeq-65.0.2/seeq/sdk/models/property_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8130 2024-05-09 20:58:00.000000 seeq-65.0.2/seeq/sdk/models/property_search_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5041 2024-05-09 20:58:00.000000 seeq-65.0.2/seeq/sdk/models/provision_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13320 2024-05-09 20:58:00.000000 seeq-65.0.2/seeq/sdk/models/put_asset_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    19360 2024-05-09 20:58:00.000000 seeq-65.0.2/seeq/sdk/models/put_scalar_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7198 2024-05-09 20:58:00.000000 seeq-65.0.2/seeq/sdk/models/put_scalars_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3288 2024-05-09 20:58:00.000000 seeq-65.0.2/seeq/sdk/models/put_signals_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3413 2024-05-09 20:58:00.000000 seeq-65.0.2/seeq/sdk/models/put_user_groups_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3276 2024-05-09 20:58:00.000000 seeq-65.0.2/seeq/sdk/models/referenced_items_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11239 2024-05-09 20:58:00.000000 seeq-65.0.2/seeq/sdk/models/regression_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4575 2024-05-09 20:58:01.000000 seeq-65.0.2/seeq/sdk/models/remote_agent_directives_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    16599 2024-05-09 20:58:01.000000 seeq-65.0.2/seeq/sdk/models/remote_agent_status_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    16708 2024-05-09 20:58:01.000000 seeq-65.0.2/seeq/sdk/models/remote_agent_status_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5135 2024-05-09 20:58:01.000000 seeq-65.0.2/seeq/sdk/models/report_input_item_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4810 2024-05-09 20:58:01.000000 seeq-65.0.2/seeq/sdk/models/report_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8329 2024-05-09 20:58:01.000000 seeq-65.0.2/seeq/sdk/models/report_notification_configuration_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6225 2024-05-09 20:58:01.000000 seeq-65.0.2/seeq/sdk/models/report_template_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15217 2024-05-09 20:58:01.000000 seeq-65.0.2/seeq/sdk/models/report_template_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15198 2024-05-09 20:58:01.000000 seeq-65.0.2/seeq/sdk/models/request_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4385 2024-05-09 20:58:01.000000 seeq-65.0.2/seeq/sdk/models/sample_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4453 2024-05-09 20:58:01.000000 seeq-65.0.2/seeq/sdk/models/sample_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3237 2024-05-09 20:58:01.000000 seeq-65.0.2/seeq/sdk/models/samples_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3501 2024-05-09 20:58:01.000000 seeq-65.0.2/seeq/sdk/models/samples_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3994 2024-05-09 20:58:01.000000 seeq-65.0.2/seeq/sdk/models/samples_overwrite_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11225 2024-05-09 20:58:01.000000 seeq-65.0.2/seeq/sdk/models/scalar_evaluate_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    17724 2024-05-09 20:58:01.000000 seeq-65.0.2/seeq/sdk/models/scalar_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5290 2024-05-09 20:58:01.000000 seeq-65.0.2/seeq/sdk/models/scalar_property_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4748 2024-05-09 20:58:01.000000 seeq-65.0.2/seeq/sdk/models/scalar_value_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4542 2024-05-09 20:58:01.000000 seeq-65.0.2/seeq/sdk/models/scale_across_tree_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8516 2024-05-09 20:58:01.000000 seeq-65.0.2/seeq/sdk/models/schedulable_admin_list_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    16074 2024-05-09 20:58:01.000000 seeq-65.0.2/seeq/sdk/models/schedulable_admin_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4210 2024-05-09 20:58:01.000000 seeq-65.0.2/seeq/sdk/models/schedulable_summary_day_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3331 2024-05-09 20:58:01.000000 seeq-65.0.2/seeq/sdk/models/schedulable_summary_week_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4216 2024-05-09 20:58:01.000000 seeq-65.0.2/seeq/sdk/models/schedule_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4974 2024-05-09 20:58:01.000000 seeq-65.0.2/seeq/sdk/models/schedule_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9394 2024-05-09 20:58:01.000000 seeq-65.0.2/seeq/sdk/models/scheduled_notebook_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4611 2024-05-09 20:58:01.000000 seeq-65.0.2/seeq/sdk/models/scheduled_notebook_list_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    20126 2024-05-09 20:58:01.000000 seeq-65.0.2/seeq/sdk/models/scheduled_notebook_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4186 2024-05-09 20:58:01.000000 seeq-65.0.2/seeq/sdk/models/scim_token_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4325 2024-05-09 20:58:01.000000 seeq-65.0.2/seeq/sdk/models/screenshot_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4142 2024-05-09 20:58:01.000000 seeq-65.0.2/seeq/sdk/models/secret_configuration_field_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5699 2024-05-09 20:58:01.000000 seeq-65.0.2/seeq/sdk/models/see_also_doc_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4926 2024-05-09 20:58:01.000000 seeq-65.0.2/seeq/sdk/models/send_email_attachment_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3804 2024-05-09 20:58:01.000000 seeq-65.0.2/seeq/sdk/models/send_email_contact_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7956 2024-05-09 20:58:01.000000 seeq-65.0.2/seeq/sdk/models/send_email_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5175 2024-05-09 20:58:01.000000 seeq-65.0.2/seeq/sdk/models/sent_email_attachment_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12471 2024-05-09 20:58:01.000000 seeq-65.0.2/seeq/sdk/models/sent_email_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3347 2024-05-09 20:58:01.000000 seeq-65.0.2/seeq/sdk/models/sent_emails_list_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3349 2024-05-09 20:58:01.000000 seeq-65.0.2/seeq/sdk/models/server_build_info_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4641 2024-05-09 20:58:01.000000 seeq-65.0.2/seeq/sdk/models/server_load_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6420 2024-05-09 20:58:01.000000 seeq-65.0.2/seeq/sdk/models/server_spec_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11947 2024-05-09 20:58:01.000000 seeq-65.0.2/seeq/sdk/models/server_status_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    18077 2024-05-09 20:58:01.000000 seeq-65.0.2/seeq/sdk/models/signal_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    27764 2024-05-09 20:58:01.000000 seeq-65.0.2/seeq/sdk/models/signal_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    23062 2024-05-09 20:58:01.000000 seeq-65.0.2/seeq/sdk/models/signal_with_id_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3267 2024-05-09 20:58:01.000000 seeq-65.0.2/seeq/sdk/models/status_message.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3515 2024-05-09 20:58:01.000000 seeq-65.0.2/seeq/sdk/models/status_message_base.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3788 2024-05-09 20:58:01.000000 seeq-65.0.2/seeq/sdk/models/store_secret_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4142 2024-05-09 20:58:01.000000 seeq-65.0.2/seeq/sdk/models/string_configuration_field_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4368 2024-05-09 20:58:01.000000 seeq-65.0.2/seeq/sdk/models/subscription_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4908 2024-05-09 20:58:01.000000 seeq-65.0.2/seeq/sdk/models/subscription_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3389 2024-05-09 20:58:01.000000 seeq-65.0.2/seeq/sdk/models/subscription_update_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10912 2024-05-09 20:58:01.000000 seeq-65.0.2/seeq/sdk/models/support_request_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4180 2024-05-09 20:58:01.000000 seeq-65.0.2/seeq/sdk/models/support_request_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4302 2024-05-09 20:58:01.000000 seeq-65.0.2/seeq/sdk/models/supported_units_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7054 2024-05-09 20:58:01.000000 seeq-65.0.2/seeq/sdk/models/swap_across_assets_search_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4209 2024-05-09 20:58:01.000000 seeq-65.0.2/seeq/sdk/models/swap_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3559 2024-05-09 20:58:01.000000 seeq-65.0.2/seeq/sdk/models/swap_option_list_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5575 2024-05-09 20:58:02.000000 seeq-65.0.2/seeq/sdk/models/swap_option_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3784 2024-05-09 20:58:02.000000 seeq-65.0.2/seeq/sdk/models/swap_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11724 2024-05-09 20:58:02.000000 seeq-65.0.2/seeq/sdk/models/sync_progress.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    18924 2024-05-09 20:58:02.000000 seeq-65.0.2/seeq/sdk/models/sync_progress_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3122 2024-05-09 20:58:02.000000 seeq-65.0.2/seeq/sdk/models/system_license_body.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4800 2024-05-09 20:58:02.000000 seeq-65.0.2/seeq/sdk/models/table_column_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10804 2024-05-09 20:58:02.000000 seeq-65.0.2/seeq/sdk/models/table_definition_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7909 2024-05-09 20:58:02.000000 seeq-65.0.2/seeq/sdk/models/table_definition_output_list_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    16936 2024-05-09 20:58:02.000000 seeq-65.0.2/seeq/sdk/models/table_definition_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5426 2024-05-09 20:58:02.000000 seeq-65.0.2/seeq/sdk/models/table_definition_update_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    19125 2024-05-09 20:58:02.000000 seeq-65.0.2/seeq/sdk/models/threshold_metric_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    28187 2024-05-09 20:58:02.000000 seeq-65.0.2/seeq/sdk/models/threshold_metric_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5042 2024-05-09 20:58:02.000000 seeq-65.0.2/seeq/sdk/models/threshold_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4793 2024-05-09 20:58:02.000000 seeq-65.0.2/seeq/sdk/models/timer_datum_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    20067 2024-05-09 20:58:02.000000 seeq-65.0.2/seeq/sdk/models/tree_item_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7244 2024-05-09 20:58:02.000000 seeq-65.0.2/seeq/sdk/models/treemap_item_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10190 2024-05-09 20:58:02.000000 seeq-65.0.2/seeq/sdk/models/treemap_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3553 2024-05-09 20:58:02.000000 seeq-65.0.2/seeq/sdk/models/units_of_measure_batch_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4051 2024-05-09 20:58:02.000000 seeq-65.0.2/seeq/sdk/models/units_of_measure_item_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3472 2024-05-09 20:58:02.000000 seeq-65.0.2/seeq/sdk/models/units_of_measure_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11015 2024-05-09 20:58:02.000000 seeq-65.0.2/seeq/sdk/models/unsubscribe_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4193 2024-05-09 20:58:02.000000 seeq-65.0.2/seeq/sdk/models/usage_output_list_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11083 2024-05-09 20:58:02.000000 seeq-65.0.2/seeq/sdk/models/usage_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3055 2024-05-09 20:58:02.000000 seeq-65.0.2/seeq/sdk/models/usage_types_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9888 2024-05-09 20:58:02.000000 seeq-65.0.2/seeq/sdk/models/user_group_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    19622 2024-05-09 20:58:02.000000 seeq-65.0.2/seeq/sdk/models/user_group_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13170 2024-05-09 20:58:02.000000 seeq-65.0.2/seeq/sdk/models/user_group_with_id_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    19192 2024-05-09 20:58:02.000000 seeq-65.0.2/seeq/sdk/models/user_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8124 2024-05-09 20:58:02.000000 seeq-65.0.2/seeq/sdk/models/user_output_list_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    30572 2024-05-09 20:58:02.000000 seeq-65.0.2/seeq/sdk/models/user_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4241 2024-05-09 20:58:02.000000 seeq-65.0.2/seeq/sdk/models/user_password_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5463 2024-05-09 20:58:02.000000 seeq-65.0.2/seeq/sdk/models/validate_cron_list_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3332 2024-05-09 20:58:02.000000 seeq-65.0.2/seeq/sdk/models/validate_cron_list_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7088 2024-05-09 20:58:02.000000 seeq-65.0.2/seeq/sdk/models/validate_cron_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9328 2024-05-09 20:58:02.000000 seeq-65.0.2/seeq/sdk/models/workbench_item_output_list_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    20603 2024-05-09 20:58:02.000000 seeq-65.0.2/seeq/sdk/models/workbench_search_result_preview_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8268 2024-05-09 20:58:02.000000 seeq-65.0.2/seeq/sdk/models/workbook_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7400 2024-05-09 20:58:02.000000 seeq-65.0.2/seeq/sdk/models/workbook_output_list_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    16804 2024-05-09 20:58:02.000000 seeq-65.0.2/seeq/sdk/models/workbook_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6769 2024-05-09 20:58:02.000000 seeq-65.0.2/seeq/sdk/models/worksheet_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7452 2024-05-09 20:58:02.000000 seeq-65.0.2/seeq/sdk/models/worksheet_output_list_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14268 2024-05-09 20:58:02.000000 seeq-65.0.2/seeq/sdk/models/worksheet_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3232 2024-05-09 20:58:02.000000 seeq-65.0.2/seeq/sdk/models/workstep_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13818 2024-05-09 20:58:02.000000 seeq-65.0.2/seeq/sdk/models/workstep_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13450 2024-05-09 20:58:04.000000 seeq-65.0.2/seeq/sdk/rest.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-09 22:12:11.867959 seeq-65.0.2/seeq.egg-info/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3869 2024-05-09 22:12:11.000000 seeq-65.0.2/seeq.egg-info/PKG-INFO
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    18230 2024-05-09 22:12:11.000000 seeq-65.0.2/seeq.egg-info/SOURCES.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-05-09 22:12:11.000000 seeq-65.0.2/seeq.egg-info/dependency_links.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-05-09 22:12:11.000000 seeq-65.0.2/seeq.egg-info/not-zip-safe
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       86 2024-05-09 22:12:11.000000 seeq-65.0.2/seeq.egg-info/requires.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        5 2024-05-09 22:12:11.000000 seeq-65.0.2/seeq.egg-info/top_level.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-05-09 22:12:11.931960 seeq-65.0.2/setup.cfg
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1192 2024-05-09 20:56:00.000000 seeq-65.0.2/setup.py
```

### Comparing `seeq-65.0.1/LICENSE` & `seeq-65.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `seeq-65.0.1/PKG-INFO` & `seeq-65.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seeq
-Version: 65.0.1
+Version: 65.0.2
 Summary: The Seeq SDK for Python
 Home-page: https://www.seeq.com
 Author: Seeq Corporation
 Author-email: support@seeq.com
 Project-URL: Documentation, https://python-docs.seeq.com/
 Project-URL: Changelog, https://python-docs.seeq.com/changelog.html
 Classifier: Programming Language :: Python :: 2
```

### Comparing `seeq-65.0.1/README.md` & `seeq-65.0.2/README.md`

 * *Files identical despite different names*

### Comparing `seeq-65.0.1/seeq/sdk/__init__.py` & `seeq-65.0.2/seeq/sdk/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 # flake8: noqa
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
-__version__ = "65.0.1"
+__version__ = "65.0.2"
 
 # import apis into sdk package
 from .api.access_keys_api import AccessKeysApi
 from .api.add_ons_api import AddOnsApi
 from .api.agents_api import AgentsApi
 from .api.annotations_api import AnnotationsApi
 from .api.assets_api import AssetsApi
```

### Comparing `seeq-65.0.1/seeq/sdk/api/__init__.py` & `seeq-65.0.2/seeq/sdk/api/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 # flake8: noqa
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
-__version__ = "65.0.1"
+__version__ = "65.0.2"
 
 # import apis into sdk package
 from .access_keys_api import AccessKeysApi
 from .add_ons_api import AddOnsApi
 from .agents_api import AgentsApi
 from .annotations_api import AnnotationsApi
 from .assets_api import AssetsApi
```

### Comparing `seeq-65.0.1/seeq/sdk/api/access_keys_api.py` & `seeq-65.0.2/seeq/sdk/api/access_keys_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-65.0.1/seeq/sdk/api/add_ons_api.py` & `seeq-65.0.2/seeq/sdk/api/add_ons_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-65.0.1/seeq/sdk/api/agents_api.py` & `seeq-65.0.2/seeq/sdk/api/agents_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-65.0.1/seeq/sdk/api/annotations_api.py` & `seeq-65.0.2/seeq/sdk/api/annotations_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-65.0.1/seeq/sdk/api/assets_api.py` & `seeq-65.0.2/seeq/sdk/api/assets_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-65.0.1/seeq/sdk/api/audit_api.py` & `seeq-65.0.2/seeq/sdk/api/audit_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-65.0.1/seeq/sdk/api/auth_api.py` & `seeq-65.0.2/seeq/sdk/api/auth_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-65.0.1/seeq/sdk/api/condition_monitors_api.py` & `seeq-65.0.2/seeq/sdk/api/condition_monitors_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-65.0.1/seeq/sdk/api/conditions_api.py` & `seeq-65.0.2/seeq/sdk/api/conditions_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-65.0.1/seeq/sdk/api/content_api.py` & `seeq-65.0.2/seeq/sdk/api/content_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-65.0.1/seeq/sdk/api/context_api.py` & `seeq-65.0.2/seeq/sdk/api/context_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-65.0.1/seeq/sdk/api/datafiles_api.py` & `seeq-65.0.2/seeq/sdk/api/datafiles_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-65.0.1/seeq/sdk/api/datasources_api.py` & `seeq-65.0.2/seeq/sdk/api/datasources_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-65.0.1/seeq/sdk/api/display_templates_api.py` & `seeq-65.0.2/seeq/sdk/api/display_templates_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-65.0.1/seeq/sdk/api/displays_api.py` & `seeq-65.0.2/seeq/sdk/api/displays_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-65.0.1/seeq/sdk/api/export_api.py` & `seeq-65.0.2/seeq/sdk/api/export_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-65.0.1/seeq/sdk/api/folders_api.py` & `seeq-65.0.2/seeq/sdk/api/folders_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-65.0.1/seeq/sdk/api/formulas_api.py` & `seeq-65.0.2/seeq/sdk/api/formulas_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 00000050: 7920 5377 6167 6765 7220 436f 6465 6765  y Swagger Codege
 00000060: 6e20 6874 7470 733a 2f2f 6769 7468 7562  n https://github
 00000070: 2e63 6f6d 2f73 7761 6767 6572 2d61 7069  .com/swagger-api
 00000080: 2f73 7761 6767 6572 2d63 6f64 6567 656e  /swagger-codegen
 00000090: 2920 2023 206e 6f71 613a 2045 3530 310a  )  # noqa: E501.
 000000a0: 0a20 2020 204f 7065 6e41 5049 2073 7065  .    OpenAPI spe
 000000b0: 6320 7665 7273 696f 6e3a 2036 352e 302e  c version: 65.0.
-000000c0: 312d 7632 3032 3430 3530 3132 3034 320a  1-v202405012042.
+000000c0: 322d 7632 3032 3430 3530 3932 3035 360a  2-v202405092056.
 000000d0: 2020 2020 0a20 2020 2047 656e 6572 6174      .    Generat
 000000e0: 6564 2062 793a 2068 7474 7073 3a2f 2f67  ed by: https://g
 000000f0: 6974 6875 622e 636f 6d2f 7377 6167 6765  ithub.com/swagge
 00000100: 722d 6170 692f 7377 6167 6765 722d 636f  r-api/swagger-co
 00000110: 6465 6765 6e2e 6769 740a 2222 220a 0a66  degen.git."""..f
 00000120: 726f 6d20 5f5f 6675 7475 7265 5f5f 2069  rom __future__ i
 00000130: 6d70 6f72 7420 6162 736f 6c75 7465 5f69  mport absolute_i
```

### Comparing `seeq-65.0.1/seeq/sdk/api/graph_ql_api.py` & `seeq-65.0.2/seeq/sdk/api/graph_ql_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-65.0.1/seeq/sdk/api/items_api.py` & `seeq-65.0.2/seeq/sdk/api/items_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-65.0.1/seeq/sdk/api/jobs_api.py` & `seeq-65.0.2/seeq/sdk/api/jobs_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-65.0.1/seeq/sdk/api/logs_api.py` & `seeq-65.0.2/seeq/sdk/api/logs_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-65.0.1/seeq/sdk/api/metrics_api.py` & `seeq-65.0.2/seeq/sdk/api/metrics_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-65.0.1/seeq/sdk/api/monitors_api.py` & `seeq-65.0.2/seeq/sdk/api/monitors_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-65.0.1/seeq/sdk/api/networks_api.py` & `seeq-65.0.2/seeq/sdk/api/networks_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-65.0.1/seeq/sdk/api/notification_configurations_api.py` & `seeq-65.0.2/seeq/sdk/api/notification_configurations_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-65.0.1/seeq/sdk/api/notifier_api.py` & `seeq-65.0.2/seeq/sdk/api/notifier_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-65.0.1/seeq/sdk/api/plugins_api.py` & `seeq-65.0.2/seeq/sdk/api/plugins_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-65.0.1/seeq/sdk/api/projects_api.py` & `seeq-65.0.2/seeq/sdk/api/projects_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-65.0.1/seeq/sdk/api/report_templates_api.py` & `seeq-65.0.2/seeq/sdk/api/report_templates_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-65.0.1/seeq/sdk/api/reports_api.py` & `seeq-65.0.2/seeq/sdk/api/reports_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-65.0.1/seeq/sdk/api/requests_api.py` & `seeq-65.0.2/seeq/sdk/api/requests_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-65.0.1/seeq/sdk/api/scalars_api.py` & `seeq-65.0.2/seeq/sdk/api/scalars_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-65.0.1/seeq/sdk/api/scim_api.py` & `seeq-65.0.2/seeq/sdk/api/scim_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-65.0.1/seeq/sdk/api/signals_api.py` & `seeq-65.0.2/seeq/sdk/api/signals_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-65.0.1/seeq/sdk/api/subscriptions_api.py` & `seeq-65.0.2/seeq/sdk/api/subscriptions_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-65.0.1/seeq/sdk/api/system_api.py` & `seeq-65.0.2/seeq/sdk/api/system_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-65.0.1/seeq/sdk/api/table_definitions_api.py` & `seeq-65.0.2/seeq/sdk/api/table_definitions_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-65.0.1/seeq/sdk/api/trees_api.py` & `seeq-65.0.2/seeq/sdk/api/trees_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-65.0.1/seeq/sdk/api/unstable_api.py` & `seeq-65.0.2/seeq/sdk/api/unstable_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-65.0.1/seeq/sdk/api/usage_api.py` & `seeq-65.0.2/seeq/sdk/api/usage_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-65.0.1/seeq/sdk/api/user_groups_api.py` & `seeq-65.0.2/seeq/sdk/api/user_groups_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-65.0.1/seeq/sdk/api/users_api.py` & `seeq-65.0.2/seeq/sdk/api/users_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-65.0.1/seeq/sdk/api/workbooks_api.py` & `seeq-65.0.2/seeq/sdk/api/workbooks_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-65.0.1/seeq/sdk/api_client.py` & `seeq-65.0.2/seeq/sdk/api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 from __future__ import absolute_import
 
 import json
 import mimetypes
@@ -73,15 +73,15 @@
             self.default_headers[header_name] = header_value
         if host is None:
             self.host = self.configuration.host
         else:
             self.host = host
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'Swagger-Codegen/65.0.1/python'
+        self.user_agent = 'Swagger-Codegen/65.0.2/python'
         self.auth_token = None
         self.identity_path = None
         self.csrf_token = None
 
     @property
     def user_agent(self):
         """
```

### Comparing `seeq-65.0.1/seeq/sdk/configuration.py` & `seeq-65.0.2/seeq/sdk/configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import urllib3
@@ -254,16 +254,16 @@
         Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 65.0.1-v202405012042\n"\
-               "SDK Package Version: 65.0.1".\
+               "Version of the API: 65.0.2-v202405092056\n"\
+               "SDK Package Version: 65.0.2".\
                format(env=sys.platform, pyversion=sys.version)
 
 
 default_configuration = ClientConfiguration()
 
 
 def Configuration():
```

### Comparing `seeq-65.0.1/seeq/sdk/models/__init__.py` & `seeq-65.0.2/seeq/sdk/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 # flake8: noqa
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
-__version__ = "65.0.1"
+__version__ = "65.0.2"
 
 # import models into sdk package
 from .access_key_input_v1 import AccessKeyInputV1
 from .access_key_output_list_v1 import AccessKeyOutputListV1
 from .access_key_output_v1 import AccessKeyOutputV1
 from .ace_input_v1 import AceInputV1
 from .ace_output_v1 import AceOutputV1
```

### Comparing `seeq-65.0.1/seeq/sdk/models/access_key_input_v1.py` & `seeq-65.0.2/seeq/sdk/models/access_key_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/access_key_output_list_v1.py` & `seeq-65.0.2/seeq/sdk/models/access_key_output_list_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/access_key_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/access_key_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/ace_input_v1.py` & `seeq-65.0.2/seeq/sdk/models/ace_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/ace_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/ace_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/acl_input_v1.py` & `seeq-65.0.2/seeq/sdk/models/acl_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/acl_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/acl_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/activity_graph_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/activity_graph_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/activity_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/activity_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/add_on_input_v1.py` & `seeq-65.0.2/seeq/sdk/models/add_on_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/add_on_output_list_v1.py` & `seeq-65.0.2/seeq/sdk/models/add_on_output_list_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/add_on_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/add_on_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/add_on_preview_output_list_v1.py` & `seeq-65.0.2/seeq/sdk/models/add_on_preview_output_list_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/add_on_preview_v1.py` & `seeq-65.0.2/seeq/sdk/models/add_on_preview_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/add_on_tool_input_v1.py` & `seeq-65.0.2/seeq/sdk/models/add_on_tool_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/add_on_tool_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/add_on_tool_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/administrator_contact_information_v1.py` & `seeq-65.0.2/seeq/sdk/models/administrator_contact_information_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/agent_input_v1.py` & `seeq-65.0.2/seeq/sdk/models/agent_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/agent_key_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/agent_key_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/agent_orchestrator_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/agent_orchestrator_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/agent_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/agent_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/agent_status_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/agent_status_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/agent_status_v1.py` & `seeq-65.0.2/seeq/sdk/models/agent_status_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/annotation_image_link_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/annotation_image_link_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/annotation_input_v1.py` & `seeq-65.0.2/seeq/sdk/models/annotation_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/annotation_interest_input_v1.py` & `seeq-65.0.2/seeq/sdk/models/annotation_interest_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/annotation_interest_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/annotation_interest_output_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/annotation_list_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/annotation_list_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/annotation_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/annotation_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/archive_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/archive_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/asset_batch_input_v1.py` & `seeq-65.0.2/seeq/sdk/models/asset_batch_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/asset_error.py` & `seeq-65.0.2/seeq/sdk/models/asset_error.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/asset_group_asset_input_v1.py` & `seeq-65.0.2/seeq/sdk/models/asset_group_asset_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/asset_group_input_v1.py` & `seeq-65.0.2/seeq/sdk/models/asset_group_input_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/asset_group_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/asset_group_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/asset_group_root_input_v1.py` & `seeq-65.0.2/seeq/sdk/models/asset_group_root_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/asset_group_tree_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/asset_group_tree_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/asset_input_v1.py` & `seeq-65.0.2/seeq/sdk/models/asset_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/asset_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/asset_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/asset_selection_input_v1.py` & `seeq-65.0.2/seeq/sdk/models/asset_selection_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/asset_selection_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/asset_selection_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/asset_tree_batch_input_v1.py` & `seeq-65.0.2/seeq/sdk/models/asset_tree_batch_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/asset_tree_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/asset_tree_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/asset_tree_single_input_v1.py` & `seeq-65.0.2/seeq/sdk/models/asset_tree_single_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/attachment_input_v1.py` & `seeq-65.0.2/seeq/sdk/models/attachment_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/audit_output_list_v1.py` & `seeq-65.0.2/seeq/sdk/models/audit_output_list_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/audit_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/audit_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/auth_input_v1.py` & `seeq-65.0.2/seeq/sdk/models/auth_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/auth_providers_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/auth_providers_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/authoritative_region_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/authoritative_region_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/boolean_configuration_field_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/boolean_configuration_field_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/cache_block.py` & `seeq-65.0.2/seeq/sdk/models/cache_block.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/cache_info_v1.py` & `seeq-65.0.2/seeq/sdk/models/cache_info_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/calculated_item_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/calculated_item_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/capsule_input_v1.py` & `seeq-65.0.2/seeq/sdk/models/capsule_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/capsule_property_input_v1.py` & `seeq-65.0.2/seeq/sdk/models/capsule_property_input_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/capsule_property_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/capsule_property_output_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/capsule_v1.py` & `seeq-65.0.2/seeq/sdk/models/capsule_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/capsules_input_v1.py` & `seeq-65.0.2/seeq/sdk/models/capsules_input_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/capsules_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/capsules_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/capsules_overwrite_input_v1.py` & `seeq-65.0.2/seeq/sdk/models/capsules_overwrite_input_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/channel_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/channel_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/column_definition_input_list_v1.py` & `seeq-65.0.2/seeq/sdk/models/column_definition_input_list_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/column_definition_input_v1.py` & `seeq-65.0.2/seeq/sdk/models/column_definition_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/column_definition_order_input_v1.py` & `seeq-65.0.2/seeq/sdk/models/column_definition_order_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/column_definition_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/column_definition_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/column_rule_ancestor_input_v1.py` & `seeq-65.0.2/seeq/sdk/models/column_rule_ancestor_input_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/column_rule_asset_creator_input_v1.py` & `seeq-65.0.2/seeq/sdk/models/column_rule_asset_creator_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/column_rule_concat_input_v1.py` & `seeq-65.0.2/seeq/sdk/models/column_rule_concat_input_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/column_rule_constant_input_v1.py` & `seeq-65.0.2/seeq/sdk/models/column_rule_constant_input_v1.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/column_rule_descendant_input_v1.py` & `seeq-65.0.2/seeq/sdk/models/column_rule_descendant_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/column_rule_event_property_input_v1.py` & `seeq-65.0.2/seeq/sdk/models/column_rule_event_property_input_v1.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/column_rule_formula_creator_input_v1.py` & `seeq-65.0.2/seeq/sdk/models/column_rule_formula_creator_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/column_rule_input_v1.py` & `seeq-65.0.2/seeq/sdk/models/column_rule_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/column_rule_item_property_input_v1.py` & `seeq-65.0.2/seeq/sdk/models/column_rule_item_property_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/column_rule_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/column_rule_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/column_rule_path_input_v1.py` & `seeq-65.0.2/seeq/sdk/models/column_rule_path_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/column_rule_tree_path_creator_input_v1.py` & `seeq-65.0.2/seeq/sdk/models/column_rule_tree_path_creator_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/condition_batch_input_v1.py` & `seeq-65.0.2/seeq/sdk/models/condition_batch_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/condition_input_v1.py` & `seeq-65.0.2/seeq/sdk/models/condition_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/condition_monitor_input_v1.py` & `seeq-65.0.2/seeq/sdk/models/condition_monitor_input_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
@@ -30,18 +30,18 @@
                             and the value is json key in definition.
     """
     swagger_types = {
         'condition_ids': 'list[str]',
         'cron_schedule': 'list[str]',
         'description': 'str',
         'enabled': 'bool',
-        'first_run_look_back': 'str',
+        'first_run_look_back': 'int',
         'item_finder_id': 'str',
         'name': 'str',
-        'query_range_look_ahead': 'str',
+        'query_range_look_ahead': 'int',
         'timezone': 'str',
         'webhook_url': 'str'
     }
 
     attribute_map = {
         'condition_ids': 'conditionIds',
         'cron_schedule': 'cronSchedule',
@@ -189,26 +189,26 @@
     @property
     def first_run_look_back(self):
         """
         Gets the first_run_look_back of this ConditionMonitorInputV1.
         On first run, how far to look back for capsules, in seconds
 
         :return: The first_run_look_back of this ConditionMonitorInputV1.
-        :rtype: str
+        :rtype: int
         """
         return self._first_run_look_back
 
     @first_run_look_back.setter
     def first_run_look_back(self, first_run_look_back):
         """
         Sets the first_run_look_back of this ConditionMonitorInputV1.
         On first run, how far to look back for capsules, in seconds
 
         :param first_run_look_back: The first_run_look_back of this ConditionMonitorInputV1.
-        :type: str
+        :type: int
         """
 
         self._first_run_look_back = first_run_look_back
 
     @property
     def item_finder_id(self):
         """
@@ -260,26 +260,26 @@
     @property
     def query_range_look_ahead(self):
         """
         Gets the query_range_look_ahead of this ConditionMonitorInputV1.
         Query range look ahead in seconds
 
         :return: The query_range_look_ahead of this ConditionMonitorInputV1.
-        :rtype: str
+        :rtype: int
         """
         return self._query_range_look_ahead
 
     @query_range_look_ahead.setter
     def query_range_look_ahead(self, query_range_look_ahead):
         """
         Sets the query_range_look_ahead of this ConditionMonitorInputV1.
         Query range look ahead in seconds
 
         :param query_range_look_ahead: The query_range_look_ahead of this ConditionMonitorInputV1.
-        :type: str
+        :type: int
         """
 
         self._query_range_look_ahead = query_range_look_ahead
 
     @property
     def timezone(self):
         """
```

### Comparing `seeq-65.0.1/seeq/sdk/models/condition_monitor_notification_configuration_input_v1.py` & `seeq-65.0.2/seeq/sdk/models/condition_monitor_notification_configuration_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/condition_monitor_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/condition_monitor_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
@@ -35,21 +35,21 @@
         'creator': 'IdentityPreviewV1',
         'cron_schedule': 'list[str]',
         'cron_schedule_description': 'str',
         'description': 'str',
         'effective_permissions': 'PermissionsV1',
         'enabled': 'bool',
         'executor_id': 'str',
-        'first_run_look_back': 'str',
+        'first_run_look_back': 'int',
         'id': 'str',
         'is_archived': 'bool',
         'is_redacted': 'bool',
         'item_finder_id': 'str',
         'name': 'str',
-        'query_range_look_ahead': 'str',
+        'query_range_look_ahead': 'int',
         'status_message': 'str',
         'timezone': 'str',
         'translation_key': 'str',
         'type': 'str',
         'updated_at': 'str',
         'webhook_url': 'str'
     }
@@ -366,26 +366,26 @@
     @property
     def first_run_look_back(self):
         """
         Gets the first_run_look_back of this ConditionMonitorOutputV1.
         On first run, how far to look back for capsules, in seconds
 
         :return: The first_run_look_back of this ConditionMonitorOutputV1.
-        :rtype: str
+        :rtype: int
         """
         return self._first_run_look_back
 
     @first_run_look_back.setter
     def first_run_look_back(self, first_run_look_back):
         """
         Sets the first_run_look_back of this ConditionMonitorOutputV1.
         On first run, how far to look back for capsules, in seconds
 
         :param first_run_look_back: The first_run_look_back of this ConditionMonitorOutputV1.
-        :type: str
+        :type: int
         """
 
         self._first_run_look_back = first_run_look_back
 
     @property
     def id(self):
         """
@@ -508,26 +508,26 @@
     @property
     def query_range_look_ahead(self):
         """
         Gets the query_range_look_ahead of this ConditionMonitorOutputV1.
         Query range look ahead in seconds
 
         :return: The query_range_look_ahead of this ConditionMonitorOutputV1.
-        :rtype: str
+        :rtype: int
         """
         return self._query_range_look_ahead
 
     @query_range_look_ahead.setter
     def query_range_look_ahead(self, query_range_look_ahead):
         """
         Sets the query_range_look_ahead of this ConditionMonitorOutputV1.
         Query range look ahead in seconds
 
         :param query_range_look_ahead: The query_range_look_ahead of this ConditionMonitorOutputV1.
-        :type: str
+        :type: int
         """
         if query_range_look_ahead is None:
             raise ValueError("Invalid value for `query_range_look_ahead`, must not be `None`")
 
         self._query_range_look_ahead = query_range_look_ahead
 
     @property
```

### Comparing `seeq-65.0.1/seeq/sdk/models/condition_notification_output_list_v1.py` & `seeq-65.0.2/seeq/sdk/models/condition_notification_output_list_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/condition_notification_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/condition_notification_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/condition_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/condition_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/condition_update_input_v1.py` & `seeq-65.0.2/seeq/sdk/models/condition_update_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/configuration_field_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/configuration_field_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/configuration_input_v1.py` & `seeq-65.0.2/seeq/sdk/models/configuration_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/configuration_option_input_v1.py` & `seeq-65.0.2/seeq/sdk/models/configuration_option_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/configuration_option_output_simple_v1.py` & `seeq-65.0.2/seeq/sdk/models/configuration_option_output_simple_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/configuration_option_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/configuration_option_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/configuration_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/configuration_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/configured_directives_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/configured_directives_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/connection_input_v1.py` & `seeq-65.0.2/seeq/sdk/models/connection_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/connection_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/connection_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/connection_status_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/connection_status_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/connection_status_v1.py` & `seeq-65.0.2/seeq/sdk/models/connection_status_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/connections_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/connections_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/connector_input_v1.py` & `seeq-65.0.2/seeq/sdk/models/connector_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/connector_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/connector_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/connectors_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/connectors_output_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/content_input_v1.py` & `seeq-65.0.2/seeq/sdk/models/content_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/content_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/content_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/content_with_metadata_list_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/content_with_metadata_list_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/content_with_metadata_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/content_with_metadata_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/context_comment_input_v1.py` & `seeq-65.0.2/seeq/sdk/models/context_comment_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/context_comment_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/context_comment_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/context_label_input_v1.py` & `seeq-65.0.2/seeq/sdk/models/context_label_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/context_label_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/context_label_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/context_opaque_input_v1.py` & `seeq-65.0.2/seeq/sdk/models/context_opaque_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/context_opaque_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/context_opaque_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/csv_datafile_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/csv_datafile_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/datafile_input_v1.py` & `seeq-65.0.2/seeq/sdk/models/datafile_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/datafile_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/datafile_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/datafiles_csv_body.py` & `seeq-65.0.2/seeq/sdk/models/datafiles_csv_body.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/datasource_clean_up_input_v1.py` & `seeq-65.0.2/seeq/sdk/models/datasource_clean_up_input_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/datasource_clean_up_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/datasource_clean_up_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/datasource_input_v1.py` & `seeq-65.0.2/seeq/sdk/models/datasource_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/datasource_output_list_v1.py` & `seeq-65.0.2/seeq/sdk/models/datasource_output_list_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/datasource_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/datasource_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/datasource_preview_v1.py` & `seeq-65.0.2/seeq/sdk/models/datasource_preview_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/datasource_statistics_v1.py` & `seeq-65.0.2/seeq/sdk/models/datasource_statistics_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/datasource_status_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/datasource_status_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/datasource_status_v1.py` & `seeq-65.0.2/seeq/sdk/models/datasource_status_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/datasource_summary_status_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/datasource_summary_status_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/datasources_status_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/datasources_status_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/date_range_input_v1.py` & `seeq-65.0.2/seeq/sdk/models/date_range_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/date_range_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/date_range_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/debug_cache_block_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/debug_cache_block_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/detailed_meter_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/detailed_meter_output_v1.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/detailed_timer_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/detailed_timer_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/directive_input_v1.py` & `seeq-65.0.2/seeq/sdk/models/directive_input_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/display_input_v1.py` & `seeq-65.0.2/seeq/sdk/models/display_input_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/display_output_list_v1.py` & `seeq-65.0.2/seeq/sdk/models/display_output_list_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/display_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/display_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/display_template_input_v1.py` & `seeq-65.0.2/seeq/sdk/models/display_template_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/display_template_output_list_v1.py` & `seeq-65.0.2/seeq/sdk/models/display_template_output_list_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/display_template_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/display_template_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/document_backup_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/document_backup_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/double_configuration_field_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/double_configuration_field_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/email_notification_recipient_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/email_notification_recipient_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/emailer_configuration_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/emailer_configuration_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/export_item_v1.py` & `seeq-65.0.2/seeq/sdk/models/export_item_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/export_items_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/export_items_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/export_items_v1.py` & `seeq-65.0.2/seeq/sdk/models/export_items_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/export_preview_list_v1.py` & `seeq-65.0.2/seeq/sdk/models/export_preview_list_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/export_preview_v1.py` & `seeq-65.0.2/seeq/sdk/models/export_preview_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/fixed_list_search_v1.py` & `seeq-65.0.2/seeq/sdk/models/fixed_list_search_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/folded_stack_node_v1.py` & `seeq-65.0.2/seeq/sdk/models/folded_stack_node_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/folder_input_v1.py` & `seeq-65.0.2/seeq/sdk/models/folder_input_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/folder_navigation_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/folder_navigation_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/folder_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/folder_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/formula_compile_input_v1.py` & `seeq-65.0.2/seeq/sdk/models/formula_compile_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/formula_compile_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/formula_compile_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/formula_compiler_error_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/formula_compiler_error_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/formula_dependency_input_v1.py` & `seeq-65.0.2/seeq/sdk/models/formula_dependency_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/formula_doc_example_input_v1.py` & `seeq-65.0.2/seeq/sdk/models/formula_doc_example_input_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/formula_doc_example_list_input_v1.py` & `seeq-65.0.2/seeq/sdk/models/formula_doc_example_list_input_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/formula_doc_input_v1.py` & `seeq-65.0.2/seeq/sdk/models/formula_doc_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/formula_doc_keyword_list_input_v1.py` & `seeq-65.0.2/seeq/sdk/models/formula_doc_keyword_list_input_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/formula_doc_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/formula_doc_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/formula_doc_summaries_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/formula_doc_summaries_output_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/formula_doc_summary_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/formula_doc_summary_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/formula_error_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/formula_error_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/formula_example_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/formula_example_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/formula_item_input_v1.py` & `seeq-65.0.2/seeq/sdk/models/formula_item_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/formula_item_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/formula_item_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/formula_log_entry.py` & `seeq-65.0.2/seeq/sdk/models/formula_log_entry.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/formula_log_entry_details.py` & `seeq-65.0.2/seeq/sdk/models/formula_log_entry_details.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/formula_log_v1.py` & `seeq-65.0.2/seeq/sdk/models/formula_log_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/formula_package_import_input_v1.py` & `seeq-65.0.2/seeq/sdk/models/formula_package_import_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/formula_package_import_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/formula_package_import_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/formula_package_input_v1.py` & `seeq-65.0.2/seeq/sdk/models/formula_package_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/formula_package_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/formula_package_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/formula_parameter_input_v1.py` & `seeq-65.0.2/seeq/sdk/models/formula_parameter_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/formula_parameter_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/formula_parameter_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/formula_run_input_v1.py` & `seeq-65.0.2/seeq/sdk/models/formula_run_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/formula_run_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/formula_run_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/formula_token.py` & `seeq-65.0.2/seeq/sdk/models/formula_token.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/formula_update_input_v1.py` & `seeq-65.0.2/seeq/sdk/models/formula_update_input_v1.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/formula_upgrade_change_v1.py` & `seeq-65.0.2/seeq/sdk/models/formula_upgrade_change_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/formula_upgrade_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/formula_upgrade_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/function_input_v1.py` & `seeq-65.0.2/seeq/sdk/models/function_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/function_parameter_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/function_parameter_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/function_variant_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/function_variant_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/gauge_datum_v1.py` & `seeq-65.0.2/seeq/sdk/models/gauge_datum_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/generic_table_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/generic_table_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/get_add_on_tools_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/get_add_on_tools_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/get_channels_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/get_channels_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/get_condition_monitor_items_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/get_condition_monitor_items_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/get_content_items_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/get_content_items_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/get_date_ranges_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/get_date_ranges_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/get_jobs_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/get_jobs_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/get_metrics_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/get_metrics_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/get_projects_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/get_projects_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/get_request_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/get_request_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/get_requests_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/get_requests_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/get_sample_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/get_sample_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/get_samples_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/get_samples_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/get_signals_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/get_signals_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/graph_ql_input_v1.py` & `seeq-65.0.2/seeq/sdk/models/graph_ql_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/graph_ql_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/graph_ql_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/id_images_body.py` & `seeq-65.0.2/seeq/sdk/models/id_images_body.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/identity_mapping_list_v1.py` & `seeq-65.0.2/seeq/sdk/models/identity_mapping_list_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/identity_mapping_v1.py` & `seeq-65.0.2/seeq/sdk/models/identity_mapping_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/identity_preview_list_v1.py` & `seeq-65.0.2/seeq/sdk/models/identity_preview_list_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/identity_preview_v1.py` & `seeq-65.0.2/seeq/sdk/models/identity_preview_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/indexing_parameters_input_v1.py` & `seeq-65.0.2/seeq/sdk/models/indexing_parameters_input_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/installer_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/installer_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/interval_v1.py` & `seeq-65.0.2/seeq/sdk/models/interval_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/invalid_swap_out_v1.py` & `seeq-65.0.2/seeq/sdk/models/invalid_swap_out_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/item_batch_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/item_batch_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/item_dependency_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/item_dependency_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/item_finder_input_v1.py` & `seeq-65.0.2/seeq/sdk/models/item_finder_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/item_finder_output_list_v1.py` & `seeq-65.0.2/seeq/sdk/models/item_finder_output_list_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/item_finder_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/report_template_output_v1.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,511 +1,477 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
 
 
-class ItemFinderOutputV1(object):
+class ReportTemplateOutputV1(object):
     """
     NOTE: This class is auto generated by the swagger code generator program.
     Do not edit the class manually.
     """
 
 
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'cron_schedule': 'list[str]',
+        'created_at': 'str',
+        'creator': 'IdentityPreviewV1',
         'description': 'str',
         'effective_permissions': 'PermissionsV1',
-        'enabled': 'bool',
-        'executor_id': 'str',
+        'html_template': 'str',
         'id': 'str',
         'is_archived': 'bool',
         'is_redacted': 'bool',
-        'last_run_warnings': 'list[str]',
         'name': 'str',
-        'scoped_to': 'str',
-        'searches': 'list[object]',
+        'owner': 'IdentityPreviewV1',
+        'parent_folder_id': 'str',
         'status_message': 'str',
-        'timezone': 'str',
         'translation_key': 'str',
-        'type': 'str'
+        'type': 'str',
+        'updated_at': 'str'
     }
 
     attribute_map = {
-        'cron_schedule': 'cronSchedule',
+        'created_at': 'createdAt',
+        'creator': 'creator',
         'description': 'description',
         'effective_permissions': 'effectivePermissions',
-        'enabled': 'enabled',
-        'executor_id': 'executorId',
+        'html_template': 'htmlTemplate',
         'id': 'id',
         'is_archived': 'isArchived',
         'is_redacted': 'isRedacted',
-        'last_run_warnings': 'lastRunWarnings',
         'name': 'name',
-        'scoped_to': 'scopedTo',
-        'searches': 'searches',
+        'owner': 'owner',
+        'parent_folder_id': 'parentFolderId',
         'status_message': 'statusMessage',
-        'timezone': 'timezone',
         'translation_key': 'translationKey',
-        'type': 'type'
+        'type': 'type',
+        'updated_at': 'updatedAt'
     }
 
-    def __init__(self, cron_schedule=None, description=None, effective_permissions=None, enabled=None, executor_id=None, id=None, is_archived=False, is_redacted=False, last_run_warnings=None, name=None, scoped_to=None, searches=None, status_message=None, timezone=None, translation_key=None, type=None):
+    def __init__(self, created_at=None, creator=None, description=None, effective_permissions=None, html_template=None, id=None, is_archived=False, is_redacted=False, name=None, owner=None, parent_folder_id=None, status_message=None, translation_key=None, type=None, updated_at=None):
         """
-        ItemFinderOutputV1 - a model defined in Swagger
+        ReportTemplateOutputV1 - a model defined in Swagger
         """
 
-        self._cron_schedule = None
+        self._created_at = None
+        self._creator = None
         self._description = None
         self._effective_permissions = None
-        self._enabled = None
-        self._executor_id = None
+        self._html_template = None
         self._id = None
         self._is_archived = None
         self._is_redacted = None
-        self._last_run_warnings = None
         self._name = None
-        self._scoped_to = None
-        self._searches = None
+        self._owner = None
+        self._parent_folder_id = None
         self._status_message = None
-        self._timezone = None
         self._translation_key = None
         self._type = None
+        self._updated_at = None
 
-        if cron_schedule is not None:
-          self.cron_schedule = cron_schedule
+        if created_at is not None:
+          self.created_at = created_at
+        if creator is not None:
+          self.creator = creator
         if description is not None:
           self.description = description
         if effective_permissions is not None:
           self.effective_permissions = effective_permissions
-        if enabled is not None:
-          self.enabled = enabled
-        if executor_id is not None:
-          self.executor_id = executor_id
+        if html_template is not None:
+          self.html_template = html_template
         if id is not None:
           self.id = id
         if is_archived is not None:
           self.is_archived = is_archived
         if is_redacted is not None:
           self.is_redacted = is_redacted
-        if last_run_warnings is not None:
-          self.last_run_warnings = last_run_warnings
         if name is not None:
           self.name = name
-        if scoped_to is not None:
-          self.scoped_to = scoped_to
-        if searches is not None:
-          self.searches = searches
+        if owner is not None:
+          self.owner = owner
+        if parent_folder_id is not None:
+          self.parent_folder_id = parent_folder_id
         if status_message is not None:
           self.status_message = status_message
-        if timezone is not None:
-          self.timezone = timezone
         if translation_key is not None:
           self.translation_key = translation_key
         if type is not None:
           self.type = type
+        if updated_at is not None:
+          self.updated_at = updated_at
 
     @property
-    def cron_schedule(self):
+    def created_at(self):
         """
-        Gets the cron_schedule of this ItemFinderOutputV1.
-        The item finder's check interval(s) as a list of cron expressions (see https://www.quartz-scheduler.org/documentation/quartz-2.3.0/tutorials/crontrigger.html)
+        Gets the created_at of this ReportTemplateOutputV1.
+        The time the template was created at
 
-        :return: The cron_schedule of this ItemFinderOutputV1.
-        :rtype: list[str]
+        :return: The created_at of this ReportTemplateOutputV1.
+        :rtype: str
+        """
+        return self._created_at
+
+    @created_at.setter
+    def created_at(self, created_at):
+        """
+        Sets the created_at of this ReportTemplateOutputV1.
+        The time the template was created at
+
+        :param created_at: The created_at of this ReportTemplateOutputV1.
+        :type: str
+        """
+        if created_at is None:
+            raise ValueError("Invalid value for `created_at`, must not be `None`")
+
+        self._created_at = created_at
+
+    @property
+    def creator(self):
+        """
+        Gets the creator of this ReportTemplateOutputV1.
+
+        :return: The creator of this ReportTemplateOutputV1.
+        :rtype: IdentityPreviewV1
         """
-        return self._cron_schedule
+        return self._creator
 
-    @cron_schedule.setter
-    def cron_schedule(self, cron_schedule):
+    @creator.setter
+    def creator(self, creator):
         """
-        Sets the cron_schedule of this ItemFinderOutputV1.
-        The item finder's check interval(s) as a list of cron expressions (see https://www.quartz-scheduler.org/documentation/quartz-2.3.0/tutorials/crontrigger.html)
+        Sets the creator of this ReportTemplateOutputV1.
 
-        :param cron_schedule: The cron_schedule of this ItemFinderOutputV1.
-        :type: list[str]
+        :param creator: The creator of this ReportTemplateOutputV1.
+        :type: IdentityPreviewV1
         """
 
-        self._cron_schedule = cron_schedule
+        self._creator = creator
 
     @property
     def description(self):
         """
-        Gets the description of this ItemFinderOutputV1.
+        Gets the description of this ReportTemplateOutputV1.
         Clarifying information or other plain language description of this item
 
-        :return: The description of this ItemFinderOutputV1.
+        :return: The description of this ReportTemplateOutputV1.
         :rtype: str
         """
         return self._description
 
     @description.setter
     def description(self, description):
         """
-        Sets the description of this ItemFinderOutputV1.
+        Sets the description of this ReportTemplateOutputV1.
         Clarifying information or other plain language description of this item
 
-        :param description: The description of this ItemFinderOutputV1.
+        :param description: The description of this ReportTemplateOutputV1.
         :type: str
         """
 
         self._description = description
 
     @property
     def effective_permissions(self):
         """
-        Gets the effective_permissions of this ItemFinderOutputV1.
+        Gets the effective_permissions of this ReportTemplateOutputV1.
 
-        :return: The effective_permissions of this ItemFinderOutputV1.
+        :return: The effective_permissions of this ReportTemplateOutputV1.
         :rtype: PermissionsV1
         """
         return self._effective_permissions
 
     @effective_permissions.setter
     def effective_permissions(self, effective_permissions):
         """
-        Sets the effective_permissions of this ItemFinderOutputV1.
+        Sets the effective_permissions of this ReportTemplateOutputV1.
 
-        :param effective_permissions: The effective_permissions of this ItemFinderOutputV1.
+        :param effective_permissions: The effective_permissions of this ReportTemplateOutputV1.
         :type: PermissionsV1
         """
 
         self._effective_permissions = effective_permissions
 
     @property
-    def enabled(self):
+    def html_template(self):
         """
-        Gets the enabled of this ItemFinderOutputV1.
-        Whether this item finder is enabled or not
+        Gets the html_template of this ReportTemplateOutputV1.
+        The html template itself
 
-        :return: The enabled of this ItemFinderOutputV1.
-        :rtype: bool
-        """
-        return self._enabled
-
-    @enabled.setter
-    def enabled(self, enabled):
-        """
-        Sets the enabled of this ItemFinderOutputV1.
-        Whether this item finder is enabled or not
-
-        :param enabled: The enabled of this ItemFinderOutputV1.
-        :type: bool
-        """
-        if enabled is None:
-            raise ValueError("Invalid value for `enabled`, must not be `None`")
-
-        self._enabled = enabled
-
-    @property
-    def executor_id(self):
-        """
-        Gets the executor_id of this ItemFinderOutputV1.
-        The ID of the user that runs the job of finding the items. The permissions of this user will be used to determine what items can be read.
-
-        :return: The executor_id of this ItemFinderOutputV1.
+        :return: The html_template of this ReportTemplateOutputV1.
         :rtype: str
         """
-        return self._executor_id
+        return self._html_template
 
-    @executor_id.setter
-    def executor_id(self, executor_id):
+    @html_template.setter
+    def html_template(self, html_template):
         """
-        Sets the executor_id of this ItemFinderOutputV1.
-        The ID of the user that runs the job of finding the items. The permissions of this user will be used to determine what items can be read.
+        Sets the html_template of this ReportTemplateOutputV1.
+        The html template itself
 
-        :param executor_id: The executor_id of this ItemFinderOutputV1.
+        :param html_template: The html_template of this ReportTemplateOutputV1.
         :type: str
         """
-        if executor_id is None:
-            raise ValueError("Invalid value for `executor_id`, must not be `None`")
+        if html_template is None:
+            raise ValueError("Invalid value for `html_template`, must not be `None`")
 
-        self._executor_id = executor_id
+        self._html_template = html_template
 
     @property
     def id(self):
         """
-        Gets the id of this ItemFinderOutputV1.
+        Gets the id of this ReportTemplateOutputV1.
         The ID that can be used to interact with the item
 
-        :return: The id of this ItemFinderOutputV1.
+        :return: The id of this ReportTemplateOutputV1.
         :rtype: str
         """
         return self._id
 
     @id.setter
     def id(self, id):
         """
-        Sets the id of this ItemFinderOutputV1.
+        Sets the id of this ReportTemplateOutputV1.
         The ID that can be used to interact with the item
 
-        :param id: The id of this ItemFinderOutputV1.
+        :param id: The id of this ReportTemplateOutputV1.
         :type: str
         """
         if id is None:
             raise ValueError("Invalid value for `id`, must not be `None`")
 
         self._id = id
 
     @property
     def is_archived(self):
         """
-        Gets the is_archived of this ItemFinderOutputV1.
+        Gets the is_archived of this ReportTemplateOutputV1.
         Whether item is archived
 
-        :return: The is_archived of this ItemFinderOutputV1.
+        :return: The is_archived of this ReportTemplateOutputV1.
         :rtype: bool
         """
         return self._is_archived
 
     @is_archived.setter
     def is_archived(self, is_archived):
         """
-        Sets the is_archived of this ItemFinderOutputV1.
+        Sets the is_archived of this ReportTemplateOutputV1.
         Whether item is archived
 
-        :param is_archived: The is_archived of this ItemFinderOutputV1.
+        :param is_archived: The is_archived of this ReportTemplateOutputV1.
         :type: bool
         """
 
         self._is_archived = is_archived
 
     @property
     def is_redacted(self):
         """
-        Gets the is_redacted of this ItemFinderOutputV1.
+        Gets the is_redacted of this ReportTemplateOutputV1.
         Whether item is redacted
 
-        :return: The is_redacted of this ItemFinderOutputV1.
+        :return: The is_redacted of this ReportTemplateOutputV1.
         :rtype: bool
         """
         return self._is_redacted
 
     @is_redacted.setter
     def is_redacted(self, is_redacted):
         """
-        Sets the is_redacted of this ItemFinderOutputV1.
+        Sets the is_redacted of this ReportTemplateOutputV1.
         Whether item is redacted
 
-        :param is_redacted: The is_redacted of this ItemFinderOutputV1.
+        :param is_redacted: The is_redacted of this ReportTemplateOutputV1.
         :type: bool
         """
 
         self._is_redacted = is_redacted
 
     @property
-    def last_run_warnings(self):
-        """
-        Gets the last_run_warnings of this ItemFinderOutputV1.
-        The most recent list of warnings or errors that resulted from evaluating any of the finder configurations, such as items that failed to swap
-
-        :return: The last_run_warnings of this ItemFinderOutputV1.
-        :rtype: list[str]
-        """
-        return self._last_run_warnings
-
-    @last_run_warnings.setter
-    def last_run_warnings(self, last_run_warnings):
-        """
-        Sets the last_run_warnings of this ItemFinderOutputV1.
-        The most recent list of warnings or errors that resulted from evaluating any of the finder configurations, such as items that failed to swap
-
-        :param last_run_warnings: The last_run_warnings of this ItemFinderOutputV1.
-        :type: list[str]
-        """
-        if last_run_warnings is None:
-            raise ValueError("Invalid value for `last_run_warnings`, must not be `None`")
-
-        self._last_run_warnings = last_run_warnings
-
-    @property
     def name(self):
         """
-        Gets the name of this ItemFinderOutputV1.
+        Gets the name of this ReportTemplateOutputV1.
         The human readable name
 
-        :return: The name of this ItemFinderOutputV1.
+        :return: The name of this ReportTemplateOutputV1.
         :rtype: str
         """
         return self._name
 
     @name.setter
     def name(self, name):
         """
-        Sets the name of this ItemFinderOutputV1.
+        Sets the name of this ReportTemplateOutputV1.
         The human readable name
 
-        :param name: The name of this ItemFinderOutputV1.
+        :param name: The name of this ReportTemplateOutputV1.
         :type: str
         """
         if name is None:
             raise ValueError("Invalid value for `name`, must not be `None`")
 
         self._name = name
 
     @property
-    def scoped_to(self):
+    def owner(self):
         """
-        Gets the scoped_to of this ItemFinderOutputV1.
-        The ID of the workbook to which this item is scoped or null if it is in the global scope.
+        Gets the owner of this ReportTemplateOutputV1.
 
-        :return: The scoped_to of this ItemFinderOutputV1.
-        :rtype: str
+        :return: The owner of this ReportTemplateOutputV1.
+        :rtype: IdentityPreviewV1
         """
-        return self._scoped_to
+        return self._owner
 
-    @scoped_to.setter
-    def scoped_to(self, scoped_to):
+    @owner.setter
+    def owner(self, owner):
         """
-        Sets the scoped_to of this ItemFinderOutputV1.
-        The ID of the workbook to which this item is scoped or null if it is in the global scope.
+        Sets the owner of this ReportTemplateOutputV1.
 
-        :param scoped_to: The scoped_to of this ItemFinderOutputV1.
-        :type: str
+        :param owner: The owner of this ReportTemplateOutputV1.
+        :type: IdentityPreviewV1
         """
 
-        self._scoped_to = scoped_to
+        self._owner = owner
 
     @property
-    def searches(self):
+    def parent_folder_id(self):
         """
-        Gets the searches of this ItemFinderOutputV1.
-        The list of configurations for finding items
+        Gets the parent_folder_id of this ReportTemplateOutputV1.
+        The ID of the parent folder which this folder, analysis, topic, or project is a subfolder of
 
-        :return: The searches of this ItemFinderOutputV1.
-        :rtype: list[object]
+        :return: The parent_folder_id of this ReportTemplateOutputV1.
+        :rtype: str
         """
-        return self._searches
+        return self._parent_folder_id
 
-    @searches.setter
-    def searches(self, searches):
+    @parent_folder_id.setter
+    def parent_folder_id(self, parent_folder_id):
         """
-        Sets the searches of this ItemFinderOutputV1.
-        The list of configurations for finding items
+        Sets the parent_folder_id of this ReportTemplateOutputV1.
+        The ID of the parent folder which this folder, analysis, topic, or project is a subfolder of
 
-        :param searches: The searches of this ItemFinderOutputV1.
-        :type: list[object]
+        :param parent_folder_id: The parent_folder_id of this ReportTemplateOutputV1.
+        :type: str
         """
-        if searches is None:
-            raise ValueError("Invalid value for `searches`, must not be `None`")
 
-        self._searches = searches
+        self._parent_folder_id = parent_folder_id
 
     @property
     def status_message(self):
         """
-        Gets the status_message of this ItemFinderOutputV1.
+        Gets the status_message of this ReportTemplateOutputV1.
         A plain language status message with information about any issues that may have been encountered during an operation
 
-        :return: The status_message of this ItemFinderOutputV1.
+        :return: The status_message of this ReportTemplateOutputV1.
         :rtype: str
         """
         return self._status_message
 
     @status_message.setter
     def status_message(self, status_message):
         """
-        Sets the status_message of this ItemFinderOutputV1.
+        Sets the status_message of this ReportTemplateOutputV1.
         A plain language status message with information about any issues that may have been encountered during an operation
 
-        :param status_message: The status_message of this ItemFinderOutputV1.
+        :param status_message: The status_message of this ReportTemplateOutputV1.
         :type: str
         """
 
         self._status_message = status_message
 
     @property
-    def timezone(self):
-        """
-        Gets the timezone of this ItemFinderOutputV1.
-        The IANA timezone in which the schedule will be run, defaults to UTC
-
-        :return: The timezone of this ItemFinderOutputV1.
-        :rtype: str
-        """
-        return self._timezone
-
-    @timezone.setter
-    def timezone(self, timezone):
-        """
-        Sets the timezone of this ItemFinderOutputV1.
-        The IANA timezone in which the schedule will be run, defaults to UTC
-
-        :param timezone: The timezone of this ItemFinderOutputV1.
-        :type: str
-        """
-
-        self._timezone = timezone
-
-    @property
     def translation_key(self):
         """
-        Gets the translation_key of this ItemFinderOutputV1.
+        Gets the translation_key of this ReportTemplateOutputV1.
         The item's translation key, if any
 
-        :return: The translation_key of this ItemFinderOutputV1.
+        :return: The translation_key of this ReportTemplateOutputV1.
         :rtype: str
         """
         return self._translation_key
 
     @translation_key.setter
     def translation_key(self, translation_key):
         """
-        Sets the translation_key of this ItemFinderOutputV1.
+        Sets the translation_key of this ReportTemplateOutputV1.
         The item's translation key, if any
 
-        :param translation_key: The translation_key of this ItemFinderOutputV1.
+        :param translation_key: The translation_key of this ReportTemplateOutputV1.
         :type: str
         """
 
         self._translation_key = translation_key
 
     @property
     def type(self):
         """
-        Gets the type of this ItemFinderOutputV1.
+        Gets the type of this ReportTemplateOutputV1.
         The type of the item
 
-        :return: The type of this ItemFinderOutputV1.
+        :return: The type of this ReportTemplateOutputV1.
         :rtype: str
         """
         return self._type
 
     @type.setter
     def type(self, type):
         """
-        Sets the type of this ItemFinderOutputV1.
+        Sets the type of this ReportTemplateOutputV1.
         The type of the item
 
-        :param type: The type of this ItemFinderOutputV1.
+        :param type: The type of this ReportTemplateOutputV1.
         :type: str
         """
         if type is None:
             raise ValueError("Invalid value for `type`, must not be `None`")
 
         self._type = type
 
+    @property
+    def updated_at(self):
+        """
+        Gets the updated_at of this ReportTemplateOutputV1.
+        The last time this template was updated
+
+        :return: The updated_at of this ReportTemplateOutputV1.
+        :rtype: str
+        """
+        return self._updated_at
+
+    @updated_at.setter
+    def updated_at(self, updated_at):
+        """
+        Sets the updated_at of this ReportTemplateOutputV1.
+        The last time this template was updated
+
+        :param updated_at: The updated_at of this ReportTemplateOutputV1.
+        :type: str
+        """
+        if updated_at is None:
+            raise ValueError("Invalid value for `updated_at`, must not be `None`")
+
+        self._updated_at = updated_at
+
     def to_dict(self):
         """
         Returns the model properties as a dict
         """
         result = {}
 
         for attr, _ in iteritems(self.swagger_types):
@@ -540,15 +506,15 @@
         """
         return self.to_str()
 
     def __eq__(self, other):
         """
         Returns true if both objects are equal
         """
-        if not isinstance(other, ItemFinderOutputV1):
+        if not isinstance(other, ReportTemplateOutputV1):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """
         Returns true if both objects are not equal
```

### Comparing `seeq-65.0.1/seeq/sdk/models/item_finder_searches_input_v1.py` & `seeq-65.0.2/seeq/sdk/models/item_finder_searches_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/item_finder_searches_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/item_finder_searches_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/item_id_list_input_v1.py` & `seeq-65.0.2/seeq/sdk/models/item_id_list_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/item_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/item_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/item_parameter_of_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/item_parameter_of_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/item_preview_list_v1.py` & `seeq-65.0.2/seeq/sdk/models/item_preview_list_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/item_preview_v1.py` & `seeq-65.0.2/seeq/sdk/models/item_preview_v1.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/item_preview_with_assets_v1.py` & `seeq-65.0.2/seeq/sdk/models/item_preview_with_assets_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/item_search_preview_list_v1.py` & `seeq-65.0.2/seeq/sdk/models/item_search_preview_list_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/item_search_preview_paginated_list_v1.py` & `seeq-65.0.2/seeq/sdk/models/item_search_preview_paginated_list_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/item_search_preview_v1.py` & `seeq-65.0.2/seeq/sdk/models/item_search_preview_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/item_swap_result_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/item_swap_result_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/item_update_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/item_update_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/item_user_attributes_input_v1.py` & `seeq-65.0.2/seeq/sdk/models/item_user_attributes_input_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/item_user_attributes_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/item_user_attributes_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/item_with_swap_pairs_v1.py` & `seeq-65.0.2/seeq/sdk/models/item_with_swap_pairs_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/jira_attachment.py` & `seeq-65.0.2/seeq/sdk/models/jira_attachment.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/jira_attachment_media_type.py` & `seeq-65.0.2/seeq/sdk/models/jira_attachment_media_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/job_accepted_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/job_accepted_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/job_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/job_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/json_backup_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/json_backup_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/label_category_input_v1.py` & `seeq-65.0.2/seeq/sdk/models/label_category_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/label_category_output_list_v1.py` & `seeq-65.0.2/seeq/sdk/models/label_category_output_list_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/label_category_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/label_category_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/label_input_v1.py` & `seeq-65.0.2/seeq/sdk/models/label_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/label_output_list_v1.py` & `seeq-65.0.2/seeq/sdk/models/label_output_list_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/label_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/label_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/license_importer_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/license_importer_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/license_status_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/license_status_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/licensed_feature_status_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/licensed_feature_status_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/log_message.py` & `seeq-65.0.2/seeq/sdk/models/log_message.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/long_configuration_field_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/long_configuration_field_output_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/meter_datum_v1.py` & `seeq-65.0.2/seeq/sdk/models/meter_datum_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/migrate_editor_input_v1.py` & `seeq-65.0.2/seeq/sdk/models/migrate_editor_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/monitor_definition_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/monitor_definition_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/monitor_definitions_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/monitor_definitions_output_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/monitor_input_v1.py` & `seeq-65.0.2/seeq/sdk/models/monitor_input_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/monitor_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/monitor_output_v1.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/monitor_values.py` & `seeq-65.0.2/seeq/sdk/models/monitor_values.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/monitors_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/monitors_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/notifiable_report_output_list_v1.py` & `seeq-65.0.2/seeq/sdk/models/notifiable_report_output_list_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/notifiable_report_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/notifiable_report_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/notification_configuration_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/notification_configuration_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/optional_report_input_v1.py` & `seeq-65.0.2/seeq/sdk/models/optional_report_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/parameter_doc_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/parameter_doc_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/permissions_v1.py` & `seeq-65.0.2/seeq/sdk/models/permissions_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/plugin_output_list_v1.py` & `seeq-65.0.2/seeq/sdk/models/plugin_output_list_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/plugin_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/plugin_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/plugins_body.py` & `seeq-65.0.2/seeq/sdk/models/plugins_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/pre_provision_input_v1.py` & `seeq-65.0.2/seeq/sdk/models/pre_provision_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/pre_provision_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/pre_provision_output_v1.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/priority_v1.py` & `seeq-65.0.2/seeq/sdk/models/priority_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/progress_information_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/progress_information_output_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/project_input_v1.py` & `seeq-65.0.2/seeq/sdk/models/project_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/project_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/project_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/property_filter_input_v1.py` & `seeq-65.0.2/seeq/sdk/models/property_filter_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/property_href_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/property_href_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/property_input_v1.py` & `seeq-65.0.2/seeq/sdk/models/property_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/property_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/property_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/property_search_v1.py` & `seeq-65.0.2/seeq/sdk/models/property_search_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/provision_input_v1.py` & `seeq-65.0.2/seeq/sdk/models/provision_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/put_asset_input_v1.py` & `seeq-65.0.2/seeq/sdk/models/put_asset_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/put_scalar_input_v1.py` & `seeq-65.0.2/seeq/sdk/models/put_scalar_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/put_scalars_input_v1.py` & `seeq-65.0.2/seeq/sdk/models/put_scalars_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/put_signals_input_v1.py` & `seeq-65.0.2/seeq/sdk/models/put_signals_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/put_user_groups_input_v1.py` & `seeq-65.0.2/seeq/sdk/models/put_user_groups_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/referenced_items_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/referenced_items_output_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/regression_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/regression_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/remote_agent_directives_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/remote_agent_directives_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/remote_agent_status_input_v1.py` & `seeq-65.0.2/seeq/sdk/models/remote_agent_status_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/remote_agent_status_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/remote_agent_status_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/report_input_item_v1.py` & `seeq-65.0.2/seeq/sdk/models/report_input_item_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/report_input_v1.py` & `seeq-65.0.2/seeq/sdk/models/report_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/report_notification_configuration_input_v1.py` & `seeq-65.0.2/seeq/sdk/models/report_notification_configuration_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/report_template_input_v1.py` & `seeq-65.0.2/seeq/sdk/models/report_template_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/report_template_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/workbook_output_v1.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,477 +1,527 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
 
 
-class ReportTemplateOutputV1(object):
+class WorkbookOutputV1(object):
     """
     NOTE: This class is auto generated by the swagger code generator program.
     Do not edit the class manually.
     """
 
 
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
+        'ancestors': 'list[ItemPreviewV1]',
         'created_at': 'str',
         'creator': 'IdentityPreviewV1',
         'description': 'str',
         'effective_permissions': 'PermissionsV1',
-        'html_template': 'str',
         'id': 'str',
         'is_archived': 'bool',
         'is_redacted': 'bool',
+        'marked_as_favorite': 'bool',
         'name': 'str',
         'owner': 'IdentityPreviewV1',
         'parent_folder_id': 'str',
         'status_message': 'str',
         'translation_key': 'str',
         'type': 'str',
-        'updated_at': 'str'
+        'updated_at': 'str',
+        'worksheets': 'str'
     }
 
     attribute_map = {
+        'ancestors': 'ancestors',
         'created_at': 'createdAt',
         'creator': 'creator',
         'description': 'description',
         'effective_permissions': 'effectivePermissions',
-        'html_template': 'htmlTemplate',
         'id': 'id',
         'is_archived': 'isArchived',
         'is_redacted': 'isRedacted',
+        'marked_as_favorite': 'markedAsFavorite',
         'name': 'name',
         'owner': 'owner',
         'parent_folder_id': 'parentFolderId',
         'status_message': 'statusMessage',
         'translation_key': 'translationKey',
         'type': 'type',
-        'updated_at': 'updatedAt'
+        'updated_at': 'updatedAt',
+        'worksheets': 'worksheets'
     }
 
-    def __init__(self, created_at=None, creator=None, description=None, effective_permissions=None, html_template=None, id=None, is_archived=False, is_redacted=False, name=None, owner=None, parent_folder_id=None, status_message=None, translation_key=None, type=None, updated_at=None):
+    def __init__(self, ancestors=None, created_at=None, creator=None, description=None, effective_permissions=None, id=None, is_archived=False, is_redacted=False, marked_as_favorite=False, name=None, owner=None, parent_folder_id=None, status_message=None, translation_key=None, type=None, updated_at=None, worksheets=None):
         """
-        ReportTemplateOutputV1 - a model defined in Swagger
+        WorkbookOutputV1 - a model defined in Swagger
         """
 
+        self._ancestors = None
         self._created_at = None
         self._creator = None
         self._description = None
         self._effective_permissions = None
-        self._html_template = None
         self._id = None
         self._is_archived = None
         self._is_redacted = None
+        self._marked_as_favorite = None
         self._name = None
         self._owner = None
         self._parent_folder_id = None
         self._status_message = None
         self._translation_key = None
         self._type = None
         self._updated_at = None
+        self._worksheets = None
 
+        if ancestors is not None:
+          self.ancestors = ancestors
         if created_at is not None:
           self.created_at = created_at
         if creator is not None:
           self.creator = creator
         if description is not None:
           self.description = description
         if effective_permissions is not None:
           self.effective_permissions = effective_permissions
-        if html_template is not None:
-          self.html_template = html_template
         if id is not None:
           self.id = id
         if is_archived is not None:
           self.is_archived = is_archived
         if is_redacted is not None:
           self.is_redacted = is_redacted
+        if marked_as_favorite is not None:
+          self.marked_as_favorite = marked_as_favorite
         if name is not None:
           self.name = name
         if owner is not None:
           self.owner = owner
         if parent_folder_id is not None:
           self.parent_folder_id = parent_folder_id
         if status_message is not None:
           self.status_message = status_message
         if translation_key is not None:
           self.translation_key = translation_key
         if type is not None:
           self.type = type
         if updated_at is not None:
           self.updated_at = updated_at
+        if worksheets is not None:
+          self.worksheets = worksheets
+
+    @property
+    def ancestors(self):
+        """
+        Gets the ancestors of this WorkbookOutputV1.
+        The list of folder ancestors, starting at the topmost folder to which the user has access
+
+        :return: The ancestors of this WorkbookOutputV1.
+        :rtype: list[ItemPreviewV1]
+        """
+        return self._ancestors
+
+    @ancestors.setter
+    def ancestors(self, ancestors):
+        """
+        Sets the ancestors of this WorkbookOutputV1.
+        The list of folder ancestors, starting at the topmost folder to which the user has access
+
+        :param ancestors: The ancestors of this WorkbookOutputV1.
+        :type: list[ItemPreviewV1]
+        """
+
+        self._ancestors = ancestors
 
     @property
     def created_at(self):
         """
-        Gets the created_at of this ReportTemplateOutputV1.
-        The time the template was created at
+        Gets the created_at of this WorkbookOutputV1.
+        The ISO 8601 date of when the folder, analysis, topic, or project was created (YYYY-MM-DDThh:mm:ss.sssssssss±hh:mm)
 
-        :return: The created_at of this ReportTemplateOutputV1.
+        :return: The created_at of this WorkbookOutputV1.
         :rtype: str
         """
         return self._created_at
 
     @created_at.setter
     def created_at(self, created_at):
         """
-        Sets the created_at of this ReportTemplateOutputV1.
-        The time the template was created at
+        Sets the created_at of this WorkbookOutputV1.
+        The ISO 8601 date of when the folder, analysis, topic, or project was created (YYYY-MM-DDThh:mm:ss.sssssssss±hh:mm)
 
-        :param created_at: The created_at of this ReportTemplateOutputV1.
+        :param created_at: The created_at of this WorkbookOutputV1.
         :type: str
         """
-        if created_at is None:
-            raise ValueError("Invalid value for `created_at`, must not be `None`")
 
         self._created_at = created_at
 
     @property
     def creator(self):
         """
-        Gets the creator of this ReportTemplateOutputV1.
+        Gets the creator of this WorkbookOutputV1.
 
-        :return: The creator of this ReportTemplateOutputV1.
+        :return: The creator of this WorkbookOutputV1.
         :rtype: IdentityPreviewV1
         """
         return self._creator
 
     @creator.setter
     def creator(self, creator):
         """
-        Sets the creator of this ReportTemplateOutputV1.
+        Sets the creator of this WorkbookOutputV1.
 
-        :param creator: The creator of this ReportTemplateOutputV1.
+        :param creator: The creator of this WorkbookOutputV1.
         :type: IdentityPreviewV1
         """
 
         self._creator = creator
 
     @property
     def description(self):
         """
-        Gets the description of this ReportTemplateOutputV1.
+        Gets the description of this WorkbookOutputV1.
         Clarifying information or other plain language description of this item
 
-        :return: The description of this ReportTemplateOutputV1.
+        :return: The description of this WorkbookOutputV1.
         :rtype: str
         """
         return self._description
 
     @description.setter
     def description(self, description):
         """
-        Sets the description of this ReportTemplateOutputV1.
+        Sets the description of this WorkbookOutputV1.
         Clarifying information or other plain language description of this item
 
-        :param description: The description of this ReportTemplateOutputV1.
+        :param description: The description of this WorkbookOutputV1.
         :type: str
         """
 
         self._description = description
 
     @property
     def effective_permissions(self):
         """
-        Gets the effective_permissions of this ReportTemplateOutputV1.
+        Gets the effective_permissions of this WorkbookOutputV1.
 
-        :return: The effective_permissions of this ReportTemplateOutputV1.
+        :return: The effective_permissions of this WorkbookOutputV1.
         :rtype: PermissionsV1
         """
         return self._effective_permissions
 
     @effective_permissions.setter
     def effective_permissions(self, effective_permissions):
         """
-        Sets the effective_permissions of this ReportTemplateOutputV1.
+        Sets the effective_permissions of this WorkbookOutputV1.
 
-        :param effective_permissions: The effective_permissions of this ReportTemplateOutputV1.
+        :param effective_permissions: The effective_permissions of this WorkbookOutputV1.
         :type: PermissionsV1
         """
 
         self._effective_permissions = effective_permissions
 
     @property
-    def html_template(self):
-        """
-        Gets the html_template of this ReportTemplateOutputV1.
-        The html template itself
-
-        :return: The html_template of this ReportTemplateOutputV1.
-        :rtype: str
-        """
-        return self._html_template
-
-    @html_template.setter
-    def html_template(self, html_template):
-        """
-        Sets the html_template of this ReportTemplateOutputV1.
-        The html template itself
-
-        :param html_template: The html_template of this ReportTemplateOutputV1.
-        :type: str
-        """
-        if html_template is None:
-            raise ValueError("Invalid value for `html_template`, must not be `None`")
-
-        self._html_template = html_template
-
-    @property
     def id(self):
         """
-        Gets the id of this ReportTemplateOutputV1.
+        Gets the id of this WorkbookOutputV1.
         The ID that can be used to interact with the item
 
-        :return: The id of this ReportTemplateOutputV1.
+        :return: The id of this WorkbookOutputV1.
         :rtype: str
         """
         return self._id
 
     @id.setter
     def id(self, id):
         """
-        Sets the id of this ReportTemplateOutputV1.
+        Sets the id of this WorkbookOutputV1.
         The ID that can be used to interact with the item
 
-        :param id: The id of this ReportTemplateOutputV1.
+        :param id: The id of this WorkbookOutputV1.
         :type: str
         """
         if id is None:
             raise ValueError("Invalid value for `id`, must not be `None`")
 
         self._id = id
 
     @property
     def is_archived(self):
         """
-        Gets the is_archived of this ReportTemplateOutputV1.
+        Gets the is_archived of this WorkbookOutputV1.
         Whether item is archived
 
-        :return: The is_archived of this ReportTemplateOutputV1.
+        :return: The is_archived of this WorkbookOutputV1.
         :rtype: bool
         """
         return self._is_archived
 
     @is_archived.setter
     def is_archived(self, is_archived):
         """
-        Sets the is_archived of this ReportTemplateOutputV1.
+        Sets the is_archived of this WorkbookOutputV1.
         Whether item is archived
 
-        :param is_archived: The is_archived of this ReportTemplateOutputV1.
+        :param is_archived: The is_archived of this WorkbookOutputV1.
         :type: bool
         """
 
         self._is_archived = is_archived
 
     @property
     def is_redacted(self):
         """
-        Gets the is_redacted of this ReportTemplateOutputV1.
+        Gets the is_redacted of this WorkbookOutputV1.
         Whether item is redacted
 
-        :return: The is_redacted of this ReportTemplateOutputV1.
+        :return: The is_redacted of this WorkbookOutputV1.
         :rtype: bool
         """
         return self._is_redacted
 
     @is_redacted.setter
     def is_redacted(self, is_redacted):
         """
-        Sets the is_redacted of this ReportTemplateOutputV1.
+        Sets the is_redacted of this WorkbookOutputV1.
         Whether item is redacted
 
-        :param is_redacted: The is_redacted of this ReportTemplateOutputV1.
+        :param is_redacted: The is_redacted of this WorkbookOutputV1.
         :type: bool
         """
 
         self._is_redacted = is_redacted
 
     @property
+    def marked_as_favorite(self):
+        """
+        Gets the marked_as_favorite of this WorkbookOutputV1.
+        Flag indicating whether this folder, analysis, topic, or project has been marked as a favorite by the current user
+
+        :return: The marked_as_favorite of this WorkbookOutputV1.
+        :rtype: bool
+        """
+        return self._marked_as_favorite
+
+    @marked_as_favorite.setter
+    def marked_as_favorite(self, marked_as_favorite):
+        """
+        Sets the marked_as_favorite of this WorkbookOutputV1.
+        Flag indicating whether this folder, analysis, topic, or project has been marked as a favorite by the current user
+
+        :param marked_as_favorite: The marked_as_favorite of this WorkbookOutputV1.
+        :type: bool
+        """
+
+        self._marked_as_favorite = marked_as_favorite
+
+    @property
     def name(self):
         """
-        Gets the name of this ReportTemplateOutputV1.
+        Gets the name of this WorkbookOutputV1.
         The human readable name
 
-        :return: The name of this ReportTemplateOutputV1.
+        :return: The name of this WorkbookOutputV1.
         :rtype: str
         """
         return self._name
 
     @name.setter
     def name(self, name):
         """
-        Sets the name of this ReportTemplateOutputV1.
+        Sets the name of this WorkbookOutputV1.
         The human readable name
 
-        :param name: The name of this ReportTemplateOutputV1.
+        :param name: The name of this WorkbookOutputV1.
         :type: str
         """
         if name is None:
             raise ValueError("Invalid value for `name`, must not be `None`")
 
         self._name = name
 
     @property
     def owner(self):
         """
-        Gets the owner of this ReportTemplateOutputV1.
+        Gets the owner of this WorkbookOutputV1.
 
-        :return: The owner of this ReportTemplateOutputV1.
+        :return: The owner of this WorkbookOutputV1.
         :rtype: IdentityPreviewV1
         """
         return self._owner
 
     @owner.setter
     def owner(self, owner):
         """
-        Sets the owner of this ReportTemplateOutputV1.
+        Sets the owner of this WorkbookOutputV1.
 
-        :param owner: The owner of this ReportTemplateOutputV1.
+        :param owner: The owner of this WorkbookOutputV1.
         :type: IdentityPreviewV1
         """
 
         self._owner = owner
 
     @property
     def parent_folder_id(self):
         """
-        Gets the parent_folder_id of this ReportTemplateOutputV1.
+        Gets the parent_folder_id of this WorkbookOutputV1.
         The ID of the parent folder which this folder, analysis, topic, or project is a subfolder of
 
-        :return: The parent_folder_id of this ReportTemplateOutputV1.
+        :return: The parent_folder_id of this WorkbookOutputV1.
         :rtype: str
         """
         return self._parent_folder_id
 
     @parent_folder_id.setter
     def parent_folder_id(self, parent_folder_id):
         """
-        Sets the parent_folder_id of this ReportTemplateOutputV1.
+        Sets the parent_folder_id of this WorkbookOutputV1.
         The ID of the parent folder which this folder, analysis, topic, or project is a subfolder of
 
-        :param parent_folder_id: The parent_folder_id of this ReportTemplateOutputV1.
+        :param parent_folder_id: The parent_folder_id of this WorkbookOutputV1.
         :type: str
         """
 
         self._parent_folder_id = parent_folder_id
 
     @property
     def status_message(self):
         """
-        Gets the status_message of this ReportTemplateOutputV1.
+        Gets the status_message of this WorkbookOutputV1.
         A plain language status message with information about any issues that may have been encountered during an operation
 
-        :return: The status_message of this ReportTemplateOutputV1.
+        :return: The status_message of this WorkbookOutputV1.
         :rtype: str
         """
         return self._status_message
 
     @status_message.setter
     def status_message(self, status_message):
         """
-        Sets the status_message of this ReportTemplateOutputV1.
+        Sets the status_message of this WorkbookOutputV1.
         A plain language status message with information about any issues that may have been encountered during an operation
 
-        :param status_message: The status_message of this ReportTemplateOutputV1.
+        :param status_message: The status_message of this WorkbookOutputV1.
         :type: str
         """
 
         self._status_message = status_message
 
     @property
     def translation_key(self):
         """
-        Gets the translation_key of this ReportTemplateOutputV1.
+        Gets the translation_key of this WorkbookOutputV1.
         The item's translation key, if any
 
-        :return: The translation_key of this ReportTemplateOutputV1.
+        :return: The translation_key of this WorkbookOutputV1.
         :rtype: str
         """
         return self._translation_key
 
     @translation_key.setter
     def translation_key(self, translation_key):
         """
-        Sets the translation_key of this ReportTemplateOutputV1.
+        Sets the translation_key of this WorkbookOutputV1.
         The item's translation key, if any
 
-        :param translation_key: The translation_key of this ReportTemplateOutputV1.
+        :param translation_key: The translation_key of this WorkbookOutputV1.
         :type: str
         """
 
         self._translation_key = translation_key
 
     @property
     def type(self):
         """
-        Gets the type of this ReportTemplateOutputV1.
+        Gets the type of this WorkbookOutputV1.
         The type of the item
 
-        :return: The type of this ReportTemplateOutputV1.
+        :return: The type of this WorkbookOutputV1.
         :rtype: str
         """
         return self._type
 
     @type.setter
     def type(self, type):
         """
-        Sets the type of this ReportTemplateOutputV1.
+        Sets the type of this WorkbookOutputV1.
         The type of the item
 
-        :param type: The type of this ReportTemplateOutputV1.
+        :param type: The type of this WorkbookOutputV1.
         :type: str
         """
         if type is None:
             raise ValueError("Invalid value for `type`, must not be `None`")
 
         self._type = type
 
     @property
     def updated_at(self):
         """
-        Gets the updated_at of this ReportTemplateOutputV1.
-        The last time this template was updated
+        Gets the updated_at of this WorkbookOutputV1.
+        The ISO 8601 date of when the folder, analysis, topic, or project was updated (YYYY-MM-DDThh:mm:ss.sssssssss±hh:mm)
 
-        :return: The updated_at of this ReportTemplateOutputV1.
+        :return: The updated_at of this WorkbookOutputV1.
         :rtype: str
         """
         return self._updated_at
 
     @updated_at.setter
     def updated_at(self, updated_at):
         """
-        Sets the updated_at of this ReportTemplateOutputV1.
-        The last time this template was updated
+        Sets the updated_at of this WorkbookOutputV1.
+        The ISO 8601 date of when the folder, analysis, topic, or project was updated (YYYY-MM-DDThh:mm:ss.sssssssss±hh:mm)
 
-        :param updated_at: The updated_at of this ReportTemplateOutputV1.
+        :param updated_at: The updated_at of this WorkbookOutputV1.
         :type: str
         """
-        if updated_at is None:
-            raise ValueError("Invalid value for `updated_at`, must not be `None`")
 
         self._updated_at = updated_at
 
+    @property
+    def worksheets(self):
+        """
+        Gets the worksheets of this WorkbookOutputV1.
+        The href to retrieve the worksheets in this workbook
+
+        :return: The worksheets of this WorkbookOutputV1.
+        :rtype: str
+        """
+        return self._worksheets
+
+    @worksheets.setter
+    def worksheets(self, worksheets):
+        """
+        Sets the worksheets of this WorkbookOutputV1.
+        The href to retrieve the worksheets in this workbook
+
+        :param worksheets: The worksheets of this WorkbookOutputV1.
+        :type: str
+        """
+
+        self._worksheets = worksheets
+
     def to_dict(self):
         """
         Returns the model properties as a dict
         """
         result = {}
 
         for attr, _ in iteritems(self.swagger_types):
@@ -506,15 +556,15 @@
         """
         return self.to_str()
 
     def __eq__(self, other):
         """
         Returns true if both objects are equal
         """
-        if not isinstance(other, ReportTemplateOutputV1):
+        if not isinstance(other, WorkbookOutputV1):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """
         Returns true if both objects are not equal
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `seeq-65.0.1/seeq/sdk/models/request_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/request_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/sample_input_v1.py` & `seeq-65.0.2/seeq/sdk/models/sample_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/sample_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/sample_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/samples_input_v1.py` & `seeq-65.0.2/seeq/sdk/models/samples_input_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/samples_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/samples_output_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/samples_overwrite_input_v1.py` & `seeq-65.0.2/seeq/sdk/models/samples_overwrite_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/scalar_evaluate_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/scalar_evaluate_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/scalar_input_v1.py` & `seeq-65.0.2/seeq/sdk/models/scalar_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/scalar_property_v1.py` & `seeq-65.0.2/seeq/sdk/models/scalar_property_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/scalar_value_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/scalar_value_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/scale_across_tree_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/scale_across_tree_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/schedulable_admin_list_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/schedulable_admin_list_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/schedulable_admin_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/schedulable_admin_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/schedulable_summary_day_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/schedulable_summary_day_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/schedulable_summary_week_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/schedulable_summary_week_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/schedule_input_v1.py` & `seeq-65.0.2/seeq/sdk/models/schedule_input_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/schedule_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/schedule_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/scheduled_notebook_input_v1.py` & `seeq-65.0.2/seeq/sdk/models/scheduled_notebook_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/scheduled_notebook_list_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/scheduled_notebook_list_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/scheduled_notebook_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/scheduled_notebook_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/scim_token_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/scim_token_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/screenshot_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/screenshot_output_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/secret_configuration_field_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/secret_configuration_field_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/see_also_doc_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/see_also_doc_output_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/send_email_attachment_v1.py` & `seeq-65.0.2/seeq/sdk/models/send_email_attachment_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/send_email_contact_v1.py` & `seeq-65.0.2/seeq/sdk/models/send_email_contact_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/send_email_input_v1.py` & `seeq-65.0.2/seeq/sdk/models/send_email_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/sent_email_attachment_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/sent_email_attachment_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/sent_email_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/sent_email_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/sent_emails_list_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/sent_emails_list_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/server_build_info_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/server_build_info_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/server_load_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/server_load_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/server_spec_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/server_spec_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/server_status_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/server_status_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/signal_input_v1.py` & `seeq-65.0.2/seeq/sdk/models/signal_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/signal_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/signal_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/signal_with_id_input_v1.py` & `seeq-65.0.2/seeq/sdk/models/signal_with_id_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/status_message.py` & `seeq-65.0.2/seeq/sdk/models/status_message.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/status_message_base.py` & `seeq-65.0.2/seeq/sdk/models/status_message_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/store_secret_input_v1.py` & `seeq-65.0.2/seeq/sdk/models/store_secret_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/string_configuration_field_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/string_configuration_field_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/subscription_input_v1.py` & `seeq-65.0.2/seeq/sdk/models/subscription_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/subscription_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/subscription_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/subscription_update_input_v1.py` & `seeq-65.0.2/seeq/sdk/models/subscription_update_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/support_request_input_v1.py` & `seeq-65.0.2/seeq/sdk/models/support_request_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/support_request_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/support_request_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/supported_units_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/supported_units_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/swap_across_assets_search_v1.py` & `seeq-65.0.2/seeq/sdk/models/swap_across_assets_search_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/swap_input_v1.py` & `seeq-65.0.2/seeq/sdk/models/swap_input_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/swap_option_list_v1.py` & `seeq-65.0.2/seeq/sdk/models/swap_option_list_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/swap_option_v1.py` & `seeq-65.0.2/seeq/sdk/models/swap_option_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/swap_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/swap_output_v1.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/sync_progress.py` & `seeq-65.0.2/seeq/sdk/models/sync_progress.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/sync_progress_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/sync_progress_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/system_license_body.py` & `seeq-65.0.2/seeq/sdk/models/system_license_body.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/table_column_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/table_column_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/table_definition_input_v1.py` & `seeq-65.0.2/seeq/sdk/models/table_definition_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/table_definition_output_list_v1.py` & `seeq-65.0.2/seeq/sdk/models/table_definition_output_list_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/table_definition_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/table_definition_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/table_definition_update_input_v1.py` & `seeq-65.0.2/seeq/sdk/models/table_definition_update_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/threshold_metric_input_v1.py` & `seeq-65.0.2/seeq/sdk/models/threshold_metric_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/threshold_metric_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/threshold_metric_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/threshold_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/threshold_output_v1.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/timer_datum_v1.py` & `seeq-65.0.2/seeq/sdk/models/timer_datum_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/tree_item_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/tree_item_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/treemap_item_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/treemap_item_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/treemap_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/treemap_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/units_of_measure_batch_input_v1.py` & `seeq-65.0.2/seeq/sdk/models/units_of_measure_batch_input_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/units_of_measure_item_v1.py` & `seeq-65.0.2/seeq/sdk/models/units_of_measure_item_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/units_of_measure_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/units_of_measure_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/unsubscribe_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/unsubscribe_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/usage_output_list_v1.py` & `seeq-65.0.2/seeq/sdk/models/usage_output_list_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/usage_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/usage_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/usage_types_v1.py` & `seeq-65.0.2/seeq/sdk/models/usage_types_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/user_group_input_v1.py` & `seeq-65.0.2/seeq/sdk/models/user_group_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/user_group_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/user_group_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/user_group_with_id_input_v1.py` & `seeq-65.0.2/seeq/sdk/models/user_group_with_id_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/user_input_v1.py` & `seeq-65.0.2/seeq/sdk/models/user_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/user_output_list_v1.py` & `seeq-65.0.2/seeq/sdk/models/user_output_list_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/user_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/user_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/user_password_input_v1.py` & `seeq-65.0.2/seeq/sdk/models/user_password_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/validate_cron_list_input_v1.py` & `seeq-65.0.2/seeq/sdk/models/validate_cron_list_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/validate_cron_list_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/validate_cron_list_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/validate_cron_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/validate_cron_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/workbench_item_output_list_v1.py` & `seeq-65.0.2/seeq/sdk/models/workbench_item_output_list_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/workbench_search_result_preview_v1.py` & `seeq-65.0.2/seeq/sdk/models/workbench_search_result_preview_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/workbook_input_v1.py` & `seeq-65.0.2/seeq/sdk/models/workbook_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/workbook_output_list_v1.py` & `seeq-65.0.2/seeq/sdk/models/workbook_output_list_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/workbook_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/workstep_output_v1.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,527 +1,449 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
 
 
-class WorkbookOutputV1(object):
+class WorkstepOutputV1(object):
     """
     NOTE: This class is auto generated by the swagger code generator program.
     Do not edit the class manually.
     """
 
 
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'ancestors': 'list[ItemPreviewV1]',
         'created_at': 'str',
-        'creator': 'IdentityPreviewV1',
+        'data': 'str',
         'description': 'str',
         'effective_permissions': 'PermissionsV1',
         'id': 'str',
         'is_archived': 'bool',
         'is_redacted': 'bool',
-        'marked_as_favorite': 'bool',
+        'last': 'str',
         'name': 'str',
-        'owner': 'IdentityPreviewV1',
-        'parent_folder_id': 'str',
+        'next': 'str',
+        'previous': 'str',
         'status_message': 'str',
         'translation_key': 'str',
-        'type': 'str',
-        'updated_at': 'str',
-        'worksheets': 'str'
+        'type': 'str'
     }
 
     attribute_map = {
-        'ancestors': 'ancestors',
         'created_at': 'createdAt',
-        'creator': 'creator',
+        'data': 'data',
         'description': 'description',
         'effective_permissions': 'effectivePermissions',
         'id': 'id',
         'is_archived': 'isArchived',
         'is_redacted': 'isRedacted',
-        'marked_as_favorite': 'markedAsFavorite',
+        'last': 'last',
         'name': 'name',
-        'owner': 'owner',
-        'parent_folder_id': 'parentFolderId',
+        'next': 'next',
+        'previous': 'previous',
         'status_message': 'statusMessage',
         'translation_key': 'translationKey',
-        'type': 'type',
-        'updated_at': 'updatedAt',
-        'worksheets': 'worksheets'
+        'type': 'type'
     }
 
-    def __init__(self, ancestors=None, created_at=None, creator=None, description=None, effective_permissions=None, id=None, is_archived=False, is_redacted=False, marked_as_favorite=False, name=None, owner=None, parent_folder_id=None, status_message=None, translation_key=None, type=None, updated_at=None, worksheets=None):
+    def __init__(self, created_at=None, data=None, description=None, effective_permissions=None, id=None, is_archived=False, is_redacted=False, last=None, name=None, next=None, previous=None, status_message=None, translation_key=None, type=None):
         """
-        WorkbookOutputV1 - a model defined in Swagger
+        WorkstepOutputV1 - a model defined in Swagger
         """
 
-        self._ancestors = None
         self._created_at = None
-        self._creator = None
+        self._data = None
         self._description = None
         self._effective_permissions = None
         self._id = None
         self._is_archived = None
         self._is_redacted = None
-        self._marked_as_favorite = None
+        self._last = None
         self._name = None
-        self._owner = None
-        self._parent_folder_id = None
+        self._next = None
+        self._previous = None
         self._status_message = None
         self._translation_key = None
         self._type = None
-        self._updated_at = None
-        self._worksheets = None
 
-        if ancestors is not None:
-          self.ancestors = ancestors
         if created_at is not None:
           self.created_at = created_at
-        if creator is not None:
-          self.creator = creator
+        if data is not None:
+          self.data = data
         if description is not None:
           self.description = description
         if effective_permissions is not None:
           self.effective_permissions = effective_permissions
         if id is not None:
           self.id = id
         if is_archived is not None:
           self.is_archived = is_archived
         if is_redacted is not None:
           self.is_redacted = is_redacted
-        if marked_as_favorite is not None:
-          self.marked_as_favorite = marked_as_favorite
+        if last is not None:
+          self.last = last
         if name is not None:
           self.name = name
-        if owner is not None:
-          self.owner = owner
-        if parent_folder_id is not None:
-          self.parent_folder_id = parent_folder_id
+        if next is not None:
+          self.next = next
+        if previous is not None:
+          self.previous = previous
         if status_message is not None:
           self.status_message = status_message
         if translation_key is not None:
           self.translation_key = translation_key
         if type is not None:
           self.type = type
-        if updated_at is not None:
-          self.updated_at = updated_at
-        if worksheets is not None:
-          self.worksheets = worksheets
-
-    @property
-    def ancestors(self):
-        """
-        Gets the ancestors of this WorkbookOutputV1.
-        The list of folder ancestors, starting at the topmost folder to which the user has access
-
-        :return: The ancestors of this WorkbookOutputV1.
-        :rtype: list[ItemPreviewV1]
-        """
-        return self._ancestors
-
-    @ancestors.setter
-    def ancestors(self, ancestors):
-        """
-        Sets the ancestors of this WorkbookOutputV1.
-        The list of folder ancestors, starting at the topmost folder to which the user has access
-
-        :param ancestors: The ancestors of this WorkbookOutputV1.
-        :type: list[ItemPreviewV1]
-        """
-
-        self._ancestors = ancestors
 
     @property
     def created_at(self):
         """
-        Gets the created_at of this WorkbookOutputV1.
-        The ISO 8601 date of when the folder, analysis, topic, or project was created (YYYY-MM-DDThh:mm:ss.sssssssss±hh:mm)
+        Gets the created_at of this WorkstepOutputV1.
+        The ISO 8601 date of when the workstep was created (YYYY-MM-DDThh:mm:ss.sssssssss±hh:mm)
 
-        :return: The created_at of this WorkbookOutputV1.
+        :return: The created_at of this WorkstepOutputV1.
         :rtype: str
         """
         return self._created_at
 
     @created_at.setter
     def created_at(self, created_at):
         """
-        Sets the created_at of this WorkbookOutputV1.
-        The ISO 8601 date of when the folder, analysis, topic, or project was created (YYYY-MM-DDThh:mm:ss.sssssssss±hh:mm)
+        Sets the created_at of this WorkstepOutputV1.
+        The ISO 8601 date of when the workstep was created (YYYY-MM-DDThh:mm:ss.sssssssss±hh:mm)
 
-        :param created_at: The created_at of this WorkbookOutputV1.
+        :param created_at: The created_at of this WorkstepOutputV1.
         :type: str
         """
 
         self._created_at = created_at
 
     @property
-    def creator(self):
+    def data(self):
         """
-        Gets the creator of this WorkbookOutputV1.
+        Gets the data of this WorkstepOutputV1.
+        JSON-encoded state for this workstep
 
-        :return: The creator of this WorkbookOutputV1.
-        :rtype: IdentityPreviewV1
+        :return: The data of this WorkstepOutputV1.
+        :rtype: str
         """
-        return self._creator
+        return self._data
 
-    @creator.setter
-    def creator(self, creator):
+    @data.setter
+    def data(self, data):
         """
-        Sets the creator of this WorkbookOutputV1.
+        Sets the data of this WorkstepOutputV1.
+        JSON-encoded state for this workstep
 
-        :param creator: The creator of this WorkbookOutputV1.
-        :type: IdentityPreviewV1
+        :param data: The data of this WorkstepOutputV1.
+        :type: str
         """
+        if data is None:
+            raise ValueError("Invalid value for `data`, must not be `None`")
 
-        self._creator = creator
+        self._data = data
 
     @property
     def description(self):
         """
-        Gets the description of this WorkbookOutputV1.
+        Gets the description of this WorkstepOutputV1.
         Clarifying information or other plain language description of this item
 
-        :return: The description of this WorkbookOutputV1.
+        :return: The description of this WorkstepOutputV1.
         :rtype: str
         """
         return self._description
 
     @description.setter
     def description(self, description):
         """
-        Sets the description of this WorkbookOutputV1.
+        Sets the description of this WorkstepOutputV1.
         Clarifying information or other plain language description of this item
 
-        :param description: The description of this WorkbookOutputV1.
+        :param description: The description of this WorkstepOutputV1.
         :type: str
         """
 
         self._description = description
 
     @property
     def effective_permissions(self):
         """
-        Gets the effective_permissions of this WorkbookOutputV1.
+        Gets the effective_permissions of this WorkstepOutputV1.
 
-        :return: The effective_permissions of this WorkbookOutputV1.
+        :return: The effective_permissions of this WorkstepOutputV1.
         :rtype: PermissionsV1
         """
         return self._effective_permissions
 
     @effective_permissions.setter
     def effective_permissions(self, effective_permissions):
         """
-        Sets the effective_permissions of this WorkbookOutputV1.
+        Sets the effective_permissions of this WorkstepOutputV1.
 
-        :param effective_permissions: The effective_permissions of this WorkbookOutputV1.
+        :param effective_permissions: The effective_permissions of this WorkstepOutputV1.
         :type: PermissionsV1
         """
 
         self._effective_permissions = effective_permissions
 
     @property
     def id(self):
         """
-        Gets the id of this WorkbookOutputV1.
+        Gets the id of this WorkstepOutputV1.
         The ID that can be used to interact with the item
 
-        :return: The id of this WorkbookOutputV1.
+        :return: The id of this WorkstepOutputV1.
         :rtype: str
         """
         return self._id
 
     @id.setter
     def id(self, id):
         """
-        Sets the id of this WorkbookOutputV1.
+        Sets the id of this WorkstepOutputV1.
         The ID that can be used to interact with the item
 
-        :param id: The id of this WorkbookOutputV1.
+        :param id: The id of this WorkstepOutputV1.
         :type: str
         """
         if id is None:
             raise ValueError("Invalid value for `id`, must not be `None`")
 
         self._id = id
 
     @property
     def is_archived(self):
         """
-        Gets the is_archived of this WorkbookOutputV1.
+        Gets the is_archived of this WorkstepOutputV1.
         Whether item is archived
 
-        :return: The is_archived of this WorkbookOutputV1.
+        :return: The is_archived of this WorkstepOutputV1.
         :rtype: bool
         """
         return self._is_archived
 
     @is_archived.setter
     def is_archived(self, is_archived):
         """
-        Sets the is_archived of this WorkbookOutputV1.
+        Sets the is_archived of this WorkstepOutputV1.
         Whether item is archived
 
-        :param is_archived: The is_archived of this WorkbookOutputV1.
+        :param is_archived: The is_archived of this WorkstepOutputV1.
         :type: bool
         """
 
         self._is_archived = is_archived
 
     @property
     def is_redacted(self):
         """
-        Gets the is_redacted of this WorkbookOutputV1.
+        Gets the is_redacted of this WorkstepOutputV1.
         Whether item is redacted
 
-        :return: The is_redacted of this WorkbookOutputV1.
+        :return: The is_redacted of this WorkstepOutputV1.
         :rtype: bool
         """
         return self._is_redacted
 
     @is_redacted.setter
     def is_redacted(self, is_redacted):
         """
-        Sets the is_redacted of this WorkbookOutputV1.
+        Sets the is_redacted of this WorkstepOutputV1.
         Whether item is redacted
 
-        :param is_redacted: The is_redacted of this WorkbookOutputV1.
+        :param is_redacted: The is_redacted of this WorkstepOutputV1.
         :type: bool
         """
 
         self._is_redacted = is_redacted
 
     @property
-    def marked_as_favorite(self):
+    def last(self):
         """
-        Gets the marked_as_favorite of this WorkbookOutputV1.
-        Flag indicating whether this folder, analysis, topic, or project has been marked as a favorite by the current user
+        Gets the last of this WorkstepOutputV1.
+        The ID that can be used to interact with the last workstep or null if there is not one
 
-        :return: The marked_as_favorite of this WorkbookOutputV1.
-        :rtype: bool
+        :return: The last of this WorkstepOutputV1.
+        :rtype: str
         """
-        return self._marked_as_favorite
+        return self._last
 
-    @marked_as_favorite.setter
-    def marked_as_favorite(self, marked_as_favorite):
+    @last.setter
+    def last(self, last):
         """
-        Sets the marked_as_favorite of this WorkbookOutputV1.
-        Flag indicating whether this folder, analysis, topic, or project has been marked as a favorite by the current user
+        Sets the last of this WorkstepOutputV1.
+        The ID that can be used to interact with the last workstep or null if there is not one
 
-        :param marked_as_favorite: The marked_as_favorite of this WorkbookOutputV1.
-        :type: bool
+        :param last: The last of this WorkstepOutputV1.
+        :type: str
         """
 
-        self._marked_as_favorite = marked_as_favorite
+        self._last = last
 
     @property
     def name(self):
         """
-        Gets the name of this WorkbookOutputV1.
+        Gets the name of this WorkstepOutputV1.
         The human readable name
 
-        :return: The name of this WorkbookOutputV1.
+        :return: The name of this WorkstepOutputV1.
         :rtype: str
         """
         return self._name
 
     @name.setter
     def name(self, name):
         """
-        Sets the name of this WorkbookOutputV1.
+        Sets the name of this WorkstepOutputV1.
         The human readable name
 
-        :param name: The name of this WorkbookOutputV1.
+        :param name: The name of this WorkstepOutputV1.
         :type: str
         """
         if name is None:
             raise ValueError("Invalid value for `name`, must not be `None`")
 
         self._name = name
 
     @property
-    def owner(self):
+    def next(self):
         """
-        Gets the owner of this WorkbookOutputV1.
+        Gets the next of this WorkstepOutputV1.
+        The ID that can be used to interact with the next workstep or null if there is not one
 
-        :return: The owner of this WorkbookOutputV1.
-        :rtype: IdentityPreviewV1
+        :return: The next of this WorkstepOutputV1.
+        :rtype: str
         """
-        return self._owner
+        return self._next
 
-    @owner.setter
-    def owner(self, owner):
+    @next.setter
+    def next(self, next):
         """
-        Sets the owner of this WorkbookOutputV1.
+        Sets the next of this WorkstepOutputV1.
+        The ID that can be used to interact with the next workstep or null if there is not one
 
-        :param owner: The owner of this WorkbookOutputV1.
-        :type: IdentityPreviewV1
+        :param next: The next of this WorkstepOutputV1.
+        :type: str
         """
 
-        self._owner = owner
+        self._next = next
 
     @property
-    def parent_folder_id(self):
+    def previous(self):
         """
-        Gets the parent_folder_id of this WorkbookOutputV1.
-        The ID of the parent folder which this folder, analysis, topic, or project is a subfolder of
+        Gets the previous of this WorkstepOutputV1.
+        The ID that can be used to interact with the previous workstep or null if there is not one
 
-        :return: The parent_folder_id of this WorkbookOutputV1.
+        :return: The previous of this WorkstepOutputV1.
         :rtype: str
         """
-        return self._parent_folder_id
+        return self._previous
 
-    @parent_folder_id.setter
-    def parent_folder_id(self, parent_folder_id):
+    @previous.setter
+    def previous(self, previous):
         """
-        Sets the parent_folder_id of this WorkbookOutputV1.
-        The ID of the parent folder which this folder, analysis, topic, or project is a subfolder of
+        Sets the previous of this WorkstepOutputV1.
+        The ID that can be used to interact with the previous workstep or null if there is not one
 
-        :param parent_folder_id: The parent_folder_id of this WorkbookOutputV1.
+        :param previous: The previous of this WorkstepOutputV1.
         :type: str
         """
 
-        self._parent_folder_id = parent_folder_id
+        self._previous = previous
 
     @property
     def status_message(self):
         """
-        Gets the status_message of this WorkbookOutputV1.
+        Gets the status_message of this WorkstepOutputV1.
         A plain language status message with information about any issues that may have been encountered during an operation
 
-        :return: The status_message of this WorkbookOutputV1.
+        :return: The status_message of this WorkstepOutputV1.
         :rtype: str
         """
         return self._status_message
 
     @status_message.setter
     def status_message(self, status_message):
         """
-        Sets the status_message of this WorkbookOutputV1.
+        Sets the status_message of this WorkstepOutputV1.
         A plain language status message with information about any issues that may have been encountered during an operation
 
-        :param status_message: The status_message of this WorkbookOutputV1.
+        :param status_message: The status_message of this WorkstepOutputV1.
         :type: str
         """
 
         self._status_message = status_message
 
     @property
     def translation_key(self):
         """
-        Gets the translation_key of this WorkbookOutputV1.
+        Gets the translation_key of this WorkstepOutputV1.
         The item's translation key, if any
 
-        :return: The translation_key of this WorkbookOutputV1.
+        :return: The translation_key of this WorkstepOutputV1.
         :rtype: str
         """
         return self._translation_key
 
     @translation_key.setter
     def translation_key(self, translation_key):
         """
-        Sets the translation_key of this WorkbookOutputV1.
+        Sets the translation_key of this WorkstepOutputV1.
         The item's translation key, if any
 
-        :param translation_key: The translation_key of this WorkbookOutputV1.
+        :param translation_key: The translation_key of this WorkstepOutputV1.
         :type: str
         """
 
         self._translation_key = translation_key
 
     @property
     def type(self):
         """
-        Gets the type of this WorkbookOutputV1.
+        Gets the type of this WorkstepOutputV1.
         The type of the item
 
-        :return: The type of this WorkbookOutputV1.
+        :return: The type of this WorkstepOutputV1.
         :rtype: str
         """
         return self._type
 
     @type.setter
     def type(self, type):
         """
-        Sets the type of this WorkbookOutputV1.
+        Sets the type of this WorkstepOutputV1.
         The type of the item
 
-        :param type: The type of this WorkbookOutputV1.
+        :param type: The type of this WorkstepOutputV1.
         :type: str
         """
         if type is None:
             raise ValueError("Invalid value for `type`, must not be `None`")
 
         self._type = type
 
-    @property
-    def updated_at(self):
-        """
-        Gets the updated_at of this WorkbookOutputV1.
-        The ISO 8601 date of when the folder, analysis, topic, or project was updated (YYYY-MM-DDThh:mm:ss.sssssssss±hh:mm)
-
-        :return: The updated_at of this WorkbookOutputV1.
-        :rtype: str
-        """
-        return self._updated_at
-
-    @updated_at.setter
-    def updated_at(self, updated_at):
-        """
-        Sets the updated_at of this WorkbookOutputV1.
-        The ISO 8601 date of when the folder, analysis, topic, or project was updated (YYYY-MM-DDThh:mm:ss.sssssssss±hh:mm)
-
-        :param updated_at: The updated_at of this WorkbookOutputV1.
-        :type: str
-        """
-
-        self._updated_at = updated_at
-
-    @property
-    def worksheets(self):
-        """
-        Gets the worksheets of this WorkbookOutputV1.
-        The href to retrieve the worksheets in this workbook
-
-        :return: The worksheets of this WorkbookOutputV1.
-        :rtype: str
-        """
-        return self._worksheets
-
-    @worksheets.setter
-    def worksheets(self, worksheets):
-        """
-        Sets the worksheets of this WorkbookOutputV1.
-        The href to retrieve the worksheets in this workbook
-
-        :param worksheets: The worksheets of this WorkbookOutputV1.
-        :type: str
-        """
-
-        self._worksheets = worksheets
-
     def to_dict(self):
         """
         Returns the model properties as a dict
         """
         result = {}
 
         for attr, _ in iteritems(self.swagger_types):
@@ -556,15 +478,15 @@
         """
         return self.to_str()
 
     def __eq__(self, other):
         """
         Returns true if both objects are equal
         """
-        if not isinstance(other, WorkbookOutputV1):
+        if not isinstance(other, WorkstepOutputV1):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """
         Returns true if both objects are not equal
```

### Comparing `seeq-65.0.1/seeq/sdk/models/worksheet_input_v1.py` & `seeq-65.0.2/seeq/sdk/models/worksheet_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/worksheet_output_list_v1.py` & `seeq-65.0.2/seeq/sdk/models/worksheet_output_list_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/worksheet_output_v1.py` & `seeq-65.0.2/seeq/sdk/models/worksheet_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/models/workstep_input_v1.py` & `seeq-65.0.2/seeq/sdk/models/workstep_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-65.0.1/seeq/sdk/rest.py` & `seeq-65.0.2/seeq/sdk/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 65.0.1-v202405012042
+    OpenAPI spec version: 65.0.2-v202405092056
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import io
```

### Comparing `seeq-65.0.1/seeq.egg-info/PKG-INFO` & `seeq-65.0.2/seeq.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seeq
-Version: 65.0.1
+Version: 65.0.2
 Summary: The Seeq SDK for Python
 Home-page: https://www.seeq.com
 Author: Seeq Corporation
 Author-email: support@seeq.com
 Project-URL: Documentation, https://python-docs.seeq.com/
 Project-URL: Changelog, https://python-docs.seeq.com/changelog.html
 Classifier: Programming Language :: Python :: 2
```

### Comparing `seeq-65.0.1/seeq.egg-info/SOURCES.txt` & `seeq-65.0.2/seeq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `seeq-65.0.1/setup.py` & `seeq-65.0.2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="seeq",
-    version="65.0.1",
+    version="65.0.2",
     author="Seeq Corporation",
     author_email="support@seeq.com",
     description="The Seeq SDK for Python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://www.seeq.com",
     project_urls={
```

