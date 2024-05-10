# Comparing `tmp/browsergym_workarena-0.1.0rc7.tar.gz` & `tmp/browsergym_workarena-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression, original size modulo 2^32 144660480 gzip compressed data, reserved method, was "", from FAT filesystem (MS-DOS, OS/2, NT)
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression, original size modulo 2^32 147292160 gzip compressed data, reserved method, was "", from FAT filesystem (MS-DOS, OS/2, NT)
```

## Comparing `browsergym_workarena-0.1.0rc7.tar` & `browsergym_workarena-0.2.0.tar`

### file list

```diff
@@ -1,84 +1,98 @@
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 browsergym_workarena-0.1.0rc7/requirements.txt
--rw-r--r--   0        0        0     3261 2020-02-02 00:00:00.000000 browsergym_workarena-0.1.0rc7/.github/workflows/pypi.yml
--rw-r--r--   0        0        0    58904 2020-02-02 00:00:00.000000 browsergym_workarena-0.1.0rc7/scripts/generate_knowledge_base.ipynb
--rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 browsergym_workarena-0.1.0rc7/src/browsergym/workarena/__init__.py
--rw-r--r--   0        0        0     6571 2020-02-02 00:00:00.000000 browsergym_workarena-0.1.0rc7/src/browsergym/workarena/config.py
--rw-r--r--   0        0        0    21373 2020-02-02 00:00:00.000000 browsergym_workarena-0.1.0rc7/src/browsergym/workarena/install.py
--rw-r--r--   0        0        0     4314 2020-02-02 00:00:00.000000 browsergym_workarena-0.1.0rc7/src/browsergym/workarena/instance.py
--rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 browsergym_workarena-0.1.0rc7/src/browsergym/workarena/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 browsergym_workarena-0.1.0rc7/src/browsergym/workarena/api/__init__.py
--rw-r--r--   0        0        0     4148 2020-02-02 00:00:00.000000 browsergym_workarena-0.1.0rc7/src/browsergym/workarena/api/requests.py
--rw-r--r--   0        0        0     3307 2020-02-02 00:00:00.000000 browsergym_workarena-0.1.0rc7/src/browsergym/workarena/api/utils.py
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 browsergym_workarena-0.1.0rc7/src/browsergym/workarena/data_files/setup_files/forms/expected_change_request_form_fields.json
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 browsergym_workarena-0.1.0rc7/src/browsergym/workarena/data_files/setup_files/forms/expected_hardware_form_fields.json
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 browsergym_workarena-0.1.0rc7/src/browsergym/workarena/data_files/setup_files/forms/expected_incident_form_fields.json
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 browsergym_workarena-0.1.0rc7/src/browsergym/workarena/data_files/setup_files/forms/expected_problem_form_fields.json
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 browsergym_workarena-0.1.0rc7/src/browsergym/workarena/data_files/setup_files/forms/expected_user_form_fields.json
--rw-r--r--   0        0        0    11500 2020-02-02 00:00:00.000000 browsergym_workarena-0.1.0rc7/src/browsergym/workarena/data_files/setup_files/knowledge/kb_autopublish_workflow.xml
--rw-r--r--   0        0        0   474939 2020-02-02 00:00:00.000000 browsergym_workarena-0.1.0rc7/src/browsergym/workarena/data_files/setup_files/knowledge/knowledge_base.json
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 browsergym_workarena-0.1.0rc7/src/browsergym/workarena/data_files/setup_files/lists/expected_asset_list_columns.json
--rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 browsergym_workarena-0.1.0rc7/src/browsergym/workarena/data_files/setup_files/lists/expected_change_request_list_columns.json
--rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 browsergym_workarena-0.1.0rc7/src/browsergym/workarena/data_files/setup_files/lists/expected_hardware_list_columns.json
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 browsergym_workarena-0.1.0rc7/src/browsergym/workarena/data_files/setup_files/lists/expected_incident_list_columns.json
--rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 browsergym_workarena-0.1.0rc7/src/browsergym/workarena/data_files/setup_files/lists/expected_service_catalog_list_columns.json
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 browsergym_workarena-0.1.0rc7/src/browsergym/workarena/data_files/setup_files/lists/expected_user_list_columns.json
--rw-r--r--   0        0        0   270388 2020-02-02 00:00:00.000000 browsergym_workarena-0.1.0rc7/src/browsergym/workarena/data_files/task_configs/all_menu.json
--rw-r--r--   0        0        0  6306733 2020-02-02 00:00:00.000000 browsergym_workarena-0.1.0rc7/src/browsergym/workarena/data_files/task_configs/create_change_request_task.json
--rw-r--r--   0        0        0  4971385 2020-02-02 00:00:00.000000 browsergym_workarena-0.1.0rc7/src/browsergym/workarena/data_files/task_configs/create_hardware_asset_task.json
--rw-r--r--   0        0        0  5812616 2020-02-02 00:00:00.000000 browsergym_workarena-0.1.0rc7/src/browsergym/workarena/data_files/task_configs/create_incident_task.json
--rw-r--r--   0        0        0  4994349 2020-02-02 00:00:00.000000 browsergym_workarena-0.1.0rc7/src/browsergym/workarena/data_files/task_configs/create_problem_task.json
--rw-r--r--   0        0        0  3981025 2020-02-02 00:00:00.000000 browsergym_workarena-0.1.0rc7/src/browsergym/workarena/data_files/task_configs/create_user_task.json
--rw-r--r--   0        0        0 11882372 2020-02-02 00:00:00.000000 browsergym_workarena-0.1.0rc7/src/browsergym/workarena/data_files/task_configs/filter_asset_list_task.json
--rw-r--r--   0        0        0 12812288 2020-02-02 00:00:00.000000 browsergym_workarena-0.1.0rc7/src/browsergym/workarena/data_files/task_configs/filter_change_request_list_task.json
--rw-r--r--   0        0        0 12785357 2020-02-02 00:00:00.000000 browsergym_workarena-0.1.0rc7/src/browsergym/workarena/data_files/task_configs/filter_hardware_list_task.json
--rw-r--r--   0        0        0 11773863 2020-02-02 00:00:00.000000 browsergym_workarena-0.1.0rc7/src/browsergym/workarena/data_files/task_configs/filter_incident_list_task.json
--rw-r--r--   0        0        0  9231689 2020-02-02 00:00:00.000000 browsergym_workarena-0.1.0rc7/src/browsergym/workarena/data_files/task_configs/filter_service_catalog_item_list_task.json
--rw-r--r--   0        0        0 55965665 2020-02-02 00:00:00.000000 browsergym_workarena-0.1.0rc7/src/browsergym/workarena/data_files/task_configs/filter_user_list_task.json
--rw-r--r--   0        0        0    13021 2020-02-02 00:00:00.000000 browsergym_workarena-0.1.0rc7/src/browsergym/workarena/data_files/task_configs/impersonation_users.json
--rw-r--r--   0        0        0   617853 2020-02-02 00:00:00.000000 browsergym_workarena-0.1.0rc7/src/browsergym/workarena/data_files/task_configs/knowledge_base_configs.json
--rw-r--r--   0        0        0     1483 2020-02-02 00:00:00.000000 browsergym_workarena-0.1.0rc7/src/browsergym/workarena/data_files/task_configs/order_apple_mac_book_pro15_task.json
--rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 browsergym_workarena-0.1.0rc7/src/browsergym/workarena/data_files/task_configs/order_apple_watch_task.json
--rw-r--r--   0        0        0   610195 2020-02-02 00:00:00.000000 browsergym_workarena-0.1.0rc7/src/browsergym/workarena/data_files/task_configs/order_developer_laptop_task.json
--rw-r--r--   0        0        0    15666 2020-02-02 00:00:00.000000 browsergym_workarena-0.1.0rc7/src/browsergym/workarena/data_files/task_configs/order_development_laptop_pc_task.json
--rw-r--r--   0        0        0    27830 2020-02-02 00:00:00.000000 browsergym_workarena-0.1.0rc7/src/browsergym/workarena/data_files/task_configs/order_ipad_mini_task.json
--rw-r--r--   0        0        0    20828 2020-02-02 00:00:00.000000 browsergym_workarena-0.1.0rc7/src/browsergym/workarena/data_files/task_configs/order_ipad_pro_task.json
--rw-r--r--   0        0        0   183107 2020-02-02 00:00:00.000000 browsergym_workarena-0.1.0rc7/src/browsergym/workarena/data_files/task_configs/order_loaner_laptop_task.json
--rw-r--r--   0        0        0   707828 2020-02-02 00:00:00.000000 browsergym_workarena-0.1.0rc7/src/browsergym/workarena/data_files/task_configs/order_sales_laptop_task.json
--rw-r--r--   0        0        0   516203 2020-02-02 00:00:00.000000 browsergym_workarena-0.1.0rc7/src/browsergym/workarena/data_files/task_configs/order_standard_laptop_task.json
--rw-r--r--   0        0        0    44721 2020-02-02 00:00:00.000000 browsergym_workarena-0.1.0rc7/src/browsergym/workarena/data_files/task_configs/sort_asset_list_task.json
--rw-r--r--   0        0        0    45862 2020-02-02 00:00:00.000000 browsergym_workarena-0.1.0rc7/src/browsergym/workarena/data_files/task_configs/sort_change_request_list_task.json
--rw-r--r--   0        0        0    45127 2020-02-02 00:00:00.000000 browsergym_workarena-0.1.0rc7/src/browsergym/workarena/data_files/task_configs/sort_hardware_list_task.json
--rw-r--r--   0        0        0    45205 2020-02-02 00:00:00.000000 browsergym_workarena-0.1.0rc7/src/browsergym/workarena/data_files/task_configs/sort_incident_list_task.json
--rw-r--r--   0        0        0    46700 2020-02-02 00:00:00.000000 browsergym_workarena-0.1.0rc7/src/browsergym/workarena/data_files/task_configs/sort_service_catalog_item_list_task.json
--rw-r--r--   0        0        0    44336 2020-02-02 00:00:00.000000 browsergym_workarena-0.1.0rc7/src/browsergym/workarena/data_files/task_configs/sort_user_list_task.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 browsergym_workarena-0.1.0rc7/src/browsergym/workarena/tasks/__init__.py
--rw-r--r--   0        0        0     3419 2020-02-02 00:00:00.000000 browsergym_workarena-0.1.0rc7/src/browsergym/workarena/tasks/base.py
--rw-r--r--   0        0        0    30599 2020-02-02 00:00:00.000000 browsergym_workarena-0.1.0rc7/src/browsergym/workarena/tasks/form.py
--rw-r--r--   0        0        0     5771 2020-02-02 00:00:00.000000 browsergym_workarena-0.1.0rc7/src/browsergym/workarena/tasks/knowledge.py
--rw-r--r--   0        0        0    37108 2020-02-02 00:00:00.000000 browsergym_workarena-0.1.0rc7/src/browsergym/workarena/tasks/list.py
--rw-r--r--   0        0        0     7384 2020-02-02 00:00:00.000000 browsergym_workarena-0.1.0rc7/src/browsergym/workarena/tasks/navigation.py
--rw-r--r--   0        0        0    21661 2020-02-02 00:00:00.000000 browsergym_workarena-0.1.0rc7/src/browsergym/workarena/tasks/service_catalog.py
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 browsergym_workarena-0.1.0rc7/src/browsergym/workarena/tasks/scripts/README.md
--rw-r--r--   0        0        0     9870 2020-02-02 00:00:00.000000 browsergym_workarena-0.1.0rc7/src/browsergym/workarena/tasks/scripts/extract_all_menu_items.py
--rw-r--r--   0        0        0     3697 2020-02-02 00:00:00.000000 browsergym_workarena-0.1.0rc7/src/browsergym/workarena/tasks/scripts/generate_forms.py
--rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 browsergym_workarena-0.1.0rc7/src/browsergym/workarena/tasks/scripts/knowledge.py
--rw-r--r--   0        0        0     4805 2020-02-02 00:00:00.000000 browsergym_workarena-0.1.0rc7/src/browsergym/workarena/tasks/scripts/list.py
--rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 browsergym_workarena-0.1.0rc7/src/browsergym/workarena/tasks/scripts/navigation.py
--rw-r--r--   0        0        0     4862 2020-02-02 00:00:00.000000 browsergym_workarena-0.1.0rc7/src/browsergym/workarena/tasks/scripts/service_catalog.py
--rw-r--r--   0        0        0     7521 2020-02-02 00:00:00.000000 browsergym_workarena-0.1.0rc7/src/browsergym/workarena/tasks/scripts/validate.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 browsergym_workarena-0.1.0rc7/src/browsergym/workarena/tasks/utils/__init__.py
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 browsergym_workarena-0.1.0rc7/src/browsergym/workarena/tasks/utils/debug.py
--rw-r--r--   0        0        0     2487 2020-02-02 00:00:00.000000 browsergym_workarena-0.1.0rc7/src/browsergym/workarena/tasks/utils/form.py
--rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 browsergym_workarena-0.1.0rc7/src/browsergym/workarena/tasks/utils/js_utils.js
--rw-r--r--   0        0        0     2772 2020-02-02 00:00:00.000000 browsergym_workarena-0.1.0rc7/tests/test_random_config_generation.py
--rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 browsergym_workarena-0.1.0rc7/tests/test_snow_instance.py
--rw-r--r--   0        0        0    10010 2020-02-02 00:00:00.000000 browsergym_workarena-0.1.0rc7/tests/test_task_from_config.py
--rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 browsergym_workarena-0.1.0rc7/tests/test_task_general.py
--rw-r--r--   0        0        0     3170 2020-02-02 00:00:00.000000 browsergym_workarena-0.1.0rc7/tests/test_task_setup.py
--rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 browsergym_workarena-0.1.0rc7/tests/test_utils.py
--rw-r--r--   0        0        0     1216 2020-02-02 00:00:00.000000 browsergym_workarena-0.1.0rc7/tests/test_validate.py
--rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 browsergym_workarena-0.1.0rc7/tests/utils.py
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 browsergym_workarena-0.1.0rc7/LICENSE
--rw-r--r--   0        0        0     6388 2020-02-02 00:00:00.000000 browsergym_workarena-0.1.0rc7/README.md
--rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 browsergym_workarena-0.1.0rc7/pyproject.toml
--rw-r--r--   0        0        0     7240 2020-02-02 00:00:00.000000 browsergym_workarena-0.1.0rc7/PKG-INFO
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 browsergym_workarena-0.2.0/requirements.txt
+-rw-r--r--   0        0        0     3220 2020-02-02 00:00:00.000000 browsergym_workarena-0.2.0/.github/workflows/pypi.yml
+-rw-r--r--   0        0        0     2478 2020-02-02 00:00:00.000000 browsergym_workarena-0.2.0/.github/workflows/unit_tests.yml
+-rw-r--r--   0        0        0    58904 2020-02-02 00:00:00.000000 browsergym_workarena-0.2.0/scripts/generate_knowledge_base.ipynb
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 browsergym_workarena-0.2.0/src/browsergym/workarena/__init__.py
+-rw-r--r--   0        0        0     7761 2020-02-02 00:00:00.000000 browsergym_workarena-0.2.0/src/browsergym/workarena/config.py
+-rw-r--r--   0        0        0    36358 2020-02-02 00:00:00.000000 browsergym_workarena-0.2.0/src/browsergym/workarena/install.py
+-rw-r--r--   0        0        0     4314 2020-02-02 00:00:00.000000 browsergym_workarena-0.2.0/src/browsergym/workarena/instance.py
+-rw-r--r--   0        0        0     3199 2020-02-02 00:00:00.000000 browsergym_workarena-0.2.0/src/browsergym/workarena/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 browsergym_workarena-0.2.0/src/browsergym/workarena/api/__init__.py
+-rw-r--r--   0        0        0     4148 2020-02-02 00:00:00.000000 browsergym_workarena-0.2.0/src/browsergym/workarena/api/requests.py
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 browsergym_workarena-0.2.0/src/browsergym/workarena/api/ui_themes.py
+-rw-r--r--   0        0        0     4627 2020-02-02 00:00:00.000000 browsergym_workarena-0.2.0/src/browsergym/workarena/api/user.py
+-rw-r--r--   0        0        0     3315 2020-02-02 00:00:00.000000 browsergym_workarena-0.2.0/src/browsergym/workarena/api/utils.py
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 browsergym_workarena-0.2.0/src/browsergym/workarena/data_files/setup_files/forms/expected_change_request_form_fields.json
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 browsergym_workarena-0.2.0/src/browsergym/workarena/data_files/setup_files/forms/expected_hardware_form_fields.json
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 browsergym_workarena-0.2.0/src/browsergym/workarena/data_files/setup_files/forms/expected_incident_form_fields.json
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 browsergym_workarena-0.2.0/src/browsergym/workarena/data_files/setup_files/forms/expected_problem_form_fields.json
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 browsergym_workarena-0.2.0/src/browsergym/workarena/data_files/setup_files/forms/expected_user_form_fields.json
+-rw-r--r--   0        0        0    11500 2020-02-02 00:00:00.000000 browsergym_workarena-0.2.0/src/browsergym/workarena/data_files/setup_files/knowledge/kb_autopublish_workflow.xml
+-rw-r--r--   0        0        0   474939 2020-02-02 00:00:00.000000 browsergym_workarena-0.2.0/src/browsergym/workarena/data_files/setup_files/knowledge/knowledge_base.json
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 browsergym_workarena-0.2.0/src/browsergym/workarena/data_files/setup_files/lists/expected_asset_list_columns.json
+-rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 browsergym_workarena-0.2.0/src/browsergym/workarena/data_files/setup_files/lists/expected_change_request_list_columns.json
+-rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 browsergym_workarena-0.2.0/src/browsergym/workarena/data_files/setup_files/lists/expected_hardware_list_columns.json
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 browsergym_workarena-0.2.0/src/browsergym/workarena/data_files/setup_files/lists/expected_incident_list_columns.json
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 browsergym_workarena-0.2.0/src/browsergym/workarena/data_files/setup_files/lists/expected_service_catalog_list_columns.json
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 browsergym_workarena-0.2.0/src/browsergym/workarena/data_files/setup_files/lists/expected_user_list_columns.json
+-rw-r--r--   0        0        0  1970309 2020-02-02 00:00:00.000000 browsergym_workarena-0.2.0/src/browsergym/workarena/data_files/setup_files/ui_themes/workarena_themes.xml
+-rw-r--r--   0        0        0   270388 2020-02-02 00:00:00.000000 browsergym_workarena-0.2.0/src/browsergym/workarena/data_files/task_configs/all_menu.json
+-rw-r--r--   0        0        0  6306733 2020-02-02 00:00:00.000000 browsergym_workarena-0.2.0/src/browsergym/workarena/data_files/task_configs/create_change_request_task.json
+-rw-r--r--   0        0        0  4971385 2020-02-02 00:00:00.000000 browsergym_workarena-0.2.0/src/browsergym/workarena/data_files/task_configs/create_hardware_asset_task.json
+-rw-r--r--   0        0        0  5812616 2020-02-02 00:00:00.000000 browsergym_workarena-0.2.0/src/browsergym/workarena/data_files/task_configs/create_incident_task.json
+-rw-r--r--   0        0        0  4994349 2020-02-02 00:00:00.000000 browsergym_workarena-0.2.0/src/browsergym/workarena/data_files/task_configs/create_problem_task.json
+-rw-r--r--   0        0        0  3981025 2020-02-02 00:00:00.000000 browsergym_workarena-0.2.0/src/browsergym/workarena/data_files/task_configs/create_user_task.json
+-rw-r--r--   0        0        0    15733 2020-02-02 00:00:00.000000 browsergym_workarena-0.2.0/src/browsergym/workarena/data_files/task_configs/dashboard_retrieval_minmax_task.json
+-rw-r--r--   0        0        0   114629 2020-02-02 00:00:00.000000 browsergym_workarena-0.2.0/src/browsergym/workarena/data_files/task_configs/dashboard_retrieval_value_task.json
+-rw-r--r--   0        0        0 11882372 2020-02-02 00:00:00.000000 browsergym_workarena-0.2.0/src/browsergym/workarena/data_files/task_configs/filter_asset_list_task.json
+-rw-r--r--   0        0        0 12812288 2020-02-02 00:00:00.000000 browsergym_workarena-0.2.0/src/browsergym/workarena/data_files/task_configs/filter_change_request_list_task.json
+-rw-r--r--   0        0        0 12785357 2020-02-02 00:00:00.000000 browsergym_workarena-0.2.0/src/browsergym/workarena/data_files/task_configs/filter_hardware_list_task.json
+-rw-r--r--   0        0        0 11773863 2020-02-02 00:00:00.000000 browsergym_workarena-0.2.0/src/browsergym/workarena/data_files/task_configs/filter_incident_list_task.json
+-rw-r--r--   0        0        0  9231689 2020-02-02 00:00:00.000000 browsergym_workarena-0.2.0/src/browsergym/workarena/data_files/task_configs/filter_service_catalog_item_list_task.json
+-rw-r--r--   0        0        0 55965665 2020-02-02 00:00:00.000000 browsergym_workarena-0.2.0/src/browsergym/workarena/data_files/task_configs/filter_user_list_task.json
+-rw-r--r--   0        0        0    13021 2020-02-02 00:00:00.000000 browsergym_workarena-0.2.0/src/browsergym/workarena/data_files/task_configs/impersonation_users.json
+-rw-r--r--   0        0        0   617853 2020-02-02 00:00:00.000000 browsergym_workarena-0.2.0/src/browsergym/workarena/data_files/task_configs/knowledge_base_configs.json
+-rw-r--r--   0        0        0     1483 2020-02-02 00:00:00.000000 browsergym_workarena-0.2.0/src/browsergym/workarena/data_files/task_configs/order_apple_mac_book_pro15_task.json
+-rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 browsergym_workarena-0.2.0/src/browsergym/workarena/data_files/task_configs/order_apple_watch_task.json
+-rw-r--r--   0        0        0   610195 2020-02-02 00:00:00.000000 browsergym_workarena-0.2.0/src/browsergym/workarena/data_files/task_configs/order_developer_laptop_task.json
+-rw-r--r--   0        0        0    15666 2020-02-02 00:00:00.000000 browsergym_workarena-0.2.0/src/browsergym/workarena/data_files/task_configs/order_development_laptop_pc_task.json
+-rw-r--r--   0        0        0    27830 2020-02-02 00:00:00.000000 browsergym_workarena-0.2.0/src/browsergym/workarena/data_files/task_configs/order_ipad_mini_task.json
+-rw-r--r--   0        0        0    20828 2020-02-02 00:00:00.000000 browsergym_workarena-0.2.0/src/browsergym/workarena/data_files/task_configs/order_ipad_pro_task.json
+-rw-r--r--   0        0        0   183107 2020-02-02 00:00:00.000000 browsergym_workarena-0.2.0/src/browsergym/workarena/data_files/task_configs/order_loaner_laptop_task.json
+-rw-r--r--   0        0        0   707828 2020-02-02 00:00:00.000000 browsergym_workarena-0.2.0/src/browsergym/workarena/data_files/task_configs/order_sales_laptop_task.json
+-rw-r--r--   0        0        0   516203 2020-02-02 00:00:00.000000 browsergym_workarena-0.2.0/src/browsergym/workarena/data_files/task_configs/order_standard_laptop_task.json
+-rw-r--r--   0        0        0   112107 2020-02-02 00:00:00.000000 browsergym_workarena-0.2.0/src/browsergym/workarena/data_files/task_configs/report_retrieval_minmax_task.json
+-rw-r--r--   0        0        0   324394 2020-02-02 00:00:00.000000 browsergym_workarena-0.2.0/src/browsergym/workarena/data_files/task_configs/report_retrieval_value_task.json
+-rw-r--r--   0        0        0    44721 2020-02-02 00:00:00.000000 browsergym_workarena-0.2.0/src/browsergym/workarena/data_files/task_configs/sort_asset_list_task.json
+-rw-r--r--   0        0        0    45862 2020-02-02 00:00:00.000000 browsergym_workarena-0.2.0/src/browsergym/workarena/data_files/task_configs/sort_change_request_list_task.json
+-rw-r--r--   0        0        0    45127 2020-02-02 00:00:00.000000 browsergym_workarena-0.2.0/src/browsergym/workarena/data_files/task_configs/sort_hardware_list_task.json
+-rw-r--r--   0        0        0    45205 2020-02-02 00:00:00.000000 browsergym_workarena-0.2.0/src/browsergym/workarena/data_files/task_configs/sort_incident_list_task.json
+-rw-r--r--   0        0        0    46700 2020-02-02 00:00:00.000000 browsergym_workarena-0.2.0/src/browsergym/workarena/data_files/task_configs/sort_service_catalog_item_list_task.json
+-rw-r--r--   0        0        0    44336 2020-02-02 00:00:00.000000 browsergym_workarena-0.2.0/src/browsergym/workarena/data_files/task_configs/sort_user_list_task.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 browsergym_workarena-0.2.0/src/browsergym/workarena/tasks/__init__.py
+-rw-r--r--   0        0        0     5102 2020-02-02 00:00:00.000000 browsergym_workarena-0.2.0/src/browsergym/workarena/tasks/base.py
+-rw-r--r--   0        0        0    25240 2020-02-02 00:00:00.000000 browsergym_workarena-0.2.0/src/browsergym/workarena/tasks/dashboard.py
+-rw-r--r--   0        0        0    32095 2020-02-02 00:00:00.000000 browsergym_workarena-0.2.0/src/browsergym/workarena/tasks/form.py
+-rw-r--r--   0        0        0     6358 2020-02-02 00:00:00.000000 browsergym_workarena-0.2.0/src/browsergym/workarena/tasks/knowledge.py
+-rw-r--r--   0        0        0    37779 2020-02-02 00:00:00.000000 browsergym_workarena-0.2.0/src/browsergym/workarena/tasks/list.py
+-rw-r--r--   0        0        0     7399 2020-02-02 00:00:00.000000 browsergym_workarena-0.2.0/src/browsergym/workarena/tasks/navigation.py
+-rw-r--r--   0        0        0    22964 2020-02-02 00:00:00.000000 browsergym_workarena-0.2.0/src/browsergym/workarena/tasks/service_catalog.py
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 browsergym_workarena-0.2.0/src/browsergym/workarena/tasks/scripts/README.md
+-rw-r--r--   0        0        0     9870 2020-02-02 00:00:00.000000 browsergym_workarena-0.2.0/src/browsergym/workarena/tasks/scripts/extract_all_menu_items.py
+-rw-r--r--   0        0        0     9915 2020-02-02 00:00:00.000000 browsergym_workarena-0.2.0/src/browsergym/workarena/tasks/scripts/generate_dashboard_configs.py
+-rw-r--r--   0        0        0     3695 2020-02-02 00:00:00.000000 browsergym_workarena-0.2.0/src/browsergym/workarena/tasks/scripts/generate_forms.py
+-rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 browsergym_workarena-0.2.0/src/browsergym/workarena/tasks/scripts/knowledge.py
+-rw-r--r--   0        0        0     4803 2020-02-02 00:00:00.000000 browsergym_workarena-0.2.0/src/browsergym/workarena/tasks/scripts/list.py
+-rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 browsergym_workarena-0.2.0/src/browsergym/workarena/tasks/scripts/navigation.py
+-rw-r--r--   0        0        0     4862 2020-02-02 00:00:00.000000 browsergym_workarena-0.2.0/src/browsergym/workarena/tasks/scripts/service_catalog.py
+-rw-r--r--   0        0        0     7521 2020-02-02 00:00:00.000000 browsergym_workarena-0.2.0/src/browsergym/workarena/tasks/scripts/validate.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 browsergym_workarena-0.2.0/src/browsergym/workarena/tasks/utils/__init__.py
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 browsergym_workarena-0.2.0/src/browsergym/workarena/tasks/utils/debug.py
+-rw-r--r--   0        0        0     2519 2020-02-02 00:00:00.000000 browsergym_workarena-0.2.0/src/browsergym/workarena/tasks/utils/form.py
+-rw-r--r--   0        0        0     5199 2020-02-02 00:00:00.000000 browsergym_workarena-0.2.0/src/browsergym/workarena/tasks/utils/js_utils.js
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 browsergym_workarena-0.2.0/src/browsergym/workarena/tasks/utils/string.py
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 browsergym_workarena-0.2.0/src/browsergym/workarena/tasks/utils/utils.py
+-rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 browsergym_workarena-0.2.0/tests/test_api.py
+-rw-r--r--   0        0        0     2834 2020-02-02 00:00:00.000000 browsergym_workarena-0.2.0/tests/test_random_config_generation.py
+-rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 browsergym_workarena-0.2.0/tests/test_snow_instance.py
+-rw-r--r--   0        0        0    10010 2020-02-02 00:00:00.000000 browsergym_workarena-0.2.0/tests/test_task_from_config.py
+-rw-r--r--   0        0        0     1348 2020-02-02 00:00:00.000000 browsergym_workarena-0.2.0/tests/test_task_general.py
+-rw-r--r--   0        0        0     3869 2020-02-02 00:00:00.000000 browsergym_workarena-0.2.0/tests/test_task_setup.py
+-rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 browsergym_workarena-0.2.0/tests/test_utils.py
+-rw-r--r--   0        0        0     1216 2020-02-02 00:00:00.000000 browsergym_workarena-0.2.0/tests/test_validate.py
+-rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 browsergym_workarena-0.2.0/tests/utils.py
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 browsergym_workarena-0.2.0/.gitignore
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 browsergym_workarena-0.2.0/LICENSE
+-rw-r--r--   0        0        0     6737 2020-02-02 00:00:00.000000 browsergym_workarena-0.2.0/README.md
+-rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 browsergym_workarena-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     7641 2020-02-02 00:00:00.000000 browsergym_workarena-0.2.0/PKG-INFO
```

### Comparing `browsergym_workarena-0.1.0rc7/.github/workflows/pypi.yml` & `browsergym_workarena-0.2.0/.github/workflows/pypi.yml`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-name: Publish Python 🐍 distribution 📦 to PyPI and TestPyPI
+name: Build and Publish
 
 on: [push, workflow_dispatch]
 
 jobs:
     build:
       name: Build
       runs-on: ubuntu-latest
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `browsergym_workarena-0.1.0rc7/scripts/generate_knowledge_base.ipynb` & `browsergym_workarena-0.2.0/scripts/generate_knowledge_base.ipynb`

 * *Files identical despite different names*

### Comparing `browsergym_workarena-0.1.0rc7/src/browsergym/workarena/config.py` & `browsergym_workarena-0.2.0/src/browsergym/workarena/config.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,18 +3,33 @@
 from ..workarena import data_files
 from ..workarena.tasks import utils
 
 # ServiceNow configuration
 SNOW_DATA_LOOKBACK_MINUTES = 5
 SNOW_BROWSER_TIMEOUT = 30000  # Milliseconds
 SNOW_JS_UTILS_FILEPATH = str(resources.files(utils).joinpath("js_utils.js"))
-SNOW_SUPPORTED_RELEASES = ["utah"]
+SNOW_SUPPORTED_RELEASES = ["washingtondc"]
 
 # Path to the Menu navigation task configuration
 ALL_MENU_PATH = str(resources.files(data_files).joinpath("task_configs/all_menu.json"))
+
+# Path to the dashboard/report retrieval task configurations
+DASHBOARD_RETRIEVAL_MINMAX_CONFIG_PATH = str(
+    resources.files(data_files).joinpath("task_configs/dashboard_retrieval_minmax_task.json")
+)
+DASHBOARD_RETRIEVAL_VALUE_CONFIG_PATH = str(
+    resources.files(data_files).joinpath("task_configs/dashboard_retrieval_value_task.json")
+)
+REPORT_RETRIEVAL_MINMAX_CONFIG_PATH = str(
+    resources.files(data_files).joinpath("task_configs/report_retrieval_minmax_task.json")
+)
+REPORT_RETRIEVAL_VALUE_CONFIG_PATH = str(
+    resources.files(data_files).joinpath("task_configs/report_retrieval_value_task.json")
+)
+
 # Path to knowledge base task configurations
 KB_CONFIG_PATH = str(
     resources.files(data_files).joinpath("task_configs/knowledge_base_configs.json")
 )
 # Path to the Impersonation task configuration
 IMPERSONATION_CONFIG_PATH = str(
     resources.files(data_files).joinpath("task_configs/impersonation_users.json")
@@ -115,14 +130,36 @@
             resources.files(data_files).joinpath(
                 "setup_files/knowledge/kb_autopublish_workflow.xml"
             )
         ),
     }
 }
 
+
+# Custom UI Themes
+UI_THEMES_UPDATE_SET = {
+    "name": "WorkArena UI Themes",
+    "update_set": str(
+        resources.files(data_files).joinpath("setup_files/ui_themes/workarena_themes.xml")
+    ),
+    "variants": [
+        "Astranova",
+        "Charlies",
+        "Great pasta",
+        "Mighty capital",
+        "Speedy tires",
+        "Skyward",
+        "Turbobots",
+        "Ultrashoes",
+        "Vitasphere",
+        "Workarena",
+    ],
+}
+
+
 # Expected columns for list tasks; used in setup
 EXPECTED_ASSET_LIST_COLUMNS_PATH = str(
     resources.files(data_files).joinpath("setup_files/lists/expected_asset_list_columns.json")
 )
 EXPECTED_CHANGE_REQUEST_COLUMNS_PATH = str(
     resources.files(data_files).joinpath(
         "setup_files/lists/expected_change_request_list_columns.json"
@@ -159,7 +196,12 @@
 )
 EXPECTED_PROBLEM_FORM_FIELDS_PATH = str(
     resources.files(data_files).joinpath("setup_files/forms/expected_problem_form_fields.json")
 )
 EXPECTED_USER_FORM_FIELDS_PATH = str(
     resources.files(data_files).joinpath("setup_files/forms/expected_user_form_fields.json")
 )
+
+
+# Report date filter patch flag
+REPORT_PATCH_FLAG = "WORKARENA_DATE_FILTER_PATCH"
+REPORT_DATE_FILTER = "2024-04-01"
```

### Comparing `browsergym_workarena-0.1.0rc7/src/browsergym/workarena/instance.py` & `browsergym_workarena-0.2.0/src/browsergym/workarena/instance.py`

 * *Files identical despite different names*

### Comparing `browsergym_workarena-0.1.0rc7/src/browsergym/workarena/utils.py` & `browsergym_workarena-0.2.0/src/browsergym/workarena/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         The page instance to use for the impersonation (you must be logged in as admin)
 
     Notes:
     ------
     * If you provide a username that matches to multiple users (e.g., a partial one), the first one will be selected
 
     """
-    page.get_by_label("Avatar: available, user preferences").click()
+    page.locator(".header-avatar-button").click()
     page.get_by_role("menuitem", name="Impersonate user").click()
     page.locator("input.now-typeahead-native-input").click()
     page.locator("input.now-typeahead-native-input").fill(username)
     page.locator("seismic-hoist").get_by_role("option", name=username).first.click()
     with page.expect_navigation():
         page.get_by_role("button", name="Impersonate user").click()
 
@@ -63,8 +63,37 @@
         page.get_by_label("Password", exact=True).fill(snow_password)
         with page.expect_navigation():
             page.get_by_role("button", name="Log in").click()
 
     # Check if we have been returned to the login page (appends /welcome.do)
     current_url = parse.urlparse(parse.unquote(page.evaluate("() => window.location.href")))
     if current_url.path.endswith("/welcome.do"):
-        raise RuntimeError("Login failed.")
+        raise RuntimeError("Login failed. Check credentials.")
+
+
+def url_login(instance: SNowInstance, page: playwright.sync_api.Page):
+    """
+    Log into the instance via the URL
+
+    Parameters:
+    -----------
+    instance:
+        The instance to log into
+    page:
+        The page instance to use for the URL login
+
+    """
+    (snow_username, snow_password) = instance.snow_credentials
+
+    # Encode special characters
+    snow_username = parse.quote(snow_username)
+    snow_password = parse.quote(snow_password)
+
+    # Log in via URL
+    page.goto(
+        f"{instance.snow_url}/login.do?user_name={snow_username}&user_password={snow_password}&sys_action=sysverb_login"
+    )
+
+    # Check if we have been returned to the login page
+    current_url = parse.urlparse(parse.unquote(page.evaluate("() => window.location.href")))
+    if "login.do" in current_url.path:
+        raise RuntimeError("Login failed. Check credentials and make sure to have run installer.")
```

### Comparing `browsergym_workarena-0.1.0rc7/src/browsergym/workarena/api/requests.py` & `browsergym_workarena-0.2.0/src/browsergym/workarena/api/requests.py`

 * *Files identical despite different names*

### Comparing `browsergym_workarena-0.1.0rc7/src/browsergym/workarena/api/utils.py` & `browsergym_workarena-0.2.0/src/browsergym/workarena/api/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,15 +82,15 @@
         headers=SNOW_API_HEADERS,
     )
     response.raise_for_status()
     meta_info = response.json()["result"]["columns"]
 
     # Clean column value choices
     for info in meta_info.values():
-        if "choices" in info:
+        if info.get("choices", None):
             info["choices"] = {c["value"]: c["label"] for c in info["choices"]}
 
     # Query the sys_dictionnary table to find more info (e.g., is this column dependent on another)
     sys_dict_info = table_api_call(
         instance=instance,
         table="sys_dictionary",
         params={
```

### Comparing `browsergym_workarena-0.1.0rc7/src/browsergym/workarena/data_files/setup_files/forms/expected_hardware_form_fields.json` & `browsergym_workarena-0.2.0/src/browsergym/workarena/data_files/setup_files/forms/expected_hardware_form_fields.json`

 * *Files identical despite different names*

### Comparing `browsergym_workarena-0.1.0rc7/src/browsergym/workarena/data_files/setup_files/forms/expected_problem_form_fields.json` & `browsergym_workarena-0.2.0/src/browsergym/workarena/data_files/setup_files/forms/expected_problem_form_fields.json`

 * *Files identical despite different names*

### Comparing `browsergym_workarena-0.1.0rc7/src/browsergym/workarena/data_files/setup_files/knowledge/kb_autopublish_workflow.xml` & `browsergym_workarena-0.2.0/src/browsergym/workarena/data_files/setup_files/knowledge/kb_autopublish_workflow.xml`

 * *Files identical despite different names*

### Comparing `browsergym_workarena-0.1.0rc7/src/browsergym/workarena/data_files/setup_files/knowledge/knowledge_base.json` & `browsergym_workarena-0.2.0/src/browsergym/workarena/data_files/setup_files/knowledge/knowledge_base.json`

 * *Files identical despite different names*

### Comparing `browsergym_workarena-0.1.0rc7/src/browsergym/workarena/data_files/setup_files/lists/expected_asset_list_columns.json` & `browsergym_workarena-0.2.0/src/browsergym/workarena/data_files/setup_files/lists/expected_asset_list_columns.json`

 * *Files identical despite different names*

### Comparing `browsergym_workarena-0.1.0rc7/src/browsergym/workarena/data_files/setup_files/lists/expected_change_request_list_columns.json` & `browsergym_workarena-0.2.0/src/browsergym/workarena/data_files/setup_files/lists/expected_change_request_list_columns.json`

 * *Files identical despite different names*

### Comparing `browsergym_workarena-0.1.0rc7/src/browsergym/workarena/data_files/setup_files/lists/expected_hardware_list_columns.json` & `browsergym_workarena-0.2.0/src/browsergym/workarena/data_files/setup_files/lists/expected_hardware_list_columns.json`

 * *Files identical despite different names*

### Comparing `browsergym_workarena-0.1.0rc7/src/browsergym/workarena/data_files/setup_files/lists/expected_service_catalog_list_columns.json` & `browsergym_workarena-0.2.0/src/browsergym/workarena/data_files/setup_files/lists/expected_service_catalog_list_columns.json`

 * *Files identical despite different names*

### Comparing `browsergym_workarena-0.1.0rc7/src/browsergym/workarena/data_files/setup_files/lists/expected_user_list_columns.json` & `browsergym_workarena-0.2.0/src/browsergym/workarena/data_files/setup_files/lists/expected_user_list_columns.json`

 * *Files identical despite different names*

### Comparing `browsergym_workarena-0.1.0rc7/src/browsergym/workarena/data_files/task_configs/all_menu.json` & `browsergym_workarena-0.2.0/src/browsergym/workarena/data_files/task_configs/all_menu.json`

 * *Files identical despite different names*

### Comparing `browsergym_workarena-0.1.0rc7/src/browsergym/workarena/data_files/task_configs/create_change_request_task.json` & `browsergym_workarena-0.2.0/src/browsergym/workarena/data_files/task_configs/create_change_request_task.json`

 * *Files identical despite different names*

### Comparing `browsergym_workarena-0.1.0rc7/src/browsergym/workarena/data_files/task_configs/create_hardware_asset_task.json` & `browsergym_workarena-0.2.0/src/browsergym/workarena/data_files/task_configs/create_hardware_asset_task.json`

 * *Files identical despite different names*

### Comparing `browsergym_workarena-0.1.0rc7/src/browsergym/workarena/data_files/task_configs/create_incident_task.json` & `browsergym_workarena-0.2.0/src/browsergym/workarena/data_files/task_configs/create_incident_task.json`

 * *Files identical despite different names*

### Comparing `browsergym_workarena-0.1.0rc7/src/browsergym/workarena/data_files/task_configs/create_problem_task.json` & `browsergym_workarena-0.2.0/src/browsergym/workarena/data_files/task_configs/create_problem_task.json`

 * *Files identical despite different names*

### Comparing `browsergym_workarena-0.1.0rc7/src/browsergym/workarena/data_files/task_configs/create_user_task.json` & `browsergym_workarena-0.2.0/src/browsergym/workarena/data_files/task_configs/create_user_task.json`

 * *Files identical despite different names*

### Comparing `browsergym_workarena-0.1.0rc7/src/browsergym/workarena/data_files/task_configs/filter_asset_list_task.json` & `browsergym_workarena-0.2.0/src/browsergym/workarena/data_files/task_configs/filter_asset_list_task.json`

 * *Files identical despite different names*

### Comparing `browsergym_workarena-0.1.0rc7/src/browsergym/workarena/data_files/task_configs/filter_change_request_list_task.json` & `browsergym_workarena-0.2.0/src/browsergym/workarena/data_files/task_configs/filter_change_request_list_task.json`

 * *Files identical despite different names*

### Comparing `browsergym_workarena-0.1.0rc7/src/browsergym/workarena/data_files/task_configs/filter_hardware_list_task.json` & `browsergym_workarena-0.2.0/src/browsergym/workarena/data_files/task_configs/filter_hardware_list_task.json`

 * *Files identical despite different names*

### Comparing `browsergym_workarena-0.1.0rc7/src/browsergym/workarena/data_files/task_configs/filter_incident_list_task.json` & `browsergym_workarena-0.2.0/src/browsergym/workarena/data_files/task_configs/filter_incident_list_task.json`

 * *Files identical despite different names*

### Comparing `browsergym_workarena-0.1.0rc7/src/browsergym/workarena/data_files/task_configs/filter_service_catalog_item_list_task.json` & `browsergym_workarena-0.2.0/src/browsergym/workarena/data_files/task_configs/filter_service_catalog_item_list_task.json`

 * *Files identical despite different names*

### Comparing `browsergym_workarena-0.1.0rc7/src/browsergym/workarena/data_files/task_configs/filter_user_list_task.json` & `browsergym_workarena-0.2.0/src/browsergym/workarena/data_files/task_configs/filter_user_list_task.json`

 * *Files identical despite different names*

### Comparing `browsergym_workarena-0.1.0rc7/src/browsergym/workarena/data_files/task_configs/impersonation_users.json` & `browsergym_workarena-0.2.0/src/browsergym/workarena/data_files/task_configs/impersonation_users.json`

 * *Files identical despite different names*

### Comparing `browsergym_workarena-0.1.0rc7/src/browsergym/workarena/data_files/task_configs/knowledge_base_configs.json` & `browsergym_workarena-0.2.0/src/browsergym/workarena/data_files/task_configs/knowledge_base_configs.json`

 * *Files identical despite different names*

### Comparing `browsergym_workarena-0.1.0rc7/src/browsergym/workarena/data_files/task_configs/order_apple_mac_book_pro15_task.json` & `browsergym_workarena-0.2.0/src/browsergym/workarena/data_files/task_configs/order_apple_mac_book_pro15_task.json`

 * *Files identical despite different names*

### Comparing `browsergym_workarena-0.1.0rc7/src/browsergym/workarena/data_files/task_configs/order_apple_watch_task.json` & `browsergym_workarena-0.2.0/src/browsergym/workarena/data_files/task_configs/order_apple_watch_task.json`

 * *Files identical despite different names*

### Comparing `browsergym_workarena-0.1.0rc7/src/browsergym/workarena/data_files/task_configs/order_developer_laptop_task.json` & `browsergym_workarena-0.2.0/src/browsergym/workarena/data_files/task_configs/order_developer_laptop_task.json`

 * *Files identical despite different names*

### Comparing `browsergym_workarena-0.1.0rc7/src/browsergym/workarena/data_files/task_configs/order_development_laptop_pc_task.json` & `browsergym_workarena-0.2.0/src/browsergym/workarena/data_files/task_configs/order_development_laptop_pc_task.json`

 * *Files identical despite different names*

### Comparing `browsergym_workarena-0.1.0rc7/src/browsergym/workarena/data_files/task_configs/order_ipad_mini_task.json` & `browsergym_workarena-0.2.0/src/browsergym/workarena/data_files/task_configs/order_ipad_mini_task.json`

 * *Files identical despite different names*

### Comparing `browsergym_workarena-0.1.0rc7/src/browsergym/workarena/data_files/task_configs/order_ipad_pro_task.json` & `browsergym_workarena-0.2.0/src/browsergym/workarena/data_files/task_configs/order_ipad_pro_task.json`

 * *Files identical despite different names*

### Comparing `browsergym_workarena-0.1.0rc7/src/browsergym/workarena/data_files/task_configs/order_loaner_laptop_task.json` & `browsergym_workarena-0.2.0/src/browsergym/workarena/data_files/task_configs/order_loaner_laptop_task.json`

 * *Files identical despite different names*

### Comparing `browsergym_workarena-0.1.0rc7/src/browsergym/workarena/data_files/task_configs/order_sales_laptop_task.json` & `browsergym_workarena-0.2.0/src/browsergym/workarena/data_files/task_configs/order_sales_laptop_task.json`

 * *Files identical despite different names*

### Comparing `browsergym_workarena-0.1.0rc7/src/browsergym/workarena/data_files/task_configs/order_standard_laptop_task.json` & `browsergym_workarena-0.2.0/src/browsergym/workarena/data_files/task_configs/order_standard_laptop_task.json`

 * *Files identical despite different names*

### Comparing `browsergym_workarena-0.1.0rc7/src/browsergym/workarena/data_files/task_configs/sort_asset_list_task.json` & `browsergym_workarena-0.2.0/src/browsergym/workarena/data_files/task_configs/sort_asset_list_task.json`

 * *Files identical despite different names*

### Comparing `browsergym_workarena-0.1.0rc7/src/browsergym/workarena/data_files/task_configs/sort_change_request_list_task.json` & `browsergym_workarena-0.2.0/src/browsergym/workarena/data_files/task_configs/sort_change_request_list_task.json`

 * *Files identical despite different names*

### Comparing `browsergym_workarena-0.1.0rc7/src/browsergym/workarena/data_files/task_configs/sort_hardware_list_task.json` & `browsergym_workarena-0.2.0/src/browsergym/workarena/data_files/task_configs/sort_hardware_list_task.json`

 * *Files identical despite different names*

### Comparing `browsergym_workarena-0.1.0rc7/src/browsergym/workarena/data_files/task_configs/sort_incident_list_task.json` & `browsergym_workarena-0.2.0/src/browsergym/workarena/data_files/task_configs/sort_incident_list_task.json`

 * *Files identical despite different names*

### Comparing `browsergym_workarena-0.1.0rc7/src/browsergym/workarena/data_files/task_configs/sort_service_catalog_item_list_task.json` & `browsergym_workarena-0.2.0/src/browsergym/workarena/data_files/task_configs/sort_service_catalog_item_list_task.json`

 * *Files identical despite different names*

### Comparing `browsergym_workarena-0.1.0rc7/src/browsergym/workarena/data_files/task_configs/sort_user_list_task.json` & `browsergym_workarena-0.2.0/src/browsergym/workarena/data_files/task_configs/sort_user_list_task.json`

 * *Files identical despite different names*

### Comparing `browsergym_workarena-0.1.0rc7/src/browsergym/workarena/tasks/form.py` & `browsergym_workarena-0.2.0/src/browsergym/workarena/tasks/form.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import playwright.sync_api
 import re
 
 from english_words import get_english_words_set
 from playwright.sync_api._generated import Page
 from time import sleep
 from typing import List, Tuple
+from urllib import parse
 
 from ..api.utils import (
     db_delete_from_table,
     table_api_call,
     table_column_info,
     HTTPError,
 )
@@ -28,22 +29,24 @@
     EXPECTED_HARDWARE_FORM_FIELDS_PATH,
     EXPECTED_INCIDENT_FORM_FIELDS_PATH,
     EXPECTED_PROBLEM_FORM_FIELDS_PATH,
     EXPECTED_USER_FORM_FIELDS_PATH,
 )
 from ..instance import SNowInstance
 from .utils.form import fill_text
+from .utils.utils import check_url_suffix_match
 
 
 ENGLISH_WORDS = list(get_english_words_set(["web2"]))
 
 
 class ServiceNowFormTask(AbstractServiceNowTask):
     def __init__(
         self,
+        seed: int,
         start_rel_url,
         instance: SNowInstance = None,
         extra_mandatory_fields: List = [],
         prohibited_fields: List = [],
     ) -> None:
         # The type of fields that we support interacting with
         self.supported_types = [
@@ -64,15 +67,15 @@
 
         # Extra mandatory fields (overriding the page specification)
         self.extra_mandatory_fields = extra_mandatory_fields
 
         # Prohibited fields: fields that we shouldn't interact with
         self.prohibited_fields = prohibited_fields
 
-        super().__init__(instance=instance, start_rel_url=start_rel_url)
+        super().__init__(seed=seed, instance=instance, start_rel_url=start_rel_url)
 
     def _get_form(self, page):
         """
         Loads a bunch of info about the form on a page into object variables
 
         """
 
@@ -101,18 +104,27 @@
             table="sys_db_object",
             params={
                 "sysparm_query": f"name={self.table_name}",
             },
         )["result"][0]["label"].lower()
 
         # Get the form fields
+        def is_field_visible(field):
+            return page.evaluate(
+                f"""
+                {self.form_js_selector}.isVisible(
+                    {self.form_js_selector}.getGlideUIElement('{field}'),
+                    {self.form_js_selector}.getControl('{field}')
+                );"""
+            )
+
         logging.debug("Extracting valid form fields")
         editable_fields = page.evaluate(f"{self.form_js_selector}.getEditableFields()")
         field_elements = page.evaluate(f"{self.form_js_selector}.elements")
-        all_visible_fields = [f["fieldName"] for f in field_elements]
+        all_fields = [f["fieldName"] for f in field_elements]
         self.fields = {
             f["fieldName"]: f
             for f in field_elements
             if f["fieldName"] in editable_fields
             and f["fieldName"] not in self.prohibited_fields
             and f["type"] in self.supported_types
             and self.table_metadata[f["fieldName"]].get(
@@ -125,24 +137,33 @@
             self.fields[f]["label"] = page.evaluate(f"{self.form_js_selector}.getLabelOf('{f}')")
 
         # Split them into mandatory and optional
         self.mandatory_fields = [f for f in self.fields.keys() if self.fields[f]["mandatory"]]
         self.optional_fields = [f for f in set(self.fields.keys()) - set(self.mandatory_fields)]
 
         # Sanity check
-        assert len(self.fields) > 0, "No editable fields found."
+        assert len(self.fields) > 0, "No fields found on page."
+        assert len(editable_fields) > 0, "No editable fields found on page."
+        # ... check that the script that marks some fields as mandatory worked
         assert set(self.extra_mandatory_fields) <= set(
             self.mandatory_fields
         ), "Some extra mandatory fields are not mandatory in the form."
+        # ... check that the script that makes some fields read-only worked
         assert all(
             f not in self.fields for f in self.prohibited_fields
         ), "Some prohibited fields are editable in the form."
-        assert set(all_visible_fields) == set(
-            self.expected_fields
-        ), "Some fields are missing from the form., Re-run workarena-install to correct this."
+        # ... check that all the fields that the config expects are present and that extra fields are not visible
+        all_visible_fields = set([f for f in all_fields if is_field_visible(f)])
+        expected_visible_fields = set([f for f in self.expected_fields if is_field_visible(f)])
+        set_diff = all_visible_fields.union(
+            expected_visible_fields
+        ) - all_visible_fields.intersection(expected_visible_fields)
+        assert (
+            len(set_diff) == 0
+        ), f"The fields {set_diff} are either missing or unexpectedly visible on the form. Re-run 'workarena-install' to correct this."
 
     def _preprocess_fields(self, field, value):
         """
         Do some preprocessing on loaded fields
 
         For example, we don't want to load old dates since they won't match newly created entries
 
@@ -169,15 +190,15 @@
             if value is not None:
                 value = value.strip().replace("\n", "").replace("\r", "")
 
         return value
 
     def _wait_for_ready(self, page: Page) -> None:
         """
-        Waits for the main iframe to be fully loaded
+        Waits for the main iframe to be fully loaded.
 
         """
         logging.debug(f"Waiting for {self.js_prefix} to be fully loaded")
         page.wait_for_function(
             f"typeof window.{self.js_prefix} !== 'undefined' && window.{self.js_prefix}.WORKARENA_LOAD_COMPLETE",
         )
         logging.debug(f"Detected {self.js_prefix} ready")
@@ -186,41 +207,35 @@
         page.wait_for_function(f"window.{self.form_js_selector}")
         logging.debug("Detected Glide form API ready")
 
         logging.debug("Waiting for Glide tabs API to be available")
         page.wait_for_function(f"typeof window.{self.js_prefix}.g_tabs2Sections !== 'undefined'")
         logging.debug("Detected Glide tabs API ready")
 
-    def pre_setup(self, seed: int, page: Page):
-        super().pre_setup(seed, page)
+    def get_init_scripts(self) -> List[str]:
+        # Extract expected URL suffix
+        url_suffix = parse.urlparse(self.start_url).path.split("/")[-1]
+
+        # Add a few initialization scripts
+        return super().get_init_scripts() + [
+            "registerGsftMainLoaded();",
+            # ... Mark the extra mandatory fields as such
+            f"""
+                function addFormMandatoryFields() {{
+                    waLog('Setting mandatory fields', 'addFormMandatoryFields');
+                    {";".join([f"{self.js_api_forms}.setMandatory('{f}', true)" for f in self.extra_mandatory_fields])}
+                    waLog('Mandatory fields set successfully.', 'addFormMandatoryFields');
+                }}
 
-        # Register a few initialization scripts
-        self._add_init_scripts_to_context_and_reload(
-            page,
-            [
-                "registerGsftMainLoaded();",
-                # ... Mark the extra mandatory fields as such
-                f"""
-            // Check that the script is running in the main iframe
-            if (window.frameElement?.id === '{self.js_prefix}') {{
-                waLog('Setting mandatory fields');
-                waitForCondition(() => typeof {self.js_api_forms} !== 'undefined', 100)
-                .then(waitForCondition(() => typeof window.WORKARENA_LOAD_COMPLETE !== 'undefined' && window.WORKARENA_LOAD_COMPLETE, 100)
-                    .then(
-                        function (){{
-                            {';'.join([self.js_api_forms + '.setMandatory("' + f + '", true)' for f in self.extra_mandatory_fields])}
-                            waLog('Mandatory fields set successfully.');
-                        }}
-                    )
-                );
-            }}
-            """,
-            ],
-        )
+                runInGsftMainOnlyAndProtectByURL(addFormMandatoryFields, '{url_suffix}');
+                """,
+        ]
 
+    def start(self, page: Page) -> None:
+        super().start(page)
         self._wait_for_ready(page)
         self._get_form(page)
 
 
 class GenericNewRecordTask(ServiceNowFormTask):
     """
     Generic task to create a new record in a table using a Glide form.
@@ -248,33 +263,39 @@
         The path to the JSON file containing all configurations for the task. Provided by subclasses
     expected_fields_path:
         The path to the JSON file containing all expected fields for the task. Provided by subclasses
     """
 
     def __init__(
         self,
+        seed: int,
         form_url: str,
+        table_label: str,
         instance: SNowInstance = None,
         extra_mandatory_fields: List = [],
         prohibited_fields: List = [],
         unique_valued_fields: dict = {},
         min_fields: int = 5,
         max_fields: int = None,
         fixed_config: dict = None,
         config_path: str = None,
         expected_fields_path: str = None,
     ) -> None:
         super().__init__(
+            seed=seed,
             instance=instance,
             start_rel_url=form_url,
             extra_mandatory_fields=extra_mandatory_fields,
             prohibited_fields=prohibited_fields,
         )
         self.form_url = form_url
 
+        # Table pretty printed name
+        self.table_label = table_label
+
         # Key in which the sys_id of the created record will be stored in the local storage
         self.session_sys_id_field = f"{id(self)}.record_sys_id"
 
         # Fields that should have a unique value (will append them with a uuid)
         self.unique_valued_fields = unique_valued_fields
 
         # Maximum number of fields to fill (except if mandatory is more)
@@ -290,78 +311,73 @@
         if config_path:
             with open(config_path, "r") as f:
                 self.all_configs = json.load(f)
         if expected_fields_path:
             with open(expected_fields_path, "r") as f:
                 self.expected_fields = json.load(f)
 
-    def setup(self, seed: int, page: Page) -> tuple[str, dict]:
-        self.pre_setup(seed, page)
-        self._run_init_scripts(page)
+    def get_init_scripts(self) -> List[str]:
+        # Extract expected URL suffix
+        url_suffix = parse.urlparse(self.start_url).path.split("/")[-1]
+
+        # Add a few initialization scripts
+        return super().get_init_scripts() + [
+            f"""
+                function patchSubmitButton() {{
+                    waLog('Attempting to override form submit function', 'patchSubmitButton');
+                    // Save the original function if it hasn't been saved yet
+                    if(typeof old_gsftSubmit == 'undefined'){{
+                        old_gsftSubmit = new Function('return ' + gsftSubmit.toString())();
+                        waLog('Saved original submit function', 'patchSubmitButton');
+                    }}
+
+                    // Override the function to save the sys_id in the local storage
+                    gsftSubmit = function(control, form, action_name) {{
+                        localStorage['{self.session_sys_id_field}'] = {self.js_api_forms}.getUniqueValue();
+                        old_gsftSubmit(control, form, action_name);
+                    }};
+                    waLog('Patched submit function. All done.', 'patchSubmitButton');
+                }}
+
+                runInGsftMainOnlyAndProtectByURL(patchSubmitButton, '{url_suffix}');
+                """
+        ]
+
+    def setup_goal(self, page: Page) -> tuple[str, dict]:
+        super().setup_goal(page=page)
+
+        # Get the task configuration
         assert self.all_configs is not None, "No configuration available for the task."
         config = self.fixed_config if self.fixed_config else self.random.choice(self.all_configs)
-
         self.template_record = config["template_record"]
         for f, func in self.unique_valued_fields.items():
             self.template_record[f] = func(self.template_record[f])
-
         self.task_fields = config["task_fields"]
         self.created_sysids = []
 
-        # generate the goal
+        # Generate the goal
         goal = (
             f"Create a new {self.table_label} with "
             + " and ".join(
                 [
                     f'a value of "{self.template_record[f]}"'
-                    + f' for field "{self.fields[f]["label"]}"'
+                    + f' for field "{config["fields"][f]}"'
                     for f in self.task_fields
                 ]
             )
             + "."
         )
         info = {}
-        return goal, info
 
-    def _run_init_scripts(self, page: Page) -> None:
-        self._add_init_scripts_to_context_and_reload(
-            page,
-            [
-                f"""
-            // Check that the script is running in the main iframe
-            if (window.frameElement?.id === '{self.js_prefix}') {{
-                waLog('Attempting to override form submit function');
-                waitForCondition(() => typeof {self.js_api_forms} !== 'undefined', 100)
-                .then(waitForCondition(() => typeof gsftSubmit !== 'undefined', 100)
-                    .then(
-                        function overrideSubmit(){{
-                            // Save the original function if it hasn't been saved yet
-                            if(typeof old_gsftSubmit == 'undefined'){{
-                                old_gsftSubmit = new Function('return ' + gsftSubmit.toString())();
-                                waLog('Saved original submit function');
-                            }}
-
-                            // Override the function to save the sys_id in the local storage
-                            gsftSubmit = function(control, form, action_name) {{
-                                localStorage['{self.session_sys_id_field}'] = {self.js_api_forms}.getUniqueValue();
-                                old_gsftSubmit(control, form, action_name);
-                            }};
-                            waLog('Patched submit function. All done.');
-                        }}
-                    )
-                );
-            }}
-            """
-            ],
-        )
+        return goal, info
 
-    def _generate_random_config(self, seed: int, page: Page) -> None:
+    def _generate_random_config(self, page: Page) -> None:
         """Generate a random configuration for the task."""
-        self.pre_setup(seed, page)
-        self._run_init_scripts(page)
+        self.setup(page=page)
+
         # Determine task fields
         logging.debug("Determining task fields")
         # ... check that we have enough fields
         assert (
             len(self.fields) >= self.min_fields
         ), f"Only {len(self.fields)} fields are available and task expects at least {self.min_fields} to fill."
         # ... make sure we select a number of fields within the allowed range
@@ -478,15 +494,15 @@
             )
             + "."
         )
         info = {}
         return goal, info
 
     def cheat(self, page: Page, chat_messages: list[str]) -> None:
-        super().cheat(page, chat_messages)
+        super().cheat(page=page, chat_messages=chat_messages)
         self._wait_for_ready(page)
         iframe = page.frame_locator(f'iframe[name="{self.js_prefix}"]')
 
         from tenacity import retry, stop_after_delay, retry_if_exception_type
 
         # Retry on TypeError since in very rare occasions, element evaluates to null, which raises a TypeError
         @retry(
@@ -518,19 +534,19 @@
                 for i, s in enumerate(page.evaluate(f"{self.js_prefix}.g_tabs2Sections.tabIDs"))
             }
 
             # If the section is not in the tabs do nothing (it's probably the main section)
             if section_id not in tab_sections:
                 return
 
-            page.evaluate(
+            page.evaluate_handle(
                 f"""{self.js_prefix}.g_tabs2Sections.tabsTabs[
                                                     {tab_sections[section_id]}
-                                                ].element.click()"""
-            )
+                                                ].element"""
+            ).click(force=True)
 
         for field in self.task_fields:
             # Get the field's input control
             control = iframe.get_by_label(
                 page.evaluate(f"{self.form_js_selector}.getLabelOf('{field}')"),
                 exact=True,
             )
@@ -567,15 +583,25 @@
         Caveat: we check only if the expected fields have the right value. We don't Check
                 if there are extra fields that shouldn't be there. We could have issues
                 matching other fields since calculation rules may have changed through time.
                 Maybe we should assign a random value from our list of choices to the fields
                 that are not part of the task.
 
         """
-
+        # check that the page is at the right url
+        right_url = check_url_suffix_match(page, expected_url=self.start_url, task=self)
+        if not right_url:
+            return (
+                0,
+                False,
+                "",
+                {
+                    "message": f"The page is not in the right URL to validate task {self.__class__.__name__}."
+                },
+            )
         # Retrieve the created record's sys_id from the session storage
         sys_id = page.evaluate("localStorage").get(self.session_sys_id_field, None)
 
         # Check that a record has actually been created
         if sys_id is None:
             logging.info("No record has been created.")
             return (
@@ -661,52 +687,58 @@
 
 class CreateChangeRequestTask(GenericNewRecordTask):
     """
     Task to create a new change request in the system.
 
     """
 
-    def __init__(self, instance=None, fixed_config: dict = None) -> None:
+    def __init__(self, seed: int, instance=None, fixed_config: dict = None) -> None:
         super().__init__(
+            seed=seed,
             instance=instance,
             form_url="/now/nav/ui/classic/params/target/change_request.do",
+            table_label="change request",
             prohibited_fields=["chg_model", "state"],
             fixed_config=fixed_config,
             config_path=CREATE_CHANGE_REQUEST_CONFIG_PATH,
             expected_fields_path=EXPECTED_CHANGE_REQUEST_FORM_FIELDS_PATH,
         )
 
 
 class CreateIncidentTask(GenericNewRecordTask):
     """
     Task to create a new incident in the system.
 
     """
 
-    def __init__(self, instance=None, fixed_config: dict = None) -> None:
+    def __init__(self, seed: int, instance=None, fixed_config: dict = None) -> None:
         super().__init__(
+            seed=seed,
             instance=instance,
             form_url="/now/nav/ui/classic/params/target/incident.do",
+            table_label="incident",
             prohibited_fields=["state"],
             fixed_config=fixed_config,
             config_path=CREATE_INCIDENT_CONFIG_PATH,
             expected_fields_path=EXPECTED_INCIDENT_FORM_FIELDS_PATH,
         )
 
 
 class CreateHardwareAssetTask(GenericNewRecordTask):
     """
     Task to create a new user in the system.
 
     """
 
-    def __init__(self, instance=None, fixed_config: dict = None) -> None:
+    def __init__(self, seed: int, instance=None, fixed_config: dict = None) -> None:
         super().__init__(
+            seed=seed,
             instance=instance,
             form_url="/now/nav/ui/classic/params/target/alm_hardware.do",
+            table_label="hardware asset",
             prohibited_fields=["install_status"],
             extra_mandatory_fields=[
                 "model",
                 "model_category",
                 "serial_number",
                 "vendor",
             ],
@@ -719,18 +751,20 @@
 
 class CreateProblemTask(GenericNewRecordTask):
     """
     Task to create a new problem in the system.
 
     """
 
-    def __init__(self, instance=None, fixed_config: dict = None) -> None:
+    def __init__(self, seed: int, instance=None, fixed_config: dict = None) -> None:
         super().__init__(
+            seed=seed,
             instance=instance,
             form_url="/now/nav/ui/classic/params/target/problem.do",
+            table_label="problem",
             prohibited_fields=["state", "first_reported_by_task"],
             fixed_config=fixed_config,
             config_path=CREATE_PROBLEM_CONFIG_PATH,
             expected_fields_path=EXPECTED_PROBLEM_FORM_FIELDS_PATH,
             # TODO: The last field is disabled because somehow the value is not in the autocomplete
             #       list even though it's in the database. I'm not sure why. It doesn't matter much
             #       since in the future we'll pre-generate tasks and keep only the ones where the
@@ -740,18 +774,20 @@
 
 class CreateUserTask(GenericNewRecordTask):
     """
     Task to create a new user in the system.
 
     """
 
-    def __init__(self, instance=None, fixed_config: dict = None) -> None:
+    def __init__(self, seed: int, instance=None, fixed_config: dict = None) -> None:
         super().__init__(
+            seed=seed,
             instance=instance,
             form_url="/now/nav/ui/classic/params/target/sys_user.do",
+            table_label="user",
             extra_mandatory_fields=["user_name", "first_name", "last_name", "email"],
             unique_valued_fields={"user_name": lambda x: str(hash(x + self.unique_id))},
             fixed_config=fixed_config,
             config_path=CREATE_USER_CONFIG_PATH,
             expected_fields_path=EXPECTED_USER_FORM_FIELDS_PATH,
         )
```

### Comparing `browsergym_workarena-0.1.0rc7/src/browsergym/workarena/tasks/knowledge.py` & `browsergym_workarena-0.2.0/src/browsergym/workarena/tasks/knowledge.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,19 +3,21 @@
 
 """
 
 import json
 import logging
 
 from playwright.sync_api import Page
+from urllib import parse
 
 from .base import AbstractServiceNowTask
-from ..config import KB_FILEPATH, KB_CONFIG_PATH, SNOW_BROWSER_TIMEOUT
+from ..config import KB_NAME, KB_FILEPATH, KB_CONFIG_PATH, SNOW_BROWSER_TIMEOUT
 from ..install import check_knowledge_base
 from ..instance import SNowInstance
+from .utils.utils import check_url_suffix_match
 
 
 class KnowledgeBaseSearchTask(AbstractServiceNowTask):
     """
     Generic task to create a search for information in the knowledge base.
 
     Parameters:
@@ -26,38 +28,39 @@
     fixed_config: dict
         Configuration to use for the task. If provided, the task will use the provided configuration instead of
         selecting a random one. See browsergym/workarena/data_files/task_configs/knowledge_base_configs.json
         for an example of a configuration file.
 
     """
 
-    def __init__(self, instance=None, fixed_config: dict = None) -> None:
+    def __init__(self, seed: int, instance=None, fixed_config: dict = None) -> None:
         super().__init__(
+            seed=seed,
             instance=instance,
-            start_rel_url="/now/nav/ui/classic/params/target/%24knowledge.do",
+            start_rel_url="/now/nav/ui/classic/params/target/kb?id=kb_home",
         )
 
         # Load the knowledge base and check its integrity
         with open(KB_FILEPATH, "r") as f:
             self.kb_entries = json.load(f)
         _, requires_install, requires_delete = check_knowledge_base(
-            self.instance, kb_data=self.kb_entries
+            self.instance, kb_data=self.kb_entries, kb_name=KB_NAME
         )
         with open(KB_CONFIG_PATH, "r") as f:
             self.all_configs = json.load(f)
         if any([requires_install, requires_delete]):
             raise RuntimeError(
                 f"The knowledge base in instance {self.instance.snow_url} is missing or corrupted. "
                 "See README for setup instructions."
             )
         self.fixed_config = fixed_config
 
     def _wait_for_ready(self, page: Page) -> None:
         """
-        Waits for the main iframe to be fully loaded
+        Checks that the main iframe is fully loaded
 
         """
         # TODO: We don't use the flag-based method used in other tasks
         #       because gsft_main doesn't have the event we register
         #       on this page. Not sure why.
         logging.debug(f"Waiting for page to be fully loaded")
         page.wait_for_load_state("networkidle")
@@ -76,40 +79,44 @@
             page.wait_for_timeout(100)
             timeout -= 100
         else:
             raise TimeoutError(
                 f"Timed out waiting for iframe to be ready in {self.instance.snow_url}"
             )
 
-    def setup(self, page: Page, seed: int = None) -> tuple[str, dict]:
-        self.pre_setup(seed, page)
+    def setup_goal(self, page: Page) -> tuple[str, dict]:
+        super().setup_goal(page=page)
+
+        # Get task configuration
         config = self.fixed_config if self.fixed_config else self.random.choice(self.all_configs)
         self.item = config["item"]
         self.answer = config["value"]
         self.alternative_answers = config["alternative_answers"]
         self.question = config["question"]
 
-        # generate goal
+        # Generate goal
         goal = f'Answer the following question using the knowledge base: "{self.question}"'
         info = {}
 
         return goal, info
 
     def cheat(self, page: Page, chat_messages: list[str]) -> None:
-        super().cheat(page, chat_messages)
+        super().cheat(page=page, chat_messages=chat_messages)
         self._wait_for_ready(page)
 
         iframe = page.frame(name="gsft_main")
-        search = iframe.locator("input.form-control-search")
+        search = iframe.locator('input[aria-label="Search"][role="textbox"]')
         search.fill(f'"{self.item}"')
-        self.page.keyboard.press("Enter")
+
+        with page.expect_navigation():
+            self.page.keyboard.press("Enter")
 
         # Click on the article
-        with self.page.expect_navigation():
-            iframe.locator(".kb_link").first.click()
+        with page.expect_navigation():
+            iframe.locator("a.kb-title").first.click()
 
         # Color the query and answer (this is just for visualization, it changes nothing to the validation)
         paragraphs = iframe.locator("p")
         for i in range(paragraphs.count()):
             paragraph = paragraphs.nth(i)
             inner_html = paragraph.inner_html()
             if self.item in inner_html:
@@ -126,15 +133,24 @@
                 break
 
         # Add the "extracted" answer to the chat messages
         # TODO: this is a hack, the message will not be displayed in the html
         chat_messages.append({"role": "assistant", "message": str(self.answer)})
 
     def validate(self, page: Page, chat_messages: list[str]) -> tuple[float, bool, str, dict]:
-
+        right_url = check_url_suffix_match(page, expected_url="target/kb", task=self)
+        if not right_url:
+            return (
+                0,
+                False,
+                "",
+                {
+                    "message": f"The page is not in the right URL to validate task {self.__class__.__name__}."
+                },
+            )
         if chat_messages and chat_messages[-1]["role"] == "assistant":
             answer = chat_messages[-1]["message"]
         else:
             return (
                 0,
                 False,
                 "",
```

### Comparing `browsergym_workarena-0.1.0rc7/src/browsergym/workarena/tasks/list.py` & `browsergym_workarena-0.2.0/src/browsergym/workarena/tasks/list.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 """
 
 import itertools
 import json
 import logging
 import playwright.sync_api
 import re
-import urllib.parse
 
 from playwright.sync_api import Page
 from tenacity import retry, retry_if_exception_type, stop_after_delay
-from typing import Tuple
+from typing import List, Tuple
+from urllib import parse
 from warnings import warn
 
 from ..api.utils import table_api_call, table_column_info
 from ..config import (
     SNOW_BROWSER_TIMEOUT,
     FILTER_ASSET_LIST_CONFIG_PATH,
     FILTER_CHANGE_REQUEST_LIST_CONFIG_PATH,
@@ -36,51 +36,55 @@
     EXPECTED_HARDWARE_COLUMNS_PATH,
     EXPECTED_INCIDENT_COLUMNS_PATH,
     EXPECTED_SERVICE_CATALOG_COLUMNS_PATH,
     EXPECTED_USER_COLUMNS_PATH,
 )
 from .base import AbstractServiceNowTask
 from .utils.form import fill_text
+from .utils.utils import check_url_suffix_match
 
 
 LISTS = {
     "alm_asset": {
-        "url": "/now/nav/ui/classic/params/target/alm_asset_list.do%3Fsysparm_view%3Ditam_workspace%26sysparm_userpref.alm_asset_list.view%3Ditam_workspace%26sysparm_userpref.alm_asset.view%3Ditam_workspace%26sysparm_query%3D%26sysparm_fixed_query%3D",
+        "url": "/now/nav/ui/classic/params/target/alm_asset_list.do",
         "forbidden_fields": ["sys_class_name"],
     },
     "alm_hardware": {
-        "url": "/now/nav/ui/classic/params/target/alm_hardware_list.do%3Fsysparm_view%3Ditam_workspace%26sysparm_userpref.alm_hardware_list.view%3Ditam_workspace%26sysparm_userpref.alm_hardware.view%3Ditam_workspace%3D%26sysparm_query%3Dinstall_status%253D6%255Esubstatus%253Dpre_allocated",
+        "url": "/now/nav/ui/classic/params/target/alm_hardware_list.do",
         "forbidden_fields": [],
     },
     "change_request": {
-        "url": "/now/nav/ui/classic/params/target/change_request_list.do%3Fsysparm_view%3Dsow%26sysparm_userpref.change_request_list.view%3Dsow%26sysparm_userpref.change_request.view%3Dsow%26sysparm_query%3D%26sysparm_fixed_query%3D",
+        "url": "/now/nav/ui/classic/params/target/change_request_list.do",
         "forbidden_fields": [],
     },
     "incident": {
-        "url": "/now/nav/ui/classic/params/target/incident_list.do%3Fsysparm_query%3Dactive%253Dtrue%26sysparm_first_row%3D1%26sysparm_view%3DMajor%2520Incidents",
+        "url": "/now/nav/ui/classic/params/target/incident_list.do",
         "forbidden_fields": [],
     },
     "sys_user": {
-        "url": "/now/nav/ui/classic/params/target/sys_user_list.do%3Fsysparm_view%3D%26sysparm_userpref.sys_user_list.view%3D%26sysparm_userpref.sys_user.view%3D%26sysparm_query%3Dactive%253Dtrue%255Ecompany%253D81fd65ecac1d55eb42a426568fc87a63",
+        "url": "/now/nav/ui/classic/params/target/sys_user_list.do",
         "forbidden_fields": [
             "sys_class_name",
             "roles",
             "sys_tags",
             "user_password",
             "password_needs_reset",
         ],
     },
     "sc_cat_item": {
-        "url": "/now/nav/ui/classic/params/target/sc_cat_item_list.do%3Fsysparm_view%3D%26sysparm_userpref.sc_cat_item_list.view%3D%26sysparm_userpref.sc_cat_item.view%3D%26sysparm_query%3D%26sysparm_fixed_query%3D",
+        "url": "/now/nav/ui/classic/params/target/sc_cat_item_list.do",
         "forbidden_fields": ["roles", "sc_catalogs"],
     },
 }
 
 
 class ServiceNowListTask(AbstractServiceNowTask):
+    def get_init_scripts(self) -> List[str]:
+        return super().get_init_scripts() + ["registerGsftMainLoaded();"]
+
     def _get_visible_list(self, page: Page):
         self._wait_for_ready(page)
 
         iframe = page.frame("gsft_main")
         lst = iframe.locator("table.data_list_table")
         lst.wait_for()
 
@@ -160,31 +164,23 @@
         )
         logging.debug("Detected gsft_main ready")
 
         logging.debug("Waiting for Glide list API to be available")
         page.wait_for_function("window.gsft_main.GlideList2 !== undefined")
         logging.debug("Detected Glide list API ready")
 
-    def pre_setup(self, seed: int, page: Page):
-        super().pre_setup(seed, page)
-
-        self._add_init_scripts_to_context_and_reload(
-            page,
-            [
-                "registerGsftMainLoaded();",
-            ],
-        )
-
 
 class SortListTask(ServiceNowListTask):
     """
     Sort a list according to a column. Works with any list.
 
     Parameters:
     -----------
+    seed: int
+        Random seed
     instance: SNowInstance
         The instance to use.
     list_url: str
         The relative URL of the list to sort.
     forbidden_fields: list[str]
         A list of fields that should not be used for sorting.
         This is used to avoid sorting by fields that are disabled
@@ -197,54 +193,60 @@
         The path to the JSON file containing all configurations for the task. Provided by subclasses
     expected_fields_path:
         The path to the JSON file containing all expected fields for the task. Provided by subclasses
     """
 
     def __init__(
         self,
+        seed: int,
         instance=None,
         list_url="",
         forbidden_fields=[],
         fixed_config: dict = None,
         config_path: str = None,
         expected_fields_path: str = None,
     ) -> None:
-        super().__init__(instance=instance, start_rel_url=list_url)
+        super().__init__(seed=seed, instance=instance, start_rel_url=list_url)
         self.min_sort_len = 1
         self.max_sort_len = 3
         self.forbidden_fields = forbidden_fields
         self.fixed_config = fixed_config
         if config_path:
             with open(config_path, "r") as f:
                 self.all_configs = json.load(f)
         with open(expected_fields_path, "r") as f:
             self.expected_fields = set(json.load(f))
 
-    def setup(self, seed: int, page: Page) -> tuple[str, dict]:
-        self.pre_setup(seed, page)
-        self._wait_for_ready(page)
-        # Extract the list from the page
-        self.list_info = self._extract_list_info(page)
-        visible_columns = set(self.list_info["fields"].split(","))
-        config = self.fixed_config if self.fixed_config else self.random.choice(self.all_configs)
+    def setup_goal(self, page: Page) -> tuple[str, dict]:
+        super().setup_goal(page=page)
 
+        # Get the task configuration
+        config = self.fixed_config if self.fixed_config else self.random.choice(self.all_configs)
         self.sort_fields = config["sort_fields"]
         self.sort_dirs = config["sort_dirs"]
-        goal = config["goal"]
-        # Ensure that the fields that need to be sorted are visible
-        assert (
-            set(self.sort_fields) <= visible_columns and visible_columns == self.expected_fields
-        ), f"Fields {self.sort_fields} are not all visible in the list. Re-run workarena-install to correct this."
 
+        # Get the task goal
+        goal = config["goal"]
         info = {}
 
         return goal, info
 
+    def start(self, page: Page) -> None:
+        super().start(page)
+        self._wait_for_ready(page)
+
+        # Ensure that the fields that need to be sorted are visible (task feasibility check)
+        self.list_info = self._extract_list_info(page)
+        visible_columns = set(self.list_info["fields"].split(","))
+        assert (
+            set(self.sort_fields) <= visible_columns and visible_columns == self.expected_fields
+        ), f"Fields {self.sort_fields} are not all visible in the list. Re-run workarena-install to correct this."
+
     def _generate_all_configs(self, seed: int, page: Page, n_fields_to_sort: int):
-        self.pre_setup(seed, page)
+        self.setup(seed=seed, page=page)
         self._wait_for_ready(page)
         list_info = self._extract_list_info(page)
 
         # Get available fields
         available_fields = list(list_info["columns"].keys())
         # ... remove forbidden fields
         available_fields = [f for f in available_fields if f not in self.forbidden_fields]
@@ -273,16 +275,16 @@
                 ),
             }
             for sort_fields, sort_dirs in all_configs
         ]
 
         return all_configs
 
-    def _generate_random_config(self, seed: int, page: Page):
-        self.pre_setup(seed, page)
+    def _generate_random_config(self, page: Page):
+        self.setup(page=page)
         self._wait_for_ready(page)
         self.list_info = self._extract_list_info(page)
         # Get available fields
         available_fields = list(self.list_info["columns"].keys())
         # ... remove forbidden fields
         available_fields = [f for f in available_fields if f not in self.forbidden_fields]
 
@@ -321,15 +323,15 @@
             [f" - {field} ({dir})" for field, dir in zip(sort_fields_txt, sort_dirs_txt)]
         )
         info = {}
 
         return goal, info
 
     def cheat(self, page: Page, chat_messages: list[str]) -> None:
-        super().cheat(page, chat_messages)
+        super().cheat(page=page, chat_messages=chat_messages)
         self._wait_for_ready(page)
 
         iframe, _, _ = self._get_visible_list(page)
 
         iframe.locator(".list_filter_toggle").click()
 
         # Wait for the filter to be visible
@@ -383,16 +385,27 @@
         # click and wait for two navigations to happen (the iframe will navigate first, the page after)
         with page.expect_event("framenavigated", predicate=n_events_passed):
             filter.get_by_label("Run filter").click()
 
     def validate(
         self, page: playwright.sync_api.Page, chat_messages: list[str]
     ) -> Tuple[float, bool, str, dict]:
+        right_url = check_url_suffix_match(
+            page, expected_url=self.start_url[: self.start_url.find("%3F")], task=self
+        )
+        if not right_url:
+            return (
+                0,
+                False,
+                "",
+                {
+                    "message": f"The page is not in the right URL to validate task {self.__class__.__name__}."
+                },
+            )
         self._wait_for_ready(page)
-
         if len(self.sort_fields) == 1:
             # XXX: Treat this as a separate case because the user may have sorted by clicking
             #      on the column header. In that case, the URL will not contain the ORDERBY.
             # ... retrieve list
             list_info = self._extract_list_info(page)
             # ... get sorting info
             sort_by = self.page.evaluate(f'{list_info["js_selector"]}.getOrderBy()')
@@ -405,17 +418,17 @@
                     "Nice work, thank you!",
                     {"message": "Correct sorting."},
                 )
 
         else:
             # pre-process the URL
             page_url = page.evaluate("() => window.location.href")
-            page_url = urllib.parse.unquote(page_url)
-            page_query = urllib.parse.urlparse(page_url).query
-            page_qs = urllib.parse.parse_qs(page_query)
+            page_url = parse.unquote(page_url)
+            page_query = parse.urlparse(page_url).query
+            page_qs = parse.parse_qs(page_query)
 
             # make sure "sysparm_query" is present
             if "sysparm_query" not in page_qs:
                 return 0, False, "", {"message": "No sysparm_query found in URL."}
 
             # concatenate desired order_by conditions
             order_dir = {"asc": "", "desc": "DESC"}
@@ -460,63 +473,71 @@
         The path to the JSON file containing all configurations for the task. Provided by subclasses
     expected_fields_path:
         The path to the JSON file containing all expected fields for the task. Provided by subclasses
     """
 
     def __init__(
         self,
+        seed: int,
         instance=None,
         list_url="",
         fixed_config: dict = None,
         config_path: str = None,
         expected_fields_path: str = None,
     ) -> None:
         self.min_filter_len = 2
         self.max_filter_len = 5
-        super().__init__(instance=instance, start_rel_url=list_url)
+        super().__init__(seed=seed, instance=instance, start_rel_url=list_url)
         self.fixed_config = fixed_config
         if config_path:
             with open(config_path, "r") as f:
                 self.all_configs = json.load(f)
         with open(expected_fields_path, "r") as f:
             self.expected_fields = set(json.load(f))
 
-    def setup(self, seed: int, page: Page) -> tuple[str, dict]:
-        self.pre_setup(seed, page)
-        self._wait_for_ready(page)
-        config = self.fixed_config if self.fixed_config else self.random.choice(self.all_configs)
+    def setup_goal(self, page: Page) -> tuple[str, dict]:
+        super().setup_goal(page=page)
 
+        # Get the task configuration
+        config = self.fixed_config if self.fixed_config else self.random.choice(self.all_configs)
         self.filter_columns = config["filter_columns"]
         self.filter_values = config["filter_values"]
         self.filter_kind = config["filter_kind"]
         self.list_info = config["list_info"]
         self.filter_len = len(self.filter_columns)
-        visible_list_info = self._extract_list_info(page)
-        visible_columns = set(visible_list_info["fields"].split(","))
-        # Assert that required fields are visible
-        assert (
-            set(self.filter_columns) <= visible_columns and visible_columns == self.expected_fields
-        ), f"Fields {self.filter_columns} are not all visible in the list. Re-run workarena-install to correct this."
-        # generate goal
+
+        # Generate goal
         goal = (
             f"Create a filter for the list to extract all entries where "
             + f" {'and' if self.filter_kind == 'AND' else 'or'} ".join(
                 [
                     f'"{self.list_info["columns"][col]["label"]}" is "{val}"'
                     for col, val in zip(self.filter_columns, self.filter_values)
                 ]
             )
             + "."
         )
         info = {}
 
         return goal, info
 
-    def _generate_random_config(self, seed: int, page: Page):
-        self.pre_setup(seed, page)
+    def start(self, page: Page) -> None:
+        super().start(page)
+
+        self._wait_for_ready(page)
+
+        # Assert that required fields are visible (task feasibility check)
+        visible_list_info = self._extract_list_info(page)
+        visible_columns = set(visible_list_info["fields"].split(","))
+        assert (
+            set(self.filter_columns) <= visible_columns and visible_columns == self.expected_fields
+        ), f"Fields {self.filter_columns} are not all visible in the list. Re-run workarena-install to correct this."
+
+    def _generate_random_config(self, page: Page):
+        self.setup(page=page)
         self._wait_for_ready(page)
 
         # Extract the list from the page
         self.list_info = self._extract_list_info(page)
 
         # Choose the columns to filter on
         allowed_types = ["string", "choice", "reference", "translated_text", "boolean"]
@@ -590,15 +611,15 @@
             )
             + "."
         )
 
         return goal, {}
 
     def cheat(self, page: Page, chat_messages: list[str]) -> None:
-        super().cheat(page, chat_messages)
+        super().cheat(page=page, chat_messages=chat_messages)
         self._wait_for_ready(page)
 
         iframe, _, _ = self._get_visible_list(page)
 
         iframe.locator(".list_filter_toggle").click()
 
         # Wait for the filter to be visible
@@ -682,16 +703,25 @@
     ) -> Tuple[float, bool, str, dict]:
         """
         Validate the solution
 
         Note: current implementation is limited to AND and OR filters (single type per filter) with equality operators
 
         """
+        right_url = check_url_suffix_match(page, expected_url=self.start_url, task=self)
+        if not right_url:
+            return (
+                0,
+                False,
+                "",
+                {
+                    "message": f"The page is not in the right URL to validate task {self.__class__.__name__}."
+                },
+            )
         self._wait_for_ready(page)
-
         if self.filter_kind not in ["AND", "OR"]:
             raise NotImplementedError("Only AND and OR filters are supported.")
         # Excludes AND because that's the default and its sep is ^ which matches everywhere
         query_sep = {"OR": "^NQ"}
 
         # Retrieve list
         list_info = self._extract_list_info(page)
@@ -763,189 +793,213 @@
 
         return 1, True, "Nice work, thank you!", {"message": "Correct filter."}
 
 
 class FilterAssetListTask(FilterListTask):
     def __init__(
         self,
+        seed: int,
         instance=None,
         fixed_config: dict = None,
     ) -> None:
         super().__init__(
-            instance,
+            seed=seed,
+            instance=instance,
             list_url=LISTS["alm_asset"]["url"],
             fixed_config=fixed_config,
             config_path=FILTER_ASSET_LIST_CONFIG_PATH,
             expected_fields_path=EXPECTED_ASSET_LIST_COLUMNS_PATH,
         )
 
 
 class FilterChangeRequestListTask(FilterListTask):
     def __init__(
         self,
+        seed: int,
         instance=None,
         fixed_config: dict = None,
     ) -> None:
         super().__init__(
-            instance,
+            seed=seed,
+            instance=instance,
             list_url=LISTS["change_request"]["url"],
             fixed_config=fixed_config,
             config_path=FILTER_CHANGE_REQUEST_LIST_CONFIG_PATH,
             expected_fields_path=EXPECTED_CHANGE_REQUEST_COLUMNS_PATH,
         )
 
 
 class FilterHardwareListTask(FilterListTask):
     def __init__(
         self,
+        seed: int,
         instance=None,
         fixed_config: dict = None,
     ) -> None:
         super().__init__(
-            instance,
+            seed=seed,
+            instance=instance,
             list_url=LISTS["alm_hardware"]["url"],
             fixed_config=fixed_config,
             config_path=FILTER_HARDWARE_LIST_CONFIG_PATH,
             expected_fields_path=EXPECTED_HARDWARE_COLUMNS_PATH,
         )
 
 
 class FilterIncidentListTask(FilterListTask):
     def __init__(
         self,
+        seed: int,
         instance=None,
         fixed_config: dict = None,
     ) -> None:
         super().__init__(
-            instance,
+            seed=seed,
+            instance=instance,
             list_url=LISTS["incident"]["url"],
             fixed_config=fixed_config,
             config_path=FILTER_INCIDENT_LIST_CONFIG_PATH,
             expected_fields_path=EXPECTED_INCIDENT_COLUMNS_PATH,
         )
 
 
 class FilterServiceCatalogItemListTask(FilterListTask):
     def __init__(
         self,
+        seed: int,
         instance=None,
         fixed_config: dict = None,
     ) -> None:
         super().__init__(
-            instance,
+            seed=seed,
+            instance=instance,
             list_url=LISTS["sc_cat_item"]["url"],
             fixed_config=fixed_config,
             config_path=FILTER_SERVICE_CATALOG_ITEM_LIST_CONFIG_PATH,
             expected_fields_path=EXPECTED_SERVICE_CATALOG_COLUMNS_PATH,
         )
 
 
 class FilterUserListTask(FilterListTask):
     def __init__(
         self,
+        seed: int,
         instance=None,
         fixed_config: dict = None,
     ) -> None:
         super().__init__(
-            instance,
+            seed=seed,
+            instance=instance,
             list_url=LISTS["sys_user"]["url"],
             fixed_config=fixed_config,
             config_path=FILTER_USER_LIST_CONFIG_PATH,
             expected_fields_path=EXPECTED_USER_COLUMNS_PATH,
         )
 
 
 class SortAssetListTask(SortListTask):
     def __init__(
         self,
+        seed: int,
         instance=None,
         fixed_config: dict = None,
     ) -> None:
         super().__init__(
-            instance,
+            seed=seed,
+            instance=instance,
             list_url=LISTS["alm_asset"]["url"],
             forbidden_fields=LISTS["alm_asset"]["forbidden_fields"],
             fixed_config=fixed_config,
             config_path=SORT_ASSET_LIST_CONFIG_PATH,
             expected_fields_path=EXPECTED_ASSET_LIST_COLUMNS_PATH,
         )
 
 
 class SortChangeRequestListTask(SortListTask):
     def __init__(
         self,
+        seed: int,
         instance=None,
         fixed_config: dict = None,
     ) -> None:
         super().__init__(
-            instance,
+            seed=seed,
+            instance=instance,
             list_url=LISTS["change_request"]["url"],
             forbidden_fields=LISTS["change_request"]["forbidden_fields"],
             fixed_config=fixed_config,
             config_path=SORT_CHANGE_REQUEST_LIST_CONFIG_PATH,
             expected_fields_path=EXPECTED_CHANGE_REQUEST_COLUMNS_PATH,
         )
 
 
 class SortHardwareListTask(SortListTask):
     def __init__(
         self,
+        seed: int,
         instance=None,
         fixed_config: dict = None,
     ) -> None:
         super().__init__(
-            instance,
+            seed=seed,
+            instance=instance,
             list_url=LISTS["alm_hardware"]["url"],
             forbidden_fields=LISTS["alm_hardware"]["forbidden_fields"],
             fixed_config=fixed_config,
             config_path=SORT_HARDWARE_LIST_CONFIG_PATH,
             expected_fields_path=EXPECTED_HARDWARE_COLUMNS_PATH,
         )
 
 
 class SortIncidentListTask(SortListTask):
     def __init__(
         self,
+        seed: int,
         instance=None,
         fixed_config: dict = None,
     ) -> None:
         super().__init__(
-            instance,
+            seed=seed,
+            instance=instance,
             list_url=LISTS["incident"]["url"],
             forbidden_fields=LISTS["incident"]["forbidden_fields"],
             fixed_config=fixed_config,
             config_path=SORT_INCIDENT_LIST_CONFIG_PATH,
             expected_fields_path=EXPECTED_INCIDENT_COLUMNS_PATH,
         )
 
 
 class SortServiceCatalogItemListTask(SortListTask):
     def __init__(
         self,
+        seed: int,
         instance=None,
         fixed_config: dict = None,
     ) -> None:
         super().__init__(
-            instance,
+            seed=seed,
+            instance=instance,
             list_url=LISTS["sc_cat_item"]["url"],
             forbidden_fields=LISTS["sc_cat_item"]["forbidden_fields"],
             fixed_config=fixed_config,
             config_path=SORT_SERVICE_CATALOG_ITEM_LIST_CONFIG_PATH,
             expected_fields_path=EXPECTED_SERVICE_CATALOG_COLUMNS_PATH,
         )
 
 
 class SortUserListTask(SortListTask):
     def __init__(
         self,
+        seed: int,
         instance=None,
         fixed_config: dict = None,
     ) -> None:
         super().__init__(
-            instance,
+            seed=seed,
+            instance=instance,
             list_url=LISTS["sys_user"]["url"],
             forbidden_fields=LISTS["sys_user"]["forbidden_fields"],
             fixed_config=fixed_config,
             config_path=SORT_USER_LIST_CONFIG_PATH,
             expected_fields_path=EXPECTED_USER_COLUMNS_PATH,
         )
```

### Comparing `browsergym_workarena-0.1.0rc7/src/browsergym/workarena/tasks/navigation.py` & `browsergym_workarena-0.2.0/src/browsergym/workarena/tasks/navigation.py`

 * *Files 11% similar despite different names*

```diff
@@ -30,35 +30,37 @@
     fixed_config: dict
         Configuration to use for the task. If provided, the task will use the provided configuration instead of
         selecting a random one. See browsergym/workarena/data_files/task_configs/all_menu.json
         for an example of a configuration file.
 
     """
 
-    def __init__(self, instance: SNowInstance = None, fixed_config: dict = None) -> None:
-        super().__init__(instance=instance, start_rel_url="/now/nav/ui/home")
+    def __init__(self, seed: int, instance: SNowInstance = None, fixed_config: dict = None) -> None:
+        super().__init__(seed=seed, instance=instance, start_rel_url="/now/nav/ui/home")
         self.fixed_config = fixed_config
         with open(ALL_MENU_PATH, "r") as f:
             self.all_configs = json.load(f)
 
-    def setup(self, page: Page, seed: int = None) -> tuple[str, dict]:
-        self.pre_setup(seed, page)
+    def setup_goal(self, page: Page) -> tuple[str, dict]:
+        super().setup_goal(page=page)
+
+        # Get task configuration
         self.module = (
             self.fixed_config if self.fixed_config else self.random.choice(self.all_configs)
         )
         self.final_url = self.instance.snow_url + self.module["url"]
 
-        # generate goal
+        # Generate goal
         goal = f'Navigate to the "{self.module["module"]}" module of the "{self.module["application"]}" application.'
         info = {}
 
         return goal, info
 
     def cheat(self, page: Page, chat_messages: list[str]) -> None:
-        super().cheat(page, chat_messages)
+        super().cheat(page=page, chat_messages=chat_messages)
 
         menu_button = page.locator('div[aria-label="All"]')
         if menu_button.get_attribute("aria-expanded").lower() != "true":
             menu_button.click()
 
         # Select the menu's main div
         menu = page.locator('div[aria-label="All menu"]')
@@ -70,15 +72,15 @@
         # We could certainly do something more fancy, but it's not
         # worth spending time on right now.
         page.wait_for_timeout(1000)
 
         path = [m.strip() for m in self.module["module"].split(">")]
         # Navigate to the application's location in the menu and select its parent
         locator = menu.get_by_label(self.module["application"], exact=True).and_(
-            menu.get_by_role("menuitem")
+            menu.get_by_role("button")
         )
         locator = locator.locator("xpath=ancestor::div[contains(@class, 'snf-collapsible-list')]")
         for module in path[:-1]:
             # Expand menu if necessary (this is mostly for visual satisfaction, cheat func would still work without it)
             # XXX: Double selector here is due to discrepancies in the UI for various ServiceNow releases
             button = locator.locator(
                 f'button[aria-label="{module}"], div[role="button"][aria-label="{module}"]'
@@ -102,14 +104,15 @@
         with page.expect_navigation():
             menu_item.click()
         page.wait_for_timeout(2000)
 
     def validate(
         self, page: playwright.sync_api.Page, chat_messages: list[str]
     ) -> Tuple[float, bool, str, dict]:
+        page.wait_for_load_state("domcontentloaded")
 
         # Get the current URL and the final URL
         current_url = urlunparse(urlparse(unquote(page.evaluate("() => window.location.href"))))
         final_url = urlunparse(urlparse(unquote(self.final_url)))
 
         if final_url == current_url:
             return 1, True, "Nice work, thank you!", {"message": "Correct module reached."}
@@ -132,43 +135,42 @@
     fixed_config: dict
         Configuration to use for the task. If provided, the task will use the provided configuration instead of
         selecting a random one. See browsergym/workarena/data_files/task_configs/impersonation_users.json
         for an example of a configuration file.
 
     """
 
-    def __init__(self, instance=None, fixed_config: dict = None) -> None:
-        super().__init__(instance=instance, start_rel_url="/now/nav/ui/home")
+    def __init__(self, seed: int, instance=None, fixed_config: dict = None) -> None:
+        super().__init__(seed=seed, instance=instance, start_rel_url="/now/nav/ui/home")
         self.fixed_config = fixed_config
         with open(IMPERSONATION_CONFIG_PATH, "r") as f:
             self.all_configs = json.load(f)
 
-    def setup(self, page: Page, seed: int = None) -> tuple[str, dict]:
-        self.pre_setup(seed, page)
-        # Retrieve the list of users from the instance
-        # XXX: We exclude the admin to avoid problems with validation (task would always be valid by default)
+    def setup_goal(self, page: Page) -> tuple[str, dict]:
+        super().setup_goal(page=page)
+
+        # Get task configuration
         self.user_full_name = (
             self.fixed_config if self.fixed_config else self.random.choice(self.all_configs)
         )
         assert self.user_full_name in self.all_configs
 
-        # generate goal
+        # Generate goal
         goal = f"Impersonate the user {self.user_full_name}."
         info = {}
 
         return goal, info
 
     def cheat(self, page: Page, chat_messages: list[str]) -> None:
-        super().cheat(page, chat_messages)
+        super().cheat(page=page, chat_messages=chat_messages)
         impersonate_user(self.user_full_name, page)
 
     def validate(
         self, page: playwright.sync_api.Page, chat_messages: list[str]
     ) -> Tuple[float, bool, str, dict]:
-
         user_info = self.page.evaluate("window.NOW")["user"]
 
         # If the current user is not being impersonated, fail.
         if not user_info["isImpersonating"]:
             return 0, False, "", {"message": "Not currently impersonating a user."}
 
         # Fetch user's full name from database
```

### Comparing `browsergym_workarena-0.1.0rc7/src/browsergym/workarena/tasks/service_catalog.py` & `browsergym_workarena-0.2.0/src/browsergym/workarena/tasks/service_catalog.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,42 @@
 """
 Tasks that require interacting with the service catalog
 
 """
 
 import json
 import logging
-from time import sleep
-from urllib import parse
-
+from typing import List
 import numpy as np
 import playwright.sync_api
+
 from playwright.sync_api import Page
-from ..instance import SNowInstance
+from time import sleep
+from urllib import parse
+
+from .base import AbstractServiceNowTask
+from .utils.form import fill_text
+
+from ..api.requests import (
+    get_request_by_id,
+    db_delete_from_table,
+)
 from ..config import (
     ORDER_DEVELOPER_LAPTOP_TASK_CONFIG_PATH,
     ORDER_IPAD_MINI_TASK_CONFIG_PATH,
     ORDER_IPAD_PRO_TASK_CONFIG_PATH,
     ORDER_SALES_LAPTOP_TASK_CONFIG_PATH,
     ORDER_STANDARD_LAPTOP_TASK_CONFIG_PATH,
     ORDER_APPLE_WATCH_TASK_CONFIG_PATH,
     ORDER_APPLE_MAC_BOOK_PRO15_TASK_CONFIG_PATH,
     ORDER_DEVELOPMENT_LAPTOP_PC_TASK_CONFIG_PATH,
     ORDER_LOANER_LAPTOP_TASK_CONFIG_PATH,
 )
-from .utils.form import fill_text
-from ..api.requests import (
-    get_request_by_id,
-    db_delete_from_table,
-)
-from .base import AbstractServiceNowTask
+from ..instance import SNowInstance
+from .utils.utils import check_url_suffix_match
 
 ADDITIONAL_SOFTWARE = [
     "Slack",
     "Trello",
     "Salesforce",
     "QuickBooks",
     "Zoom",
@@ -138,32 +142,36 @@
 
 class OrderHardwareTask(AbstractServiceNowTask):
     """
     Order an item from the service catalog.
 
     Parameters:
     -----------
+    seed: int
+        Random seed
     instance: SNowInstance
         The instance to use.
     fixed_config: dict
         Configuration to use for the task. If provided, the task will use the provided configuration instead of
         selecting a random one. See browsergym/workarena/data_files/task_configs/order_ipda_pro_task.json
         for an example of a configuration file.
     config_path:
         The path to the JSON file containing all configurations for the task. Provided by subclasses
     """
 
     def __init__(
         self,
+        seed: int,
         instance: SNowInstance = None,
         fixed_request_item: str = None,
         fixed_config: dict = None,
         config_path: str = None,
     ):
         super().__init__(
+            seed=seed,
             instance=instance,
             start_rel_url="/now/nav/ui/classic/params/target/catalog_home.do%3Fsysparm_view%3Dcatalog_default",
             final_rel_url="/now/nav/ui/classic/params/target/com.glideapp.servicecatalog_checkout_view_v2.do",
         )
 
         if fixed_request_item is not None and fixed_config is not None:
             if fixed_request_item != fixed_config["item"]:
@@ -173,17 +181,17 @@
         self.fixed_request_item = fixed_request_item
 
         self.js_prefix = "gsft_main"
         self.js_api_forms = "g_form"
         with open(config_path, "r") as f:
             self.all_configs = json.load(f)
 
-    def _wait_for_ready(self, page: Page, wait_for_form_api=False) -> None:
+    def _wait_for_ready(self, page: Page, wait_for_form_api: bool = False) -> None:
         """
-        Waits for the main iframe to be fully loaded
+        Waits for the the main iframe to be loaded
 
         """
         logging.debug(f"Waiting for {self.js_prefix} to be fully loaded")
         page.wait_for_function(
             f"typeof window.{self.js_prefix} !== 'undefined' && window.{self.js_prefix}.WORKARENA_LOAD_COMPLETE"
         )
         logging.debug(f"Detected {self.js_prefix} ready")
@@ -193,68 +201,94 @@
             page.wait_for_function(f"window.{self.form_js_selector}")
             logging.debug("Detected Glide form API ready")
 
     @property
     def form_js_selector(self):
         return self.js_prefix + "." + self.js_api_forms
 
-    def setup(self, page: playwright.sync_api.Page, seed: int = None) -> None:
-        self.pre_setup(page=page, seed=seed)
-        # the cart is shared for all agents running in parallel. The "Order Now" button
-        # is not affected so we'll make sure the agent can only use that one
-        disable_add_to_cart = """
-        window.addEventListener('DOMContentLoaded', (event) => {
-            const button = document.querySelector('button[aria-label="Add to Cart"]');
-            if (button) {
-                button.disabled = true;
+    def get_init_scripts(self) -> List[str]:
+        return super().get_init_scripts() + [
+            "registerGsftMainLoaded()",
+            self._get_disable_add_to_cart_script(),
+            self._get_remove_top_items_panel_script(),
+        ]
+
+    def _get_disable_add_to_cart_script(self):
+        """
+        Disables the 'Add to Cart' button on the service catalog page
+        This is necessary so that agents running in parallel do not interfere with each other (cart is shared between sessions)
+
+        """
+        script = """
+            function disableAddToCartButton() {
+                waLog('Searching for top items panel...', 'disableAddToCartButton');
+                let button = document.querySelector('button[aria-label="Add to Cart"]');
+                if (button) {
+                    button.disabled = true;
+                    waLog('WorkArena: Disabled the "Add to Cart" button', 'disableAddToCartButton');
+                } else {
+                    waLog('WorkArena: Could not find the "Add to Cart" button', 'disableAddToCartButton');
+                }
             }
-        });
+
+            runInGsftMainOnlyAndProtectByURL(disableAddToCartButton, 'glideapp.servicecatalog_cat_item_view.do');
         """
-        self._add_init_scripts_to_context_and_reload(
-            page, ["registerGsftMainLoaded()", disable_add_to_cart]
-        )
-        self._wait_for_ready(page)
-        self._remove_top_items_panel(page)
+        return script
+
+    def _get_remove_top_items_panel_script(self):
+        """Get script that removes the 'top items' panel that sometimes on the landing page of service catalog
+        Disables the 'Top Requests' panel that sometimes appears on the landing page of the service catalog
+        Runs in a loop to keep checking for the host element and shadow root
+        URL is secured by running only on the catalog_home page; this is a heuristic to avoid running on other pages
+        and does not check that the URL is an exact match, as moving back and forth between pages can cause the URL
+        to change, but catalog_home will always be present.
+        """
+        script = """
+            function removeTopItemsPanel() {
+                waLog('Searching for top items panel...', 'removeTopItemsPanel');
+                let headings = Array.from(document.querySelectorAll('[role="heading"]'));
+                headings.forEach((heading) => {
+                    if (heading.textContent.includes("Top Requests")) {
+                        let parentDiv = heading.closest('div.drag_section');
+                        if (parentDiv) {
+                            parentDiv.remove();
+                            waLog('Removed parent div for heading: ' + heading.textContent, 'removeTopItemsPanel');
+                        }
+                    }
+                });
+            }
+
+            runInGsftMainOnlyAndProtectByURL(removeTopItemsPanel, `catalog_home`);
+            """
+        return script
+
+    def setup_goal(self, page: Page) -> tuple[str, dict]:
+        super().setup_goal(page=page)
+
+        # Get the task configuration
         assert self.all_configs is not None, "No configuration available for the task."
         config = self.fixed_config if self.fixed_config else self.random.choice(self.all_configs)
-        # use fixed config if any
         self.requested_item = config["item"]
         self.short_description = config["description"]
         self.quantity = config["quantity"]
         self.requested_configuration = config["configuration"]
 
-        self.request_sysid = None
-
-        # generate goal
+        # Generate goal
         goal = f'Go to the hardware store and order {self.quantity} "{self.requested_item}"'
         if len(self.requested_configuration) > 0:
             goal += f" with configuration {dict((k, v[1]) for k, v in self.requested_configuration.items())}"
         info = {}
 
-        return goal, info
+        # Used to keep track of the sysid of the request for validation
+        self.request_sysid = None
 
-    def _remove_top_items_panel(self, page: Page):
-        """Removes the 'top items' panel that sometimes on the landing page"""
-        frame = page.wait_for_selector("iframe#gsft_main").content_frame()
-
-        # Use evaluate to find and remove divs containing an element with role="heading" and the text "Top Requests"
-        frame.evaluate(
-            """() => {
-                const headings = Array.from(document.querySelectorAll('[role="heading"]'));
-                headings.forEach((heading) => {
-                    if (heading.textContent.includes("Top Requests")) {
-                        let parentDiv = heading.closest('div.drag_section');
-                        if (parentDiv) parentDiv.remove();
-                    }
-                });
-            }"""
-        )
+        return goal, info
 
     def cheat(self, page: Page, chat_messages: list[str]) -> None:
-        super().cheat(page, chat_messages)
+        super().cheat(page=page, chat_messages=chat_messages)
         self._wait_for_ready(page=page)
 
         iframe = page.frame(self.js_prefix)
 
         # Find hardware buttons
         element = iframe.wait_for_selector("a:text('Hardware')", strict=True)
         element.click()
@@ -319,46 +353,34 @@
                 raise ValueError(f"Unknown control type {control_type}")
 
         order_now_button = iframe.wait_for_selector("#oi_order_now_button", strict=True)
 
         with page.expect_navigation():
             order_now_button.click()
 
-    def _generate_random_config(self, seed: int, page: Page):
-        self.pre_setup(page=page, seed=seed)
-        # the cart is shared for all agents running in parallel. The "Order Now" button
-        # is not affected so we'll make sure the agent can only use that one
-        disable_add_to_cart = """
-        window.addEventListener('DOMContentLoaded', (event) => {
-            const button = document.querySelector('button[aria-label="Add to Cart"]');
-            if (button) {
-                button.disabled = true;
-            }
-        });
-        """
-        self._add_init_scripts_to_context_and_reload(
-            page, ["registerGsftMainLoaded()", disable_add_to_cart]
-        )
-        self._wait_for_ready(page)
+    def _generate_random_config(self, page: Page):
+        """Generate a random configuration for the task"""
+        self.setup(page=page, do_start=False)
         if self.fixed_request_item:
             self.requested_item = self.fixed_request_item
         else:
             # ... choose a random item to order
             self.requested_item = self.random.choice(list(META_CONFIGS.keys()))
 
         meta_config = META_CONFIGS[self.requested_item]
-        self.short_description = meta_config["desc"]
-        # ... choose a random quantity and configuration
-        self.quantity = self.random.randint(1, 11)
-        self.requested_configuration = {
-            ctrl_name: (ctrl_type, self.random.choice(values))
-            for ctrl_name, (ctrl_type, values) in meta_config["options"].items()
+        self.fixed_config = {
+            "item": self.requested_item,
+            "description": meta_config["desc"],
+            "quantity": self.random.randint(1, 11),
+            "configuration": {
+                ctrl_name: (ctrl_type, self.random.choice(values))
+                for ctrl_name, (ctrl_type, values) in meta_config["options"].items()
+            },
         }
-
-        self.request_sysid = None
+        self.setup(page=page, do_start=True)
 
     def _get_control_description(self, page, field):
         """
         Get the description of a control (e.g., the text of a radio button)
         """
         # Wait for everything to be ready
         self._wait_for_ready(page, wait_for_form_api=True)
@@ -390,15 +412,25 @@
 
         if hasattr(self, "request_sysid") and self.request_sysid is not None:
             db_delete_from_table(
                 instance=self.instance, sys_id=self.request_sysid, table="sc_request"
             )
 
     def validate(self, page: Page, chat_messages: list[str]) -> tuple[int, bool, str, dict]:
-        self._wait_for_ready(page)
+        right_url = check_url_suffix_match(page, expected_url=self.final_url, task=self)
+        if not right_url:
+            return (
+                0,
+                False,
+                "",
+                {
+                    "message": f"The page is not in the right URL to validate task {self.__class__.__name__}."
+                },
+            )
+
         # Retrieve the request sysid from the URL
         current_url = parse.urlparse(
             parse.unquote(self.page.evaluate("() => window.location.href"))
         )
         (self.request_sysid,) = parse.parse_qs(current_url.query).get("sysparm_sys_id", [None])
         if self.request_sysid is None:
             return (
```

### Comparing `browsergym_workarena-0.1.0rc7/src/browsergym/workarena/tasks/scripts/extract_all_menu_items.py` & `browsergym_workarena-0.2.0/src/browsergym/workarena/tasks/scripts/extract_all_menu_items.py`

 * *Files identical despite different names*

### Comparing `browsergym_workarena-0.1.0rc7/src/browsergym/workarena/tasks/scripts/generate_forms.py` & `browsergym_workarena-0.2.0/src/browsergym/workarena/tasks/scripts/generate_forms.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,20 +24,20 @@
         reraise=False,
         before_sleep=lambda _: logging.info("Retrying due to a TimeoutError..."),
     )
     def try_setup_and_cheat(task_class, seed, current_task_configs):
         """Try to setup and cheat a task, and return its configuration if it's new"""
         try:
             with sync_playwright() as p:
-                task = task_class()
+                task = task_class(seed=seed)
                 browser = p.chromium.launch()
                 context = browser.new_context()  # Set the timeout here
                 context.set_default_timeout(5000)
                 page = context.new_page()
-                task._generate_random_config(seed=seed, page=page)
+                task._generate_random_config(page=page)
                 config = {
                     "template_record": task.template_record,
                     "fields": {
                         f: task.fields[f]["label"] for f in task.fields
                     },  # the validate function only needs the field names
                     "task_fields": task.task_fields,
                 }
```

### Comparing `browsergym_workarena-0.1.0rc7/src/browsergym/workarena/tasks/scripts/knowledge.py` & `browsergym_workarena-0.2.0/src/browsergym/workarena/tasks/scripts/knowledge.py`

 * *Files identical despite different names*

### Comparing `browsergym_workarena-0.1.0rc7/src/browsergym/workarena/tasks/scripts/list.py` & `browsergym_workarena-0.2.0/src/browsergym/workarena/tasks/scripts/list.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,20 +43,20 @@
 
 
 def generate_task_configs(task_class, num_configs=1000, task_type="sort"):
     def try_setup_and_cheat(task_class, seed, current_task_configs):
         """Try to setup and cheat a task, and return its configuration if it's new"""
         try:
             with sync_playwright() as p:
-                task = task_class()
+                task = task_class(seed=seed)
                 browser = p.chromium.launch()
                 context = browser.new_context()  # Set the timeout here
                 context.set_default_timeout(5000)
                 page = context.new_page()
-                goal, _ = task._generate_random_config(seed=seed, page=page)
+                goal, _ = task._generate_random_config(page=page)
                 chat_messages = []
                 try:
                     task.cheat(page=page, chat_messages=chat_messages)
                     reward, done, message, info = task.validate(page, chat_messages)
                     task_successful = done is True and reward == 1.0
                 except Exception as e:  # Catch the exception
                     print(f"Error cheating on task {task_name} with seed {seed}: {str(e)}")
```

### Comparing `browsergym_workarena-0.1.0rc7/src/browsergym/workarena/tasks/scripts/navigation.py` & `browsergym_workarena-0.2.0/src/browsergym/workarena/tasks/scripts/navigation.py`

 * *Files identical despite different names*

### Comparing `browsergym_workarena-0.1.0rc7/src/browsergym/workarena/tasks/scripts/service_catalog.py` & `browsergym_workarena-0.2.0/src/browsergym/workarena/tasks/scripts/service_catalog.py`

 * *Files identical despite different names*

### Comparing `browsergym_workarena-0.1.0rc7/src/browsergym/workarena/tasks/scripts/validate.py` & `browsergym_workarena-0.2.0/src/browsergym/workarena/tasks/scripts/validate.py`

 * *Files 0% similar despite different names*

```diff
@@ -139,16 +139,16 @@
 
 
 def validate_on_page(task_class, task_config, page):
     """Validate a configuration on a given page"""
     cheat_passed = False
     task_done = False
     reward = 0.0
-    task = task_class(fixed_config=task_config)
-    task.setup(page=page, seed=1)
+    task = task_class(seed=1, fixed_config=task_config)
+    task.setup(page=page)
     chat_messages = []
     task.cheat(page=page, chat_messages=chat_messages)
     cheat_passed = True
     page.wait_for_timeout(2000)
     reward, task_done, _, _ = task.validate(page, chat_messages)
     task.teardown()
```

### Comparing `browsergym_workarena-0.1.0rc7/src/browsergym/workarena/tasks/utils/debug.py` & `browsergym_workarena-0.2.0/src/browsergym/workarena/tasks/utils/debug.py`

 * *Files identical despite different names*

### Comparing `browsergym_workarena-0.1.0rc7/src/browsergym/workarena/tasks/utils/form.py` & `browsergym_workarena-0.2.0/src/browsergym/workarena/tasks/utils/form.py`

 * *Files 7% similar despite different names*

```diff
@@ -28,27 +28,29 @@
     input_field.click(force=True)
 
     # If the field uses autocomplete, we need to wait for Ajax to finish (and expand the menu)
     if input_field.get_attribute("aria-autocomplete") == "list":
         # Fill in the value using a procedure that triggers the autocomplete
         input_field.fill(value[:-1])
         page.keyboard.press(value[-1])
+        time.sleep(0.5)
 
-        # Wait until the attribute of the locator changes to the desired value
+        # Wait for the autocomplete menu to open and be ready
         max_wait_time = SNOW_BROWSER_TIMEOUT  # maximum time to wait in seconds
         start_time = time.time()
         while True:
-            if input_field.get_attribute("aria-expanded") == "true":
+            if input_field.get_attribute("aria-expanded") == "true" and not input_field.evaluate(
+                "e => e.ac.isResolving()"
+            ):
                 break
             if time.time() - start_time > (max_wait_time / 1000):
                 raise TimeoutError("Timeout waiting for autocompletion menu to open")
             time.sleep(0.5)  # wait for a short period before checking again
 
         # Select the desired value
-        time.sleep(0.5)  # wait for the list to be populated
         options = iframe.locator("[id^='ac_option_']")
         for i in range(options.count()):
             opt = options.nth(i)
 
             # Extract the value from the option element
             if opt.locator(".ac_cell").count() > 0:
                 # ... element is multi part (use only the main info)
```

### Comparing `browsergym_workarena-0.1.0rc7/tests/test_random_config_generation.py` & `browsergym_workarena-0.2.0/tests/test_random_config_generation.py`

 * *Files 14% similar despite different names*

```diff
@@ -44,54 +44,55 @@
     OrderAppleWatchTask,
     OrderAppleMacBookPro15Task,
     OrderDevelopmentLaptopPCTask,
     OrderLoanerLaptopTask,
 )
 
 RANDOMLY_CONFIGURALBE_TASKS = [
-    CreateChangeRequestTask,
-    CreateHardwareAssetTask,
-    CreateIncidentTask,
-    CreateProblemTask,
-    CreateUserTask,
-    FilterAssetListTask,
-    FilterChangeRequestListTask,
-    FilterHardwareListTask,
-    FilterIncidentListTask,
-    FilterServiceCatalogItemListTask,
-    FilterUserListTask,
-    SortAssetListTask,
-    SortChangeRequestListTask,
-    SortHardwareListTask,
-    SortIncidentListTask,
-    SortServiceCatalogItemListTask,
-    SortUserListTask,
+    # CreateChangeRequestTask,
+    # CreateHardwareAssetTask,
+    # CreateIncidentTask,
+    # CreateProblemTask,
+    # CreateUserTask,
+    # FilterAssetListTask,
+    # FilterChangeRequestListTask,
+    # FilterHardwareListTask,
+    # FilterIncidentListTask,
+    # FilterServiceCatalogItemListTask,
+    # FilterUserListTask,
+    # SortAssetListTask,
+    # SortChangeRequestListTask,
+    # SortHardwareListTask,
+    # SortIncidentListTask,
+    # SortServiceCatalogItemListTask,
+    # SortUserListTask,
     OrderDeveloperLaptopTask,
     OrderIpadMiniTask,
     OrderIpadProTask,
     OrderSalesLaptopTask,
     OrderStandardLaptopTask,
     OrderAppleWatchTask,
     OrderAppleMacBookPro15Task,
     OrderDevelopmentLaptopPCTask,
     OrderLoanerLaptopTask,
 ]
 
 
-@retry(
-    stop=stop_after_attempt(5),
-    retry=retry_if_exception_type(TimeoutError),
-    reraise=True,
-    before_sleep=lambda _: logging.info("Retrying due to a TimeoutError..."),
-)
+# @retry(
+#     stop=stop_after_attempt(5),
+#     retry=retry_if_exception_type(TimeoutError),
+#     reraise=True,
+#     before_sleep=lambda _: logging.info("Retrying due to a TimeoutError..."),
+# )
 @pytest.mark.parametrize("task_entrypoint", RANDOMLY_CONFIGURALBE_TASKS)
 @pytest.mark.parametrize("random_seed", range(1))
+@pytest.mark.slow
 def test_cheat_from_random_config(task_entrypoint, random_seed: int, page: Page):
-    task = task_entrypoint()
-    task._generate_random_config(seed=random_seed, page=page)
+    task = task_entrypoint(seed=random_seed)
+    task._generate_random_config(page=page)
     chat_messages = []
     reward, done, message, info = task.validate(page, chat_messages)
     assert done is False and reward == 0.0
     task.cheat(page=page, chat_messages=chat_messages)
     reward, done, message, info = task.validate(page, chat_messages)
     assert done is True and reward == 1.0
     task.teardown()
```

### Comparing `browsergym_workarena-0.1.0rc7/tests/test_snow_instance.py` & `browsergym_workarena-0.2.0/tests/test_snow_instance.py`

 * *Files identical despite different names*

### Comparing `browsergym_workarena-0.1.0rc7/tests/test_task_from_config.py` & `browsergym_workarena-0.2.0/tests/test_task_from_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,16 +88,16 @@
     stop=stop_after_attempt(5),
     retry=retry_if_exception_type(TimeoutError),
     reraise=True,
     before_sleep=lambda _: logging.info("Retrying due to a TimeoutError..."),
 )
 def generic_task_cheat_test(task_class, config_path, page: Page, expected_goal: str = None):
     task_config = json.load(open(config_path, "r"))[0]
-    task = task_class(fixed_config=task_config)
-    goal, _ = task.setup(page=page, seed=1)
+    task = task_class(seed=1, fixed_config=task_config)
+    goal, _ = task.setup(page=page)
     if expected_goal:
         assert goal == expected_goal
     chat_messages = []
     reward, done, message, info = task.validate(page, chat_messages)
     assert (
         isinstance(reward, (int, float))
         and type(done) == bool
```

### Comparing `browsergym_workarena-0.1.0rc7/tests/test_task_general.py` & `browsergym_workarena-0.2.0/tests/test_task_general.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,16 +23,16 @@
     reraise=True,
     before_sleep=lambda _: logging.info("Retrying due to a TimeoutError..."),
 )
 @pytest.mark.parametrize("task_entrypoint", ALL_WORKARENA_TASKS)
 @pytest.mark.parametrize("random_seed", range(1))
 @pytest.mark.slow
 def test_cheat(task_entrypoint, random_seed: int, page: Page):
-    task = task_entrypoint()
-    goal, info = task.setup(seed=random_seed, page=page)
+    task = task_entrypoint(seed=random_seed)
+    goal, info = task.setup(page=page)
     chat_messages = []
     reward, done, message, info = task.validate(page, chat_messages)
     assert done is False and reward == 0.0
     assert (
         isinstance(reward, (int, float))
         and type(done) == bool
         and type(message) == str
```

### Comparing `browsergym_workarena-0.1.0rc7/tests/test_task_setup.py` & `browsergym_workarena-0.2.0/tests/test_task_setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -10,43 +10,51 @@
 
 # bugfix: use same playwright instance in browsergym and pytest
 from utils import setup_playwright
 from playwright.sync_api import Page, TimeoutError
 from tenacity import retry, stop_after_attempt, retry_if_exception_type
 from browsergym.workarena.config import ORDER_APPLE_WATCH_TASK_CONFIG_PATH
 
+from browsergym.workarena.tasks.navigation import AllMenuTask
 from browsergym.workarena.tasks.service_catalog import OrderAppleWatchTask
 
 
 @retry(
     stop=stop_after_attempt(5),
     retry=retry_if_exception_type(TimeoutError),
     reraise=True,
     before_sleep=lambda _: logging.info("Retrying due to a TimeoutError..."),
 )
 @pytest.mark.slow
 def test_add_to_cart_disabled(page: Page):
     task_config = json.load(open(ORDER_APPLE_WATCH_TASK_CONFIG_PATH, "r"))[0]
-    task = OrderAppleWatchTask(fixed_config=task_config)
+    task = OrderAppleWatchTask(seed=1, fixed_config=task_config)
     # setup the task and try clicking on the "Add to cart button"
     task.setup(page=page)
     order_apple_watch_page = (
         task.instance.snow_url
         + "/now/nav/ui/classic/params/target/com.glideapp.servicecatalog_cat_item_view.do%3Fv%3D1%26sysparm_id%3D774906834fbb4200086eeed18110c737%26sysparm_link_parent%3Dd258b953c611227a0146101fb1be7c31%26sysparm_catalog%3De0d08b13c3330100c8b837659bba8fb4%26sysparm_catalog_view%3Dcatalog_default%26sysparm_view%3Dcatalog_default"
     )
     task.page.goto(order_apple_watch_page)
-    page.wait_for_timeout(1000)
+    task.page.wait_for_timeout(1000)
     iframe_element = task.page.wait_for_selector("#gsft_main")
     iframe = iframe_element.content_frame()
-
+    task.teardown()
     # verify that Add to cart is disabled and order now is enabled
     assert iframe.locator('button[aria-label="Add to Cart"]').is_disabled()
     assert iframe.locator('button[aria-label="Order Now"]').is_enabled()
 
 
+@retry(
+    stop=stop_after_attempt(5),
+    retry=retry_if_exception_type(TimeoutError),
+    reraise=True,
+    before_sleep=lambda _: logging.info("Retrying due to a TimeoutError..."),
+)
+@pytest.mark.slow
 def test_top_items_panel_removed(page: Page):
     def check_top_items_panel(page: Page) -> bool:
         """Checks if the 'top items' panel exists on the landing page"""
         frame = page.wait_for_selector("iframe#gsft_main").content_frame()
 
         # Use evaluate to find divs containing an element with role="heading" and the text "Top Requests"
         panel_exists = frame.evaluate(
@@ -60,20 +68,27 @@
                 });
                 return panelExists;
             }"""
         )
 
         return panel_exists
 
-    task_config = json.load(open(ORDER_APPLE_WATCH_TASK_CONFIG_PATH, "r"))[0]
-    task = OrderAppleWatchTask(fixed_config=task_config)
+    # # Create a new task outside the service catalog and check if the Top Items panel exists
+    # TODO: Uncomment this code and fix the test; it is currently failing, but the functionality is optional
+    menu_task = AllMenuTask(seed=1)
+    menu_task.setup(page=page)
+    menu_task.page.goto(
+        menu_task.instance.snow_url
+        + r"/now/nav/ui/classic/params/target/catalog_home.do%3Fsysparm_view%3Dcatalog_default"
+    )
+    menu_task.page.wait_for_timeout(2000)
+    panel_exists = check_top_items_panel(page=menu_task.page)
+    menu_task.teardown()
+    assert panel_exists is True
 
+    service_catalog_task = OrderAppleWatchTask(seed=1)
     # Setup the task and check if the Top Items panel exists
-    task.setup(page=page)
-    panel_exists = check_top_items_panel(page=page)
-    page.wait_for_timeout(2000)
+    service_catalog_task.setup(page=page)
+    service_catalog_task.page.wait_for_timeout(2000)
+    panel_exists = check_top_items_panel(page=service_catalog_task.page)
+    service_catalog_task.teardown()
     assert panel_exists is False
-    # Reload the page and check if the Top Items panel exists
-    page.goto(task.start_url)
-    page.wait_for_timeout(2000)
-    panel_exists = check_top_items_panel(page=page)
-    assert panel_exists is True
```

### Comparing `browsergym_workarena-0.1.0rc7/tests/test_utils.py` & `browsergym_workarena-0.2.0/tests/test_utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,29 +2,31 @@
 
 # bugfix: use same playwright instance in browsergym and pytest
 from utils import setup_playwright
 
 from playwright.sync_api import Page
 
 from browsergym.workarena.instance import SNowInstance
-from browsergym.workarena.utils import ui_login
+from browsergym.workarena.utils import ui_login, url_login
 
 
-def test_ui_login_correct_credentials(page: Page):
+@pytest.mark.parametrize("login_func", [ui_login, url_login])
+def test_login_correct_credentials(login_func, page: Page):
     """
-    Test logging into the instance via the UI with the correct credentials
+    Test logging into the instance with the correct credentials
 
     """
     # Log in with correct credentials
     instance = SNowInstance()
-    ui_login(instance=instance, page=page)
+    login_func(instance=instance, page=page)
 
 
-def test_ui_login_wrong_credentials(page: Page):
+@pytest.mark.parametrize("login_func", [ui_login, url_login])
+def test_login_wrong_credentials(login_func, page: Page):
     """
-    Test logging into the instance via the UI with the wrong credentials
+    Test logging into the instance with the wrong credentials
 
     """
     # Log in with wrong credentials
     instance = SNowInstance(snow_credentials=("wrong", "wrong"))
     with pytest.raises(RuntimeError):
-        ui_login(instance=instance, page=page)
+        login_func(instance=instance, page=page)
```

### Comparing `browsergym_workarena-0.1.0rc7/tests/test_validate.py` & `browsergym_workarena-0.2.0/tests/test_validate.py`

 * *Files identical despite different names*

### Comparing `browsergym_workarena-0.1.0rc7/tests/utils.py` & `browsergym_workarena-0.2.0/tests/utils.py`

 * *Files identical despite different names*

### Comparing `browsergym_workarena-0.1.0rc7/LICENSE` & `browsergym_workarena-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `browsergym_workarena-0.1.0rc7/README.md` & `browsergym_workarena-0.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -6,18 +6,20 @@
 By harnessing the ubiquitous [ServiceNow](https://www.servicenow.com/what-is-servicenow.html) platform, this benchmark will be instrumental in assessing the widespread state of such automations in modern knowledge work environments.
 
 WorkArena is included in [BrowserGym](https://github.com/ServiceNow/BrowserGym), a conversational gym environment for the evaluation of web agents.
 
 
 https://github.com/ServiceNow/WorkArena/assets/2374980/68640f09-7d6f-4eb1-b556-c294a6afef70
 
+## ⚠️ Pre-Release warning ⚠️
+Please note that the WorkArena benchmark is still undergoing minor bug fixes and updates, which may cause discrepancies with results reported in our latest arXiv preprint. We plan to release soon a stable version of WorkArena v0.1.0 with enhanced stability, and a final version v1.0.0 with a new suite of tasks.
 
 ## Benchmark Contents
 
-At the moment, WorkArena includes `23,150` task instances drawn from `29` tasks that cover the main components of the ServiceNow user interface. The following videos show an agent built on `GPT-4-vision` interacting with every such component. As emphasized by our results, this benchmark is not solved and thus, the performance of the agent is not always on point.
+At the moment, WorkArena includes `18,050` task instances drawn from `29` tasks that cover the main components of the ServiceNow user interface. The following videos show an agent built on `GPT-4-vision` interacting with every such component. As emphasized by our results, this benchmark is not solved and thus, the performance of the agent is not always on point.
 
 ### Knowledge Bases
 
 **Goal:** The agent must search for specific information in the company knowledge base.
 
 _The agent interacts with the user via BrowserGym's conversational interface._
```

### Comparing `browsergym_workarena-0.1.0rc7/pyproject.toml` & `browsergym_workarena-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `browsergym_workarena-0.1.0rc7/PKG-INFO` & `browsergym_workarena-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,45 +1,49 @@
 Metadata-Version: 2.3
 Name: browsergym-workarena
-Version: 0.1.0rc7
+Version: 0.2.0
 Summary: WorkArena benchmark for BrowserGym
 Project-URL: homepage, https://github.com/ServiceNow/WorkArena
 Author: Léo Boisvert, Alex Drouin, Maxime Gasse, Alex Lacoste, Manuel Del Verme
 License: Apache-2.0
 License-File: LICENSE
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >3.7
-Requires-Dist: browsergym-core==0.1.0rc7
+Requires-Dist: browsergym-core==0.2.0
 Requires-Dist: english-words>=2.0.1
+Requires-Dist: faker>=24.11.0
 Requires-Dist: numpy>=1.14
 Requires-Dist: requests>=2.31
 Requires-Dist: tenacity>=8.2.3
+Requires-Dist: tqdm>=4.66.2
 Description-Content-Type: text/markdown
 
 # WorkArena: How Capable are Web Agents at Solving Common Knowledge Work Tasks?
 
 [[Paper]](https://arxiv.org/abs/2403.07718) ♦ [[Benchmark Contents]](#benchmark-contents) ♦ [[Getting Started]](#getting-started) ♦ [[Live Demo]](#live-demo) ♦ [[BrowserGym]](https://github.com/ServiceNow/BrowserGym) ♦ [[Citing This Work]](#citing-this-work)
 
 `WorkArena` is a suite of browser-based tasks tailored to gauge web agents' effectiveness in supporting routine tasks for knowledge workers. 
 By harnessing the ubiquitous [ServiceNow](https://www.servicenow.com/what-is-servicenow.html) platform, this benchmark will be instrumental in assessing the widespread state of such automations in modern knowledge work environments.
 
 WorkArena is included in [BrowserGym](https://github.com/ServiceNow/BrowserGym), a conversational gym environment for the evaluation of web agents.
 
 
 https://github.com/ServiceNow/WorkArena/assets/2374980/68640f09-7d6f-4eb1-b556-c294a6afef70
 
+## ⚠️ Pre-Release warning ⚠️
+Please note that the WorkArena benchmark is still undergoing minor bug fixes and updates, which may cause discrepancies with results reported in our latest arXiv preprint. We plan to release soon a stable version of WorkArena v0.1.0 with enhanced stability, and a final version v1.0.0 with a new suite of tasks.
 
 ## Benchmark Contents
 
-At the moment, WorkArena includes `23,150` task instances drawn from `29` tasks that cover the main components of the ServiceNow user interface. The following videos show an agent built on `GPT-4-vision` interacting with every such component. As emphasized by our results, this benchmark is not solved and thus, the performance of the agent is not always on point.
+At the moment, WorkArena includes `18,050` task instances drawn from `29` tasks that cover the main components of the ServiceNow user interface. The following videos show an agent built on `GPT-4-vision` interacting with every such component. As emphasized by our results, this benchmark is not solved and thus, the performance of the agent is not always on point.
 
 ### Knowledge Bases
 
 **Goal:** The agent must search for specific information in the company knowledge base.
 
 _The agent interacts with the user via BrowserGym's conversational interface._
```

