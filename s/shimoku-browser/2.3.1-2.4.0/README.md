# Comparing `tmp/shimoku-browser-2.3.1.tar.gz` & `tmp/shimoku_browser-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shimoku-browser-2.3.1.tar", last modified: Tue Apr  9 08:02:21 2024, max compression
+gzip compressed data, was "shimoku_browser-2.4.0.tar", last modified: Fri May 10 08:27:52 2024, max compression
```

## Comparing `shimoku-browser-2.3.1.tar` & `shimoku_browser-2.4.0.tar`

### file list

```diff
@@ -1,309 +1,309 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:02:21.581793 shimoku-browser-2.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:02:21.541793 shimoku-browser-2.3.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:02:21.541793 shimoku-browser-2.3.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      833 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:02:21.541793 shimoku-browser-2.3.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/.github/workflows/publish-testpypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7570 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     5220 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-09 08:02:21.581793 shimoku-browser-2.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8321 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/SECURITY.md
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:02:21.541793 shimoku-browser-2.3.1/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     5818 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/scripts/user_classes_header_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-04-09 08:02:21.581793 shimoku-browser-2.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/setup_browser.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:02:21.537793 shimoku-browser-2.3.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:02:21.541793 shimoku-browser-2.3.1/src/shimoku/
--rw-r--r--   0 runner    (1001) docker     (127)    17476 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/src/shimoku/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:02:21.541793 shimoku-browser-2.3.1/src/shimoku/actions_execution/
--rw-r--r--   0 runner    (1001) docker     (127)    15089 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/src/shimoku/actions_execution/execute_action.py
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/src/shimoku/actions_execution/front_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:02:21.541793 shimoku-browser-2.3.1/src/shimoku/ai/
--rw-r--r--   0 runner    (1001) docker     (127)    33016 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/src/shimoku/ai/ai_layer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:02:21.541793 shimoku-browser-2.3.1/src/shimoku/ai/generated_headers/
--rw-r--r--   0 runner    (1001) docker     (127)     4761 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/src/shimoku/ai/generated_headers/AILayerHeader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:02:21.541793 shimoku-browser-2.3.1/src/shimoku/api/
--rw-r--r--   0 runner    (1001) docker     (127)    30469 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/src/shimoku/api/base_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    19697 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/src/shimoku/api/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:02:21.545793 shimoku-browser-2.3.1/src/shimoku/api/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     3718 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/src/shimoku/api/resources/action.py
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/src/shimoku/api/resources/action_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     9183 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/src/shimoku/api/resources/activity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/src/shimoku/api/resources/activity_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    17613 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/src/shimoku/api/resources/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     8524 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/src/shimoku/api/resources/business.py
--rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/src/shimoku/api/resources/business_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     4993 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/src/shimoku/api/resources/dashboard.py
--rw-r--r--   0 runner    (1001) docker     (127)    11235 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/src/shimoku/api/resources/data_set.py
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/src/shimoku/api/resources/event.py
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/src/shimoku/api/resources/file.py
--rw-r--r--   0 runner    (1001) docker     (127)    10082 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/src/shimoku/api/resources/report.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:02:21.545793 shimoku-browser-2.3.1/src/shimoku/api/resources/reports/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:02:21.545793 shimoku-browser-2.3.1/src/shimoku/api/resources/reports/charts/
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/src/shimoku/api/resources/reports/charts/annotated_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/src/shimoku/api/resources/reports/charts/button.py
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/src/shimoku/api/resources/reports/charts/echart.py
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/src/shimoku/api/resources/reports/charts/html.py
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/src/shimoku/api/resources/reports/charts/iframe.py
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/src/shimoku/api/resources/reports/charts/indicator.py
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/src/shimoku/api/resources/reports/charts/input_form.py
--rw-r--r--   0 runner    (1001) docker     (127)     2271 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/src/shimoku/api/resources/reports/charts/table.py
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/src/shimoku/api/resources/reports/filter_data_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/src/shimoku/api/resources/reports/modal.py
--rw-r--r--   0 runner    (1001) docker     (127)     3779 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/src/shimoku/api/resources/reports/tabs_group.py
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/src/shimoku/api/resources/reports/unsupported.py
--rw-r--r--   0 runner    (1001) docker     (127)     6665 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/src/shimoku/api/resources/role.py
--rw-r--r--   0 runner    (1001) docker     (127)     6653 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/src/shimoku/api/resources/universe.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:02:21.549793 shimoku-browser-2.3.1/src/shimoku/api/user_access_classes/
--rw-r--r--   0 runner    (1001) docker     (127)     5868 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/src/shimoku/api/user_access_classes/actions_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)    11082 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/src/shimoku/api/user_access_classes/activities_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/src/shimoku/api/user_access_classes/activity_templates_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)    10255 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/src/shimoku/api/user_access_classes/apps_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)    14638 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/src/shimoku/api/user_access_classes/businesses_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     9947 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/src/shimoku/api/user_access_classes/dashboards_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3664 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/src/shimoku/api/user_access_classes/data_sets_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     9899 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/src/shimoku/api/user_access_classes/files_layer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:02:21.549793 shimoku-browser-2.3.1/src/shimoku/api/user_access_classes/generated_headers/
--rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/src/shimoku/api/user_access_classes/generated_headers/ActionsLayerHeader.py
--rw-r--r--   0 runner    (1001) docker     (127)     6666 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/src/shimoku/api/user_access_classes/generated_headers/ActivitiesLayerHeader.py
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/src/shimoku/api/user_access_classes/generated_headers/ActivityTemplatesLayerHeader.py
--rw-r--r--   0 runner    (1001) docker     (127)     6979 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/src/shimoku/api/user_access_classes/generated_headers/BoardsLayerHeader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/src/shimoku/api/user_access_classes/generated_headers/ComponentsLayerHeader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/src/shimoku/api/user_access_classes/generated_headers/DataSetsLayerHeader.py
--rw-r--r--   0 runner    (1001) docker     (127)     4909 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/src/shimoku/api/user_access_classes/generated_headers/FilesLayerHeader.py
--rw-r--r--   0 runner    (1001) docker     (127)     6887 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/src/shimoku/api/user_access_classes/generated_headers/MenuPathsLayerHeader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/src/shimoku/api/user_access_classes/generated_headers/UniversesLayerHeader.py
--rw-r--r--   0 runner    (1001) docker     (127)     7870 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/src/shimoku/api/user_access_classes/generated_headers/WorkspacesLayerHeader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/src/shimoku/api/user_access_classes/reports_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4240 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/src/shimoku/api/user_access_classes/universes_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)    20693 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/src/shimoku/api/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7129 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/src/shimoku/async_execution_pool.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:02:21.553793 shimoku-browser-2.3.1/src/shimoku/cli/
--rw-r--r--   0 runner    (1001) docker     (127)    20258 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/src/shimoku/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:02:21.553793 shimoku-browser-2.3.1/src/shimoku/cli/cloud/
--rw-r--r--   0 runner    (1001) docker     (127)    14378 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/src/shimoku/cli/cloud/cascade_get_resources.py
--rw-r--r--   0 runner    (1001) docker     (127)    11288 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/src/shimoku/cli/cloud/create.py
--rw-r--r--   0 runner    (1001) docker     (127)    19454 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/src/shimoku/cli/cloud/delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     5696 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/src/shimoku/cli/cloud/execute.py
--rw-r--r--   0 runner    (1001) docker     (127)     9860 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/src/shimoku/cli/cloud/get.py
--rw-r--r--   0 runner    (1001) docker     (127)    32158 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/src/shimoku/cli/cloud/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     9309 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/src/shimoku/cli/cloud/update.py
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/src/shimoku/cli/cloud_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     6064 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/src/shimoku/cli/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     3812 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/src/shimoku/cli/listen.py
--rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/src/shimoku/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     8608 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/src/shimoku/cli/persistence.py
--rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/src/shimoku/cli/playground.py
--rw-r--r--   0 runner    (1001) docker     (127)    14917 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/src/shimoku/cli/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:02:21.553793 shimoku-browser-2.3.1/src/shimoku/code_gen/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:02:21.553793 shimoku-browser-2.3.1/src/shimoku/code_gen/business_code_gen/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:02:21.553793 shimoku-browser-2.3.1/src/shimoku/code_gen/business_code_gen/apps_code_gen/
--rw-r--r--   0 runner    (1001) docker     (127)     5067 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/src/shimoku/code_gen/business_code_gen/apps_code_gen/code_gen_from_apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:02:21.553793 shimoku-browser-2.3.1/src/shimoku/code_gen/business_code_gen/apps_code_gen/data_sets_code_gen/
--rw-r--r--   0 runner    (1001) docker     (127)     3634 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/src/shimoku/code_gen/business_code_gen/apps_code_gen/data_sets_code_gen/code_gen_from_data_sets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:02:21.553793 shimoku-browser-2.3.1/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/code_gen_from_reports.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:02:21.557793 shimoku-browser-2.3.1/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/
--rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_annotated_echart.py
--rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_button.py
--rw-r--r--   0 runner    (1001) docker     (127)     4272 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_echarts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_form.py
--rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_html.py
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_iframe.py
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_indicators.py
--rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_modal.py
--rw-r--r--   0 runner    (1001) docker     (127)     4165 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_other.py
--rw-r--r--   0 runner    (1001) docker     (127)     6631 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     5810 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_tabs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5418 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/src/shimoku/code_gen/business_code_gen/code_gen_from_business.py
--rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/src/shimoku/code_gen/file_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/src/shimoku/code_gen/main_code_gen.py
--rw-r--r--   0 runner    (1001) docker     (127)    10222 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/src/shimoku/code_gen/tree_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/src/shimoku/code_gen/utils_code_gen.py
--rw-r--r--   0 runner    (1001) docker     (127)     3218 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/src/shimoku/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6258 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/src/shimoku/execution_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:02:21.557793 shimoku-browser-2.3.1/src/shimoku/playground/
--rw-r--r--   0 runner    (1001) docker     (127)     3630 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/src/shimoku/playground/execute_local_server.py
--rw-r--r--   0 runner    (1001) docker     (127)    35031 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/src/shimoku/playground/local_server.py
--rw-r--r--   0 runner    (1001) docker     (127)    40234 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/src/shimoku/playground/schema_classes.py
--rw-r--r--   0 runner    (1001) docker     (127)    14949 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/src/shimoku/playground/schema_parameter_classses.py
--rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/src/shimoku/playground/websockets_server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:02:21.557793 shimoku-browser-2.3.1/src/shimoku/plt/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:02:21.561793 shimoku-browser-2.3.1/src/shimoku/plt/EChart_definitions/
--rw-r--r--   0 runner    (1001) docker     (127)    12979 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/src/shimoku/plt/EChart_definitions/bar.py
--rw-r--r--   0 runner    (1001) docker     (127)    16008 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/src/shimoku/plt/EChart_definitions/default_echart_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/src/shimoku/plt/EChart_definitions/funnel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/src/shimoku/plt/EChart_definitions/gauge.py
--rw-r--r--   0 runner    (1001) docker     (127)     3595 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/src/shimoku/plt/EChart_definitions/gauge_indicator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3204 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/src/shimoku/plt/EChart_definitions/heatmap.py
--rw-r--r--   0 runner    (1001) docker     (127)    20924 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/src/shimoku/plt/EChart_definitions/line.py
--rw-r--r--   0 runner    (1001) docker     (127)     6117 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/src/shimoku/plt/EChart_definitions/line_and_bar.py
--rw-r--r--   0 runner    (1001) docker     (127)     5164 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/src/shimoku/plt/EChart_definitions/pie.py
--rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/src/shimoku/plt/EChart_definitions/radar.py
--rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/src/shimoku/plt/EChart_definitions/sankey.py
--rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/src/shimoku/plt/EChart_definitions/scatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5580 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/src/shimoku/plt/EChart_definitions/shimoku_gauge.py
--rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/src/shimoku/plt/EChart_definitions/sunburst.py
--rw-r--r--   0 runner    (1001) docker     (127)     6576 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/src/shimoku/plt/EChart_definitions/top_bottom.py
--rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/src/shimoku/plt/EChart_definitions/tree.py
--rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/src/shimoku/plt/EChart_definitions/treemap.py
--rw-r--r--   0 runner    (1001) docker     (127)     7822 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/src/shimoku/plt/EChart_definitions/waterfall.py
--rw-r--r--   0 runner    (1001) docker     (127)    13178 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/src/shimoku/plt/bentobox_charts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:02:21.561793 shimoku-browser-2.3.1/src/shimoku/plt/generated_headers/
--rw-r--r--   0 runner    (1001) docker     (127)    37818 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/src/shimoku/plt/generated_headers/PlotLayerHeader.py
--rw-r--r--   0 runner    (1001) docker     (127)    88351 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/src/shimoku/plt/plt_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)    19762 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/src/shimoku/plt/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4304 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/src/shimoku/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:02:21.581793 shimoku-browser-2.3.1/src/shimoku_browser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-09 08:02:21.000000 shimoku-browser-2.3.1/src/shimoku_browser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14978 2024-04-09 08:02:21.000000 shimoku-browser-2.3.1/src/shimoku_browser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 08:02:21.000000 shimoku-browser-2.3.1/src/shimoku_browser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 08:02:21.000000 shimoku-browser-2.3.1/src/shimoku_browser.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-09 08:02:21.000000 shimoku-browser-2.3.1/src/shimoku_browser.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-09 08:02:21.000000 shimoku-browser-2.3.1/src/shimoku_browser.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:02:21.561793 shimoku-browser-2.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4939 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/tests/Jupyter_notebook_test.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:02:21.565793 shimoku-browser-2.3.1/tests/mockable_tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:02:21.565793 shimoku-browser-2.3.1/tests/mockable_tests/correct_action_scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/tests/mockable_tests/correct_action_scripts/correct_action.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:02:21.569793 shimoku-browser-2.3.1/tests/mockable_tests/error_action_scripts/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/tests/mockable_tests/error_action_scripts/action_cant_have_no_params.py
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/tests/mockable_tests/error_action_scripts/action_param_must_be_Client.py
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/tests/mockable_tests/error_action_scripts/action_param_must_be_annotated.py
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/tests/mockable_tests/error_action_scripts/action_param_must_be_shimoku_client.py
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/tests/mockable_tests/error_action_scripts/cant_annotate_client_param_to_arb_name.py
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/tests/mockable_tests/error_action_scripts/cant_assign_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/tests/mockable_tests/error_action_scripts/cant_assign_client_in_class.py
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/tests/mockable_tests/error_action_scripts/cant_assign_client_to_subscript.py
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/tests/mockable_tests/error_action_scripts/cant_assign_to_shimoku_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/tests/mockable_tests/error_action_scripts/cant_define_action_in_class.py
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/tests/mockable_tests/error_action_scripts/cant_define_async_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/tests/mockable_tests/error_action_scripts/cant_define_more_than_one_action.py
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/tests/mockable_tests/error_action_scripts/cant_have_arb_params_in_action.py
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/tests/mockable_tests/error_action_scripts/cant_have_client_as_part_of_annotation.py
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/tests/mockable_tests/error_action_scripts/cant_have_non_annotated_param.py
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/tests/mockable_tests/error_action_scripts/cant_import_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/tests/mockable_tests/error_action_scripts/cant_import_from_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/tests/mockable_tests/error_action_scripts/cant_pass_incorrect_type_to_function.py
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/tests/mockable_tests/error_action_scripts/cant_pass_incorrect_type_to_kwargs.py
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/tests/mockable_tests/error_action_scripts/cant_rename_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/tests/mockable_tests/error_action_scripts/cant_return_shimoku_client.py
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/tests/mockable_tests/error_action_scripts/needs_action_function.py
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/tests/mockable_tests/error_action_scripts/needs_import_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/tests/mockable_tests/error_action_scripts/shimoku_client_param_must_be_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3457 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/tests/mockable_tests/mock_classes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2135 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/tests/mockable_tests/test_actions.py
--rw-r--r--   0 runner    (1001) docker     (127)    14050 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/tests/mockable_tests/test_activity_metadata_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4926 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/tests/mockable_tests/test_app_metadata_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     6922 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/tests/mockable_tests/test_business_metadata_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    16015 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/tests/mockable_tests/test_code_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6594 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/tests/mockable_tests/test_dashboard_metadata_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    22109 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:02:21.573793 shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/annotation_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/area.py
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/bar.py
--rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/bar_and_line_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/bentobox.py
--rw-r--r--   0 runner    (1001) docker     (127)     4111 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/chart_and_indicators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:02:21.581793 shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/data/
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/data/annotation_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/data/bar_and_line.py
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/data/bentobox_indicator.py
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/data/default.py
--rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/data/dynamic_conditional_and_auto_send_input_form.py
--rw-r--r--   0 runner    (1001) docker     (127)   129464 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/data/flow_and_rainfall.py
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/data/free_echarts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/data/free_echarts_raw.py
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/data/funnel.py
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/data/heatmap.py
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/data/horizontal_bar.py
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/data/html.py
--rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/data/indicator.py
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/data/indicator_color_by_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/data/input_form.py
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/data/line_with_confidence_area.py
--rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/data/noise.py
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/data/pie.py
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/data/radar.py
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/data/random_waterfall.py
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/data/sankey.py
--rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/data/scatter_test.csv
--rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/data/scatter_with_effect.py
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/data/segmented_line.py
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/data/stacked_area.py
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/data/suburst.py
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/data/summary_line.py
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/data/table.py
--rw-r--r--   0 runner    (1001) docker     (127)     9810 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/data/table_with_labels.py
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/data/test_stack_distribution.csv
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/data/tree.py
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/data/waterfall.py
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/data/zero_centered.py
--rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/doughnut.py
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/dynamic_conditional_and_auto_send_input_form.py
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/free_echarts.py
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/free_echarts_raw.py
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/funnel.py
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/gauge_indicator.py
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/get_input_forms.py
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/heatmap.py
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/horizontal_bar.py
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/html.py
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/iframe.py
--rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/indicator.py
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/indicator_color_by_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     7594 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/infographics.py
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/input_form.py
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/line.py
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/line_with_confidence_area.py
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/marked_line.py
--rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/modal.py
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/pie.py
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/predictive_line.py
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/radar.py
--rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/rainfall_area.py
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/rainfall_line.py
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/rose.py
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/sankey.py
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/scatter.py
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/scatter_with_effect.py
--rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/segmented_area_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)      921 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/segmented_line_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/shimoku_gauges.py
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/speed_gauge.py
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/stacked_area.py
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/stacked_bar.py
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/stacked_horizontal_bar.py
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/summary_line.py
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/sunburst.py
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/table.py
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/table_with_lables.py
--rw-r--r--   0 runner    (1001) docker     (127)     4610 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/tabs.py
--rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/tree.py
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/treemap.py
--rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/variants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/waterfall.py
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/zero_centered_bar.py
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/tests/mockable_tests/test_report_metadata_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4480 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/tests/mockable_tests/test_roles.py
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/tests/mockable_tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7905 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/tests/test_ai_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3124 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/tests/test_components_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/tests/test_data_managing_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4696 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/tests/test_file_metadata_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-09 08:02:06.000000 shimoku-browser-2.3.1/tests/test_universe_metadata_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:27:52.107904 shimoku_browser-2.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:27:52.059903 shimoku_browser-2.4.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:27:52.059903 shimoku_browser-2.4.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:27:52.059903 shimoku_browser-2.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/.github/workflows/publish-testpypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7625 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5220 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-10 08:27:52.107904 shimoku_browser-2.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8321 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/SECURITY.md
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:27:52.059903 shimoku_browser-2.4.0/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     7028 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/scripts/user_classes_header_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-05-10 08:27:52.107904 shimoku_browser-2.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/setup_browser.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:27:52.055903 shimoku_browser-2.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:27:52.059903 shimoku_browser-2.4.0/src/shimoku/
+-rw-r--r--   0 runner    (1001) docker     (127)    17476 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/src/shimoku/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:27:52.059903 shimoku_browser-2.4.0/src/shimoku/actions_execution/
+-rw-r--r--   0 runner    (1001) docker     (127)    15089 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/src/shimoku/actions_execution/execute_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/src/shimoku/actions_execution/front_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:27:52.063903 shimoku_browser-2.4.0/src/shimoku/ai/
+-rw-r--r--   0 runner    (1001) docker     (127)    33016 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/src/shimoku/ai/ai_layer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:27:52.063903 shimoku_browser-2.4.0/src/shimoku/ai/generated_headers/
+-rw-r--r--   0 runner    (1001) docker     (127)     4810 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/src/shimoku/ai/generated_headers/AILayerHeader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:27:52.063903 shimoku_browser-2.4.0/src/shimoku/api/
+-rw-r--r--   0 runner    (1001) docker     (127)    30469 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/src/shimoku/api/base_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19697 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/src/shimoku/api/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:27:52.063903 shimoku_browser-2.4.0/src/shimoku/api/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     3718 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/src/shimoku/api/resources/action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/src/shimoku/api/resources/action_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9183 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/src/shimoku/api/resources/activity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/src/shimoku/api/resources/activity_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17613 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/src/shimoku/api/resources/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8524 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/src/shimoku/api/resources/business.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/src/shimoku/api/resources/business_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4993 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/src/shimoku/api/resources/dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11235 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/src/shimoku/api/resources/data_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/src/shimoku/api/resources/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/src/shimoku/api/resources/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10082 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/src/shimoku/api/resources/report.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:27:52.063903 shimoku_browser-2.4.0/src/shimoku/api/resources/reports/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:27:52.067903 shimoku_browser-2.4.0/src/shimoku/api/resources/reports/charts/
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/src/shimoku/api/resources/reports/charts/annotated_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/src/shimoku/api/resources/reports/charts/button.py
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/src/shimoku/api/resources/reports/charts/echart.py
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/src/shimoku/api/resources/reports/charts/html.py
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/src/shimoku/api/resources/reports/charts/iframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/src/shimoku/api/resources/reports/charts/indicator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/src/shimoku/api/resources/reports/charts/input_form.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2271 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/src/shimoku/api/resources/reports/charts/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/src/shimoku/api/resources/reports/filter_data_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/src/shimoku/api/resources/reports/modal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3779 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/src/shimoku/api/resources/reports/tabs_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/src/shimoku/api/resources/reports/unsupported.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6665 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/src/shimoku/api/resources/role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6653 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/src/shimoku/api/resources/universe.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:27:52.067903 shimoku_browser-2.4.0/src/shimoku/api/user_access_classes/
+-rw-r--r--   0 runner    (1001) docker     (127)     5868 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/src/shimoku/api/user_access_classes/actions_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11082 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/src/shimoku/api/user_access_classes/activities_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/src/shimoku/api/user_access_classes/activity_templates_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10255 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/src/shimoku/api/user_access_classes/apps_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14675 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/src/shimoku/api/user_access_classes/businesses_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9947 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/src/shimoku/api/user_access_classes/dashboards_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3664 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/src/shimoku/api/user_access_classes/data_sets_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9899 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/src/shimoku/api/user_access_classes/files_layer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:27:52.071903 shimoku_browser-2.4.0/src/shimoku/api/user_access_classes/generated_headers/
+-rw-r--r--   0 runner    (1001) docker     (127)     2630 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/src/shimoku/api/user_access_classes/generated_headers/ActionsLayerHeader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6715 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/src/shimoku/api/user_access_classes/generated_headers/ActivitiesLayerHeader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/src/shimoku/api/user_access_classes/generated_headers/ActivityTemplatesLayerHeader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7028 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/src/shimoku/api/user_access_classes/generated_headers/BoardsLayerHeader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/src/shimoku/api/user_access_classes/generated_headers/ComponentsLayerHeader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/src/shimoku/api/user_access_classes/generated_headers/DataSetsLayerHeader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4958 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/src/shimoku/api/user_access_classes/generated_headers/FilesLayerHeader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6936 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/src/shimoku/api/user_access_classes/generated_headers/MenuPathsLayerHeader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/src/shimoku/api/user_access_classes/generated_headers/UniversesLayerHeader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7919 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/src/shimoku/api/user_access_classes/generated_headers/WorkspacesLayerHeader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/src/shimoku/api/user_access_classes/reports_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4240 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/src/shimoku/api/user_access_classes/universes_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20693 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/src/shimoku/api/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7223 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/src/shimoku/async_execution_pool.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:27:52.071903 shimoku_browser-2.4.0/src/shimoku/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)    20258 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/src/shimoku/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:27:52.071903 shimoku_browser-2.4.0/src/shimoku/cli/cloud/
+-rw-r--r--   0 runner    (1001) docker     (127)    14378 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/src/shimoku/cli/cloud/cascade_get_resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11288 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/src/shimoku/cli/cloud/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19454 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/src/shimoku/cli/cloud/delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5696 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/src/shimoku/cli/cloud/execute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9860 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/src/shimoku/cli/cloud/get.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32158 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/src/shimoku/cli/cloud/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9309 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/src/shimoku/cli/cloud/update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/src/shimoku/cli/cloud_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6064 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/src/shimoku/cli/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3812 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/src/shimoku/cli/listen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/src/shimoku/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8608 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/src/shimoku/cli/persistence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/src/shimoku/cli/playground.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14917 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/src/shimoku/cli/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:27:52.075904 shimoku_browser-2.4.0/src/shimoku/code_gen/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:27:52.075904 shimoku_browser-2.4.0/src/shimoku/code_gen/business_code_gen/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:27:52.075904 shimoku_browser-2.4.0/src/shimoku/code_gen/business_code_gen/apps_code_gen/
+-rw-r--r--   0 runner    (1001) docker     (127)     5067 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/src/shimoku/code_gen/business_code_gen/apps_code_gen/code_gen_from_apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:27:52.075904 shimoku_browser-2.4.0/src/shimoku/code_gen/business_code_gen/apps_code_gen/data_sets_code_gen/
+-rw-r--r--   0 runner    (1001) docker     (127)     3634 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/src/shimoku/code_gen/business_code_gen/apps_code_gen/data_sets_code_gen/code_gen_from_data_sets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:27:52.075904 shimoku_browser-2.4.0/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/code_gen_from_reports.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:27:52.075904 shimoku_browser-2.4.0/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/
+-rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_annotated_echart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_button.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4272 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_echarts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_form.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_html.py
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_iframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_indicators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_modal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4165 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_other.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6631 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5810 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_tabs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5418 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/src/shimoku/code_gen/business_code_gen/code_gen_from_business.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/src/shimoku/code_gen/file_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/src/shimoku/code_gen/main_code_gen.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10222 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/src/shimoku/code_gen/tree_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/src/shimoku/code_gen/utils_code_gen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3218 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/src/shimoku/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6258 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/src/shimoku/execution_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:27:52.079903 shimoku_browser-2.4.0/src/shimoku/playground/
+-rw-r--r--   0 runner    (1001) docker     (127)     3630 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/src/shimoku/playground/execute_local_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35031 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/src/shimoku/playground/local_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40234 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/src/shimoku/playground/schema_classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14949 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/src/shimoku/playground/schema_parameter_classses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/src/shimoku/playground/websockets_server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:27:52.079903 shimoku_browser-2.4.0/src/shimoku/plt/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:27:52.083903 shimoku_browser-2.4.0/src/shimoku/plt/EChart_definitions/
+-rw-r--r--   0 runner    (1001) docker     (127)    12979 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/src/shimoku/plt/EChart_definitions/bar.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16008 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/src/shimoku/plt/EChart_definitions/default_echart_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/src/shimoku/plt/EChart_definitions/funnel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/src/shimoku/plt/EChart_definitions/gauge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3595 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/src/shimoku/plt/EChart_definitions/gauge_indicator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3204 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/src/shimoku/plt/EChart_definitions/heatmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20924 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/src/shimoku/plt/EChart_definitions/line.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6117 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/src/shimoku/plt/EChart_definitions/line_and_bar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5164 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/src/shimoku/plt/EChart_definitions/pie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/src/shimoku/plt/EChart_definitions/radar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/src/shimoku/plt/EChart_definitions/sankey.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/src/shimoku/plt/EChart_definitions/scatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5580 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/src/shimoku/plt/EChart_definitions/shimoku_gauge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/src/shimoku/plt/EChart_definitions/sunburst.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6576 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/src/shimoku/plt/EChart_definitions/top_bottom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/src/shimoku/plt/EChart_definitions/tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/src/shimoku/plt/EChart_definitions/treemap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7822 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/src/shimoku/plt/EChart_definitions/waterfall.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13178 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/src/shimoku/plt/bentobox_charts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:27:52.083903 shimoku_browser-2.4.0/src/shimoku/plt/generated_headers/
+-rw-r--r--   0 runner    (1001) docker     (127)    38439 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/src/shimoku/plt/generated_headers/PlotLayerHeader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    91547 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/src/shimoku/plt/plt_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19762 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/src/shimoku/plt/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4304 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/src/shimoku/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:27:52.107904 shimoku_browser-2.4.0/src/shimoku_browser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-10 08:27:52.000000 shimoku_browser-2.4.0/src/shimoku_browser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14978 2024-05-10 08:27:52.000000 shimoku_browser-2.4.0/src/shimoku_browser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 08:27:52.000000 shimoku_browser-2.4.0/src/shimoku_browser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 08:27:51.000000 shimoku_browser-2.4.0/src/shimoku_browser.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-10 08:27:52.000000 shimoku_browser-2.4.0/src/shimoku_browser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-10 08:27:52.000000 shimoku_browser-2.4.0/src/shimoku_browser.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:27:52.083903 shimoku_browser-2.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4939 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/tests/Jupyter_notebook_test.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:27:52.087904 shimoku_browser-2.4.0/tests/mockable_tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:27:52.087904 shimoku_browser-2.4.0/tests/mockable_tests/correct_action_scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/tests/mockable_tests/correct_action_scripts/correct_action.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:27:52.091904 shimoku_browser-2.4.0/tests/mockable_tests/error_action_scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/tests/mockable_tests/error_action_scripts/action_cant_have_no_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/tests/mockable_tests/error_action_scripts/action_param_must_be_Client.py
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/tests/mockable_tests/error_action_scripts/action_param_must_be_annotated.py
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/tests/mockable_tests/error_action_scripts/action_param_must_be_shimoku_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/tests/mockable_tests/error_action_scripts/cant_annotate_client_param_to_arb_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/tests/mockable_tests/error_action_scripts/cant_assign_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/tests/mockable_tests/error_action_scripts/cant_assign_client_in_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/tests/mockable_tests/error_action_scripts/cant_assign_client_to_subscript.py
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/tests/mockable_tests/error_action_scripts/cant_assign_to_shimoku_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/tests/mockable_tests/error_action_scripts/cant_define_action_in_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/tests/mockable_tests/error_action_scripts/cant_define_async_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/tests/mockable_tests/error_action_scripts/cant_define_more_than_one_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/tests/mockable_tests/error_action_scripts/cant_have_arb_params_in_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/tests/mockable_tests/error_action_scripts/cant_have_client_as_part_of_annotation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/tests/mockable_tests/error_action_scripts/cant_have_non_annotated_param.py
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/tests/mockable_tests/error_action_scripts/cant_import_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/tests/mockable_tests/error_action_scripts/cant_import_from_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/tests/mockable_tests/error_action_scripts/cant_pass_incorrect_type_to_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/tests/mockable_tests/error_action_scripts/cant_pass_incorrect_type_to_kwargs.py
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/tests/mockable_tests/error_action_scripts/cant_rename_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/tests/mockable_tests/error_action_scripts/cant_return_shimoku_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/tests/mockable_tests/error_action_scripts/needs_action_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/tests/mockable_tests/error_action_scripts/needs_import_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/tests/mockable_tests/error_action_scripts/shimoku_client_param_must_be_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3457 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/tests/mockable_tests/mock_classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2135 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/tests/mockable_tests/test_actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14050 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/tests/mockable_tests/test_activity_metadata_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4926 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/tests/mockable_tests/test_app_metadata_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6922 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/tests/mockable_tests/test_business_metadata_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16015 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/tests/mockable_tests/test_code_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6594 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/tests/mockable_tests/test_dashboard_metadata_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22109 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:27:52.099904 shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/annotation_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/area.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/bar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/bar_and_line_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/bentobox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4111 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/chart_and_indicators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:27:52.107904 shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/data/annotation_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/data/bar_and_line.py
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/data/bentobox_indicator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/data/default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/data/dynamic_conditional_and_auto_send_input_form.py
+-rw-r--r--   0 runner    (1001) docker     (127)   129464 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/data/flow_and_rainfall.py
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/data/free_echarts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/data/free_echarts_raw.py
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/data/funnel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/data/heatmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/data/horizontal_bar.py
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/data/html.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/data/indicator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/data/indicator_color_by_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/data/input_form.py
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/data/line_with_confidence_area.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/data/noise.py
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/data/pie.py
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/data/radar.py
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/data/random_waterfall.py
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/data/sankey.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/data/scatter_test.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/data/scatter_with_effect.py
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/data/segmented_line.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/data/stacked_area.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/data/suburst.py
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/data/summary_line.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/data/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9810 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/data/table_with_labels.py
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/data/test_stack_distribution.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/data/tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/data/waterfall.py
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/data/zero_centered.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/doughnut.py
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/dynamic_conditional_and_auto_send_input_form.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/free_echarts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/free_echarts_raw.py
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/funnel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/gauge_indicator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/get_input_forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/heatmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/horizontal_bar.py
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/html.py
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/iframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/indicator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/indicator_color_by_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7594 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/infographics.py
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/input_form.py
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/line.py
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/line_with_confidence_area.py
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/marked_line.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/modal.py
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/pie.py
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/predictive_line.py
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/radar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/rainfall_area.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/rainfall_line.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/rose.py
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/sankey.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/scatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/scatter_with_effect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/segmented_area_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/segmented_line_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/shimoku_gauges.py
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/speed_gauge.py
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/stacked_area.py
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/stacked_bar.py
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/stacked_horizontal_bar.py
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/summary_line.py
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/sunburst.py
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/table_with_lables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4610 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/tabs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/treemap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/variants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/waterfall.py
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/zero_centered_bar.py
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/tests/mockable_tests/test_report_metadata_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4480 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/tests/mockable_tests/test_roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/tests/mockable_tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7905 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/tests/test_ai_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3124 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/tests/test_components_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/tests/test_data_managing_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4696 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/tests/test_file_metadata_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-10 08:27:40.000000 shimoku_browser-2.4.0/tests/test_universe_metadata_api.py
```

### Comparing `shimoku-browser-2.3.1/.coveragerc` & `shimoku_browser-2.4.0/.coveragerc`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/.github/ISSUE_TEMPLATE/bug_report.md` & `shimoku_browser-2.4.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/.github/ISSUE_TEMPLATE/feature_request.md` & `shimoku_browser-2.4.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/.github/pull_request_template.md` & `shimoku_browser-2.4.0/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/.github/workflows/publish-testpypi.yml` & `shimoku_browser-2.4.0/.github/workflows/publish-testpypi.yml`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/.github/workflows/publish-to-pypi.yml` & `shimoku_browser-2.4.0/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/.gitignore` & `shimoku_browser-2.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/CHANGELOG.md` & `shimoku_browser-2.4.0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # CHANGELOG
 
+## 2.4.0 (2024-10-05)
+
+-  Added buttons to table rows
+
 ## 2.3.1 (2024-09-04)
 
 - Fixed CORS error when deleting resources with Actions
 
 ## 2.3.0 (2024-08-04)
 
 - User accounts handling through the SDK
```

### Comparing `shimoku-browser-2.3.1/CODE_OF_CONDUCT.md` & `shimoku_browser-2.4.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/CONTRIBUTING.md` & `shimoku_browser-2.4.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/LICENSE.txt` & `shimoku_browser-2.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/PKG-INFO` & `shimoku_browser-2.4.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shimoku-browser
-Version: 2.3.1
+Version: 2.4.0
 Summary: Shimoku enables you to build Data Products in just hours and allows you to create Predictive Analytics Products with Artificial Intelligence capabilities.
 Home-page: https://github.com/shimoku-tech/shimoku-api-python
 Author: Shimoku
 Author-email: contact@shimoku.com
 License: MIT
 Project-URL: Documentation, https://docs.shimoku.com/
 Platform: any
```

### Comparing `shimoku-browser-2.3.1/README.md` & `shimoku_browser-2.4.0/README.md`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/SECURITY.md` & `shimoku_browser-2.4.0/SECURITY.md`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/scripts/user_classes_header_generator.py` & `shimoku_browser-2.4.0/scripts/user_classes_header_generator.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import dataclasses
 import inspect
 import importlib
 import os
 from shimoku.utils import get_args_with_defaults
 import subprocess
 
 base_path = os.path.abspath(os.path.join(os.path.dirname(__file__), ".."))
@@ -35,108 +36,165 @@
         if isinstance(default_value, str):
             default_value = f'"{default_value}"'
         return f"        {name}: {handle_annotation(annotation)} = {default_value},"
     else:
         return f"        {name}: {handle_annotation(annotation)},"
 
 
-for target_path, target_file in target_paths.items():
-    output_path = os.path.join(target_path, "generated_headers")
-    if not os.path.exists(output_path):
-        os.makedirs(output_path)
-    for file in os.listdir(target_path):
-        if file != target_file and target_file != "*":
+def handle_method(method) -> list[str]:
+    method_code_lines = []
+    method_code_lines.extend(
+        [
+            f"    def {method[0]}(",
+            "        self,",
+            *[
+                handle_parameter(
+                    arg,
+                    method[1].__annotations__[arg],
+                    get_args_with_defaults(method[1]),
+                )
+                for arg in method[1].__annotations__
+                if arg not in ["self", "return"]
+            ],
+        ]
+    )
+    sig = inspect.signature(method[1])
+    params = sig.parameters.values()
+    has_kwargs = any([True for p in params if p.kind == p.VAR_KEYWORD])
+    if has_kwargs:
+        method_code_lines.append("        **kwargs,")
+    if "return" in method[1].__annotations__:
+        method_code_lines.append(
+            f'    ) -> {handle_annotation(method[1].__annotations__["return"])}:'
+        )
+    else:
+        method_code_lines.append("    ):")
+    method_code_lines.extend(
+        [
+            f'        """{method[1].__doc__}"""',
+            "        pass",
+            "",
+        ]
+    )
+    return method_code_lines
+
+
+def handle_class(class_for_generation) -> list[str]:
+    print(class_for_generation[0])
+    is_dataclass = hasattr(class_for_generation[1], "__dataclass_fields__")
+
+    fields_code_lines = []
+    if is_dataclass:
+        for field in class_for_generation[1].__dataclass_fields__.values():
+            if field.default is dataclasses.MISSING:
+                fields_code_lines.append(f"    {field.name}: {handle_annotation(field.type)}")
+            else:
+                fields_code_lines.append(
+                    f"    {field.name}: {handle_annotation(field.type)} = {field.default}"
+                )
+
+    methods = inspect.getmembers(
+        class_for_generation[1], predicate=inspect.isfunction
+    )
+    methods_code_lines = []
+    for method in methods:
+        if method[0].startswith("_"):
             continue
-        if file.endswith(".py") and not file.startswith("__"):
-            print(
-                f'{os.path.relpath(target_path, base_path).replace(os.sep, ".")[4:]}.{file[:-3]}'
-            )
-            module = importlib.import_module(
-                f'{os.path.relpath(target_path, base_path).replace(os.sep, ".")[4:]}.{file[:-3]}'
-            )
-            classes_for_generation = []
-            for name, obj in inspect.getmembers(module):
-                if not inspect.isclass(obj):
-                    continue
-                if name.startswith("_"):
-                    continue
-                if not hasattr(obj, "_use_info_logging") or not obj._use_info_logging:
-                    continue
-                classes_for_generation.append((name, obj))
+        methods_code_lines.extend(handle_method(method))
 
-            if not classes_for_generation:
-                continue
+    inner_classes = inspect.getmembers(
+        class_for_generation[1], predicate=inspect.isclass
+    )
 
-            classes_code_lines = []
-            for class_for_generation in classes_for_generation:
-                print(class_for_generation[0])
-                methods = inspect.getmembers(
-                    class_for_generation[1], predicate=inspect.isfunction
+    inner_classes_code_lines = []
+    for inner_class in inner_classes:
+        if inner_class[0].startswith("_"):
+            continue
+        inner_classes_code_lines.extend(["    "+line for line in handle_class(inner_class)])
+
+    if is_dataclass:
+        class_header_code_lines = [
+            f"@dataclass",
+            f"class {class_for_generation[0]}:",
+            '    """',
+            *["    " + line for line in fields_code_lines],
+            '    """',
+        ]
+    else:
+        class_header_code_lines = [
+            f"class {class_for_generation[0]}Header:",
+            f'    """{class_for_generation[1].__doc__}"""',
+            ""
+        ]
+
+    class_code_lines = [
+        "",
+        *class_header_code_lines,
+        *fields_code_lines,
+        "",
+        *inner_classes_code_lines,
+        *methods_code_lines,
+    ]
+    return class_code_lines
+
+
+def main():
+    for target_path, target_file in target_paths.items():
+        output_path = os.path.join(target_path, "generated_headers")
+        if not os.path.exists(output_path):
+            os.makedirs(output_path)
+        for file in os.listdir(target_path):
+            if file != target_file and target_file != "*":
+                continue
+            if file.endswith(".py") and not file.startswith("__"):
+                print(
+                    f'{os.path.relpath(target_path, base_path).replace(os.sep, ".")[4:]}.{file[:-3]}'
                 )
-                methods_code_lines = []
-                for method in methods:
-                    if method[0].startswith("_"):
+                module = importlib.import_module(
+                    f'{os.path.relpath(target_path, base_path).replace(os.sep, ".")[4:]}.{file[:-3]}'
+                )
+                classes_for_generation = []
+                for name, obj in inspect.getmembers(module):
+                    if not inspect.isclass(obj):
+                        continue
+                    if name.startswith("_"):
+                        continue
+                    if not hasattr(obj, "_use_info_logging") or not obj._use_info_logging:
                         continue
-                    methods_code_lines.extend(
-                        [
-                            f"    def {method[0]}(",
-                            "        self,",
-                            *[
-                                handle_parameter(
-                                    arg,
-                                    method[1].__annotations__[arg],
-                                    get_args_with_defaults(method[1]),
-                                )
-                                for arg in method[1].__annotations__
-                                if arg not in ["self", "return"]
-                            ],
-                        ]
-                    )
-                    sig = inspect.signature(method[1])
-                    params = sig.parameters.values()
-                    has_kwargs = any([True for p in params if p.kind == p.VAR_KEYWORD])
-                    if has_kwargs:
-                        methods_code_lines.append("        **kwargs,")
-                    if "return" in method[1].__annotations__:
-                        methods_code_lines.append(
-                            f'    ) -> {handle_annotation(method[1].__annotations__["return"])}:'
-                        )
-                    else:
-                        methods_code_lines.append("    ):")
-                    methods_code_lines.extend(
-                        [
-                            f'        """{method[1].__doc__}"""',
-                            "        pass",
-                            "",
-                        ]
-                    )
+                    classes_for_generation.append((name, obj))
 
-                class_code_lines = [
-                    "",
-                    f"class {class_for_generation[0]}Header:",
-                    f'    """{class_for_generation[1].__doc__}"""',
+                if not classes_for_generation:
+                    continue
+
+                classes_code_lines = []
+                for class_for_generation in classes_for_generation:
+                    classes_code_lines.extend(handle_class(class_for_generation))
+
+                main_code_lines = [
+                    "# This file was generated automatically by "
+                    "scripts/user_classes_header_generator.py do not modify it!",
+                    "# If the user access files are modified, this file has to be regenerated with the script.",
+                    "from typing import Optional, Union",
+                    "from pandas import DataFrame",
+                    "from dataclasses import dataclass",
+                    "import shimoku",
                     "",
-                    *methods_code_lines,
-                ]
-                classes_code_lines.extend(class_code_lines)
-            main_code_lines = [
-                "# This file was generated automatically by scripts/user_classes_header_generator.py do not modify it!",
-                "# If the user access files are modified, this file has to be regenerated with the script.",
-                "from typing import Optional, Union",
-                "from pandas import DataFrame",
-                "",
-                *classes_code_lines,
-            ]
-            with open(
-                os.path.join(output_path, f"{classes_for_generation[-1][0]}Header.py"),
-                "w",
-            ) as f:
-                f.write("\n".join(main_code_lines))
-
-            subprocess.run(
-                [
-                    "black",
-                    os.path.join(
-                        output_path, f"{classes_for_generation[-1][0]}Header.py"
-                    ),
+                    *classes_code_lines,
                 ]
-            )
+                with open(
+                    os.path.join(output_path, f"{classes_for_generation[-1][0]}Header.py"),
+                    "w",
+                ) as f:
+                    f.write("\n".join(main_code_lines))
+
+                subprocess.run(
+                    [
+                        "black",
+                        os.path.join(
+                            output_path, f"{classes_for_generation[-1][0]}Header.py"
+                        ),
+                    ]
+                )
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `shimoku-browser-2.3.1/setup.cfg` & `shimoku_browser-2.4.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/setup.py` & `shimoku_browser-2.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/setup_browser.cfg` & `shimoku_browser-2.4.0/setup_browser.cfg`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/src/shimoku/__init__.py` & `shimoku_browser-2.4.0/src/shimoku/__init__.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/src/shimoku/actions_execution/execute_action.py` & `shimoku_browser-2.4.0/src/shimoku/actions_execution/execute_action.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/src/shimoku/actions_execution/front_connection.py` & `shimoku_browser-2.4.0/src/shimoku/actions_execution/front_connection.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/src/shimoku/ai/ai_layer.py` & `shimoku_browser-2.4.0/src/shimoku/ai/ai_layer.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/src/shimoku/ai/generated_headers/AILayerHeader.py` & `shimoku_browser-2.4.0/src/shimoku/ai/generated_headers/AILayerHeader.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # This file was generated automatically by scripts/user_classes_header_generator.py do not modify it!
 # If the user access files are modified, this file has to be regenerated with the script.
 from typing import Optional, Union
 from pandas import DataFrame
+from dataclasses import dataclass
+import shimoku
 
 
 class AIFunctionMethodsHeader:
     """None"""
 
     def create_model(
         self,
```

### Comparing `shimoku-browser-2.3.1/src/shimoku/api/base_resource.py` & `shimoku_browser-2.4.0/src/shimoku/api/base_resource.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/src/shimoku/api/client.py` & `shimoku_browser-2.4.0/src/shimoku/api/client.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/src/shimoku/api/resources/action.py` & `shimoku_browser-2.4.0/src/shimoku/api/resources/action.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/src/shimoku/api/resources/action_template.py` & `shimoku_browser-2.4.0/src/shimoku/api/resources/action_template.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/src/shimoku/api/resources/activity.py` & `shimoku_browser-2.4.0/src/shimoku/api/resources/activity.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/src/shimoku/api/resources/activity_template.py` & `shimoku_browser-2.4.0/src/shimoku/api/resources/activity_template.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/src/shimoku/api/resources/app.py` & `shimoku_browser-2.4.0/src/shimoku/api/resources/app.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/src/shimoku/api/resources/business.py` & `shimoku_browser-2.4.0/src/shimoku/api/resources/business.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/src/shimoku/api/resources/business_user.py` & `shimoku_browser-2.4.0/src/shimoku/api/resources/business_user.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/src/shimoku/api/resources/dashboard.py` & `shimoku_browser-2.4.0/src/shimoku/api/resources/dashboard.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/src/shimoku/api/resources/data_set.py` & `shimoku_browser-2.4.0/src/shimoku/api/resources/data_set.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/src/shimoku/api/resources/event.py` & `shimoku_browser-2.4.0/src/shimoku/api/resources/event.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/src/shimoku/api/resources/file.py` & `shimoku_browser-2.4.0/src/shimoku/api/resources/file.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/src/shimoku/api/resources/report.py` & `shimoku_browser-2.4.0/src/shimoku/api/resources/report.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/src/shimoku/api/resources/reports/charts/indicator.py` & `shimoku_browser-2.4.0/src/shimoku/api/resources/reports/charts/indicator.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/src/shimoku/api/resources/reports/charts/table.py` & `shimoku_browser-2.4.0/src/shimoku/api/resources/reports/charts/table.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/src/shimoku/api/resources/reports/filter_data_set.py` & `shimoku_browser-2.4.0/src/shimoku/api/resources/reports/filter_data_set.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/src/shimoku/api/resources/reports/modal.py` & `shimoku_browser-2.4.0/src/shimoku/api/resources/reports/modal.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/src/shimoku/api/resources/reports/tabs_group.py` & `shimoku_browser-2.4.0/src/shimoku/api/resources/reports/tabs_group.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/src/shimoku/api/resources/role.py` & `shimoku_browser-2.4.0/src/shimoku/api/resources/role.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/src/shimoku/api/resources/universe.py` & `shimoku_browser-2.4.0/src/shimoku/api/resources/universe.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/src/shimoku/api/user_access_classes/actions_layer.py` & `shimoku_browser-2.4.0/src/shimoku/api/user_access_classes/actions_layer.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/src/shimoku/api/user_access_classes/activities_layer.py` & `shimoku_browser-2.4.0/src/shimoku/api/user_access_classes/activities_layer.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/src/shimoku/api/user_access_classes/activity_templates_layer.py` & `shimoku_browser-2.4.0/src/shimoku/api/user_access_classes/activity_templates_layer.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/src/shimoku/api/user_access_classes/apps_layer.py` & `shimoku_browser-2.4.0/src/shimoku/api/user_access_classes/apps_layer.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/src/shimoku/api/user_access_classes/businesses_layer.py` & `shimoku_browser-2.4.0/src/shimoku/api/user_access_classes/businesses_layer.py`

 * *Files 1% similar despite different names*

```diff
@@ -268,15 +268,15 @@
         non_referenced_reports = sorted(
             [
                 report
                 for report in reports
                 if report["path"] is not None
                 and create_normalized_name(report["path"]) not in sub_paths
             ],
-            key=lambda x: x["pathOrder"],
+            key=lambda x: x["pathOrder"] if x["pathOrder"] is not None else 0,
         )
         for report in non_referenced_reports:
             sub_path = report["path"]
             if sub_path not in sub_paths:
                 sub_paths.append(sub_path)
 
         tasks = []
```

### Comparing `shimoku-browser-2.3.1/src/shimoku/api/user_access_classes/dashboards_layer.py` & `shimoku_browser-2.4.0/src/shimoku/api/user_access_classes/dashboards_layer.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/src/shimoku/api/user_access_classes/data_sets_layer.py` & `shimoku_browser-2.4.0/src/shimoku/api/user_access_classes/data_sets_layer.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/src/shimoku/api/user_access_classes/files_layer.py` & `shimoku_browser-2.4.0/src/shimoku/api/user_access_classes/files_layer.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/src/shimoku/api/user_access_classes/generated_headers/ActionsLayerHeader.py` & `shimoku_browser-2.4.0/src/shimoku/api/user_access_classes/generated_headers/ActionsLayerHeader.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # This file was generated automatically by scripts/user_classes_header_generator.py do not modify it!
 # If the user access files are modified, this file has to be regenerated with the script.
 from typing import Optional, Union
 from pandas import DataFrame
+from dataclasses import dataclass
+import shimoku
 
 
 class ActionsLayerHeader:
     """
     This class is used to interact with the API at the Workspace layer
     """
```

### Comparing `shimoku-browser-2.3.1/src/shimoku/api/user_access_classes/generated_headers/ActivitiesLayerHeader.py` & `shimoku_browser-2.4.0/src/shimoku/api/user_access_classes/generated_headers/ActivitiesLayerHeader.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # This file was generated automatically by scripts/user_classes_header_generator.py do not modify it!
 # If the user access files are modified, this file has to be regenerated with the script.
 from typing import Optional, Union
 from pandas import DataFrame
+from dataclasses import dataclass
+import shimoku
 
 
 class ActivitiesLayerHeader:
     """
     This class is used to interact with the activities that are available in a menu path, through the API.
     """
```

### Comparing `shimoku-browser-2.3.1/src/shimoku/api/user_access_classes/generated_headers/ActivityTemplatesLayerHeader.py` & `shimoku_browser-2.4.0/src/shimoku/api/user_access_classes/generated_headers/ActivityTemplatesLayerHeader.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/src/shimoku/api/user_access_classes/generated_headers/BoardsLayerHeader.py` & `shimoku_browser-2.4.0/src/shimoku/api/user_access_classes/generated_headers/BoardsLayerHeader.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # This file was generated automatically by scripts/user_classes_header_generator.py do not modify it!
 # If the user access files are modified, this file has to be regenerated with the script.
 from typing import Optional, Union
 from pandas import DataFrame
+from dataclasses import dataclass
+import shimoku
 
 
 class BoardsLayerHeader:
     """
     This class is used to interact with the API at the board level.
     """
```

### Comparing `shimoku-browser-2.3.1/src/shimoku/api/user_access_classes/generated_headers/ComponentsLayerHeader.py` & `shimoku_browser-2.4.0/src/shimoku/api/user_access_classes/generated_headers/ComponentsLayerHeader.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # This file was generated automatically by scripts/user_classes_header_generator.py do not modify it!
 # If the user access files are modified, this file has to be regenerated with the script.
 from typing import Optional, Union
 from pandas import DataFrame
+from dataclasses import dataclass
+import shimoku
 
 
 class ComponentsLayerHeader:
     """
     This class is used to interact with the API at the component level.
     """
```

### Comparing `shimoku-browser-2.3.1/src/shimoku/api/user_access_classes/generated_headers/DataSetsLayerHeader.py` & `shimoku_browser-2.4.0/src/shimoku/api/user_access_classes/generated_headers/DataSetsLayerHeader.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # This file was generated automatically by scripts/user_classes_header_generator.py do not modify it!
 # If the user access files are modified, this file has to be regenerated with the script.
 from typing import Optional, Union
 from pandas import DataFrame
+from dataclasses import dataclass
+import shimoku
 
 
 class DataSetsLayerHeader:
     """
     This class is used to interact with the API at the data set level.
     """
```

### Comparing `shimoku-browser-2.3.1/src/shimoku/api/user_access_classes/generated_headers/FilesLayerHeader.py` & `shimoku_browser-2.4.0/src/shimoku/api/user_access_classes/generated_headers/FilesLayerHeader.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # This file was generated automatically by scripts/user_classes_header_generator.py do not modify it!
 # If the user access files are modified, this file has to be regenerated with the script.
 from typing import Optional, Union
 from pandas import DataFrame
+from dataclasses import dataclass
+import shimoku
 
 
 class FilesLayerHeader:
     """
     This class is used to interact with the API at the file level.
     """
```

### Comparing `shimoku-browser-2.3.1/src/shimoku/api/user_access_classes/generated_headers/MenuPathsLayerHeader.py` & `shimoku_browser-2.4.0/src/shimoku/api/user_access_classes/generated_headers/MenuPathsLayerHeader.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # This file was generated automatically by scripts/user_classes_header_generator.py do not modify it!
 # If the user access files are modified, this file has to be regenerated with the script.
 from typing import Optional, Union
 from pandas import DataFrame
+from dataclasses import dataclass
+import shimoku
 
 
 class MenuPathsLayerHeader:
     """
     This class is used to interact with the API at the Menu Path level.
     """
```

### Comparing `shimoku-browser-2.3.1/src/shimoku/api/user_access_classes/generated_headers/UniversesLayerHeader.py` & `shimoku_browser-2.4.0/src/shimoku/api/user_access_classes/generated_headers/UniversesLayerHeader.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # This file was generated automatically by scripts/user_classes_header_generator.py do not modify it!
 # If the user access files are modified, this file has to be regenerated with the script.
 from typing import Optional, Union
 from pandas import DataFrame
+from dataclasses import dataclass
+import shimoku
 
 
 class UniversesLayerHeader:
     """
     Class used to interact with the API at the universe level
     """
```

### Comparing `shimoku-browser-2.3.1/src/shimoku/api/user_access_classes/generated_headers/WorkspacesLayerHeader.py` & `shimoku_browser-2.4.0/src/shimoku/api/user_access_classes/generated_headers/WorkspacesLayerHeader.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # This file was generated automatically by scripts/user_classes_header_generator.py do not modify it!
 # If the user access files are modified, this file has to be regenerated with the script.
 from typing import Optional, Union
 from pandas import DataFrame
+from dataclasses import dataclass
+import shimoku
 
 
 class WorkspacesLayerHeader:
     """
     This class is used to interact with the API at the Workspace layer
     """
```

### Comparing `shimoku-browser-2.3.1/src/shimoku/api/user_access_classes/reports_layer.py` & `shimoku_browser-2.4.0/src/shimoku/api/user_access_classes/reports_layer.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/src/shimoku/api/user_access_classes/universes_layer.py` & `shimoku_browser-2.4.0/src/shimoku/api/user_access_classes/universes_layer.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/src/shimoku/api/utils.py` & `shimoku_browser-2.4.0/src/shimoku/api/utils.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/src/shimoku/async_execution_pool.py` & `shimoku_browser-2.4.0/src/shimoku/async_execution_pool.py`

 * *Files 2% similar despite different names*

```diff
@@ -180,11 +180,15 @@
             return result
 
         return wrapper
 
     new_class = type(cls.__name__, (cls,), {})
     for attr_name in dir(cls):
         attr = getattr(cls, attr_name)
-        if callable(attr) and not attr_name.startswith("_"):
+        if (
+            callable(attr) and
+            not attr_name.startswith("_") and
+            not hasattr(attr, "__dataclass_fields__")
+        ):
             setattr(new_class, attr_name, decorate_to_auto_async(attr))
 
     return new_class
```

### Comparing `shimoku-browser-2.3.1/src/shimoku/cli/__init__.py` & `shimoku_browser-2.4.0/src/shimoku/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/src/shimoku/cli/cloud/cascade_get_resources.py` & `shimoku_browser-2.4.0/src/shimoku/cli/cloud/cascade_get_resources.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/src/shimoku/cli/cloud/create.py` & `shimoku_browser-2.4.0/src/shimoku/cli/cloud/create.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/src/shimoku/cli/cloud/delete.py` & `shimoku_browser-2.4.0/src/shimoku/cli/cloud/delete.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/src/shimoku/cli/cloud/execute.py` & `shimoku_browser-2.4.0/src/shimoku/cli/cloud/execute.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/src/shimoku/cli/cloud/get.py` & `shimoku_browser-2.4.0/src/shimoku/cli/cloud/get.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/src/shimoku/cli/cloud/list.py` & `shimoku_browser-2.4.0/src/shimoku/cli/cloud/list.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/src/shimoku/cli/cloud/update.py` & `shimoku_browser-2.4.0/src/shimoku/cli/cloud/update.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/src/shimoku/cli/cloud_parser.py` & `shimoku_browser-2.4.0/src/shimoku/cli/cloud_parser.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/src/shimoku/cli/configuration.py` & `shimoku_browser-2.4.0/src/shimoku/cli/configuration.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/src/shimoku/cli/listen.py` & `shimoku_browser-2.4.0/src/shimoku/cli/listen.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/src/shimoku/cli/main.py` & `shimoku_browser-2.4.0/src/shimoku/cli/main.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/src/shimoku/cli/persistence.py` & `shimoku_browser-2.4.0/src/shimoku/cli/persistence.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/src/shimoku/cli/playground.py` & `shimoku_browser-2.4.0/src/shimoku/cli/playground.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/src/shimoku/cli/utils.py` & `shimoku_browser-2.4.0/src/shimoku/cli/utils.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/src/shimoku/code_gen/business_code_gen/apps_code_gen/code_gen_from_apps.py` & `shimoku_browser-2.4.0/src/shimoku/code_gen/business_code_gen/apps_code_gen/code_gen_from_apps.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/src/shimoku/code_gen/business_code_gen/apps_code_gen/data_sets_code_gen/code_gen_from_data_sets.py` & `shimoku_browser-2.4.0/src/shimoku/code_gen/business_code_gen/apps_code_gen/data_sets_code_gen/code_gen_from_data_sets.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/code_gen_from_reports.py` & `shimoku_browser-2.4.0/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/code_gen_from_reports.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_annotated_echart.py` & `shimoku_browser-2.4.0/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_annotated_echart.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_button.py` & `shimoku_browser-2.4.0/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_button.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_echarts.py` & `shimoku_browser-2.4.0/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_echarts.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_filter.py` & `shimoku_browser-2.4.0/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_filter.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_form.py` & `shimoku_browser-2.4.0/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_form.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_html.py` & `shimoku_browser-2.4.0/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_html.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_iframe.py` & `shimoku_browser-2.4.0/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_iframe.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_indicators.py` & `shimoku_browser-2.4.0/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_indicators.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_modal.py` & `shimoku_browser-2.4.0/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_modal.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_other.py` & `shimoku_browser-2.4.0/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_other.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_table.py` & `shimoku_browser-2.4.0/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_table.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_tabs.py` & `shimoku_browser-2.4.0/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_tabs.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/src/shimoku/code_gen/business_code_gen/code_gen_from_business.py` & `shimoku_browser-2.4.0/src/shimoku/code_gen/business_code_gen/code_gen_from_business.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/src/shimoku/code_gen/file_generator.py` & `shimoku_browser-2.4.0/src/shimoku/code_gen/file_generator.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/src/shimoku/code_gen/main_code_gen.py` & `shimoku_browser-2.4.0/src/shimoku/code_gen/main_code_gen.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/src/shimoku/code_gen/tree_generation.py` & `shimoku_browser-2.4.0/src/shimoku/code_gen/tree_generation.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/src/shimoku/code_gen/utils_code_gen.py` & `shimoku_browser-2.4.0/src/shimoku/code_gen/utils_code_gen.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/src/shimoku/exceptions.py` & `shimoku_browser-2.4.0/src/shimoku/exceptions.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/src/shimoku/execution_logger.py` & `shimoku_browser-2.4.0/src/shimoku/execution_logger.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/src/shimoku/playground/execute_local_server.py` & `shimoku_browser-2.4.0/src/shimoku/playground/execute_local_server.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/src/shimoku/playground/local_server.py` & `shimoku_browser-2.4.0/src/shimoku/playground/local_server.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/src/shimoku/playground/schema_classes.py` & `shimoku_browser-2.4.0/src/shimoku/playground/schema_classes.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/src/shimoku/playground/schema_parameter_classses.py` & `shimoku_browser-2.4.0/src/shimoku/playground/schema_parameter_classses.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/src/shimoku/playground/websockets_server.py` & `shimoku_browser-2.4.0/src/shimoku/playground/websockets_server.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/src/shimoku/plt/EChart_definitions/bar.py` & `shimoku_browser-2.4.0/src/shimoku/plt/EChart_definitions/bar.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/src/shimoku/plt/EChart_definitions/default_echart_options.py` & `shimoku_browser-2.4.0/src/shimoku/plt/EChart_definitions/default_echart_options.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/src/shimoku/plt/EChart_definitions/funnel.py` & `shimoku_browser-2.4.0/src/shimoku/plt/EChart_definitions/funnel.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/src/shimoku/plt/EChart_definitions/gauge.py` & `shimoku_browser-2.4.0/src/shimoku/plt/EChart_definitions/gauge.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/src/shimoku/plt/EChart_definitions/gauge_indicator.py` & `shimoku_browser-2.4.0/src/shimoku/plt/EChart_definitions/gauge_indicator.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/src/shimoku/plt/EChart_definitions/heatmap.py` & `shimoku_browser-2.4.0/src/shimoku/plt/EChart_definitions/heatmap.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/src/shimoku/plt/EChart_definitions/line.py` & `shimoku_browser-2.4.0/src/shimoku/plt/EChart_definitions/line.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/src/shimoku/plt/EChart_definitions/line_and_bar.py` & `shimoku_browser-2.4.0/src/shimoku/plt/EChart_definitions/line_and_bar.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/src/shimoku/plt/EChart_definitions/pie.py` & `shimoku_browser-2.4.0/src/shimoku/plt/EChart_definitions/pie.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/src/shimoku/plt/EChart_definitions/radar.py` & `shimoku_browser-2.4.0/src/shimoku/plt/EChart_definitions/radar.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/src/shimoku/plt/EChart_definitions/sankey.py` & `shimoku_browser-2.4.0/src/shimoku/plt/EChart_definitions/sankey.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/src/shimoku/plt/EChart_definitions/scatter.py` & `shimoku_browser-2.4.0/src/shimoku/plt/EChart_definitions/scatter.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/src/shimoku/plt/EChart_definitions/shimoku_gauge.py` & `shimoku_browser-2.4.0/src/shimoku/plt/EChart_definitions/shimoku_gauge.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/src/shimoku/plt/EChart_definitions/sunburst.py` & `shimoku_browser-2.4.0/src/shimoku/plt/EChart_definitions/sunburst.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/src/shimoku/plt/EChart_definitions/top_bottom.py` & `shimoku_browser-2.4.0/src/shimoku/plt/EChart_definitions/top_bottom.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/src/shimoku/plt/EChart_definitions/tree.py` & `shimoku_browser-2.4.0/src/shimoku/plt/EChart_definitions/tree.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/src/shimoku/plt/EChart_definitions/treemap.py` & `shimoku_browser-2.4.0/src/shimoku/plt/EChart_definitions/treemap.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/src/shimoku/plt/EChart_definitions/waterfall.py` & `shimoku_browser-2.4.0/src/shimoku/plt/EChart_definitions/waterfall.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/src/shimoku/plt/bentobox_charts.py` & `shimoku_browser-2.4.0/src/shimoku/plt/bentobox_charts.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/src/shimoku/plt/generated_headers/PlotLayerHeader.py` & `shimoku_browser-2.4.0/src/shimoku/plt/generated_headers/PlotLayerHeader.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,36 @@
 # This file was generated automatically by scripts/user_classes_header_generator.py do not modify it!
 # If the user access files are modified, this file has to be regenerated with the script.
 from typing import Optional, Union
 from pandas import DataFrame
+from dataclasses import dataclass
+import shimoku
 
 
 class PlotLayerHeader:
     """
     This class is a high level abstraction of the API, it is used to create components and data sets easily.
     """
 
+    @dataclass
+    class TableButtonColumnDefinition:
+        """
+        column_name: str
+        label: str
+        modals_column: Optional[str] = None
+        activities_column: Optional[str] = None
+        actions_column: Optional[str] = None
+        """
+
+        column_name: str
+        label: str
+        modals_column: Optional[str] = None
+        activities_column: Optional[str] = None
+        actions_column: Optional[str] = None
+
     def action_button(
         self,
         label: str,
         order: int,
         action_id: str,
         rows_size: Optional[int] = 1,
         cols_size: int = 2,
@@ -1049,22 +1067,25 @@
     ):
         """Create a sunburst chart"""
         pass
 
     def table(
         self,
         order: int,
-        data: Union[str, DataFrame, list[dict], dict],
+        data: Union[str, DataFrame, list[dict]],
         columns: Optional[list[str]] = None,
         columns_button: bool = True,
         filters: bool = True,
         export_to_csv: bool = True,
         search: bool = True,
         page_size: int = 10,
         page_size_options: Optional[list[int]] = None,
+        buttons_column_definition: Optional[
+            shimoku.plt.plt_layer.PlotLayer.TableButtonColumnDefinition
+        ] = None,
         initial_sort_column: Optional[str] = None,
         sort_descending: bool = False,
         columns_options: Optional[dict] = None,
         categorical_columns: Optional[list[str]] = None,
         label_columns: Optional[dict] = None,
         web_link_column: Optional[str] = None,
         open_link_in_new_tab: bool = False,
@@ -1079,20 +1100,20 @@
         :param columns: the columns of the table
         :param columns_button: whether to show the columns button
         :param filters: whether to show the filters button
         :param export_to_csv: whether to show the export to csv button
         :param search: whether to show the search bar
         :param page_size: the number of rows per page
         :param page_size_options: the options for the number of rows per page
+        :param buttons_column_definition: the definition of the buttons column
         :param initial_sort_column: the initial sorting column
         :param sort_descending: whether to sort descending by the initial sorting column
         :param columns_options: the options for the columns
         :param categorical_columns: the categorical columns
         :param label_columns: the label columns
-        :param report_params: additional report parameters as key-value pairs
         :param web_link_column: the column to use as web link
         :param open_link_in_new_tab: whether to open the web link in a new tab
         :param title: the title of the table
         :param padding: the padding of the table
         :param rows_size: the rows size of the table
         :param cols_size: the columns size of the table
         """
```

### Comparing `shimoku-browser-2.3.1/src/shimoku/plt/plt_layer.py` & `shimoku_browser-2.4.0/src/shimoku/plt/plt_layer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,5522 +1,5722 @@
 00000000: 696d 706f 7274 2070 616e 6461 7320 6173  import pandas as
 00000010: 2070 640a 696d 706f 7274 2061 7379 6e63   pd.import async
 00000020: 696f 0a69 6d70 6f72 7420 6e75 6d70 7920  io.import numpy 
-00000030: 6173 206e 700a 0a66 726f 6d20 636f 7079  as np..from copy
-00000040: 2069 6d70 6f72 7420 6465 6570 636f 7079   import deepcopy
-00000050: 0a0a 6672 6f6d 2070 616e 6461 7320 696d  ..from pandas im
-00000060: 706f 7274 2044 6174 6146 7261 6d65 0a66  port DataFrame.f
-00000070: 726f 6d20 6d61 7468 2069 6d70 6f72 7420  rom math import 
-00000080: 6365 696c 0a66 726f 6d20 7368 696d 6f6b  ceil.from shimok
-00000090: 752e 6173 796e 635f 6578 6563 7574 696f  u.async_executio
-000000a0: 6e5f 706f 6f6c 2069 6d70 6f72 7420 280a  n_pool import (.
-000000b0: 2020 2020 4175 746f 4173 796e 6345 7865      AutoAsyncExe
-000000c0: 6375 7469 6f6e 506f 6f6c 2c0a 2020 2020  cutionPool,.    
-000000d0: 6164 645f 746f 5f67 656e 6572 616c 5f61  add_to_general_a
-000000e0: 7379 6e63 5f67 726f 7570 2c0a 290a 0a66  sync_group,.)..f
-000000f0: 726f 6d20 7479 7069 6e67 2069 6d70 6f72  rom typing impor
-00000100: 7420 4f70 7469 6f6e 616c 2c20 556e 696f  t Optional, Unio
-00000110: 6e0a 0a66 726f 6d20 7368 696d 6f6b 752e  n..from shimoku.
-00000120: 7574 696c 7320 696d 706f 7274 2045 7665  utils import Eve
-00000130: 6e74 5479 7065 0a0a 6672 6f6d 2073 6869  ntType..from shi
-00000140: 6d6f 6b75 2e61 7069 2e72 6573 6f75 7263  moku.api.resourc
-00000150: 6573 2e61 7070 2069 6d70 6f72 7420 4170  es.app import Ap
-00000160: 700a 6672 6f6d 2073 6869 6d6f 6b75 2e61  p.from shimoku.a
-00000170: 7069 2e72 6573 6f75 7263 6573 2e62 7573  pi.resources.bus
-00000180: 696e 6573 7320 696d 706f 7274 2042 7573  iness import Bus
-00000190: 696e 6573 730a 6672 6f6d 2073 6869 6d6f  iness.from shimo
-000001a0: 6b75 2e61 7069 2e72 6573 6f75 7263 6573  ku.api.resources
-000001b0: 2e72 6570 6f72 7420 696d 706f 7274 2052  .report import R
-000001c0: 6570 6f72 740a 6672 6f6d 2073 6869 6d6f  eport.from shimo
-000001d0: 6b75 2e61 7069 2e72 6573 6f75 7263 6573  ku.api.resources
-000001e0: 2e64 6174 615f 7365 7420 696d 706f 7274  .data_set import
-000001f0: 2028 0a20 2020 2044 6174 6153 6574 2c0a   (.    DataSet,.
-00000200: 2020 2020 4d61 7070 696e 672c 0a20 2020      Mapping,.   
-00000210: 2063 6f6e 7665 7274 5f69 6e70 7574 5f64   convert_input_d
-00000220: 6174 615f 746f 5f64 625f 6974 656d 732c  ata_to_db_items,
-00000230: 0a20 2020 2063 6f6e 7665 7274 5f64 6174  .    convert_dat
-00000240: 615f 616e 645f 6765 745f 7365 7269 6573  a_and_get_series
-00000250: 5f6e 616d 652c 0a29 0a66 726f 6d20 7368  _name,.).from sh
-00000260: 696d 6f6b 752e 6170 692e 7265 736f 7572  imoku.api.resour
-00000270: 6365 732e 7265 706f 7274 732e 6669 6c74  ces.reports.filt
-00000280: 6572 5f64 6174 615f 7365 7420 696d 706f  er_data_set impo
-00000290: 7274 2046 696c 7465 7244 6174 6153 6574  rt FilterDataSet
-000002a0: 0a66 726f 6d20 7368 696d 6f6b 752e 6170  .from shimoku.ap
-000002b0: 692e 7265 736f 7572 6365 732e 7265 706f  i.resources.repo
-000002c0: 7274 732e 7461 6273 5f67 726f 7570 2069  rts.tabs_group i
-000002d0: 6d70 6f72 7420 5461 6273 4772 6f75 700a  mport TabsGroup.
-000002e0: 6672 6f6d 2073 6869 6d6f 6b75 2e61 7069  from shimoku.api
-000002f0: 2e72 6573 6f75 7263 6573 2e72 6570 6f72  .resources.repor
-00000300: 7473 2e6d 6f64 616c 2069 6d70 6f72 7420  ts.modal import 
-00000310: 4d6f 6461 6c0a 6672 6f6d 2073 6869 6d6f  Modal.from shimo
-00000320: 6b75 2e61 7069 2e72 6573 6f75 7263 6573  ku.api.resources
-00000330: 2e72 6570 6f72 7473 2e63 6861 7274 732e  .reports.charts.
-00000340: 696e 6469 6361 746f 7220 696d 706f 7274  indicator import
-00000350: 2049 6e64 6963 6174 6f72 0a66 726f 6d20   Indicator.from 
-00000360: 7368 696d 6f6b 752e 6170 692e 7265 736f  shimoku.api.reso
-00000370: 7572 6365 732e 7265 706f 7274 732e 6368  urces.reports.ch
-00000380: 6172 7473 2e65 6368 6172 7420 696d 706f  arts.echart impo
-00000390: 7274 2045 4368 6172 740a 6672 6f6d 2073  rt EChart.from s
-000003a0: 6869 6d6f 6b75 2e61 7069 2e72 6573 6f75  himoku.api.resou
-000003b0: 7263 6573 2e72 6570 6f72 7473 2e63 6861  rces.reports.cha
-000003c0: 7274 732e 7461 626c 6520 696d 706f 7274  rts.table import
-000003d0: 2054 6162 6c65 2c20 696e 7465 7270 7265   Table, interpre
-000003e0: 745f 6c61 6265 6c5f 696e 666f 0a66 726f  t_label_info.fro
-000003f0: 6d20 7368 696d 6f6b 752e 6170 692e 7265  m shimoku.api.re
-00000400: 736f 7572 6365 732e 7265 706f 7274 732e  sources.reports.
-00000410: 6368 6172 7473 2e61 6e6e 6f74 6174 6564  charts.annotated
-00000420: 5f63 6861 7274 2069 6d70 6f72 7420 416e  _chart import An
-00000430: 6e6f 7461 7465 6445 4368 6172 740a 6672  notatedEChart.fr
-00000440: 6f6d 2073 6869 6d6f 6b75 2e61 7069 2e72  om shimoku.api.r
-00000450: 6573 6f75 7263 6573 2e72 6570 6f72 7473  esources.reports
-00000460: 2e63 6861 7274 732e 6874 6d6c 2069 6d70  .charts.html imp
-00000470: 6f72 7420 4854 4d4c 0a66 726f 6d20 7368  ort HTML.from sh
-00000480: 696d 6f6b 752e 6170 692e 7265 736f 7572  imoku.api.resour
-00000490: 6365 732e 7265 706f 7274 732e 6368 6172  ces.reports.char
-000004a0: 7473 2e62 7574 746f 6e20 696d 706f 7274  ts.button import
-000004b0: 2042 7574 746f 6e0a 6672 6f6d 2073 6869   Button.from shi
-000004c0: 6d6f 6b75 2e61 7069 2e72 6573 6f75 7263  moku.api.resourc
-000004d0: 6573 2e72 6570 6f72 7473 2e63 6861 7274  es.reports.chart
-000004e0: 732e 696e 7075 745f 666f 726d 2069 6d70  s.input_form imp
-000004f0: 6f72 7420 496e 7075 7446 6f72 6d0a 6672  ort InputForm.fr
-00000500: 6f6d 2073 6869 6d6f 6b75 2e61 7069 2e72  om shimoku.api.r
-00000510: 6573 6f75 7263 6573 2e72 6570 6f72 7473  esources.reports
-00000520: 2e63 6861 7274 732e 6966 7261 6d65 2069  .charts.iframe i
-00000530: 6d70 6f72 7420 4946 7261 6d65 0a66 726f  mport IFrame.fro
-00000540: 6d20 7368 696d 6f6b 752e 706c 742e 4543  m shimoku.plt.EC
-00000550: 6861 7274 5f64 6566 696e 6974 696f 6e73  hart_definitions
-00000560: 2e6c 696e 6520 696d 706f 7274 2028 0a20  .line import (. 
-00000570: 2020 206c 696e 655f 6368 6172 742c 0a20     line_chart,. 
-00000580: 2020 2061 7265 615f 6368 6172 742c 0a20     area_chart,. 
-00000590: 2020 2073 7461 636b 6564 5f61 7265 615f     stacked_area_
-000005a0: 6368 6172 742c 0a20 2020 2070 7265 6469  chart,.    predi
-000005b0: 6374 6976 655f 6c69 6e65 5f63 6861 7274  ctive_line_chart
-000005c0: 2c0a 2020 2020 6d61 726b 6564 5f6c 696e  ,.    marked_lin
-000005d0: 655f 6368 6172 742c 0a20 2020 2073 6567  e_chart,.    seg
-000005e0: 6d65 6e74 6564 5f61 7265 615f 6368 6172  mented_area_char
-000005f0: 742c 0a20 2020 206c 696e 655f 7769 7468  t,.    line_with
-00000600: 5f63 6f6e 6669 6465 6e63 655f 6172 6561  _confidence_area
-00000610: 5f63 6861 7274 2c0a 2020 2020 7365 676d  _chart,.    segm
-00000620: 656e 7465 645f 6c69 6e65 5f63 6861 7274  ented_line_chart
-00000630: 2c0a 290a 6672 6f6d 2073 6869 6d6f 6b75  ,.).from shimoku
-00000640: 2e70 6c74 2e45 4368 6172 745f 6465 6669  .plt.EChart_defi
-00000650: 6e69 7469 6f6e 732e 6261 7220 696d 706f  nitions.bar impo
-00000660: 7274 2028 0a20 2020 2062 6172 5f63 6861  rt (.    bar_cha
-00000670: 7274 2c0a 2020 2020 7374 6163 6b65 645f  rt,.    stacked_
-00000680: 6261 725f 6368 6172 742c 0a20 2020 2068  bar_chart,.    h
-00000690: 6f72 697a 6f6e 7461 6c5f 6261 725f 6368  orizontal_bar_ch
-000006a0: 6172 742c 0a20 2020 2073 7461 636b 6564  art,.    stacked
-000006b0: 5f68 6f72 697a 6f6e 7461 6c5f 6261 725f  _horizontal_bar_
-000006c0: 6368 6172 742c 0a20 2020 207a 6572 6f5f  chart,.    zero_
-000006d0: 6365 6e74 6572 6564 5f62 6172 5f63 6861  centered_bar_cha
-000006e0: 7274 2c0a 290a 6672 6f6d 2073 6869 6d6f  rt,.).from shimo
-000006f0: 6b75 2e70 6c74 2e45 4368 6172 745f 6465  ku.plt.EChart_de
-00000700: 6669 6e69 7469 6f6e 732e 7363 6174 7465  finitions.scatte
-00000710: 7220 696d 706f 7274 2028 0a20 2020 2073  r import (.    s
-00000720: 6361 7474 6572 5f63 6861 7274 2c0a 2020  catter_chart,.  
-00000730: 2020 7363 6174 7465 725f 7769 7468 5f65    scatter_with_e
-00000740: 6666 6563 745f 6368 6172 742c 0a29 0a66  ffect_chart,.).f
-00000750: 726f 6d20 7368 696d 6f6b 752e 706c 742e  rom shimoku.plt.
-00000760: 4543 6861 7274 5f64 6566 696e 6974 696f  EChart_definitio
-00000770: 6e73 2e66 756e 6e65 6c20 696d 706f 7274  ns.funnel import
-00000780: 2066 756e 6e65 6c5f 6368 6172 740a 6672   funnel_chart.fr
-00000790: 6f6d 2073 6869 6d6f 6b75 2e70 6c74 2e45  om shimoku.plt.E
-000007a0: 4368 6172 745f 6465 6669 6e69 7469 6f6e  Chart_definition
-000007b0: 732e 7472 6565 2069 6d70 6f72 7420 7472  s.tree import tr
-000007c0: 6565 5f63 6861 7274 0a66 726f 6d20 7368  ee_chart.from sh
-000007d0: 696d 6f6b 752e 706c 742e 4543 6861 7274  imoku.plt.EChart
-000007e0: 5f64 6566 696e 6974 696f 6e73 2e72 6164  _definitions.rad
-000007f0: 6172 2069 6d70 6f72 7420 7261 6461 725f  ar import radar_
-00000800: 6368 6172 740a 6672 6f6d 2073 6869 6d6f  chart.from shimo
-00000810: 6b75 2e70 6c74 2e45 4368 6172 745f 6465  ku.plt.EChart_de
-00000820: 6669 6e69 7469 6f6e 732e 7069 6520 696d  finitions.pie im
-00000830: 706f 7274 2070 6965 5f63 6861 7274 2c20  port pie_chart, 
-00000840: 646f 7567 686e 7574 5f63 6861 7274 2c20  doughnut_chart, 
-00000850: 726f 7365 5f63 6861 7274 0a66 726f 6d20  rose_chart.from 
-00000860: 7368 696d 6f6b 752e 706c 742e 4543 6861  shimoku.plt.ECha
-00000870: 7274 5f64 6566 696e 6974 696f 6e73 2e67  rt_definitions.g
-00000880: 6175 6765 2069 6d70 6f72 7420 7370 6565  auge import spee
-00000890: 645f 6761 7567 655f 6368 6172 740a 6672  d_gauge_chart.fr
-000008a0: 6f6d 2073 6869 6d6f 6b75 2e70 6c74 2e45  om shimoku.plt.E
-000008b0: 4368 6172 745f 6465 6669 6e69 7469 6f6e  Chart_definition
-000008c0: 732e 7368 696d 6f6b 755f 6761 7567 6520  s.shimoku_gauge 
-000008d0: 696d 706f 7274 2028 0a20 2020 2073 6869  import (.    shi
-000008e0: 6d6f 6b75 5f67 6175 6765 5f63 6861 7274  moku_gauge_chart
-000008f0: 2c0a 2020 2020 7368 696d 6f6b 755f 6761  ,.    shimoku_ga
-00000900: 7567 6573 5f67 726f 7570 2c0a 290a 6672  uges_group,.).fr
-00000910: 6f6d 2073 6869 6d6f 6b75 2e70 6c74 2e45  om shimoku.plt.E
-00000920: 4368 6172 745f 6465 6669 6e69 7469 6f6e  Chart_definition
-00000930: 732e 7375 6e62 7572 7374 2069 6d70 6f72  s.sunburst impor
-00000940: 7420 7375 6e62 7572 7374 5f63 6861 7274  t sunburst_chart
-00000950: 0a66 726f 6d20 7368 696d 6f6b 752e 706c  .from shimoku.pl
-00000960: 742e 4543 6861 7274 5f64 6566 696e 6974  t.EChart_definit
-00000970: 696f 6e73 2e74 7265 656d 6170 2069 6d70  ions.treemap imp
-00000980: 6f72 7420 7472 6565 6d61 705f 6368 6172  ort treemap_char
-00000990: 740a 6672 6f6d 2073 6869 6d6f 6b75 2e70  t.from shimoku.p
-000009a0: 6c74 2e45 4368 6172 745f 6465 6669 6e69  lt.EChart_defini
-000009b0: 7469 6f6e 732e 7361 6e6b 6579 2069 6d70  tions.sankey imp
-000009c0: 6f72 7420 7361 6e6b 6579 5f63 6861 7274  ort sankey_chart
-000009d0: 0a66 726f 6d20 7368 696d 6f6b 752e 706c  .from shimoku.pl
-000009e0: 742e 4543 6861 7274 5f64 6566 696e 6974  t.EChart_definit
-000009f0: 696f 6e73 2e68 6561 746d 6170 2069 6d70  ions.heatmap imp
-00000a00: 6f72 7420 6865 6174 6d61 705f 6368 6172  ort heatmap_char
-00000a10: 740a 6672 6f6d 2073 6869 6d6f 6b75 2e70  t.from shimoku.p
-00000a20: 6c74 2e45 4368 6172 745f 6465 6669 6e69  lt.EChart_defini
-00000a30: 7469 6f6e 732e 6761 7567 655f 696e 6469  tions.gauge_indi
-00000a40: 6361 746f 7220 696d 706f 7274 2067 6175  cator import gau
-00000a50: 6765 5f69 6e64 6963 6174 6f72 0a66 726f  ge_indicator.fro
-00000a60: 6d20 7368 696d 6f6b 752e 706c 742e 4543  m shimoku.plt.EC
-00000a70: 6861 7274 5f64 6566 696e 6974 696f 6e73  hart_definitions
-00000a80: 2e74 6f70 5f62 6f74 746f 6d20 696d 706f  .top_bottom impo
-00000a90: 7274 2028 0a20 2020 2074 6f70 5f62 6f74  rt (.    top_bot
-00000aa0: 746f 6d5f 6172 6561 5f63 6861 7274 732c  tom_area_charts,
-00000ab0: 0a20 2020 2074 6f70 5f62 6f74 746f 6d5f  .    top_bottom_
-00000ac0: 6c69 6e65 5f63 6861 7274 732c 0a29 0a66  line_charts,.).f
-00000ad0: 726f 6d20 7368 696d 6f6b 752e 706c 742e  rom shimoku.plt.
-00000ae0: 4543 6861 7274 5f64 6566 696e 6974 696f  EChart_definitio
-00000af0: 6e73 2e77 6174 6572 6661 6c6c 2069 6d70  ns.waterfall imp
-00000b00: 6f72 7420 7761 7465 7266 616c 6c5f 6368  ort waterfall_ch
-00000b10: 6172 740a 6672 6f6d 2073 6869 6d6f 6b75  art.from shimoku
-00000b20: 2e70 6c74 2e45 4368 6172 745f 6465 6669  .plt.EChart_defi
-00000b30: 6e69 7469 6f6e 732e 6c69 6e65 5f61 6e64  nitions.line_and
-00000b40: 5f62 6172 2069 6d70 6f72 7420 6c69 6e65  _bar import line
-00000b50: 5f61 6e64 5f62 6172 5f63 6861 7274 730a  _and_bar_charts.
-00000b60: 6672 6f6d 2073 6869 6d6f 6b75 2e70 6c74  from shimoku.plt
-00000b70: 2e62 656e 746f 626f 785f 6368 6172 7473  .bentobox_charts
-00000b80: 2069 6d70 6f72 7420 280a 2020 2020 6368   import (.    ch
-00000b90: 6172 745f 616e 645f 6d6f 6461 6c5f 6275  art_and_modal_bu
-00000ba0: 7474 6f6e 2c0a 2020 2020 696e 666f 6772  tton,.    infogr
-00000bb0: 6170 6869 6373 5f74 6578 745f 6275 6262  aphics_text_bubb
-00000bc0: 6c65 2c0a 2020 2020 696e 6469 6361 746f  le,.    indicato
-00000bd0: 7273 5f77 6974 685f 6865 6164 6572 2c0a  rs_with_header,.
-00000be0: 2020 2020 6368 6172 745f 616e 645f 696e      chart_and_in
-00000bf0: 6469 6361 746f 7273 2c0a 2020 2020 6c69  dicators,.    li
-00000c00: 6e65 5f77 6974 685f 7375 6d6d 6172 792c  ne_with_summary,
-00000c10: 0a29 0a0a 6672 6f6d 2073 6869 6d6f 6b75  .)..from shimoku
-00000c20: 2e65 7863 6570 7469 6f6e 7320 696d 706f  .exceptions impo
-00000c30: 7274 2054 6162 7345 7272 6f72 2c20 4d6f  rt TabsError, Mo
-00000c40: 6461 6c45 7272 6f72 2c20 4461 7461 4572  dalError, DataEr
-00000c50: 726f 722c 2042 656e 746f 626f 7845 7272  ror, BentoboxErr
-00000c60: 6f72 0a66 726f 6d20 7368 696d 6f6b 752e  or.from shimoku.
-00000c70: 706c 742e 7574 696c 7320 696d 706f 7274  plt.utils import
-00000c80: 2028 0a20 2020 2064 6565 705f 7570 6461   (.    deep_upda
-00000c90: 7465 2c0a 2020 2020 6765 745f 7575 6964  te,.    get_uuid
-00000ca0: 735f 6672 6f6d 5f64 6963 742c 0a20 2020  s_from_dict,.   
-00000cb0: 2067 6574 5f64 6174 615f 7265 6665 7265   get_data_refere
-00000cc0: 6e63 6573 5f66 726f 6d5f 6469 6374 2c0a  nces_from_dict,.
-00000cd0: 2020 2020 7661 6c69 6461 7465 5f64 6174      validate_dat
-00000ce0: 615f 6973 5f70 616e 6461 7261 626c 652c  a_is_pandarable,
-00000cf0: 0a20 2020 2061 6464 5f73 6f72 7469 6e67  .    add_sorting
-00000d00: 5f74 6f5f 6466 2c0a 2020 2020 7472 616e  _to_df,.    tran
-00000d10: 7366 6f72 6d5f 6469 6374 5f6a 735f 746f  sform_dict_js_to
-00000d20: 5f70 792c 0a20 2020 2072 6574 7269 6576  _py,.    retriev
-00000d30: 655f 6461 7461 5f66 726f 6d5f 6f70 7469  e_data_from_opti
-00000d40: 6f6e 732c 0a20 2020 2076 616c 6964 6174  ons,.    validat
-00000d50: 655f 696e 7075 745f 666f 726d 5f64 6174  e_input_form_dat
-00000d60: 612c 0a20 2020 2063 7265 6174 655f 6e6f  a,.    create_no
-00000d70: 726d 616c 697a 6564 5f6e 616d 652c 0a29  rmalized_name,.)
-00000d80: 0a0a 696d 706f 7274 206c 6f67 6769 6e67  ..import logging
-00000d90: 0a66 726f 6d20 7368 696d 6f6b 752e 6578  .from shimoku.ex
-00000da0: 6563 7574 696f 6e5f 6c6f 6767 6572 2069  ecution_logger i
-00000db0: 6d70 6f72 7420 6c6f 675f 6572 726f 722c  mport log_error,
-00000dc0: 2043 6c61 7373 5769 7468 4c6f 6767 696e   ClassWithLoggin
-00000dd0: 670a 0a6c 6f67 6765 7220 3d20 6c6f 6767  g..logger = logg
-00000de0: 696e 672e 6765 744c 6f67 6765 7228 5f5f  ing.getLogger(__
-00000df0: 6e61 6d65 5f5f 290a 0a0a 636c 6173 7320  name__)...class 
-00000e00: 506c 6f74 4c61 7965 7228 436c 6173 7357  PlotLayer(ClassW
-00000e10: 6974 684c 6f67 6769 6e67 293a 0a20 2020  ithLogging):.   
-00000e20: 2022 2222 0a20 2020 2054 6869 7320 636c   """.    This cl
-00000e30: 6173 7320 6973 2061 2068 6967 6820 6c65  ass is a high le
-00000e40: 7665 6c20 6162 7374 7261 6374 696f 6e20  vel abstraction 
-00000e50: 6f66 2074 6865 2041 5049 2c20 6974 2069  of the API, it i
-00000e60: 7320 7573 6564 2074 6f20 6372 6561 7465  s used to create
-00000e70: 2063 6f6d 706f 6e65 6e74 7320 616e 6420   components and 
-00000e80: 6461 7461 2073 6574 7320 6561 7369 6c79  data sets easily
-00000e90: 2e0a 2020 2020 2222 220a 0a20 2020 205f  ..    """..    _
-00000ea0: 6d6f 6475 6c65 5f6c 6f67 6765 7220 3d20  module_logger = 
-00000eb0: 6c6f 6767 6572 0a20 2020 205f 7573 655f  logger.    _use_
-00000ec0: 696e 666f 5f6c 6f67 6769 6e67 203d 2054  info_logging = T
-00000ed0: 7275 650a 0a20 2020 2064 6566 205f 5f69  rue..    def __i
-00000ee0: 6e69 745f 5f28 0a20 2020 2020 2020 2073  nit__(.        s
-00000ef0: 656c 662c 0a20 2020 2020 2020 2061 7379  elf,.        asy
-00000f00: 6e63 5f70 6f6f 6c3a 2041 7574 6f41 7379  nc_pool: AutoAsy
-00000f10: 6e63 4578 6563 7574 696f 6e50 6f6f 6c2c  ncExecutionPool,
-00000f20: 0a20 2020 2020 2020 2061 7070 3a20 4f70  .        app: Op
-00000f30: 7469 6f6e 616c 5b41 7070 5d2c 0a20 2020  tional[App],.   
-00000f40: 2020 2020 2072 6575 7365 5f64 6174 615f       reuse_data_
-00000f50: 7365 7473 3a20 626f 6f6c 203d 2046 616c  sets: bool = Fal
-00000f60: 7365 2c0a 2020 2020 293a 0a20 2020 2020  se,.    ):.     
-00000f70: 2020 2073 656c 662e 5f61 7070 203d 2061     self._app = a
-00000f80: 7070 0a20 2020 2020 2020 2073 656c 662e  pp.        self.
-00000f90: 5f62 7573 696e 6573 733a 2042 7573 696e  _business: Busin
-00000fa0: 6573 7320 3d20 6170 702e 7061 7265 6e74  ess = app.parent
-00000fb0: 2069 6620 6170 7020 656c 7365 204e 6f6e   if app else Non
-00000fc0: 650a 2020 2020 2020 2020 7365 6c66 2e5f  e.        self._
-00000fd0: 6375 7272 656e 745f 7061 7468 3a20 4f70  current_path: Op
-00000fe0: 7469 6f6e 616c 5b73 7472 5d20 3d20 4e6f  tional[str] = No
-00000ff0: 6e65 0a20 2020 2020 2020 2073 656c 662e  ne.        self.
-00001000: 5f63 7572 7265 6e74 5f74 6162 735f 6772  _current_tabs_gr
-00001010: 6f75 703a 204f 7074 696f 6e61 6c5b 5461  oup: Optional[Ta
-00001020: 6273 4772 6f75 705d 203d 204e 6f6e 650a  bsGroup] = None.
-00001030: 2020 2020 2020 2020 7365 6c66 2e5f 6375          self._cu
-00001040: 7272 656e 745f 7461 623a 204f 7074 696f  rrent_tab: Optio
-00001050: 6e61 6c5b 7374 725d 203d 204e 6f6e 650a  nal[str] = None.
-00001060: 2020 2020 2020 2020 7365 6c66 2e5f 6375          self._cu
-00001070: 7272 656e 745f 6d6f 6461 6c3a 204f 7074  rrent_modal: Opt
-00001080: 696f 6e61 6c5b 4d6f 6461 6c5d 203d 204e  ional[Modal] = N
-00001090: 6f6e 650a 2020 2020 2020 2020 7365 6c66  one.        self
-000010a0: 2e5f 6265 6e74 6f62 6f78 5f64 6174 613a  ._bentobox_data:
-000010b0: 2064 6963 7420 3d20 7b7d 0a20 2020 2020   dict = {}.     
-000010c0: 2020 2073 656c 662e 7265 7573 655f 6461     self.reuse_da
-000010d0: 7461 5f73 6574 733a 2062 6f6f 6c20 3d20  ta_sets: bool = 
-000010e0: 7265 7573 655f 6461 7461 5f73 6574 730a  reuse_data_sets.
-000010f0: 2020 2020 2020 2020 7365 6c66 2e5f 6465          self._de
-00001100: 6c65 7465 5f64 6174 615f 7365 745f 6c6f  lete_data_set_lo
-00001110: 636b 203d 204e 6f6e 650a 2020 2020 2020  ck = None.      
-00001120: 2020 7365 6c66 2e5f 7368 6172 6564 5f64    self._shared_d
-00001130: 6174 615f 6d61 703a 2064 6963 745b 7374  ata_map: dict[st
-00001140: 722c 2064 6963 745b 7374 722c 2074 7570  r, dict[str, tup
-00001150: 6c65 5b4d 6170 7069 6e67 2c20 4461 7461  le[Mapping, Data
-00001160: 5365 742c 2064 6963 745d 5d5d 203d 207b  Set, dict]]] = {
-00001170: 7d0a 2020 2020 2020 2020 7365 6c66 2e5f  }.        self._
-00001180: 7368 6172 6564 5f64 6174 613a 2064 6963  shared_data: dic
-00001190: 745b 7374 722c 2061 6e79 5d20 3d20 7b7d  t[str, any] = {}
-000011a0: 0a20 2020 2020 2020 2073 656c 662e 5f65  .        self._e
-000011b0: 7865 6375 7469 6f6e 5f70 6174 685f 6f72  xecution_path_or
-000011c0: 6465 7273 3a20 6c69 7374 5b73 7472 5d20  ders: list[str] 
-000011d0: 3d20 5b5d 0a20 2020 2020 2020 2073 656c  = [].        sel
-000011e0: 662e 5f61 7379 6e63 5f70 6f6f 6c20 3d20  f._async_pool = 
-000011f0: 6173 796e 635f 706f 6f6c 0a0a 2020 2020  async_pool..    
-00001200: 6173 796e 6320 6465 6620 5f63 7265 6174  async def _creat
-00001210: 655f 6576 656e 7428 0a20 2020 2020 2020  e_event(.       
-00001220: 2073 656c 662c 2065 7665 6e74 5f74 7970   self, event_typ
-00001230: 653a 2045 7665 6e74 5479 7065 2c20 636f  e: EventType, co
-00001240: 6e74 656e 743a 2064 6963 742c 2072 6573  ntent: dict, res
-00001250: 6f75 7263 655f 6964 3a20 4f70 7469 6f6e  ource_id: Option
-00001260: 616c 5b73 7472 5d20 3d20 4e6f 6e65 0a20  al[str] = None. 
-00001270: 2020 2029 3a0a 2020 2020 2020 2020 2222     ):.        ""
-00001280: 2243 7265 6174 6520 616e 2065 7665 6e74  "Create an event
-00001290: 2e0a 2020 2020 2020 2020 3a70 6172 616d  ..        :param
-000012a0: 2065 7665 6e74 5f74 7970 653a 2074 6865   event_type: the
-000012b0: 2074 7970 6520 6f66 2074 6865 2065 7665   type of the eve
-000012c0: 6e74 0a20 2020 2020 2020 203a 7061 7261  nt.        :para
-000012d0: 6d20 636f 6e74 656e 743a 2074 6865 2063  m content: the c
-000012e0: 6f6e 7465 6e74 206f 6620 7468 6520 6576  ontent of the ev
-000012f0: 656e 740a 2020 2020 2020 2020 2222 220a  ent.        """.
-00001300: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00001310: 5f61 7070 2e61 7069 5f63 6c69 656e 742e  _app.api_client.
-00001320: 706c 6179 6772 6f75 6e64 3a0a 2020 2020  playground:.    
-00001330: 2020 2020 2020 2020 6177 6169 7420 7365          await se
-00001340: 6c66 2e5f 6275 7369 6e65 7373 2e63 7265  lf._business.cre
-00001350: 6174 655f 6576 656e 7428 6576 656e 745f  ate_event(event_
-00001360: 7479 7065 2c20 636f 6e74 656e 742c 2072  type, content, r
-00001370: 6573 6f75 7263 655f 6964 290a 0a20 2020  esource_id)..   
-00001380: 2064 6566 2063 6c65 6172 5f63 6f6e 7465   def clear_conte
-00001390: 7874 2873 656c 6629 3a0a 2020 2020 2020  xt(self):.      
-000013a0: 2020 6966 2073 656c 662e 5f62 656e 746f    if self._bento
-000013b0: 626f 785f 6461 7461 3a0a 2020 2020 2020  box_data:.      
-000013c0: 2020 2020 2020 7365 6c66 2e5f 6265 6e74        self._bent
-000013d0: 6f62 6f78 5f64 6174 6120 3d20 7b7d 0a20  obox_data = {}. 
-000013e0: 2020 2020 2020 2020 2020 206c 6f67 6765             logge
-000013f0: 722e 696e 666f 2822 506f 7070 6564 206f  r.info("Popped o
-00001400: 7574 206f 6620 6265 6e74 6f62 6f78 2229  ut of bentobox")
-00001410: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-00001420: 2e5f 6375 7272 656e 745f 7461 6273 5f67  ._current_tabs_g
-00001430: 726f 7570 3a0a 2020 2020 2020 2020 2020  roup:.          
-00001440: 2020 7365 6c66 2e5f 6375 7272 656e 745f    self._current_
-00001450: 7461 6273 5f67 726f 7570 203d 204e 6f6e  tabs_group = Non
-00001460: 650a 2020 2020 2020 2020 2020 2020 7365  e.            se
-00001470: 6c66 2e5f 6375 7272 656e 745f 7461 6220  lf._current_tab 
-00001480: 3d20 4e6f 6e65 0a20 2020 2020 2020 2020  = None.         
-00001490: 2020 206c 6f67 6765 722e 696e 666f 2822     logger.info("
-000014a0: 506f 7070 6564 206f 7574 206f 6620 7461  Popped out of ta
-000014b0: 6273 2067 726f 7570 2229 0a20 2020 2020  bs group").     
-000014c0: 2020 2069 6620 7365 6c66 2e5f 6375 7272     if self._curr
-000014d0: 656e 745f 6d6f 6461 6c3a 0a20 2020 2020  ent_modal:.     
-000014e0: 2020 2020 2020 2073 656c 662e 5f63 7572         self._cur
-000014f0: 7265 6e74 5f6d 6f64 616c 203d 204e 6f6e  rent_modal = Non
-00001500: 650a 2020 2020 2020 2020 2020 2020 6c6f  e.            lo
-00001510: 6767 6572 2e69 6e66 6f28 2250 6f70 7065  gger.info("Poppe
-00001520: 6420 6f75 7420 6f66 206d 6f64 616c 2229  d out of modal")
-00001530: 0a0a 2020 2020 6465 6620 5f63 6865 636b  ..    def _check
-00001540: 5f66 6f72 5f63 6f6e 666c 6963 7473 2873  _for_conflicts(s
-00001550: 656c 662c 2061 7379 6e63 5f70 6f6f 6c3a  elf, async_pool:
-00001560: 2041 7574 6f41 7379 6e63 4578 6563 7574   AutoAsyncExecut
-00001570: 696f 6e50 6f6f 6c2c 206f 7264 6572 3a20  ionPool, order: 
-00001580: 696e 7429 3a0a 2020 2020 2020 2020 2222  int):.        ""
-00001590: 220a 2020 2020 2020 2020 4368 6563 6b20  ".        Check 
-000015a0: 6966 2074 6865 7265 2061 7265 2063 6861  if there are cha
-000015b0: 7274 7320 7769 7468 2074 6865 2073 616d  rts with the sam
-000015c0: 6520 6f72 6465 722e 0a20 2020 2020 2020  e order..       
-000015d0: 203a 7061 7261 6d20 6f72 6465 723a 2074   :param order: t
-000015e0: 6865 206f 7264 6572 206f 6620 7468 6520  he order of the 
-000015f0: 6368 6172 740a 2020 2020 2020 2020 2222  chart.        ""
-00001600: 220a 2020 2020 2020 2020 725f 6861 7368  ".        r_hash
-00001610: 203d 2073 656c 662e 5f67 6574 5f63 6861   = self._get_cha
-00001620: 7274 5f68 6173 6828 6f72 6465 7229 0a20  rt_hash(order). 
-00001630: 2020 2020 2020 2066 7265 655f 636f 6e74         free_cont
-00001640: 6578 743a 2064 6963 7420 3d20 6173 796e  ext: dict = asyn
-00001650: 635f 706f 6f6c 2e66 7265 655f 636f 6e74  c_pool.free_cont
-00001660: 6578 740a 2020 2020 2020 2020 6966 2022  ext.        if "
-00001670: 6c69 7374 5f66 6f72 5f63 6f6e 666c 6963  list_for_conflic
-00001680: 7473 2220 6e6f 7420 696e 2066 7265 655f  ts" not in free_
-00001690: 636f 6e74 6578 743a 0a20 2020 2020 2020  context:.       
-000016a0: 2020 2020 2066 7265 655f 636f 6e74 6578       free_contex
-000016b0: 745b 226c 6973 745f 666f 725f 636f 6e66  t["list_for_conf
-000016c0: 6c69 6374 7322 5d20 3d20 5b5d 0a0a 2020  licts"] = []..  
-000016d0: 2020 2020 2020 6966 2072 5f68 6173 6820        if r_hash 
-000016e0: 696e 2066 7265 655f 636f 6e74 6578 745b  in free_context[
-000016f0: 226c 6973 745f 666f 725f 636f 6e66 6c69  "list_for_confli
-00001700: 6374 7322 5d3a 0a20 2020 2020 2020 2020  cts"]:.         
-00001710: 2020 2061 7379 6e63 5f70 6f6f 6c2e 636c     async_pool.cl
-00001720: 6561 7228 290a 2020 2020 2020 2020 2020  ear().          
-00001730: 2020 7365 6c66 2e63 6c65 6172 5f63 6f6e    self.clear_con
-00001740: 7465 7874 2829 0a20 2020 2020 2020 2020  text().         
-00001750: 2020 206c 6f67 5f65 7272 6f72 280a 2020     log_error(.  
-00001760: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
-00001770: 6767 6572 2c0a 2020 2020 2020 2020 2020  gger,.          
-00001780: 2020 2020 2020 2243 6861 7274 206f 7264        "Chart ord
-00001790: 6572 2063 6f6c 6c69 7369 6f6e 2c20 7477  er collision, tw
-000017a0: 6f20 6368 6172 7473 2077 6974 6820 7468  o charts with th
-000017b0: 6520 7361 6d65 206f 7264 6572 2063 616e  e same order can
-000017c0: 206e 6f74 2062 6520 6578 6563 7574 6564   not be executed
-000017d0: 2022 0a20 2020 2020 2020 2020 2020 2020   ".             
-000017e0: 2020 2022 6174 2074 6865 2073 616d 6520     "at the same 
-000017f0: 7469 6d65 222c 0a20 2020 2020 2020 2020  time",.         
-00001800: 2020 2020 2020 2052 756e 7469 6d65 4572         RuntimeEr
-00001810: 726f 722c 0a20 2020 2020 2020 2020 2020  ror,.           
-00001820: 2029 0a0a 2020 2020 2020 2020 6672 6565   )..        free
-00001830: 5f63 6f6e 7465 7874 5b22 6c69 7374 5f66  _context["list_f
-00001840: 6f72 5f63 6f6e 666c 6963 7473 225d 2e61  or_conflicts"].a
-00001850: 7070 656e 6428 725f 6861 7368 290a 0a20  ppend(r_hash).. 
-00001860: 2020 2064 6566 205f 6368 6563 6b5f 6265     def _check_be
-00001870: 666f 7265 5f61 7379 6e63 5f65 7865 6375  fore_async_execu
-00001880: 7469 6f6e 280a 2020 2020 2020 2020 7365  tion(.        se
-00001890: 6c66 2c20 6173 796e 635f 706f 6f6c 3a20  lf, async_pool: 
-000018a0: 4175 746f 4173 796e 6345 7865 6375 7469  AutoAsyncExecuti
-000018b0: 6f6e 506f 6f6c 2c20 6675 6e63 3a20 6361  onPool, func: ca
-000018c0: 6c6c 6162 6c65 2c20 2a61 7267 732c 202a  llable, *args, *
-000018d0: 2a6b 7761 7267 730a 2020 2020 293a 0a20  *kwargs.    ):. 
-000018e0: 2020 2020 2020 2022 2222 4368 6563 6b20         """Check 
-000018f0: 6576 6572 7974 6869 6e67 2069 7320 636f  everything is co
-00001900: 7272 6563 7420 6265 666f 7265 2065 7865  rrect before exe
-00001910: 6375 7469 6e67 2074 6865 2074 6173 6b20  cuting the task 
-00001920: 706f 6f6c 2222 220a 2020 2020 2020 2020  pool""".        
-00001930: 6966 2022 6f72 6465 7222 2069 6e20 6b77  if "order" in kw
-00001940: 6172 6773 3a0a 2020 2020 2020 2020 2020  args:.          
-00001950: 2020 7365 6c66 2e5f 6368 6563 6b5f 666f    self._check_fo
-00001960: 725f 636f 6e66 6c69 6374 7328 6173 796e  r_conflicts(asyn
-00001970: 635f 706f 6f6c 2c20 6b77 6172 6773 5b22  c_pool, kwargs["
-00001980: 6f72 6465 7222 5d29 0a0a 2020 2020 6465  order"])..    de
-00001990: 6620 7261 6973 655f 6966 5f63 616e 745f  f raise_if_cant_
-000019a0: 6368 616e 6765 5f70 6174 6828 7365 6c66  change_path(self
-000019b0: 293a 0a20 2020 2020 2020 2022 2222 5261  ):.        """Ra
-000019c0: 6973 6520 616e 2065 7272 6f72 2069 6620  ise an error if 
-000019d0: 6120 7461 6273 2067 726f 7570 206f 7220  a tabs group or 
-000019e0: 6120 6d6f 6461 6c20 6973 2061 6c72 6561  a modal is alrea
-000019f0: 6479 206f 7065 6e2e 2222 220a 2020 2020  dy open.""".    
-00001a00: 2020 2020 6966 2073 656c 662e 5f63 7572      if self._cur
-00001a10: 7265 6e74 5f74 6162 735f 6772 6f75 703a  rent_tabs_group:
-00001a20: 0a20 2020 2020 2020 2020 2020 206c 6f67  .            log
-00001a30: 5f65 7272 6f72 280a 2020 2020 2020 2020  _error(.        
-00001a40: 2020 2020 2020 2020 6c6f 6767 6572 2c20          logger, 
-00001a50: 2243 616e 6e6f 7420 6368 616e 6765 2070  "Cannot change p
-00001a60: 6174 6820 7768 696c 6520 6120 7461 6273  ath while a tabs
-00001a70: 2067 726f 7570 2069 7320 6f70 656e 222c   group is open",
-00001a80: 2054 6162 7345 7272 6f72 0a20 2020 2020   TabsError.     
-00001a90: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-00001aa0: 2069 6620 7365 6c66 2e5f 6375 7272 656e   if self._curren
-00001ab0: 745f 6d6f 6461 6c3a 0a20 2020 2020 2020  t_modal:.       
-00001ac0: 2020 2020 206c 6f67 5f65 7272 6f72 286c       log_error(l
-00001ad0: 6f67 6765 722c 2022 4361 6e6e 6f74 2063  ogger, "Cannot c
-00001ae0: 6861 6e67 6520 7061 7468 2077 6869 6c65  hange path while
-00001af0: 2061 206d 6f64 616c 2069 7320 6f70 656e   a modal is open
-00001b00: 222c 204d 6f64 616c 4572 726f 7229 0a20  ", ModalError). 
-00001b10: 2020 2020 2020 2069 6620 7365 6c66 2e5f         if self._
-00001b20: 6265 6e74 6f62 6f78 5f64 6174 613a 0a20  bentobox_data:. 
-00001b30: 2020 2020 2020 2020 2020 206c 6f67 5f65             log_e
-00001b40: 7272 6f72 280a 2020 2020 2020 2020 2020  rror(.          
-00001b50: 2020 2020 2020 6c6f 6767 6572 2c20 2243        logger, "C
-00001b60: 616e 6e6f 7420 6368 616e 6765 2070 6174  annot change pat
-00001b70: 6820 7768 696c 6520 6120 6265 6e74 6f62  h while a bentob
-00001b80: 6f78 2069 7320 6f70 656e 222c 2042 656e  ox is open", Ben
-00001b90: 746f 626f 7845 7272 6f72 0a20 2020 2020  toboxError.     
-00001ba0: 2020 2020 2020 2029 0a0a 2020 2020 6465         )..    de
-00001bb0: 6620 6765 745f 7368 6172 6564 5f64 6174  f get_shared_dat
-00001bc0: 615f 6e61 6d65 7328 7365 6c66 2920 2d3e  a_names(self) ->
-00001bd0: 206c 6973 745b 7374 725d 3a0a 2020 2020   list[str]:.    
-00001be0: 2020 2020 2222 2247 6574 2074 6865 206e      """Get the n
-00001bf0: 616d 6573 206f 6620 7468 6520 7368 6172  ames of the shar
-00001c00: 6564 2064 6174 6122 2222 0a20 2020 2020  ed data""".     
-00001c10: 2020 2072 6574 7572 6e20 6c69 7374 2873     return list(s
-00001c20: 656c 662e 5f73 6861 7265 645f 6461 7461  elf._shared_data
-00001c30: 5f6d 6170 2e6b 6579 7328 2929 0a0a 2020  _map.keys())..  
-00001c40: 2020 6465 6620 6368 616e 6765 5f70 6174    def change_pat
-00001c50: 6828 7365 6c66 2c20 7061 7468 3a20 7374  h(self, path: st
-00001c60: 7229 3a0a 2020 2020 2020 2020 2222 2243  r):.        """C
-00001c70: 6861 6e67 6520 7468 6520 6375 7272 656e  hange the curren
-00001c80: 7420 7061 7468 2222 220a 2020 2020 2020  t path""".      
-00001c90: 2020 7365 6c66 2e72 6169 7365 5f69 665f    self.raise_if_
-00001ca0: 6361 6e74 5f63 6861 6e67 655f 7061 7468  cant_change_path
-00001cb0: 2829 0a20 2020 2020 2020 2073 656c 662e  ().        self.
-00001cc0: 5f63 7572 7265 6e74 5f70 6174 6820 3d20  _current_path = 
-00001cd0: 7061 7468 0a20 2020 2020 2020 2069 6620  path.        if 
-00001ce0: 7061 7468 2061 6e64 2070 6174 6820 6e6f  path and path no
-00001cf0: 7420 696e 2073 656c 662e 5f65 7865 6375  t in self._execu
-00001d00: 7469 6f6e 5f70 6174 685f 6f72 6465 7273  tion_path_orders
-00001d10: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00001d20: 6c66 2e5f 6578 6563 7574 696f 6e5f 7061  lf._execution_pa
-00001d30: 7468 5f6f 7264 6572 732e 6170 7065 6e64  th_orders.append
-00001d40: 2870 6174 6829 0a0a 2020 2020 6465 6620  (path)..    def 
-00001d50: 5f67 6574 5f68 6173 685f 666f 725f 636f  _get_hash_for_co
-00001d60: 6e74 6169 6e65 7228 7365 6c66 2c20 6e61  ntainer(self, na
-00001d70: 6d65 3a20 7374 7229 3a0a 2020 2020 2020  me: str):.      
-00001d80: 2020 2222 2247 6574 2074 6865 2068 6173    """Get the has
-00001d90: 6820 666f 7220 6120 636f 6e74 6169 6e65  h for a containe
-00001da0: 7222 2222 0a20 2020 2020 2020 2072 6574  r""".        ret
-00001db0: 7572 6e20 2866 227b 7365 6c66 2e5f 6375  urn (f"{self._cu
-00001dc0: 7272 656e 745f 7061 7468 7d5f 2220 6966  rrent_path}_" if
-00001dd0: 2073 656c 662e 5f63 7572 7265 6e74 5f70   self._current_p
-00001de0: 6174 6820 656c 7365 2022 2229 202b 206e  ath else "") + n
-00001df0: 616d 650a 0a20 2020 2061 7379 6e63 2064  ame..    async d
-00001e00: 6566 2063 6c65 6172 5f6d 656e 755f 7061  ef clear_menu_pa
-00001e10: 7468 2873 656c 6629 3a0a 2020 2020 2020  th(self):.      
-00001e20: 2020 2222 220a 2020 2020 2020 2020 436c    """.        Cl
-00001e30: 6561 7220 7468 6520 6375 7272 656e 7420  ear the current 
-00001e40: 7061 7468 206f 7220 6120 7375 6270 6174  path or a subpat
-00001e50: 680a 2020 2020 2020 2020 2222 220a 2020  h.        """.  
-00001e60: 2020 2020 2020 7265 706f 7274 7320 3d20        reports = 
-00001e70: 6177 6169 7420 7365 6c66 2e5f 6170 702e  await self._app.
-00001e80: 6765 745f 7265 706f 7274 7328 290a 2020  get_reports().  
-00001e90: 2020 2020 2020 746f 7563 6865 645f 6461        touched_da
-00001ea0: 7461 5f73 6574 5f69 6473 203d 205b 5d0a  ta_set_ids = [].
-00001eb0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00001ec0: 5f63 7572 7265 6e74 5f70 6174 6820 6973  _current_path is
-00001ed0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00001ee0: 2020 2020 2020 2070 6174 6820 3d20 6372         path = cr
-00001ef0: 6561 7465 5f6e 6f72 6d61 6c69 7a65 645f  eate_normalized_
-00001f00: 6e61 6d65 2873 656c 662e 5f63 7572 7265  name(self._curre
-00001f10: 6e74 5f70 6174 6829 0a20 2020 2020 2020  nt_path).       
-00001f20: 2020 2020 2072 6570 6f72 7473 203d 205b       reports = [
-00001f30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001f40: 2072 6570 6f72 740a 2020 2020 2020 2020   report.        
-00001f50: 2020 2020 2020 2020 666f 7220 7265 706f          for repo
-00001f60: 7274 2069 6e20 7265 706f 7274 730a 2020  rt in reports.  
-00001f70: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00001f80: 2072 6570 6f72 745b 2270 6174 6822 5d20   report["path"] 
-00001f90: 616e 6420 6372 6561 7465 5f6e 6f72 6d61  and create_norma
-00001fa0: 6c69 7a65 645f 6e61 6d65 2872 6570 6f72  lized_name(repor
-00001fb0: 745b 2270 6174 6822 5d29 203d 3d20 7061  t["path"]) == pa
-00001fc0: 7468 0a20 2020 2020 2020 2020 2020 205d  th.            ]
-00001fd0: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
-00001fe0: 2020 2020 2020 2020 2020 2074 6f75 6368             touch
-00001ff0: 6564 5f64 6174 615f 7365 745f 6964 7320  ed_data_set_ids 
-00002000: 3d20 5b64 735b 2269 6422 5d20 666f 7220  = [ds["id"] for 
-00002010: 6473 2069 6e20 6177 6169 7420 7365 6c66  ds in await self
-00002020: 2e5f 6170 702e 6765 745f 6461 7461 5f73  ._app.get_data_s
-00002030: 6574 7328 295d 0a0a 2020 2020 2020 2020  ets()]..        
-00002040: 636f 6e74 6169 6e65 7273 3a20 6c69 7374  containers: list
-00002050: 203d 205b 0a20 2020 2020 2020 2020 2020   = [.           
-00002060: 2072 6570 6f72 7420 666f 7220 7265 706f   report for repo
-00002070: 7274 2069 6e20 7265 706f 7274 7320 6966  rt in reports if
-00002080: 2072 6570 6f72 742e 7265 706f 7274 5f74   report.report_t
-00002090: 7970 6520 696e 205b 2254 4142 5322 2c20  ype in ["TABS", 
-000020a0: 224d 4f44 414c 225d 0a20 2020 2020 2020  "MODAL"].       
-000020b0: 205d 0a0a 2020 2020 2020 2020 666f 7220   ]..        for 
-000020c0: 636f 6e74 6169 6e65 7220 696e 2063 6f6e  container in con
-000020d0: 7461 696e 6572 733a 0a20 2020 2020 2020  tainers:.       
-000020e0: 2020 2020 2063 6f6e 7461 696e 6572 2e63       container.c
-000020f0: 6c65 6172 5f63 6f6e 7465 6e74 2829 0a20  lear_content(). 
-00002100: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
-00002110: 7420 7365 6c66 2e5f 6170 702e 6170 695f  t self._app.api_
-00002120: 636c 6965 6e74 2e63 6163 6865 5f65 6e61  client.cache_ena
-00002130: 626c 6564 3a0a 2020 2020 2020 2020 2020  bled:.          
-00002140: 2020 2020 2020 6177 6169 7420 636f 6e74        await cont
-00002150: 6169 6e65 722e 7570 6461 7465 2829 0a0a  ainer.update()..
-00002160: 2020 2020 2020 2020 7264 7320 3d20 6177          rds = aw
-00002170: 6169 7420 6173 796e 6369 6f2e 6761 7468  ait asyncio.gath
-00002180: 6572 280a 2020 2020 2020 2020 2020 2020  er(.            
-00002190: 2a5b 7265 706f 7274 2e67 6574 5f72 6570  *[report.get_rep
-000021a0: 6f72 745f 6461 7461 5f73 6574 7328 2920  ort_data_sets() 
-000021b0: 666f 7220 7265 706f 7274 2069 6e20 7265  for report in re
-000021c0: 706f 7274 735d 0a20 2020 2020 2020 2029  ports].        )
-000021d0: 0a20 2020 2020 2020 2074 6f75 6368 6564  .        touched
-000021e0: 5f64 6174 615f 7365 745f 6964 732e 6578  _data_set_ids.ex
-000021f0: 7465 6e64 285b 7264 5b22 6461 7461 5365  tend([rd["dataSe
-00002200: 7449 6422 5d20 666f 7220 7264 7320 696e  tId"] for rds in
-00002210: 2072 6473 2066 6f72 2072 6420 696e 2072   rds for rd in r
-00002220: 6473 5d29 0a0a 2020 2020 2020 2020 6177  ds])..        aw
-00002230: 6169 7420 6173 796e 6369 6f2e 6761 7468  ait asyncio.gath
-00002240: 6572 280a 2020 2020 2020 2020 2020 2020  er(.            
-00002250: 2a5b 7365 6c66 2e5f 6170 702e 6465 6c65  *[self._app.dele
-00002260: 7465 5f72 6570 6f72 7428 7265 706f 7274  te_report(report
-00002270: 5b22 6964 225d 2920 666f 7220 7265 706f  ["id"]) for repo
-00002280: 7274 2069 6e20 7265 706f 7274 735d 0a20  rt in reports]. 
-00002290: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-000022a0: 206c 6f67 6765 722e 696e 666f 2866 2244   logger.info(f"D
-000022b0: 656c 6574 6564 207b 6c65 6e28 7265 706f  eleted {len(repo
-000022c0: 7274 7329 7d20 636f 6d70 6f6e 656e 7473  rts)} components
-000022d0: 2229 0a20 2020 2020 2020 2061 7761 6974  ").        await
-000022e0: 2073 656c 662e 5f61 7070 2e64 656c 6574   self._app.delet
-000022f0: 655f 756e 7573 6564 5f64 6174 615f 7365  e_unused_data_se
-00002300: 7473 280a 2020 2020 2020 2020 2020 2020  ts(.            
-00002310: 6c6f 673d 5472 7565 2c20 6461 7461 5f73  log=True, data_s
-00002320: 6574 5f69 6473 3d74 6f75 6368 6564 5f64  et_ids=touched_d
-00002330: 6174 615f 7365 745f 6964 730a 2020 2020  ata_set_ids.    
-00002340: 2020 2020 290a 0a20 2020 2061 7379 6e63      )..    async
-00002350: 2064 6566 2064 656c 6574 655f 6368 6172   def delete_char
-00002360: 745f 6279 5f6f 7264 6572 2873 656c 662c  t_by_order(self,
-00002370: 206f 7264 6572 3a20 696e 7429 3a0a 2020   order: int):.  
-00002380: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00002390: 2020 4465 6c65 7465 2061 2072 6570 6f72    Delete a repor
-000023a0: 7420 6279 206f 7264 6572 2061 6e64 2063  t by order and c
-000023b0: 6f6e 7465 7874 0a20 2020 2020 2020 2022  ontext.        "
-000023c0: 2222 0a20 2020 2020 2020 2072 5f68 6173  "".        r_has
-000023d0: 682c 2072 6570 6f72 7420 3d20 6177 6169  h, report = awai
-000023e0: 7420 7365 6c66 2e5f 6765 745f 6368 6172  t self._get_char
-000023f0: 745f 7265 706f 7274 280a 2020 2020 2020  t_report(.      
-00002400: 2020 2020 2020 6f72 6465 722c 2054 6162        order, Tab
-00002410: 6c65 2c20 6372 6561 7465 5f69 665f 6e6f  le, create_if_no
-00002420: 745f 6578 6973 7473 3d46 616c 7365 0a20  t_exists=False. 
-00002430: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-00002440: 2069 6620 6e6f 7420 7265 706f 7274 3a0a   if not report:.
-00002450: 2020 2020 2020 2020 2020 2020 6c6f 675f              log_
-00002460: 6572 726f 7228 6c6f 6767 6572 2c20 6622  error(logger, f"
-00002470: 4e6f 2063 6861 7274 2066 6f75 6e64 2077  No chart found w
-00002480: 6974 6820 6f72 6465 7220 7b6f 7264 6572  ith order {order
-00002490: 7d22 2c20 5275 6e74 696d 6545 7272 6f72  }", RuntimeError
-000024a0: 290a 2020 2020 2020 2020 6177 6169 7420  ).        await 
-000024b0: 7365 6c66 2e5f 6170 702e 6465 6c65 7465  self._app.delete
-000024c0: 5f72 6570 6f72 7428 725f 6861 7368 3d72  _report(r_hash=r
-000024d0: 5f68 6173 6829 0a0a 2020 2020 6173 796e  _hash)..    asyn
-000024e0: 6320 6465 6620 6465 6c65 7465 5f74 6162  c def delete_tab
-000024f0: 735f 6772 6f75 7028 7365 6c66 2c20 6e61  s_group(self, na
-00002500: 6d65 3a20 7374 7229 3a0a 2020 2020 2020  me: str):.      
-00002510: 2020 2222 2244 656c 6574 6520 6120 7461    """Delete a ta
-00002520: 6273 2067 726f 7570 2222 220a 2020 2020  bs group""".    
-00002530: 2020 2020 725f 6861 7368 203d 2073 656c      r_hash = sel
-00002540: 662e 5f67 6574 5f68 6173 685f 666f 725f  f._get_hash_for_
-00002550: 636f 6e74 6169 6e65 7228 6e61 6d65 290a  container(name).
-00002560: 2020 2020 2020 2020 7461 6273 5f67 726f          tabs_gro
-00002570: 7570 203d 2061 7761 6974 2073 656c 662e  up = await self.
-00002580: 5f61 7070 2e67 6574 5f72 6570 6f72 7428  _app.get_report(
-00002590: 725f 6861 7368 3d72 5f68 6173 6829 0a20  r_hash=r_hash). 
-000025a0: 2020 2020 2020 2069 6620 6e6f 7420 7461         if not ta
-000025b0: 6273 5f67 726f 7570 3a0a 2020 2020 2020  bs_group:.      
-000025c0: 2020 2020 2020 6c6f 675f 6572 726f 7228        log_error(
-000025d0: 6c6f 6767 6572 2c20 6622 4e6f 2074 6162  logger, f"No tab
-000025e0: 7320 6772 6f75 7020 666f 756e 6420 7769  s group found wi
-000025f0: 7468 206e 616d 6520 7b6e 616d 657d 222c  th name {name}",
-00002600: 2054 6162 7345 7272 6f72 290a 2020 2020   TabsError).    
-00002610: 2020 2020 6177 6169 7420 7365 6c66 2e5f      await self._
-00002620: 6170 702e 6465 6c65 7465 5f72 6570 6f72  app.delete_repor
-00002630: 7428 725f 6861 7368 3d72 5f68 6173 6829  t(r_hash=r_hash)
-00002640: 0a0a 2020 2020 6173 796e 6320 6465 6620  ..    async def 
-00002650: 6465 6c65 7465 5f6d 6f64 616c 2873 656c  delete_modal(sel
-00002660: 662c 206e 616d 653a 2073 7472 293a 0a20  f, name: str):. 
-00002670: 2020 2020 2020 2022 2222 4465 6c65 7465         """Delete
-00002680: 2061 206d 6f64 616c 2222 220a 2020 2020   a modal""".    
-00002690: 2020 2020 725f 6861 7368 203d 2073 656c      r_hash = sel
-000026a0: 662e 5f67 6574 5f68 6173 685f 666f 725f  f._get_hash_for_
-000026b0: 636f 6e74 6169 6e65 7228 6e61 6d65 290a  container(name).
-000026c0: 2020 2020 2020 2020 6d6f 6461 6c20 3d20          modal = 
-000026d0: 6177 6169 7420 7365 6c66 2e5f 6170 702e  await self._app.
-000026e0: 6765 745f 7265 706f 7274 2872 5f68 6173  get_report(r_has
-000026f0: 683d 725f 6861 7368 290a 2020 2020 2020  h=r_hash).      
-00002700: 2020 6966 206e 6f74 206d 6f64 616c 3a0a    if not modal:.
-00002710: 2020 2020 2020 2020 2020 2020 6c6f 675f              log_
-00002720: 6572 726f 7228 6c6f 6767 6572 2c20 6622  error(logger, f"
-00002730: 4e6f 206d 6f64 616c 2066 6f75 6e64 2077  No modal found w
-00002740: 6974 6820 6e61 6d65 207b 6e61 6d65 7d22  ith name {name}"
-00002750: 2c20 4d6f 6461 6c45 7272 6f72 290a 2020  , ModalError).  
-00002760: 2020 2020 2020 6177 6169 7420 7365 6c66        await self
-00002770: 2e5f 6170 702e 6465 6c65 7465 5f72 6570  ._app.delete_rep
-00002780: 6f72 7428 725f 6861 7368 3d72 5f68 6173  ort(r_hash=r_has
-00002790: 6829 0a0a 2020 2020 6465 6620 7365 745f  h)..    def set_
-000027a0: 6265 6e74 6f62 6f78 2873 656c 662c 2063  bentobox(self, c
-000027b0: 6f6c 735f 7369 7a65 3a20 696e 742c 2072  ols_size: int, r
-000027c0: 6f77 735f 7369 7a65 3a20 696e 7429 3a0a  ows_size: int):.
-000027d0: 2020 2020 2020 2020 2222 2253 7461 7274          """Start
-000027e0: 2075 7369 6e67 2061 2062 656e 746f 626f   using a bentobo
-000027f0: 782c 2074 6865 2069 6420 616e 6420 7468  x, the id and th
-00002800: 6520 6f72 6465 7220 7769 6c6c 2062 6520  e order will be 
-00002810: 7365 7420 7768 656e 2074 6865 2062 656e  set when the ben
-00002820: 746f 626f 7820 6973 2075 7365 6420 666f  tobox is used fo
-00002830: 7220 7468 6520 6669 7273 7420 7469 6d65  r the first time
-00002840: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-00002850: 636f 6c73 5f73 697a 653a 2074 6865 206e  cols_size: the n
-00002860: 756d 6265 7220 6f66 2063 6f6c 756d 6e73  umber of columns
-00002870: 2069 6e20 7468 6520 6265 6e74 6f62 6f78   in the bentobox
-00002880: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-00002890: 726f 7773 5f73 697a 653a 2074 6865 206e  rows_size: the n
-000028a0: 756d 6265 7220 6f66 2072 6f77 7320 696e  umber of rows in
-000028b0: 2074 6865 2062 656e 746f 626f 7822 2222   the bentobox"""
-000028c0: 0a20 2020 2020 2020 2073 656c 662e 5f62  .        self._b
-000028d0: 656e 746f 626f 785f 6461 7461 3a20 6469  entobox_data: di
-000028e0: 6374 203d 207b 0a20 2020 2020 2020 2020  ct = {.         
-000028f0: 2020 2022 6265 6e74 6f62 6f78 4964 223a     "bentoboxId":
-00002900: 204e 6f6e 652c 0a20 2020 2020 2020 2020   None,.         
-00002910: 2020 2022 6265 6e74 6f62 6f78 4f72 6465     "bentoboxOrde
-00002920: 7222 3a20 4e6f 6e65 2c0a 2020 2020 2020  r": None,.      
-00002930: 2020 2020 2020 2262 656e 746f 626f 7853        "bentoboxS
-00002940: 697a 6543 6f6c 756d 6e73 223a 2063 6f6c  izeColumns": col
-00002950: 735f 7369 7a65 2c0a 2020 2020 2020 2020  s_size,.        
-00002960: 2020 2020 2262 656e 746f 626f 7853 697a      "bentoboxSiz
-00002970: 6552 6f77 7322 3a20 726f 7773 5f73 697a  eRows": rows_siz
-00002980: 652c 0a20 2020 2020 2020 207d 0a0a 2020  e,.        }..  
-00002990: 2020 6465 6620 706f 705f 6f75 745f 6f66    def pop_out_of
-000029a0: 5f62 656e 746f 626f 7828 7365 6c66 293a  _bentobox(self):
-000029b0: 0a20 2020 2020 2020 2022 2222 5374 6f70  .        """Stop
-000029c0: 2075 7369 6e67 2061 2062 656e 746f 626f   using a bentobo
-000029d0: 7822 2222 0a20 2020 2020 2020 2073 656c  x""".        sel
-000029e0: 662e 5f62 656e 746f 626f 785f 6461 7461  f._bentobox_data
-000029f0: 203d 207b 7d0a 0a20 2020 2064 6566 205f   = {}..    def _
-00002a00: 6765 745f 6265 6e74 6f62 6f78 5f64 6174  get_bentobox_dat
-00002a10: 6128 7365 6c66 2c20 6f72 6465 723a 2069  a(self, order: i
-00002a20: 6e74 2920 2d3e 2064 6963 743a 0a20 2020  nt) -> dict:.   
-00002a30: 2020 2020 2022 2222 4765 7420 7468 6520       """Get the 
-00002a40: 6265 6e74 6f62 6f78 2064 6174 6122 2222  bentobox data"""
-00002a50: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
-00002a60: 7365 6c66 2e5f 6265 6e74 6f62 6f78 5f64  self._bentobox_d
-00002a70: 6174 613a 0a20 2020 2020 2020 2020 2020  ata:.           
-00002a80: 2072 6574 7572 6e20 7b7d 0a20 2020 2020   return {}.     
-00002a90: 2020 2069 6620 6e6f 7420 7365 6c66 2e5f     if not self._
-00002aa0: 6265 6e74 6f62 6f78 5f64 6174 615b 2262  bentobox_data["b
-00002ab0: 656e 746f 626f 7849 6422 5d3a 0a20 2020  entoboxId"]:.   
-00002ac0: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
-00002ad0: 7365 6c66 2e5f 6265 6e74 6f62 6f78 5f64  self._bentobox_d
-00002ae0: 6174 615b 2262 656e 746f 626f 7849 6422  ata["bentoboxId"
-00002af0: 5d3a 0a20 2020 2020 2020 2020 2020 2020  ]:.             
-00002b00: 2020 2073 656c 662e 5f62 656e 746f 626f     self._bentobo
-00002b10: 785f 6461 7461 2e75 7064 6174 6528 0a20  x_data.update(. 
-00002b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002b30: 2020 207b 0a20 2020 2020 2020 2020 2020     {.           
-00002b40: 2020 2020 2020 2020 2020 2020 2022 6265               "be
-00002b50: 6e74 6f62 6f78 4964 223a 2022 5f22 202b  ntoboxId": "_" +
-00002b60: 2073 7472 286f 7264 6572 292c 0a20 2020   str(order),.   
-00002b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002b80: 2020 2020 2022 6265 6e74 6f62 6f78 4f72       "bentoboxOr
-00002b90: 6465 7222 3a20 6f72 6465 722c 0a20 2020  der": order,.   
-00002ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002bb0: 207d 0a20 2020 2020 2020 2020 2020 2020   }.             
-00002bc0: 2020 2029 0a20 2020 2020 2020 2072 6574     ).        ret
-00002bd0: 7572 6e20 7365 6c66 2e5f 6265 6e74 6f62  urn self._bentob
-00002be0: 6f78 5f64 6174 610a 0a20 2020 2061 7379  ox_data..    asy
-00002bf0: 6e63 2064 6566 205f 7570 6461 7465 5f63  nc def _update_c
-00002c00: 6f6e 7461 696e 6572 7328 7365 6c66 293a  ontainers(self):
-00002c10: 0a20 2020 2020 2020 2022 2222 5570 6461  .        """Upda
-00002c20: 7465 2074 6865 2072 6570 6f72 7473 2074  te the reports t
-00002c30: 6861 7420 6163 7420 6173 2063 6f6e 7461  hat act as conta
-00002c40: 696e 6572 7322 2222 0a20 2020 2020 2020  iners""".       
-00002c50: 2072 6570 6f72 7473 203d 2061 7761 6974   reports = await
-00002c60: 2073 656c 662e 5f61 7070 2e67 6574 5f72   self._app.get_r
-00002c70: 6570 6f72 7473 2829 0a20 2020 2020 2020  eports().       
-00002c80: 2063 6f6e 7461 696e 6572 733a 206c 6973   containers: lis
-00002c90: 745b 5265 706f 7274 5d20 3d20 5b0a 2020  t[Report] = [.  
-00002ca0: 2020 2020 2020 2020 2020 7265 706f 7274            report
-00002cb0: 2066 6f72 2072 6570 6f72 7420 696e 2072   for report in r
-00002cc0: 6570 6f72 7473 2069 6620 7265 706f 7274  eports if report
-00002cd0: 2e72 6570 6f72 745f 7479 7065 2069 6e20  .report_type in 
-00002ce0: 5b22 5441 4253 222c 2022 4d4f 4441 4c22  ["TABS", "MODAL"
-00002cf0: 5d0a 2020 2020 2020 2020 5d0a 2020 2020  ].        ].    
-00002d00: 2020 2020 6177 6169 7420 6173 796e 6369      await asynci
-00002d10: 6f2e 6761 7468 6572 282a 5b63 6f6e 7461  o.gather(*[conta
-00002d20: 696e 6572 2e75 7064 6174 6528 2920 666f  iner.update() fo
-00002d30: 7220 636f 6e74 6169 6e65 7220 696e 2063  r container in c
-00002d40: 6f6e 7461 696e 6572 735d 290a 2020 2020  ontainers]).    
-00002d50: 2020 2020 6c6f 6767 6572 2e69 6e66 6f28      logger.info(
-00002d60: 2255 7064 6174 6564 2074 6162 2067 726f  "Updated tab gro
-00002d70: 7570 7320 616e 6420 6d6f 6461 6c73 2229  ups and modals")
-00002d80: 0a0a 2020 2020 6173 796e 6320 6465 6620  ..    async def 
-00002d90: 7365 745f 7461 6273 5f69 6e64 6578 280a  set_tabs_index(.
-00002da0: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
-00002db0: 2020 2020 2020 7461 6273 5f69 6e64 6578        tabs_index
-00002dc0: 3a20 7475 706c 655b 7374 722c 2073 7472  : tuple[str, str
-00002dd0: 5d2c 0a20 2020 2020 2020 206f 7264 6572  ],.        order
-00002de0: 3a20 4f70 7469 6f6e 616c 5b69 6e74 5d20  : Optional[int] 
-00002df0: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-00002e00: 7061 7265 6e74 5f74 6162 735f 696e 6465  parent_tabs_inde
-00002e10: 783a 204f 7074 696f 6e61 6c5b 7475 706c  x: Optional[tupl
-00002e20: 655b 7374 722c 2073 7472 5d5d 203d 204e  e[str, str]] = N
-00002e30: 6f6e 652c 0a20 2020 2020 2020 2070 6164  one,.        pad
-00002e40: 6469 6e67 3a20 4f70 7469 6f6e 616c 5b73  ding: Optional[s
-00002e50: 7472 5d20 3d20 4e6f 6e65 2c0a 2020 2020  tr] = None,.    
-00002e60: 2020 2020 636f 6c73 5f73 697a 653a 204f      cols_size: O
-00002e70: 7074 696f 6e61 6c5b 696e 745d 203d 204e  ptional[int] = N
-00002e80: 6f6e 652c 0a20 2020 2020 2020 2072 6f77  one,.        row
-00002e90: 735f 7369 7a65 3a20 4f70 7469 6f6e 616c  s_size: Optional
-00002ea0: 5b69 6e74 5d20 3d20 4e6f 6e65 2c0a 2020  [int] = None,.  
-00002eb0: 2020 2020 2020 6a75 7374 5f6c 6162 656c        just_label
-00002ec0: 733a 204f 7074 696f 6e61 6c5b 626f 6f6c  s: Optional[bool
-00002ed0: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
-00002ee0: 2020 7374 6963 6b79 3a20 4f70 7469 6f6e    sticky: Option
-00002ef0: 616c 5b62 6f6f 6c5d 203d 204e 6f6e 652c  al[bool] = None,
-00002f00: 0a20 2020 2029 3a0a 2020 2020 2020 2020  .    ):.        
-00002f10: 2222 2253 6574 2074 6865 2063 7572 7265  """Set the curre
-00002f20: 6e74 2074 6162 7320 696e 6465 782e 0a20  nt tabs index.. 
-00002f30: 2020 2020 2020 203a 7061 7261 6d20 7461         :param ta
-00002f40: 6273 5f69 6e64 6578 3a20 7468 6520 696e  bs_index: the in
-00002f50: 6465 7820 6f66 2074 6865 2074 6162 7320  dex of the tabs 
-00002f60: 6772 6f75 700a 2020 2020 2020 2020 3a70  group.        :p
-00002f70: 6172 616d 206f 7264 6572 3a20 7468 6520  aram order: the 
-00002f80: 6f72 6465 7220 6f66 2074 6865 2074 6162  order of the tab
-00002f90: 7320 6772 6f75 7020 696e 2074 6865 2064  s group in the d
-00002fa0: 6173 6862 6f61 7264 0a20 2020 2020 2020  ashboard.       
-00002fb0: 203a 7061 7261 6d20 7061 7265 6e74 5f74   :param parent_t
-00002fc0: 6162 735f 696e 6465 783a 2074 6865 2069  abs_index: the i
-00002fd0: 6e64 6578 206f 6620 7468 6520 7061 7265  ndex of the pare
-00002fe0: 6e74 2074 6162 7320 6772 6f75 700a 2020  nt tabs group.  
-00002ff0: 2020 2020 2020 3a70 6172 616d 2063 6f6c        :param col
-00003000: 735f 7369 7a65 3a20 7468 6520 7369 7a65  s_size: the size
-00003010: 206f 6620 7468 6520 636f 6c75 6d6e 7320   of the columns 
-00003020: 696e 2074 6865 2074 6162 7320 6772 6f75  in the tabs grou
-00003030: 700a 2020 2020 2020 2020 3a70 6172 616d  p.        :param
-00003040: 2070 6164 6469 6e67 3a20 7468 6520 7061   padding: the pa
-00003050: 6464 696e 6720 6f66 2074 6865 2074 6162  dding of the tab
-00003060: 7320 6772 6f75 700a 2020 2020 2020 2020  s group.        
-00003070: 3a70 6172 616d 2072 6f77 735f 7369 7a65  :param rows_size
-00003080: 3a20 7468 6520 7369 7a65 206f 6620 7468  : the size of th
-00003090: 6520 726f 7773 2069 6e20 7468 6520 7461  e rows in the ta
-000030a0: 6273 2067 726f 7570 0a20 2020 2020 2020  bs group.       
-000030b0: 203a 7061 7261 6d20 6a75 7374 5f6c 6162   :param just_lab
-000030c0: 656c 733a 2077 6865 7468 6572 2074 6f20  els: whether to 
-000030d0: 7368 6f77 206a 7573 7420 7468 6520 6c61  show just the la
-000030e0: 6265 6c73 2069 6e20 7468 6520 7461 6273  bels in the tabs
-000030f0: 2067 726f 7570 0a20 2020 2020 2020 203a   group.        :
-00003100: 7061 7261 6d20 7374 6963 6b79 3a20 7768  param sticky: wh
-00003110: 6574 6865 7220 746f 206d 616b 6520 7468  ether to make th
-00003120: 6520 7461 6273 2067 726f 7570 2073 7469  e tabs group sti
-00003130: 636b 790a 2020 2020 2020 2020 2222 220a  cky.        """.
-00003140: 2020 2020 2020 2020 725f 6861 7368 203d          r_hash =
-00003150: 2073 656c 662e 5f67 6574 5f68 6173 685f   self._get_hash_
-00003160: 666f 725f 636f 6e74 6169 6e65 7228 7461  for_container(ta
-00003170: 6273 5f69 6e64 6578 5b30 5d29 0a20 2020  bs_index[0]).   
-00003180: 2020 2020 2074 6162 735f 6772 6f75 703a       tabs_group:
-00003190: 204f 7074 696f 6e61 6c5b 5461 6273 4772   Optional[TabsGr
-000031a0: 6f75 705d 203d 2061 7761 6974 2073 656c  oup] = await sel
-000031b0: 662e 5f61 7070 2e67 6574 5f72 6570 6f72  f._app.get_repor
-000031c0: 7428 725f 6861 7368 3d72 5f68 6173 6829  t(r_hash=r_hash)
-000031d0: 0a20 2020 2020 2020 2070 6172 616d 7320  .        params 
-000031e0: 3d20 7b22 7072 6f70 6572 7469 6573 223a  = {"properties":
-000031f0: 207b 7d7d 0a20 2020 2020 2020 2069 6620   {}}.        if 
-00003200: 636f 6c73 5f73 697a 653a 0a20 2020 2020  cols_size:.     
-00003210: 2020 2020 2020 2070 6172 616d 735b 2273         params["s
-00003220: 697a 6543 6f6c 756d 6e73 225d 203d 2063  izeColumns"] = c
-00003230: 6f6c 735f 7369 7a65 0a20 2020 2020 2020  ols_size.       
-00003240: 2069 6620 7061 6464 696e 673a 0a20 2020   if padding:.   
-00003250: 2020 2020 2020 2020 2070 6172 616d 735b           params[
-00003260: 2273 697a 6550 6164 6469 6e67 225d 203d  "sizePadding"] =
-00003270: 2070 6164 6469 6e67 0a20 2020 2020 2020   padding.       
-00003280: 2069 6620 726f 7773 5f73 697a 653a 0a20   if rows_size:. 
-00003290: 2020 2020 2020 2020 2020 2070 6172 616d             param
-000032a0: 735b 2273 697a 6552 6f77 7322 5d20 3d20  s["sizeRows"] = 
-000032b0: 726f 7773 5f73 697a 650a 2020 2020 2020  rows_size.      
-000032c0: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
-000032d0: 6a75 7374 5f6c 6162 656c 732c 2062 6f6f  just_labels, boo
-000032e0: 6c29 3a0a 2020 2020 2020 2020 2020 2020  l):.            
-000032f0: 7061 7261 6d73 5b22 7072 6f70 6572 7469  params["properti
-00003300: 6573 225d 5b22 7661 7269 616e 7422 5d20  es"]["variant"] 
-00003310: 3d20 280a 2020 2020 2020 2020 2020 2020  = (.            
-00003320: 2020 2020 2273 6f6c 6964 526f 756e 6465      "solidRounde
-00003330: 6422 2069 6620 6a75 7374 5f6c 6162 656c  d" if just_label
-00003340: 7320 656c 7365 2022 656e 636c 6f73 6564  s else "enclosed
-00003350: 536f 6c69 6452 6f75 6e64 6564 220a 2020  SolidRounded".  
-00003360: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-00003370: 2020 2020 6966 2069 7369 6e73 7461 6e63      if isinstanc
-00003380: 6528 7374 6963 6b79 2c20 626f 6f6c 293a  e(sticky, bool):
-00003390: 0a20 2020 2020 2020 2020 2020 2070 6172  .            par
-000033a0: 616d 735b 2270 726f 7065 7274 6965 7322  ams["properties"
-000033b0: 5d5b 2273 7469 636b 7922 5d20 3d20 7374  ]["sticky"] = st
-000033c0: 6963 6b79 0a20 2020 2020 2020 2062 656e  icky.        ben
-000033d0: 746f 626f 785f 6461 7461 203d 2073 656c  tobox_data = sel
-000033e0: 662e 5f67 6574 5f62 656e 746f 626f 785f  f._get_bentobox_
-000033f0: 6461 7461 286f 7264 6572 290a 2020 2020  data(order).    
-00003400: 2020 2020 6966 2062 656e 746f 626f 785f      if bentobox_
-00003410: 6461 7461 3a0a 2020 2020 2020 2020 2020  data:.          
-00003420: 2020 7061 7261 6d73 5b22 6265 6e74 6f62    params["bentob
-00003430: 6f78 225d 203d 2062 656e 746f 626f 785f  ox"] = bentobox_
-00003440: 6461 7461 0a20 2020 2020 2020 2069 6620  data.        if 
-00003450: 7365 6c66 2e5f 6375 7272 656e 745f 7061  self._current_pa
-00003460: 7468 3a0a 2020 2020 2020 2020 2020 2020  th:.            
-00003470: 7061 7261 6d73 5b22 7061 7468 225d 203d  params["path"] =
-00003480: 2073 656c 662e 5f63 7572 7265 6e74 5f70   self._current_p
-00003490: 6174 680a 0a20 2020 2020 2020 2069 6620  ath..        if 
-000034a0: 6e6f 7420 7461 6273 5f67 726f 7570 3a0a  not tabs_group:.
-000034b0: 2020 2020 2020 2020 2020 2020 6966 206e              if n
-000034c0: 6f74 2069 7369 6e73 7461 6e63 6528 6f72  ot isinstance(or
-000034d0: 6465 722c 2069 6e74 293a 0a20 2020 2020  der, int):.     
-000034e0: 2020 2020 2020 2020 2020 206c 6f67 5f65             log_e
-000034f0: 7272 6f72 280a 2020 2020 2020 2020 2020  rror(.          
-00003500: 2020 2020 2020 2020 2020 6c6f 6767 6572            logger
-00003510: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00003520: 2020 2020 2020 6622 4361 6e6e 6f74 2063        f"Cannot c
-00003530: 7265 6174 6520 7461 6273 2067 726f 7570  reate tabs group
-00003540: 207b 7461 6273 5f69 6e64 6578 5b30 5d7d   {tabs_index[0]}
-00003550: 2077 6974 686f 7574 206f 7264 6572 222c   without order",
-00003560: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003570: 2020 2020 2054 6162 7345 7272 6f72 2c0a       TabsError,.
-00003580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003590: 290a 2020 2020 2020 2020 2020 2020 7461  ).            ta
-000035a0: 6273 5f67 726f 7570 3a20 5461 6273 4772  bs_group: TabsGr
-000035b0: 6f75 7020 3d20 6177 6169 7420 7365 6c66  oup = await self
-000035c0: 2e5f 6170 702e 6372 6561 7465 5f72 6570  ._app.create_rep
-000035d0: 6f72 7428 0a20 2020 2020 2020 2020 2020  ort(.           
-000035e0: 2020 2020 2054 6162 7347 726f 7570 2c20       TabsGroup, 
-000035f0: 725f 6861 7368 3d72 5f68 6173 682c 206f  r_hash=r_hash, o
-00003600: 7264 6572 3d6f 7264 6572 2c20 2a2a 7061  rder=order, **pa
-00003610: 7261 6d73 0a20 2020 2020 2020 2020 2020  rams.           
-00003620: 2029 0a20 2020 2020 2020 2020 2020 206c   ).            l
-00003630: 6f67 6765 722e 696e 666f 280a 2020 2020  ogger.info(.    
-00003640: 2020 2020 2020 2020 2020 2020 6627 4372              f'Cr
-00003650: 6561 7465 6420 7461 6273 2067 726f 7570  eated tabs group
-00003660: 207b 7461 6273 5f69 6e64 6578 5b30 5d7d   {tabs_index[0]}
-00003670: 2077 6974 6820 6964 207b 7461 6273 5f67   with id {tabs_g
-00003680: 726f 7570 5b22 6964 225d 7d27 0a20 2020  roup["id"]}'.   
-00003690: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-000036a0: 2020 2065 6c69 6620 6f72 6465 723a 0a20     elif order:. 
-000036b0: 2020 2020 2020 2020 2020 2061 7761 6974             await
-000036c0: 2073 656c 662e 5f61 7070 2e75 7064 6174   self._app.updat
-000036d0: 655f 7265 706f 7274 2872 5f68 6173 683d  e_report(r_hash=
-000036e0: 725f 6861 7368 2c20 6f72 6465 723d 6f72  r_hash, order=or
-000036f0: 6465 722c 202a 2a70 6172 616d 7329 0a0a  der, **params)..
-00003700: 2020 2020 2020 2020 6966 2070 6172 656e          if paren
-00003710: 745f 7461 6273 5f69 6e64 6578 3a0a 2020  t_tabs_index:.  
-00003720: 2020 2020 2020 2020 2020 705f 6861 7368            p_hash
-00003730: 203d 2073 656c 662e 5f67 6574 5f68 6173   = self._get_has
-00003740: 685f 666f 725f 636f 6e74 6169 6e65 7228  h_for_container(
-00003750: 7061 7265 6e74 5f74 6162 735f 696e 6465  parent_tabs_inde
-00003760: 785b 305d 290a 2020 2020 2020 2020 2020  x[0]).          
-00003770: 2020 7061 7265 6e74 5f74 6162 735f 6772    parent_tabs_gr
-00003780: 6f75 703a 204f 7074 696f 6e61 6c5b 5461  oup: Optional[Ta
-00003790: 6273 4772 6f75 705d 203d 2061 7761 6974  bsGroup] = await
-000037a0: 2073 656c 662e 5f61 7070 2e67 6574 5f72   self._app.get_r
-000037b0: 6570 6f72 7428 0a20 2020 2020 2020 2020  eport(.         
-000037c0: 2020 2020 2020 2072 5f68 6173 683d 705f         r_hash=p_
-000037d0: 6861 7368 0a20 2020 2020 2020 2020 2020  hash.           
-000037e0: 2029 0a20 2020 2020 2020 2020 2020 2069   ).            i
-000037f0: 6620 6e6f 7420 7061 7265 6e74 5f74 6162  f not parent_tab
-00003800: 735f 6772 6f75 703a 0a20 2020 2020 2020  s_group:.       
-00003810: 2020 2020 2020 2020 206c 6f67 5f65 7272           log_err
-00003820: 6f72 280a 2020 2020 2020 2020 2020 2020  or(.            
-00003830: 2020 2020 2020 2020 6c6f 6767 6572 2c0a          logger,.
-00003840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003850: 2020 2020 6622 4e6f 2074 6162 7320 6772      f"No tabs gr
-00003860: 6f75 7020 666f 756e 6420 7769 7468 206e  oup found with n
-00003870: 616d 6520 7b70 6172 656e 745f 7461 6273  ame {parent_tabs
-00003880: 5f69 6e64 6578 5b30 5d7d 222c 0a20 2020  _index[0]}",.   
-00003890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000038a0: 2054 6162 7345 7272 6f72 2c0a 2020 2020   TabsError,.    
-000038b0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-000038c0: 2020 2020 2020 2020 2020 6966 2070 6172            if par
-000038d0: 656e 745f 7461 6273 5f67 726f 7570 5b22  ent_tabs_group["
-000038e0: 6964 225d 203d 3d20 7461 6273 5f67 726f  id"] == tabs_gro
-000038f0: 7570 5b22 6964 225d 3a0a 2020 2020 2020  up["id"]:.      
-00003900: 2020 2020 2020 2020 2020 6c6f 675f 6572            log_er
-00003910: 726f 7228 6c6f 6767 6572 2c20 2243 616e  ror(logger, "Can
-00003920: 6e6f 7420 696e 636c 7564 6520 7461 6273  not include tabs
-00003930: 2067 726f 7570 2069 6e20 6974 7365 6c66   group in itself
-00003940: 222c 2054 6162 7345 7272 6f72 290a 2020  ", TabsError).  
-00003950: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
-00003960: 662e 5f63 7572 7265 6e74 5f6d 6f64 616c  f._current_modal
-00003970: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00003980: 2020 6c6f 675f 6572 726f 7228 0a20 2020    log_error(.   
-00003990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000039a0: 206c 6f67 6765 722c 0a20 2020 2020 2020   logger,.       
-000039b0: 2020 2020 2020 2020 2020 2020 2022 4361               "Ca
-000039c0: 6e6e 6f74 2069 6e63 6c75 6465 2061 2074  nnot include a t
-000039d0: 6162 7320 6772 6f75 7020 696e 2061 206d  abs group in a m
-000039e0: 6f64 616c 2061 6e64 2069 6e20 616e 6f74  odal and in anot
-000039f0: 6865 7220 7461 6273 2067 726f 7570 222c  her tabs group",
-00003a00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003a10: 2020 2020 2054 6162 7345 7272 6f72 2c0a       TabsError,.
-00003a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003a30: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
-00003a40: 206e 6f74 2070 6172 656e 745f 7461 6273   not parent_tabs
-00003a50: 5f67 726f 7570 2e68 6173 5f72 6570 6f72  _group.has_repor
-00003a60: 7428 7461 6273 5f67 726f 7570 293a 0a20  t(tabs_group):. 
-00003a70: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-00003a80: 6172 656e 745f 7461 6273 5f67 726f 7570  arent_tabs_group
-00003a90: 2e61 6464 5f72 6570 6f72 7428 0a20 2020  .add_report(.   
-00003aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003ab0: 2074 6162 3d70 6172 656e 745f 7461 6273   tab=parent_tabs
-00003ac0: 5f69 6e64 6578 5b31 5d2c 2072 6570 6f72  _index[1], repor
-00003ad0: 743d 7461 6273 5f67 726f 7570 0a20 2020  t=tabs_group.   
-00003ae0: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
-00003af0: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-00003b00: 6f67 6765 722e 696e 666f 280a 2020 2020  ogger.info(.    
-00003b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003b20: 6622 496e 636c 7564 6564 2074 6162 7320  f"Included tabs 
-00003b30: 6772 6f75 7020 7b74 6162 735f 696e 6465  group {tabs_inde
-00003b40: 785b 305d 7d20 696e 2074 6162 7320 6772  x[0]} in tabs gr
-00003b50: 6f75 7020 7b70 6172 656e 745f 7461 6273  oup {parent_tabs
-00003b60: 5f69 6e64 6578 5b30 5d7d 220a 2020 2020  _index[0]}".    
-00003b70: 2020 2020 2020 2020 2020 2020 290a 0a20              ).. 
-00003b80: 2020 2020 2020 2065 6c69 6620 7365 6c66         elif self
-00003b90: 2e5f 6375 7272 656e 745f 6d6f 6461 6c20  ._current_modal 
-00003ba0: 616e 6420 6e6f 7420 7365 6c66 2e5f 6375  and not self._cu
-00003bb0: 7272 656e 745f 6d6f 6461 6c2e 6861 735f  rrent_modal.has_
-00003bc0: 7265 706f 7274 2874 6162 735f 6772 6f75  report(tabs_grou
-00003bd0: 7029 3a0a 2020 2020 2020 2020 2020 2020  p):.            
-00003be0: 2861 7761 6974 2073 656c 662e 5f67 6574  (await self._get
-00003bf0: 5f63 7572 7265 6e74 5f6d 6f64 616c 2829  _current_modal()
-00003c00: 292e 6164 645f 7265 706f 7274 2874 6162  ).add_report(tab
-00003c10: 735f 6772 6f75 7029 0a20 2020 2020 2020  s_group).       
-00003c20: 2020 2020 206c 6f67 6765 722e 696e 666f       logger.info
-00003c30: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00003c40: 2020 6622 496e 636c 7564 6564 2074 6162    f"Included tab
-00003c50: 7320 6772 6f75 7020 7b74 6162 735f 696e  s group {tabs_in
-00003c60: 6465 785b 305d 7d20 696e 206d 6f64 616c  dex[0]} in modal
-00003c70: 207b 7374 7228 7365 6c66 2e5f 6375 7272   {str(self._curr
-00003c80: 656e 745f 6d6f 6461 6c29 7d22 0a20 2020  ent_modal)}".   
-00003c90: 2020 2020 2020 2020 2029 0a0a 2020 2020           )..    
-00003ca0: 2020 2020 7365 6c66 2e5f 6375 7272 656e      self._curren
-00003cb0: 745f 7461 6273 5f67 726f 7570 203d 2074  t_tabs_group = t
-00003cc0: 6162 735f 6772 6f75 700a 2020 2020 2020  abs_group.      
-00003cd0: 2020 7461 6273 5f67 726f 7570 2e61 6464    tabs_group.add
-00003ce0: 5f74 6162 2874 6162 735f 696e 6465 785b  _tab(tabs_index[
-00003cf0: 315d 290a 2020 2020 2020 2020 7365 6c66  1]).        self
-00003d00: 2e5f 6375 7272 656e 745f 7461 6220 3d20  ._current_tab = 
-00003d10: 7461 6273 5f69 6e64 6578 5b31 5d0a 0a20  tabs_index[1].. 
-00003d20: 2020 2020 2020 2069 6620 2275 7064 6174         if "updat
-00003d30: 655f 636f 6e74 6169 6e65 7273 2220 6e6f  e_containers" no
-00003d40: 7420 696e 2073 656c 662e 5f61 7379 6e63  t in self._async
-00003d50: 5f70 6f6f 6c2e 656e 6469 6e67 5f74 6173  _pool.ending_tas
-00003d60: 6b73 3a0a 2020 2020 2020 2020 2020 2020  ks:.            
-00003d70: 7365 6c66 2e5f 6173 796e 635f 706f 6f6c  self._async_pool
-00003d80: 2e65 6e64 696e 675f 7461 736b 735b 0a20  .ending_tasks[. 
-00003d90: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00003da0: 7570 6461 7465 5f63 6f6e 7461 696e 6572  update_container
-00003db0: 7322 0a20 2020 2020 2020 2020 2020 205d  s".            ]
-00003dc0: 203d 2073 656c 662e 5f75 7064 6174 655f   = self._update_
-00003dd0: 636f 6e74 6169 6e65 7273 2829 0a0a 2020  containers()..  
-00003de0: 2020 6465 6620 706f 705f 6f75 745f 6f66    def pop_out_of
-00003df0: 5f74 6162 735f 6772 6f75 7028 7365 6c66  _tabs_group(self
-00003e00: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
-00003e10: 2020 2020 2020 2050 6f70 2074 6865 2063         Pop the c
-00003e20: 7572 7265 6e74 2074 6162 7320 696e 6465  urrent tabs inde
-00003e30: 782e 0a20 2020 2020 2020 2022 2222 0a20  x..        """. 
-00003e40: 2020 2020 2020 2069 6620 6e6f 7420 7365         if not se
-00003e50: 6c66 2e5f 6375 7272 656e 745f 7461 6273  lf._current_tabs
-00003e60: 5f67 726f 7570 3a0a 2020 2020 2020 2020  _group:.        
-00003e70: 2020 2020 6c6f 675f 6572 726f 7228 6c6f      log_error(lo
-00003e80: 6767 6572 2c20 224e 6f20 7461 6273 2067  gger, "No tabs g
-00003e90: 726f 7570 2074 6f20 706f 7020 6f75 7420  roup to pop out 
-00003ea0: 6f66 222c 2054 6162 7345 7272 6f72 290a  of", TabsError).
-00003eb0: 0a20 2020 2020 2020 2073 656c 662e 5f63  .        self._c
-00003ec0: 7572 7265 6e74 5f74 6162 735f 6772 6f75  urrent_tabs_grou
-00003ed0: 7020 3d20 4e6f 6e65 0a20 2020 2020 2020  p = None.       
-00003ee0: 2073 656c 662e 5f63 7572 7265 6e74 5f74   self._current_t
-00003ef0: 6162 203d 204e 6f6e 650a 0a20 2020 2064  ab = None..    d
-00003f00: 6566 2063 6861 6e67 655f 6375 7272 656e  ef change_curren
-00003f10: 745f 7461 6228 7365 6c66 2c20 7461 623a  t_tab(self, tab:
-00003f20: 2073 7472 293a 0a20 2020 2020 2020 2022   str):.        "
-00003f30: 2222 0a20 2020 2020 2020 2043 6861 6e67  "".        Chang
-00003f40: 6520 7468 6520 6375 7272 656e 7420 7461  e the current ta
-00003f50: 622e 0a20 2020 2020 2020 203a 7061 7261  b..        :para
-00003f60: 6d20 7461 623a 2074 6865 206e 616d 6520  m tab: the name 
-00003f70: 6f66 2074 6865 2074 6162 0a20 2020 2020  of the tab.     
-00003f80: 2020 2022 2222 0a20 2020 2020 2020 2069     """.        i
-00003f90: 6620 6e6f 7420 7365 6c66 2e5f 6375 7272  f not self._curr
-00003fa0: 656e 745f 7461 6273 5f67 726f 7570 3a0a  ent_tabs_group:.
-00003fb0: 2020 2020 2020 2020 2020 2020 6c6f 675f              log_
-00003fc0: 6572 726f 7228 6c6f 6767 6572 2c20 224e  error(logger, "N
-00003fd0: 6f20 7461 6273 2067 726f 7570 2074 6f20  o tabs group to 
-00003fe0: 6368 616e 6765 2074 6162 222c 2054 6162  change tab", Tab
-00003ff0: 7345 7272 6f72 290a 0a20 2020 2020 2020  sError)..       
-00004000: 2073 656c 662e 5f63 7572 7265 6e74 5f74   self._current_t
-00004010: 6162 735f 6772 6f75 702e 6164 645f 7461  abs_group.add_ta
-00004020: 6228 7461 6229 0a20 2020 2020 2020 2073  b(tab).        s
-00004030: 656c 662e 5f63 7572 7265 6e74 5f74 6162  elf._current_tab
-00004040: 203d 2074 6162 0a0a 2020 2020 2020 2020   = tab..        
-00004050: 6966 2022 7570 6461 7465 5f63 6f6e 7461  if "update_conta
-00004060: 696e 6572 7322 206e 6f74 2069 6e20 7365  iners" not in se
-00004070: 6c66 2e5f 6173 796e 635f 706f 6f6c 2e65  lf._async_pool.e
-00004080: 6e64 696e 675f 7461 736b 733a 0a20 2020  nding_tasks:.   
-00004090: 2020 2020 2020 2020 2073 656c 662e 5f61           self._a
-000040a0: 7379 6e63 5f70 6f6f 6c2e 656e 6469 6e67  sync_pool.ending
-000040b0: 5f74 6173 6b73 5b0a 2020 2020 2020 2020  _tasks[.        
-000040c0: 2020 2020 2020 2020 2275 7064 6174 655f          "update_
-000040d0: 636f 6e74 6169 6e65 7273 220a 2020 2020  containers".    
-000040e0: 2020 2020 2020 2020 5d20 3d20 7365 6c66          ] = self
-000040f0: 2e5f 7570 6461 7465 5f63 6f6e 7461 696e  ._update_contain
-00004100: 6572 7328 290a 0a20 2020 2061 7379 6e63  ers()..    async
-00004110: 2064 6566 205f 6765 745f 6d6f 6461 6c28   def _get_modal(
-00004120: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
-00004130: 2020 2020 2020 206d 6f64 616c 5f6e 616d         modal_nam
-00004140: 653a 2073 7472 2c0a 2020 2020 2020 2020  e: str,.        
-00004150: 7769 6474 683a 204f 7074 696f 6e61 6c5b  width: Optional[
-00004160: 696e 745d 203d 204e 6f6e 652c 0a20 2020  int] = None,.   
-00004170: 2020 2020 2068 6569 6768 743a 204f 7074       height: Opt
-00004180: 696f 6e61 6c5b 696e 745d 203d 204e 6f6e  ional[int] = Non
-00004190: 652c 0a20 2020 2020 2020 206f 7065 6e5f  e,.        open_
-000041a0: 6279 5f64 6566 6175 6c74 3a20 4f70 7469  by_default: Opti
-000041b0: 6f6e 616c 5b62 6f6f 6c5d 203d 204e 6f6e  onal[bool] = Non
-000041c0: 652c 0a20 2020 2029 202d 3e20 4d6f 6461  e,.    ) -> Moda
-000041d0: 6c3a 0a20 2020 2020 2020 2072 5f68 6173  l:.        r_has
-000041e0: 6820 3d20 7365 6c66 2e5f 6765 745f 6861  h = self._get_ha
-000041f0: 7368 5f66 6f72 5f63 6f6e 7461 696e 6572  sh_for_container
-00004200: 286d 6f64 616c 5f6e 616d 6529 0a20 2020  (modal_name).   
-00004210: 2020 2020 206d 6f64 616c 3a20 4f70 7469       modal: Opti
-00004220: 6f6e 616c 5b4d 6f64 616c 5d20 3d20 6177  onal[Modal] = aw
-00004230: 6169 7420 7365 6c66 2e5f 6170 702e 6765  ait self._app.ge
-00004240: 745f 7265 706f 7274 2872 5f68 6173 683d  t_report(r_hash=
-00004250: 725f 6861 7368 290a 2020 2020 2020 2020  r_hash).        
-00004260: 6966 206e 6f74 206d 6f64 616c 3a0a 2020  if not modal:.  
-00004270: 2020 2020 2020 2020 2020 6d6f 6461 6c3a            modal:
-00004280: 2052 6570 6f72 7420 3d20 6177 6169 7420   Report = await 
-00004290: 7365 6c66 2e5f 6170 702e 6372 6561 7465  self._app.create
-000042a0: 5f72 6570 6f72 7428 0a20 2020 2020 2020  _report(.       
-000042b0: 2020 2020 2020 2020 204d 6f64 616c 2c0a           Modal,.
-000042c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000042d0: 725f 6861 7368 3d72 5f68 6173 682c 0a20  r_hash=r_hash,. 
-000042e0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-000042f0: 6174 683d 7365 6c66 2e5f 6375 7272 656e  ath=self._curren
-00004300: 745f 7061 7468 2c0a 2020 2020 2020 2020  t_path,.        
-00004310: 2020 2020 2020 2020 7072 6f70 6572 7469          properti
-00004320: 6573 3d7b 2277 6964 7468 223a 2077 6964  es={"width": wid
-00004330: 7468 2c20 2268 6569 6768 7422 3a20 6865  th, "height": he
-00004340: 6967 6874 2c20 226f 7065 6e22 3a20 6f70  ight, "open": op
-00004350: 656e 5f62 795f 6465 6661 756c 747d 2c0a  en_by_default},.
-00004360: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-00004370: 2020 2020 2020 2020 2020 6c6f 6767 6572            logger
-00004380: 2e69 6e66 6f28 6627 4372 6561 7465 6420  .info(f'Created 
-00004390: 6d6f 6461 6c20 7b6d 6f64 616c 5f6e 616d  modal {modal_nam
-000043a0: 657d 2077 6974 6820 6964 207b 6d6f 6461  e} with id {moda
-000043b0: 6c5b 2269 6422 5d7d 2729 0a20 2020 2020  l["id"]}').     
-000043c0: 2020 2020 2020 2072 6574 7572 6e20 6d6f         return mo
-000043d0: 6461 6c0a 2020 2020 2020 2020 7072 6f70  dal.        prop
-000043e0: 6572 7469 6573 203d 207b 7d0a 2020 2020  erties = {}.    
-000043f0: 2020 2020 6966 2077 6964 7468 3a0a 2020      if width:.  
-00004400: 2020 2020 2020 2020 2020 7072 6f70 6572            proper
-00004410: 7469 6573 5b22 7769 6474 6822 5d20 3d20  ties["width"] = 
-00004420: 7769 6474 680a 2020 2020 2020 2020 6966  width.        if
-00004430: 2068 6569 6768 743a 0a20 2020 2020 2020   height:.       
-00004440: 2020 2020 2070 726f 7065 7274 6965 735b       properties[
-00004450: 2268 6569 6768 7422 5d20 3d20 6865 6967  "height"] = heig
-00004460: 6874 0a20 2020 2020 2020 2069 6620 6f70  ht.        if op
-00004470: 656e 5f62 795f 6465 6661 756c 743a 0a20  en_by_default:. 
-00004480: 2020 2020 2020 2020 2020 2070 726f 7065             prope
-00004490: 7274 6965 735b 226f 7065 6e22 5d20 3d20  rties["open"] = 
-000044a0: 6f70 656e 5f62 795f 6465 6661 756c 740a  open_by_default.
-000044b0: 2020 2020 2020 2020 6966 2070 726f 7065          if prope
-000044c0: 7274 6965 733a 0a20 2020 2020 2020 2020  rties:.         
-000044d0: 2020 2061 7761 6974 2073 656c 662e 5f61     await self._a
-000044e0: 7070 2e75 7064 6174 655f 7265 706f 7274  pp.update_report
-000044f0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00004500: 2020 725f 6861 7368 3d72 5f68 6173 682c    r_hash=r_hash,
-00004510: 2070 726f 7065 7274 6965 733d 7072 6f70   properties=prop
-00004520: 6572 7469 6573 2c20 7061 7468 3d73 656c  erties, path=sel
-00004530: 662e 5f63 7572 7265 6e74 5f70 6174 680a  f._current_path.
-00004540: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-00004550: 2020 2020 2020 2020 2020 6c6f 6767 6572            logger
-00004560: 2e69 6e66 6f28 6627 5570 6461 7465 6420  .info(f'Updated 
-00004570: 6d6f 6461 6c20 7b6d 6f64 616c 5f6e 616d  modal {modal_nam
-00004580: 657d 2077 6974 6820 6964 207b 6d6f 6461  e} with id {moda
-00004590: 6c5b 2269 6422 5d7d 2729 0a20 2020 2020  l["id"]}').     
-000045a0: 2020 2072 6574 7572 6e20 6d6f 6461 6c0a     return modal.
-000045b0: 0a20 2020 2061 7379 6e63 2064 6566 2073  .    async def s
-000045c0: 6574 5f6d 6f64 616c 280a 2020 2020 2020  et_modal(.      
-000045d0: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
-000045e0: 6d6f 6461 6c5f 6e61 6d65 3a20 7374 722c  modal_name: str,
-000045f0: 0a20 2020 2020 2020 2077 6964 7468 3a20  .        width: 
-00004600: 4f70 7469 6f6e 616c 5b69 6e74 5d20 3d20  Optional[int] = 
-00004610: 4e6f 6e65 2c0a 2020 2020 2020 2020 6865  None,.        he
-00004620: 6967 6874 3a20 4f70 7469 6f6e 616c 5b69  ight: Optional[i
-00004630: 6e74 5d20 3d20 4e6f 6e65 2c0a 2020 2020  nt] = None,.    
-00004640: 2020 2020 6f70 656e 5f62 795f 6465 6661      open_by_defa
-00004650: 756c 743a 204f 7074 696f 6e61 6c5b 626f  ult: Optional[bo
-00004660: 6f6c 5d20 3d20 4e6f 6e65 2c0a 2020 2020  ol] = None,.    
-00004670: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
-00004680: 2020 2022 2222 5365 7420 7468 6520 6375     """Set the cu
-00004690: 7272 656e 7420 6d6f 6461 6c2e 0a20 2020  rrent modal..   
-000046a0: 2020 2020 203a 7061 7261 6d20 6d6f 6461       :param moda
-000046b0: 6c5f 6e61 6d65 3a20 7468 6520 6e61 6d65  l_name: the name
-000046c0: 206f 6620 7468 6520 6d6f 6461 6c0a 2020   of the modal.  
-000046d0: 2020 2020 2020 3a70 6172 616d 2077 6964        :param wid
-000046e0: 7468 3a20 7468 6520 7769 6474 6820 6f66  th: the width of
-000046f0: 2074 6865 206d 6f64 616c 0a20 2020 2020   the modal.     
-00004700: 2020 203a 7061 7261 6d20 6865 6967 6874     :param height
-00004710: 3a20 7468 6520 6865 6967 6874 206f 6620  : the height of 
-00004720: 7468 6520 6d6f 6461 6c0a 2020 2020 2020  the modal.      
-00004730: 2020 3a70 6172 616d 206f 7065 6e5f 6279    :param open_by
-00004740: 5f64 6566 6175 6c74 3a20 7768 6574 6865  _default: whethe
-00004750: 7220 7468 6520 6d6f 6461 6c20 6973 206f  r the modal is o
-00004760: 7065 6e20 6279 2064 6566 6175 6c74 0a20  pen by default. 
-00004770: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00004780: 2020 2069 6620 7365 6c66 2e5f 6375 7272     if self._curr
-00004790: 656e 745f 7461 6273 5f67 726f 7570 3a0a  ent_tabs_group:.
-000047a0: 2020 2020 2020 2020 2020 2020 6c6f 675f              log_
-000047b0: 6572 726f 7228 0a20 2020 2020 2020 2020  error(.         
-000047c0: 2020 2020 2020 206c 6f67 6765 722c 0a20         logger,. 
-000047d0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-000047e0: 4361 6e6e 6f74 2073 6574 2061 206d 6f64  Cannot set a mod
-000047f0: 616c 2069 6e20 6120 7461 6273 2067 726f  al in a tabs gro
-00004800: 7570 2c20 706f 7020 6f75 7420 6f66 2074  up, pop out of t
-00004810: 6865 2074 6162 7320 6772 6f75 7020 6669  he tabs group fi
-00004820: 7273 7422 2c0a 2020 2020 2020 2020 2020  rst",.          
-00004830: 2020 2020 2020 4d6f 6461 6c45 7272 6f72        ModalError
-00004840: 2c0a 2020 2020 2020 2020 2020 2020 290a  ,.            ).
-00004850: 0a20 2020 2020 2020 206d 6f64 616c 203d  .        modal =
-00004860: 2061 7761 6974 2073 656c 662e 5f67 6574   await self._get
-00004870: 5f6d 6f64 616c 286d 6f64 616c 5f6e 616d  _modal(modal_nam
-00004880: 652c 2077 6964 7468 2c20 6865 6967 6874  e, width, height
-00004890: 2c20 6f70 656e 5f62 795f 6465 6661 756c  , open_by_defaul
-000048a0: 7429 0a20 2020 2020 2020 2073 656c 662e  t).        self.
-000048b0: 5f63 7572 7265 6e74 5f6d 6f64 616c 203d  _current_modal =
-000048c0: 206d 6f64 616c 0a0a 2020 2020 2020 2020   modal..        
-000048d0: 6966 2022 7570 6461 7465 5f63 6f6e 7461  if "update_conta
-000048e0: 696e 6572 7322 206e 6f74 2069 6e20 7365  iners" not in se
-000048f0: 6c66 2e5f 6173 796e 635f 706f 6f6c 2e65  lf._async_pool.e
-00004900: 6e64 696e 675f 7461 736b 733a 0a20 2020  nding_tasks:.   
-00004910: 2020 2020 2020 2020 2073 656c 662e 5f61           self._a
-00004920: 7379 6e63 5f70 6f6f 6c2e 656e 6469 6e67  sync_pool.ending
-00004930: 5f74 6173 6b73 5b0a 2020 2020 2020 2020  _tasks[.        
-00004940: 2020 2020 2020 2020 2275 7064 6174 655f          "update_
-00004950: 636f 6e74 6169 6e65 7273 220a 2020 2020  containers".    
-00004960: 2020 2020 2020 2020 5d20 3d20 7365 6c66          ] = self
-00004970: 2e5f 7570 6461 7465 5f63 6f6e 7461 696e  ._update_contain
-00004980: 6572 7328 290a 0a20 2020 2064 6566 2070  ers()..    def p
-00004990: 6f70 5f6f 7574 5f6f 665f 6d6f 6461 6c28  op_out_of_modal(
-000049a0: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
-000049b0: 2222 506f 7020 7468 6520 6375 7272 656e  ""Pop the curren
-000049c0: 7420 6d6f 6461 6c2e 2222 220a 2020 2020  t modal.""".    
-000049d0: 2020 2020 6966 206e 6f74 2073 656c 662e      if not self.
-000049e0: 5f63 7572 7265 6e74 5f6d 6f64 616c 3a0a  _current_modal:.
-000049f0: 2020 2020 2020 2020 2020 2020 6c6f 675f              log_
-00004a00: 6572 726f 7228 6c6f 6767 6572 2c20 224e  error(logger, "N
-00004a10: 6f20 6d6f 6461 6c20 746f 2070 6f70 206f  o modal to pop o
-00004a20: 7574 206f 6622 2c20 4d6f 6461 6c45 7272  ut of", ModalErr
-00004a30: 6f72 290a 0a20 2020 2020 2020 2069 6620  or)..        if 
-00004a40: 7365 6c66 2e5f 6375 7272 656e 745f 7461  self._current_ta
-00004a50: 6273 5f67 726f 7570 3a0a 2020 2020 2020  bs_group:.      
-00004a60: 2020 2020 2020 6c6f 675f 6572 726f 7228        log_error(
-00004a70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004a80: 206c 6f67 6765 722c 0a20 2020 2020 2020   logger,.       
-00004a90: 2020 2020 2020 2020 2022 4361 6e6e 6f74           "Cannot
-00004aa0: 2070 6f70 206f 7574 206f 6620 6120 6d6f   pop out of a mo
-00004ab0: 6461 6c20 7768 656e 2069 6e20 6120 7461  dal when in a ta
-00004ac0: 6273 2067 726f 7570 2c20 706f 7020 6f75  bs group, pop ou
-00004ad0: 7420 6f66 2074 6865 2074 6162 7320 6772  t of the tabs gr
-00004ae0: 6f75 7020 6669 7273 7422 2c0a 2020 2020  oup first",.    
-00004af0: 2020 2020 2020 2020 2020 2020 4d6f 6461              Moda
-00004b00: 6c45 7272 6f72 2c0a 2020 2020 2020 2020  lError,.        
-00004b10: 2020 2020 290a 2020 2020 2020 2020 6966      ).        if
-00004b20: 2073 656c 662e 5f62 656e 746f 626f 785f   self._bentobox_
-00004b30: 6461 7461 3a0a 2020 2020 2020 2020 2020  data:.          
-00004b40: 2020 6c6f 675f 6572 726f 7228 0a20 2020    log_error(.   
-00004b50: 2020 2020 2020 2020 2020 2020 206c 6f67               log
-00004b60: 6765 722c 0a20 2020 2020 2020 2020 2020  ger,.           
-00004b70: 2020 2020 2022 4361 6e6e 6f74 2070 6f70       "Cannot pop
-00004b80: 206f 7574 206f 6620 6120 6d6f 6461 6c20   out of a modal 
-00004b90: 7768 656e 2069 6e20 6120 6265 6e74 6f62  when in a bentob
-00004ba0: 6f78 2c20 636c 6f73 6520 7468 6520 6265  ox, close the be
-00004bb0: 6e74 6f62 6f78 2066 6972 7374 222c 0a20  ntobox first",. 
-00004bc0: 2020 2020 2020 2020 2020 2020 2020 204d                 M
-00004bd0: 6f64 616c 4572 726f 722c 0a20 2020 2020  odalError,.     
-00004be0: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
-00004bf0: 2020 7365 6c66 2e5f 6375 7272 656e 745f    self._current_
-00004c00: 6d6f 6461 6c20 3d20 4e6f 6e65 0a0a 2020  modal = None..  
-00004c10: 2020 6173 796e 6320 6465 6620 5f67 6574    async def _get
-00004c20: 5f63 7572 7265 6e74 5f6d 6f64 616c 2873  _current_modal(s
-00004c30: 656c 6629 202d 3e20 4d6f 6461 6c3a 0a20  elf) -> Modal:. 
-00004c40: 2020 2020 2020 2022 2222 4765 7420 7468         """Get th
-00004c50: 6520 6375 7272 656e 7420 6d6f 6461 6c2e  e current modal.
-00004c60: 2222 220a 2020 2020 2020 2020 6966 206e  """.        if n
-00004c70: 6f74 2073 656c 662e 5f63 7572 7265 6e74  ot self._current
-00004c80: 5f6d 6f64 616c 3a0a 2020 2020 2020 2020  _modal:.        
-00004c90: 2020 2020 6c6f 675f 6572 726f 7228 6c6f      log_error(lo
-00004ca0: 6767 6572 2c20 224e 6f20 6d6f 6461 6c20  gger, "No modal 
-00004cb0: 7365 7422 2c20 4d6f 6461 6c45 7272 6f72  set", ModalError
-00004cc0: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
-00004cd0: 662e 5f61 7070 2e61 7069 5f63 6c69 656e  f._app.api_clien
-00004ce0: 742e 6361 6368 655f 656e 6162 6c65 643a  t.cache_enabled:
-00004cf0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00004d00: 7572 6e20 7365 6c66 2e5f 6375 7272 656e  urn self._curren
-00004d10: 745f 6d6f 6461 6c0a 2020 2020 2020 2020  t_modal.        
-00004d20: 6c61 7374 5f6d 6f64 616c 203d 2073 656c  last_modal = sel
-00004d30: 662e 5f63 7572 7265 6e74 5f6d 6f64 616c  f._current_modal
-00004d40: 0a20 2020 2020 2020 2073 656c 662e 5f63  .        self._c
-00004d50: 7572 7265 6e74 5f6d 6f64 616c 203d 2061  urrent_modal = a
-00004d60: 7761 6974 2073 656c 662e 5f61 7070 2e67  wait self._app.g
-00004d70: 6574 5f72 6570 6f72 7428 0a20 2020 2020  et_report(.     
-00004d80: 2020 2020 2020 2072 5f68 6173 683d 7365         r_hash=se
-00004d90: 6c66 2e5f 6375 7272 656e 745f 6d6f 6461  lf._current_moda
-00004da0: 6c5b 2270 726f 7065 7274 6965 7322 5d5b  l["properties"][
-00004db0: 2268 6173 6822 5d0a 2020 2020 2020 2020  "hash"].        
-00004dc0: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
-00004dd0: 662e 5f63 7572 7265 6e74 5f6d 6f64 616c  f._current_modal
-00004de0: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
-00004df0: 2020 2020 2020 6c6f 675f 6572 726f 7228        log_error(
-00004e00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004e10: 206c 6f67 6765 722c 0a20 2020 2020 2020   logger,.       
-00004e20: 2020 2020 2020 2020 2066 274e 6f20 6d6f           f'No mo
-00004e30: 6461 6c20 666f 756e 6420 7769 7468 206e  dal found with n
-00004e40: 616d 6520 7b6c 6173 745f 6d6f 6461 6c5b  ame {last_modal[
-00004e50: 2270 726f 7065 7274 6965 7322 5d5b 226e  "properties"]["n
-00004e60: 616d 6522 5d7d 272c 0a20 2020 2020 2020  ame"]}',.       
-00004e70: 2020 2020 2020 2020 204d 6f64 616c 4572           ModalEr
-00004e80: 726f 722c 0a20 2020 2020 2020 2020 2020  ror,.           
-00004e90: 2029 0a20 2020 2020 2020 2072 6574 7572   ).        retur
-00004ea0: 6e20 7365 6c66 2e5f 6375 7272 656e 745f  n self._current_
-00004eb0: 6d6f 6461 6c0a 0a20 2020 2061 7379 6e63  modal..    async
-00004ec0: 2064 6566 205f 6765 745f 6375 7272 656e   def _get_curren
-00004ed0: 745f 7461 6273 5f67 726f 7570 2873 656c  t_tabs_group(sel
-00004ee0: 6629 202d 3e20 5461 6273 4772 6f75 703a  f) -> TabsGroup:
-00004ef0: 0a20 2020 2020 2020 2022 2222 4765 7420  .        """Get 
-00004f00: 7468 6520 6375 7272 656e 7420 7461 6273  the current tabs
-00004f10: 2067 726f 7570 2e22 2222 0a20 2020 2020   group.""".     
-00004f20: 2020 2069 6620 6e6f 7420 7365 6c66 2e5f     if not self._
-00004f30: 6375 7272 656e 745f 7461 6273 5f67 726f  current_tabs_gro
-00004f40: 7570 3a0a 2020 2020 2020 2020 2020 2020  up:.            
-00004f50: 6c6f 675f 6572 726f 7228 6c6f 6767 6572  log_error(logger
-00004f60: 2c20 224e 6f20 7461 6273 2067 726f 7570  , "No tabs group
-00004f70: 2067 6574 222c 2054 6162 7345 7272 6f72   get", TabsError
-00004f80: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
-00004f90: 662e 5f61 7070 2e61 7069 5f63 6c69 656e  f._app.api_clien
-00004fa0: 742e 6361 6368 655f 656e 6162 6c65 643a  t.cache_enabled:
-00004fb0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00004fc0: 7572 6e20 7365 6c66 2e5f 6375 7272 656e  urn self._curren
-00004fd0: 745f 7461 6273 5f67 726f 7570 0a20 2020  t_tabs_group.   
-00004fe0: 2020 2020 206c 6173 745f 7461 6273 5f67       last_tabs_g
-00004ff0: 726f 7570 203d 2073 656c 662e 5f63 7572  roup = self._cur
-00005000: 7265 6e74 5f74 6162 735f 6772 6f75 700a  rent_tabs_group.
-00005010: 2020 2020 2020 2020 7365 6c66 2e5f 6375          self._cu
-00005020: 7272 656e 745f 7461 6273 5f67 726f 7570  rrent_tabs_group
-00005030: 203d 2061 7761 6974 2073 656c 662e 5f61   = await self._a
-00005040: 7070 2e67 6574 5f72 6570 6f72 7428 0a20  pp.get_report(. 
-00005050: 2020 2020 2020 2020 2020 2072 5f68 6173             r_has
-00005060: 683d 7365 6c66 2e5f 6375 7272 656e 745f  h=self._current_
-00005070: 7461 6273 5f67 726f 7570 5b22 7072 6f70  tabs_group["prop
-00005080: 6572 7469 6573 225d 5b22 6861 7368 225d  erties"]["hash"]
-00005090: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
-000050a0: 2020 2069 6620 7365 6c66 2e5f 6375 7272     if self._curr
-000050b0: 656e 745f 7461 6273 5f67 726f 7570 2069  ent_tabs_group i
-000050c0: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
-000050d0: 2020 2020 6c6f 675f 6572 726f 7228 0a20      log_error(. 
-000050e0: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-000050f0: 6f67 6765 722c 0a20 2020 2020 2020 2020  ogger,.         
-00005100: 2020 2020 2020 2066 274e 6f20 7461 6273         f'No tabs
-00005110: 2067 726f 7570 2066 6f75 6e64 2077 6974   group found wit
-00005120: 6820 6e61 6d65 207b 6c61 7374 5f74 6162  h name {last_tab
-00005130: 735f 6772 6f75 705b 2270 726f 7065 7274  s_group["propert
-00005140: 6965 7322 5d5b 226e 616d 6522 5d7d 272c  ies"]["name"]}',
-00005150: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005160: 2054 6162 7345 7272 6f72 2c0a 2020 2020   TabsError,.    
-00005170: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00005180: 2020 7265 7475 726e 2073 656c 662e 5f63    return self._c
-00005190: 7572 7265 6e74 5f74 6162 735f 6772 6f75  urrent_tabs_grou
-000051a0: 700a 0a20 2020 2064 6566 205f 6765 745f  p..    def _get_
-000051b0: 6368 6172 745f 6861 7368 2873 656c 662c  chart_hash(self,
-000051c0: 206f 7264 6572 3a20 696e 7429 202d 3e20   order: int) -> 
-000051d0: 7374 723a 0a20 2020 2020 2020 2072 5f68  str:.        r_h
-000051e0: 6173 6820 3d20 6622 7b6f 7264 6572 7d22  ash = f"{order}"
-000051f0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-00005200: 2e5f 6375 7272 656e 745f 7461 6273 5f67  ._current_tabs_g
-00005210: 726f 7570 3a0a 2020 2020 2020 2020 2020  roup:.          
-00005220: 2020 725f 6861 7368 203d 2066 277b 7365    r_hash = f'{se
-00005230: 6c66 2e5f 6375 7272 656e 745f 7461 6273  lf._current_tabs
-00005240: 5f67 726f 7570 5b22 7072 6f70 6572 7469  _group["properti
-00005250: 6573 225d 5b22 6861 7368 225d 7d5f 7b73  es"]["hash"]}_{s
-00005260: 656c 662e 5f63 7572 7265 6e74 5f74 6162  elf._current_tab
-00005270: 7d5f 7b6f 7264 6572 7d27 0a20 2020 2020  }_{order}'.     
-00005280: 2020 2065 6c69 6620 7365 6c66 2e5f 6375     elif self._cu
-00005290: 7272 656e 745f 6d6f 6461 6c3a 0a20 2020  rrent_modal:.   
-000052a0: 2020 2020 2020 2020 2072 5f68 6173 6820           r_hash 
-000052b0: 3d20 6627 7b73 656c 662e 5f63 7572 7265  = f'{self._curre
-000052c0: 6e74 5f6d 6f64 616c 5b22 7072 6f70 6572  nt_modal["proper
-000052d0: 7469 6573 225d 5b22 6861 7368 225d 7d5f  ties"]["hash"]}_
-000052e0: 7b6f 7264 6572 7d27 0a20 2020 2020 2020  {order}'.       
-000052f0: 2065 6c69 6620 7365 6c66 2e5f 6375 7272   elif self._curr
-00005300: 656e 745f 7061 7468 3a0a 2020 2020 2020  ent_path:.      
-00005310: 2020 2020 2020 725f 6861 7368 203d 2066        r_hash = f
-00005320: 227b 7365 6c66 2e5f 6375 7272 656e 745f  "{self._current_
-00005330: 7061 7468 7d5f 7b6f 7264 6572 7d22 0a20  path}_{order}". 
-00005340: 2020 2020 2020 2072 6574 7572 6e20 725f         return r_
-00005350: 6861 7368 0a0a 2020 2020 6173 796e 6320  hash..    async 
-00005360: 6465 6620 5f67 6574 5f63 6861 7274 5f72  def _get_chart_r
-00005370: 6570 6f72 7428 0a20 2020 2020 2020 2073  eport(.        s
-00005380: 656c 662c 206f 7264 6572 3a20 696e 742c  elf, order: int,
-00005390: 2063 6861 7274 5f63 6c61 7373 3a20 7479   chart_class: ty
-000053a0: 7065 5b52 6570 6f72 745d 2c20 6372 6561  pe[Report], crea
-000053b0: 7465 5f69 665f 6e6f 745f 6578 6973 7473  te_if_not_exists
-000053c0: 3a20 626f 6f6c 203d 2054 7275 650a 2020  : bool = True.  
-000053d0: 2020 2920 2d3e 2074 7570 6c65 5b73 7472    ) -> tuple[str
-000053e0: 2c20 4f70 7469 6f6e 616c 5b52 6570 6f72  , Optional[Repor
-000053f0: 745d 5d3a 0a20 2020 2020 2020 2022 2222  t]]:.        """
-00005400: 4765 7420 7468 6520 6368 6172 7420 7265  Get the chart re
-00005410: 706f 7274 2e0a 2020 2020 2020 2020 3a70  port..        :p
-00005420: 6172 616d 206f 7264 6572 3a20 7468 6520  aram order: the 
-00005430: 6f72 6465 7220 6f66 2074 6865 2063 6861  order of the cha
-00005440: 7274 0a20 2020 2020 2020 203a 7061 7261  rt.        :para
-00005450: 6d20 6368 6172 745f 636c 6173 733a 2074  m chart_class: t
-00005460: 6865 2063 6861 7274 2063 6c61 7373 0a20  he chart class. 
-00005470: 2020 2020 2020 203a 7061 7261 6d20 6372         :param cr
-00005480: 6561 7465 5f69 665f 6e6f 745f 6578 6973  eate_if_not_exis
-00005490: 7473 3a20 7768 6574 6865 7220 746f 2063  ts: whether to c
-000054a0: 7265 6174 6520 7468 6520 6368 6172 7420  reate the chart 
-000054b0: 6966 2069 7420 646f 6573 6e27 7420 6578  if it doesn't ex
-000054c0: 6973 740a 2020 2020 2020 2020 2222 220a  ist.        """.
-000054d0: 2020 2020 2020 2020 725f 6861 7368 203d          r_hash =
-000054e0: 2073 656c 662e 5f67 6574 5f63 6861 7274   self._get_chart
-000054f0: 5f68 6173 6828 6f72 6465 7229 0a20 2020  _hash(order).   
-00005500: 2020 2020 2072 6570 6f72 7420 3d20 6177       report = aw
-00005510: 6169 7420 7365 6c66 2e5f 6170 702e 6765  ait self._app.ge
-00005520: 745f 7265 706f 7274 2872 5f68 6173 683d  t_report(r_hash=
-00005530: 725f 6861 7368 290a 0a20 2020 2020 2020  r_hash)..       
-00005540: 2069 6620 6e6f 7420 7265 706f 7274 3a0a   if not report:.
-00005550: 2020 2020 2020 2020 2020 2020 6966 2063              if c
-00005560: 7265 6174 655f 6966 5f6e 6f74 5f65 7869  reate_if_not_exi
-00005570: 7374 733a 0a20 2020 2020 2020 2020 2020  sts:.           
-00005580: 2020 2020 2072 6570 6f72 7420 3d20 6177       report = aw
-00005590: 6169 7420 7365 6c66 2e5f 6170 702e 6372  ait self._app.cr
-000055a0: 6561 7465 5f72 6570 6f72 7428 0a20 2020  eate_report(.   
-000055b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000055c0: 2063 6861 7274 5f63 6c61 7373 2c20 725f   chart_class, r_
-000055d0: 6861 7368 3d72 5f68 6173 682c 206f 7264  hash=r_hash, ord
-000055e0: 6572 3d6f 7264 6572 0a20 2020 2020 2020  er=order.       
-000055f0: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-00005600: 2020 2020 2020 2020 2020 206c 6f67 6765             logge
-00005610: 722e 696e 666f 2866 2743 7265 6174 6564  r.info(f'Created
-00005620: 207b 6368 6172 745f 636c 6173 732e 5f5f   {chart_class.__
-00005630: 6e61 6d65 5f5f 7d20 7769 7468 2069 6420  name__} with id 
-00005640: 7b72 6570 6f72 745b 2269 6422 5d7d 2729  {report["id"]}')
-00005650: 0a20 2020 2020 2020 2065 6c69 6620 7265  .        elif re
-00005660: 706f 7274 2e72 6570 6f72 745f 7479 7065  port.report_type
-00005670: 2021 3d20 6368 6172 745f 636c 6173 732e   != chart_class.
-00005680: 7265 706f 7274 5f74 7970 653a 0a20 2020  report_type:.   
-00005690: 2020 2020 2020 2020 2061 7761 6974 2072           await r
-000056a0: 6570 6f72 742e 6368 616e 6765 5f72 6570  eport.change_rep
-000056b0: 6f72 745f 7479 7065 2863 6861 7274 5f63  ort_type(chart_c
-000056c0: 6c61 7373 290a 0a20 2020 2020 2020 2072  lass)..        r
-000056d0: 6574 7572 6e20 725f 6861 7368 2c20 7265  eturn r_hash, re
-000056e0: 706f 7274 0a0a 2020 2020 6173 796e 6320  port..    async 
-000056f0: 6465 6620 6765 745f 636f 6d70 6f6e 656e  def get_componen
-00005700: 745f 6279 5f6f 7264 6572 2873 656c 662c  t_by_order(self,
-00005710: 206f 7264 6572 3a20 696e 7429 202d 3e20   order: int) -> 
-00005720: 4f70 7469 6f6e 616c 5b64 6963 745d 3a0a  Optional[dict]:.
-00005730: 2020 2020 2020 2020 2222 2247 6574 2074          """Get t
-00005740: 6865 2063 6f6d 706f 6e65 6e74 2062 7920  he component by 
-00005750: 6f72 6465 722e 0a20 2020 2020 2020 203a  order..        :
-00005760: 7061 7261 6d20 6f72 6465 723a 2074 6865  param order: the
-00005770: 206f 7264 6572 206f 6620 7468 6520 636f   order of the co
-00005780: 6d70 6f6e 656e 740a 2020 2020 2020 2020  mponent.        
-00005790: 2222 220a 2020 2020 2020 2020 725f 6861  """.        r_ha
-000057a0: 7368 203d 2073 656c 662e 5f67 6574 5f63  sh = self._get_c
-000057b0: 6861 7274 5f68 6173 6828 6f72 6465 7229  hart_hash(order)
-000057c0: 0a20 2020 2020 2020 2072 6570 6f72 7420  .        report 
-000057d0: 3d20 6177 6169 7420 7365 6c66 2e5f 6170  = await self._ap
-000057e0: 702e 6765 745f 7265 706f 7274 2872 5f68  p.get_report(r_h
-000057f0: 6173 683d 725f 6861 7368 290a 2020 2020  ash=r_hash).    
-00005800: 2020 2020 6966 206e 6f74 2072 6570 6f72      if not repor
-00005810: 743a 0a20 2020 2020 2020 2020 2020 2072  t:.            r
-00005820: 6574 7572 6e20 4e6f 6e65 0a20 2020 2020  eturn None.     
-00005830: 2020 2072 6574 7572 6e20 7265 706f 7274     return report
-00005840: 2e63 6173 6361 6465 5f74 6f5f 6469 6374  .cascade_to_dict
-00005850: 2829 0a0a 2020 2020 6173 796e 6320 6465  ()..    async de
-00005860: 6620 6765 745f 6d6f 6461 6c28 7365 6c66  f get_modal(self
-00005870: 2c20 6d6f 6461 6c5f 6e61 6d65 3a20 7374  , modal_name: st
-00005880: 7229 202d 3e20 4f70 7469 6f6e 616c 5b64  r) -> Optional[d
-00005890: 6963 745d 3a0a 2020 2020 2020 2020 2222  ict]:.        ""
-000058a0: 2247 6574 2074 6865 206d 6f64 616c 2e0a  "Get the modal..
-000058b0: 2020 2020 2020 2020 3a70 6172 616d 206d          :param m
-000058c0: 6f64 616c 5f6e 616d 653a 2074 6865 206e  odal_name: the n
-000058d0: 616d 6520 6f66 2074 6865 206d 6f64 616c  ame of the modal
-000058e0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-000058f0: 2020 2020 2072 5f68 6173 6820 3d20 7365       r_hash = se
-00005900: 6c66 2e5f 6765 745f 6861 7368 5f66 6f72  lf._get_hash_for
-00005910: 5f63 6f6e 7461 696e 6572 286d 6f64 616c  _container(modal
-00005920: 5f6e 616d 6529 0a20 2020 2020 2020 206d  _name).        m
-00005930: 6f64 616c 203d 2061 7761 6974 2073 656c  odal = await sel
-00005940: 662e 5f61 7070 2e67 6574 5f72 6570 6f72  f._app.get_repor
-00005950: 7428 725f 6861 7368 3d72 5f68 6173 6829  t(r_hash=r_hash)
-00005960: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
-00005970: 6d6f 6461 6c3a 0a20 2020 2020 2020 2020  modal:.         
-00005980: 2020 2072 6574 7572 6e20 4e6f 6e65 0a20     return None. 
-00005990: 2020 2020 2020 2072 6574 7572 6e20 6d6f         return mo
-000059a0: 6461 6c2e 6361 7363 6164 655f 746f 5f64  dal.cascade_to_d
-000059b0: 6963 7428 290a 0a20 2020 2061 7379 6e63  ict()..    async
-000059c0: 2064 6566 2067 6574 5f74 6162 735f 6772   def get_tabs_gr
-000059d0: 6f75 7028 7365 6c66 2c20 7461 6273 5f69  oup(self, tabs_i
-000059e0: 6e64 6578 3a20 7475 706c 655b 7374 722c  ndex: tuple[str,
-000059f0: 2073 7472 5d29 202d 3e20 4f70 7469 6f6e   str]) -> Option
-00005a00: 616c 5b64 6963 745d 3a0a 2020 2020 2020  al[dict]:.      
-00005a10: 2020 2222 2247 6574 2074 6865 2074 6162    """Get the tab
-00005a20: 7320 6772 6f75 702e 0a20 2020 2020 2020  s group..       
-00005a30: 203a 7061 7261 6d20 7461 6273 5f69 6e64   :param tabs_ind
-00005a40: 6578 3a20 7468 6520 696e 6465 7820 6f66  ex: the index of
-00005a50: 2074 6865 2074 6162 7320 6772 6f75 700a   the tabs group.
-00005a60: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00005a70: 2020 2020 725f 6861 7368 203d 2073 656c      r_hash = sel
-00005a80: 662e 5f67 6574 5f68 6173 685f 666f 725f  f._get_hash_for_
-00005a90: 636f 6e74 6169 6e65 7228 7461 6273 5f69  container(tabs_i
-00005aa0: 6e64 6578 5b30 5d29 0a20 2020 2020 2020  ndex[0]).       
-00005ab0: 2074 6162 735f 6772 6f75 7020 3d20 6177   tabs_group = aw
-00005ac0: 6169 7420 7365 6c66 2e5f 6170 702e 6765  ait self._app.ge
-00005ad0: 745f 7265 706f 7274 2872 5f68 6173 683d  t_report(r_hash=
-00005ae0: 725f 6861 7368 290a 2020 2020 2020 2020  r_hash).        
-00005af0: 6966 206e 6f74 2074 6162 735f 6772 6f75  if not tabs_grou
-00005b00: 703a 0a20 2020 2020 2020 2020 2020 2072  p:.            r
-00005b10: 6574 7572 6e20 4e6f 6e65 0a20 2020 2020  eturn None.     
-00005b20: 2020 2072 6574 7572 6e20 7461 6273 5f67     return tabs_g
-00005b30: 726f 7570 2e63 6173 6361 6465 5f74 6f5f  roup.cascade_to_
-00005b40: 6469 6374 2829 0a0a 2020 2020 6173 796e  dict()..    asyn
-00005b50: 6320 6465 6620 5f74 7279 5f74 6f5f 7265  c def _try_to_re
-00005b60: 7573 655f 6461 7461 280a 2020 2020 2020  use_data(.      
-00005b70: 2020 7365 6c66 2c20 6461 7461 5f73 6574    self, data_set
-00005b80: 3a20 4461 7461 5365 742c 2064 6174 613a  : DataSet, data:
-00005b90: 2055 6e69 6f6e 5b6c 6973 742c 2070 642e   Union[list, pd.
-00005ba0: 4461 7461 4672 616d 655d 0a20 2020 2029  DataFrame].    )
-00005bb0: 202d 3e20 6469 6374 5b73 7472 2c20 7475   -> dict[str, tu
-00005bc0: 706c 655b 4d61 7070 696e 672c 2044 6174  ple[Mapping, Dat
-00005bd0: 6153 6574 2c20 6469 6374 5d5d 3a0a 2020  aSet, dict]]:.  
-00005be0: 2020 2020 2020 2222 2254 7279 2074 6f20        """Try to 
-00005bf0: 7265 7573 6520 7468 6520 6461 7461 2073  reuse the data s
-00005c00: 6574 2e0a 2020 2020 2020 2020 3a70 6172  et..        :par
-00005c10: 616d 2064 6174 615f 7365 743a 2074 6865  am data_set: the
-00005c20: 2064 6174 6120 7365 740a 2020 2020 2020   data set.      
-00005c30: 2020 3a70 6172 616d 2064 6174 613a 2074    :param data: t
-00005c40: 6865 2064 6174 610a 2020 2020 2020 2020  he data.        
-00005c50: 2222 220a 2020 2020 2020 2020 6466 203d  """.        df =
-00005c60: 2076 616c 6964 6174 655f 6461 7461 5f69   validate_data_i
-00005c70: 735f 7061 6e64 6172 6162 6c65 2864 6174  s_pandarable(dat
-00005c80: 6129 0a20 2020 2020 2020 2061 7578 5f64  a).        aux_d
-00005c90: 6174 615f 706f 696e 7420 3d20 6177 6169  ata_point = awai
-00005ca0: 7420 6461 7461 5f73 6574 2e67 6574 5f6f  t data_set.get_o
-00005cb0: 6e65 5f64 6174 615f 706f 696e 7428 290a  ne_data_point().
-00005cc0: 2020 2020 2020 2020 6966 206e 6f74 2061          if not a
-00005cd0: 7578 5f64 6174 615f 706f 696e 743a 0a20  ux_data_point:. 
-00005ce0: 2020 2020 2020 2020 2020 206c 6f67 5f65             log_e
-00005cf0: 7272 6f72 280a 2020 2020 2020 2020 2020  rror(.          
-00005d00: 2020 2020 2020 6c6f 6767 6572 2c0a 2020        logger,.  
-00005d10: 2020 2020 2020 2020 2020 2020 2020 6622                f"
-00005d20: 4361 6e6e 6f74 2072 6575 7365 2064 6174  Cannot reuse dat
-00005d30: 6120 7365 7420 7b73 7472 2864 6174 615f  a set {str(data_
-00005d40: 7365 7429 7d20 6265 6361 7573 6520 7468  set)} because th
-00005d50: 6520 6461 7461 2073 6574 2069 7320 656d  e data set is em
-00005d60: 7074 7922 2c0a 2020 2020 2020 2020 2020  pty",.          
-00005d70: 2020 2020 2020 4461 7461 4572 726f 722c        DataError,
-00005d80: 0a20 2020 2020 2020 2020 2020 2029 0a0a  .            )..
-00005d90: 2020 2020 2020 2020 6d61 7070 696e 6773          mappings
-00005da0: 203d 205b 636f 6c20 666f 7220 636f 6c20   = [col for col 
-00005db0: 696e 2061 7578 5f64 6174 615f 706f 696e  in aux_data_poin
-00005dc0: 7420 6966 2061 7578 5f64 6174 615f 706f  t if aux_data_po
-00005dd0: 696e 745b 636f 6c5d 2069 7320 6e6f 7420  int[col] is not 
-00005de0: 4e6f 6e65 5d0a 2020 2020 2020 2020 6466  None].        df
-00005df0: 2c20 736f 7274 203d 2061 6464 5f73 6f72  , sort = add_sor
-00005e00: 7469 6e67 5f74 6f5f 6466 2864 6629 2069  ting_to_df(df) i
-00005e10: 6620 226f 7264 6572 4669 656c 6431 2220  f "orderField1" 
-00005e20: 696e 206d 6170 7069 6e67 7320 656c 7365  in mappings else
-00005e30: 2028 6466 2c20 4e6f 6e65 290a 0a20 2020   (df, None)..   
-00005e40: 2020 2020 2063 6f6e 7665 7274 6564 5f64       converted_d
-00005e50: 6174 615f 706f 696e 7473 203d 2063 6f6e  ata_points = con
-00005e60: 7665 7274 5f69 6e70 7574 5f64 6174 615f  vert_input_data_
-00005e70: 746f 5f64 625f 6974 656d 7328 6466 2c20  to_db_items(df, 
-00005e80: 736f 7274 3d73 6f72 7429 0a20 2020 2020  sort=sort).     
-00005e90: 2020 2066 6f72 206d 6170 7069 6e67 2c20     for mapping, 
-00005ea0: 7620 696e 2063 6f6e 7665 7274 6564 5f64  v in converted_d
-00005eb0: 6174 615f 706f 696e 7473 5b30 5d2e 6974  ata_points[0].it
-00005ec0: 656d 7328 293a 0a20 2020 2020 2020 2020  ems():.         
-00005ed0: 2020 2069 6620 6d61 7070 696e 6720 6e6f     if mapping no
-00005ee0: 7420 696e 206d 6170 7069 6e67 733a 0a20  t in mappings:. 
-00005ef0: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-00005f00: 6f67 5f65 7272 6f72 280a 2020 2020 2020  og_error(.      
-00005f10: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
-00005f20: 6767 6572 2c0a 2020 2020 2020 2020 2020  gger,.          
-00005f30: 2020 2020 2020 2020 2020 6622 4361 6e6e            f"Cann
-00005f40: 6f74 2072 6575 7365 2064 6174 6120 7365  ot reuse data se
-00005f50: 7420 7b73 7472 2864 6174 615f 7365 7429  t {str(data_set)
-00005f60: 7d20 6265 6361 7573 6520 7468 6520 6461  } because the da
-00005f70: 7461 2070 726f 7669 6465 6420 220a 2020  ta provided ".  
-00005f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005f90: 2020 6622 6973 206e 6f74 2063 6f6e 7369    f"is not consi
-00005fa0: 7374 656e 7420 7769 7468 2074 6865 2064  stent with the d
-00005fb0: 6174 6120 7365 7422 2c0a 2020 2020 2020  ata set",.      
-00005fc0: 2020 2020 2020 2020 2020 2020 2020 4461                Da
-00005fd0: 7461 4572 726f 722c 0a20 2020 2020 2020  taError,.       
-00005fe0: 2020 2020 2020 2020 2029 0a0a 2020 2020           )..    
-00005ff0: 2020 2020 6669 7273 745f 6466 5f69 7465      first_df_ite
-00006000: 6d20 3d20 6466 2e69 6c6f 635b 305d 2e74  m = df.iloc[0].t
-00006010: 6f5f 6469 6374 2829 0a20 2020 2020 2020  o_dict().       
-00006020: 2072 6574 7572 6e20 7b0a 2020 2020 2020   return {.      
-00006030: 2020 2020 2020 636f 6c3a 2028 6d61 7070        col: (mapp
-00006040: 696e 672c 2064 6174 615f 7365 742c 2073  ing, data_set, s
-00006050: 6f72 7429 0a20 2020 2020 2020 2020 2020  ort).           
-00006060: 2066 6f72 2063 6f6c 2c20 6d61 7070 696e   for col, mappin
-00006070: 6720 696e 207a 6970 280a 2020 2020 2020  g in zip(.      
-00006080: 2020 2020 2020 2020 2020 6669 7273 745f            first_
-00006090: 6466 5f69 7465 6d2e 6b65 7973 2829 2c20  df_item.keys(), 
-000060a0: 636f 6e76 6572 7465 645f 6461 7461 5f70  converted_data_p
-000060b0: 6f69 6e74 735b 305d 2e6b 6579 7328 290a  oints[0].keys().
-000060c0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-000060d0: 2020 2020 2020 2020 2020 6966 2063 6f6c            if col
-000060e0: 2021 3d20 2273 6f72 745f 7661 6c75 6573   != "sort_values
-000060f0: 220a 2020 2020 2020 2020 7d0a 0a20 2020  ".        }..   
-00006100: 2061 7379 6e63 2064 6566 205f 6465 6c65   async def _dele
-00006110: 7465 5f64 6174 615f 7365 745f 6966 5f65  te_data_set_if_e
-00006120: 7869 7374 7328 7365 6c66 2c20 6461 7461  xists(self, data
-00006130: 5f73 6574 5f6e 616d 653a 2073 7472 2920  _set_name: str) 
-00006140: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
-00006150: 2022 2222 4465 6c65 7465 2074 6865 2064   """Delete the d
-00006160: 6174 6120 7365 7420 6966 2069 7420 6578  ata set if it ex
-00006170: 6973 7473 2e0a 2020 2020 2020 2020 3a70  ists..        :p
-00006180: 6172 616d 2064 6174 615f 7365 745f 6e61  aram data_set_na
-00006190: 6d65 3a20 7468 6520 6e61 6d65 206f 6620  me: the name of 
-000061a0: 7468 6520 6461 7461 2073 6574 0a20 2020  the data set.   
-000061b0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-000061c0: 2069 6620 6177 6169 7420 7365 6c66 2e5f   if await self._
-000061d0: 6170 702e 666f 7263 655f 6465 6c65 7465  app.force_delete
-000061e0: 5f64 6174 615f 7365 7428 6e61 6d65 3d64  _data_set(name=d
-000061f0: 6174 615f 7365 745f 6e61 6d65 293a 0a20  ata_set_name):. 
-00006200: 2020 2020 2020 2020 2020 206c 6f67 6765             logge
-00006210: 722e 696e 666f 2866 2244 656c 6574 6564  r.info(f"Deleted
-00006220: 2064 6174 6120 7365 7420 7769 7468 206e   data set with n
-00006230: 616d 6520 7b64 6174 615f 7365 745f 6e61  ame {data_set_na
-00006240: 6d65 7d22 290a 0a20 2020 2061 7379 6e63  me}")..    async
-00006250: 2064 6566 205f 6372 6561 7465 5f64 6174   def _create_dat
-00006260: 615f 7365 745f 6672 6f6d 5f64 6628 0a20  a_set_from_df(. 
-00006270: 2020 2020 2020 2073 656c 662c 2064 6174         self, dat
-00006280: 615f 7365 745f 6e61 6d65 3a20 7374 722c  a_set_name: str,
-00006290: 2064 663a 2070 642e 4461 7461 4672 616d   df: pd.DataFram
-000062a0: 652c 2073 6f72 743a 204f 7074 696f 6e61  e, sort: Optiona
-000062b0: 6c5b 6469 6374 5d20 3d20 4e6f 6e65 0a20  l[dict] = None. 
-000062c0: 2020 2029 202d 3e20 6469 6374 5b73 7472     ) -> dict[str
-000062d0: 2c20 7475 706c 655b 4d61 7070 696e 672c  , tuple[Mapping,
-000062e0: 2044 6174 6153 6574 2c20 6469 6374 5d5d   DataSet, dict]]
-000062f0: 3a0a 2020 2020 2020 2020 2222 2247 6574  :.        """Get
-00006300: 2074 6865 2064 6174 6120 6d61 7070 696e   the data mappin
-00006310: 6720 746f 2074 7570 6c65 2e0a 2020 2020  g to tuple..    
-00006320: 2020 2020 3a70 6172 616d 2064 663a 2074      :param df: t
-00006330: 6865 2064 6174 6120 6672 616d 650a 2020  he data frame.  
-00006340: 2020 2020 2020 3a72 6574 7572 6e3a 2074        :return: t
-00006350: 6865 2064 6174 6120 6d61 7070 696e 6720  he data mapping 
-00006360: 746f 2074 7570 6c65 0a20 2020 2020 2020  to tuple.       
-00006370: 2022 2222 0a20 2020 2020 2020 2064 662c   """.        df,
-00006380: 2073 6f72 7420 3d20 6164 645f 736f 7274   sort = add_sort
-00006390: 696e 675f 746f 5f64 6628 6466 2c20 736f  ing_to_df(df, so
-000063a0: 7274 290a 2020 2020 2020 2020 636f 6c75  rt).        colu
-000063b0: 6d6e 7320 3d20 6466 2e63 6f6c 756d 6e73  mns = df.columns
-000063c0: 2e74 6f6c 6973 7428 290a 2020 2020 2020  .tolist().      
-000063d0: 2020 6461 7461 5f6d 6170 7069 6e67 5f74    data_mapping_t
-000063e0: 6f5f 7475 706c 6520 3d20 7b7d 0a20 2020  o_tuple = {}.   
-000063f0: 2020 2020 2028 6d61 7070 696e 672c 2064       (mapping, d
-00006400: 6174 615f 7365 742c 2072 6573 5f73 6f72  ata_set, res_sor
-00006410: 7429 203d 2061 7761 6974 2073 656c 662e  t) = await self.
-00006420: 5f61 7070 2e61 7070 656e 645f 6461 7461  _app.append_data
-00006430: 5f74 6f5f 6461 7461 5f73 6574 280a 2020  _to_data_set(.  
-00006440: 2020 2020 2020 2020 2020 6e61 6d65 3d64            name=d
-00006450: 6174 615f 7365 745f 6e61 6d65 2c20 6461  ata_set_name, da
-00006460: 7461 3d64 662c 2073 6f72 743d 736f 7274  ta=df, sort=sort
-00006470: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
-00006480: 2020 206c 6f67 6765 722e 696e 666f 280a     logger.info(.
-00006490: 2020 2020 2020 2020 2020 2020 6627 4372              f'Cr
-000064a0: 6561 7465 6420 6461 7461 2073 6574 2077  eated data set w
-000064b0: 6974 6820 6964 207b 6461 7461 5f73 6574  ith id {data_set
-000064c0: 5b22 6964 225d 7d20 616e 6420 6e61 6d65  ["id"]} and name
-000064d0: 207b 6461 7461 5f73 6574 5f6e 616d 657d   {data_set_name}
-000064e0: 270a 2020 2020 2020 2020 290a 2020 2020  '.        ).    
-000064f0: 2020 2020 666f 7220 636f 6c2c 206d 6170      for col, map
-00006500: 5f76 616c 2069 6e20 7a69 7028 636f 6c75  _val in zip(colu
-00006510: 6d6e 732c 206d 6170 7069 6e67 293a 0a20  mns, mapping):. 
-00006520: 2020 2020 2020 2020 2020 2064 6174 615f             data_
-00006530: 6d61 7070 696e 675f 746f 5f74 7570 6c65  mapping_to_tuple
-00006540: 5b63 6f6c 5d20 3d20 286d 6170 5f76 616c  [col] = (map_val
-00006550: 2c20 6461 7461 5f73 6574 2c20 7265 735f  , data_set, res_
-00006560: 736f 7274 290a 2020 2020 2020 2020 7265  sort).        re
-00006570: 7475 726e 2064 6174 615f 6d61 7070 696e  turn data_mappin
-00006580: 675f 746f 5f74 7570 6c65 0a0a 2020 2020  g_to_tuple..    
-00006590: 6173 796e 6320 6465 6620 5f63 7265 6174  async def _creat
-000065a0: 655f 6475 6d70 6564 5f64 6174 615f 7365  e_dumped_data_se
-000065b0: 7428 0a20 2020 2020 2020 2073 656c 662c  t(.        self,
-000065c0: 2064 6174 615f 7365 745f 6e61 6d65 3a20   data_set_name: 
-000065d0: 7374 722c 2064 6174 613a 206c 6973 745b  str, data: list[
-000065e0: 6469 6374 5d0a 2020 2020 2920 2d3e 2064  dict].    ) -> d
-000065f0: 6963 743a 0a20 2020 2020 2020 2022 2222  ict:.        """
-00006600: 4765 7420 7468 6520 6d61 7070 696e 6720  Get the mapping 
-00006610: 6672 6f6d 2061 2064 6963 742e 0a20 2020  from a dict..   
-00006620: 2020 2020 203a 7061 7261 6d20 6461 7461       :param data
-00006630: 3a20 7468 6520 6461 7461 0a20 2020 2020  : the data.     
-00006640: 2020 203a 7265 7475 726e 3a20 7468 6520     :return: the 
-00006650: 6d61 7070 696e 6720 7475 706c 650a 2020  mapping tuple.  
-00006660: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00006670: 2020 6d61 7070 696e 672c 2064 6174 615f    mapping, data_
-00006680: 7365 742c 2073 6f72 7420 3d20 6177 6169  set, sort = awai
-00006690: 7420 7365 6c66 2e5f 6170 702e 6170 7065  t self._app.appe
-000066a0: 6e64 5f64 6174 615f 746f 5f64 6174 615f  nd_data_to_data_
-000066b0: 7365 7428 0a20 2020 2020 2020 2020 2020  set(.           
-000066c0: 206e 616d 653d 6461 7461 5f73 6574 5f6e   name=data_set_n
-000066d0: 616d 652c 2064 6174 613d 6461 7461 2c20  ame, data=data, 
-000066e0: 6475 6d70 5f77 686f 6c65 3d54 7275 650a  dump_whole=True.
-000066f0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00006700: 2020 6c6f 6767 6572 2e69 6e66 6f28 0a20    logger.info(. 
-00006710: 2020 2020 2020 2020 2020 2066 2743 7265             f'Cre
-00006720: 6174 6564 2064 6174 6120 7365 7420 7769  ated data set wi
-00006730: 7468 2069 6420 7b64 6174 615f 7365 745b  th id {data_set[
-00006740: 2269 6422 5d7d 2061 6e64 206e 616d 6520  "id"]} and name 
-00006750: 7b64 6174 615f 7365 745f 6e61 6d65 7d27  {data_set_name}'
-00006760: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
-00006770: 2020 2061 7373 6572 7420 6d61 7070 696e     assert mappin
-00006780: 675b 305d 203d 3d20 2263 7573 746f 6d46  g[0] == "customF
-00006790: 6965 6c64 3122 0a20 2020 2020 2020 2072  ield1".        r
-000067a0: 6574 7572 6e20 7b22 6461 7461 223a 2028  eturn {"data": (
-000067b0: 2263 7573 746f 6d46 6965 6c64 3122 2c20  "customField1", 
-000067c0: 6461 7461 5f73 6574 2c20 736f 7274 297d  data_set, sort)}
-000067d0: 0a0a 2020 2020 6173 796e 6320 6465 6620  ..    async def 
-000067e0: 5f63 7265 6174 655f 6461 7461 5f73 6574  _create_data_set
-000067f0: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
-00006800: 2020 2020 2020 2020 6e61 6d65 3a20 7374          name: st
-00006810: 722c 0a20 2020 2020 2020 2064 6174 613a  r,.        data:
-00006820: 2055 6e69 6f6e 5b6c 6973 745b 6469 6374   Union[list[dict
-00006830: 5d2c 2070 642e 4461 7461 4672 616d 652c  ], pd.DataFrame,
-00006840: 2064 6963 742c 2073 7472 5d2c 0a20 2020   dict, str],.   
-00006850: 2020 2020 2064 756d 705f 7768 6f6c 653a       dump_whole:
-00006860: 2062 6f6f 6c20 3d20 4661 6c73 652c 0a20   bool = False,. 
-00006870: 2020 2029 202d 3e20 6469 6374 5b73 7472     ) -> dict[str
-00006880: 2c20 7475 706c 655b 4d61 7070 696e 672c  , tuple[Mapping,
-00006890: 2044 6174 6153 6574 2c20 6469 6374 5d5d   DataSet, dict]]
-000068a0: 3a0a 2020 2020 2020 2020 2222 2253 6574  :.        """Set
-000068b0: 2061 2073 6861 7265 6420 6461 7461 2065   a shared data e
-000068c0: 6e74 7279 2e0a 2020 2020 2020 2020 3a70  ntry..        :p
-000068d0: 6172 616d 206e 616d 653a 2074 6865 206b  aram name: the k
-000068e0: 6579 206f 6620 7468 6520 7368 6172 6564  ey of the shared
-000068f0: 2064 6174 6120 656e 7472 790a 2020 2020   data entry.    
-00006900: 2020 2020 3a70 6172 616d 2064 6174 613a      :param data:
-00006910: 2074 6865 2076 616c 7565 206f 6620 7468   the value of th
-00006920: 6520 7368 6172 6564 2064 6174 6120 656e  e shared data en
-00006930: 7472 790a 2020 2020 2020 2020 3a70 6172  try.        :par
-00006940: 616d 2064 756d 705f 7768 6f6c 653a 2077  am dump_whole: w
-00006950: 6865 7468 6572 2074 6f20 6475 6d70 2074  hether to dump t
-00006960: 6865 2077 686f 6c65 2064 6174 6120 7365  he whole data se
-00006970: 740a 2020 2020 2020 2020 2222 220a 2020  t.        """.  
-00006980: 2020 2020 2020 6966 2073 656c 662e 7265        if self.re
-00006990: 7573 655f 6461 7461 5f73 6574 733a 0a20  use_data_sets:. 
-000069a0: 2020 2020 2020 2020 2020 2064 6174 615f             data_
-000069b0: 7365 7420 3d20 6177 6169 7420 7365 6c66  set = await self
-000069c0: 2e5f 6170 702e 6765 745f 6461 7461 5f73  ._app.get_data_s
-000069d0: 6574 280a 2020 2020 2020 2020 2020 2020  et(.            
-000069e0: 2020 2020 6e61 6d65 3d6e 616d 652c 2063      name=name, c
-000069f0: 7265 6174 655f 6966 5f6e 6f74 5f65 7869  reate_if_not_exi
-00006a00: 7374 733d 4661 6c73 650a 2020 2020 2020  sts=False.      
-00006a10: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-00006a20: 2020 2020 6966 2064 6174 615f 7365 743a      if data_set:
-00006a30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006a40: 2072 6574 7572 6e20 280a 2020 2020 2020   return (.      
-00006a50: 2020 2020 2020 2020 2020 2020 2020 6177                aw
-00006a60: 6169 7420 7365 6c66 2e5f 7472 795f 746f  ait self._try_to
-00006a70: 5f72 6575 7365 5f64 6174 6128 6461 7461  _reuse_data(data
-00006a80: 5f73 6574 2c20 6461 7461 290a 2020 2020  _set, data).    
-00006a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006aa0: 6966 206e 6f74 2064 756d 705f 7768 6f6c  if not dump_whol
-00006ab0: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
-00006ac0: 2020 2020 2020 656c 7365 207b 2264 6174        else {"dat
-00006ad0: 6122 3a20 2822 6375 7374 6f6d 4669 656c  a": ("customFiel
-00006ae0: 6431 222c 2064 6174 615f 7365 742c 207b  d1", data_set, {
-00006af0: 7d29 7d0a 2020 2020 2020 2020 2020 2020  })}.            
-00006b00: 2020 2020 290a 0a20 2020 2020 2020 2061      )..        a
-00006b10: 7761 6974 2073 656c 662e 5f64 656c 6574  wait self._delet
-00006b20: 655f 6461 7461 5f73 6574 5f69 665f 6578  e_data_set_if_ex
-00006b30: 6973 7473 2864 6174 615f 7365 745f 6e61  ists(data_set_na
-00006b40: 6d65 3d6e 616d 6529 0a0a 2020 2020 2020  me=name)..      
-00006b50: 2020 6966 2064 756d 705f 7768 6f6c 653a    if dump_whole:
-00006b60: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00006b70: 7572 6e20 6177 6169 7420 7365 6c66 2e5f  urn await self._
-00006b80: 6372 6561 7465 5f64 756d 7065 645f 6461  create_dumped_da
-00006b90: 7461 5f73 6574 286e 616d 652c 2064 6174  ta_set(name, dat
-00006ba0: 6129 0a0a 2020 2020 2020 2020 7265 7475  a)..        retu
-00006bb0: 726e 2061 7761 6974 2073 656c 662e 5f63  rn await self._c
-00006bc0: 7265 6174 655f 6461 7461 5f73 6574 5f66  reate_data_set_f
-00006bd0: 726f 6d5f 6466 286e 616d 652c 2044 6174  rom_df(name, Dat
-00006be0: 6146 7261 6d65 2864 6174 6129 290a 0a20  aFrame(data)).. 
-00006bf0: 2020 2061 7379 6e63 2064 6566 205f 7365     async def _se
-00006c00: 745f 7368 6172 6564 5f64 6174 615f 656e  t_shared_data_en
-00006c10: 7472 7928 0a20 2020 2020 2020 2073 656c  try(.        sel
-00006c20: 662c 0a20 2020 2020 2020 206e 616d 653a  f,.        name:
-00006c30: 2073 7472 2c0a 2020 2020 2020 2020 6461   str,.        da
-00006c40: 7461 3a20 556e 696f 6e5b 6c69 7374 5b64  ta: Union[list[d
-00006c50: 6963 745d 2c20 7064 2e44 6174 6146 7261  ict], pd.DataFra
-00006c60: 6d65 2c20 6469 6374 2c20 7374 725d 2c0a  me, dict, str],.
-00006c70: 2020 2020 2020 2020 6475 6d70 5f77 686f          dump_who
-00006c80: 6c65 3a20 626f 6f6c 203d 2046 616c 7365  le: bool = False
-00006c90: 2c0a 2020 2020 293a 0a20 2020 2020 2020  ,.    ):.       
-00006ca0: 2022 2222 0a20 2020 2020 2020 2053 6574   """.        Set
-00006cb0: 2061 2073 6861 7265 6420 6461 7461 2065   a shared data e
-00006cc0: 6e74 7279 2e0a 2020 2020 2020 2020 3a70  ntry..        :p
-00006cd0: 6172 616d 206e 616d 653a 2074 6865 206b  aram name: the k
-00006ce0: 6579 206f 6620 7468 6520 7368 6172 6564  ey of the shared
-00006cf0: 2064 6174 6120 656e 7472 790a 2020 2020   data entry.    
-00006d00: 2020 2020 3a70 6172 616d 2064 6174 613a      :param data:
-00006d10: 2074 6865 2076 616c 7565 206f 6620 7468   the value of th
-00006d20: 6520 7368 6172 6564 2064 6174 6120 656e  e shared data en
-00006d30: 7472 790a 2020 2020 2020 2020 3a70 6172  try.        :par
-00006d40: 616d 2064 756d 705f 7768 6f6c 653a 2077  am dump_whole: w
-00006d50: 6865 7468 6572 2074 6f20 6475 6d70 2074  hether to dump t
-00006d60: 6865 2077 686f 6c65 2064 6174 6120 7365  he whole data se
-00006d70: 740a 2020 2020 2020 2020 2222 220a 2020  t.        """.  
-00006d80: 2020 2020 2020 6966 206e 616d 6520 696e        if name in
-00006d90: 2073 656c 662e 5f73 6861 7265 645f 6461   self._shared_da
-00006da0: 7461 5f6d 6170 3a0a 2020 2020 2020 2020  ta_map:.        
-00006db0: 2020 2020 6c6f 675f 6572 726f 7228 0a20      log_error(. 
-00006dc0: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-00006dd0: 6f67 6765 722c 0a20 2020 2020 2020 2020  ogger,.         
-00006de0: 2020 2020 2020 2066 2243 616e 6e6f 7420         f"Cannot 
-00006df0: 7365 7420 7368 6172 6564 2064 6174 6120  set shared data 
-00006e00: 656e 7472 7920 7b6e 616d 657d 2062 6563  entry {name} bec
-00006e10: 6175 7365 2069 7420 616c 7265 6164 7920  ause it already 
-00006e20: 6578 6973 7473 222c 0a20 2020 2020 2020  exists",.       
-00006e30: 2020 2020 2020 2020 2044 6174 6145 7272           DataErr
-00006e40: 6f72 2c0a 2020 2020 2020 2020 2020 2020  or,.            
-00006e50: 290a 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00006e60: 5f73 6861 7265 645f 6461 7461 5f6d 6170  _shared_data_map
-00006e70: 5b6e 616d 655d 203d 2061 7761 6974 2073  [name] = await s
-00006e80: 656c 662e 5f63 7265 6174 655f 6461 7461  elf._create_data
-00006e90: 5f73 6574 280a 2020 2020 2020 2020 2020  _set(.          
-00006ea0: 2020 6e61 6d65 2c20 6461 7461 2c20 6475    name, data, du
-00006eb0: 6d70 5f77 686f 6c65 0a20 2020 2020 2020  mp_whole.       
-00006ec0: 2029 0a20 2020 2020 2020 2073 656c 662e   ).        self.
-00006ed0: 5f73 6861 7265 645f 6461 7461 5b6e 616d  _shared_data[nam
-00006ee0: 655d 203d 2064 6174 610a 0a20 2020 2061  e] = data..    a
-00006ef0: 7379 6e63 2064 6566 2073 6574 5f73 6861  sync def set_sha
-00006f00: 7265 645f 6461 7461 280a 2020 2020 2020  red_data(.      
-00006f10: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
-00006f20: 6466 733a 2064 6963 745b 7374 722c 2055  dfs: dict[str, U
-00006f30: 6e69 6f6e 5b6c 6973 745b 6469 6374 5d2c  nion[list[dict],
-00006f40: 2070 642e 4461 7461 4672 616d 655d 5d20   pd.DataFrame]] 
-00006f50: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-00006f60: 6375 7374 6f6d 5f64 6174 613a 2064 6963  custom_data: dic
-00006f70: 745b 7374 722c 2061 6e79 5d20 3d20 4e6f  t[str, any] = No
-00006f80: 6e65 2c0a 2020 2020 293a 0a20 2020 2020  ne,.    ):.     
-00006f90: 2020 2022 2222 0a20 2020 2020 2020 2053     """.        S
-00006fa0: 6574 2073 6861 7265 6420 6461 7461 2066  et shared data f
-00006fb0: 6f72 2074 6865 2073 2e70 6c74 2074 6f20  or the s.plt to 
-00006fc0: 7573 652e 0a20 2020 2020 2020 203a 7061  use..        :pa
-00006fd0: 7261 6d20 6466 733a 2074 6865 2064 6174  ram dfs: the dat
-00006fe0: 6120 6672 616d 6573 0a20 2020 2020 2020  a frames.       
-00006ff0: 203a 7061 7261 6d20 6375 7374 6f6d 5f64   :param custom_d
-00007000: 6174 613a 2074 6865 2063 7573 746f 6d20  ata: the custom 
-00007010: 6461 7461 0a20 2020 2020 2020 2022 2222  data.        """
-00007020: 0a20 2020 2020 2020 2074 6173 6b73 203d  .        tasks =
-00007030: 205b 5d0a 2020 2020 2020 2020 666f 7220   [].        for 
-00007040: 6b2c 2064 6620 696e 2028 6466 7320 6966  k, df in (dfs if
-00007050: 2064 6673 2065 6c73 6520 7b7d 292e 6974   dfs else {}).it
-00007060: 656d 7328 293a 0a20 2020 2020 2020 2020  ems():.         
-00007070: 2020 2074 6173 6b73 2e61 7070 656e 6428     tasks.append(
-00007080: 7365 6c66 2e5f 7365 745f 7368 6172 6564  self._set_shared
-00007090: 5f64 6174 615f 656e 7472 7928 6b2c 2064  _data_entry(k, d
-000070a0: 6629 290a 2020 2020 2020 2020 666f 7220  f)).        for 
-000070b0: 6b2c 2076 2069 6e20 2863 7573 746f 6d5f  k, v in (custom_
-000070c0: 6461 7461 2069 6620 6375 7374 6f6d 5f64  data if custom_d
-000070d0: 6174 6120 656c 7365 207b 7d29 2e69 7465  ata else {}).ite
-000070e0: 6d73 2829 3a0a 2020 2020 2020 2020 2020  ms():.          
-000070f0: 2020 7461 736b 732e 6170 7065 6e64 2873    tasks.append(s
-00007100: 656c 662e 5f73 6574 5f73 6861 7265 645f  elf._set_shared_
-00007110: 6461 7461 5f65 6e74 7279 286b 2c20 762c  data_entry(k, v,
-00007120: 2064 756d 705f 7768 6f6c 653d 5472 7565   dump_whole=True
-00007130: 2929 0a20 2020 2020 2020 2069 6620 7461  )).        if ta
-00007140: 736b 733a 0a20 2020 2020 2020 2020 2020  sks:.           
-00007150: 2061 7761 6974 2061 7379 6e63 696f 2e67   await asyncio.g
-00007160: 6174 6865 7228 2a74 6173 6b73 290a 2020  ather(*tasks).  
-00007170: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-00007180: 2020 2020 2020 2020 6c6f 675f 6572 726f          log_erro
-00007190: 7228 6c6f 6767 6572 2c20 224e 6f20 6461  r(logger, "No da
-000071a0: 7461 2070 726f 7669 6465 6422 2c20 4461  ta provided", Da
-000071b0: 7461 4572 726f 7229 0a0a 2020 2020 6173  taError)..    as
-000071c0: 796e 6320 6465 6620 5f63 686f 6f73 655f  ync def _choose_
-000071d0: 6461 7461 280a 2020 2020 2020 2020 7365  data(.        se
-000071e0: 6c66 2c0a 2020 2020 2020 2020 6f72 6465  lf,.        orde
-000071f0: 723a 2069 6e74 2c0a 2020 2020 2020 2020  r: int,.        
-00007200: 6461 7461 3a20 556e 696f 6e5b 6c69 7374  data: Union[list
-00007210: 5b64 6963 745d 2c20 7064 2e44 6174 6146  [dict], pd.DataF
-00007220: 7261 6d65 2c20 6469 6374 2c20 7374 725d  rame, dict, str]
-00007230: 2c0a 2020 2020 2020 2020 6368 6172 745f  ,.        chart_
-00007240: 636c 6173 733a 2074 7970 655b 5265 706f  class: type[Repo
-00007250: 7274 5d20 3d20 4543 6861 7274 2c0a 2020  rt] = EChart,.  
-00007260: 2020 2020 2020 6475 6d70 5f77 686f 6c65        dump_whole
-00007270: 3a20 626f 6f6c 203d 2046 616c 7365 2c0a  : bool = False,.
-00007280: 2020 2020 2920 2d3e 2064 6963 745b 7374      ) -> dict[st
-00007290: 722c 2074 7570 6c65 5b4d 6170 7069 6e67  r, tuple[Mapping
-000072a0: 2c20 4461 7461 5365 742c 2064 6963 745d  , DataSet, dict]
-000072b0: 5d3a 0a20 2020 2020 2020 2022 2222 4765  ]:.        """Ge
-000072c0: 7420 7468 6520 6461 7461 206d 6170 7069  t the data mappi
-000072d0: 6e67 7320 6f66 2074 6865 2064 6174 612e  ngs of the data.
-000072e0: 2049 6620 7468 6520 6461 7461 2069 7320   If the data is 
-000072f0: 6120 7374 7269 6e67 2c20 6974 2069 7320  a string, it is 
-00007300: 6173 7375 6d65 6420 746f 2062 6520 6120  assumed to be a 
-00007310: 7368 6172 6564 2064 6174 6120 656e 7472  shared data entr
-00007320: 792e 0a20 2020 2020 2020 203a 7061 7261  y..        :para
-00007330: 6d20 6f72 6465 723a 2074 6865 206f 7264  m order: the ord
-00007340: 6572 206f 6620 7468 6520 6368 6172 740a  er of the chart.
-00007350: 2020 2020 2020 2020 3a70 6172 616d 2064          :param d
-00007360: 6174 613a 2074 6865 2064 6174 610a 2020  ata: the data.  
-00007370: 2020 2020 2020 3a70 6172 616d 2064 756d        :param dum
-00007380: 705f 7768 6f6c 653a 2077 6865 7468 6572  p_whole: whether
-00007390: 2074 6f20 6475 6d70 2074 6865 2077 686f   to dump the who
-000073a0: 6c65 2064 6174 6120 7365 740a 2020 2020  le data set.    
-000073b0: 2020 2020 3a72 6574 7572 6e3a 2074 6865      :return: the
-000073c0: 2064 6174 6120 6d61 7070 696e 6773 0a20   data mappings. 
-000073d0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-000073e0: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
-000073f0: 2864 6174 612c 2073 7472 293a 0a20 2020  (data, str):.   
-00007400: 2020 2020 2020 2020 2069 6620 6461 7461           if data
-00007410: 206e 6f74 2069 6e20 7365 6c66 2e5f 7368   not in self._sh
-00007420: 6172 6564 5f64 6174 615f 6d61 703a 0a20  ared_data_map:. 
-00007430: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-00007440: 6f67 5f65 7272 6f72 286c 6f67 6765 722c  og_error(logger,
-00007450: 2066 224e 6f20 7368 6172 6564 2064 6174   f"No shared dat
-00007460: 6120 7769 7468 206e 616d 6520 7b64 6174  a with name {dat
-00007470: 617d 2066 6f75 6e64 222c 2044 6174 6145  a} found", DataE
-00007480: 7272 6f72 290a 2020 2020 2020 2020 2020  rror).          
-00007490: 2020 7265 7475 726e 2073 656c 662e 5f73    return self._s
-000074a0: 6861 7265 645f 6461 7461 5f6d 6170 5b64  hared_data_map[d
-000074b0: 6174 615d 0a0a 2020 2020 2020 2020 5f2c  ata]..        _,
-000074c0: 2072 6570 6f72 7420 3d20 6177 6169 7420   report = await 
-000074d0: 7365 6c66 2e5f 6765 745f 6368 6172 745f  self._get_chart_
-000074e0: 7265 706f 7274 286f 7264 6572 2c20 6368  report(order, ch
-000074f0: 6172 745f 636c 6173 7329 0a20 2020 2020  art_class).     
-00007500: 2020 206e 616d 6520 3d20 7265 706f 7274     name = report
-00007510: 5b22 6964 225d 0a0a 2020 2020 2020 2020  ["id"]..        
-00007520: 7265 7475 726e 2061 7761 6974 2073 656c  return await sel
-00007530: 662e 5f63 7265 6174 655f 6461 7461 5f73  f._create_data_s
-00007540: 6574 286e 616d 652c 2064 6174 612c 2064  et(name, data, d
-00007550: 756d 705f 7768 6f6c 6529 0a0a 2020 2020  ump_whole)..    
-00007560: 6173 796e 6320 6465 6620 5f63 6865 636b  async def _check
-00007570: 5f70 7265 7669 6f75 735f 7061 7468 7328  _previous_paths(
-00007580: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
-00007590: 2222 4368 6563 6b20 6966 2074 6865 7265  ""Check if there
-000075a0: 2061 7265 2070 6174 6873 2074 6861 7420   are paths that 
-000075b0: 6861 7665 206e 6f74 2062 6565 6e20 6578  have not been ex
-000075c0: 6563 7574 6564 2079 6574 2e22 2222 0a20  ecuted yet.""". 
-000075d0: 2020 2020 2020 2070 6174 6873 5f69 6e5f         paths_in_
-000075e0: 6f72 6465 7220 3d20 6177 6169 7420 7365  order = await se
-000075f0: 6c66 2e5f 6170 702e 6765 745f 7061 7468  lf._app.get_path
-00007600: 735f 696e 5f6f 7264 6572 2829 0a20 2020  s_in_order().   
-00007610: 2020 2020 206e 6f74 5f65 7865 6375 7465       not_execute
-00007620: 645f 7061 7468 7320 3d20 5b0a 2020 2020  d_paths = [.    
-00007630: 2020 2020 2020 2020 7020 666f 7220 7020          p for p 
-00007640: 696e 2070 6174 6873 5f69 6e5f 6f72 6465  in paths_in_orde
-00007650: 7220 6966 2070 206e 6f74 2069 6e20 7365  r if p not in se
-00007660: 6c66 2e5f 6578 6563 7574 696f 6e5f 7061  lf._execution_pa
-00007670: 7468 5f6f 7264 6572 730a 2020 2020 2020  th_orders.      
-00007680: 2020 5d0a 2020 2020 2020 2020 6966 206c    ].        if l
-00007690: 656e 286e 6f74 5f65 7865 6375 7465 645f  en(not_executed_
-000076a0: 7061 7468 7329 203e 2030 3a0a 2020 2020  paths) > 0:.    
-000076b0: 2020 2020 2020 2020 6e6f 745f 7570 6c6f          not_uplo
-000076c0: 6164 6564 5f70 6174 6873 203d 205b 0a20  aded_paths = [. 
-000076d0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-000076e0: 2066 6f72 2070 2069 6e20 7365 6c66 2e5f   for p in self._
-000076f0: 6578 6563 7574 696f 6e5f 7061 7468 5f6f  execution_path_o
-00007700: 7264 6572 7320 6966 2070 206e 6f74 2069  rders if p not i
-00007710: 6e20 7061 7468 735f 696e 5f6f 7264 6572  n paths_in_order
-00007720: 0a20 2020 2020 2020 2020 2020 205d 0a20  .            ]. 
-00007730: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00007740: 5f65 7865 6375 7469 6f6e 5f70 6174 685f  _execution_path_
-00007750: 6f72 6465 7273 2e63 6c65 6172 2829 0a20  orders.clear(). 
-00007760: 2020 2020 2020 2020 2020 2066 6f72 2070             for p
-00007770: 2069 6e20 7061 7468 735f 696e 5f6f 7264   in paths_in_ord
-00007780: 6572 202b 206e 6f74 5f75 706c 6f61 6465  er + not_uploade
-00007790: 645f 7061 7468 733a 0a20 2020 2020 2020  d_paths:.       
-000077a0: 2020 2020 2020 2020 2073 656c 662e 5f65           self._e
-000077b0: 7865 6375 7469 6f6e 5f70 6174 685f 6f72  xecution_path_or
-000077c0: 6465 7273 2e61 7070 656e 6428 7029 0a0a  ders.append(p)..
-000077d0: 2020 2020 6173 796e 6320 6465 6620 5f63      async def _c
-000077e0: 7265 6174 655f 6368 6172 7428 0a20 2020  reate_chart(.   
-000077f0: 2020 2020 2073 656c 662c 2063 6861 7274       self, chart
-00007800: 5f63 6c61 7373 3a20 7479 7065 5b52 6570  _class: type[Rep
-00007810: 6f72 745d 2c20 6f72 6465 723a 2069 6e74  ort], order: int
-00007820: 2c20 2a2a 7061 7261 6d73 0a20 2020 2029  , **params.    )
-00007830: 202d 3e20 5265 706f 7274 3a0a 2020 2020   -> Report:.    
-00007840: 2020 2020 2222 2243 7265 6174 6520 6120      """Create a 
-00007850: 6368 6172 7420 616e 6420 6164 6420 6974  chart and add it
-00007860: 2074 6f20 7468 6520 6375 7272 656e 7420   to the current 
-00007870: 7461 6273 2067 726f 7570 206f 7220 6d6f  tabs group or mo
-00007880: 6461 6c2e 0a20 2020 2020 2020 203a 7061  dal..        :pa
-00007890: 7261 6d20 6368 6172 745f 636c 6173 733a  ram chart_class:
-000078a0: 2074 6865 2063 6c61 7373 206f 6620 7468   the class of th
-000078b0: 6520 6368 6172 740a 2020 2020 2020 2020  e chart.        
-000078c0: 3a70 6172 616d 206f 7264 6572 3a20 7468  :param order: th
-000078d0: 6520 6f72 6465 7220 6f66 2074 6865 2063  e order of the c
-000078e0: 6861 7274 2069 6e20 7468 6520 6461 7368  hart in the dash
-000078f0: 626f 6172 640a 2020 2020 2020 2020 3a70  board.        :p
-00007900: 6172 616d 2070 6172 616d 733a 2074 6865  aram params: the
-00007910: 2061 7267 756d 656e 7473 206f 6620 7468   arguments of th
-00007920: 6520 6368 6172 740a 2020 2020 2020 2020  e chart.        
-00007930: 2222 220a 2020 2020 2020 2020 6966 2022  """.        if "
-00007940: 6c6f 6767 696e 675f 6675 6e63 5f6e 616d  logging_func_nam
-00007950: 6522 2069 6e20 7061 7261 6d73 3a0a 2020  e" in params:.  
-00007960: 2020 2020 2020 2020 2020 6465 6c20 7061            del pa
-00007970: 7261 6d73 5b22 6c6f 6767 696e 675f 6675  rams["logging_fu
-00007980: 6e63 5f6e 616d 6522 5d0a 0a20 2020 2020  nc_name"]..     
-00007990: 2020 2069 6620 6e6f 7420 7061 7261 6d73     if not params
-000079a0: 2e67 6574 2822 7469 746c 6522 293a 0a20  .get("title"):. 
-000079b0: 2020 2020 2020 2020 2020 2070 6172 616d             param
-000079c0: 735b 2274 6974 6c65 225d 203d 2022 220a  s["title"] = "".
-000079d0: 2020 2020 2020 2020 6966 206e 6f74 2070          if not p
-000079e0: 6172 616d 732e 6765 7428 2273 697a 6552  arams.get("sizeR
-000079f0: 6f77 7322 293a 0a20 2020 2020 2020 2020  ows"):.         
-00007a00: 2020 2070 6172 616d 735b 2273 697a 6552     params["sizeR
-00007a10: 6f77 7322 5d20 3d20 330a 2020 2020 2020  ows"] = 3.      
-00007a20: 2020 6966 206e 6f74 2070 6172 616d 732e    if not params.
-00007a30: 6765 7428 2273 697a 6543 6f6c 756d 6e73  get("sizeColumns
-00007a40: 2229 3a0a 2020 2020 2020 2020 2020 2020  "):.            
-00007a50: 7061 7261 6d73 5b22 7369 7a65 436f 6c75  params["sizeColu
-00007a60: 6d6e 7322 5d20 3d20 3132 0a20 2020 2020  mns"] = 12.     
-00007a70: 2020 2069 6620 6e6f 7420 7061 7261 6d73     if not params
-00007a80: 2e67 6574 2822 7369 7a65 5061 6464 696e  .get("sizePaddin
-00007a90: 6722 293a 0a20 2020 2020 2020 2020 2020  g"):.           
-00007aa0: 2070 6172 616d 735b 2273 697a 6550 6164   params["sizePad
-00007ab0: 6469 6e67 225d 203d 2022 302c 302c 302c  ding"] = "0,0,0,
-00007ac0: 3022 0a0a 2020 2020 2020 2020 7061 7261  0"..        para
-00007ad0: 6d73 5b22 6265 6e74 6f62 6f78 225d 203d  ms["bentobox"] =
-00007ae0: 2073 656c 662e 5f67 6574 5f62 656e 746f   self._get_bento
-00007af0: 626f 785f 6461 7461 286f 7264 6572 3d6f  box_data(order=o
-00007b00: 7264 6572 290a 2020 2020 2020 2020 7061  rder).        pa
-00007b10: 7261 6d73 5b22 7061 7468 225d 203d 2073  rams["path"] = s
-00007b20: 656c 662e 5f63 7572 7265 6e74 5f70 6174  elf._current_pat
-00007b30: 680a 0a20 2020 2020 2020 2069 6620 6861  h..        if ha
-00007b40: 7361 7474 7228 7365 6c66 2c20 2263 6f64  sattr(self, "cod
-00007b50: 655f 6765 6e65 7261 7469 6f6e 5f6d 6574  e_generation_met
-00007b60: 6164 6174 6122 293a 0a20 2020 2020 2020  adata"):.       
-00007b70: 2020 2020 2069 6620 2270 726f 7065 7274       if "propert
-00007b80: 6965 7322 206e 6f74 2069 6e20 7061 7261  ies" not in para
-00007b90: 6d73 3a0a 2020 2020 2020 2020 2020 2020  ms:.            
-00007ba0: 2020 2020 7061 7261 6d73 5b22 7072 6f70      params["prop
-00007bb0: 6572 7469 6573 225d 203d 207b 7d0a 2020  erties"] = {}.  
-00007bc0: 2020 2020 2020 2020 2020 7061 7261 6d73            params
-00007bd0: 5b22 7072 6f70 6572 7469 6573 225d 5b22  ["properties"]["
-00007be0: 636f 6465 5f67 656e 6572 6174 696f 6e5f  code_generation_
-00007bf0: 6d65 7461 6461 7461 225d 203d 2067 6574  metadata"] = get
-00007c00: 6174 7472 280a 2020 2020 2020 2020 2020  attr(.          
-00007c10: 2020 2020 2020 7365 6c66 2c20 2263 6f64        self, "cod
-00007c20: 655f 6765 6e65 7261 7469 6f6e 5f6d 6574  e_generation_met
-00007c30: 6164 6174 6122 0a20 2020 2020 2020 2020  adata".         
-00007c40: 2020 2029 0a0a 2020 2020 2020 2020 6576     )..        ev
-00007c50: 656e 745f 7479 7065 3a20 4576 656e 7454  ent_type: EventT
-00007c60: 7970 6520 3d20 4576 656e 7454 7970 652e  ype = EventType.
-00007c70: 5245 504f 5254 5f55 5044 4154 4544 0a20  REPORT_UPDATED. 
-00007c80: 2020 2020 2020 2072 5f68 6173 682c 2063         r_hash, c
-00007c90: 6861 7274 203d 2061 7761 6974 2073 656c  hart = await sel
-00007ca0: 662e 5f67 6574 5f63 6861 7274 5f72 6570  f._get_chart_rep
-00007cb0: 6f72 7428 0a20 2020 2020 2020 2020 2020  ort(.           
-00007cc0: 206f 7264 6572 2c20 6368 6172 745f 636c   order, chart_cl
-00007cd0: 6173 732c 2063 7265 6174 655f 6966 5f6e  ass, create_if_n
-00007ce0: 6f74 5f65 7869 7374 733d 4661 6c73 650a  ot_exists=False.
-00007cf0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00007d00: 2020 6966 2063 6861 7274 3a0a 2020 2020    if chart:.    
-00007d10: 2020 2020 2020 2020 7061 7261 6d73 5b22          params["
-00007d20: 7061 7468 4f72 6465 7222 5d20 3d20 6368  pathOrder"] = ch
-00007d30: 6172 745b 2270 6174 684f 7264 6572 225d  art["pathOrder"]
-00007d40: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00007d50: 7365 6c66 2e5f 6375 7272 656e 745f 7061  self._current_pa
-00007d60: 7468 2061 6e64 2070 6172 616d 735b 2270  th and params["p
-00007d70: 6174 684f 7264 6572 225d 2069 7320 4e6f  athOrder"] is No
-00007d80: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00007d90: 2020 2020 6177 6169 7420 7365 6c66 2e5f      await self._
-00007da0: 6368 6563 6b5f 7072 6576 696f 7573 5f70  check_previous_p
-00007db0: 6174 6873 2829 0a20 2020 2020 2020 2020  aths().         
-00007dc0: 2020 2020 2020 2070 6172 616d 735b 2270         params["p
-00007dd0: 6174 684f 7264 6572 225d 203d 2073 656c  athOrder"] = sel
-00007de0: 662e 5f65 7865 6375 7469 6f6e 5f70 6174  f._execution_pat
-00007df0: 685f 6f72 6465 7273 2e69 6e64 6578 280a  h_orders.index(.
-00007e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007e10: 2020 2020 7365 6c66 2e5f 6375 7272 656e      self._curren
-00007e20: 745f 7061 7468 0a20 2020 2020 2020 2020  t_path.         
-00007e30: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-00007e40: 2020 2020 2069 6620 6368 6172 7420 213d       if chart !=
-00007e50: 2073 656c 662e 5f61 7070 2e6d 6f63 6b5f   self._app.mock_
-00007e60: 6372 6561 7465 5f72 6570 6f72 7428 0a20  create_report(. 
-00007e70: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00007e80: 6861 7274 5f63 6c61 7373 2c20 725f 6861  hart_class, r_ha
-00007e90: 7368 3d72 5f68 6173 682c 206f 7264 6572  sh=r_hash, order
-00007ea0: 3d6f 7264 6572 2c20 2a2a 7061 7261 6d73  =order, **params
-00007eb0: 0a20 2020 2020 2020 2020 2020 2029 3a0a  .            ):.
-00007ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007ed0: 6177 6169 7420 7365 6c66 2e5f 6170 702e  await self._app.
-00007ee0: 7570 6461 7465 5f72 6570 6f72 7428 725f  update_report(r_
-00007ef0: 6861 7368 3d72 5f68 6173 682c 202a 2a70  hash=r_hash, **p
-00007f00: 6172 616d 7329 0a20 2020 2020 2020 2020  arams).         
-00007f10: 2020 2020 2020 206c 6f67 6765 722e 696e         logger.in
-00007f20: 666f 2866 2255 7064 6174 6564 207b 6368  fo(f"Updated {ch
-00007f30: 6172 745f 636c 6173 732e 5f5f 6e61 6d65  art_class.__name
-00007f40: 5f5f 7d20 6174 207b 7374 7228 6368 6172  __} at {str(char
-00007f50: 7429 7d22 290a 2020 2020 2020 2020 2020  t)}").          
-00007f60: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00007f70: 2020 2020 2020 2020 6c6f 6767 6572 2e69          logger.i
-00007f80: 6e66 6f28 0a20 2020 2020 2020 2020 2020  nfo(.           
-00007f90: 2020 2020 2020 2020 2066 224e 6f20 6368           f"No ch
-00007fa0: 616e 6765 7320 6e65 6564 6564 2066 6f72  anges needed for
-00007fb0: 207b 6368 6172 745f 636c 6173 732e 5f5f   {chart_class.__
-00007fc0: 6e61 6d65 5f5f 7d20 6174 207b 7374 7228  name__} at {str(
-00007fd0: 6368 6172 7429 7d22 0a20 2020 2020 2020  chart)}".       
-00007fe0: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-00007ff0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00008000: 6e20 6368 6172 740a 2020 2020 2020 2020  n chart.        
-00008010: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-00008020: 2020 6576 656e 745f 7479 7065 3a20 4576    event_type: Ev
-00008030: 656e 7454 7970 6520 3d20 4576 656e 7454  entType = EventT
-00008040: 7970 652e 5245 504f 5254 5f43 5245 4154  ype.REPORT_CREAT
-00008050: 4544 0a20 2020 2020 2020 2020 2020 2061  ED.            a
-00008060: 7761 6974 2073 656c 662e 5f63 6865 636b  wait self._check
-00008070: 5f70 7265 7669 6f75 735f 7061 7468 7328  _previous_paths(
-00008080: 290a 2020 2020 2020 2020 2020 2020 7061  ).            pa
-00008090: 7261 6d73 5b22 7061 7468 4f72 6465 7222  rams["pathOrder"
-000080a0: 5d20 3d20 280a 2020 2020 2020 2020 2020  ] = (.          
-000080b0: 2020 2020 2020 7365 6c66 2e5f 6578 6563        self._exec
-000080c0: 7574 696f 6e5f 7061 7468 5f6f 7264 6572  ution_path_order
-000080d0: 732e 696e 6465 7828 7365 6c66 2e5f 6375  s.index(self._cu
-000080e0: 7272 656e 745f 7061 7468 290a 2020 2020  rrent_path).    
-000080f0: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-00008100: 656c 662e 5f63 7572 7265 6e74 5f70 6174  elf._current_pat
-00008110: 680a 2020 2020 2020 2020 2020 2020 2020  h.              
-00008120: 2020 656c 7365 204e 6f6e 650a 2020 2020    else None.    
-00008130: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00008140: 2020 2020 2020 7061 7261 6d73 5b22 6f72        params["or
-00008150: 6465 7222 5d20 3d20 6f72 6465 720a 2020  der"] = order.  
-00008160: 2020 2020 2020 2020 2020 6368 6172 743a            chart:
-00008170: 2052 6570 6f72 7420 3d20 6177 6169 7420   Report = await 
-00008180: 7365 6c66 2e5f 6170 702e 6372 6561 7465  self._app.create
-00008190: 5f72 6570 6f72 7428 0a20 2020 2020 2020  _report(.       
-000081a0: 2020 2020 2020 2020 2063 6861 7274 5f63           chart_c
-000081b0: 6c61 7373 2c20 725f 6861 7368 3d72 5f68  lass, r_hash=r_h
-000081c0: 6173 682c 202a 2a70 6172 616d 730a 2020  ash, **params.  
-000081d0: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-000081e0: 2020 2020 2020 2020 6c6f 6767 6572 2e69          logger.i
-000081f0: 6e66 6f28 0a20 2020 2020 2020 2020 2020  nfo(.           
-00008200: 2020 2020 2066 2743 7265 6174 6564 207b       f'Created {
-00008210: 6368 6172 745f 636c 6173 732e 5f5f 6e61  chart_class.__na
-00008220: 6d65 5f5f 7d20 6174 207b 7374 7228 6368  me__} at {str(ch
-00008230: 6172 7429 7d20 7769 7468 2069 6420 7b63  art)} with id {c
-00008240: 6861 7274 5b22 6964 225d 7d27 0a20 2020  hart["id"]}'.   
-00008250: 2020 2020 2020 2020 2029 0a0a 2020 2020           )..    
-00008260: 2020 2020 6164 6465 645f 746f 5f63 6f6e      added_to_con
-00008270: 7461 696e 6572 203d 2046 616c 7365 0a20  tainer = False. 
-00008280: 2020 2020 2020 2069 6620 7365 6c66 2e5f         if self._
-00008290: 6375 7272 656e 745f 7461 6273 5f67 726f  current_tabs_gro
-000082a0: 7570 3a0a 2020 2020 2020 2020 2020 2020  up:.            
-000082b0: 6966 206e 6f74 2073 656c 662e 5f63 7572  if not self._cur
-000082c0: 7265 6e74 5f74 6162 735f 6772 6f75 702e  rent_tabs_group.
-000082d0: 6861 735f 7265 706f 7274 2863 6861 7274  has_report(chart
-000082e0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-000082f0: 2020 2028 6177 6169 7420 7365 6c66 2e5f     (await self._
-00008300: 6765 745f 6375 7272 656e 745f 7461 6273  get_current_tabs
-00008310: 5f67 726f 7570 2829 292e 6164 645f 7265  _group()).add_re
-00008320: 706f 7274 280a 2020 2020 2020 2020 2020  port(.          
-00008330: 2020 2020 2020 2020 2020 7461 623d 7365            tab=se
-00008340: 6c66 2e5f 6375 7272 656e 745f 7461 622c  lf._current_tab,
-00008350: 2072 6570 6f72 743d 6368 6172 740a 2020   report=chart.  
-00008360: 2020 2020 2020 2020 2020 2020 2020 290a                ).
-00008370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008380: 6c6f 6767 6572 2e69 6e66 6f28 0a20 2020  logger.info(.   
-00008390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000083a0: 2066 2249 6e63 6c75 6465 6420 6368 6172   f"Included char
-000083b0: 7420 7b73 7472 2863 6861 7274 297d 2069  t {str(chart)} i
-000083c0: 6e20 7461 6273 2067 726f 7570 207b 7374  n tabs group {st
-000083d0: 7228 7365 6c66 2e5f 6375 7272 656e 745f  r(self._current_
-000083e0: 7461 6273 5f67 726f 7570 297d 220a 2020  tabs_group)}".  
-000083f0: 2020 2020 2020 2020 2020 2020 2020 290a                ).
-00008400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008410: 6164 6465 645f 746f 5f63 6f6e 7461 696e  added_to_contain
-00008420: 6572 203d 2054 7275 650a 2020 2020 2020  er = True.      
-00008430: 2020 656c 6966 2073 656c 662e 5f63 7572    elif self._cur
-00008440: 7265 6e74 5f6d 6f64 616c 2061 6e64 206e  rent_modal and n
-00008450: 6f74 2073 656c 662e 5f63 7572 7265 6e74  ot self._current
-00008460: 5f6d 6f64 616c 2e68 6173 5f72 6570 6f72  _modal.has_repor
-00008470: 7428 6368 6172 7429 3a0a 2020 2020 2020  t(chart):.      
-00008480: 2020 2020 2020 2861 7761 6974 2073 656c        (await sel
-00008490: 662e 5f67 6574 5f63 7572 7265 6e74 5f6d  f._get_current_m
-000084a0: 6f64 616c 2829 292e 6164 645f 7265 706f  odal()).add_repo
-000084b0: 7274 2863 6861 7274 290a 2020 2020 2020  rt(chart).      
-000084c0: 2020 2020 2020 6c6f 6767 6572 2e69 6e66        logger.inf
-000084d0: 6f28 0a20 2020 2020 2020 2020 2020 2020  o(.             
-000084e0: 2020 2066 2249 6e63 6c75 6465 6420 6368     f"Included ch
-000084f0: 6172 7420 7b73 7472 2863 6861 7274 297d  art {str(chart)}
-00008500: 2069 6e20 6d6f 6461 6c20 7b73 7472 2873   in modal {str(s
-00008510: 656c 662e 5f63 7572 7265 6e74 5f6d 6f64  elf._current_mod
-00008520: 616c 297d 220a 2020 2020 2020 2020 2020  al)}".          
-00008530: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
-00008540: 6164 6465 645f 746f 5f63 6f6e 7461 696e  added_to_contain
-00008550: 6572 203d 2054 7275 650a 0a20 2020 2020  er = True..     
-00008560: 2020 2069 6620 280a 2020 2020 2020 2020     if (.        
-00008570: 2020 2020 6164 6465 645f 746f 5f63 6f6e      added_to_con
-00008580: 7461 696e 6572 0a20 2020 2020 2020 2020  tainer.         
-00008590: 2020 2061 6e64 2022 7570 6461 7465 5f63     and "update_c
-000085a0: 6f6e 7461 696e 6572 7322 206e 6f74 2069  ontainers" not i
-000085b0: 6e20 7365 6c66 2e5f 6173 796e 635f 706f  n self._async_po
-000085c0: 6f6c 2e65 6e64 696e 675f 7461 736b 730a  ol.ending_tasks.
-000085d0: 2020 2020 2020 2020 293a 0a20 2020 2020          ):.     
-000085e0: 2020 2020 2020 2073 656c 662e 5f61 7379         self._asy
-000085f0: 6e63 5f70 6f6f 6c2e 656e 6469 6e67 5f74  nc_pool.ending_t
-00008600: 6173 6b73 5b0a 2020 2020 2020 2020 2020  asks[.          
-00008610: 2020 2020 2020 2275 7064 6174 655f 636f        "update_co
-00008620: 6e74 6169 6e65 7273 220a 2020 2020 2020  ntainers".      
-00008630: 2020 2020 2020 5d20 3d20 7365 6c66 2e5f        ] = self._
-00008640: 7570 6461 7465 5f63 6f6e 7461 696e 6572  update_container
-00008650: 7328 290a 0a20 2020 2020 2020 2061 7761  s()..        awa
-00008660: 6974 2073 656c 662e 5f63 7265 6174 655f  it self._create_
-00008670: 6576 656e 7428 6576 656e 745f 7479 7065  event(event_type
-00008680: 2c20 7b7d 2c20 6368 6172 745b 2269 6422  , {}, chart["id"
-00008690: 5d29 0a0a 2020 2020 2020 2020 7265 7475  ])..        retu
-000086a0: 726e 2063 6861 7274 0a0a 2020 2020 6465  rn chart..    de
-000086b0: 6620 5f67 6574 5f66 6965 6c64 5f6d 6170  f _get_field_map
-000086c0: 7069 6e67 280a 2020 2020 2020 2020 7365  ping(.        se
-000086d0: 6c66 2c20 6669 656c 643a 2055 6e69 6f6e  lf, field: Union
-000086e0: 5b73 7472 2c20 7475 706c 652c 206c 6973  [str, tuple, lis
-000086f0: 742c 2064 6963 745d 2c20 6461 7461 5f6d  t, dict], data_m
-00008700: 6170 7069 6e67 5f74 6f5f 7475 706c 653a  apping_to_tuple:
-00008710: 2064 6963 740a 2020 2020 2920 2d3e 2055   dict.    ) -> U
-00008720: 6e69 6f6e 5b73 7472 2c20 6c69 7374 2c20  nion[str, list, 
-00008730: 6469 6374 5d3a 0a20 2020 2020 2020 2022  dict]:.        "
-00008740: 2222 4765 7420 7468 6520 6d61 7070 696e  ""Get the mappin
-00008750: 6720 6f66 2061 2066 6965 6c64 2e22 2222  g of a field."""
-00008760: 0a20 2020 2020 2020 2069 6620 6973 696e  .        if isin
-00008770: 7374 616e 6365 2866 6965 6c64 2c20 7374  stance(field, st
-00008780: 7229 3a0a 2020 2020 2020 2020 2020 2020  r):.            
-00008790: 7265 7475 726e 2064 6174 615f 6d61 7070  return data_mapp
-000087a0: 696e 675f 746f 5f74 7570 6c65 5b66 6965  ing_to_tuple[fie
-000087b0: 6c64 5d5b 305d 0a20 2020 2020 2020 2065  ld][0].        e
-000087c0: 6c69 6620 6973 696e 7374 616e 6365 2866  lif isinstance(f
-000087d0: 6965 6c64 2c20 2874 7570 6c65 2c20 6c69  ield, (tuple, li
-000087e0: 7374 2929 3a0a 2020 2020 2020 2020 2020  st)):.          
-000087f0: 2020 7265 7475 726e 205b 6461 7461 5f6d    return [data_m
-00008800: 6170 7069 6e67 5f74 6f5f 7475 706c 655b  apping_to_tuple[
-00008810: 665d 5b30 5d20 666f 7220 6620 696e 2066  f][0] for f in f
-00008820: 6965 6c64 5d0a 2020 2020 2020 2020 656c  ield].        el
-00008830: 6966 2069 7369 6e73 7461 6e63 6528 6669  if isinstance(fi
-00008840: 656c 642c 2064 6963 7429 3a0a 2020 2020  eld, dict):.    
-00008850: 2020 2020 2020 2020 7265 7475 726e 207b          return {
-00008860: 6b3a 2064 6174 615f 6d61 7070 696e 675f  k: data_mapping_
-00008870: 746f 5f74 7570 6c65 5b76 5d5b 305d 2066  to_tuple[v][0] f
-00008880: 6f72 206b 2c20 7620 696e 2066 6965 6c64  or k, v in field
-00008890: 2e69 7465 6d73 2829 7d0a 0a20 2020 2064  .items()}..    d
-000088a0: 6566 205f 6368 6563 6b5f 6d61 7070 696e  ef _check_mappin
-000088b0: 675f 696e 5f72 6570 6f72 745f 6461 7461  g_in_report_data
-000088c0: 5f73 6574 280a 2020 2020 2020 2020 7365  _set(.        se
-000088d0: 6c66 2c20 7265 706f 7274 5f64 6174 615f  lf, report_data_
-000088e0: 7365 743a 2052 6570 6f72 742e 5265 706f  set: Report.Repo
-000088f0: 7274 4461 7461 5365 742c 206d 6170 7069  rtDataSet, mappi
-00008900: 6e67 3a20 4d61 7070 696e 670a 2020 2020  ng: Mapping.    
-00008910: 2920 2d3e 2062 6f6f 6c3a 0a20 2020 2020  ) -> bool:.     
-00008920: 2020 2022 2222 4368 6563 6b20 6966 2074     """Check if t
-00008930: 6865 206d 6170 7069 6e67 2069 7320 636f  he mapping is co
-00008940: 7272 6563 7420 696e 2074 6865 2072 6570  rrect in the rep
-00008950: 6f72 7420 6461 7461 2073 6574 2e0a 2020  ort data set..  
-00008960: 2020 2020 2020 3a70 6172 616d 2072 6570        :param rep
-00008970: 6f72 745f 6461 7461 5f73 6574 3a20 7468  ort_data_set: th
-00008980: 6520 7265 706f 7274 2064 6174 6120 7365  e report data se
-00008990: 740a 2020 2020 2020 2020 3a70 6172 616d  t.        :param
-000089a0: 206d 6170 7069 6e67 3a20 7468 6520 6d61   mapping: the ma
-000089b0: 7070 696e 670a 2020 2020 2020 2020 3a72  pping.        :r
-000089c0: 6574 7572 6e3a 2054 7275 6520 6966 2074  eturn: True if t
-000089d0: 6865 206d 6170 7069 6e67 2069 7320 636f  he mapping is co
-000089e0: 6e73 6973 7465 6e74 2c20 4661 6c73 6520  nsistent, False 
-000089f0: 6f74 6865 7277 6973 650a 2020 2020 2020  otherwise.      
-00008a00: 2020 2222 220a 2020 2020 2020 2020 7265    """.        re
-00008a10: 706f 7274 5f64 6174 615f 7365 745f 6d61  port_data_set_ma
-00008a20: 7070 696e 6720 3d20 7265 706f 7274 5f64  pping = report_d
-00008a30: 6174 615f 7365 745b 2270 726f 7065 7274  ata_set["propert
-00008a40: 6965 7322 5d5b 226d 6170 7069 6e67 225d  ies"]["mapping"]
-00008a50: 0a20 2020 2020 2020 2069 6620 7265 706f  .        if repo
-00008a60: 7274 5f64 6174 615f 7365 745f 6d61 7070  rt_data_set_mapp
-00008a70: 696e 6720 213d 206d 6170 7069 6e67 3a0a  ing != mapping:.
-00008a80: 2020 2020 2020 2020 2020 2020 6c6f 6767              logg
-00008a90: 6572 2e77 6172 6e69 6e67 280a 2020 2020  er.warning(.    
-00008aa0: 2020 2020 2020 2020 2020 2020 6622 4d61              f"Ma
-00008ab0: 7070 696e 6720 696e 636f 6e73 6973 7465  pping inconsiste
-00008ac0: 6e74 2069 6e20 636f 6d70 6f6e 656e 7420  nt in component 
-00008ad0: 6461 7461 2073 6574 206c 696e 6b20 7b73  data set link {s
-00008ae0: 7472 2872 6570 6f72 745f 6461 7461 5f73  tr(report_data_s
-00008af0: 6574 297d 220a 2020 2020 2020 2020 2020  et)}".          
-00008b00: 2020 290a 2020 2020 2020 2020 7265 7475    ).        retu
-00008b10: 726e 2072 6570 6f72 745f 6461 7461 5f73  rn report_data_s
-00008b20: 6574 5f6d 6170 7069 6e67 203d 3d20 6d61  et_mapping == ma
-00008b30: 7070 696e 670a 0a20 2020 2040 7374 6174  pping..    @stat
-00008b40: 6963 6d65 7468 6f64 0a20 2020 2064 6566  icmethod.    def
-00008b50: 205f 6765 745f 6669 6c74 6572 5f70 726f   _get_filter_pro
-00008b60: 7065 7274 6965 7328 0a20 2020 2020 2020  perties(.       
-00008b70: 2073 6572 6965 735f 6e61 6d65 3a20 7374   series_name: st
-00008b80: 722c 2063 6f6e 7665 7274 6564 5f64 6174  r, converted_dat
-00008b90: 613a 2070 642e 4461 7461 4672 616d 652c  a: pd.DataFrame,
-00008ba0: 206d 756c 7469 5f73 656c 6563 743a 2062   multi_select: b
-00008bb0: 6f6f 6c0a 2020 2020 2920 2d3e 2074 7570  ool.    ) -> tup
-00008bc0: 6c65 5b4f 7074 696f 6e61 6c5b 6c69 7374  le[Optional[list
-00008bd0: 5b73 7472 5d5d 2c20 4f70 7469 6f6e 616c  [str]], Optional
-00008be0: 5b6c 6973 745b 7374 725d 5d2c 2046 696c  [list[str]], Fil
-00008bf0: 7465 7244 6174 6153 6574 2e49 6e70 7574  terDataSet.Input
-00008c00: 5479 7065 5d3a 0a20 2020 2020 2020 2069  Type]:.        i
-00008c10: 6620 7365 7269 6573 5f6e 616d 652e 7374  f series_name.st
-00008c20: 6172 7473 7769 7468 2822 6461 7465 2229  artswith("date")
-00008c30: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-00008c40: 7475 726e 204e 6f6e 652c 205b 2263 6f6e  turn None, ["con
-00008c50: 7461 696e 7322 5d2c 2046 696c 7465 7244  tains"], FilterD
-00008c60: 6174 6153 6574 2e49 6e70 7574 5479 7065  ataSet.InputType
-00008c70: 2e44 4154 4552 414e 4745 0a20 2020 2020  .DATERANGE.     
-00008c80: 2020 2065 6c69 6620 7365 7269 6573 5f6e     elif series_n
-00008c90: 616d 652e 7374 6172 7473 7769 7468 2822  ame.startswith("
-00008ca0: 696e 7422 293a 0a20 2020 2020 2020 2020  int"):.         
-00008cb0: 2020 2072 6574 7572 6e20 4e6f 6e65 2c20     return None, 
-00008cc0: 4e6f 6e65 2c20 4669 6c74 6572 4461 7461  None, FilterData
-00008cd0: 5365 742e 496e 7075 7454 7970 652e 4e55  Set.InputType.NU
-00008ce0: 4d45 5249 430a 2020 2020 2020 2020 656c  MERIC.        el
-00008cf0: 6966 2073 6572 6965 735f 6e61 6d65 2e73  if series_name.s
-00008d00: 7461 7274 7377 6974 6828 2273 7472 696e  tartswith("strin
-00008d10: 6722 293a 0a20 2020 2020 2020 2020 2020  g"):.           
-00008d20: 2072 6574 7572 6e20 280a 2020 2020 2020   return (.      
-00008d30: 2020 2020 2020 2020 2020 636f 6e76 6572            conver
-00008d40: 7465 645f 6461 7461 5b73 6572 6965 735f  ted_data[series_
-00008d50: 6e61 6d65 5d2e 756e 6971 7565 2829 2e74  name].unique().t
-00008d60: 6f6c 6973 7428 292c 0a20 2020 2020 2020  olist(),.       
-00008d70: 2020 2020 2020 2020 205b 2265 7122 5d2c           ["eq"],
-00008d80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00008d90: 2046 696c 7465 7244 6174 6153 6574 2e49   FilterDataSet.I
-00008da0: 6e70 7574 5479 7065 2e43 4154 4547 4f52  nputType.CATEGOR
-00008db0: 4943 414c 5f53 494e 474c 450a 2020 2020  ICAL_SINGLE.    
-00008dc0: 2020 2020 2020 2020 2020 2020 6966 206e              if n
-00008dd0: 6f74 206d 756c 7469 5f73 656c 6563 740a  ot multi_select.
-00008de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008df0: 656c 7365 2046 696c 7465 7244 6174 6153  else FilterDataS
-00008e00: 6574 2e49 6e70 7574 5479 7065 2e43 4154  et.InputType.CAT
-00008e10: 4547 4f52 4943 414c 5f4d 554c 5449 2c0a  EGORICAL_MULTI,.
-00008e20: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-00008e30: 2020 2020 2020 6c6f 675f 6572 726f 7228        log_error(
-00008e40: 0a20 2020 2020 2020 2020 2020 206c 6f67  .            log
-00008e50: 6765 722c 2066 2246 6965 6c64 2074 7970  ger, f"Field typ
-00008e60: 6520 7b73 6572 6965 735f 6e61 6d65 7d20  e {series_name} 
-00008e70: 6973 206e 6f74 2073 7570 706f 7274 6564  is not supported
-00008e80: 222c 204e 6f74 496d 706c 656d 656e 7465  ", NotImplemente
-00008e90: 6445 7272 6f72 0a20 2020 2020 2020 2029  dError.        )
-00008ea0: 0a0a 2020 2020 4061 6464 5f74 6f5f 6765  ..    @add_to_ge
-00008eb0: 6e65 7261 6c5f 6173 796e 635f 6772 6f75  neral_async_grou
-00008ec0: 700a 2020 2020 6173 796e 6320 6465 6620  p.    async def 
-00008ed0: 6669 6c74 6572 280a 2020 2020 2020 2020  filter(.        
-00008ee0: 7365 6c66 2c0a 2020 2020 2020 2020 6f72  self,.        or
-00008ef0: 6465 723a 2069 6e74 2c0a 2020 2020 2020  der: int,.      
-00008f00: 2020 6461 7461 3a20 7374 722c 0a20 2020    data: str,.   
-00008f10: 2020 2020 2066 6965 6c64 3a20 7374 722c       field: str,
-00008f20: 0a20 2020 2020 2020 206d 756c 7469 5f73  .        multi_s
-00008f30: 656c 6563 743a 2062 6f6f 6c20 3d20 4661  elect: bool = Fa
-00008f40: 6c73 652c 0a20 2020 2020 2020 2063 6f6c  lse,.        col
-00008f50: 735f 7369 7a65 3a20 696e 7420 3d20 342c  s_size: int = 4,
-00008f60: 0a20 2020 2020 2020 2072 6f77 735f 7369  .        rows_si
-00008f70: 7a65 3a20 696e 7420 3d20 312c 0a20 2020  ze: int = 1,.   
-00008f80: 2020 2020 2070 6164 6469 6e67 3a20 4f70       padding: Op
-00008f90: 7469 6f6e 616c 5b73 7472 5d20 3d20 4e6f  tional[str] = No
-00008fa0: 6e65 2c0a 2020 2020 293a 0a20 2020 2020  ne,.    ):.     
-00008fb0: 2020 2022 2222 0a20 2020 2020 2020 2046     """.        F
-00008fc0: 696c 7465 7220 7468 6520 6461 7461 2073  ilter the data s
-00008fd0: 6574 2e0a 2020 2020 2020 2020 3a70 6172  et..        :par
-00008fe0: 616d 206f 7264 6572 3a20 7468 6520 6f72  am order: the or
-00008ff0: 6465 7220 6f66 2074 6865 2063 6861 7274  der of the chart
-00009000: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-00009010: 6461 7461 3a20 7468 6520 6461 7461 0a20  data: the data. 
-00009020: 2020 2020 2020 203a 7061 7261 6d20 6669         :param fi
-00009030: 656c 643a 2074 6865 2066 6965 6c64 2074  eld: the field t
-00009040: 6f20 6669 6c74 6572 0a20 2020 2020 2020  o filter.       
-00009050: 203a 7061 7261 6d20 6d75 6c74 695f 7365   :param multi_se
-00009060: 6c65 6374 3a20 7768 6574 6865 7220 746f  lect: whether to
-00009070: 2061 6c6c 6f77 206d 756c 7469 2073 656c   allow multi sel
-00009080: 6563 740a 2020 2020 2020 2020 3a70 6172  ect.        :par
-00009090: 616d 2063 6f6c 735f 7369 7a65 3a20 7468  am cols_size: th
-000090a0: 6520 7369 7a65 206f 6620 7468 6520 636f  e size of the co
-000090b0: 6c75 6d6e 730a 2020 2020 2020 2020 3a70  lumns.        :p
-000090c0: 6172 616d 2072 6f77 735f 7369 7a65 3a20  aram rows_size: 
-000090d0: 7468 6520 7369 7a65 206f 6620 7468 6520  the size of the 
-000090e0: 726f 7773 0a20 2020 2020 2020 203a 7061  rows.        :pa
-000090f0: 7261 6d20 7061 6464 696e 673a 2074 6865  ram padding: the
-00009100: 2070 6164 6469 6e67 0a20 2020 2020 2020   padding.       
-00009110: 2022 2222 0a0a 2020 2020 2020 2020 6966   """..        if
-00009120: 206e 6f74 2069 7369 6e73 7461 6e63 6528   not isinstance(
-00009130: 6461 7461 2c20 7374 7229 3a0a 2020 2020  data, str):.    
-00009140: 2020 2020 2020 2020 6c6f 675f 6572 726f          log_erro
-00009150: 7228 0a20 2020 2020 2020 2020 2020 2020  r(.             
-00009160: 2020 206c 6f67 6765 722c 0a20 2020 2020     logger,.     
-00009170: 2020 2020 2020 2020 2020 2022 546f 2066             "To f
-00009180: 696c 7465 7220 6120 6461 7461 2073 6574  ilter a data set
-00009190: 2c20 7468 6520 6461 7461 206d 7573 7420  , the data must 
-000091a0: 6265 2061 2073 6861 7265 6420 6461 7461  be a shared data
-000091b0: 2065 6e74 7279 222c 0a20 2020 2020 2020   entry",.       
-000091c0: 2020 2020 2020 2020 2044 6174 6145 7272           DataErr
-000091d0: 6f72 2c0a 2020 2020 2020 2020 2020 2020  or,.            
-000091e0: 290a 0a20 2020 2020 2020 2069 6620 6461  )..        if da
-000091f0: 7461 206e 6f74 2069 6e20 7365 6c66 2e5f  ta not in self._
-00009200: 7368 6172 6564 5f64 6174 615f 6d61 703a  shared_data_map:
-00009210: 0a20 2020 2020 2020 2020 2020 206c 6f67  .            log
-00009220: 5f65 7272 6f72 286c 6f67 6765 722c 2066  _error(logger, f
-00009230: 224e 6f20 7368 6172 6564 2064 6174 6120  "No shared data 
-00009240: 7769 7468 206e 616d 6520 7b64 6174 617d  with name {data}
-00009250: 2066 6f75 6e64 222c 2044 6174 6145 7272   found", DataErr
-00009260: 6f72 290a 0a20 2020 2020 2020 205f 2c20  or)..        _, 
-00009270: 6461 7461 5f73 6574 2c20 5f20 3d20 7365  data_set, _ = se
-00009280: 6c66 2e5f 7368 6172 6564 5f64 6174 615f  lf._shared_data_
-00009290: 6d61 705b 6461 7461 5d5b 6669 656c 645d  map[data][field]
-000092a0: 0a20 2020 2020 2020 2064 6174 6120 3d20  .        data = 
-000092b0: 7365 6c66 2e5f 7368 6172 6564 5f64 6174  self._shared_dat
-000092c0: 615b 6461 7461 5d0a 0a20 2020 2020 2020  a[data]..       
-000092d0: 2063 6f6e 7665 7274 6564 5f64 6174 612c   converted_data,
-000092e0: 2073 6572 6965 735f 6e61 6d65 203d 2063   series_name = c
-000092f0: 6f6e 7665 7274 5f64 6174 615f 616e 645f  onvert_data_and_
-00009300: 6765 745f 7365 7269 6573 5f6e 616d 6528  get_series_name(
-00009310: 6461 7461 2c20 6669 656c 6429 0a20 2020  data, field).   
-00009320: 2020 2020 206f 7074 696f 6e73 2c20 6f70       options, op
-00009330: 6572 6174 696f 6e73 2c20 696e 7075 745f  erations, input_
-00009340: 7479 7065 203d 2073 656c 662e 5f67 6574  type = self._get
-00009350: 5f66 696c 7465 725f 7072 6f70 6572 7469  _filter_properti
-00009360: 6573 280a 2020 2020 2020 2020 2020 2020  es(.            
-00009370: 7365 7269 6573 5f6e 616d 652c 2063 6f6e  series_name, con
-00009380: 7665 7274 6564 5f64 6174 612c 206d 756c  verted_data, mul
-00009390: 7469 5f73 656c 6563 740a 2020 2020 2020  ti_select.      
-000093a0: 2020 290a 0a20 2020 2020 2020 2070 726f    )..        pro
-000093b0: 7065 7274 6965 7320 3d20 7b0a 2020 2020  perties = {.    
-000093c0: 2020 2020 2020 2020 2266 696c 7465 7222          "filter"
-000093d0: 3a20 5b0a 2020 2020 2020 2020 2020 2020  : [.            
-000093e0: 2020 2020 7b0a 2020 2020 2020 2020 2020      {.          
-000093f0: 2020 2020 2020 2020 2020 2266 6965 6c64            "field
-00009400: 223a 2066 6965 6c64 2c0a 2020 2020 2020  ": field,.      
-00009410: 2020 2020 2020 2020 2020 2020 2020 2269                "i
-00009420: 6e70 7574 5479 7065 223a 2069 6e70 7574  nputType": input
-00009430: 5f74 7970 652e 7661 6c75 652c 0a20 2020  _type.value,.   
-00009440: 2020 2020 2020 2020 2020 2020 207d 0a20               }. 
-00009450: 2020 2020 2020 2020 2020 205d 2c0a 2020             ],.  
-00009460: 2020 2020 2020 2020 2020 226d 6170 7069            "mappi
-00009470: 6e67 223a 205b 7b66 6965 6c64 3a20 7365  ng": [{field: se
-00009480: 7269 6573 5f6e 616d 652c 2022 6964 223a  ries_name, "id":
-00009490: 2064 6174 615f 7365 745b 2269 6422 5d7d   data_set["id"]}
-000094a0: 5d2c 0a20 2020 2020 2020 207d 0a0a 2020  ],.        }..  
-000094b0: 2020 2020 2020 6966 206f 7065 7261 7469        if operati
-000094c0: 6f6e 733a 0a20 2020 2020 2020 2020 2020  ons:.           
-000094d0: 2070 726f 7065 7274 6965 735b 2266 696c   properties["fil
-000094e0: 7465 7222 5d5b 305d 5b22 6f70 6572 6174  ter"][0]["operat
-000094f0: 696f 6e73 225d 203d 206f 7065 7261 7469  ions"] = operati
-00009500: 6f6e 730a 2020 2020 2020 2020 6966 206f  ons.        if o
-00009510: 7074 696f 6e73 3a0a 2020 2020 2020 2020  ptions:.        
-00009520: 2020 2020 7072 6f70 6572 7469 6573 5b22      properties["
-00009530: 6669 6c74 6572 225d 5b30 5d5b 226f 7074  filter"][0]["opt
-00009540: 696f 6e73 225d 203d 206f 7074 696f 6e73  ions"] = options
-00009550: 0a0a 2020 2020 2020 2020 6177 6169 7420  ..        await 
-00009560: 7365 6c66 2e5f 6372 6561 7465 5f63 6861  self._create_cha
-00009570: 7274 280a 2020 2020 2020 2020 2020 2020  rt(.            
-00009580: 6368 6172 745f 636c 6173 733d 4669 6c74  chart_class=Filt
-00009590: 6572 4461 7461 5365 742c 0a20 2020 2020  erDataSet,.     
-000095a0: 2020 2020 2020 206f 7264 6572 3d6f 7264         order=ord
-000095b0: 6572 2c0a 2020 2020 2020 2020 2020 2020  er,.            
-000095c0: 7469 746c 653d 2222 2c0a 2020 2020 2020  title="",.      
-000095d0: 2020 2020 2020 7369 7a65 526f 7773 3d72        sizeRows=r
-000095e0: 6f77 735f 7369 7a65 2c0a 2020 2020 2020  ows_size,.      
-000095f0: 2020 2020 2020 7369 7a65 436f 6c75 6d6e        sizeColumn
-00009600: 733d 636f 6c73 5f73 697a 652c 0a20 2020  s=cols_size,.   
-00009610: 2020 2020 2020 2020 2073 697a 6550 6164           sizePad
-00009620: 6469 6e67 3d70 6164 6469 6e67 2c0a 2020  ding=padding,.  
-00009630: 2020 2020 2020 2020 2020 7072 6f70 6572            proper
-00009640: 7469 6573 3d70 726f 7065 7274 6965 732c  ties=properties,
-00009650: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
-00009660: 4061 6464 5f74 6f5f 6765 6e65 7261 6c5f  @add_to_general_
-00009670: 6173 796e 635f 6772 6f75 700a 2020 2020  async_group.    
-00009680: 6173 796e 6320 6465 6620 6966 7261 6d65  async def iframe
-00009690: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
-000096a0: 2020 2020 2020 2020 7572 6c3a 2073 7472          url: str
-000096b0: 2c0a 2020 2020 2020 2020 6f72 6465 723a  ,.        order:
-000096c0: 2069 6e74 2c0a 2020 2020 2020 2020 6865   int,.        he
-000096d0: 6967 6874 3a20 696e 7420 3d20 3634 302c  ight: int = 640,
-000096e0: 0a20 2020 2020 2020 2063 6f6c 735f 7369  .        cols_si
-000096f0: 7a65 3a20 4f70 7469 6f6e 616c 5b69 6e74  ze: Optional[int
-00009700: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
-00009710: 2020 7061 6464 696e 673a 204f 7074 696f    padding: Optio
-00009720: 6e61 6c5b 7374 725d 203d 204e 6f6e 652c  nal[str] = None,
-00009730: 0a20 2020 2029 3a0a 2020 2020 2020 2020  .    ):.        
-00009740: 2222 2243 7265 6174 6520 616e 2069 6672  """Create an ifr
-00009750: 616d 6520 7265 706f 7274 2069 6e20 7468  ame report in th
-00009760: 6520 6461 7368 626f 6172 642e 0a20 2020  e dashboard..   
-00009770: 2020 2020 203a 7061 7261 6d20 7572 6c3a       :param url:
-00009780: 2074 6865 2075 726c 206f 6620 7468 6520   the url of the 
-00009790: 6966 7261 6d65 0a20 2020 2020 2020 203a  iframe.        :
-000097a0: 7061 7261 6d20 6f72 6465 723a 2074 6865  param order: the
-000097b0: 206f 7264 6572 206f 6620 7468 6520 6966   order of the if
-000097c0: 7261 6d65 0a20 2020 2020 2020 203a 7061  rame.        :pa
-000097d0: 7261 6d20 6865 6967 6874 3a20 7468 6520  ram height: the 
-000097e0: 6865 6967 6874 206f 6620 7468 6520 6966  height of the if
-000097f0: 7261 6d65 0a20 2020 2020 2020 203a 7061  rame.        :pa
-00009800: 7261 6d20 636f 6c73 5f73 697a 653a 2074  ram cols_size: t
-00009810: 6865 2063 6f6c 756d 6e73 2074 6861 7420  he columns that 
-00009820: 7468 6520 6966 7261 6d65 206f 6363 7570  the iframe occup
-00009830: 6965 730a 2020 2020 2020 2020 3a70 6172  ies.        :par
-00009840: 616d 2070 6164 6469 6e67 3a20 7061 6464  am padding: padd
-00009850: 696e 670a 2020 2020 2020 2020 2222 220a  ing.        """.
-00009860: 2020 2020 2020 2020 6177 6169 7420 7365          await se
-00009870: 6c66 2e5f 6372 6561 7465 5f63 6861 7274  lf._create_chart
-00009880: 280a 2020 2020 2020 2020 2020 2020 6368  (.            ch
-00009890: 6172 745f 636c 6173 733d 4946 7261 6d65  art_class=IFrame
-000098a0: 2c0a 2020 2020 2020 2020 2020 2020 6f72  ,.            or
-000098b0: 6465 723d 6f72 6465 722c 0a20 2020 2020  der=order,.     
-000098c0: 2020 2020 2020 2064 6174 6146 6965 6c64         dataField
-000098d0: 733d 6469 6374 280a 2020 2020 2020 2020  s=dict(.        
-000098e0: 2020 2020 2020 2020 7572 6c3d 7572 6c2c          url=url,
-000098f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009900: 2068 6569 6768 743d 6865 6967 6874 2c0a   height=height,.
-00009910: 2020 2020 2020 2020 2020 2020 292c 0a20              ),. 
-00009920: 2020 2020 2020 2020 2020 2073 697a 6550             sizeP
-00009930: 6164 6469 6e67 3d70 6164 6469 6e67 2c0a  adding=padding,.
-00009940: 2020 2020 2020 2020 2020 2020 7369 7a65              size
-00009950: 436f 6c75 6d6e 733d 636f 6c73 5f73 697a  Columns=cols_siz
-00009960: 652c 0a20 2020 2020 2020 2020 2020 2073  e,.            s
-00009970: 697a 6552 6f77 733d 6365 696c 2868 6569  izeRows=ceil(hei
-00009980: 6768 7420 2f20 3234 3029 2c0a 2020 2020  ght / 240),.    
-00009990: 2020 2020 290a 0a20 2020 2061 7379 6e63      )..    async
-000099a0: 2064 6566 205f 6874 6d6c 280a 2020 2020   def _html(.    
-000099b0: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
-000099c0: 2020 6874 6d6c 3a20 7374 722c 0a20 2020    html: str,.   
-000099d0: 2020 2020 206f 7264 6572 3a20 696e 742c       order: int,
-000099e0: 0a20 2020 2020 2020 2063 6f6c 735f 7369  .        cols_si
-000099f0: 7a65 3a20 4f70 7469 6f6e 616c 5b69 6e74  ze: Optional[int
-00009a00: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
-00009a10: 2020 726f 7773 5f73 697a 653a 204f 7074    rows_size: Opt
-00009a20: 696f 6e61 6c5b 696e 745d 203d 204e 6f6e  ional[int] = Non
-00009a30: 652c 0a20 2020 2020 2020 2070 6164 6469  e,.        paddi
-00009a40: 6e67 3a20 4f70 7469 6f6e 616c 5b73 7472  ng: Optional[str
-00009a50: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 293a  ] = None,.    ):
-00009a60: 0a20 2020 2020 2020 2022 2222 6874 6d6c  .        """html
-00009a70: 2066 6f72 2069 6e74 6572 6e61 6c20 7573   for internal us
-00009a80: 6522 2222 0a20 2020 2020 2020 2061 7761  e""".        awa
-00009a90: 6974 2073 656c 662e 5f63 7265 6174 655f  it self._create_
-00009aa0: 6368 6172 7428 0a20 2020 2020 2020 2020  chart(.         
-00009ab0: 2020 2063 6861 7274 5f63 6c61 7373 3d48     chart_class=H
-00009ac0: 544d 4c2c 0a20 2020 2020 2020 2020 2020  TML,.           
-00009ad0: 206f 7264 6572 3d6f 7264 6572 2c0a 2020   order=order,.  
-00009ae0: 2020 2020 2020 2020 2020 6368 6172 7444            chartD
-00009af0: 6174 613d 5b7b 2276 616c 7565 223a 2068  ata=[{"value": h
-00009b00: 746d 6c7d 5d2c 0a20 2020 2020 2020 2020  tml}],.         
-00009b10: 2020 2073 697a 6550 6164 6469 6e67 3d70     sizePadding=p
-00009b20: 6164 6469 6e67 2c0a 2020 2020 2020 2020  adding,.        
-00009b30: 2020 2020 7369 7a65 436f 6c75 6d6e 733d      sizeColumns=
-00009b40: 636f 6c73 5f73 697a 652c 0a20 2020 2020  cols_size,.     
-00009b50: 2020 2020 2020 2073 697a 6552 6f77 733d         sizeRows=
-00009b60: 726f 7773 5f73 697a 652c 0a20 2020 2020  rows_size,.     
-00009b70: 2020 2029 0a0a 2020 2020 4061 6464 5f74     )..    @add_t
-00009b80: 6f5f 6765 6e65 7261 6c5f 6173 796e 635f  o_general_async_
-00009b90: 6772 6f75 700a 2020 2020 6173 796e 6320  group.    async 
-00009ba0: 6465 6620 6874 6d6c 280a 2020 2020 2020  def html(.      
-00009bb0: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
-00009bc0: 6874 6d6c 3a20 7374 722c 0a20 2020 2020  html: str,.     
-00009bd0: 2020 206f 7264 6572 3a20 696e 742c 0a20     order: int,. 
-00009be0: 2020 2020 2020 2063 6f6c 735f 7369 7a65         cols_size
-00009bf0: 3a20 4f70 7469 6f6e 616c 5b69 6e74 5d20  : Optional[int] 
-00009c00: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-00009c10: 726f 7773 5f73 697a 653a 204f 7074 696f  rows_size: Optio
-00009c20: 6e61 6c5b 696e 745d 203d 204e 6f6e 652c  nal[int] = None,
-00009c30: 0a20 2020 2020 2020 2070 6164 6469 6e67  .        padding
-00009c40: 3a20 4f70 7469 6f6e 616c 5b73 7472 5d20  : Optional[str] 
-00009c50: 3d20 4e6f 6e65 2c0a 2020 2020 293a 0a20  = None,.    ):. 
-00009c60: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00009c70: 2020 2043 7265 6174 6520 616e 2068 746d     Create an htm
-00009c80: 6c20 7265 706f 7274 2069 6e20 7468 6520  l report in the 
-00009c90: 6461 7368 626f 6172 642e 0a20 2020 2020  dashboard..     
-00009ca0: 2020 203a 7061 7261 6d20 6874 6d6c 3a20     :param html: 
-00009cb0: 7468 6520 6874 6d6c 2063 6f64 650a 2020  the html code.  
-00009cc0: 2020 2020 2020 3a70 6172 616d 206f 7264        :param ord
-00009cd0: 6572 3a20 7468 6520 6f72 6465 7220 6f66  er: the order of
-00009ce0: 2074 6865 2068 746d 6c0a 2020 2020 2020   the html.      
-00009cf0: 2020 3a63 6f6c 735f 7369 7a65 3a20 7468    :cols_size: th
-00009d00: 6520 636f 6c75 6d6e 7320 7468 6174 2074  e columns that t
-00009d10: 6865 2068 746d 6c20 6f63 6375 7069 6573  he html occupies
-00009d20: 0a20 2020 2020 2020 203a 726f 7773 5f73  .        :rows_s
-00009d30: 697a 653a 2074 6865 2072 6f77 7320 7468  ize: the rows th
-00009d40: 6174 2074 6865 2068 746d 6c20 6f63 6375  at the html occu
-00009d50: 7069 6573 0a20 2020 2020 2020 203a 7061  pies.        :pa
-00009d60: 6464 696e 673a 2070 6164 6469 6e67 0a20  dding: padding. 
-00009d70: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00009d80: 2020 2061 7761 6974 2073 656c 662e 5f68     await self._h
-00009d90: 746d 6c28 6874 6d6c 2c20 6f72 6465 722c  tml(html, order,
-00009da0: 2063 6f6c 735f 7369 7a65 2c20 726f 7773   cols_size, rows
-00009db0: 5f73 697a 652c 2070 6164 6469 6e67 290a  _size, padding).
-00009dc0: 0a20 2020 2040 6164 645f 746f 5f67 656e  .    @add_to_gen
-00009dd0: 6572 616c 5f61 7379 6e63 5f67 726f 7570  eral_async_group
-00009de0: 0a20 2020 2061 7379 6e63 2064 6566 2073  .    async def s
-00009df0: 696e 676c 655f 696e 6469 6361 746f 7228  ingle_indicator(
-00009e00: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
-00009e10: 2020 2020 2020 2064 6174 613a 2064 6963         data: dic
-00009e20: 742c 0a20 2020 2020 2020 206f 7264 6572  t,.        order
-00009e30: 3a20 696e 742c 0a20 2020 2020 2020 2063  : int,.        c
-00009e40: 6f6c 735f 7369 7a65 3a20 4f70 7469 6f6e  ols_size: Option
-00009e50: 616c 5b69 6e74 5d20 3d20 4e6f 6e65 2c0a  al[int] = None,.
-00009e60: 2020 2020 2020 2020 726f 7773 5f73 697a          rows_siz
-00009e70: 653a 204f 7074 696f 6e61 6c5b 696e 745d  e: Optional[int]
-00009e80: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-00009e90: 2070 6164 6469 6e67 3a20 4f70 7469 6f6e   padding: Option
-00009ea0: 616c 5b73 7472 5d20 3d20 4e6f 6e65 2c0a  al[str] = None,.
-00009eb0: 2020 2020 293a 0a20 2020 2020 2020 2022      ):.        "
-00009ec0: 2222 0a20 2020 2020 2020 2043 7265 6174  "".        Creat
-00009ed0: 6520 616e 2069 6e64 6963 6174 6f72 2072  e an indicator r
-00009ee0: 6570 6f72 7420 696e 2074 6865 2064 6173  eport in the das
-00009ef0: 6862 6f61 7264 2e0a 2020 2020 2020 2020  hboard..        
-00009f00: 3a70 6172 616d 2064 6174 613a 2074 6865  :param data: the
-00009f10: 2064 6174 6120 6f66 2074 6865 2069 6e64   data of the ind
-00009f20: 6963 6174 6f72 0a20 2020 2020 2020 203a  icator.        :
-00009f30: 7061 7261 6d20 6f72 6465 723a 2074 6865  param order: the
-00009f40: 206f 7264 6572 206f 6620 7468 6520 696e   order of the in
-00009f50: 6469 6361 746f 720a 2020 2020 2020 2020  dicator.        
-00009f60: 3a63 6f6c 735f 7369 7a65 3a20 7468 6520  :cols_size: the 
-00009f70: 636f 6c75 6d6e 7320 7468 6174 2074 6865  columns that the
-00009f80: 2069 6e64 6963 6174 6f72 206f 6363 7570   indicator occup
-00009f90: 6965 730a 2020 2020 2020 2020 3a72 6f77  ies.        :row
-00009fa0: 735f 7369 7a65 3a20 7468 6520 726f 7773  s_size: the rows
-00009fb0: 2074 6861 7420 7468 6520 696e 6469 6361   that the indica
-00009fc0: 746f 7220 6f63 6375 7069 6573 0a20 2020  tor occupies.   
-00009fd0: 2020 2020 203a 7061 6464 696e 673a 2070       :padding: p
-00009fe0: 6164 6469 6e67 0a20 2020 2020 2020 2022  adding.        "
-00009ff0: 2222 0a20 2020 2020 2020 2061 7761 6974  "".        await
-0000a000: 2073 656c 662e 5f63 7265 6174 655f 6368   self._create_ch
-0000a010: 6172 7428 0a20 2020 2020 2020 2020 2020  art(.           
-0000a020: 2063 6861 7274 5f63 6c61 7373 3d49 6e64   chart_class=Ind
-0000a030: 6963 6174 6f72 2c0a 2020 2020 2020 2020  icator,.        
-0000a040: 2020 2020 7061 7468 3d73 656c 662e 5f63      path=self._c
-0000a050: 7572 7265 6e74 5f70 6174 682c 0a20 2020  urrent_path,.   
-0000a060: 2020 2020 2020 2020 206f 7264 6572 3d6f           order=o
-0000a070: 7264 6572 2c0a 2020 2020 2020 2020 2020  rder,.          
-0000a080: 2020 7369 7a65 5061 6464 696e 673d 7061    sizePadding=pa
-0000a090: 6464 696e 672c 0a20 2020 2020 2020 2020  dding,.         
-0000a0a0: 2020 2073 697a 6552 6f77 733d 726f 7773     sizeRows=rows
-0000a0b0: 5f73 697a 652c 0a20 2020 2020 2020 2020  _size,.         
-0000a0c0: 2020 2073 697a 6543 6f6c 756d 6e73 3d63     sizeColumns=c
-0000a0d0: 6f6c 735f 7369 7a65 2c0a 2020 2020 2020  ols_size,.      
-0000a0e0: 2020 2020 2020 7072 6f70 6572 7469 6573        properties
-0000a0f0: 3d64 6174 612c 0a20 2020 2020 2020 2029  =data,.        )
-0000a100: 0a0a 2020 2020 6465 6620 696e 6469 6361  ..    def indica
-0000a110: 746f 7228 0a20 2020 2020 2020 2073 656c  tor(.        sel
-0000a120: 662c 0a20 2020 2020 2020 2064 6174 613a  f,.        data:
-0000a130: 2055 6e69 6f6e 5b73 7472 2c20 7064 2e44   Union[str, pd.D
-0000a140: 6174 6146 7261 6d65 2c20 6c69 7374 5b64  ataFrame, list[d
-0000a150: 6963 745d 2c20 6469 6374 5d2c 0a20 2020  ict], dict],.   
-0000a160: 2020 2020 206f 7264 6572 3a20 696e 742c       order: int,
-0000a170: 0a20 2020 2020 2020 2076 6572 7469 6361  .        vertica
-0000a180: 6c3a 2055 6e69 6f6e 5b62 6f6f 6c2c 2073  l: Union[bool, s
-0000a190: 7472 5d20 3d20 4661 6c73 652c 0a20 2020  tr] = False,.   
-0000a1a0: 2020 2020 2063 6f6c 6f72 5f62 795f 7661       color_by_va
-0000a1b0: 6c75 653a 2062 6f6f 6c20 3d20 4661 6c73  lue: bool = Fals
-0000a1c0: 652c 0a20 2020 2020 2020 2063 6f6c 735f  e,.        cols_
-0000a1d0: 7369 7a65 3a20 696e 7420 3d20 3132 2c0a  size: int = 12,.
-0000a1e0: 2020 2020 2020 2020 726f 7773 5f73 697a          rows_siz
-0000a1f0: 653a 2069 6e74 203d 2031 2c0a 2020 2020  e: int = 1,.    
-0000a200: 2020 2020 7061 6464 696e 673a 204f 7074      padding: Opt
-0000a210: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
-0000a220: 652c 0a20 2020 2020 2020 202a 2a6b 7761  e,.        **kwa
-0000a230: 7267 732c 2020 2320 6d61 6b65 7320 6261  rgs,  # makes ba
-0000a240: 636b 7761 7264 7320 636f 6d70 6174 6962  ckwards compatib
-0000a250: 696c 6974 7920 6561 7369 6572 0a20 2020  ility easier.   
-0000a260: 2029 3a0a 2020 2020 2020 2020 2222 220a   ):.        """.
-0000a270: 2020 2020 2020 2020 4372 6561 7465 2061          Create a
-0000a280: 6e20 696e 6469 6361 746f 7220 7265 706f  n indicator repo
-0000a290: 7274 2069 6e20 7468 6520 6461 7368 626f  rt in the dashbo
-0000a2a0: 6172 642e 0a20 2020 2020 2020 203a 7061  ard..        :pa
-0000a2b0: 7261 6d20 6461 7461 3a20 7468 6520 6461  ram data: the da
-0000a2c0: 7461 206f 6620 7468 6520 696e 6469 6361  ta of the indica
-0000a2d0: 746f 720a 2020 2020 2020 2020 3a70 6172  tor.        :par
-0000a2e0: 616d 206f 7264 6572 3a20 7468 6520 6f72  am order: the or
-0000a2f0: 6465 7220 6f66 2074 6865 2069 6e64 6963  der of the indic
-0000a300: 6174 6f72 0a20 2020 2020 2020 203a 7061  ator.        :pa
-0000a310: 7261 6d20 7665 7274 6963 616c 3a20 7768  ram vertical: wh
-0000a320: 6574 6865 7220 7468 6520 696e 6469 6361  ether the indica
-0000a330: 746f 7220 6973 2076 6572 7469 6361 6c0a  tor is vertical.
-0000a340: 2020 2020 2020 2020 3a70 6172 616d 2063          :param c
-0000a350: 6f6c 6f72 5f62 795f 7661 6c75 653a 2077  olor_by_value: w
-0000a360: 6865 7468 6572 2074 6f20 636f 6c6f 7220  hether to color 
-0000a370: 7468 6520 696e 6469 6361 746f 7220 6279  the indicator by
-0000a380: 2076 616c 7565 0a20 2020 2020 2020 203a   value.        :
-0000a390: 636f 6c73 5f73 697a 653a 2074 6865 2063  cols_size: the c
-0000a3a0: 6f6c 756d 6e73 2074 6861 7420 7468 6520  olumns that the 
-0000a3b0: 696e 6469 6361 746f 7220 6f63 6375 7069  indicator occupi
-0000a3c0: 6573 0a20 2020 2020 2020 203a 726f 7773  es.        :rows
-0000a3d0: 5f73 697a 653a 2074 6865 2072 6f77 7320  _size: the rows 
-0000a3e0: 7468 6174 2074 6865 2069 6e64 6963 6174  that the indicat
-0000a3f0: 6f72 206f 6363 7570 6965 730a 2020 2020  or occupies.    
-0000a400: 2020 2020 3a70 6164 6469 6e67 3a20 7061      :padding: pa
-0000a410: 6464 696e 670a 2020 2020 2020 2020 3a74  dding.        :t
-0000a420: 6974 6c65 3a20 7468 6520 7469 746c 6520  itle: the title 
-0000a430: 6f66 2074 6865 2069 6e64 6963 6174 6f72  of the indicator
-0000a440: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0000a450: 2020 2020 2064 6620 3d20 7064 2e44 6174       df = pd.Dat
-0000a460: 6146 7261 6d65 2864 6174 6120 6966 2069  aFrame(data if i
-0000a470: 7369 6e73 7461 6e63 6528 6461 7461 2c20  sinstance(data, 
-0000a480: 6c69 7374 2920 656c 7365 205b 6461 7461  list) else [data
-0000a490: 5d29 0a20 2020 2020 2020 206b 6565 705f  ]).        keep_
-0000a4a0: 636f 6c75 6d6e 7320 3d20 5b0a 2020 2020  columns = [.    
-0000a4b0: 2020 2020 2020 2020 6b20 666f 7220 6b20          k for k 
-0000a4c0: 696e 2064 662e 636f 6c75 6d6e 7320 6966  in df.columns if
-0000a4d0: 206b 2069 6e20 6c69 7374 2849 6e64 6963   k in list(Indic
-0000a4e0: 6174 6f72 2e64 6566 6175 6c74 5f70 726f  ator.default_pro
-0000a4f0: 7065 7274 6965 732e 6b65 7973 2829 290a  perties.keys()).
-0000a500: 2020 2020 2020 2020 5d0a 2020 2020 2020          ].      
-0000a510: 2020 6466 203d 2064 665b 6b65 6570 5f63    df = df[keep_c
-0000a520: 6f6c 756d 6e73 5d0a 0a20 2020 2020 2020  olumns]..       
-0000a530: 206f 7269 6769 6e61 6c5f 7061 6464 696e   original_paddin
-0000a540: 6720 3d20 7061 6464 696e 670a 0a20 2020  g = padding..   
-0000a550: 2020 2020 206c 656e 5f64 6620 3d20 6c65       len_df = le
-0000a560: 6e28 6466 290a 2020 2020 2020 2020 6966  n(df).        if
-0000a570: 2076 6572 7469 6361 6c20 616e 6420 286c   vertical and (l
-0000a580: 656e 5f64 6620 3e20 3120 6f72 2069 7369  en_df > 1 or isi
-0000a590: 6e73 7461 6e63 6528 7665 7274 6963 616c  nstance(vertical
-0000a5a0: 2c20 7374 7229 293a 0a20 2020 2020 2020  , str)):.       
-0000a5b0: 2020 2020 2069 6620 7365 6c66 2e5f 6265       if self._be
-0000a5c0: 6e74 6f62 6f78 5f64 6174 613a 0a20 2020  ntobox_data:.   
-0000a5d0: 2020 2020 2020 2020 2020 2020 206c 6f67               log
-0000a5e0: 5f65 7272 6f72 280a 2020 2020 2020 2020  _error(.        
-0000a5f0: 2020 2020 2020 2020 2020 2020 6c6f 6767              logg
-0000a600: 6572 2c0a 2020 2020 2020 2020 2020 2020  er,.            
-0000a610: 2020 2020 2020 2020 2243 616e 6e6f 7420          "Cannot 
-0000a620: 6372 6561 7465 2076 6572 7469 6361 6c20  create vertical 
-0000a630: 696e 6469 6361 746f 7273 2069 6e20 6120  indicators in a 
-0000a640: 6265 6e74 6f62 6f78 222c 0a20 2020 2020  bentobox",.     
-0000a650: 2020 2020 2020 2020 2020 2020 2020 2052                 R
-0000a660: 756e 7469 6d65 4572 726f 722c 0a20 2020  untimeError,.   
-0000a670: 2020 2020 2020 2020 2020 2020 2029 0a0a               )..
-0000a680: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000a690: 2e73 6574 5f62 656e 746f 626f 7828 636f  .set_bentobox(co
-0000a6a0: 6c73 5f73 697a 653d 636f 6c73 5f73 697a  ls_size=cols_siz
-0000a6b0: 652c 2072 6f77 735f 7369 7a65 3d72 6f77  e, rows_size=row
-0000a6c0: 735f 7369 7a65 202a 206c 656e 5f64 6629  s_size * len_df)
-0000a6d0: 0a0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
-0000a6e0: 6669 7865 7864 2063 6f6c 735f 7369 7a65  fixexd cols_size
-0000a6f0: 2066 6f72 2062 656e 746f 626f 7820 616e   for bentobox an
-0000a700: 6420 7661 7269 6162 6c65 2072 6f77 7320  d variable rows 
-0000a710: 7369 7a65 0a20 2020 2020 2020 2020 2020  size.           
-0000a720: 2063 6f6c 735f 7369 7a65 203d 2032 320a   cols_size = 22.
-0000a730: 2020 2020 2020 2020 2020 2020 726f 7773              rows
-0000a740: 5f73 697a 6520 3d20 726f 7773 5f73 697a  _size = rows_siz
-0000a750: 6520 2a20 3130 202d 2032 0a0a 2020 2020  e * 10 - 2..    
-0000a760: 2020 2020 2020 2020 7061 6464 696e 6720          padding 
-0000a770: 3d20 2231 2c31 2c30 2c31 220a 2020 2020  = "1,1,0,1".    
-0000a780: 2020 2020 2020 2020 6966 2069 7369 6e73          if isins
-0000a790: 7461 6e63 6528 7665 7274 6963 616c 2c20  tance(vertical, 
-0000a7a0: 7374 7229 3a0a 2020 2020 2020 2020 2020  str):.          
-0000a7b0: 2020 2020 2020 6874 6d6c 203d 2066 223c        html = f"<
-0000a7c0: 6835 2073 7479 6c65 3d27 666f 6e74 2d66  h5 style='font-f
-0000a7d0: 616d 696c 793a 2052 7562 696b 273e 7b76  amily: Rubik'>{v
-0000a7e0: 6572 7469 6361 6c7d 3c2f 6835 3e22 0a20  ertical}</h5>". 
-0000a7f0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000a800: 656c 662e 6874 6d6c 280a 2020 2020 2020  elf.html(.      
-0000a810: 2020 2020 2020 2020 2020 2020 2020 6874                ht
-0000a820: 6d6c 3d68 746d 6c2c 0a20 2020 2020 2020  ml=html,.       
-0000a830: 2020 2020 2020 2020 2020 2020 206f 7264               ord
-0000a840: 6572 3d6f 7264 6572 2c0a 2020 2020 2020  er=order,.      
-0000a850: 2020 2020 2020 2020 2020 2020 2020 726f                ro
-0000a860: 7773 5f73 697a 653d 322c 0a20 2020 2020  ws_size=2,.     
-0000a870: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-0000a880: 6f6c 735f 7369 7a65 3d63 6f6c 735f 7369  ols_size=cols_si
-0000a890: 7a65 2c0a 2020 2020 2020 2020 2020 2020  ze,.            
-0000a8a0: 2020 2020 2020 2020 7061 6464 696e 673d          padding=
-0000a8b0: 7061 6464 696e 672c 0a20 2020 2020 2020  padding,.       
-0000a8c0: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-0000a8d0: 2020 2020 2020 2020 2020 206f 7264 6572             order
-0000a8e0: 202b 3d20 310a 2020 2020 2020 2020 656c   += 1.        el
-0000a8f0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-0000a900: 6265 6e74 6f62 6f78 5f64 6174 6120 3d20  bentobox_data = 
-0000a910: 7365 6c66 2e5f 6265 6e74 6f62 6f78 5f64  self._bentobox_d
-0000a920: 6174 610a 2020 2020 2020 2020 2020 2020  ata.            
-0000a930: 6966 2070 6164 6469 6e67 2069 7320 4e6f  if padding is No
-0000a940: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0000a950: 2020 2020 7061 6464 696e 6720 3d20 2230      padding = "0
-0000a960: 2c30 2c30 2c30 220a 0a20 2020 2020 2020  ,0,0,0"..       
-0000a970: 2020 2020 2070 6164 6469 6e67 203d 2070       padding = p
-0000a980: 6164 6469 6e67 2e72 6570 6c61 6365 2822  adding.replace("
-0000a990: 2022 2c20 2222 290a 0a20 2020 2020 2020   ", "")..       
-0000a9a0: 2020 2020 2072 656d 6169 6e69 6e67 5f63       remaining_c
-0000a9b0: 6f6c 7320 3d20 636f 6c73 5f73 697a 6520  ols = cols_size 
-0000a9c0: 2520 6c65 6e5f 6466 0a0a 2020 2020 2020  % len_df..      
-0000a9d0: 2020 2020 2020 6578 7472 615f 7061 6464        extra_padd
-0000a9e0: 696e 6720 3d20 7265 6d61 696e 696e 675f  ing = remaining_
-0000a9f0: 636f 6c73 202f 2f20 320a 2020 2020 2020  cols // 2.      
-0000aa00: 2020 2020 2020 7061 6464 696e 675f 6c65        padding_le
-0000aa10: 6674 5f69 6e74 203d 2069 6e74 2870 6164  ft_int = int(pad
-0000aa20: 6469 6e67 5b36 5d29 202b 2065 7874 7261  ding[6]) + extra
-0000aa30: 5f70 6164 6469 6e67 0a20 2020 2020 2020  _padding.       
-0000aa40: 2020 2020 2070 6164 6469 6e67 5f72 6967       padding_rig
-0000aa50: 6874 5f69 6e74 203d 2069 6e74 2870 6164  ht_int = int(pad
-0000aa60: 6469 6e67 5b32 5d29 202b 2065 7874 7261  ding[2]) + extra
-0000aa70: 5f70 6164 6469 6e67 202b 2072 656d 6169  _padding + remai
-0000aa80: 6e69 6e67 5f63 6f6c 7320 2520 320a 0a20  ning_cols % 2.. 
-0000aa90: 2020 2020 2020 2020 2020 2070 6164 6469             paddi
-0000aaa0: 6e67 5f6c 6566 7420 3d20 6622 7b70 6164  ng_left = f"{pad
-0000aab0: 6469 6e67 5b30 5d7d 2c30 2c7b 7061 6464  ding[0]},0,{padd
-0000aac0: 696e 675b 345d 7d2c 7b70 6164 6469 6e67  ing[4]},{padding
-0000aad0: 5f6c 6566 745f 696e 747d 220a 2020 2020  _left_int}".    
-0000aae0: 2020 2020 2020 2020 7061 6464 696e 675f          padding_
-0000aaf0: 7269 6768 7420 3d20 6622 7b70 6164 6469  right = f"{paddi
-0000ab00: 6e67 5b30 5d7d 2c7b 7061 6464 696e 675f  ng[0]},{padding_
-0000ab10: 7269 6768 745f 696e 747d 2c7b 7061 6464  right_int},{padd
-0000ab20: 696e 675b 345d 7d2c 7b69 6e74 2862 6f6f  ing[4]},{int(boo
-0000ab30: 6c28 6265 6e74 6f62 6f78 5f64 6174 6129  l(bentobox_data)
-0000ab40: 297d 220a 2020 2020 2020 2020 2020 2020  )}".            
-0000ab50: 7061 6464 696e 675f 656c 7365 203d 2066  padding_else = f
-0000ab60: 227b 7061 6464 696e 675b 305d 7d2c 302c  "{padding[0]},0,
-0000ab70: 7b70 6164 6469 6e67 5b34 5d7d 2c7b 696e  {padding[4]},{in
-0000ab80: 7428 626f 6f6c 2862 656e 746f 626f 785f  t(bool(bentobox_
-0000ab90: 6461 7461 2929 7d22 0a0a 2020 2020 2020  data))}"..      
-0000aba0: 2020 2020 2020 636f 6c73 5f73 697a 6520        cols_size 
-0000abb0: 3d20 636f 6c73 5f73 697a 6520 2f2f 206c  = cols_size // l
-0000abc0: 656e 5f64 6620 2d20 696e 7428 626f 6f6c  en_df - int(bool
-0000abd0: 2862 656e 746f 626f 785f 6461 7461 2929  (bentobox_data))
-0000abe0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-0000abf0: 636f 6c73 5f73 697a 6520 3c20 323a 0a20  cols_size < 2:. 
-0000ac00: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-0000ac10: 6f67 5f65 7272 6f72 280a 2020 2020 2020  og_error(.      
-0000ac20: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
-0000ac30: 6767 6572 2c0a 2020 2020 2020 2020 2020  gger,.          
-0000ac40: 2020 2020 2020 2020 2020 6622 5468 6520            f"The 
-0000ac50: 6361 6c63 756c 6174 696f 6e20 6f66 2074  calculation of t
-0000ac60: 6865 2069 6e64 6976 6964 7561 6c20 636f  he individual co
-0000ac70: 6c73 5f73 697a 6520 666f 7220 6561 6368  ls_size for each
-0000ac80: 2069 6e64 6963 6174 6f72 2022 0a20 2020   indicator ".   
-0000ac90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000aca0: 2066 2269 7320 746f 6f20 736d 616c 6c20   f"is too small 
-0000acb0: 2863 6f6c 735f 7369 7a65 2f6c 656e 2864  (cols_size/len(d
-0000acc0: 6629 293a 207b 636f 6c73 5f73 697a 657d  f)): {cols_size}
-0000acd0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-0000ace0: 2020 2020 2020 2056 616c 7565 4572 726f         ValueErro
-0000acf0: 722c 0a20 2020 2020 2020 2020 2020 2020  r,.             
-0000ad00: 2020 2029 0a0a 2020 2020 2020 2020 6c61     )..        la
-0000ad10: 7374 5f69 6e64 6578 203d 2064 662e 696e  st_index = df.in
-0000ad20: 6465 785b 2d31 5d0a 2020 2020 2020 2020  dex[-1].        
-0000ad30: 6669 7273 745f 696e 6465 7820 3d20 6466  first_index = df
-0000ad40: 2e69 6e64 6578 5b30 5d0a 0a20 2020 2020  .index[0]..     
-0000ad50: 2020 2066 6f72 2069 6e64 6578 2c20 6466     for index, df
-0000ad60: 5f72 6f77 2069 6e20 6466 2e69 7465 7272  _row in df.iterr
-0000ad70: 6f77 7328 293a 0a20 2020 2020 2020 2020  ows():.         
-0000ad80: 2020 2069 6620 6e6f 7420 7665 7274 6963     if not vertic
-0000ad90: 616c 3a0a 2020 2020 2020 2020 2020 2020  al:.            
-0000ada0: 2020 2020 6966 2069 6e64 6578 203d 3d20      if index == 
-0000adb0: 6669 7273 745f 696e 6465 7820 616e 6420  first_index and 
-0000adc0: 696e 6465 7820 3d3d 206c 6173 745f 696e  index == last_in
-0000add0: 6465 783a 0a20 2020 2020 2020 2020 2020  dex:.           
-0000ade0: 2020 2020 2020 2020 2070 6164 6469 6e67           padding
-0000adf0: 203d 206f 7269 6769 6e61 6c5f 7061 6464   = original_padd
-0000ae00: 696e 670a 2020 2020 2020 2020 2020 2020  ing.            
-0000ae10: 2020 2020 656c 6966 2069 6e64 6578 203d      elif index =
-0000ae20: 3d20 6669 7273 745f 696e 6465 783a 0a20  = first_index:. 
-0000ae30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ae40: 2020 2070 6164 6469 6e67 203d 2070 6164     padding = pad
-0000ae50: 6469 6e67 5f6c 6566 740a 2020 2020 2020  ding_left.      
-0000ae60: 2020 2020 2020 2020 2020 656c 6966 2069            elif i
-0000ae70: 6e64 6578 203d 3d20 6c61 7374 5f69 6e64  ndex == last_ind
-0000ae80: 6578 3a0a 2020 2020 2020 2020 2020 2020  ex:.            
-0000ae90: 2020 2020 2020 2020 7061 6464 696e 6720          padding 
-0000aea0: 3d20 7061 6464 696e 675f 7269 6768 740a  = padding_right.
-0000aeb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000aec0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-0000aed0: 2020 2020 2020 2020 2020 7061 6464 696e            paddin
-0000aee0: 6720 3d20 7061 6464 696e 675f 656c 7365  g = padding_else
-0000aef0: 0a20 2020 2020 2020 2020 2020 2065 6c69  .            eli
-0000af00: 6620 280a 2020 2020 2020 2020 2020 2020  f (.            
-0000af10: 2020 2020 696e 6465 7820 3d3d 206c 6173      index == las
-0000af20: 745f 696e 6465 780a 2020 2020 2020 2020  t_index.        
-0000af30: 2020 2020 2020 2020 616e 6420 7665 7274          and vert
-0000af40: 6963 616c 0a20 2020 2020 2020 2020 2020  ical.           
-0000af50: 2020 2020 2061 6e64 2028 6c65 6e5f 6466       and (len_df
-0000af60: 203e 2031 206f 7220 6973 696e 7374 616e   > 1 or isinstan
-0000af70: 6365 2876 6572 7469 6361 6c2c 2073 7472  ce(vertical, str
-0000af80: 2929 0a20 2020 2020 2020 2020 2020 2029  )).            )
-0000af90: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000afa0: 2020 7061 6464 696e 6720 3d20 2231 2c31    padding = "1,1
-0000afb0: 2c31 2c31 220a 0a20 2020 2020 2020 2020  ,1,1"..         
-0000afc0: 2020 2069 6620 636f 6c6f 725f 6279 5f76     if color_by_v
-0000afd0: 616c 7565 2061 6e64 2022 636f 6c6f 7222  alue and "color"
-0000afe0: 206e 6f74 2069 6e20 6466 5f72 6f77 2061   not in df_row a
-0000aff0: 6e64 2022 6963 6f6e 2220 6e6f 7420 696e  nd "icon" not in
-0000b000: 2064 665f 726f 773a 0a20 2020 2020 2020   df_row:.       
-0000b010: 2020 2020 2020 2020 2064 665f 726f 775b           df_row[
-0000b020: 2263 6f6c 6f72 225d 203d 2028 0a20 2020  "color"] = (.   
-0000b030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b040: 2022 7375 6363 6573 7322 0a20 2020 2020   "success".     
-0000b050: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0000b060: 6620 6466 5f72 6f77 5b22 7661 6c75 6522  f df_row["value"
-0000b070: 5d20 3e20 300a 2020 2020 2020 2020 2020  ] > 0.          
-0000b080: 2020 2020 2020 2020 2020 656c 7365 2022            else "
-0000b090: 6572 726f 7222 0a20 2020 2020 2020 2020  error".         
-0000b0a0: 2020 2020 2020 2020 2020 2069 6620 6466             if df
-0000b0b0: 5f72 6f77 5b22 7661 6c75 6522 5d20 3c20  _row["value"] < 
-0000b0c0: 300a 2020 2020 2020 2020 2020 2020 2020  0.              
-0000b0d0: 2020 2020 2020 656c 7365 2022 6e65 7574        else "neut
-0000b0e0: 7261 6c22 0a20 2020 2020 2020 2020 2020  ral".           
-0000b0f0: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
-0000b100: 2020 2020 2020 2064 665f 726f 775b 2269         df_row["i
-0000b110: 636f 6e22 5d20 3d20 280a 2020 2020 2020  con"] = (.      
-0000b120: 2020 2020 2020 2020 2020 2020 2020 224c                "L
-0000b130: 696e 652f 6172 726f 772d 7570 220a 2020  ine/arrow-up".  
+00000030: 6173 206e 700a 0a66 726f 6d20 6461 7461  as np..from data
+00000040: 636c 6173 7365 7320 696d 706f 7274 2064  classes import d
+00000050: 6174 6163 6c61 7373 0a66 726f 6d20 636f  ataclass.from co
+00000060: 7079 2069 6d70 6f72 7420 6465 6570 636f  py import deepco
+00000070: 7079 0a0a 6672 6f6d 2070 616e 6461 7320  py..from pandas 
+00000080: 696d 706f 7274 2044 6174 6146 7261 6d65  import DataFrame
+00000090: 0a66 726f 6d20 6d61 7468 2069 6d70 6f72  .from math impor
+000000a0: 7420 6365 696c 0a66 726f 6d20 7368 696d  t ceil.from shim
+000000b0: 6f6b 752e 6173 796e 635f 6578 6563 7574  oku.async_execut
+000000c0: 696f 6e5f 706f 6f6c 2069 6d70 6f72 7420  ion_pool import 
+000000d0: 280a 2020 2020 4175 746f 4173 796e 6345  (.    AutoAsyncE
+000000e0: 7865 6375 7469 6f6e 506f 6f6c 2c0a 2020  xecutionPool,.  
+000000f0: 2020 6164 645f 746f 5f67 656e 6572 616c    add_to_general
+00000100: 5f61 7379 6e63 5f67 726f 7570 2c0a 290a  _async_group,.).
+00000110: 0a66 726f 6d20 7479 7069 6e67 2069 6d70  .from typing imp
+00000120: 6f72 7420 4f70 7469 6f6e 616c 2c20 556e  ort Optional, Un
+00000130: 696f 6e0a 0a66 726f 6d20 7368 696d 6f6b  ion..from shimok
+00000140: 752e 7574 696c 7320 696d 706f 7274 2045  u.utils import E
+00000150: 7665 6e74 5479 7065 0a0a 6672 6f6d 2073  ventType..from s
+00000160: 6869 6d6f 6b75 2e61 7069 2e72 6573 6f75  himoku.api.resou
+00000170: 7263 6573 2e61 7070 2069 6d70 6f72 7420  rces.app import 
+00000180: 4170 700a 6672 6f6d 2073 6869 6d6f 6b75  App.from shimoku
+00000190: 2e61 7069 2e72 6573 6f75 7263 6573 2e62  .api.resources.b
+000001a0: 7573 696e 6573 7320 696d 706f 7274 2042  usiness import B
+000001b0: 7573 696e 6573 730a 6672 6f6d 2073 6869  usiness.from shi
+000001c0: 6d6f 6b75 2e61 7069 2e72 6573 6f75 7263  moku.api.resourc
+000001d0: 6573 2e72 6570 6f72 7420 696d 706f 7274  es.report import
+000001e0: 2052 6570 6f72 740a 6672 6f6d 2073 6869   Report.from shi
+000001f0: 6d6f 6b75 2e61 7069 2e72 6573 6f75 7263  moku.api.resourc
+00000200: 6573 2e64 6174 615f 7365 7420 696d 706f  es.data_set impo
+00000210: 7274 2028 0a20 2020 2044 6174 6153 6574  rt (.    DataSet
+00000220: 2c0a 2020 2020 4d61 7070 696e 672c 0a20  ,.    Mapping,. 
+00000230: 2020 2063 6f6e 7665 7274 5f69 6e70 7574     convert_input
+00000240: 5f64 6174 615f 746f 5f64 625f 6974 656d  _data_to_db_item
+00000250: 732c 0a20 2020 2063 6f6e 7665 7274 5f64  s,.    convert_d
+00000260: 6174 615f 616e 645f 6765 745f 7365 7269  ata_and_get_seri
+00000270: 6573 5f6e 616d 652c 0a29 0a66 726f 6d20  es_name,.).from 
+00000280: 7368 696d 6f6b 752e 6170 692e 7265 736f  shimoku.api.reso
+00000290: 7572 6365 732e 7265 706f 7274 732e 6669  urces.reports.fi
+000002a0: 6c74 6572 5f64 6174 615f 7365 7420 696d  lter_data_set im
+000002b0: 706f 7274 2046 696c 7465 7244 6174 6153  port FilterDataS
+000002c0: 6574 0a66 726f 6d20 7368 696d 6f6b 752e  et.from shimoku.
+000002d0: 6170 692e 7265 736f 7572 6365 732e 7265  api.resources.re
+000002e0: 706f 7274 732e 7461 6273 5f67 726f 7570  ports.tabs_group
+000002f0: 2069 6d70 6f72 7420 5461 6273 4772 6f75   import TabsGrou
+00000300: 700a 6672 6f6d 2073 6869 6d6f 6b75 2e61  p.from shimoku.a
+00000310: 7069 2e72 6573 6f75 7263 6573 2e72 6570  pi.resources.rep
+00000320: 6f72 7473 2e6d 6f64 616c 2069 6d70 6f72  orts.modal impor
+00000330: 7420 4d6f 6461 6c0a 6672 6f6d 2073 6869  t Modal.from shi
+00000340: 6d6f 6b75 2e61 7069 2e72 6573 6f75 7263  moku.api.resourc
+00000350: 6573 2e72 6570 6f72 7473 2e63 6861 7274  es.reports.chart
+00000360: 732e 696e 6469 6361 746f 7220 696d 706f  s.indicator impo
+00000370: 7274 2049 6e64 6963 6174 6f72 0a66 726f  rt Indicator.fro
+00000380: 6d20 7368 696d 6f6b 752e 6170 692e 7265  m shimoku.api.re
+00000390: 736f 7572 6365 732e 7265 706f 7274 732e  sources.reports.
+000003a0: 6368 6172 7473 2e65 6368 6172 7420 696d  charts.echart im
+000003b0: 706f 7274 2045 4368 6172 740a 6672 6f6d  port EChart.from
+000003c0: 2073 6869 6d6f 6b75 2e61 7069 2e72 6573   shimoku.api.res
+000003d0: 6f75 7263 6573 2e72 6570 6f72 7473 2e63  ources.reports.c
+000003e0: 6861 7274 732e 7461 626c 6520 696d 706f  harts.table impo
+000003f0: 7274 2054 6162 6c65 2c20 696e 7465 7270  rt Table, interp
+00000400: 7265 745f 6c61 6265 6c5f 696e 666f 0a66  ret_label_info.f
+00000410: 726f 6d20 7368 696d 6f6b 752e 6170 692e  rom shimoku.api.
+00000420: 7265 736f 7572 6365 732e 7265 706f 7274  resources.report
+00000430: 732e 6368 6172 7473 2e61 6e6e 6f74 6174  s.charts.annotat
+00000440: 6564 5f63 6861 7274 2069 6d70 6f72 7420  ed_chart import 
+00000450: 416e 6e6f 7461 7465 6445 4368 6172 740a  AnnotatedEChart.
+00000460: 6672 6f6d 2073 6869 6d6f 6b75 2e61 7069  from shimoku.api
+00000470: 2e72 6573 6f75 7263 6573 2e72 6570 6f72  .resources.repor
+00000480: 7473 2e63 6861 7274 732e 6874 6d6c 2069  ts.charts.html i
+00000490: 6d70 6f72 7420 4854 4d4c 0a66 726f 6d20  mport HTML.from 
+000004a0: 7368 696d 6f6b 752e 6170 692e 7265 736f  shimoku.api.reso
+000004b0: 7572 6365 732e 7265 706f 7274 732e 6368  urces.reports.ch
+000004c0: 6172 7473 2e62 7574 746f 6e20 696d 706f  arts.button impo
+000004d0: 7274 2042 7574 746f 6e0a 6672 6f6d 2073  rt Button.from s
+000004e0: 6869 6d6f 6b75 2e61 7069 2e72 6573 6f75  himoku.api.resou
+000004f0: 7263 6573 2e72 6570 6f72 7473 2e63 6861  rces.reports.cha
+00000500: 7274 732e 696e 7075 745f 666f 726d 2069  rts.input_form i
+00000510: 6d70 6f72 7420 496e 7075 7446 6f72 6d0a  mport InputForm.
+00000520: 6672 6f6d 2073 6869 6d6f 6b75 2e61 7069  from shimoku.api
+00000530: 2e72 6573 6f75 7263 6573 2e72 6570 6f72  .resources.repor
+00000540: 7473 2e63 6861 7274 732e 6966 7261 6d65  ts.charts.iframe
+00000550: 2069 6d70 6f72 7420 4946 7261 6d65 0a66   import IFrame.f
+00000560: 726f 6d20 7368 696d 6f6b 752e 706c 742e  rom shimoku.plt.
+00000570: 4543 6861 7274 5f64 6566 696e 6974 696f  EChart_definitio
+00000580: 6e73 2e6c 696e 6520 696d 706f 7274 2028  ns.line import (
+00000590: 0a20 2020 206c 696e 655f 6368 6172 742c  .    line_chart,
+000005a0: 0a20 2020 2061 7265 615f 6368 6172 742c  .    area_chart,
+000005b0: 0a20 2020 2073 7461 636b 6564 5f61 7265  .    stacked_are
+000005c0: 615f 6368 6172 742c 0a20 2020 2070 7265  a_chart,.    pre
+000005d0: 6469 6374 6976 655f 6c69 6e65 5f63 6861  dictive_line_cha
+000005e0: 7274 2c0a 2020 2020 6d61 726b 6564 5f6c  rt,.    marked_l
+000005f0: 696e 655f 6368 6172 742c 0a20 2020 2073  ine_chart,.    s
+00000600: 6567 6d65 6e74 6564 5f61 7265 615f 6368  egmented_area_ch
+00000610: 6172 742c 0a20 2020 206c 696e 655f 7769  art,.    line_wi
+00000620: 7468 5f63 6f6e 6669 6465 6e63 655f 6172  th_confidence_ar
+00000630: 6561 5f63 6861 7274 2c0a 2020 2020 7365  ea_chart,.    se
+00000640: 676d 656e 7465 645f 6c69 6e65 5f63 6861  gmented_line_cha
+00000650: 7274 2c0a 290a 6672 6f6d 2073 6869 6d6f  rt,.).from shimo
+00000660: 6b75 2e70 6c74 2e45 4368 6172 745f 6465  ku.plt.EChart_de
+00000670: 6669 6e69 7469 6f6e 732e 6261 7220 696d  finitions.bar im
+00000680: 706f 7274 2028 0a20 2020 2062 6172 5f63  port (.    bar_c
+00000690: 6861 7274 2c0a 2020 2020 7374 6163 6b65  hart,.    stacke
+000006a0: 645f 6261 725f 6368 6172 742c 0a20 2020  d_bar_chart,.   
+000006b0: 2068 6f72 697a 6f6e 7461 6c5f 6261 725f   horizontal_bar_
+000006c0: 6368 6172 742c 0a20 2020 2073 7461 636b  chart,.    stack
+000006d0: 6564 5f68 6f72 697a 6f6e 7461 6c5f 6261  ed_horizontal_ba
+000006e0: 725f 6368 6172 742c 0a20 2020 207a 6572  r_chart,.    zer
+000006f0: 6f5f 6365 6e74 6572 6564 5f62 6172 5f63  o_centered_bar_c
+00000700: 6861 7274 2c0a 290a 6672 6f6d 2073 6869  hart,.).from shi
+00000710: 6d6f 6b75 2e70 6c74 2e45 4368 6172 745f  moku.plt.EChart_
+00000720: 6465 6669 6e69 7469 6f6e 732e 7363 6174  definitions.scat
+00000730: 7465 7220 696d 706f 7274 2028 0a20 2020  ter import (.   
+00000740: 2073 6361 7474 6572 5f63 6861 7274 2c0a   scatter_chart,.
+00000750: 2020 2020 7363 6174 7465 725f 7769 7468      scatter_with
+00000760: 5f65 6666 6563 745f 6368 6172 742c 0a29  _effect_chart,.)
+00000770: 0a66 726f 6d20 7368 696d 6f6b 752e 706c  .from shimoku.pl
+00000780: 742e 4543 6861 7274 5f64 6566 696e 6974  t.EChart_definit
+00000790: 696f 6e73 2e66 756e 6e65 6c20 696d 706f  ions.funnel impo
+000007a0: 7274 2066 756e 6e65 6c5f 6368 6172 740a  rt funnel_chart.
+000007b0: 6672 6f6d 2073 6869 6d6f 6b75 2e70 6c74  from shimoku.plt
+000007c0: 2e45 4368 6172 745f 6465 6669 6e69 7469  .EChart_definiti
+000007d0: 6f6e 732e 7472 6565 2069 6d70 6f72 7420  ons.tree import 
+000007e0: 7472 6565 5f63 6861 7274 0a66 726f 6d20  tree_chart.from 
+000007f0: 7368 696d 6f6b 752e 706c 742e 4543 6861  shimoku.plt.ECha
+00000800: 7274 5f64 6566 696e 6974 696f 6e73 2e72  rt_definitions.r
+00000810: 6164 6172 2069 6d70 6f72 7420 7261 6461  adar import rada
+00000820: 725f 6368 6172 740a 6672 6f6d 2073 6869  r_chart.from shi
+00000830: 6d6f 6b75 2e70 6c74 2e45 4368 6172 745f  moku.plt.EChart_
+00000840: 6465 6669 6e69 7469 6f6e 732e 7069 6520  definitions.pie 
+00000850: 696d 706f 7274 2070 6965 5f63 6861 7274  import pie_chart
+00000860: 2c20 646f 7567 686e 7574 5f63 6861 7274  , doughnut_chart
+00000870: 2c20 726f 7365 5f63 6861 7274 0a66 726f  , rose_chart.fro
+00000880: 6d20 7368 696d 6f6b 752e 706c 742e 4543  m shimoku.plt.EC
+00000890: 6861 7274 5f64 6566 696e 6974 696f 6e73  hart_definitions
+000008a0: 2e67 6175 6765 2069 6d70 6f72 7420 7370  .gauge import sp
+000008b0: 6565 645f 6761 7567 655f 6368 6172 740a  eed_gauge_chart.
+000008c0: 6672 6f6d 2073 6869 6d6f 6b75 2e70 6c74  from shimoku.plt
+000008d0: 2e45 4368 6172 745f 6465 6669 6e69 7469  .EChart_definiti
+000008e0: 6f6e 732e 7368 696d 6f6b 755f 6761 7567  ons.shimoku_gaug
+000008f0: 6520 696d 706f 7274 2028 0a20 2020 2073  e import (.    s
+00000900: 6869 6d6f 6b75 5f67 6175 6765 5f63 6861  himoku_gauge_cha
+00000910: 7274 2c0a 2020 2020 7368 696d 6f6b 755f  rt,.    shimoku_
+00000920: 6761 7567 6573 5f67 726f 7570 2c0a 290a  gauges_group,.).
+00000930: 6672 6f6d 2073 6869 6d6f 6b75 2e70 6c74  from shimoku.plt
+00000940: 2e45 4368 6172 745f 6465 6669 6e69 7469  .EChart_definiti
+00000950: 6f6e 732e 7375 6e62 7572 7374 2069 6d70  ons.sunburst imp
+00000960: 6f72 7420 7375 6e62 7572 7374 5f63 6861  ort sunburst_cha
+00000970: 7274 0a66 726f 6d20 7368 696d 6f6b 752e  rt.from shimoku.
+00000980: 706c 742e 4543 6861 7274 5f64 6566 696e  plt.EChart_defin
+00000990: 6974 696f 6e73 2e74 7265 656d 6170 2069  itions.treemap i
+000009a0: 6d70 6f72 7420 7472 6565 6d61 705f 6368  mport treemap_ch
+000009b0: 6172 740a 6672 6f6d 2073 6869 6d6f 6b75  art.from shimoku
+000009c0: 2e70 6c74 2e45 4368 6172 745f 6465 6669  .plt.EChart_defi
+000009d0: 6e69 7469 6f6e 732e 7361 6e6b 6579 2069  nitions.sankey i
+000009e0: 6d70 6f72 7420 7361 6e6b 6579 5f63 6861  mport sankey_cha
+000009f0: 7274 0a66 726f 6d20 7368 696d 6f6b 752e  rt.from shimoku.
+00000a00: 706c 742e 4543 6861 7274 5f64 6566 696e  plt.EChart_defin
+00000a10: 6974 696f 6e73 2e68 6561 746d 6170 2069  itions.heatmap i
+00000a20: 6d70 6f72 7420 6865 6174 6d61 705f 6368  mport heatmap_ch
+00000a30: 6172 740a 6672 6f6d 2073 6869 6d6f 6b75  art.from shimoku
+00000a40: 2e70 6c74 2e45 4368 6172 745f 6465 6669  .plt.EChart_defi
+00000a50: 6e69 7469 6f6e 732e 6761 7567 655f 696e  nitions.gauge_in
+00000a60: 6469 6361 746f 7220 696d 706f 7274 2067  dicator import g
+00000a70: 6175 6765 5f69 6e64 6963 6174 6f72 0a66  auge_indicator.f
+00000a80: 726f 6d20 7368 696d 6f6b 752e 706c 742e  rom shimoku.plt.
+00000a90: 4543 6861 7274 5f64 6566 696e 6974 696f  EChart_definitio
+00000aa0: 6e73 2e74 6f70 5f62 6f74 746f 6d20 696d  ns.top_bottom im
+00000ab0: 706f 7274 2028 0a20 2020 2074 6f70 5f62  port (.    top_b
+00000ac0: 6f74 746f 6d5f 6172 6561 5f63 6861 7274  ottom_area_chart
+00000ad0: 732c 0a20 2020 2074 6f70 5f62 6f74 746f  s,.    top_botto
+00000ae0: 6d5f 6c69 6e65 5f63 6861 7274 732c 0a29  m_line_charts,.)
+00000af0: 0a66 726f 6d20 7368 696d 6f6b 752e 706c  .from shimoku.pl
+00000b00: 742e 4543 6861 7274 5f64 6566 696e 6974  t.EChart_definit
+00000b10: 696f 6e73 2e77 6174 6572 6661 6c6c 2069  ions.waterfall i
+00000b20: 6d70 6f72 7420 7761 7465 7266 616c 6c5f  mport waterfall_
+00000b30: 6368 6172 740a 6672 6f6d 2073 6869 6d6f  chart.from shimo
+00000b40: 6b75 2e70 6c74 2e45 4368 6172 745f 6465  ku.plt.EChart_de
+00000b50: 6669 6e69 7469 6f6e 732e 6c69 6e65 5f61  finitions.line_a
+00000b60: 6e64 5f62 6172 2069 6d70 6f72 7420 6c69  nd_bar import li
+00000b70: 6e65 5f61 6e64 5f62 6172 5f63 6861 7274  ne_and_bar_chart
+00000b80: 730a 6672 6f6d 2073 6869 6d6f 6b75 2e70  s.from shimoku.p
+00000b90: 6c74 2e62 656e 746f 626f 785f 6368 6172  lt.bentobox_char
+00000ba0: 7473 2069 6d70 6f72 7420 280a 2020 2020  ts import (.    
+00000bb0: 6368 6172 745f 616e 645f 6d6f 6461 6c5f  chart_and_modal_
+00000bc0: 6275 7474 6f6e 2c0a 2020 2020 696e 666f  button,.    info
+00000bd0: 6772 6170 6869 6373 5f74 6578 745f 6275  graphics_text_bu
+00000be0: 6262 6c65 2c0a 2020 2020 696e 6469 6361  bble,.    indica
+00000bf0: 746f 7273 5f77 6974 685f 6865 6164 6572  tors_with_header
+00000c00: 2c0a 2020 2020 6368 6172 745f 616e 645f  ,.    chart_and_
+00000c10: 696e 6469 6361 746f 7273 2c0a 2020 2020  indicators,.    
+00000c20: 6c69 6e65 5f77 6974 685f 7375 6d6d 6172  line_with_summar
+00000c30: 792c 0a29 0a0a 6672 6f6d 2073 6869 6d6f  y,.)..from shimo
+00000c40: 6b75 2e65 7863 6570 7469 6f6e 7320 696d  ku.exceptions im
+00000c50: 706f 7274 2054 6162 7345 7272 6f72 2c20  port TabsError, 
+00000c60: 4d6f 6461 6c45 7272 6f72 2c20 4461 7461  ModalError, Data
+00000c70: 4572 726f 722c 2042 656e 746f 626f 7845  Error, BentoboxE
+00000c80: 7272 6f72 0a66 726f 6d20 7368 696d 6f6b  rror.from shimok
+00000c90: 752e 706c 742e 7574 696c 7320 696d 706f  u.plt.utils impo
+00000ca0: 7274 2028 0a20 2020 2064 6565 705f 7570  rt (.    deep_up
+00000cb0: 6461 7465 2c0a 2020 2020 6765 745f 7575  date,.    get_uu
+00000cc0: 6964 735f 6672 6f6d 5f64 6963 742c 0a20  ids_from_dict,. 
+00000cd0: 2020 2067 6574 5f64 6174 615f 7265 6665     get_data_refe
+00000ce0: 7265 6e63 6573 5f66 726f 6d5f 6469 6374  rences_from_dict
+00000cf0: 2c0a 2020 2020 7661 6c69 6461 7465 5f64  ,.    validate_d
+00000d00: 6174 615f 6973 5f70 616e 6461 7261 626c  ata_is_pandarabl
+00000d10: 652c 0a20 2020 2061 6464 5f73 6f72 7469  e,.    add_sorti
+00000d20: 6e67 5f74 6f5f 6466 2c0a 2020 2020 7472  ng_to_df,.    tr
+00000d30: 616e 7366 6f72 6d5f 6469 6374 5f6a 735f  ansform_dict_js_
+00000d40: 746f 5f70 792c 0a20 2020 2072 6574 7269  to_py,.    retri
+00000d50: 6576 655f 6461 7461 5f66 726f 6d5f 6f70  eve_data_from_op
+00000d60: 7469 6f6e 732c 0a20 2020 2076 616c 6964  tions,.    valid
+00000d70: 6174 655f 696e 7075 745f 666f 726d 5f64  ate_input_form_d
+00000d80: 6174 612c 0a20 2020 2063 7265 6174 655f  ata,.    create_
+00000d90: 6e6f 726d 616c 697a 6564 5f6e 616d 652c  normalized_name,
+00000da0: 0a29 0a0a 696d 706f 7274 206c 6f67 6769  .)..import loggi
+00000db0: 6e67 0a66 726f 6d20 7368 696d 6f6b 752e  ng.from shimoku.
+00000dc0: 6578 6563 7574 696f 6e5f 6c6f 6767 6572  execution_logger
+00000dd0: 2069 6d70 6f72 7420 6c6f 675f 6572 726f   import log_erro
+00000de0: 722c 2043 6c61 7373 5769 7468 4c6f 6767  r, ClassWithLogg
+00000df0: 696e 670a 0a6c 6f67 6765 7220 3d20 6c6f  ing..logger = lo
+00000e00: 6767 696e 672e 6765 744c 6f67 6765 7228  gging.getLogger(
+00000e10: 5f5f 6e61 6d65 5f5f 290a 0a0a 636c 6173  __name__)...clas
+00000e20: 7320 506c 6f74 4c61 7965 7228 436c 6173  s PlotLayer(Clas
+00000e30: 7357 6974 684c 6f67 6769 6e67 293a 0a20  sWithLogging):. 
+00000e40: 2020 2022 2222 0a20 2020 2054 6869 7320     """.    This 
+00000e50: 636c 6173 7320 6973 2061 2068 6967 6820  class is a high 
+00000e60: 6c65 7665 6c20 6162 7374 7261 6374 696f  level abstractio
+00000e70: 6e20 6f66 2074 6865 2041 5049 2c20 6974  n of the API, it
+00000e80: 2069 7320 7573 6564 2074 6f20 6372 6561   is used to crea
+00000e90: 7465 2063 6f6d 706f 6e65 6e74 7320 616e  te components an
+00000ea0: 6420 6461 7461 2073 6574 7320 6561 7369  d data sets easi
+00000eb0: 6c79 2e0a 2020 2020 2222 220a 0a20 2020  ly..    """..   
+00000ec0: 205f 6d6f 6475 6c65 5f6c 6f67 6765 7220   _module_logger 
+00000ed0: 3d20 6c6f 6767 6572 0a20 2020 205f 7573  = logger.    _us
+00000ee0: 655f 696e 666f 5f6c 6f67 6769 6e67 203d  e_info_logging =
+00000ef0: 2054 7275 650a 0a20 2020 2064 6566 205f   True..    def _
+00000f00: 5f69 6e69 745f 5f28 0a20 2020 2020 2020  _init__(.       
+00000f10: 2073 656c 662c 0a20 2020 2020 2020 2061   self,.        a
+00000f20: 7379 6e63 5f70 6f6f 6c3a 2041 7574 6f41  sync_pool: AutoA
+00000f30: 7379 6e63 4578 6563 7574 696f 6e50 6f6f  syncExecutionPoo
+00000f40: 6c2c 0a20 2020 2020 2020 2061 7070 3a20  l,.        app: 
+00000f50: 4f70 7469 6f6e 616c 5b41 7070 5d2c 0a20  Optional[App],. 
+00000f60: 2020 2020 2020 2072 6575 7365 5f64 6174         reuse_dat
+00000f70: 615f 7365 7473 3a20 626f 6f6c 203d 2046  a_sets: bool = F
+00000f80: 616c 7365 2c0a 2020 2020 293a 0a20 2020  alse,.    ):.   
+00000f90: 2020 2020 2073 656c 662e 5f61 7070 203d       self._app =
+00000fa0: 2061 7070 0a20 2020 2020 2020 2073 656c   app.        sel
+00000fb0: 662e 5f62 7573 696e 6573 733a 2042 7573  f._business: Bus
+00000fc0: 696e 6573 7320 3d20 6170 702e 7061 7265  iness = app.pare
+00000fd0: 6e74 2069 6620 6170 7020 656c 7365 204e  nt if app else N
+00000fe0: 6f6e 650a 2020 2020 2020 2020 7365 6c66  one.        self
+00000ff0: 2e5f 6375 7272 656e 745f 7061 7468 3a20  ._current_path: 
+00001000: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
+00001010: 4e6f 6e65 0a20 2020 2020 2020 2073 656c  None.        sel
+00001020: 662e 5f63 7572 7265 6e74 5f74 6162 735f  f._current_tabs_
+00001030: 6772 6f75 703a 204f 7074 696f 6e61 6c5b  group: Optional[
+00001040: 5461 6273 4772 6f75 705d 203d 204e 6f6e  TabsGroup] = Non
+00001050: 650a 2020 2020 2020 2020 7365 6c66 2e5f  e.        self._
+00001060: 6375 7272 656e 745f 7461 623a 204f 7074  current_tab: Opt
+00001070: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
+00001080: 650a 2020 2020 2020 2020 7365 6c66 2e5f  e.        self._
+00001090: 6375 7272 656e 745f 6d6f 6461 6c3a 204f  current_modal: O
+000010a0: 7074 696f 6e61 6c5b 4d6f 6461 6c5d 203d  ptional[Modal] =
+000010b0: 204e 6f6e 650a 2020 2020 2020 2020 7365   None.        se
+000010c0: 6c66 2e5f 6265 6e74 6f62 6f78 5f64 6174  lf._bentobox_dat
+000010d0: 613a 2064 6963 7420 3d20 7b7d 0a20 2020  a: dict = {}.   
+000010e0: 2020 2020 2073 656c 662e 7265 7573 655f       self.reuse_
+000010f0: 6461 7461 5f73 6574 733a 2062 6f6f 6c20  data_sets: bool 
+00001100: 3d20 7265 7573 655f 6461 7461 5f73 6574  = reuse_data_set
+00001110: 730a 2020 2020 2020 2020 7365 6c66 2e5f  s.        self._
+00001120: 6465 6c65 7465 5f64 6174 615f 7365 745f  delete_data_set_
+00001130: 6c6f 636b 203d 204e 6f6e 650a 2020 2020  lock = None.    
+00001140: 2020 2020 7365 6c66 2e5f 7368 6172 6564      self._shared
+00001150: 5f64 6174 615f 6d61 703a 2064 6963 745b  _data_map: dict[
+00001160: 7374 722c 2064 6963 745b 7374 722c 2074  str, dict[str, t
+00001170: 7570 6c65 5b4d 6170 7069 6e67 2c20 4461  uple[Mapping, Da
+00001180: 7461 5365 742c 2064 6963 745d 5d5d 203d  taSet, dict]]] =
+00001190: 207b 7d0a 2020 2020 2020 2020 7365 6c66   {}.        self
+000011a0: 2e5f 7368 6172 6564 5f64 6174 613a 2064  ._shared_data: d
+000011b0: 6963 745b 7374 722c 2061 6e79 5d20 3d20  ict[str, any] = 
+000011c0: 7b7d 0a20 2020 2020 2020 2073 656c 662e  {}.        self.
+000011d0: 5f65 7865 6375 7469 6f6e 5f70 6174 685f  _execution_path_
+000011e0: 6f72 6465 7273 3a20 6c69 7374 5b73 7472  orders: list[str
+000011f0: 5d20 3d20 5b5d 0a20 2020 2020 2020 2073  ] = [].        s
+00001200: 656c 662e 5f61 7379 6e63 5f70 6f6f 6c20  elf._async_pool 
+00001210: 3d20 6173 796e 635f 706f 6f6c 0a0a 2020  = async_pool..  
+00001220: 2020 6173 796e 6320 6465 6620 5f63 7265    async def _cre
+00001230: 6174 655f 6576 656e 7428 0a20 2020 2020  ate_event(.     
+00001240: 2020 2073 656c 662c 2065 7665 6e74 5f74     self, event_t
+00001250: 7970 653a 2045 7665 6e74 5479 7065 2c20  ype: EventType, 
+00001260: 636f 6e74 656e 743a 2064 6963 742c 2072  content: dict, r
+00001270: 6573 6f75 7263 655f 6964 3a20 4f70 7469  esource_id: Opti
+00001280: 6f6e 616c 5b73 7472 5d20 3d20 4e6f 6e65  onal[str] = None
+00001290: 0a20 2020 2029 3a0a 2020 2020 2020 2020  .    ):.        
+000012a0: 2222 2243 7265 6174 6520 616e 2065 7665  """Create an eve
+000012b0: 6e74 2e0a 2020 2020 2020 2020 3a70 6172  nt..        :par
+000012c0: 616d 2065 7665 6e74 5f74 7970 653a 2074  am event_type: t
+000012d0: 6865 2074 7970 6520 6f66 2074 6865 2065  he type of the e
+000012e0: 7665 6e74 0a20 2020 2020 2020 203a 7061  vent.        :pa
+000012f0: 7261 6d20 636f 6e74 656e 743a 2074 6865  ram content: the
+00001300: 2063 6f6e 7465 6e74 206f 6620 7468 6520   content of the 
+00001310: 6576 656e 740a 2020 2020 2020 2020 2222  event.        ""
+00001320: 220a 2020 2020 2020 2020 6966 2073 656c  ".        if sel
+00001330: 662e 5f61 7070 2e61 7069 5f63 6c69 656e  f._app.api_clien
+00001340: 742e 706c 6179 6772 6f75 6e64 3a0a 2020  t.playground:.  
+00001350: 2020 2020 2020 2020 2020 6177 6169 7420            await 
+00001360: 7365 6c66 2e5f 6275 7369 6e65 7373 2e63  self._business.c
+00001370: 7265 6174 655f 6576 656e 7428 6576 656e  reate_event(even
+00001380: 745f 7479 7065 2c20 636f 6e74 656e 742c  t_type, content,
+00001390: 2072 6573 6f75 7263 655f 6964 290a 0a20   resource_id).. 
+000013a0: 2020 2064 6566 2063 6c65 6172 5f63 6f6e     def clear_con
+000013b0: 7465 7874 2873 656c 6629 3a0a 2020 2020  text(self):.    
+000013c0: 2020 2020 6966 2073 656c 662e 5f62 656e      if self._ben
+000013d0: 746f 626f 785f 6461 7461 3a0a 2020 2020  tobox_data:.    
+000013e0: 2020 2020 2020 2020 7365 6c66 2e5f 6265          self._be
+000013f0: 6e74 6f62 6f78 5f64 6174 6120 3d20 7b7d  ntobox_data = {}
+00001400: 0a20 2020 2020 2020 2020 2020 206c 6f67  .            log
+00001410: 6765 722e 696e 666f 2822 506f 7070 6564  ger.info("Popped
+00001420: 206f 7574 206f 6620 6265 6e74 6f62 6f78   out of bentobox
+00001430: 2229 0a20 2020 2020 2020 2069 6620 7365  ").        if se
+00001440: 6c66 2e5f 6375 7272 656e 745f 7461 6273  lf._current_tabs
+00001450: 5f67 726f 7570 3a0a 2020 2020 2020 2020  _group:.        
+00001460: 2020 2020 7365 6c66 2e5f 6375 7272 656e      self._curren
+00001470: 745f 7461 6273 5f67 726f 7570 203d 204e  t_tabs_group = N
+00001480: 6f6e 650a 2020 2020 2020 2020 2020 2020  one.            
+00001490: 7365 6c66 2e5f 6375 7272 656e 745f 7461  self._current_ta
+000014a0: 6220 3d20 4e6f 6e65 0a20 2020 2020 2020  b = None.       
+000014b0: 2020 2020 206c 6f67 6765 722e 696e 666f       logger.info
+000014c0: 2822 506f 7070 6564 206f 7574 206f 6620  ("Popped out of 
+000014d0: 7461 6273 2067 726f 7570 2229 0a20 2020  tabs group").   
+000014e0: 2020 2020 2069 6620 7365 6c66 2e5f 6375       if self._cu
+000014f0: 7272 656e 745f 6d6f 6461 6c3a 0a20 2020  rrent_modal:.   
+00001500: 2020 2020 2020 2020 2073 656c 662e 5f63           self._c
+00001510: 7572 7265 6e74 5f6d 6f64 616c 203d 204e  urrent_modal = N
+00001520: 6f6e 650a 2020 2020 2020 2020 2020 2020  one.            
+00001530: 6c6f 6767 6572 2e69 6e66 6f28 2250 6f70  logger.info("Pop
+00001540: 7065 6420 6f75 7420 6f66 206d 6f64 616c  ped out of modal
+00001550: 2229 0a0a 2020 2020 6465 6620 5f63 6865  ")..    def _che
+00001560: 636b 5f66 6f72 5f63 6f6e 666c 6963 7473  ck_for_conflicts
+00001570: 2873 656c 662c 2061 7379 6e63 5f70 6f6f  (self, async_poo
+00001580: 6c3a 2041 7574 6f41 7379 6e63 4578 6563  l: AutoAsyncExec
+00001590: 7574 696f 6e50 6f6f 6c2c 206f 7264 6572  utionPool, order
+000015a0: 3a20 696e 7429 3a0a 2020 2020 2020 2020  : int):.        
+000015b0: 2222 220a 2020 2020 2020 2020 4368 6563  """.        Chec
+000015c0: 6b20 6966 2074 6865 7265 2061 7265 2063  k if there are c
+000015d0: 6861 7274 7320 7769 7468 2074 6865 2073  harts with the s
+000015e0: 616d 6520 6f72 6465 722e 0a20 2020 2020  ame order..     
+000015f0: 2020 203a 7061 7261 6d20 6f72 6465 723a     :param order:
+00001600: 2074 6865 206f 7264 6572 206f 6620 7468   the order of th
+00001610: 6520 6368 6172 740a 2020 2020 2020 2020  e chart.        
+00001620: 2222 220a 2020 2020 2020 2020 725f 6861  """.        r_ha
+00001630: 7368 203d 2073 656c 662e 5f67 6574 5f63  sh = self._get_c
+00001640: 6861 7274 5f68 6173 6828 6f72 6465 7229  hart_hash(order)
+00001650: 0a20 2020 2020 2020 2066 7265 655f 636f  .        free_co
+00001660: 6e74 6578 743a 2064 6963 7420 3d20 6173  ntext: dict = as
+00001670: 796e 635f 706f 6f6c 2e66 7265 655f 636f  ync_pool.free_co
+00001680: 6e74 6578 740a 2020 2020 2020 2020 6966  ntext.        if
+00001690: 2022 6c69 7374 5f66 6f72 5f63 6f6e 666c   "list_for_confl
+000016a0: 6963 7473 2220 6e6f 7420 696e 2066 7265  icts" not in fre
+000016b0: 655f 636f 6e74 6578 743a 0a20 2020 2020  e_context:.     
+000016c0: 2020 2020 2020 2066 7265 655f 636f 6e74         free_cont
+000016d0: 6578 745b 226c 6973 745f 666f 725f 636f  ext["list_for_co
+000016e0: 6e66 6c69 6374 7322 5d20 3d20 5b5d 0a0a  nflicts"] = []..
+000016f0: 2020 2020 2020 2020 6966 2072 5f68 6173          if r_has
+00001700: 6820 696e 2066 7265 655f 636f 6e74 6578  h in free_contex
+00001710: 745b 226c 6973 745f 666f 725f 636f 6e66  t["list_for_conf
+00001720: 6c69 6374 7322 5d3a 0a20 2020 2020 2020  licts"]:.       
+00001730: 2020 2020 2061 7379 6e63 5f70 6f6f 6c2e       async_pool.
+00001740: 636c 6561 7228 290a 2020 2020 2020 2020  clear().        
+00001750: 2020 2020 7365 6c66 2e63 6c65 6172 5f63      self.clear_c
+00001760: 6f6e 7465 7874 2829 0a20 2020 2020 2020  ontext().       
+00001770: 2020 2020 206c 6f67 5f65 7272 6f72 280a       log_error(.
+00001780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001790: 6c6f 6767 6572 2c0a 2020 2020 2020 2020  logger,.        
+000017a0: 2020 2020 2020 2020 2243 6861 7274 206f          "Chart o
+000017b0: 7264 6572 2063 6f6c 6c69 7369 6f6e 2c20  rder collision, 
+000017c0: 7477 6f20 6368 6172 7473 2077 6974 6820  two charts with 
+000017d0: 7468 6520 7361 6d65 206f 7264 6572 2063  the same order c
+000017e0: 616e 206e 6f74 2062 6520 6578 6563 7574  an not be execut
+000017f0: 6564 2022 0a20 2020 2020 2020 2020 2020  ed ".           
+00001800: 2020 2020 2022 6174 2074 6865 2073 616d       "at the sam
+00001810: 6520 7469 6d65 222c 0a20 2020 2020 2020  e time",.       
+00001820: 2020 2020 2020 2020 2052 756e 7469 6d65           Runtime
+00001830: 4572 726f 722c 0a20 2020 2020 2020 2020  Error,.         
+00001840: 2020 2029 0a0a 2020 2020 2020 2020 6672     )..        fr
+00001850: 6565 5f63 6f6e 7465 7874 5b22 6c69 7374  ee_context["list
+00001860: 5f66 6f72 5f63 6f6e 666c 6963 7473 225d  _for_conflicts"]
+00001870: 2e61 7070 656e 6428 725f 6861 7368 290a  .append(r_hash).
+00001880: 0a20 2020 2064 6566 205f 6368 6563 6b5f  .    def _check_
+00001890: 6265 666f 7265 5f61 7379 6e63 5f65 7865  before_async_exe
+000018a0: 6375 7469 6f6e 280a 2020 2020 2020 2020  cution(.        
+000018b0: 7365 6c66 2c20 6173 796e 635f 706f 6f6c  self, async_pool
+000018c0: 3a20 4175 746f 4173 796e 6345 7865 6375  : AutoAsyncExecu
+000018d0: 7469 6f6e 506f 6f6c 2c20 6675 6e63 3a20  tionPool, func: 
+000018e0: 6361 6c6c 6162 6c65 2c20 2a61 7267 732c  callable, *args,
+000018f0: 202a 2a6b 7761 7267 730a 2020 2020 293a   **kwargs.    ):
+00001900: 0a20 2020 2020 2020 2022 2222 4368 6563  .        """Chec
+00001910: 6b20 6576 6572 7974 6869 6e67 2069 7320  k everything is 
+00001920: 636f 7272 6563 7420 6265 666f 7265 2065  correct before e
+00001930: 7865 6375 7469 6e67 2074 6865 2074 6173  xecuting the tas
+00001940: 6b20 706f 6f6c 2222 220a 2020 2020 2020  k pool""".      
+00001950: 2020 6966 2022 6f72 6465 7222 2069 6e20    if "order" in 
+00001960: 6b77 6172 6773 3a0a 2020 2020 2020 2020  kwargs:.        
+00001970: 2020 2020 7365 6c66 2e5f 6368 6563 6b5f      self._check_
+00001980: 666f 725f 636f 6e66 6c69 6374 7328 6173  for_conflicts(as
+00001990: 796e 635f 706f 6f6c 2c20 6b77 6172 6773  ync_pool, kwargs
+000019a0: 5b22 6f72 6465 7222 5d29 0a0a 2020 2020  ["order"])..    
+000019b0: 6465 6620 7261 6973 655f 6966 5f63 616e  def raise_if_can
+000019c0: 745f 6368 616e 6765 5f70 6174 6828 7365  t_change_path(se
+000019d0: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
+000019e0: 5261 6973 6520 616e 2065 7272 6f72 2069  Raise an error i
+000019f0: 6620 6120 7461 6273 2067 726f 7570 206f  f a tabs group o
+00001a00: 7220 6120 6d6f 6461 6c20 6973 2061 6c72  r a modal is alr
+00001a10: 6561 6479 206f 7065 6e2e 2222 220a 2020  eady open.""".  
+00001a20: 2020 2020 2020 6966 2073 656c 662e 5f63        if self._c
+00001a30: 7572 7265 6e74 5f74 6162 735f 6772 6f75  urrent_tabs_grou
+00001a40: 703a 0a20 2020 2020 2020 2020 2020 206c  p:.            l
+00001a50: 6f67 5f65 7272 6f72 280a 2020 2020 2020  og_error(.      
+00001a60: 2020 2020 2020 2020 2020 6c6f 6767 6572            logger
+00001a70: 2c20 2243 616e 6e6f 7420 6368 616e 6765  , "Cannot change
+00001a80: 2070 6174 6820 7768 696c 6520 6120 7461   path while a ta
+00001a90: 6273 2067 726f 7570 2069 7320 6f70 656e  bs group is open
+00001aa0: 222c 2054 6162 7345 7272 6f72 0a20 2020  ", TabsError.   
+00001ab0: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+00001ac0: 2020 2069 6620 7365 6c66 2e5f 6375 7272     if self._curr
+00001ad0: 656e 745f 6d6f 6461 6c3a 0a20 2020 2020  ent_modal:.     
+00001ae0: 2020 2020 2020 206c 6f67 5f65 7272 6f72         log_error
+00001af0: 286c 6f67 6765 722c 2022 4361 6e6e 6f74  (logger, "Cannot
+00001b00: 2063 6861 6e67 6520 7061 7468 2077 6869   change path whi
+00001b10: 6c65 2061 206d 6f64 616c 2069 7320 6f70  le a modal is op
+00001b20: 656e 222c 204d 6f64 616c 4572 726f 7229  en", ModalError)
+00001b30: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00001b40: 2e5f 6265 6e74 6f62 6f78 5f64 6174 613a  ._bentobox_data:
+00001b50: 0a20 2020 2020 2020 2020 2020 206c 6f67  .            log
+00001b60: 5f65 7272 6f72 280a 2020 2020 2020 2020  _error(.        
+00001b70: 2020 2020 2020 2020 6c6f 6767 6572 2c20          logger, 
+00001b80: 2243 616e 6e6f 7420 6368 616e 6765 2070  "Cannot change p
+00001b90: 6174 6820 7768 696c 6520 6120 6265 6e74  ath while a bent
+00001ba0: 6f62 6f78 2069 7320 6f70 656e 222c 2042  obox is open", B
+00001bb0: 656e 746f 626f 7845 7272 6f72 0a20 2020  entoboxError.   
+00001bc0: 2020 2020 2020 2020 2029 0a0a 2020 2020           )..    
+00001bd0: 6465 6620 6765 745f 7368 6172 6564 5f64  def get_shared_d
+00001be0: 6174 615f 6e61 6d65 7328 7365 6c66 2920  ata_names(self) 
+00001bf0: 2d3e 206c 6973 745b 7374 725d 3a0a 2020  -> list[str]:.  
+00001c00: 2020 2020 2020 2222 2247 6574 2074 6865        """Get the
+00001c10: 206e 616d 6573 206f 6620 7468 6520 7368   names of the sh
+00001c20: 6172 6564 2064 6174 6122 2222 0a20 2020  ared data""".   
+00001c30: 2020 2020 2072 6574 7572 6e20 6c69 7374       return list
+00001c40: 2873 656c 662e 5f73 6861 7265 645f 6461  (self._shared_da
+00001c50: 7461 5f6d 6170 2e6b 6579 7328 2929 0a0a  ta_map.keys())..
+00001c60: 2020 2020 6465 6620 6368 616e 6765 5f70      def change_p
+00001c70: 6174 6828 7365 6c66 2c20 7061 7468 3a20  ath(self, path: 
+00001c80: 7374 7229 3a0a 2020 2020 2020 2020 2222  str):.        ""
+00001c90: 2243 6861 6e67 6520 7468 6520 6375 7272  "Change the curr
+00001ca0: 656e 7420 7061 7468 2222 220a 2020 2020  ent path""".    
+00001cb0: 2020 2020 7365 6c66 2e72 6169 7365 5f69      self.raise_i
+00001cc0: 665f 6361 6e74 5f63 6861 6e67 655f 7061  f_cant_change_pa
+00001cd0: 7468 2829 0a20 2020 2020 2020 2073 656c  th().        sel
+00001ce0: 662e 5f63 7572 7265 6e74 5f70 6174 6820  f._current_path 
+00001cf0: 3d20 7061 7468 0a20 2020 2020 2020 2069  = path.        i
+00001d00: 6620 7061 7468 2061 6e64 2070 6174 6820  f path and path 
+00001d10: 6e6f 7420 696e 2073 656c 662e 5f65 7865  not in self._exe
+00001d20: 6375 7469 6f6e 5f70 6174 685f 6f72 6465  cution_path_orde
+00001d30: 7273 3a0a 2020 2020 2020 2020 2020 2020  rs:.            
+00001d40: 7365 6c66 2e5f 6578 6563 7574 696f 6e5f  self._execution_
+00001d50: 7061 7468 5f6f 7264 6572 732e 6170 7065  path_orders.appe
+00001d60: 6e64 2870 6174 6829 0a0a 2020 2020 6465  nd(path)..    de
+00001d70: 6620 5f67 6574 5f68 6173 685f 666f 725f  f _get_hash_for_
+00001d80: 636f 6e74 6169 6e65 7228 7365 6c66 2c20  container(self, 
+00001d90: 6e61 6d65 3a20 7374 7229 3a0a 2020 2020  name: str):.    
+00001da0: 2020 2020 2222 2247 6574 2074 6865 2068      """Get the h
+00001db0: 6173 6820 666f 7220 6120 636f 6e74 6169  ash for a contai
+00001dc0: 6e65 7222 2222 0a20 2020 2020 2020 2072  ner""".        r
+00001dd0: 6574 7572 6e20 2866 227b 7365 6c66 2e5f  eturn (f"{self._
+00001de0: 6375 7272 656e 745f 7061 7468 7d5f 2220  current_path}_" 
+00001df0: 6966 2073 656c 662e 5f63 7572 7265 6e74  if self._current
+00001e00: 5f70 6174 6820 656c 7365 2022 2229 202b  _path else "") +
+00001e10: 206e 616d 650a 0a20 2020 2061 7379 6e63   name..    async
+00001e20: 2064 6566 2063 6c65 6172 5f6d 656e 755f   def clear_menu_
+00001e30: 7061 7468 2873 656c 6629 3a0a 2020 2020  path(self):.    
+00001e40: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00001e50: 436c 6561 7220 7468 6520 6375 7272 656e  Clear the curren
+00001e60: 7420 7061 7468 206f 7220 6120 7375 6270  t path or a subp
+00001e70: 6174 680a 2020 2020 2020 2020 2222 220a  ath.        """.
+00001e80: 2020 2020 2020 2020 7265 706f 7274 7320          reports 
+00001e90: 3d20 6177 6169 7420 7365 6c66 2e5f 6170  = await self._ap
+00001ea0: 702e 6765 745f 7265 706f 7274 7328 290a  p.get_reports().
+00001eb0: 2020 2020 2020 2020 746f 7563 6865 645f          touched_
+00001ec0: 6461 7461 5f73 6574 5f69 6473 203d 205b  data_set_ids = [
+00001ed0: 5d0a 2020 2020 2020 2020 6966 2073 656c  ].        if sel
+00001ee0: 662e 5f63 7572 7265 6e74 5f70 6174 6820  f._current_path 
+00001ef0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00001f00: 2020 2020 2020 2020 2070 6174 6820 3d20           path = 
+00001f10: 6372 6561 7465 5f6e 6f72 6d61 6c69 7a65  create_normalize
+00001f20: 645f 6e61 6d65 2873 656c 662e 5f63 7572  d_name(self._cur
+00001f30: 7265 6e74 5f70 6174 6829 0a20 2020 2020  rent_path).     
+00001f40: 2020 2020 2020 2072 6570 6f72 7473 203d         reports =
+00001f50: 205b 0a20 2020 2020 2020 2020 2020 2020   [.             
+00001f60: 2020 2072 6570 6f72 740a 2020 2020 2020     report.      
+00001f70: 2020 2020 2020 2020 2020 666f 7220 7265            for re
+00001f80: 706f 7274 2069 6e20 7265 706f 7274 730a  port in reports.
+00001f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001fa0: 6966 2072 6570 6f72 745b 2270 6174 6822  if report["path"
+00001fb0: 5d20 616e 6420 6372 6561 7465 5f6e 6f72  ] and create_nor
+00001fc0: 6d61 6c69 7a65 645f 6e61 6d65 2872 6570  malized_name(rep
+00001fd0: 6f72 745b 2270 6174 6822 5d29 203d 3d20  ort["path"]) == 
+00001fe0: 7061 7468 0a20 2020 2020 2020 2020 2020  path.           
+00001ff0: 205d 0a20 2020 2020 2020 2065 6c73 653a   ].        else:
+00002000: 0a20 2020 2020 2020 2020 2020 2074 6f75  .            tou
+00002010: 6368 6564 5f64 6174 615f 7365 745f 6964  ched_data_set_id
+00002020: 7320 3d20 5b64 735b 2269 6422 5d20 666f  s = [ds["id"] fo
+00002030: 7220 6473 2069 6e20 6177 6169 7420 7365  r ds in await se
+00002040: 6c66 2e5f 6170 702e 6765 745f 6461 7461  lf._app.get_data
+00002050: 5f73 6574 7328 295d 0a0a 2020 2020 2020  _sets()]..      
+00002060: 2020 636f 6e74 6169 6e65 7273 3a20 6c69    containers: li
+00002070: 7374 203d 205b 0a20 2020 2020 2020 2020  st = [.         
+00002080: 2020 2072 6570 6f72 7420 666f 7220 7265     report for re
+00002090: 706f 7274 2069 6e20 7265 706f 7274 7320  port in reports 
+000020a0: 6966 2072 6570 6f72 742e 7265 706f 7274  if report.report
+000020b0: 5f74 7970 6520 696e 205b 2254 4142 5322  _type in ["TABS"
+000020c0: 2c20 224d 4f44 414c 225d 0a20 2020 2020  , "MODAL"].     
+000020d0: 2020 205d 0a0a 2020 2020 2020 2020 666f     ]..        fo
+000020e0: 7220 636f 6e74 6169 6e65 7220 696e 2063  r container in c
+000020f0: 6f6e 7461 696e 6572 733a 0a20 2020 2020  ontainers:.     
+00002100: 2020 2020 2020 2063 6f6e 7461 696e 6572         container
+00002110: 2e63 6c65 6172 5f63 6f6e 7465 6e74 2829  .clear_content()
+00002120: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00002130: 6e6f 7420 7365 6c66 2e5f 6170 702e 6170  not self._app.ap
+00002140: 695f 636c 6965 6e74 2e63 6163 6865 5f65  i_client.cache_e
+00002150: 6e61 626c 6564 3a0a 2020 2020 2020 2020  nabled:.        
+00002160: 2020 2020 2020 2020 6177 6169 7420 636f          await co
+00002170: 6e74 6169 6e65 722e 7570 6461 7465 2829  ntainer.update()
+00002180: 0a0a 2020 2020 2020 2020 7264 7320 3d20  ..        rds = 
+00002190: 6177 6169 7420 6173 796e 6369 6f2e 6761  await asyncio.ga
+000021a0: 7468 6572 280a 2020 2020 2020 2020 2020  ther(.          
+000021b0: 2020 2a5b 7265 706f 7274 2e67 6574 5f72    *[report.get_r
+000021c0: 6570 6f72 745f 6461 7461 5f73 6574 7328  eport_data_sets(
+000021d0: 2920 666f 7220 7265 706f 7274 2069 6e20  ) for report in 
+000021e0: 7265 706f 7274 735d 0a20 2020 2020 2020  reports].       
+000021f0: 2029 0a20 2020 2020 2020 2074 6f75 6368   ).        touch
+00002200: 6564 5f64 6174 615f 7365 745f 6964 732e  ed_data_set_ids.
+00002210: 6578 7465 6e64 285b 7264 5b22 6461 7461  extend([rd["data
+00002220: 5365 7449 6422 5d20 666f 7220 7264 7320  SetId"] for rds 
+00002230: 696e 2072 6473 2066 6f72 2072 6420 696e  in rds for rd in
+00002240: 2072 6473 5d29 0a0a 2020 2020 2020 2020   rds])..        
+00002250: 6177 6169 7420 6173 796e 6369 6f2e 6761  await asyncio.ga
+00002260: 7468 6572 280a 2020 2020 2020 2020 2020  ther(.          
+00002270: 2020 2a5b 7365 6c66 2e5f 6170 702e 6465    *[self._app.de
+00002280: 6c65 7465 5f72 6570 6f72 7428 7265 706f  lete_report(repo
+00002290: 7274 5b22 6964 225d 2920 666f 7220 7265  rt["id"]) for re
+000022a0: 706f 7274 2069 6e20 7265 706f 7274 735d  port in reports]
+000022b0: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
+000022c0: 2020 206c 6f67 6765 722e 696e 666f 2866     logger.info(f
+000022d0: 2244 656c 6574 6564 207b 6c65 6e28 7265  "Deleted {len(re
+000022e0: 706f 7274 7329 7d20 636f 6d70 6f6e 656e  ports)} componen
+000022f0: 7473 2229 0a20 2020 2020 2020 2061 7761  ts").        awa
+00002300: 6974 2073 656c 662e 5f61 7070 2e64 656c  it self._app.del
+00002310: 6574 655f 756e 7573 6564 5f64 6174 615f  ete_unused_data_
+00002320: 7365 7473 280a 2020 2020 2020 2020 2020  sets(.          
+00002330: 2020 6c6f 673d 5472 7565 2c20 6461 7461    log=True, data
+00002340: 5f73 6574 5f69 6473 3d74 6f75 6368 6564  _set_ids=touched
+00002350: 5f64 6174 615f 7365 745f 6964 730a 2020  _data_set_ids.  
+00002360: 2020 2020 2020 290a 0a20 2020 2061 7379        )..    asy
+00002370: 6e63 2064 6566 2064 656c 6574 655f 6368  nc def delete_ch
+00002380: 6172 745f 6279 5f6f 7264 6572 2873 656c  art_by_order(sel
+00002390: 662c 206f 7264 6572 3a20 696e 7429 3a0a  f, order: int):.
+000023a0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+000023b0: 2020 2020 4465 6c65 7465 2061 2072 6570      Delete a rep
+000023c0: 6f72 7420 6279 206f 7264 6572 2061 6e64  ort by order and
+000023d0: 2063 6f6e 7465 7874 0a20 2020 2020 2020   context.       
+000023e0: 2022 2222 0a20 2020 2020 2020 2072 5f68   """.        r_h
+000023f0: 6173 682c 2072 6570 6f72 7420 3d20 6177  ash, report = aw
+00002400: 6169 7420 7365 6c66 2e5f 6765 745f 6368  ait self._get_ch
+00002410: 6172 745f 7265 706f 7274 280a 2020 2020  art_report(.    
+00002420: 2020 2020 2020 2020 6f72 6465 722c 2054          order, T
+00002430: 6162 6c65 2c20 6372 6561 7465 5f69 665f  able, create_if_
+00002440: 6e6f 745f 6578 6973 7473 3d46 616c 7365  not_exists=False
+00002450: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
+00002460: 2020 2069 6620 6e6f 7420 7265 706f 7274     if not report
+00002470: 3a0a 2020 2020 2020 2020 2020 2020 6c6f  :.            lo
+00002480: 675f 6572 726f 7228 6c6f 6767 6572 2c20  g_error(logger, 
+00002490: 6622 4e6f 2063 6861 7274 2066 6f75 6e64  f"No chart found
+000024a0: 2077 6974 6820 6f72 6465 7220 7b6f 7264   with order {ord
+000024b0: 6572 7d22 2c20 5275 6e74 696d 6545 7272  er}", RuntimeErr
+000024c0: 6f72 290a 2020 2020 2020 2020 6177 6169  or).        awai
+000024d0: 7420 7365 6c66 2e5f 6170 702e 6465 6c65  t self._app.dele
+000024e0: 7465 5f72 6570 6f72 7428 725f 6861 7368  te_report(r_hash
+000024f0: 3d72 5f68 6173 6829 0a0a 2020 2020 6173  =r_hash)..    as
+00002500: 796e 6320 6465 6620 6465 6c65 7465 5f74  ync def delete_t
+00002510: 6162 735f 6772 6f75 7028 7365 6c66 2c20  abs_group(self, 
+00002520: 6e61 6d65 3a20 7374 7229 3a0a 2020 2020  name: str):.    
+00002530: 2020 2020 2222 2244 656c 6574 6520 6120      """Delete a 
+00002540: 7461 6273 2067 726f 7570 2222 220a 2020  tabs group""".  
+00002550: 2020 2020 2020 725f 6861 7368 203d 2073        r_hash = s
+00002560: 656c 662e 5f67 6574 5f68 6173 685f 666f  elf._get_hash_fo
+00002570: 725f 636f 6e74 6169 6e65 7228 6e61 6d65  r_container(name
+00002580: 290a 2020 2020 2020 2020 7461 6273 5f67  ).        tabs_g
+00002590: 726f 7570 203d 2061 7761 6974 2073 656c  roup = await sel
+000025a0: 662e 5f61 7070 2e67 6574 5f72 6570 6f72  f._app.get_repor
+000025b0: 7428 725f 6861 7368 3d72 5f68 6173 6829  t(r_hash=r_hash)
+000025c0: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
+000025d0: 7461 6273 5f67 726f 7570 3a0a 2020 2020  tabs_group:.    
+000025e0: 2020 2020 2020 2020 6c6f 675f 6572 726f          log_erro
+000025f0: 7228 6c6f 6767 6572 2c20 6622 4e6f 2074  r(logger, f"No t
+00002600: 6162 7320 6772 6f75 7020 666f 756e 6420  abs group found 
+00002610: 7769 7468 206e 616d 6520 7b6e 616d 657d  with name {name}
+00002620: 222c 2054 6162 7345 7272 6f72 290a 2020  ", TabsError).  
+00002630: 2020 2020 2020 6177 6169 7420 7365 6c66        await self
+00002640: 2e5f 6170 702e 6465 6c65 7465 5f72 6570  ._app.delete_rep
+00002650: 6f72 7428 725f 6861 7368 3d72 5f68 6173  ort(r_hash=r_has
+00002660: 6829 0a0a 2020 2020 6173 796e 6320 6465  h)..    async de
+00002670: 6620 6465 6c65 7465 5f6d 6f64 616c 2873  f delete_modal(s
+00002680: 656c 662c 206e 616d 653a 2073 7472 293a  elf, name: str):
+00002690: 0a20 2020 2020 2020 2022 2222 4465 6c65  .        """Dele
+000026a0: 7465 2061 206d 6f64 616c 2222 220a 2020  te a modal""".  
+000026b0: 2020 2020 2020 725f 6861 7368 203d 2073        r_hash = s
+000026c0: 656c 662e 5f67 6574 5f68 6173 685f 666f  elf._get_hash_fo
+000026d0: 725f 636f 6e74 6169 6e65 7228 6e61 6d65  r_container(name
+000026e0: 290a 2020 2020 2020 2020 6d6f 6461 6c20  ).        modal 
+000026f0: 3d20 6177 6169 7420 7365 6c66 2e5f 6170  = await self._ap
+00002700: 702e 6765 745f 7265 706f 7274 2872 5f68  p.get_report(r_h
+00002710: 6173 683d 725f 6861 7368 290a 2020 2020  ash=r_hash).    
+00002720: 2020 2020 6966 206e 6f74 206d 6f64 616c      if not modal
+00002730: 3a0a 2020 2020 2020 2020 2020 2020 6c6f  :.            lo
+00002740: 675f 6572 726f 7228 6c6f 6767 6572 2c20  g_error(logger, 
+00002750: 6622 4e6f 206d 6f64 616c 2066 6f75 6e64  f"No modal found
+00002760: 2077 6974 6820 6e61 6d65 207b 6e61 6d65   with name {name
+00002770: 7d22 2c20 4d6f 6461 6c45 7272 6f72 290a  }", ModalError).
+00002780: 2020 2020 2020 2020 6177 6169 7420 7365          await se
+00002790: 6c66 2e5f 6170 702e 6465 6c65 7465 5f72  lf._app.delete_r
+000027a0: 6570 6f72 7428 725f 6861 7368 3d72 5f68  eport(r_hash=r_h
+000027b0: 6173 6829 0a0a 2020 2020 6465 6620 7365  ash)..    def se
+000027c0: 745f 6265 6e74 6f62 6f78 2873 656c 662c  t_bentobox(self,
+000027d0: 2063 6f6c 735f 7369 7a65 3a20 696e 742c   cols_size: int,
+000027e0: 2072 6f77 735f 7369 7a65 3a20 696e 7429   rows_size: int)
+000027f0: 3a0a 2020 2020 2020 2020 2222 2253 7461  :.        """Sta
+00002800: 7274 2075 7369 6e67 2061 2062 656e 746f  rt using a bento
+00002810: 626f 782c 2074 6865 2069 6420 616e 6420  box, the id and 
+00002820: 7468 6520 6f72 6465 7220 7769 6c6c 2062  the order will b
+00002830: 6520 7365 7420 7768 656e 2074 6865 2062  e set when the b
+00002840: 656e 746f 626f 7820 6973 2075 7365 6420  entobox is used 
+00002850: 666f 7220 7468 6520 6669 7273 7420 7469  for the first ti
+00002860: 6d65 0a20 2020 2020 2020 203a 7061 7261  me.        :para
+00002870: 6d20 636f 6c73 5f73 697a 653a 2074 6865  m cols_size: the
+00002880: 206e 756d 6265 7220 6f66 2063 6f6c 756d   number of colum
+00002890: 6e73 2069 6e20 7468 6520 6265 6e74 6f62  ns in the bentob
+000028a0: 6f78 0a20 2020 2020 2020 203a 7061 7261  ox.        :para
+000028b0: 6d20 726f 7773 5f73 697a 653a 2074 6865  m rows_size: the
+000028c0: 206e 756d 6265 7220 6f66 2072 6f77 7320   number of rows 
+000028d0: 696e 2074 6865 2062 656e 746f 626f 7822  in the bentobox"
+000028e0: 2222 0a20 2020 2020 2020 2073 656c 662e  "".        self.
+000028f0: 5f62 656e 746f 626f 785f 6461 7461 3a20  _bentobox_data: 
+00002900: 6469 6374 203d 207b 0a20 2020 2020 2020  dict = {.       
+00002910: 2020 2020 2022 6265 6e74 6f62 6f78 4964       "bentoboxId
+00002920: 223a 204e 6f6e 652c 0a20 2020 2020 2020  ": None,.       
+00002930: 2020 2020 2022 6265 6e74 6f62 6f78 4f72       "bentoboxOr
+00002940: 6465 7222 3a20 4e6f 6e65 2c0a 2020 2020  der": None,.    
+00002950: 2020 2020 2020 2020 2262 656e 746f 626f          "bentobo
+00002960: 7853 697a 6543 6f6c 756d 6e73 223a 2063  xSizeColumns": c
+00002970: 6f6c 735f 7369 7a65 2c0a 2020 2020 2020  ols_size,.      
+00002980: 2020 2020 2020 2262 656e 746f 626f 7853        "bentoboxS
+00002990: 697a 6552 6f77 7322 3a20 726f 7773 5f73  izeRows": rows_s
+000029a0: 697a 652c 0a20 2020 2020 2020 207d 0a0a  ize,.        }..
+000029b0: 2020 2020 6465 6620 706f 705f 6f75 745f      def pop_out_
+000029c0: 6f66 5f62 656e 746f 626f 7828 7365 6c66  of_bentobox(self
+000029d0: 293a 0a20 2020 2020 2020 2022 2222 5374  ):.        """St
+000029e0: 6f70 2075 7369 6e67 2061 2062 656e 746f  op using a bento
+000029f0: 626f 7822 2222 0a20 2020 2020 2020 2073  box""".        s
+00002a00: 656c 662e 5f62 656e 746f 626f 785f 6461  elf._bentobox_da
+00002a10: 7461 203d 207b 7d0a 0a20 2020 2064 6566  ta = {}..    def
+00002a20: 205f 6765 745f 6265 6e74 6f62 6f78 5f64   _get_bentobox_d
+00002a30: 6174 6128 7365 6c66 2c20 6f72 6465 723a  ata(self, order:
+00002a40: 2069 6e74 2920 2d3e 2064 6963 743a 0a20   int) -> dict:. 
+00002a50: 2020 2020 2020 2022 2222 4765 7420 7468         """Get th
+00002a60: 6520 6265 6e74 6f62 6f78 2064 6174 6122  e bentobox data"
+00002a70: 2222 0a20 2020 2020 2020 2069 6620 6e6f  "".        if no
+00002a80: 7420 7365 6c66 2e5f 6265 6e74 6f62 6f78  t self._bentobox
+00002a90: 5f64 6174 613a 0a20 2020 2020 2020 2020  _data:.         
+00002aa0: 2020 2072 6574 7572 6e20 7b7d 0a20 2020     return {}.   
+00002ab0: 2020 2020 2069 6620 6e6f 7420 7365 6c66       if not self
+00002ac0: 2e5f 6265 6e74 6f62 6f78 5f64 6174 615b  ._bentobox_data[
+00002ad0: 2262 656e 746f 626f 7849 6422 5d3a 0a20  "bentoboxId"]:. 
+00002ae0: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
+00002af0: 7420 7365 6c66 2e5f 6265 6e74 6f62 6f78  t self._bentobox
+00002b00: 5f64 6174 615b 2262 656e 746f 626f 7849  _data["bentoboxI
+00002b10: 6422 5d3a 0a20 2020 2020 2020 2020 2020  d"]:.           
+00002b20: 2020 2020 2073 656c 662e 5f62 656e 746f       self._bento
+00002b30: 626f 785f 6461 7461 2e75 7064 6174 6528  box_data.update(
+00002b40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002b50: 2020 2020 207b 0a20 2020 2020 2020 2020       {.         
+00002b60: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00002b70: 6265 6e74 6f62 6f78 4964 223a 2022 5f22  bentoboxId": "_"
+00002b80: 202b 2073 7472 286f 7264 6572 292c 0a20   + str(order),. 
+00002b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002ba0: 2020 2020 2020 2022 6265 6e74 6f62 6f78         "bentobox
+00002bb0: 4f72 6465 7222 3a20 6f72 6465 722c 0a20  Order": order,. 
+00002bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002bd0: 2020 207d 0a20 2020 2020 2020 2020 2020     }.           
+00002be0: 2020 2020 2029 0a20 2020 2020 2020 2072       ).        r
+00002bf0: 6574 7572 6e20 7365 6c66 2e5f 6265 6e74  eturn self._bent
+00002c00: 6f62 6f78 5f64 6174 610a 0a20 2020 2061  obox_data..    a
+00002c10: 7379 6e63 2064 6566 205f 7570 6461 7465  sync def _update
+00002c20: 5f63 6f6e 7461 696e 6572 7328 7365 6c66  _containers(self
+00002c30: 293a 0a20 2020 2020 2020 2022 2222 5570  ):.        """Up
+00002c40: 6461 7465 2074 6865 2072 6570 6f72 7473  date the reports
+00002c50: 2074 6861 7420 6163 7420 6173 2063 6f6e   that act as con
+00002c60: 7461 696e 6572 7322 2222 0a20 2020 2020  tainers""".     
+00002c70: 2020 2072 6570 6f72 7473 203d 2061 7761     reports = awa
+00002c80: 6974 2073 656c 662e 5f61 7070 2e67 6574  it self._app.get
+00002c90: 5f72 6570 6f72 7473 2829 0a20 2020 2020  _reports().     
+00002ca0: 2020 2063 6f6e 7461 696e 6572 733a 206c     containers: l
+00002cb0: 6973 745b 5265 706f 7274 5d20 3d20 5b0a  ist[Report] = [.
+00002cc0: 2020 2020 2020 2020 2020 2020 7265 706f              repo
+00002cd0: 7274 2066 6f72 2072 6570 6f72 7420 696e  rt for report in
+00002ce0: 2072 6570 6f72 7473 2069 6620 7265 706f   reports if repo
+00002cf0: 7274 2e72 6570 6f72 745f 7479 7065 2069  rt.report_type i
+00002d00: 6e20 5b22 5441 4253 222c 2022 4d4f 4441  n ["TABS", "MODA
+00002d10: 4c22 5d0a 2020 2020 2020 2020 5d0a 2020  L"].        ].  
+00002d20: 2020 2020 2020 6177 6169 7420 6173 796e        await asyn
+00002d30: 6369 6f2e 6761 7468 6572 282a 5b63 6f6e  cio.gather(*[con
+00002d40: 7461 696e 6572 2e75 7064 6174 6528 2920  tainer.update() 
+00002d50: 666f 7220 636f 6e74 6169 6e65 7220 696e  for container in
+00002d60: 2063 6f6e 7461 696e 6572 735d 290a 2020   containers]).  
+00002d70: 2020 2020 2020 6c6f 6767 6572 2e69 6e66        logger.inf
+00002d80: 6f28 2255 7064 6174 6564 2074 6162 2067  o("Updated tab g
+00002d90: 726f 7570 7320 616e 6420 6d6f 6461 6c73  roups and modals
+00002da0: 2229 0a0a 2020 2020 6173 796e 6320 6465  ")..    async de
+00002db0: 6620 7365 745f 7461 6273 5f69 6e64 6578  f set_tabs_index
+00002dc0: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
+00002dd0: 2020 2020 2020 2020 7461 6273 5f69 6e64          tabs_ind
+00002de0: 6578 3a20 7475 706c 655b 7374 722c 2073  ex: tuple[str, s
+00002df0: 7472 5d2c 0a20 2020 2020 2020 206f 7264  tr],.        ord
+00002e00: 6572 3a20 4f70 7469 6f6e 616c 5b69 6e74  er: Optional[int
+00002e10: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
+00002e20: 2020 7061 7265 6e74 5f74 6162 735f 696e    parent_tabs_in
+00002e30: 6465 783a 204f 7074 696f 6e61 6c5b 7475  dex: Optional[tu
+00002e40: 706c 655b 7374 722c 2073 7472 5d5d 203d  ple[str, str]] =
+00002e50: 204e 6f6e 652c 0a20 2020 2020 2020 2070   None,.        p
+00002e60: 6164 6469 6e67 3a20 4f70 7469 6f6e 616c  adding: Optional
+00002e70: 5b73 7472 5d20 3d20 4e6f 6e65 2c0a 2020  [str] = None,.  
+00002e80: 2020 2020 2020 636f 6c73 5f73 697a 653a        cols_size:
+00002e90: 204f 7074 696f 6e61 6c5b 696e 745d 203d   Optional[int] =
+00002ea0: 204e 6f6e 652c 0a20 2020 2020 2020 2072   None,.        r
+00002eb0: 6f77 735f 7369 7a65 3a20 4f70 7469 6f6e  ows_size: Option
+00002ec0: 616c 5b69 6e74 5d20 3d20 4e6f 6e65 2c0a  al[int] = None,.
+00002ed0: 2020 2020 2020 2020 6a75 7374 5f6c 6162          just_lab
+00002ee0: 656c 733a 204f 7074 696f 6e61 6c5b 626f  els: Optional[bo
+00002ef0: 6f6c 5d20 3d20 4e6f 6e65 2c0a 2020 2020  ol] = None,.    
+00002f00: 2020 2020 7374 6963 6b79 3a20 4f70 7469      sticky: Opti
+00002f10: 6f6e 616c 5b62 6f6f 6c5d 203d 204e 6f6e  onal[bool] = Non
+00002f20: 652c 0a20 2020 2029 3a0a 2020 2020 2020  e,.    ):.      
+00002f30: 2020 2222 2253 6574 2074 6865 2063 7572    """Set the cur
+00002f40: 7265 6e74 2074 6162 7320 696e 6465 782e  rent tabs index.
+00002f50: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+00002f60: 7461 6273 5f69 6e64 6578 3a20 7468 6520  tabs_index: the 
+00002f70: 696e 6465 7820 6f66 2074 6865 2074 6162  index of the tab
+00002f80: 7320 6772 6f75 700a 2020 2020 2020 2020  s group.        
+00002f90: 3a70 6172 616d 206f 7264 6572 3a20 7468  :param order: th
+00002fa0: 6520 6f72 6465 7220 6f66 2074 6865 2074  e order of the t
+00002fb0: 6162 7320 6772 6f75 7020 696e 2074 6865  abs group in the
+00002fc0: 2064 6173 6862 6f61 7264 0a20 2020 2020   dashboard.     
+00002fd0: 2020 203a 7061 7261 6d20 7061 7265 6e74     :param parent
+00002fe0: 5f74 6162 735f 696e 6465 783a 2074 6865  _tabs_index: the
+00002ff0: 2069 6e64 6578 206f 6620 7468 6520 7061   index of the pa
+00003000: 7265 6e74 2074 6162 7320 6772 6f75 700a  rent tabs group.
+00003010: 2020 2020 2020 2020 3a70 6172 616d 2063          :param c
+00003020: 6f6c 735f 7369 7a65 3a20 7468 6520 7369  ols_size: the si
+00003030: 7a65 206f 6620 7468 6520 636f 6c75 6d6e  ze of the column
+00003040: 7320 696e 2074 6865 2074 6162 7320 6772  s in the tabs gr
+00003050: 6f75 700a 2020 2020 2020 2020 3a70 6172  oup.        :par
+00003060: 616d 2070 6164 6469 6e67 3a20 7468 6520  am padding: the 
+00003070: 7061 6464 696e 6720 6f66 2074 6865 2074  padding of the t
+00003080: 6162 7320 6772 6f75 700a 2020 2020 2020  abs group.      
+00003090: 2020 3a70 6172 616d 2072 6f77 735f 7369    :param rows_si
+000030a0: 7a65 3a20 7468 6520 7369 7a65 206f 6620  ze: the size of 
+000030b0: 7468 6520 726f 7773 2069 6e20 7468 6520  the rows in the 
+000030c0: 7461 6273 2067 726f 7570 0a20 2020 2020  tabs group.     
+000030d0: 2020 203a 7061 7261 6d20 6a75 7374 5f6c     :param just_l
+000030e0: 6162 656c 733a 2077 6865 7468 6572 2074  abels: whether t
+000030f0: 6f20 7368 6f77 206a 7573 7420 7468 6520  o show just the 
+00003100: 6c61 6265 6c73 2069 6e20 7468 6520 7461  labels in the ta
+00003110: 6273 2067 726f 7570 0a20 2020 2020 2020  bs group.       
+00003120: 203a 7061 7261 6d20 7374 6963 6b79 3a20   :param sticky: 
+00003130: 7768 6574 6865 7220 746f 206d 616b 6520  whether to make 
+00003140: 7468 6520 7461 6273 2067 726f 7570 2073  the tabs group s
+00003150: 7469 636b 790a 2020 2020 2020 2020 2222  ticky.        ""
+00003160: 220a 2020 2020 2020 2020 725f 6861 7368  ".        r_hash
+00003170: 203d 2073 656c 662e 5f67 6574 5f68 6173   = self._get_has
+00003180: 685f 666f 725f 636f 6e74 6169 6e65 7228  h_for_container(
+00003190: 7461 6273 5f69 6e64 6578 5b30 5d29 0a20  tabs_index[0]). 
+000031a0: 2020 2020 2020 2074 6162 735f 6772 6f75         tabs_grou
+000031b0: 703a 204f 7074 696f 6e61 6c5b 5461 6273  p: Optional[Tabs
+000031c0: 4772 6f75 705d 203d 2061 7761 6974 2073  Group] = await s
+000031d0: 656c 662e 5f61 7070 2e67 6574 5f72 6570  elf._app.get_rep
+000031e0: 6f72 7428 725f 6861 7368 3d72 5f68 6173  ort(r_hash=r_has
+000031f0: 6829 0a20 2020 2020 2020 2070 6172 616d  h).        param
+00003200: 7320 3d20 7b22 7072 6f70 6572 7469 6573  s = {"properties
+00003210: 223a 207b 7d7d 0a20 2020 2020 2020 2069  ": {}}.        i
+00003220: 6620 636f 6c73 5f73 697a 653a 0a20 2020  f cols_size:.   
+00003230: 2020 2020 2020 2020 2070 6172 616d 735b           params[
+00003240: 2273 697a 6543 6f6c 756d 6e73 225d 203d  "sizeColumns"] =
+00003250: 2063 6f6c 735f 7369 7a65 0a20 2020 2020   cols_size.     
+00003260: 2020 2069 6620 7061 6464 696e 673a 0a20     if padding:. 
+00003270: 2020 2020 2020 2020 2020 2070 6172 616d             param
+00003280: 735b 2273 697a 6550 6164 6469 6e67 225d  s["sizePadding"]
+00003290: 203d 2070 6164 6469 6e67 0a20 2020 2020   = padding.     
+000032a0: 2020 2069 6620 726f 7773 5f73 697a 653a     if rows_size:
+000032b0: 0a20 2020 2020 2020 2020 2020 2070 6172  .            par
+000032c0: 616d 735b 2273 697a 6552 6f77 7322 5d20  ams["sizeRows"] 
+000032d0: 3d20 726f 7773 5f73 697a 650a 2020 2020  = rows_size.    
+000032e0: 2020 2020 6966 2069 7369 6e73 7461 6e63      if isinstanc
+000032f0: 6528 6a75 7374 5f6c 6162 656c 732c 2062  e(just_labels, b
+00003300: 6f6f 6c29 3a0a 2020 2020 2020 2020 2020  ool):.          
+00003310: 2020 7061 7261 6d73 5b22 7072 6f70 6572    params["proper
+00003320: 7469 6573 225d 5b22 7661 7269 616e 7422  ties"]["variant"
+00003330: 5d20 3d20 280a 2020 2020 2020 2020 2020  ] = (.          
+00003340: 2020 2020 2020 2273 6f6c 6964 526f 756e        "solidRoun
+00003350: 6465 6422 2069 6620 6a75 7374 5f6c 6162  ded" if just_lab
+00003360: 656c 7320 656c 7365 2022 656e 636c 6f73  els else "enclos
+00003370: 6564 536f 6c69 6452 6f75 6e64 6564 220a  edSolidRounded".
+00003380: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+00003390: 2020 2020 2020 6966 2069 7369 6e73 7461        if isinsta
+000033a0: 6e63 6528 7374 6963 6b79 2c20 626f 6f6c  nce(sticky, bool
+000033b0: 293a 0a20 2020 2020 2020 2020 2020 2070  ):.            p
+000033c0: 6172 616d 735b 2270 726f 7065 7274 6965  arams["propertie
+000033d0: 7322 5d5b 2273 7469 636b 7922 5d20 3d20  s"]["sticky"] = 
+000033e0: 7374 6963 6b79 0a20 2020 2020 2020 2062  sticky.        b
+000033f0: 656e 746f 626f 785f 6461 7461 203d 2073  entobox_data = s
+00003400: 656c 662e 5f67 6574 5f62 656e 746f 626f  elf._get_bentobo
+00003410: 785f 6461 7461 286f 7264 6572 290a 2020  x_data(order).  
+00003420: 2020 2020 2020 6966 2062 656e 746f 626f        if bentobo
+00003430: 785f 6461 7461 3a0a 2020 2020 2020 2020  x_data:.        
+00003440: 2020 2020 7061 7261 6d73 5b22 6265 6e74      params["bent
+00003450: 6f62 6f78 225d 203d 2062 656e 746f 626f  obox"] = bentobo
+00003460: 785f 6461 7461 0a20 2020 2020 2020 2069  x_data.        i
+00003470: 6620 7365 6c66 2e5f 6375 7272 656e 745f  f self._current_
+00003480: 7061 7468 3a0a 2020 2020 2020 2020 2020  path:.          
+00003490: 2020 7061 7261 6d73 5b22 7061 7468 225d    params["path"]
+000034a0: 203d 2073 656c 662e 5f63 7572 7265 6e74   = self._current
+000034b0: 5f70 6174 680a 0a20 2020 2020 2020 2069  _path..        i
+000034c0: 6620 6e6f 7420 7461 6273 5f67 726f 7570  f not tabs_group
+000034d0: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
+000034e0: 206e 6f74 2069 7369 6e73 7461 6e63 6528   not isinstance(
+000034f0: 6f72 6465 722c 2069 6e74 293a 0a20 2020  order, int):.   
+00003500: 2020 2020 2020 2020 2020 2020 206c 6f67               log
+00003510: 5f65 7272 6f72 280a 2020 2020 2020 2020  _error(.        
+00003520: 2020 2020 2020 2020 2020 2020 6c6f 6767              logg
+00003530: 6572 2c0a 2020 2020 2020 2020 2020 2020  er,.            
+00003540: 2020 2020 2020 2020 6622 4361 6e6e 6f74          f"Cannot
+00003550: 2063 7265 6174 6520 7461 6273 2067 726f   create tabs gro
+00003560: 7570 207b 7461 6273 5f69 6e64 6578 5b30  up {tabs_index[0
+00003570: 5d7d 2077 6974 686f 7574 206f 7264 6572  ]} without order
+00003580: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00003590: 2020 2020 2020 2054 6162 7345 7272 6f72         TabsError
+000035a0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000035b0: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
+000035c0: 7461 6273 5f67 726f 7570 3a20 5461 6273  tabs_group: Tabs
+000035d0: 4772 6f75 7020 3d20 6177 6169 7420 7365  Group = await se
+000035e0: 6c66 2e5f 6170 702e 6372 6561 7465 5f72  lf._app.create_r
+000035f0: 6570 6f72 7428 0a20 2020 2020 2020 2020  eport(.         
+00003600: 2020 2020 2020 2054 6162 7347 726f 7570         TabsGroup
+00003610: 2c20 725f 6861 7368 3d72 5f68 6173 682c  , r_hash=r_hash,
+00003620: 206f 7264 6572 3d6f 7264 6572 2c20 2a2a   order=order, **
+00003630: 7061 7261 6d73 0a20 2020 2020 2020 2020  params.         
+00003640: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+00003650: 206c 6f67 6765 722e 696e 666f 280a 2020   logger.info(.  
+00003660: 2020 2020 2020 2020 2020 2020 2020 6627                f'
+00003670: 4372 6561 7465 6420 7461 6273 2067 726f  Created tabs gro
+00003680: 7570 207b 7461 6273 5f69 6e64 6578 5b30  up {tabs_index[0
+00003690: 5d7d 2077 6974 6820 6964 207b 7461 6273  ]} with id {tabs
+000036a0: 5f67 726f 7570 5b22 6964 225d 7d27 0a20  _group["id"]}'. 
+000036b0: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+000036c0: 2020 2020 2065 6c69 6620 6f72 6465 723a       elif order:
+000036d0: 0a20 2020 2020 2020 2020 2020 2061 7761  .            awa
+000036e0: 6974 2073 656c 662e 5f61 7070 2e75 7064  it self._app.upd
+000036f0: 6174 655f 7265 706f 7274 2872 5f68 6173  ate_report(r_has
+00003700: 683d 725f 6861 7368 2c20 6f72 6465 723d  h=r_hash, order=
+00003710: 6f72 6465 722c 202a 2a70 6172 616d 7329  order, **params)
+00003720: 0a0a 2020 2020 2020 2020 6966 2070 6172  ..        if par
+00003730: 656e 745f 7461 6273 5f69 6e64 6578 3a0a  ent_tabs_index:.
+00003740: 2020 2020 2020 2020 2020 2020 705f 6861              p_ha
+00003750: 7368 203d 2073 656c 662e 5f67 6574 5f68  sh = self._get_h
+00003760: 6173 685f 666f 725f 636f 6e74 6169 6e65  ash_for_containe
+00003770: 7228 7061 7265 6e74 5f74 6162 735f 696e  r(parent_tabs_in
+00003780: 6465 785b 305d 290a 2020 2020 2020 2020  dex[0]).        
+00003790: 2020 2020 7061 7265 6e74 5f74 6162 735f      parent_tabs_
+000037a0: 6772 6f75 703a 204f 7074 696f 6e61 6c5b  group: Optional[
+000037b0: 5461 6273 4772 6f75 705d 203d 2061 7761  TabsGroup] = awa
+000037c0: 6974 2073 656c 662e 5f61 7070 2e67 6574  it self._app.get
+000037d0: 5f72 6570 6f72 7428 0a20 2020 2020 2020  _report(.       
+000037e0: 2020 2020 2020 2020 2072 5f68 6173 683d           r_hash=
+000037f0: 705f 6861 7368 0a20 2020 2020 2020 2020  p_hash.         
+00003800: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+00003810: 2069 6620 6e6f 7420 7061 7265 6e74 5f74   if not parent_t
+00003820: 6162 735f 6772 6f75 703a 0a20 2020 2020  abs_group:.     
+00003830: 2020 2020 2020 2020 2020 206c 6f67 5f65             log_e
+00003840: 7272 6f72 280a 2020 2020 2020 2020 2020  rror(.          
+00003850: 2020 2020 2020 2020 2020 6c6f 6767 6572            logger
+00003860: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00003870: 2020 2020 2020 6622 4e6f 2074 6162 7320        f"No tabs 
+00003880: 6772 6f75 7020 666f 756e 6420 7769 7468  group found with
+00003890: 206e 616d 6520 7b70 6172 656e 745f 7461   name {parent_ta
+000038a0: 6273 5f69 6e64 6578 5b30 5d7d 222c 0a20  bs_index[0]}",. 
+000038b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000038c0: 2020 2054 6162 7345 7272 6f72 2c0a 2020     TabsError,.  
+000038d0: 2020 2020 2020 2020 2020 2020 2020 290a                ).
+000038e0: 2020 2020 2020 2020 2020 2020 6966 2070              if p
+000038f0: 6172 656e 745f 7461 6273 5f67 726f 7570  arent_tabs_group
+00003900: 5b22 6964 225d 203d 3d20 7461 6273 5f67  ["id"] == tabs_g
+00003910: 726f 7570 5b22 6964 225d 3a0a 2020 2020  roup["id"]:.    
+00003920: 2020 2020 2020 2020 2020 2020 6c6f 675f              log_
+00003930: 6572 726f 7228 6c6f 6767 6572 2c20 2243  error(logger, "C
+00003940: 616e 6e6f 7420 696e 636c 7564 6520 7461  annot include ta
+00003950: 6273 2067 726f 7570 2069 6e20 6974 7365  bs group in itse
+00003960: 6c66 222c 2054 6162 7345 7272 6f72 290a  lf", TabsError).
+00003970: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+00003980: 656c 662e 5f63 7572 7265 6e74 5f6d 6f64  elf._current_mod
+00003990: 616c 3a0a 2020 2020 2020 2020 2020 2020  al:.            
+000039a0: 2020 2020 6c6f 675f 6572 726f 7228 0a20      log_error(. 
+000039b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000039c0: 2020 206c 6f67 6765 722c 0a20 2020 2020     logger,.     
+000039d0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+000039e0: 4361 6e6e 6f74 2069 6e63 6c75 6465 2061  Cannot include a
+000039f0: 2074 6162 7320 6772 6f75 7020 696e 2061   tabs group in a
+00003a00: 206d 6f64 616c 2061 6e64 2069 6e20 616e   modal and in an
+00003a10: 6f74 6865 7220 7461 6273 2067 726f 7570  other tabs group
+00003a20: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00003a30: 2020 2020 2020 2054 6162 7345 7272 6f72         TabsError
+00003a40: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00003a50: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
+00003a60: 6966 206e 6f74 2070 6172 656e 745f 7461  if not parent_ta
+00003a70: 6273 5f67 726f 7570 2e68 6173 5f72 6570  bs_group.has_rep
+00003a80: 6f72 7428 7461 6273 5f67 726f 7570 293a  ort(tabs_group):
+00003a90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003aa0: 2070 6172 656e 745f 7461 6273 5f67 726f   parent_tabs_gro
+00003ab0: 7570 2e61 6464 5f72 6570 6f72 7428 0a20  up.add_report(. 
+00003ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003ad0: 2020 2074 6162 3d70 6172 656e 745f 7461     tab=parent_ta
+00003ae0: 6273 5f69 6e64 6578 5b31 5d2c 2072 6570  bs_index[1], rep
+00003af0: 6f72 743d 7461 6273 5f67 726f 7570 0a20  ort=tabs_group. 
+00003b00: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+00003b10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003b20: 206c 6f67 6765 722e 696e 666f 280a 2020   logger.info(.  
+00003b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003b40: 2020 6622 496e 636c 7564 6564 2074 6162    f"Included tab
+00003b50: 7320 6772 6f75 7020 7b74 6162 735f 696e  s group {tabs_in
+00003b60: 6465 785b 305d 7d20 696e 2074 6162 7320  dex[0]} in tabs 
+00003b70: 6772 6f75 7020 7b70 6172 656e 745f 7461  group {parent_ta
+00003b80: 6273 5f69 6e64 6578 5b30 5d7d 220a 2020  bs_index[0]}".  
+00003b90: 2020 2020 2020 2020 2020 2020 2020 290a                ).
+00003ba0: 0a20 2020 2020 2020 2065 6c69 6620 7365  .        elif se
+00003bb0: 6c66 2e5f 6375 7272 656e 745f 6d6f 6461  lf._current_moda
+00003bc0: 6c20 616e 6420 6e6f 7420 7365 6c66 2e5f  l and not self._
+00003bd0: 6375 7272 656e 745f 6d6f 6461 6c2e 6861  current_modal.ha
+00003be0: 735f 7265 706f 7274 2874 6162 735f 6772  s_report(tabs_gr
+00003bf0: 6f75 7029 3a0a 2020 2020 2020 2020 2020  oup):.          
+00003c00: 2020 2861 7761 6974 2073 656c 662e 5f67    (await self._g
+00003c10: 6574 5f63 7572 7265 6e74 5f6d 6f64 616c  et_current_modal
+00003c20: 2829 292e 6164 645f 7265 706f 7274 2874  ()).add_report(t
+00003c30: 6162 735f 6772 6f75 7029 0a20 2020 2020  abs_group).     
+00003c40: 2020 2020 2020 206c 6f67 6765 722e 696e         logger.in
+00003c50: 666f 280a 2020 2020 2020 2020 2020 2020  fo(.            
+00003c60: 2020 2020 6622 496e 636c 7564 6564 2074      f"Included t
+00003c70: 6162 7320 6772 6f75 7020 7b74 6162 735f  abs group {tabs_
+00003c80: 696e 6465 785b 305d 7d20 696e 206d 6f64  index[0]} in mod
+00003c90: 616c 207b 7374 7228 7365 6c66 2e5f 6375  al {str(self._cu
+00003ca0: 7272 656e 745f 6d6f 6461 6c29 7d22 0a20  rrent_modal)}". 
+00003cb0: 2020 2020 2020 2020 2020 2029 0a0a 2020             )..  
+00003cc0: 2020 2020 2020 7365 6c66 2e5f 6375 7272        self._curr
+00003cd0: 656e 745f 7461 6273 5f67 726f 7570 203d  ent_tabs_group =
+00003ce0: 2074 6162 735f 6772 6f75 700a 2020 2020   tabs_group.    
+00003cf0: 2020 2020 7461 6273 5f67 726f 7570 2e61      tabs_group.a
+00003d00: 6464 5f74 6162 2874 6162 735f 696e 6465  dd_tab(tabs_inde
+00003d10: 785b 315d 290a 2020 2020 2020 2020 7365  x[1]).        se
+00003d20: 6c66 2e5f 6375 7272 656e 745f 7461 6220  lf._current_tab 
+00003d30: 3d20 7461 6273 5f69 6e64 6578 5b31 5d0a  = tabs_index[1].
+00003d40: 0a20 2020 2020 2020 2069 6620 2275 7064  .        if "upd
+00003d50: 6174 655f 636f 6e74 6169 6e65 7273 2220  ate_containers" 
+00003d60: 6e6f 7420 696e 2073 656c 662e 5f61 7379  not in self._asy
+00003d70: 6e63 5f70 6f6f 6c2e 656e 6469 6e67 5f74  nc_pool.ending_t
+00003d80: 6173 6b73 3a0a 2020 2020 2020 2020 2020  asks:.          
+00003d90: 2020 7365 6c66 2e5f 6173 796e 635f 706f    self._async_po
+00003da0: 6f6c 2e65 6e64 696e 675f 7461 736b 735b  ol.ending_tasks[
+00003db0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003dc0: 2022 7570 6461 7465 5f63 6f6e 7461 696e   "update_contain
+00003dd0: 6572 7322 0a20 2020 2020 2020 2020 2020  ers".           
+00003de0: 205d 203d 2073 656c 662e 5f75 7064 6174   ] = self._updat
+00003df0: 655f 636f 6e74 6169 6e65 7273 2829 0a0a  e_containers()..
+00003e00: 2020 2020 6465 6620 706f 705f 6f75 745f      def pop_out_
+00003e10: 6f66 5f74 6162 735f 6772 6f75 7028 7365  of_tabs_group(se
+00003e20: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
+00003e30: 0a20 2020 2020 2020 2050 6f70 2074 6865  .        Pop the
+00003e40: 2063 7572 7265 6e74 2074 6162 7320 696e   current tabs in
+00003e50: 6465 782e 0a20 2020 2020 2020 2022 2222  dex..        """
+00003e60: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
+00003e70: 7365 6c66 2e5f 6375 7272 656e 745f 7461  self._current_ta
+00003e80: 6273 5f67 726f 7570 3a0a 2020 2020 2020  bs_group:.      
+00003e90: 2020 2020 2020 6c6f 675f 6572 726f 7228        log_error(
+00003ea0: 6c6f 6767 6572 2c20 224e 6f20 7461 6273  logger, "No tabs
+00003eb0: 2067 726f 7570 2074 6f20 706f 7020 6f75   group to pop ou
+00003ec0: 7420 6f66 222c 2054 6162 7345 7272 6f72  t of", TabsError
+00003ed0: 290a 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+00003ee0: 5f63 7572 7265 6e74 5f74 6162 735f 6772  _current_tabs_gr
+00003ef0: 6f75 7020 3d20 4e6f 6e65 0a20 2020 2020  oup = None.     
+00003f00: 2020 2073 656c 662e 5f63 7572 7265 6e74     self._current
+00003f10: 5f74 6162 203d 204e 6f6e 650a 0a20 2020  _tab = None..   
+00003f20: 2064 6566 2063 6861 6e67 655f 6375 7272   def change_curr
+00003f30: 656e 745f 7461 6228 7365 6c66 2c20 7461  ent_tab(self, ta
+00003f40: 623a 2073 7472 293a 0a20 2020 2020 2020  b: str):.       
+00003f50: 2022 2222 0a20 2020 2020 2020 2043 6861   """.        Cha
+00003f60: 6e67 6520 7468 6520 6375 7272 656e 7420  nge the current 
+00003f70: 7461 622e 0a20 2020 2020 2020 203a 7061  tab..        :pa
+00003f80: 7261 6d20 7461 623a 2074 6865 206e 616d  ram tab: the nam
+00003f90: 6520 6f66 2074 6865 2074 6162 0a20 2020  e of the tab.   
+00003fa0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00003fb0: 2069 6620 6e6f 7420 7365 6c66 2e5f 6375   if not self._cu
+00003fc0: 7272 656e 745f 7461 6273 5f67 726f 7570  rrent_tabs_group
+00003fd0: 3a0a 2020 2020 2020 2020 2020 2020 6c6f  :.            lo
+00003fe0: 675f 6572 726f 7228 6c6f 6767 6572 2c20  g_error(logger, 
+00003ff0: 224e 6f20 7461 6273 2067 726f 7570 2074  "No tabs group t
+00004000: 6f20 6368 616e 6765 2074 6162 222c 2054  o change tab", T
+00004010: 6162 7345 7272 6f72 290a 0a20 2020 2020  absError)..     
+00004020: 2020 2073 656c 662e 5f63 7572 7265 6e74     self._current
+00004030: 5f74 6162 735f 6772 6f75 702e 6164 645f  _tabs_group.add_
+00004040: 7461 6228 7461 6229 0a20 2020 2020 2020  tab(tab).       
+00004050: 2073 656c 662e 5f63 7572 7265 6e74 5f74   self._current_t
+00004060: 6162 203d 2074 6162 0a0a 2020 2020 2020  ab = tab..      
+00004070: 2020 6966 2022 7570 6461 7465 5f63 6f6e    if "update_con
+00004080: 7461 696e 6572 7322 206e 6f74 2069 6e20  tainers" not in 
+00004090: 7365 6c66 2e5f 6173 796e 635f 706f 6f6c  self._async_pool
+000040a0: 2e65 6e64 696e 675f 7461 736b 733a 0a20  .ending_tasks:. 
+000040b0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000040c0: 5f61 7379 6e63 5f70 6f6f 6c2e 656e 6469  _async_pool.endi
+000040d0: 6e67 5f74 6173 6b73 5b0a 2020 2020 2020  ng_tasks[.      
+000040e0: 2020 2020 2020 2020 2020 2275 7064 6174            "updat
+000040f0: 655f 636f 6e74 6169 6e65 7273 220a 2020  e_containers".  
+00004100: 2020 2020 2020 2020 2020 5d20 3d20 7365            ] = se
+00004110: 6c66 2e5f 7570 6461 7465 5f63 6f6e 7461  lf._update_conta
+00004120: 696e 6572 7328 290a 0a20 2020 2061 7379  iners()..    asy
+00004130: 6e63 2064 6566 205f 6765 745f 6d6f 6461  nc def _get_moda
+00004140: 6c28 0a20 2020 2020 2020 2073 656c 662c  l(.        self,
+00004150: 0a20 2020 2020 2020 206d 6f64 616c 5f6e  .        modal_n
+00004160: 616d 653a 2073 7472 2c0a 2020 2020 2020  ame: str,.      
+00004170: 2020 7769 6474 683a 204f 7074 696f 6e61    width: Optiona
+00004180: 6c5b 696e 745d 203d 204e 6f6e 652c 0a20  l[int] = None,. 
+00004190: 2020 2020 2020 2068 6569 6768 743a 204f         height: O
+000041a0: 7074 696f 6e61 6c5b 696e 745d 203d 204e  ptional[int] = N
+000041b0: 6f6e 652c 0a20 2020 2020 2020 206f 7065  one,.        ope
+000041c0: 6e5f 6279 5f64 6566 6175 6c74 3a20 4f70  n_by_default: Op
+000041d0: 7469 6f6e 616c 5b62 6f6f 6c5d 203d 204e  tional[bool] = N
+000041e0: 6f6e 652c 0a20 2020 2029 202d 3e20 4d6f  one,.    ) -> Mo
+000041f0: 6461 6c3a 0a20 2020 2020 2020 2072 5f68  dal:.        r_h
+00004200: 6173 6820 3d20 7365 6c66 2e5f 6765 745f  ash = self._get_
+00004210: 6861 7368 5f66 6f72 5f63 6f6e 7461 696e  hash_for_contain
+00004220: 6572 286d 6f64 616c 5f6e 616d 6529 0a20  er(modal_name). 
+00004230: 2020 2020 2020 206d 6f64 616c 3a20 4f70         modal: Op
+00004240: 7469 6f6e 616c 5b4d 6f64 616c 5d20 3d20  tional[Modal] = 
+00004250: 6177 6169 7420 7365 6c66 2e5f 6170 702e  await self._app.
+00004260: 6765 745f 7265 706f 7274 2872 5f68 6173  get_report(r_has
+00004270: 683d 725f 6861 7368 290a 2020 2020 2020  h=r_hash).      
+00004280: 2020 6966 206e 6f74 206d 6f64 616c 3a0a    if not modal:.
+00004290: 2020 2020 2020 2020 2020 2020 6d6f 6461              moda
+000042a0: 6c3a 2052 6570 6f72 7420 3d20 6177 6169  l: Report = awai
+000042b0: 7420 7365 6c66 2e5f 6170 702e 6372 6561  t self._app.crea
+000042c0: 7465 5f72 6570 6f72 7428 0a20 2020 2020  te_report(.     
+000042d0: 2020 2020 2020 2020 2020 204d 6f64 616c             Modal
+000042e0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000042f0: 2020 725f 6861 7368 3d72 5f68 6173 682c    r_hash=r_hash,
+00004300: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004310: 2070 6174 683d 7365 6c66 2e5f 6375 7272   path=self._curr
+00004320: 656e 745f 7061 7468 2c0a 2020 2020 2020  ent_path,.      
+00004330: 2020 2020 2020 2020 2020 7072 6f70 6572            proper
+00004340: 7469 6573 3d7b 2277 6964 7468 223a 2077  ties={"width": w
+00004350: 6964 7468 2c20 2268 6569 6768 7422 3a20  idth, "height": 
+00004360: 6865 6967 6874 2c20 226f 7065 6e22 3a20  height, "open": 
+00004370: 6f70 656e 5f62 795f 6465 6661 756c 747d  open_by_default}
+00004380: 2c0a 2020 2020 2020 2020 2020 2020 290a  ,.            ).
+00004390: 2020 2020 2020 2020 2020 2020 6c6f 6767              logg
+000043a0: 6572 2e69 6e66 6f28 6627 4372 6561 7465  er.info(f'Create
+000043b0: 6420 6d6f 6461 6c20 7b6d 6f64 616c 5f6e  d modal {modal_n
+000043c0: 616d 657d 2077 6974 6820 6964 207b 6d6f  ame} with id {mo
+000043d0: 6461 6c5b 2269 6422 5d7d 2729 0a20 2020  dal["id"]}').   
+000043e0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+000043f0: 6d6f 6461 6c0a 2020 2020 2020 2020 7072  modal.        pr
+00004400: 6f70 6572 7469 6573 203d 207b 7d0a 2020  operties = {}.  
+00004410: 2020 2020 2020 6966 2077 6964 7468 3a0a        if width:.
+00004420: 2020 2020 2020 2020 2020 2020 7072 6f70              prop
+00004430: 6572 7469 6573 5b22 7769 6474 6822 5d20  erties["width"] 
+00004440: 3d20 7769 6474 680a 2020 2020 2020 2020  = width.        
+00004450: 6966 2068 6569 6768 743a 0a20 2020 2020  if height:.     
+00004460: 2020 2020 2020 2070 726f 7065 7274 6965         propertie
+00004470: 735b 2268 6569 6768 7422 5d20 3d20 6865  s["height"] = he
+00004480: 6967 6874 0a20 2020 2020 2020 2069 6620  ight.        if 
+00004490: 6f70 656e 5f62 795f 6465 6661 756c 743a  open_by_default:
+000044a0: 0a20 2020 2020 2020 2020 2020 2070 726f  .            pro
+000044b0: 7065 7274 6965 735b 226f 7065 6e22 5d20  perties["open"] 
+000044c0: 3d20 6f70 656e 5f62 795f 6465 6661 756c  = open_by_defaul
+000044d0: 740a 2020 2020 2020 2020 6966 2070 726f  t.        if pro
+000044e0: 7065 7274 6965 733a 0a20 2020 2020 2020  perties:.       
+000044f0: 2020 2020 2061 7761 6974 2073 656c 662e       await self.
+00004500: 5f61 7070 2e75 7064 6174 655f 7265 706f  _app.update_repo
+00004510: 7274 280a 2020 2020 2020 2020 2020 2020  rt(.            
+00004520: 2020 2020 725f 6861 7368 3d72 5f68 6173      r_hash=r_has
+00004530: 682c 2070 726f 7065 7274 6965 733d 7072  h, properties=pr
+00004540: 6f70 6572 7469 6573 2c20 7061 7468 3d73  operties, path=s
+00004550: 656c 662e 5f63 7572 7265 6e74 5f70 6174  elf._current_pat
+00004560: 680a 2020 2020 2020 2020 2020 2020 290a  h.            ).
+00004570: 2020 2020 2020 2020 2020 2020 6c6f 6767              logg
+00004580: 6572 2e69 6e66 6f28 6627 5570 6461 7465  er.info(f'Update
+00004590: 6420 6d6f 6461 6c20 7b6d 6f64 616c 5f6e  d modal {modal_n
+000045a0: 616d 657d 2077 6974 6820 6964 207b 6d6f  ame} with id {mo
+000045b0: 6461 6c5b 2269 6422 5d7d 2729 0a20 2020  dal["id"]}').   
+000045c0: 2020 2020 2072 6574 7572 6e20 6d6f 6461       return moda
+000045d0: 6c0a 0a20 2020 2061 7379 6e63 2064 6566  l..    async def
+000045e0: 2073 6574 5f6d 6f64 616c 280a 2020 2020   set_modal(.    
+000045f0: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
+00004600: 2020 6d6f 6461 6c5f 6e61 6d65 3a20 7374    modal_name: st
+00004610: 722c 0a20 2020 2020 2020 2077 6964 7468  r,.        width
+00004620: 3a20 4f70 7469 6f6e 616c 5b69 6e74 5d20  : Optional[int] 
+00004630: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+00004640: 6865 6967 6874 3a20 4f70 7469 6f6e 616c  height: Optional
+00004650: 5b69 6e74 5d20 3d20 4e6f 6e65 2c0a 2020  [int] = None,.  
+00004660: 2020 2020 2020 6f70 656e 5f62 795f 6465        open_by_de
+00004670: 6661 756c 743a 204f 7074 696f 6e61 6c5b  fault: Optional[
+00004680: 626f 6f6c 5d20 3d20 4e6f 6e65 2c0a 2020  bool] = None,.  
+00004690: 2020 2920 2d3e 204e 6f6e 653a 0a20 2020    ) -> None:.   
+000046a0: 2020 2020 2022 2222 5365 7420 7468 6520       """Set the 
+000046b0: 6375 7272 656e 7420 6d6f 6461 6c2e 0a20  current modal.. 
+000046c0: 2020 2020 2020 203a 7061 7261 6d20 6d6f         :param mo
+000046d0: 6461 6c5f 6e61 6d65 3a20 7468 6520 6e61  dal_name: the na
+000046e0: 6d65 206f 6620 7468 6520 6d6f 6461 6c0a  me of the modal.
+000046f0: 2020 2020 2020 2020 3a70 6172 616d 2077          :param w
+00004700: 6964 7468 3a20 7468 6520 7769 6474 6820  idth: the width 
+00004710: 6f66 2074 6865 206d 6f64 616c 0a20 2020  of the modal.   
+00004720: 2020 2020 203a 7061 7261 6d20 6865 6967       :param heig
+00004730: 6874 3a20 7468 6520 6865 6967 6874 206f  ht: the height o
+00004740: 6620 7468 6520 6d6f 6461 6c0a 2020 2020  f the modal.    
+00004750: 2020 2020 3a70 6172 616d 206f 7065 6e5f      :param open_
+00004760: 6279 5f64 6566 6175 6c74 3a20 7768 6574  by_default: whet
+00004770: 6865 7220 7468 6520 6d6f 6461 6c20 6973  her the modal is
+00004780: 206f 7065 6e20 6279 2064 6566 6175 6c74   open by default
+00004790: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+000047a0: 2020 2020 2069 6620 7365 6c66 2e5f 6375       if self._cu
+000047b0: 7272 656e 745f 7461 6273 5f67 726f 7570  rrent_tabs_group
+000047c0: 3a0a 2020 2020 2020 2020 2020 2020 6c6f  :.            lo
+000047d0: 675f 6572 726f 7228 0a20 2020 2020 2020  g_error(.       
+000047e0: 2020 2020 2020 2020 206c 6f67 6765 722c           logger,
+000047f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004800: 2022 4361 6e6e 6f74 2073 6574 2061 206d   "Cannot set a m
+00004810: 6f64 616c 2069 6e20 6120 7461 6273 2067  odal in a tabs g
+00004820: 726f 7570 2c20 706f 7020 6f75 7420 6f66  roup, pop out of
+00004830: 2074 6865 2074 6162 7320 6772 6f75 7020   the tabs group 
+00004840: 6669 7273 7422 2c0a 2020 2020 2020 2020  first",.        
+00004850: 2020 2020 2020 2020 4d6f 6461 6c45 7272          ModalErr
+00004860: 6f72 2c0a 2020 2020 2020 2020 2020 2020  or,.            
+00004870: 290a 0a20 2020 2020 2020 206d 6f64 616c  )..        modal
+00004880: 203d 2061 7761 6974 2073 656c 662e 5f67   = await self._g
+00004890: 6574 5f6d 6f64 616c 286d 6f64 616c 5f6e  et_modal(modal_n
+000048a0: 616d 652c 2077 6964 7468 2c20 6865 6967  ame, width, heig
+000048b0: 6874 2c20 6f70 656e 5f62 795f 6465 6661  ht, open_by_defa
+000048c0: 756c 7429 0a20 2020 2020 2020 2073 656c  ult).        sel
+000048d0: 662e 5f63 7572 7265 6e74 5f6d 6f64 616c  f._current_modal
+000048e0: 203d 206d 6f64 616c 0a0a 2020 2020 2020   = modal..      
+000048f0: 2020 6966 2022 7570 6461 7465 5f63 6f6e    if "update_con
+00004900: 7461 696e 6572 7322 206e 6f74 2069 6e20  tainers" not in 
+00004910: 7365 6c66 2e5f 6173 796e 635f 706f 6f6c  self._async_pool
+00004920: 2e65 6e64 696e 675f 7461 736b 733a 0a20  .ending_tasks:. 
+00004930: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00004940: 5f61 7379 6e63 5f70 6f6f 6c2e 656e 6469  _async_pool.endi
+00004950: 6e67 5f74 6173 6b73 5b0a 2020 2020 2020  ng_tasks[.      
+00004960: 2020 2020 2020 2020 2020 2275 7064 6174            "updat
+00004970: 655f 636f 6e74 6169 6e65 7273 220a 2020  e_containers".  
+00004980: 2020 2020 2020 2020 2020 5d20 3d20 7365            ] = se
+00004990: 6c66 2e5f 7570 6461 7465 5f63 6f6e 7461  lf._update_conta
+000049a0: 696e 6572 7328 290a 0a20 2020 2064 6566  iners()..    def
+000049b0: 2070 6f70 5f6f 7574 5f6f 665f 6d6f 6461   pop_out_of_moda
+000049c0: 6c28 7365 6c66 293a 0a20 2020 2020 2020  l(self):.       
+000049d0: 2022 2222 506f 7020 7468 6520 6375 7272   """Pop the curr
+000049e0: 656e 7420 6d6f 6461 6c2e 2222 220a 2020  ent modal.""".  
+000049f0: 2020 2020 2020 6966 206e 6f74 2073 656c        if not sel
+00004a00: 662e 5f63 7572 7265 6e74 5f6d 6f64 616c  f._current_modal
+00004a10: 3a0a 2020 2020 2020 2020 2020 2020 6c6f  :.            lo
+00004a20: 675f 6572 726f 7228 6c6f 6767 6572 2c20  g_error(logger, 
+00004a30: 224e 6f20 6d6f 6461 6c20 746f 2070 6f70  "No modal to pop
+00004a40: 206f 7574 206f 6622 2c20 4d6f 6461 6c45   out of", ModalE
+00004a50: 7272 6f72 290a 0a20 2020 2020 2020 2069  rror)..        i
+00004a60: 6620 7365 6c66 2e5f 6375 7272 656e 745f  f self._current_
+00004a70: 7461 6273 5f67 726f 7570 3a0a 2020 2020  tabs_group:.    
+00004a80: 2020 2020 2020 2020 6c6f 675f 6572 726f          log_erro
+00004a90: 7228 0a20 2020 2020 2020 2020 2020 2020  r(.             
+00004aa0: 2020 206c 6f67 6765 722c 0a20 2020 2020     logger,.     
+00004ab0: 2020 2020 2020 2020 2020 2022 4361 6e6e             "Cann
+00004ac0: 6f74 2070 6f70 206f 7574 206f 6620 6120  ot pop out of a 
+00004ad0: 6d6f 6461 6c20 7768 656e 2069 6e20 6120  modal when in a 
+00004ae0: 7461 6273 2067 726f 7570 2c20 706f 7020  tabs group, pop 
+00004af0: 6f75 7420 6f66 2074 6865 2074 6162 7320  out of the tabs 
+00004b00: 6772 6f75 7020 6669 7273 7422 2c0a 2020  group first",.  
+00004b10: 2020 2020 2020 2020 2020 2020 2020 4d6f                Mo
+00004b20: 6461 6c45 7272 6f72 2c0a 2020 2020 2020  dalError,.      
+00004b30: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+00004b40: 6966 2073 656c 662e 5f62 656e 746f 626f  if self._bentobo
+00004b50: 785f 6461 7461 3a0a 2020 2020 2020 2020  x_data:.        
+00004b60: 2020 2020 6c6f 675f 6572 726f 7228 0a20      log_error(. 
+00004b70: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+00004b80: 6f67 6765 722c 0a20 2020 2020 2020 2020  ogger,.         
+00004b90: 2020 2020 2020 2022 4361 6e6e 6f74 2070         "Cannot p
+00004ba0: 6f70 206f 7574 206f 6620 6120 6d6f 6461  op out of a moda
+00004bb0: 6c20 7768 656e 2069 6e20 6120 6265 6e74  l when in a bent
+00004bc0: 6f62 6f78 2c20 636c 6f73 6520 7468 6520  obox, close the 
+00004bd0: 6265 6e74 6f62 6f78 2066 6972 7374 222c  bentobox first",
+00004be0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004bf0: 204d 6f64 616c 4572 726f 722c 0a20 2020   ModalError,.   
+00004c00: 2020 2020 2020 2020 2029 0a0a 2020 2020           )..    
+00004c10: 2020 2020 7365 6c66 2e5f 6375 7272 656e      self._curren
+00004c20: 745f 6d6f 6461 6c20 3d20 4e6f 6e65 0a0a  t_modal = None..
+00004c30: 2020 2020 6173 796e 6320 6465 6620 5f67      async def _g
+00004c40: 6574 5f63 7572 7265 6e74 5f6d 6f64 616c  et_current_modal
+00004c50: 2873 656c 6629 202d 3e20 4d6f 6461 6c3a  (self) -> Modal:
+00004c60: 0a20 2020 2020 2020 2022 2222 4765 7420  .        """Get 
+00004c70: 7468 6520 6375 7272 656e 7420 6d6f 6461  the current moda
+00004c80: 6c2e 2222 220a 2020 2020 2020 2020 6966  l.""".        if
+00004c90: 206e 6f74 2073 656c 662e 5f63 7572 7265   not self._curre
+00004ca0: 6e74 5f6d 6f64 616c 3a0a 2020 2020 2020  nt_modal:.      
+00004cb0: 2020 2020 2020 6c6f 675f 6572 726f 7228        log_error(
+00004cc0: 6c6f 6767 6572 2c20 224e 6f20 6d6f 6461  logger, "No moda
+00004cd0: 6c20 7365 7422 2c20 4d6f 6461 6c45 7272  l set", ModalErr
+00004ce0: 6f72 290a 2020 2020 2020 2020 6966 2073  or).        if s
+00004cf0: 656c 662e 5f61 7070 2e61 7069 5f63 6c69  elf._app.api_cli
+00004d00: 656e 742e 6361 6368 655f 656e 6162 6c65  ent.cache_enable
+00004d10: 643a 0a20 2020 2020 2020 2020 2020 2072  d:.            r
+00004d20: 6574 7572 6e20 7365 6c66 2e5f 6375 7272  eturn self._curr
+00004d30: 656e 745f 6d6f 6461 6c0a 2020 2020 2020  ent_modal.      
+00004d40: 2020 6c61 7374 5f6d 6f64 616c 203d 2073    last_modal = s
+00004d50: 656c 662e 5f63 7572 7265 6e74 5f6d 6f64  elf._current_mod
+00004d60: 616c 0a20 2020 2020 2020 2073 656c 662e  al.        self.
+00004d70: 5f63 7572 7265 6e74 5f6d 6f64 616c 203d  _current_modal =
+00004d80: 2061 7761 6974 2073 656c 662e 5f61 7070   await self._app
+00004d90: 2e67 6574 5f72 6570 6f72 7428 0a20 2020  .get_report(.   
+00004da0: 2020 2020 2020 2020 2072 5f68 6173 683d           r_hash=
+00004db0: 7365 6c66 2e5f 6375 7272 656e 745f 6d6f  self._current_mo
+00004dc0: 6461 6c5b 2270 726f 7065 7274 6965 7322  dal["properties"
+00004dd0: 5d5b 2268 6173 6822 5d0a 2020 2020 2020  ]["hash"].      
+00004de0: 2020 290a 2020 2020 2020 2020 6966 2073    ).        if s
+00004df0: 656c 662e 5f63 7572 7265 6e74 5f6d 6f64  elf._current_mod
+00004e00: 616c 2069 7320 4e6f 6e65 3a0a 2020 2020  al is None:.    
+00004e10: 2020 2020 2020 2020 6c6f 675f 6572 726f          log_erro
+00004e20: 7228 0a20 2020 2020 2020 2020 2020 2020  r(.             
+00004e30: 2020 206c 6f67 6765 722c 0a20 2020 2020     logger,.     
+00004e40: 2020 2020 2020 2020 2020 2066 274e 6f20             f'No 
+00004e50: 6d6f 6461 6c20 666f 756e 6420 7769 7468  modal found with
+00004e60: 206e 616d 6520 7b6c 6173 745f 6d6f 6461   name {last_moda
+00004e70: 6c5b 2270 726f 7065 7274 6965 7322 5d5b  l["properties"][
+00004e80: 226e 616d 6522 5d7d 272c 0a20 2020 2020  "name"]}',.     
+00004e90: 2020 2020 2020 2020 2020 204d 6f64 616c             Modal
+00004ea0: 4572 726f 722c 0a20 2020 2020 2020 2020  Error,.         
+00004eb0: 2020 2029 0a20 2020 2020 2020 2072 6574     ).        ret
+00004ec0: 7572 6e20 7365 6c66 2e5f 6375 7272 656e  urn self._curren
+00004ed0: 745f 6d6f 6461 6c0a 0a20 2020 2061 7379  t_modal..    asy
+00004ee0: 6e63 2064 6566 205f 6765 745f 6375 7272  nc def _get_curr
+00004ef0: 656e 745f 7461 6273 5f67 726f 7570 2873  ent_tabs_group(s
+00004f00: 656c 6629 202d 3e20 5461 6273 4772 6f75  elf) -> TabsGrou
+00004f10: 703a 0a20 2020 2020 2020 2022 2222 4765  p:.        """Ge
+00004f20: 7420 7468 6520 6375 7272 656e 7420 7461  t the current ta
+00004f30: 6273 2067 726f 7570 2e22 2222 0a20 2020  bs group.""".   
+00004f40: 2020 2020 2069 6620 6e6f 7420 7365 6c66       if not self
+00004f50: 2e5f 6375 7272 656e 745f 7461 6273 5f67  ._current_tabs_g
+00004f60: 726f 7570 3a0a 2020 2020 2020 2020 2020  roup:.          
+00004f70: 2020 6c6f 675f 6572 726f 7228 6c6f 6767    log_error(logg
+00004f80: 6572 2c20 224e 6f20 7461 6273 2067 726f  er, "No tabs gro
+00004f90: 7570 2067 6574 222c 2054 6162 7345 7272  up get", TabsErr
+00004fa0: 6f72 290a 2020 2020 2020 2020 6966 2073  or).        if s
+00004fb0: 656c 662e 5f61 7070 2e61 7069 5f63 6c69  elf._app.api_cli
+00004fc0: 656e 742e 6361 6368 655f 656e 6162 6c65  ent.cache_enable
+00004fd0: 643a 0a20 2020 2020 2020 2020 2020 2072  d:.            r
+00004fe0: 6574 7572 6e20 7365 6c66 2e5f 6375 7272  eturn self._curr
+00004ff0: 656e 745f 7461 6273 5f67 726f 7570 0a20  ent_tabs_group. 
+00005000: 2020 2020 2020 206c 6173 745f 7461 6273         last_tabs
+00005010: 5f67 726f 7570 203d 2073 656c 662e 5f63  _group = self._c
+00005020: 7572 7265 6e74 5f74 6162 735f 6772 6f75  urrent_tabs_grou
+00005030: 700a 2020 2020 2020 2020 7365 6c66 2e5f  p.        self._
+00005040: 6375 7272 656e 745f 7461 6273 5f67 726f  current_tabs_gro
+00005050: 7570 203d 2061 7761 6974 2073 656c 662e  up = await self.
+00005060: 5f61 7070 2e67 6574 5f72 6570 6f72 7428  _app.get_report(
+00005070: 0a20 2020 2020 2020 2020 2020 2072 5f68  .            r_h
+00005080: 6173 683d 7365 6c66 2e5f 6375 7272 656e  ash=self._curren
+00005090: 745f 7461 6273 5f67 726f 7570 5b22 7072  t_tabs_group["pr
+000050a0: 6f70 6572 7469 6573 225d 5b22 6861 7368  operties"]["hash
+000050b0: 225d 0a20 2020 2020 2020 2029 0a20 2020  "].        ).   
+000050c0: 2020 2020 2069 6620 7365 6c66 2e5f 6375       if self._cu
+000050d0: 7272 656e 745f 7461 6273 5f67 726f 7570  rrent_tabs_group
+000050e0: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
+000050f0: 2020 2020 2020 6c6f 675f 6572 726f 7228        log_error(
+00005100: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005110: 206c 6f67 6765 722c 0a20 2020 2020 2020   logger,.       
+00005120: 2020 2020 2020 2020 2066 274e 6f20 7461           f'No ta
+00005130: 6273 2067 726f 7570 2066 6f75 6e64 2077  bs group found w
+00005140: 6974 6820 6e61 6d65 207b 6c61 7374 5f74  ith name {last_t
+00005150: 6162 735f 6772 6f75 705b 2270 726f 7065  abs_group["prope
+00005160: 7274 6965 7322 5d5b 226e 616d 6522 5d7d  rties"]["name"]}
+00005170: 272c 0a20 2020 2020 2020 2020 2020 2020  ',.             
+00005180: 2020 2054 6162 7345 7272 6f72 2c0a 2020     TabsError,.  
+00005190: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+000051a0: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+000051b0: 5f63 7572 7265 6e74 5f74 6162 735f 6772  _current_tabs_gr
+000051c0: 6f75 700a 0a20 2020 2064 6566 205f 6765  oup..    def _ge
+000051d0: 745f 6368 6172 745f 6861 7368 2873 656c  t_chart_hash(sel
+000051e0: 662c 206f 7264 6572 3a20 696e 7429 202d  f, order: int) -
+000051f0: 3e20 7374 723a 0a20 2020 2020 2020 2072  > str:.        r
+00005200: 5f68 6173 6820 3d20 6622 7b6f 7264 6572  _hash = f"{order
+00005210: 7d22 0a20 2020 2020 2020 2069 6620 7365  }".        if se
+00005220: 6c66 2e5f 6375 7272 656e 745f 7461 6273  lf._current_tabs
+00005230: 5f67 726f 7570 3a0a 2020 2020 2020 2020  _group:.        
+00005240: 2020 2020 725f 6861 7368 203d 2066 277b      r_hash = f'{
+00005250: 7365 6c66 2e5f 6375 7272 656e 745f 7461  self._current_ta
+00005260: 6273 5f67 726f 7570 5b22 7072 6f70 6572  bs_group["proper
+00005270: 7469 6573 225d 5b22 6861 7368 225d 7d5f  ties"]["hash"]}_
+00005280: 7b73 656c 662e 5f63 7572 7265 6e74 5f74  {self._current_t
+00005290: 6162 7d5f 7b6f 7264 6572 7d27 0a20 2020  ab}_{order}'.   
+000052a0: 2020 2020 2065 6c69 6620 7365 6c66 2e5f       elif self._
+000052b0: 6375 7272 656e 745f 6d6f 6461 6c3a 0a20  current_modal:. 
+000052c0: 2020 2020 2020 2020 2020 2072 5f68 6173             r_has
+000052d0: 6820 3d20 6627 7b73 656c 662e 5f63 7572  h = f'{self._cur
+000052e0: 7265 6e74 5f6d 6f64 616c 5b22 7072 6f70  rent_modal["prop
+000052f0: 6572 7469 6573 225d 5b22 6861 7368 225d  erties"]["hash"]
+00005300: 7d5f 7b6f 7264 6572 7d27 0a20 2020 2020  }_{order}'.     
+00005310: 2020 2065 6c69 6620 7365 6c66 2e5f 6375     elif self._cu
+00005320: 7272 656e 745f 7061 7468 3a0a 2020 2020  rrent_path:.    
+00005330: 2020 2020 2020 2020 725f 6861 7368 203d          r_hash =
+00005340: 2066 227b 7365 6c66 2e5f 6375 7272 656e   f"{self._curren
+00005350: 745f 7061 7468 7d5f 7b6f 7264 6572 7d22  t_path}_{order}"
+00005360: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00005370: 725f 6861 7368 0a0a 2020 2020 6173 796e  r_hash..    asyn
+00005380: 6320 6465 6620 5f67 6574 5f63 6861 7274  c def _get_chart
+00005390: 5f72 6570 6f72 7428 0a20 2020 2020 2020  _report(.       
+000053a0: 2073 656c 662c 206f 7264 6572 3a20 696e   self, order: in
+000053b0: 742c 2063 6861 7274 5f63 6c61 7373 3a20  t, chart_class: 
+000053c0: 7479 7065 5b52 6570 6f72 745d 2c20 6372  type[Report], cr
+000053d0: 6561 7465 5f69 665f 6e6f 745f 6578 6973  eate_if_not_exis
+000053e0: 7473 3a20 626f 6f6c 203d 2054 7275 650a  ts: bool = True.
+000053f0: 2020 2020 2920 2d3e 2074 7570 6c65 5b73      ) -> tuple[s
+00005400: 7472 2c20 4f70 7469 6f6e 616c 5b52 6570  tr, Optional[Rep
+00005410: 6f72 745d 5d3a 0a20 2020 2020 2020 2022  ort]]:.        "
+00005420: 2222 4765 7420 7468 6520 6368 6172 7420  ""Get the chart 
+00005430: 7265 706f 7274 2e0a 2020 2020 2020 2020  report..        
+00005440: 3a70 6172 616d 206f 7264 6572 3a20 7468  :param order: th
+00005450: 6520 6f72 6465 7220 6f66 2074 6865 2063  e order of the c
+00005460: 6861 7274 0a20 2020 2020 2020 203a 7061  hart.        :pa
+00005470: 7261 6d20 6368 6172 745f 636c 6173 733a  ram chart_class:
+00005480: 2074 6865 2063 6861 7274 2063 6c61 7373   the chart class
+00005490: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+000054a0: 6372 6561 7465 5f69 665f 6e6f 745f 6578  create_if_not_ex
+000054b0: 6973 7473 3a20 7768 6574 6865 7220 746f  ists: whether to
+000054c0: 2063 7265 6174 6520 7468 6520 6368 6172   create the char
+000054d0: 7420 6966 2069 7420 646f 6573 6e27 7420  t if it doesn't 
+000054e0: 6578 6973 740a 2020 2020 2020 2020 2222  exist.        ""
+000054f0: 220a 2020 2020 2020 2020 725f 6861 7368  ".        r_hash
+00005500: 203d 2073 656c 662e 5f67 6574 5f63 6861   = self._get_cha
+00005510: 7274 5f68 6173 6828 6f72 6465 7229 0a20  rt_hash(order). 
+00005520: 2020 2020 2020 2072 6570 6f72 7420 3d20         report = 
+00005530: 6177 6169 7420 7365 6c66 2e5f 6170 702e  await self._app.
+00005540: 6765 745f 7265 706f 7274 2872 5f68 6173  get_report(r_has
+00005550: 683d 725f 6861 7368 290a 0a20 2020 2020  h=r_hash)..     
+00005560: 2020 2069 6620 6e6f 7420 7265 706f 7274     if not report
+00005570: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
+00005580: 2063 7265 6174 655f 6966 5f6e 6f74 5f65   create_if_not_e
+00005590: 7869 7374 733a 0a20 2020 2020 2020 2020  xists:.         
+000055a0: 2020 2020 2020 2072 6570 6f72 7420 3d20         report = 
+000055b0: 6177 6169 7420 7365 6c66 2e5f 6170 702e  await self._app.
+000055c0: 6372 6561 7465 5f72 6570 6f72 7428 0a20  create_report(. 
+000055d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000055e0: 2020 2063 6861 7274 5f63 6c61 7373 2c20     chart_class, 
+000055f0: 725f 6861 7368 3d72 5f68 6173 682c 206f  r_hash=r_hash, o
+00005600: 7264 6572 3d6f 7264 6572 0a20 2020 2020  rder=order.     
+00005610: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+00005620: 2020 2020 2020 2020 2020 2020 206c 6f67               log
+00005630: 6765 722e 696e 666f 2866 2743 7265 6174  ger.info(f'Creat
+00005640: 6564 207b 6368 6172 745f 636c 6173 732e  ed {chart_class.
+00005650: 5f5f 6e61 6d65 5f5f 7d20 7769 7468 2069  __name__} with i
+00005660: 6420 7b72 6570 6f72 745b 2269 6422 5d7d  d {report["id"]}
+00005670: 2729 0a20 2020 2020 2020 2065 6c69 6620  ').        elif 
+00005680: 7265 706f 7274 2e72 6570 6f72 745f 7479  report.report_ty
+00005690: 7065 2021 3d20 6368 6172 745f 636c 6173  pe != chart_clas
+000056a0: 732e 7265 706f 7274 5f74 7970 653a 0a20  s.report_type:. 
+000056b0: 2020 2020 2020 2020 2020 2061 7761 6974             await
+000056c0: 2072 6570 6f72 742e 6368 616e 6765 5f72   report.change_r
+000056d0: 6570 6f72 745f 7479 7065 2863 6861 7274  eport_type(chart
+000056e0: 5f63 6c61 7373 290a 0a20 2020 2020 2020  _class)..       
+000056f0: 2072 6574 7572 6e20 725f 6861 7368 2c20   return r_hash, 
+00005700: 7265 706f 7274 0a0a 2020 2020 6173 796e  report..    asyn
+00005710: 6320 6465 6620 6765 745f 636f 6d70 6f6e  c def get_compon
+00005720: 656e 745f 6279 5f6f 7264 6572 2873 656c  ent_by_order(sel
+00005730: 662c 206f 7264 6572 3a20 696e 7429 202d  f, order: int) -
+00005740: 3e20 4f70 7469 6f6e 616c 5b64 6963 745d  > Optional[dict]
+00005750: 3a0a 2020 2020 2020 2020 2222 2247 6574  :.        """Get
+00005760: 2074 6865 2063 6f6d 706f 6e65 6e74 2062   the component b
+00005770: 7920 6f72 6465 722e 0a20 2020 2020 2020  y order..       
+00005780: 203a 7061 7261 6d20 6f72 6465 723a 2074   :param order: t
+00005790: 6865 206f 7264 6572 206f 6620 7468 6520  he order of the 
+000057a0: 636f 6d70 6f6e 656e 740a 2020 2020 2020  component.      
+000057b0: 2020 2222 220a 2020 2020 2020 2020 725f    """.        r_
+000057c0: 6861 7368 203d 2073 656c 662e 5f67 6574  hash = self._get
+000057d0: 5f63 6861 7274 5f68 6173 6828 6f72 6465  _chart_hash(orde
+000057e0: 7229 0a20 2020 2020 2020 2072 6570 6f72  r).        repor
+000057f0: 7420 3d20 6177 6169 7420 7365 6c66 2e5f  t = await self._
+00005800: 6170 702e 6765 745f 7265 706f 7274 2872  app.get_report(r
+00005810: 5f68 6173 683d 725f 6861 7368 290a 2020  _hash=r_hash).  
+00005820: 2020 2020 2020 6966 206e 6f74 2072 6570        if not rep
+00005830: 6f72 743a 0a20 2020 2020 2020 2020 2020  ort:.           
+00005840: 2072 6574 7572 6e20 4e6f 6e65 0a20 2020   return None.   
+00005850: 2020 2020 2072 6574 7572 6e20 7265 706f       return repo
+00005860: 7274 2e63 6173 6361 6465 5f74 6f5f 6469  rt.cascade_to_di
+00005870: 6374 2829 0a0a 2020 2020 6173 796e 6320  ct()..    async 
+00005880: 6465 6620 6765 745f 6d6f 6461 6c28 7365  def get_modal(se
+00005890: 6c66 2c20 6d6f 6461 6c5f 6e61 6d65 3a20  lf, modal_name: 
+000058a0: 7374 7229 202d 3e20 4f70 7469 6f6e 616c  str) -> Optional
+000058b0: 5b64 6963 745d 3a0a 2020 2020 2020 2020  [dict]:.        
+000058c0: 2222 2247 6574 2074 6865 206d 6f64 616c  """Get the modal
+000058d0: 2e0a 2020 2020 2020 2020 3a70 6172 616d  ..        :param
+000058e0: 206d 6f64 616c 5f6e 616d 653a 2074 6865   modal_name: the
+000058f0: 206e 616d 6520 6f66 2074 6865 206d 6f64   name of the mod
+00005900: 616c 0a20 2020 2020 2020 2022 2222 0a20  al.        """. 
+00005910: 2020 2020 2020 2072 5f68 6173 6820 3d20         r_hash = 
+00005920: 7365 6c66 2e5f 6765 745f 6861 7368 5f66  self._get_hash_f
+00005930: 6f72 5f63 6f6e 7461 696e 6572 286d 6f64  or_container(mod
+00005940: 616c 5f6e 616d 6529 0a20 2020 2020 2020  al_name).       
+00005950: 206d 6f64 616c 203d 2061 7761 6974 2073   modal = await s
+00005960: 656c 662e 5f61 7070 2e67 6574 5f72 6570  elf._app.get_rep
+00005970: 6f72 7428 725f 6861 7368 3d72 5f68 6173  ort(r_hash=r_has
+00005980: 6829 0a20 2020 2020 2020 2069 6620 6e6f  h).        if no
+00005990: 7420 6d6f 6461 6c3a 0a20 2020 2020 2020  t modal:.       
+000059a0: 2020 2020 2072 6574 7572 6e20 4e6f 6e65       return None
+000059b0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+000059c0: 6d6f 6461 6c2e 6361 7363 6164 655f 746f  modal.cascade_to
+000059d0: 5f64 6963 7428 290a 0a20 2020 2061 7379  _dict()..    asy
+000059e0: 6e63 2064 6566 2067 6574 5f74 6162 735f  nc def get_tabs_
+000059f0: 6772 6f75 7028 7365 6c66 2c20 7461 6273  group(self, tabs
+00005a00: 5f69 6e64 6578 3a20 7475 706c 655b 7374  _index: tuple[st
+00005a10: 722c 2073 7472 5d29 202d 3e20 4f70 7469  r, str]) -> Opti
+00005a20: 6f6e 616c 5b64 6963 745d 3a0a 2020 2020  onal[dict]:.    
+00005a30: 2020 2020 2222 2247 6574 2074 6865 2074      """Get the t
+00005a40: 6162 7320 6772 6f75 702e 0a20 2020 2020  abs group..     
+00005a50: 2020 203a 7061 7261 6d20 7461 6273 5f69     :param tabs_i
+00005a60: 6e64 6578 3a20 7468 6520 696e 6465 7820  ndex: the index 
+00005a70: 6f66 2074 6865 2074 6162 7320 6772 6f75  of the tabs grou
+00005a80: 700a 2020 2020 2020 2020 2222 220a 2020  p.        """.  
+00005a90: 2020 2020 2020 725f 6861 7368 203d 2073        r_hash = s
+00005aa0: 656c 662e 5f67 6574 5f68 6173 685f 666f  elf._get_hash_fo
+00005ab0: 725f 636f 6e74 6169 6e65 7228 7461 6273  r_container(tabs
+00005ac0: 5f69 6e64 6578 5b30 5d29 0a20 2020 2020  _index[0]).     
+00005ad0: 2020 2074 6162 735f 6772 6f75 7020 3d20     tabs_group = 
+00005ae0: 6177 6169 7420 7365 6c66 2e5f 6170 702e  await self._app.
+00005af0: 6765 745f 7265 706f 7274 2872 5f68 6173  get_report(r_has
+00005b00: 683d 725f 6861 7368 290a 2020 2020 2020  h=r_hash).      
+00005b10: 2020 6966 206e 6f74 2074 6162 735f 6772    if not tabs_gr
+00005b20: 6f75 703a 0a20 2020 2020 2020 2020 2020  oup:.           
+00005b30: 2072 6574 7572 6e20 4e6f 6e65 0a20 2020   return None.   
+00005b40: 2020 2020 2072 6574 7572 6e20 7461 6273       return tabs
+00005b50: 5f67 726f 7570 2e63 6173 6361 6465 5f74  _group.cascade_t
+00005b60: 6f5f 6469 6374 2829 0a0a 2020 2020 6173  o_dict()..    as
+00005b70: 796e 6320 6465 6620 5f74 7279 5f74 6f5f  ync def _try_to_
+00005b80: 7265 7573 655f 6461 7461 280a 2020 2020  reuse_data(.    
+00005b90: 2020 2020 7365 6c66 2c20 6461 7461 5f73      self, data_s
+00005ba0: 6574 3a20 4461 7461 5365 742c 2064 6174  et: DataSet, dat
+00005bb0: 613a 2055 6e69 6f6e 5b6c 6973 742c 2070  a: Union[list, p
+00005bc0: 642e 4461 7461 4672 616d 655d 0a20 2020  d.DataFrame].   
+00005bd0: 2029 202d 3e20 6469 6374 5b73 7472 2c20   ) -> dict[str, 
+00005be0: 7475 706c 655b 4d61 7070 696e 672c 2044  tuple[Mapping, D
+00005bf0: 6174 6153 6574 2c20 6469 6374 5d5d 3a0a  ataSet, dict]]:.
+00005c00: 2020 2020 2020 2020 2222 2254 7279 2074          """Try t
+00005c10: 6f20 7265 7573 6520 7468 6520 6461 7461  o reuse the data
+00005c20: 2073 6574 2e0a 2020 2020 2020 2020 3a70   set..        :p
+00005c30: 6172 616d 2064 6174 615f 7365 743a 2074  aram data_set: t
+00005c40: 6865 2064 6174 6120 7365 740a 2020 2020  he data set.    
+00005c50: 2020 2020 3a70 6172 616d 2064 6174 613a      :param data:
+00005c60: 2074 6865 2064 6174 610a 2020 2020 2020   the data.      
+00005c70: 2020 2222 220a 2020 2020 2020 2020 6466    """.        df
+00005c80: 203d 2076 616c 6964 6174 655f 6461 7461   = validate_data
+00005c90: 5f69 735f 7061 6e64 6172 6162 6c65 2864  _is_pandarable(d
+00005ca0: 6174 6129 0a20 2020 2020 2020 2061 7578  ata).        aux
+00005cb0: 5f64 6174 615f 706f 696e 7420 3d20 6177  _data_point = aw
+00005cc0: 6169 7420 6461 7461 5f73 6574 2e67 6574  ait data_set.get
+00005cd0: 5f6f 6e65 5f64 6174 615f 706f 696e 7428  _one_data_point(
+00005ce0: 290a 2020 2020 2020 2020 6966 206e 6f74  ).        if not
+00005cf0: 2061 7578 5f64 6174 615f 706f 696e 743a   aux_data_point:
+00005d00: 0a20 2020 2020 2020 2020 2020 206c 6f67  .            log
+00005d10: 5f65 7272 6f72 280a 2020 2020 2020 2020  _error(.        
+00005d20: 2020 2020 2020 2020 6c6f 6767 6572 2c0a          logger,.
+00005d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005d40: 6622 4361 6e6e 6f74 2072 6575 7365 2064  f"Cannot reuse d
+00005d50: 6174 6120 7365 7420 7b73 7472 2864 6174  ata set {str(dat
+00005d60: 615f 7365 7429 7d20 6265 6361 7573 6520  a_set)} because 
+00005d70: 7468 6520 6461 7461 2073 6574 2069 7320  the data set is 
+00005d80: 656d 7074 7922 2c0a 2020 2020 2020 2020  empty",.        
+00005d90: 2020 2020 2020 2020 4461 7461 4572 726f          DataErro
+00005da0: 722c 0a20 2020 2020 2020 2020 2020 2029  r,.            )
+00005db0: 0a0a 2020 2020 2020 2020 6d61 7070 696e  ..        mappin
+00005dc0: 6773 203d 205b 636f 6c20 666f 7220 636f  gs = [col for co
+00005dd0: 6c20 696e 2061 7578 5f64 6174 615f 706f  l in aux_data_po
+00005de0: 696e 7420 6966 2061 7578 5f64 6174 615f  int if aux_data_
+00005df0: 706f 696e 745b 636f 6c5d 2069 7320 6e6f  point[col] is no
+00005e00: 7420 4e6f 6e65 5d0a 2020 2020 2020 2020  t None].        
+00005e10: 6466 2c20 736f 7274 203d 2061 6464 5f73  df, sort = add_s
+00005e20: 6f72 7469 6e67 5f74 6f5f 6466 2864 6629  orting_to_df(df)
+00005e30: 2069 6620 226f 7264 6572 4669 656c 6431   if "orderField1
+00005e40: 2220 696e 206d 6170 7069 6e67 7320 656c  " in mappings el
+00005e50: 7365 2028 6466 2c20 4e6f 6e65 290a 0a20  se (df, None).. 
+00005e60: 2020 2020 2020 2063 6f6e 7665 7274 6564         converted
+00005e70: 5f64 6174 615f 706f 696e 7473 203d 2063  _data_points = c
+00005e80: 6f6e 7665 7274 5f69 6e70 7574 5f64 6174  onvert_input_dat
+00005e90: 615f 746f 5f64 625f 6974 656d 7328 6466  a_to_db_items(df
+00005ea0: 2c20 736f 7274 3d73 6f72 7429 0a20 2020  , sort=sort).   
+00005eb0: 2020 2020 2066 6f72 206d 6170 7069 6e67       for mapping
+00005ec0: 2c20 7620 696e 2063 6f6e 7665 7274 6564  , v in converted
+00005ed0: 5f64 6174 615f 706f 696e 7473 5b30 5d2e  _data_points[0].
+00005ee0: 6974 656d 7328 293a 0a20 2020 2020 2020  items():.       
+00005ef0: 2020 2020 2069 6620 6d61 7070 696e 6720       if mapping 
+00005f00: 6e6f 7420 696e 206d 6170 7069 6e67 733a  not in mappings:
+00005f10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005f20: 206c 6f67 5f65 7272 6f72 280a 2020 2020   log_error(.    
+00005f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005f40: 6c6f 6767 6572 2c0a 2020 2020 2020 2020  logger,.        
+00005f50: 2020 2020 2020 2020 2020 2020 6622 4361              f"Ca
+00005f60: 6e6e 6f74 2072 6575 7365 2064 6174 6120  nnot reuse data 
+00005f70: 7365 7420 7b73 7472 2864 6174 615f 7365  set {str(data_se
+00005f80: 7429 7d20 6265 6361 7573 6520 7468 6520  t)} because the 
+00005f90: 6461 7461 2070 726f 7669 6465 6420 220a  data provided ".
+00005fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005fb0: 2020 2020 6622 6973 206e 6f74 2063 6f6e      f"is not con
+00005fc0: 7369 7374 656e 7420 7769 7468 2074 6865  sistent with the
+00005fd0: 2064 6174 6120 7365 7422 2c0a 2020 2020   data set",.    
+00005fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005ff0: 4461 7461 4572 726f 722c 0a20 2020 2020  DataError,.     
+00006000: 2020 2020 2020 2020 2020 2029 0a0a 2020             )..  
+00006010: 2020 2020 2020 6669 7273 745f 6466 5f69        first_df_i
+00006020: 7465 6d20 3d20 6466 2e69 6c6f 635b 305d  tem = df.iloc[0]
+00006030: 2e74 6f5f 6469 6374 2829 0a20 2020 2020  .to_dict().     
+00006040: 2020 2072 6574 7572 6e20 7b0a 2020 2020     return {.    
+00006050: 2020 2020 2020 2020 636f 6c3a 2028 6d61          col: (ma
+00006060: 7070 696e 672c 2064 6174 615f 7365 742c  pping, data_set,
+00006070: 2073 6f72 7429 0a20 2020 2020 2020 2020   sort).         
+00006080: 2020 2066 6f72 2063 6f6c 2c20 6d61 7070     for col, mapp
+00006090: 696e 6720 696e 207a 6970 280a 2020 2020  ing in zip(.    
+000060a0: 2020 2020 2020 2020 2020 2020 6669 7273              firs
+000060b0: 745f 6466 5f69 7465 6d2e 6b65 7973 2829  t_df_item.keys()
+000060c0: 2c20 636f 6e76 6572 7465 645f 6461 7461  , converted_data
+000060d0: 5f70 6f69 6e74 735b 305d 2e6b 6579 7328  _points[0].keys(
+000060e0: 290a 2020 2020 2020 2020 2020 2020 290a  ).            ).
+000060f0: 2020 2020 2020 2020 2020 2020 6966 2063              if c
+00006100: 6f6c 2021 3d20 2273 6f72 745f 7661 6c75  ol != "sort_valu
+00006110: 6573 220a 2020 2020 2020 2020 7d0a 0a20  es".        }.. 
+00006120: 2020 2061 7379 6e63 2064 6566 205f 6465     async def _de
+00006130: 6c65 7465 5f64 6174 615f 7365 745f 6966  lete_data_set_if
+00006140: 5f65 7869 7374 7328 7365 6c66 2c20 6461  _exists(self, da
+00006150: 7461 5f73 6574 5f6e 616d 653a 2073 7472  ta_set_name: str
+00006160: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
+00006170: 2020 2022 2222 4465 6c65 7465 2074 6865     """Delete the
+00006180: 2064 6174 6120 7365 7420 6966 2069 7420   data set if it 
+00006190: 6578 6973 7473 2e0a 2020 2020 2020 2020  exists..        
+000061a0: 3a70 6172 616d 2064 6174 615f 7365 745f  :param data_set_
+000061b0: 6e61 6d65 3a20 7468 6520 6e61 6d65 206f  name: the name o
+000061c0: 6620 7468 6520 6461 7461 2073 6574 0a20  f the data set. 
+000061d0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+000061e0: 2020 2069 6620 6177 6169 7420 7365 6c66     if await self
+000061f0: 2e5f 6170 702e 666f 7263 655f 6465 6c65  ._app.force_dele
+00006200: 7465 5f64 6174 615f 7365 7428 6e61 6d65  te_data_set(name
+00006210: 3d64 6174 615f 7365 745f 6e61 6d65 293a  =data_set_name):
+00006220: 0a20 2020 2020 2020 2020 2020 206c 6f67  .            log
+00006230: 6765 722e 696e 666f 2866 2244 656c 6574  ger.info(f"Delet
+00006240: 6564 2064 6174 6120 7365 7420 7769 7468  ed data set with
+00006250: 206e 616d 6520 7b64 6174 615f 7365 745f   name {data_set_
+00006260: 6e61 6d65 7d22 290a 0a20 2020 2061 7379  name}")..    asy
+00006270: 6e63 2064 6566 205f 6372 6561 7465 5f64  nc def _create_d
+00006280: 6174 615f 7365 745f 6672 6f6d 5f64 6628  ata_set_from_df(
+00006290: 0a20 2020 2020 2020 2073 656c 662c 2064  .        self, d
+000062a0: 6174 615f 7365 745f 6e61 6d65 3a20 7374  ata_set_name: st
+000062b0: 722c 2064 663a 2070 642e 4461 7461 4672  r, df: pd.DataFr
+000062c0: 616d 652c 2073 6f72 743a 204f 7074 696f  ame, sort: Optio
+000062d0: 6e61 6c5b 6469 6374 5d20 3d20 4e6f 6e65  nal[dict] = None
+000062e0: 0a20 2020 2029 202d 3e20 6469 6374 5b73  .    ) -> dict[s
+000062f0: 7472 2c20 7475 706c 655b 4d61 7070 696e  tr, tuple[Mappin
+00006300: 672c 2044 6174 6153 6574 2c20 6469 6374  g, DataSet, dict
+00006310: 5d5d 3a0a 2020 2020 2020 2020 2222 2247  ]]:.        """G
+00006320: 6574 2074 6865 2064 6174 6120 6d61 7070  et the data mapp
+00006330: 696e 6720 746f 2074 7570 6c65 2e0a 2020  ing to tuple..  
+00006340: 2020 2020 2020 3a70 6172 616d 2064 663a        :param df:
+00006350: 2074 6865 2064 6174 6120 6672 616d 650a   the data frame.
+00006360: 2020 2020 2020 2020 3a72 6574 7572 6e3a          :return:
+00006370: 2074 6865 2064 6174 6120 6d61 7070 696e   the data mappin
+00006380: 6720 746f 2074 7570 6c65 0a20 2020 2020  g to tuple.     
+00006390: 2020 2022 2222 0a20 2020 2020 2020 2064     """.        d
+000063a0: 662c 2073 6f72 7420 3d20 6164 645f 736f  f, sort = add_so
+000063b0: 7274 696e 675f 746f 5f64 6628 6466 2c20  rting_to_df(df, 
+000063c0: 736f 7274 290a 2020 2020 2020 2020 636f  sort).        co
+000063d0: 6c75 6d6e 7320 3d20 6466 2e63 6f6c 756d  lumns = df.colum
+000063e0: 6e73 2e74 6f6c 6973 7428 290a 2020 2020  ns.tolist().    
+000063f0: 2020 2020 6461 7461 5f6d 6170 7069 6e67      data_mapping
+00006400: 5f74 6f5f 7475 706c 6520 3d20 7b7d 0a20  _to_tuple = {}. 
+00006410: 2020 2020 2020 2028 6d61 7070 696e 672c         (mapping,
+00006420: 2064 6174 615f 7365 742c 2072 6573 5f73   data_set, res_s
+00006430: 6f72 7429 203d 2061 7761 6974 2073 656c  ort) = await sel
+00006440: 662e 5f61 7070 2e61 7070 656e 645f 6461  f._app.append_da
+00006450: 7461 5f74 6f5f 6461 7461 5f73 6574 280a  ta_to_data_set(.
+00006460: 2020 2020 2020 2020 2020 2020 6e61 6d65              name
+00006470: 3d64 6174 615f 7365 745f 6e61 6d65 2c20  =data_set_name, 
+00006480: 6461 7461 3d64 662c 2073 6f72 743d 736f  data=df, sort=so
+00006490: 7274 0a20 2020 2020 2020 2029 0a20 2020  rt.        ).   
+000064a0: 2020 2020 206c 6f67 6765 722e 696e 666f       logger.info
+000064b0: 280a 2020 2020 2020 2020 2020 2020 6627  (.            f'
+000064c0: 4372 6561 7465 6420 6461 7461 2073 6574  Created data set
+000064d0: 2077 6974 6820 6964 207b 6461 7461 5f73   with id {data_s
+000064e0: 6574 5b22 6964 225d 7d20 616e 6420 6e61  et["id"]} and na
+000064f0: 6d65 207b 6461 7461 5f73 6574 5f6e 616d  me {data_set_nam
+00006500: 657d 270a 2020 2020 2020 2020 290a 2020  e}'.        ).  
+00006510: 2020 2020 2020 666f 7220 636f 6c2c 206d        for col, m
+00006520: 6170 5f76 616c 2069 6e20 7a69 7028 636f  ap_val in zip(co
+00006530: 6c75 6d6e 732c 206d 6170 7069 6e67 293a  lumns, mapping):
+00006540: 0a20 2020 2020 2020 2020 2020 2064 6174  .            dat
+00006550: 615f 6d61 7070 696e 675f 746f 5f74 7570  a_mapping_to_tup
+00006560: 6c65 5b63 6f6c 5d20 3d20 286d 6170 5f76  le[col] = (map_v
+00006570: 616c 2c20 6461 7461 5f73 6574 2c20 7265  al, data_set, re
+00006580: 735f 736f 7274 290a 2020 2020 2020 2020  s_sort).        
+00006590: 7265 7475 726e 2064 6174 615f 6d61 7070  return data_mapp
+000065a0: 696e 675f 746f 5f74 7570 6c65 0a0a 2020  ing_to_tuple..  
+000065b0: 2020 6173 796e 6320 6465 6620 5f63 7265    async def _cre
+000065c0: 6174 655f 6475 6d70 6564 5f64 6174 615f  ate_dumped_data_
+000065d0: 7365 7428 0a20 2020 2020 2020 2073 656c  set(.        sel
+000065e0: 662c 2064 6174 615f 7365 745f 6e61 6d65  f, data_set_name
+000065f0: 3a20 7374 722c 2064 6174 613a 206c 6973  : str, data: lis
+00006600: 745b 6469 6374 5d0a 2020 2020 2920 2d3e  t[dict].    ) ->
+00006610: 2064 6963 743a 0a20 2020 2020 2020 2022   dict:.        "
+00006620: 2222 4765 7420 7468 6520 6d61 7070 696e  ""Get the mappin
+00006630: 6720 6672 6f6d 2061 2064 6963 742e 0a20  g from a dict.. 
+00006640: 2020 2020 2020 203a 7061 7261 6d20 6461         :param da
+00006650: 7461 3a20 7468 6520 6461 7461 0a20 2020  ta: the data.   
+00006660: 2020 2020 203a 7265 7475 726e 3a20 7468       :return: th
+00006670: 6520 6d61 7070 696e 6720 7475 706c 650a  e mapping tuple.
+00006680: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00006690: 2020 2020 6d61 7070 696e 672c 2064 6174      mapping, dat
+000066a0: 615f 7365 742c 2073 6f72 7420 3d20 6177  a_set, sort = aw
+000066b0: 6169 7420 7365 6c66 2e5f 6170 702e 6170  ait self._app.ap
+000066c0: 7065 6e64 5f64 6174 615f 746f 5f64 6174  pend_data_to_dat
+000066d0: 615f 7365 7428 0a20 2020 2020 2020 2020  a_set(.         
+000066e0: 2020 206e 616d 653d 6461 7461 5f73 6574     name=data_set
+000066f0: 5f6e 616d 652c 2064 6174 613d 6461 7461  _name, data=data
+00006700: 2c20 6475 6d70 5f77 686f 6c65 3d54 7275  , dump_whole=Tru
+00006710: 650a 2020 2020 2020 2020 290a 2020 2020  e.        ).    
+00006720: 2020 2020 6c6f 6767 6572 2e69 6e66 6f28      logger.info(
+00006730: 0a20 2020 2020 2020 2020 2020 2066 2743  .            f'C
+00006740: 7265 6174 6564 2064 6174 6120 7365 7420  reated data set 
+00006750: 7769 7468 2069 6420 7b64 6174 615f 7365  with id {data_se
+00006760: 745b 2269 6422 5d7d 2061 6e64 206e 616d  t["id"]} and nam
+00006770: 6520 7b64 6174 615f 7365 745f 6e61 6d65  e {data_set_name
+00006780: 7d27 0a20 2020 2020 2020 2029 0a20 2020  }'.        ).   
+00006790: 2020 2020 2061 7373 6572 7420 6d61 7070       assert mapp
+000067a0: 696e 675b 305d 203d 3d20 2263 7573 746f  ing[0] == "custo
+000067b0: 6d46 6965 6c64 3122 0a20 2020 2020 2020  mField1".       
+000067c0: 2072 6574 7572 6e20 7b22 6461 7461 223a   return {"data":
+000067d0: 2028 2263 7573 746f 6d46 6965 6c64 3122   ("customField1"
+000067e0: 2c20 6461 7461 5f73 6574 2c20 736f 7274  , data_set, sort
+000067f0: 297d 0a0a 2020 2020 6173 796e 6320 6465  )}..    async de
+00006800: 6620 5f63 7265 6174 655f 6461 7461 5f73  f _create_data_s
+00006810: 6574 280a 2020 2020 2020 2020 7365 6c66  et(.        self
+00006820: 2c0a 2020 2020 2020 2020 6e61 6d65 3a20  ,.        name: 
+00006830: 7374 722c 0a20 2020 2020 2020 2064 6174  str,.        dat
+00006840: 613a 2055 6e69 6f6e 5b6c 6973 745b 6469  a: Union[list[di
+00006850: 6374 5d2c 2070 642e 4461 7461 4672 616d  ct], pd.DataFram
+00006860: 652c 2064 6963 742c 2073 7472 5d2c 0a20  e, dict, str],. 
+00006870: 2020 2020 2020 2064 756d 705f 7768 6f6c         dump_whol
+00006880: 653a 2062 6f6f 6c20 3d20 4661 6c73 652c  e: bool = False,
+00006890: 0a20 2020 2029 202d 3e20 6469 6374 5b73  .    ) -> dict[s
+000068a0: 7472 2c20 7475 706c 655b 4d61 7070 696e  tr, tuple[Mappin
+000068b0: 672c 2044 6174 6153 6574 2c20 6469 6374  g, DataSet, dict
+000068c0: 5d5d 3a0a 2020 2020 2020 2020 2222 2253  ]]:.        """S
+000068d0: 6574 2061 2073 6861 7265 6420 6461 7461  et a shared data
+000068e0: 2065 6e74 7279 2e0a 2020 2020 2020 2020   entry..        
+000068f0: 3a70 6172 616d 206e 616d 653a 2074 6865  :param name: the
+00006900: 206b 6579 206f 6620 7468 6520 7368 6172   key of the shar
+00006910: 6564 2064 6174 6120 656e 7472 790a 2020  ed data entry.  
+00006920: 2020 2020 2020 3a70 6172 616d 2064 6174        :param dat
+00006930: 613a 2074 6865 2076 616c 7565 206f 6620  a: the value of 
+00006940: 7468 6520 7368 6172 6564 2064 6174 6120  the shared data 
+00006950: 656e 7472 790a 2020 2020 2020 2020 3a70  entry.        :p
+00006960: 6172 616d 2064 756d 705f 7768 6f6c 653a  aram dump_whole:
+00006970: 2077 6865 7468 6572 2074 6f20 6475 6d70   whether to dump
+00006980: 2074 6865 2077 686f 6c65 2064 6174 6120   the whole data 
+00006990: 7365 740a 2020 2020 2020 2020 2222 220a  set.        """.
+000069a0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+000069b0: 7265 7573 655f 6461 7461 5f73 6574 733a  reuse_data_sets:
+000069c0: 0a20 2020 2020 2020 2020 2020 2064 6174  .            dat
+000069d0: 615f 7365 7420 3d20 6177 6169 7420 7365  a_set = await se
+000069e0: 6c66 2e5f 6170 702e 6765 745f 6461 7461  lf._app.get_data
+000069f0: 5f73 6574 280a 2020 2020 2020 2020 2020  _set(.          
+00006a00: 2020 2020 2020 6e61 6d65 3d6e 616d 652c        name=name,
+00006a10: 2063 7265 6174 655f 6966 5f6e 6f74 5f65   create_if_not_e
+00006a20: 7869 7374 733d 4661 6c73 650a 2020 2020  xists=False.    
+00006a30: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+00006a40: 2020 2020 2020 6966 2064 6174 615f 7365        if data_se
+00006a50: 743a 0a20 2020 2020 2020 2020 2020 2020  t:.             
+00006a60: 2020 2072 6574 7572 6e20 280a 2020 2020     return (.    
+00006a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006a80: 6177 6169 7420 7365 6c66 2e5f 7472 795f  await self._try_
+00006a90: 746f 5f72 6575 7365 5f64 6174 6128 6461  to_reuse_data(da
+00006aa0: 7461 5f73 6574 2c20 6461 7461 290a 2020  ta_set, data).  
+00006ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006ac0: 2020 6966 206e 6f74 2064 756d 705f 7768    if not dump_wh
+00006ad0: 6f6c 650a 2020 2020 2020 2020 2020 2020  ole.            
+00006ae0: 2020 2020 2020 2020 656c 7365 207b 2264          else {"d
+00006af0: 6174 6122 3a20 2822 6375 7374 6f6d 4669  ata": ("customFi
+00006b00: 656c 6431 222c 2064 6174 615f 7365 742c  eld1", data_set,
+00006b10: 207b 7d29 7d0a 2020 2020 2020 2020 2020   {})}.          
+00006b20: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
+00006b30: 2061 7761 6974 2073 656c 662e 5f64 656c   await self._del
+00006b40: 6574 655f 6461 7461 5f73 6574 5f69 665f  ete_data_set_if_
+00006b50: 6578 6973 7473 2864 6174 615f 7365 745f  exists(data_set_
+00006b60: 6e61 6d65 3d6e 616d 6529 0a0a 2020 2020  name=name)..    
+00006b70: 2020 2020 6966 2064 756d 705f 7768 6f6c      if dump_whol
+00006b80: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+00006b90: 6574 7572 6e20 6177 6169 7420 7365 6c66  eturn await self
+00006ba0: 2e5f 6372 6561 7465 5f64 756d 7065 645f  ._create_dumped_
+00006bb0: 6461 7461 5f73 6574 286e 616d 652c 2064  data_set(name, d
+00006bc0: 6174 6129 0a0a 2020 2020 2020 2020 7265  ata)..        re
+00006bd0: 7475 726e 2061 7761 6974 2073 656c 662e  turn await self.
+00006be0: 5f63 7265 6174 655f 6461 7461 5f73 6574  _create_data_set
+00006bf0: 5f66 726f 6d5f 6466 286e 616d 652c 2044  _from_df(name, D
+00006c00: 6174 6146 7261 6d65 2864 6174 6129 290a  ataFrame(data)).
+00006c10: 0a20 2020 2061 7379 6e63 2064 6566 205f  .    async def _
+00006c20: 7365 745f 7368 6172 6564 5f64 6174 615f  set_shared_data_
+00006c30: 656e 7472 7928 0a20 2020 2020 2020 2073  entry(.        s
+00006c40: 656c 662c 0a20 2020 2020 2020 206e 616d  elf,.        nam
+00006c50: 653a 2073 7472 2c0a 2020 2020 2020 2020  e: str,.        
+00006c60: 6461 7461 3a20 556e 696f 6e5b 6c69 7374  data: Union[list
+00006c70: 5b64 6963 745d 2c20 7064 2e44 6174 6146  [dict], pd.DataF
+00006c80: 7261 6d65 2c20 6469 6374 2c20 7374 725d  rame, dict, str]
+00006c90: 2c0a 2020 2020 2020 2020 6475 6d70 5f77  ,.        dump_w
+00006ca0: 686f 6c65 3a20 626f 6f6c 203d 2046 616c  hole: bool = Fal
+00006cb0: 7365 2c0a 2020 2020 293a 0a20 2020 2020  se,.    ):.     
+00006cc0: 2020 2022 2222 0a20 2020 2020 2020 2053     """.        S
+00006cd0: 6574 2061 2073 6861 7265 6420 6461 7461  et a shared data
+00006ce0: 2065 6e74 7279 2e0a 2020 2020 2020 2020   entry..        
+00006cf0: 3a70 6172 616d 206e 616d 653a 2074 6865  :param name: the
+00006d00: 206b 6579 206f 6620 7468 6520 7368 6172   key of the shar
+00006d10: 6564 2064 6174 6120 656e 7472 790a 2020  ed data entry.  
+00006d20: 2020 2020 2020 3a70 6172 616d 2064 6174        :param dat
+00006d30: 613a 2074 6865 2076 616c 7565 206f 6620  a: the value of 
+00006d40: 7468 6520 7368 6172 6564 2064 6174 6120  the shared data 
+00006d50: 656e 7472 790a 2020 2020 2020 2020 3a70  entry.        :p
+00006d60: 6172 616d 2064 756d 705f 7768 6f6c 653a  aram dump_whole:
+00006d70: 2077 6865 7468 6572 2074 6f20 6475 6d70   whether to dump
+00006d80: 2074 6865 2077 686f 6c65 2064 6174 6120   the whole data 
+00006d90: 7365 740a 2020 2020 2020 2020 2222 220a  set.        """.
+00006da0: 2020 2020 2020 2020 6966 206e 616d 6520          if name 
+00006db0: 696e 2073 656c 662e 5f73 6861 7265 645f  in self._shared_
+00006dc0: 6461 7461 5f6d 6170 3a0a 2020 2020 2020  data_map:.      
+00006dd0: 2020 2020 2020 6c6f 675f 6572 726f 7228        log_error(
+00006de0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006df0: 206c 6f67 6765 722c 0a20 2020 2020 2020   logger,.       
+00006e00: 2020 2020 2020 2020 2066 2243 616e 6e6f           f"Canno
+00006e10: 7420 7365 7420 7368 6172 6564 2064 6174  t set shared dat
+00006e20: 6120 656e 7472 7920 7b6e 616d 657d 2062  a entry {name} b
+00006e30: 6563 6175 7365 2069 7420 616c 7265 6164  ecause it alread
+00006e40: 7920 6578 6973 7473 222c 0a20 2020 2020  y exists",.     
+00006e50: 2020 2020 2020 2020 2020 2044 6174 6145             DataE
+00006e60: 7272 6f72 2c0a 2020 2020 2020 2020 2020  rror,.          
+00006e70: 2020 290a 0a20 2020 2020 2020 2073 656c    )..        sel
+00006e80: 662e 5f73 6861 7265 645f 6461 7461 5f6d  f._shared_data_m
+00006e90: 6170 5b6e 616d 655d 203d 2061 7761 6974  ap[name] = await
+00006ea0: 2073 656c 662e 5f63 7265 6174 655f 6461   self._create_da
+00006eb0: 7461 5f73 6574 280a 2020 2020 2020 2020  ta_set(.        
+00006ec0: 2020 2020 6e61 6d65 2c20 6461 7461 2c20      name, data, 
+00006ed0: 6475 6d70 5f77 686f 6c65 0a20 2020 2020  dump_whole.     
+00006ee0: 2020 2029 0a20 2020 2020 2020 2073 656c     ).        sel
+00006ef0: 662e 5f73 6861 7265 645f 6461 7461 5b6e  f._shared_data[n
+00006f00: 616d 655d 203d 2064 6174 610a 0a20 2020  ame] = data..   
+00006f10: 2061 7379 6e63 2064 6566 2073 6574 5f73   async def set_s
+00006f20: 6861 7265 645f 6461 7461 280a 2020 2020  hared_data(.    
+00006f30: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
+00006f40: 2020 6466 733a 2064 6963 745b 7374 722c    dfs: dict[str,
+00006f50: 2055 6e69 6f6e 5b6c 6973 745b 6469 6374   Union[list[dict
+00006f60: 5d2c 2070 642e 4461 7461 4672 616d 655d  ], pd.DataFrame]
+00006f70: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
+00006f80: 2020 6375 7374 6f6d 5f64 6174 613a 2064    custom_data: d
+00006f90: 6963 745b 7374 722c 2061 6e79 5d20 3d20  ict[str, any] = 
+00006fa0: 4e6f 6e65 2c0a 2020 2020 293a 0a20 2020  None,.    ):.   
+00006fb0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00006fc0: 2053 6574 2073 6861 7265 6420 6461 7461   Set shared data
+00006fd0: 2066 6f72 2074 6865 2073 2e70 6c74 2074   for the s.plt t
+00006fe0: 6f20 7573 652e 0a20 2020 2020 2020 203a  o use..        :
+00006ff0: 7061 7261 6d20 6466 733a 2074 6865 2064  param dfs: the d
+00007000: 6174 6120 6672 616d 6573 0a20 2020 2020  ata frames.     
+00007010: 2020 203a 7061 7261 6d20 6375 7374 6f6d     :param custom
+00007020: 5f64 6174 613a 2074 6865 2063 7573 746f  _data: the custo
+00007030: 6d20 6461 7461 0a20 2020 2020 2020 2022  m data.        "
+00007040: 2222 0a20 2020 2020 2020 2074 6173 6b73  "".        tasks
+00007050: 203d 205b 5d0a 2020 2020 2020 2020 666f   = [].        fo
+00007060: 7220 6b2c 2064 6620 696e 2028 6466 7320  r k, df in (dfs 
+00007070: 6966 2064 6673 2065 6c73 6520 7b7d 292e  if dfs else {}).
+00007080: 6974 656d 7328 293a 0a20 2020 2020 2020  items():.       
+00007090: 2020 2020 2074 6173 6b73 2e61 7070 656e       tasks.appen
+000070a0: 6428 7365 6c66 2e5f 7365 745f 7368 6172  d(self._set_shar
+000070b0: 6564 5f64 6174 615f 656e 7472 7928 6b2c  ed_data_entry(k,
+000070c0: 2064 6629 290a 2020 2020 2020 2020 666f   df)).        fo
+000070d0: 7220 6b2c 2076 2069 6e20 2863 7573 746f  r k, v in (custo
+000070e0: 6d5f 6461 7461 2069 6620 6375 7374 6f6d  m_data if custom
+000070f0: 5f64 6174 6120 656c 7365 207b 7d29 2e69  _data else {}).i
+00007100: 7465 6d73 2829 3a0a 2020 2020 2020 2020  tems():.        
+00007110: 2020 2020 7461 736b 732e 6170 7065 6e64      tasks.append
+00007120: 2873 656c 662e 5f73 6574 5f73 6861 7265  (self._set_share
+00007130: 645f 6461 7461 5f65 6e74 7279 286b 2c20  d_data_entry(k, 
+00007140: 762c 2064 756d 705f 7768 6f6c 653d 5472  v, dump_whole=Tr
+00007150: 7565 2929 0a20 2020 2020 2020 2069 6620  ue)).        if 
+00007160: 7461 736b 733a 0a20 2020 2020 2020 2020  tasks:.         
+00007170: 2020 2061 7761 6974 2061 7379 6e63 696f     await asyncio
+00007180: 2e67 6174 6865 7228 2a74 6173 6b73 290a  .gather(*tasks).
+00007190: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+000071a0: 2020 2020 2020 2020 2020 6c6f 675f 6572            log_er
+000071b0: 726f 7228 6c6f 6767 6572 2c20 224e 6f20  ror(logger, "No 
+000071c0: 6461 7461 2070 726f 7669 6465 6422 2c20  data provided", 
+000071d0: 4461 7461 4572 726f 7229 0a0a 2020 2020  DataError)..    
+000071e0: 6173 796e 6320 6465 6620 5f63 686f 6f73  async def _choos
+000071f0: 655f 6461 7461 280a 2020 2020 2020 2020  e_data(.        
+00007200: 7365 6c66 2c0a 2020 2020 2020 2020 6f72  self,.        or
+00007210: 6465 723a 2069 6e74 2c0a 2020 2020 2020  der: int,.      
+00007220: 2020 6461 7461 3a20 556e 696f 6e5b 6c69    data: Union[li
+00007230: 7374 5b64 6963 745d 2c20 7064 2e44 6174  st[dict], pd.Dat
+00007240: 6146 7261 6d65 2c20 6469 6374 2c20 7374  aFrame, dict, st
+00007250: 725d 2c0a 2020 2020 2020 2020 6368 6172  r],.        char
+00007260: 745f 636c 6173 733a 2074 7970 655b 5265  t_class: type[Re
+00007270: 706f 7274 5d20 3d20 4543 6861 7274 2c0a  port] = EChart,.
+00007280: 2020 2020 2020 2020 6475 6d70 5f77 686f          dump_who
+00007290: 6c65 3a20 626f 6f6c 203d 2046 616c 7365  le: bool = False
+000072a0: 2c0a 2020 2020 2920 2d3e 2064 6963 745b  ,.    ) -> dict[
+000072b0: 7374 722c 2074 7570 6c65 5b4d 6170 7069  str, tuple[Mappi
+000072c0: 6e67 2c20 4461 7461 5365 742c 2064 6963  ng, DataSet, dic
+000072d0: 745d 5d3a 0a20 2020 2020 2020 2022 2222  t]]:.        """
+000072e0: 4765 7420 7468 6520 6461 7461 206d 6170  Get the data map
+000072f0: 7069 6e67 7320 6f66 2074 6865 2064 6174  pings of the dat
+00007300: 612e 2049 6620 7468 6520 6461 7461 2069  a. If the data i
+00007310: 7320 6120 7374 7269 6e67 2c20 6974 2069  s a string, it i
+00007320: 7320 6173 7375 6d65 6420 746f 2062 6520  s assumed to be 
+00007330: 6120 7368 6172 6564 2064 6174 6120 656e  a shared data en
+00007340: 7472 792e 0a20 2020 2020 2020 203a 7061  try..        :pa
+00007350: 7261 6d20 6f72 6465 723a 2074 6865 206f  ram order: the o
+00007360: 7264 6572 206f 6620 7468 6520 6368 6172  rder of the char
+00007370: 740a 2020 2020 2020 2020 3a70 6172 616d  t.        :param
+00007380: 2064 6174 613a 2074 6865 2064 6174 610a   data: the data.
+00007390: 2020 2020 2020 2020 3a70 6172 616d 2064          :param d
+000073a0: 756d 705f 7768 6f6c 653a 2077 6865 7468  ump_whole: wheth
+000073b0: 6572 2074 6f20 6475 6d70 2074 6865 2077  er to dump the w
+000073c0: 686f 6c65 2064 6174 6120 7365 740a 2020  hole data set.  
+000073d0: 2020 2020 2020 3a72 6574 7572 6e3a 2074        :return: t
+000073e0: 6865 2064 6174 6120 6d61 7070 696e 6773  he data mappings
+000073f0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00007400: 2020 2020 2069 6620 6973 696e 7374 616e       if isinstan
+00007410: 6365 2864 6174 612c 2073 7472 293a 0a20  ce(data, str):. 
+00007420: 2020 2020 2020 2020 2020 2069 6620 6461             if da
+00007430: 7461 206e 6f74 2069 6e20 7365 6c66 2e5f  ta not in self._
+00007440: 7368 6172 6564 5f64 6174 615f 6d61 703a  shared_data_map:
+00007450: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007460: 206c 6f67 5f65 7272 6f72 286c 6f67 6765   log_error(logge
+00007470: 722c 2066 224e 6f20 7368 6172 6564 2064  r, f"No shared d
+00007480: 6174 6120 7769 7468 206e 616d 6520 7b64  ata with name {d
+00007490: 6174 617d 2066 6f75 6e64 222c 2044 6174  ata} found", Dat
+000074a0: 6145 7272 6f72 290a 2020 2020 2020 2020  aError).        
+000074b0: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+000074c0: 5f73 6861 7265 645f 6461 7461 5f6d 6170  _shared_data_map
+000074d0: 5b64 6174 615d 0a0a 2020 2020 2020 2020  [data]..        
+000074e0: 5f2c 2072 6570 6f72 7420 3d20 6177 6169  _, report = awai
+000074f0: 7420 7365 6c66 2e5f 6765 745f 6368 6172  t self._get_char
+00007500: 745f 7265 706f 7274 286f 7264 6572 2c20  t_report(order, 
+00007510: 6368 6172 745f 636c 6173 7329 0a20 2020  chart_class).   
+00007520: 2020 2020 206e 616d 6520 3d20 7265 706f       name = repo
+00007530: 7274 5b22 6964 225d 0a0a 2020 2020 2020  rt["id"]..      
+00007540: 2020 7265 7475 726e 2061 7761 6974 2073    return await s
+00007550: 656c 662e 5f63 7265 6174 655f 6461 7461  elf._create_data
+00007560: 5f73 6574 286e 616d 652c 2064 6174 612c  _set(name, data,
+00007570: 2064 756d 705f 7768 6f6c 6529 0a0a 2020   dump_whole)..  
+00007580: 2020 6173 796e 6320 6465 6620 5f63 6865    async def _che
+00007590: 636b 5f70 7265 7669 6f75 735f 7061 7468  ck_previous_path
+000075a0: 7328 7365 6c66 293a 0a20 2020 2020 2020  s(self):.       
+000075b0: 2022 2222 4368 6563 6b20 6966 2074 6865   """Check if the
+000075c0: 7265 2061 7265 2070 6174 6873 2074 6861  re are paths tha
+000075d0: 7420 6861 7665 206e 6f74 2062 6565 6e20  t have not been 
+000075e0: 6578 6563 7574 6564 2079 6574 2e22 2222  executed yet."""
+000075f0: 0a20 2020 2020 2020 2070 6174 6873 5f69  .        paths_i
+00007600: 6e5f 6f72 6465 7220 3d20 6177 6169 7420  n_order = await 
+00007610: 7365 6c66 2e5f 6170 702e 6765 745f 7061  self._app.get_pa
+00007620: 7468 735f 696e 5f6f 7264 6572 2829 0a20  ths_in_order(). 
+00007630: 2020 2020 2020 206e 6f74 5f65 7865 6375         not_execu
+00007640: 7465 645f 7061 7468 7320 3d20 5b0a 2020  ted_paths = [.  
+00007650: 2020 2020 2020 2020 2020 7020 666f 7220            p for 
+00007660: 7020 696e 2070 6174 6873 5f69 6e5f 6f72  p in paths_in_or
+00007670: 6465 7220 6966 2070 206e 6f74 2069 6e20  der if p not in 
+00007680: 7365 6c66 2e5f 6578 6563 7574 696f 6e5f  self._execution_
+00007690: 7061 7468 5f6f 7264 6572 730a 2020 2020  path_orders.    
+000076a0: 2020 2020 5d0a 2020 2020 2020 2020 6966      ].        if
+000076b0: 206c 656e 286e 6f74 5f65 7865 6375 7465   len(not_execute
+000076c0: 645f 7061 7468 7329 203e 2030 3a0a 2020  d_paths) > 0:.  
+000076d0: 2020 2020 2020 2020 2020 6e6f 745f 7570            not_up
+000076e0: 6c6f 6164 6564 5f70 6174 6873 203d 205b  loaded_paths = [
+000076f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007700: 2070 2066 6f72 2070 2069 6e20 7365 6c66   p for p in self
+00007710: 2e5f 6578 6563 7574 696f 6e5f 7061 7468  ._execution_path
+00007720: 5f6f 7264 6572 7320 6966 2070 206e 6f74  _orders if p not
+00007730: 2069 6e20 7061 7468 735f 696e 5f6f 7264   in paths_in_ord
+00007740: 6572 0a20 2020 2020 2020 2020 2020 205d  er.            ]
+00007750: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00007760: 662e 5f65 7865 6375 7469 6f6e 5f70 6174  f._execution_pat
+00007770: 685f 6f72 6465 7273 2e63 6c65 6172 2829  h_orders.clear()
+00007780: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
+00007790: 2070 2069 6e20 7061 7468 735f 696e 5f6f   p in paths_in_o
+000077a0: 7264 6572 202b 206e 6f74 5f75 706c 6f61  rder + not_uploa
+000077b0: 6465 645f 7061 7468 733a 0a20 2020 2020  ded_paths:.     
+000077c0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000077d0: 5f65 7865 6375 7469 6f6e 5f70 6174 685f  _execution_path_
+000077e0: 6f72 6465 7273 2e61 7070 656e 6428 7029  orders.append(p)
+000077f0: 0a0a 2020 2020 6173 796e 6320 6465 6620  ..    async def 
+00007800: 5f63 7265 6174 655f 6368 6172 7428 0a20  _create_chart(. 
+00007810: 2020 2020 2020 2073 656c 662c 2063 6861         self, cha
+00007820: 7274 5f63 6c61 7373 3a20 7479 7065 5b52  rt_class: type[R
+00007830: 6570 6f72 745d 2c20 6f72 6465 723a 2069  eport], order: i
+00007840: 6e74 2c20 2a2a 7061 7261 6d73 0a20 2020  nt, **params.   
+00007850: 2029 202d 3e20 5265 706f 7274 3a0a 2020   ) -> Report:.  
+00007860: 2020 2020 2020 2222 2243 7265 6174 6520        """Create 
+00007870: 6120 6368 6172 7420 616e 6420 6164 6420  a chart and add 
+00007880: 6974 2074 6f20 7468 6520 6375 7272 656e  it to the curren
+00007890: 7420 7461 6273 2067 726f 7570 206f 7220  t tabs group or 
+000078a0: 6d6f 6461 6c2e 0a20 2020 2020 2020 203a  modal..        :
+000078b0: 7061 7261 6d20 6368 6172 745f 636c 6173  param chart_clas
+000078c0: 733a 2074 6865 2063 6c61 7373 206f 6620  s: the class of 
+000078d0: 7468 6520 6368 6172 740a 2020 2020 2020  the chart.      
+000078e0: 2020 3a70 6172 616d 206f 7264 6572 3a20    :param order: 
+000078f0: 7468 6520 6f72 6465 7220 6f66 2074 6865  the order of the
+00007900: 2063 6861 7274 2069 6e20 7468 6520 6461   chart in the da
+00007910: 7368 626f 6172 640a 2020 2020 2020 2020  shboard.        
+00007920: 3a70 6172 616d 2070 6172 616d 733a 2074  :param params: t
+00007930: 6865 2061 7267 756d 656e 7473 206f 6620  he arguments of 
+00007940: 7468 6520 6368 6172 740a 2020 2020 2020  the chart.      
+00007950: 2020 2222 220a 2020 2020 2020 2020 6966    """.        if
+00007960: 2022 6c6f 6767 696e 675f 6675 6e63 5f6e   "logging_func_n
+00007970: 616d 6522 2069 6e20 7061 7261 6d73 3a0a  ame" in params:.
+00007980: 2020 2020 2020 2020 2020 2020 6465 6c20              del 
+00007990: 7061 7261 6d73 5b22 6c6f 6767 696e 675f  params["logging_
+000079a0: 6675 6e63 5f6e 616d 6522 5d0a 0a20 2020  func_name"]..   
+000079b0: 2020 2020 2069 6620 6e6f 7420 7061 7261       if not para
+000079c0: 6d73 2e67 6574 2822 7469 746c 6522 293a  ms.get("title"):
+000079d0: 0a20 2020 2020 2020 2020 2020 2070 6172  .            par
+000079e0: 616d 735b 2274 6974 6c65 225d 203d 2022  ams["title"] = "
+000079f0: 220a 2020 2020 2020 2020 6966 206e 6f74  ".        if not
+00007a00: 2070 6172 616d 732e 6765 7428 2273 697a   params.get("siz
+00007a10: 6552 6f77 7322 293a 0a20 2020 2020 2020  eRows"):.       
+00007a20: 2020 2020 2070 6172 616d 735b 2273 697a       params["siz
+00007a30: 6552 6f77 7322 5d20 3d20 330a 2020 2020  eRows"] = 3.    
+00007a40: 2020 2020 6966 206e 6f74 2070 6172 616d      if not param
+00007a50: 732e 6765 7428 2273 697a 6543 6f6c 756d  s.get("sizeColum
+00007a60: 6e73 2229 3a0a 2020 2020 2020 2020 2020  ns"):.          
+00007a70: 2020 7061 7261 6d73 5b22 7369 7a65 436f    params["sizeCo
+00007a80: 6c75 6d6e 7322 5d20 3d20 3132 0a20 2020  lumns"] = 12.   
+00007a90: 2020 2020 2069 6620 6e6f 7420 7061 7261       if not para
+00007aa0: 6d73 2e67 6574 2822 7369 7a65 5061 6464  ms.get("sizePadd
+00007ab0: 696e 6722 293a 0a20 2020 2020 2020 2020  ing"):.         
+00007ac0: 2020 2070 6172 616d 735b 2273 697a 6550     params["sizeP
+00007ad0: 6164 6469 6e67 225d 203d 2022 302c 302c  adding"] = "0,0,
+00007ae0: 302c 3022 0a0a 2020 2020 2020 2020 7061  0,0"..        pa
+00007af0: 7261 6d73 5b22 6265 6e74 6f62 6f78 225d  rams["bentobox"]
+00007b00: 203d 2073 656c 662e 5f67 6574 5f62 656e   = self._get_ben
+00007b10: 746f 626f 785f 6461 7461 286f 7264 6572  tobox_data(order
+00007b20: 3d6f 7264 6572 290a 2020 2020 2020 2020  =order).        
+00007b30: 7061 7261 6d73 5b22 7061 7468 225d 203d  params["path"] =
+00007b40: 2073 656c 662e 5f63 7572 7265 6e74 5f70   self._current_p
+00007b50: 6174 680a 0a20 2020 2020 2020 2069 6620  ath..        if 
+00007b60: 6861 7361 7474 7228 7365 6c66 2c20 2263  hasattr(self, "c
+00007b70: 6f64 655f 6765 6e65 7261 7469 6f6e 5f6d  ode_generation_m
+00007b80: 6574 6164 6174 6122 293a 0a20 2020 2020  etadata"):.     
+00007b90: 2020 2020 2020 2069 6620 2270 726f 7065         if "prope
+00007ba0: 7274 6965 7322 206e 6f74 2069 6e20 7061  rties" not in pa
+00007bb0: 7261 6d73 3a0a 2020 2020 2020 2020 2020  rams:.          
+00007bc0: 2020 2020 2020 7061 7261 6d73 5b22 7072        params["pr
+00007bd0: 6f70 6572 7469 6573 225d 203d 207b 7d0a  operties"] = {}.
+00007be0: 2020 2020 2020 2020 2020 2020 7061 7261              para
+00007bf0: 6d73 5b22 7072 6f70 6572 7469 6573 225d  ms["properties"]
+00007c00: 5b22 636f 6465 5f67 656e 6572 6174 696f  ["code_generatio
+00007c10: 6e5f 6d65 7461 6461 7461 225d 203d 2067  n_metadata"] = g
+00007c20: 6574 6174 7472 280a 2020 2020 2020 2020  etattr(.        
+00007c30: 2020 2020 2020 2020 7365 6c66 2c20 2263          self, "c
+00007c40: 6f64 655f 6765 6e65 7261 7469 6f6e 5f6d  ode_generation_m
+00007c50: 6574 6164 6174 6122 0a20 2020 2020 2020  etadata".       
+00007c60: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
+00007c70: 6576 656e 745f 7479 7065 3a20 4576 656e  event_type: Even
+00007c80: 7454 7970 6520 3d20 4576 656e 7454 7970  tType = EventTyp
+00007c90: 652e 5245 504f 5254 5f55 5044 4154 4544  e.REPORT_UPDATED
+00007ca0: 0a20 2020 2020 2020 2072 5f68 6173 682c  .        r_hash,
+00007cb0: 2063 6861 7274 203d 2061 7761 6974 2073   chart = await s
+00007cc0: 656c 662e 5f67 6574 5f63 6861 7274 5f72  elf._get_chart_r
+00007cd0: 6570 6f72 7428 0a20 2020 2020 2020 2020  eport(.         
+00007ce0: 2020 206f 7264 6572 2c20 6368 6172 745f     order, chart_
+00007cf0: 636c 6173 732c 2063 7265 6174 655f 6966  class, create_if
+00007d00: 5f6e 6f74 5f65 7869 7374 733d 4661 6c73  _not_exists=Fals
+00007d10: 650a 2020 2020 2020 2020 290a 2020 2020  e.        ).    
+00007d20: 2020 2020 6966 2063 6861 7274 3a0a 2020      if chart:.  
+00007d30: 2020 2020 2020 2020 2020 7061 7261 6d73            params
+00007d40: 5b22 7061 7468 4f72 6465 7222 5d20 3d20  ["pathOrder"] = 
+00007d50: 6368 6172 745b 2270 6174 684f 7264 6572  chart["pathOrder
+00007d60: 225d 0a20 2020 2020 2020 2020 2020 2069  "].            i
+00007d70: 6620 7365 6c66 2e5f 6375 7272 656e 745f  f self._current_
+00007d80: 7061 7468 2061 6e64 2070 6172 616d 735b  path and params[
+00007d90: 2270 6174 684f 7264 6572 225d 2069 7320  "pathOrder"] is 
+00007da0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00007db0: 2020 2020 2020 6177 6169 7420 7365 6c66        await self
+00007dc0: 2e5f 6368 6563 6b5f 7072 6576 696f 7573  ._check_previous
+00007dd0: 5f70 6174 6873 2829 0a20 2020 2020 2020  _paths().       
+00007de0: 2020 2020 2020 2020 2070 6172 616d 735b           params[
+00007df0: 2270 6174 684f 7264 6572 225d 203d 2073  "pathOrder"] = s
+00007e00: 656c 662e 5f65 7865 6375 7469 6f6e 5f70  elf._execution_p
+00007e10: 6174 685f 6f72 6465 7273 2e69 6e64 6578  ath_orders.index
+00007e20: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00007e30: 2020 2020 2020 7365 6c66 2e5f 6375 7272        self._curr
+00007e40: 656e 745f 7061 7468 0a20 2020 2020 2020  ent_path.       
+00007e50: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+00007e60: 2020 2020 2020 2069 6620 6368 6172 7420         if chart 
+00007e70: 213d 2073 656c 662e 5f61 7070 2e6d 6f63  != self._app.moc
+00007e80: 6b5f 6372 6561 7465 5f72 6570 6f72 7428  k_create_report(
+00007e90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007ea0: 2063 6861 7274 5f63 6c61 7373 2c20 725f   chart_class, r_
+00007eb0: 6861 7368 3d72 5f68 6173 682c 206f 7264  hash=r_hash, ord
+00007ec0: 6572 3d6f 7264 6572 2c20 2a2a 7061 7261  er=order, **para
+00007ed0: 6d73 0a20 2020 2020 2020 2020 2020 2029  ms.            )
+00007ee0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00007ef0: 2020 6177 6169 7420 7365 6c66 2e5f 6170    await self._ap
+00007f00: 702e 7570 6461 7465 5f72 6570 6f72 7428  p.update_report(
+00007f10: 725f 6861 7368 3d72 5f68 6173 682c 202a  r_hash=r_hash, *
+00007f20: 2a70 6172 616d 7329 0a20 2020 2020 2020  *params).       
+00007f30: 2020 2020 2020 2020 206c 6f67 6765 722e           logger.
+00007f40: 696e 666f 2866 2255 7064 6174 6564 207b  info(f"Updated {
+00007f50: 6368 6172 745f 636c 6173 732e 5f5f 6e61  chart_class.__na
+00007f60: 6d65 5f5f 7d20 6174 207b 7374 7228 6368  me__} at {str(ch
+00007f70: 6172 7429 7d22 290a 2020 2020 2020 2020  art)}").        
+00007f80: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00007f90: 2020 2020 2020 2020 2020 6c6f 6767 6572            logger
+00007fa0: 2e69 6e66 6f28 0a20 2020 2020 2020 2020  .info(.         
+00007fb0: 2020 2020 2020 2020 2020 2066 224e 6f20             f"No 
+00007fc0: 6368 616e 6765 7320 6e65 6564 6564 2066  changes needed f
+00007fd0: 6f72 207b 6368 6172 745f 636c 6173 732e  or {chart_class.
+00007fe0: 5f5f 6e61 6d65 5f5f 7d20 6174 207b 7374  __name__} at {st
+00007ff0: 7228 6368 6172 7429 7d22 0a20 2020 2020  r(chart)}".     
+00008000: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+00008010: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+00008020: 7572 6e20 6368 6172 740a 2020 2020 2020  urn chart.      
+00008030: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00008040: 2020 2020 6576 656e 745f 7479 7065 3a20      event_type: 
+00008050: 4576 656e 7454 7970 6520 3d20 4576 656e  EventType = Even
+00008060: 7454 7970 652e 5245 504f 5254 5f43 5245  tType.REPORT_CRE
+00008070: 4154 4544 0a20 2020 2020 2020 2020 2020  ATED.           
+00008080: 2061 7761 6974 2073 656c 662e 5f63 6865   await self._che
+00008090: 636b 5f70 7265 7669 6f75 735f 7061 7468  ck_previous_path
+000080a0: 7328 290a 2020 2020 2020 2020 2020 2020  s().            
+000080b0: 7061 7261 6d73 5b22 7061 7468 4f72 6465  params["pathOrde
+000080c0: 7222 5d20 3d20 280a 2020 2020 2020 2020  r"] = (.        
+000080d0: 2020 2020 2020 2020 7365 6c66 2e5f 6578          self._ex
+000080e0: 6563 7574 696f 6e5f 7061 7468 5f6f 7264  ecution_path_ord
+000080f0: 6572 732e 696e 6465 7828 7365 6c66 2e5f  ers.index(self._
+00008100: 6375 7272 656e 745f 7061 7468 290a 2020  current_path).  
+00008110: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00008120: 2073 656c 662e 5f63 7572 7265 6e74 5f70   self._current_p
+00008130: 6174 680a 2020 2020 2020 2020 2020 2020  ath.            
+00008140: 2020 2020 656c 7365 204e 6f6e 650a 2020      else None.  
+00008150: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+00008160: 2020 2020 2020 2020 7061 7261 6d73 5b22          params["
+00008170: 6f72 6465 7222 5d20 3d20 6f72 6465 720a  order"] = order.
+00008180: 2020 2020 2020 2020 2020 2020 6368 6172              char
+00008190: 743a 2052 6570 6f72 7420 3d20 6177 6169  t: Report = awai
+000081a0: 7420 7365 6c66 2e5f 6170 702e 6372 6561  t self._app.crea
+000081b0: 7465 5f72 6570 6f72 7428 0a20 2020 2020  te_report(.     
+000081c0: 2020 2020 2020 2020 2020 2063 6861 7274             chart
+000081d0: 5f63 6c61 7373 2c20 725f 6861 7368 3d72  _class, r_hash=r
+000081e0: 5f68 6173 682c 202a 2a70 6172 616d 730a  _hash, **params.
+000081f0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+00008200: 2020 2020 2020 2020 2020 6c6f 6767 6572            logger
+00008210: 2e69 6e66 6f28 0a20 2020 2020 2020 2020  .info(.         
+00008220: 2020 2020 2020 2066 2743 7265 6174 6564         f'Created
+00008230: 207b 6368 6172 745f 636c 6173 732e 5f5f   {chart_class.__
+00008240: 6e61 6d65 5f5f 7d20 6174 207b 7374 7228  name__} at {str(
+00008250: 6368 6172 7429 7d20 7769 7468 2069 6420  chart)} with id 
+00008260: 7b63 6861 7274 5b22 6964 225d 7d27 0a20  {chart["id"]}'. 
+00008270: 2020 2020 2020 2020 2020 2029 0a0a 2020             )..  
+00008280: 2020 2020 2020 6164 6465 645f 746f 5f63        added_to_c
+00008290: 6f6e 7461 696e 6572 203d 2046 616c 7365  ontainer = False
+000082a0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+000082b0: 2e5f 6375 7272 656e 745f 7461 6273 5f67  ._current_tabs_g
+000082c0: 726f 7570 3a0a 2020 2020 2020 2020 2020  roup:.          
+000082d0: 2020 6966 206e 6f74 2073 656c 662e 5f63    if not self._c
+000082e0: 7572 7265 6e74 5f74 6162 735f 6772 6f75  urrent_tabs_grou
+000082f0: 702e 6861 735f 7265 706f 7274 2863 6861  p.has_report(cha
+00008300: 7274 293a 0a20 2020 2020 2020 2020 2020  rt):.           
+00008310: 2020 2020 2028 6177 6169 7420 7365 6c66       (await self
+00008320: 2e5f 6765 745f 6375 7272 656e 745f 7461  ._get_current_ta
+00008330: 6273 5f67 726f 7570 2829 292e 6164 645f  bs_group()).add_
+00008340: 7265 706f 7274 280a 2020 2020 2020 2020  report(.        
+00008350: 2020 2020 2020 2020 2020 2020 7461 623d              tab=
+00008360: 7365 6c66 2e5f 6375 7272 656e 745f 7461  self._current_ta
+00008370: 622c 2072 6570 6f72 743d 6368 6172 740a  b, report=chart.
+00008380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008390: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+000083a0: 2020 6c6f 6767 6572 2e69 6e66 6f28 0a20    logger.info(. 
+000083b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000083c0: 2020 2066 2249 6e63 6c75 6465 6420 6368     f"Included ch
+000083d0: 6172 7420 7b73 7472 2863 6861 7274 297d  art {str(chart)}
+000083e0: 2069 6e20 7461 6273 2067 726f 7570 207b   in tabs group {
+000083f0: 7374 7228 7365 6c66 2e5f 6375 7272 656e  str(self._curren
+00008400: 745f 7461 6273 5f67 726f 7570 297d 220a  t_tabs_group)}".
+00008410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008420: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00008430: 2020 6164 6465 645f 746f 5f63 6f6e 7461    added_to_conta
+00008440: 696e 6572 203d 2054 7275 650a 2020 2020  iner = True.    
+00008450: 2020 2020 656c 6966 2073 656c 662e 5f63      elif self._c
+00008460: 7572 7265 6e74 5f6d 6f64 616c 2061 6e64  urrent_modal and
+00008470: 206e 6f74 2073 656c 662e 5f63 7572 7265   not self._curre
+00008480: 6e74 5f6d 6f64 616c 2e68 6173 5f72 6570  nt_modal.has_rep
+00008490: 6f72 7428 6368 6172 7429 3a0a 2020 2020  ort(chart):.    
+000084a0: 2020 2020 2020 2020 2861 7761 6974 2073          (await s
+000084b0: 656c 662e 5f67 6574 5f63 7572 7265 6e74  elf._get_current
+000084c0: 5f6d 6f64 616c 2829 292e 6164 645f 7265  _modal()).add_re
+000084d0: 706f 7274 2863 6861 7274 290a 2020 2020  port(chart).    
+000084e0: 2020 2020 2020 2020 6c6f 6767 6572 2e69          logger.i
+000084f0: 6e66 6f28 0a20 2020 2020 2020 2020 2020  nfo(.           
+00008500: 2020 2020 2066 2249 6e63 6c75 6465 6420       f"Included 
+00008510: 6368 6172 7420 7b73 7472 2863 6861 7274  chart {str(chart
+00008520: 297d 2069 6e20 6d6f 6461 6c20 7b73 7472  )} in modal {str
+00008530: 2873 656c 662e 5f63 7572 7265 6e74 5f6d  (self._current_m
+00008540: 6f64 616c 297d 220a 2020 2020 2020 2020  odal)}".        
+00008550: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
+00008560: 2020 6164 6465 645f 746f 5f63 6f6e 7461    added_to_conta
+00008570: 696e 6572 203d 2054 7275 650a 0a20 2020  iner = True..   
+00008580: 2020 2020 2069 6620 280a 2020 2020 2020       if (.      
+00008590: 2020 2020 2020 6164 6465 645f 746f 5f63        added_to_c
+000085a0: 6f6e 7461 696e 6572 0a20 2020 2020 2020  ontainer.       
+000085b0: 2020 2020 2061 6e64 2022 7570 6461 7465       and "update
+000085c0: 5f63 6f6e 7461 696e 6572 7322 206e 6f74  _containers" not
+000085d0: 2069 6e20 7365 6c66 2e5f 6173 796e 635f   in self._async_
+000085e0: 706f 6f6c 2e65 6e64 696e 675f 7461 736b  pool.ending_task
+000085f0: 730a 2020 2020 2020 2020 293a 0a20 2020  s.        ):.   
+00008600: 2020 2020 2020 2020 2073 656c 662e 5f61           self._a
+00008610: 7379 6e63 5f70 6f6f 6c2e 656e 6469 6e67  sync_pool.ending
+00008620: 5f74 6173 6b73 5b0a 2020 2020 2020 2020  _tasks[.        
+00008630: 2020 2020 2020 2020 2275 7064 6174 655f          "update_
+00008640: 636f 6e74 6169 6e65 7273 220a 2020 2020  containers".    
+00008650: 2020 2020 2020 2020 5d20 3d20 7365 6c66          ] = self
+00008660: 2e5f 7570 6461 7465 5f63 6f6e 7461 696e  ._update_contain
+00008670: 6572 7328 290a 0a20 2020 2020 2020 2061  ers()..        a
+00008680: 7761 6974 2073 656c 662e 5f63 7265 6174  wait self._creat
+00008690: 655f 6576 656e 7428 6576 656e 745f 7479  e_event(event_ty
+000086a0: 7065 2c20 7b7d 2c20 6368 6172 745b 2269  pe, {}, chart["i
+000086b0: 6422 5d29 0a0a 2020 2020 2020 2020 7265  d"])..        re
+000086c0: 7475 726e 2063 6861 7274 0a0a 2020 2020  turn chart..    
+000086d0: 6465 6620 5f67 6574 5f66 6965 6c64 5f6d  def _get_field_m
+000086e0: 6170 7069 6e67 280a 2020 2020 2020 2020  apping(.        
+000086f0: 7365 6c66 2c20 6669 656c 643a 2055 6e69  self, field: Uni
+00008700: 6f6e 5b73 7472 2c20 7475 706c 652c 206c  on[str, tuple, l
+00008710: 6973 742c 2064 6963 745d 2c20 6461 7461  ist, dict], data
+00008720: 5f6d 6170 7069 6e67 5f74 6f5f 7475 706c  _mapping_to_tupl
+00008730: 653a 2064 6963 740a 2020 2020 2920 2d3e  e: dict.    ) ->
+00008740: 2055 6e69 6f6e 5b73 7472 2c20 6c69 7374   Union[str, list
+00008750: 2c20 6469 6374 5d3a 0a20 2020 2020 2020  , dict]:.       
+00008760: 2022 2222 4765 7420 7468 6520 6d61 7070   """Get the mapp
+00008770: 696e 6720 6f66 2061 2066 6965 6c64 2e22  ing of a field."
+00008780: 2222 0a20 2020 2020 2020 2069 6620 6973  "".        if is
+00008790: 696e 7374 616e 6365 2866 6965 6c64 2c20  instance(field, 
+000087a0: 7374 7229 3a0a 2020 2020 2020 2020 2020  str):.          
+000087b0: 2020 7265 7475 726e 2064 6174 615f 6d61    return data_ma
+000087c0: 7070 696e 675f 746f 5f74 7570 6c65 5b66  pping_to_tuple[f
+000087d0: 6965 6c64 5d5b 305d 0a20 2020 2020 2020  ield][0].       
+000087e0: 2065 6c69 6620 6973 696e 7374 616e 6365   elif isinstance
+000087f0: 2866 6965 6c64 2c20 2874 7570 6c65 2c20  (field, (tuple, 
+00008800: 6c69 7374 2929 3a0a 2020 2020 2020 2020  list)):.        
+00008810: 2020 2020 7265 7475 726e 205b 6461 7461      return [data
+00008820: 5f6d 6170 7069 6e67 5f74 6f5f 7475 706c  _mapping_to_tupl
+00008830: 655b 665d 5b30 5d20 666f 7220 6620 696e  e[f][0] for f in
+00008840: 2066 6965 6c64 5d0a 2020 2020 2020 2020   field].        
+00008850: 656c 6966 2069 7369 6e73 7461 6e63 6528  elif isinstance(
+00008860: 6669 656c 642c 2064 6963 7429 3a0a 2020  field, dict):.  
+00008870: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00008880: 207b 6b3a 2064 6174 615f 6d61 7070 696e   {k: data_mappin
+00008890: 675f 746f 5f74 7570 6c65 5b76 5d5b 305d  g_to_tuple[v][0]
+000088a0: 2066 6f72 206b 2c20 7620 696e 2066 6965   for k, v in fie
+000088b0: 6c64 2e69 7465 6d73 2829 7d0a 0a20 2020  ld.items()}..   
+000088c0: 2064 6566 205f 6368 6563 6b5f 6d61 7070   def _check_mapp
+000088d0: 696e 675f 696e 5f72 6570 6f72 745f 6461  ing_in_report_da
+000088e0: 7461 5f73 6574 280a 2020 2020 2020 2020  ta_set(.        
+000088f0: 7365 6c66 2c20 7265 706f 7274 5f64 6174  self, report_dat
+00008900: 615f 7365 743a 2052 6570 6f72 742e 5265  a_set: Report.Re
+00008910: 706f 7274 4461 7461 5365 742c 206d 6170  portDataSet, map
+00008920: 7069 6e67 3a20 4d61 7070 696e 670a 2020  ping: Mapping.  
+00008930: 2020 2920 2d3e 2062 6f6f 6c3a 0a20 2020    ) -> bool:.   
+00008940: 2020 2020 2022 2222 4368 6563 6b20 6966       """Check if
+00008950: 2074 6865 206d 6170 7069 6e67 2069 7320   the mapping is 
+00008960: 636f 7272 6563 7420 696e 2074 6865 2072  correct in the r
+00008970: 6570 6f72 7420 6461 7461 2073 6574 2e0a  eport data set..
+00008980: 2020 2020 2020 2020 3a70 6172 616d 2072          :param r
+00008990: 6570 6f72 745f 6461 7461 5f73 6574 3a20  eport_data_set: 
+000089a0: 7468 6520 7265 706f 7274 2064 6174 6120  the report data 
+000089b0: 7365 740a 2020 2020 2020 2020 3a70 6172  set.        :par
+000089c0: 616d 206d 6170 7069 6e67 3a20 7468 6520  am mapping: the 
+000089d0: 6d61 7070 696e 670a 2020 2020 2020 2020  mapping.        
+000089e0: 3a72 6574 7572 6e3a 2054 7275 6520 6966  :return: True if
+000089f0: 2074 6865 206d 6170 7069 6e67 2069 7320   the mapping is 
+00008a00: 636f 6e73 6973 7465 6e74 2c20 4661 6c73  consistent, Fals
+00008a10: 6520 6f74 6865 7277 6973 650a 2020 2020  e otherwise.    
+00008a20: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00008a30: 7265 706f 7274 5f64 6174 615f 7365 745f  report_data_set_
+00008a40: 6d61 7070 696e 6720 3d20 7265 706f 7274  mapping = report
+00008a50: 5f64 6174 615f 7365 745b 2270 726f 7065  _data_set["prope
+00008a60: 7274 6965 7322 5d5b 226d 6170 7069 6e67  rties"]["mapping
+00008a70: 225d 0a20 2020 2020 2020 2069 6620 7265  "].        if re
+00008a80: 706f 7274 5f64 6174 615f 7365 745f 6d61  port_data_set_ma
+00008a90: 7070 696e 6720 213d 206d 6170 7069 6e67  pping != mapping
+00008aa0: 3a0a 2020 2020 2020 2020 2020 2020 6c6f  :.            lo
+00008ab0: 6767 6572 2e77 6172 6e69 6e67 280a 2020  gger.warning(.  
+00008ac0: 2020 2020 2020 2020 2020 2020 2020 6622                f"
+00008ad0: 4d61 7070 696e 6720 696e 636f 6e73 6973  Mapping inconsis
+00008ae0: 7465 6e74 2069 6e20 636f 6d70 6f6e 656e  tent in componen
+00008af0: 7420 6461 7461 2073 6574 206c 696e 6b20  t data set link 
+00008b00: 7b73 7472 2872 6570 6f72 745f 6461 7461  {str(report_data
+00008b10: 5f73 6574 297d 220a 2020 2020 2020 2020  _set)}".        
+00008b20: 2020 2020 290a 2020 2020 2020 2020 7265      ).        re
+00008b30: 7475 726e 2072 6570 6f72 745f 6461 7461  turn report_data
+00008b40: 5f73 6574 5f6d 6170 7069 6e67 203d 3d20  _set_mapping == 
+00008b50: 6d61 7070 696e 670a 0a20 2020 2040 7374  mapping..    @st
+00008b60: 6174 6963 6d65 7468 6f64 0a20 2020 2064  aticmethod.    d
+00008b70: 6566 205f 6765 745f 6669 6c74 6572 5f70  ef _get_filter_p
+00008b80: 726f 7065 7274 6965 7328 0a20 2020 2020  roperties(.     
+00008b90: 2020 2073 6572 6965 735f 6e61 6d65 3a20     series_name: 
+00008ba0: 7374 722c 2063 6f6e 7665 7274 6564 5f64  str, converted_d
+00008bb0: 6174 613a 2070 642e 4461 7461 4672 616d  ata: pd.DataFram
+00008bc0: 652c 206d 756c 7469 5f73 656c 6563 743a  e, multi_select:
+00008bd0: 2062 6f6f 6c0a 2020 2020 2920 2d3e 2074   bool.    ) -> t
+00008be0: 7570 6c65 5b4f 7074 696f 6e61 6c5b 6c69  uple[Optional[li
+00008bf0: 7374 5b73 7472 5d5d 2c20 4f70 7469 6f6e  st[str]], Option
+00008c00: 616c 5b6c 6973 745b 7374 725d 5d2c 2046  al[list[str]], F
+00008c10: 696c 7465 7244 6174 6153 6574 2e49 6e70  ilterDataSet.Inp
+00008c20: 7574 5479 7065 5d3a 0a20 2020 2020 2020  utType]:.       
+00008c30: 2069 6620 7365 7269 6573 5f6e 616d 652e   if series_name.
+00008c40: 7374 6172 7473 7769 7468 2822 6461 7465  startswith("date
+00008c50: 2229 3a0a 2020 2020 2020 2020 2020 2020  "):.            
+00008c60: 7265 7475 726e 204e 6f6e 652c 205b 2263  return None, ["c
+00008c70: 6f6e 7461 696e 7322 5d2c 2046 696c 7465  ontains"], Filte
+00008c80: 7244 6174 6153 6574 2e49 6e70 7574 5479  rDataSet.InputTy
+00008c90: 7065 2e44 4154 4552 414e 4745 0a20 2020  pe.DATERANGE.   
+00008ca0: 2020 2020 2065 6c69 6620 7365 7269 6573       elif series
+00008cb0: 5f6e 616d 652e 7374 6172 7473 7769 7468  _name.startswith
+00008cc0: 2822 696e 7422 293a 0a20 2020 2020 2020  ("int"):.       
+00008cd0: 2020 2020 2072 6574 7572 6e20 4e6f 6e65       return None
+00008ce0: 2c20 4e6f 6e65 2c20 4669 6c74 6572 4461  , None, FilterDa
+00008cf0: 7461 5365 742e 496e 7075 7454 7970 652e  taSet.InputType.
+00008d00: 4e55 4d45 5249 430a 2020 2020 2020 2020  NUMERIC.        
+00008d10: 656c 6966 2073 6572 6965 735f 6e61 6d65  elif series_name
+00008d20: 2e73 7461 7274 7377 6974 6828 2273 7472  .startswith("str
+00008d30: 696e 6722 293a 0a20 2020 2020 2020 2020  ing"):.         
+00008d40: 2020 2072 6574 7572 6e20 280a 2020 2020     return (.    
+00008d50: 2020 2020 2020 2020 2020 2020 636f 6e76              conv
+00008d60: 6572 7465 645f 6461 7461 5b73 6572 6965  erted_data[serie
+00008d70: 735f 6e61 6d65 5d2e 756e 6971 7565 2829  s_name].unique()
+00008d80: 2e74 6f6c 6973 7428 292c 0a20 2020 2020  .tolist(),.     
+00008d90: 2020 2020 2020 2020 2020 205b 2265 7122             ["eq"
+00008da0: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
+00008db0: 2020 2046 696c 7465 7244 6174 6153 6574     FilterDataSet
+00008dc0: 2e49 6e70 7574 5479 7065 2e43 4154 4547  .InputType.CATEG
+00008dd0: 4f52 4943 414c 5f53 494e 474c 450a 2020  ORICAL_SINGLE.  
+00008de0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00008df0: 206e 6f74 206d 756c 7469 5f73 656c 6563   not multi_selec
+00008e00: 740a 2020 2020 2020 2020 2020 2020 2020  t.              
+00008e10: 2020 656c 7365 2046 696c 7465 7244 6174    else FilterDat
+00008e20: 6153 6574 2e49 6e70 7574 5479 7065 2e43  aSet.InputType.C
+00008e30: 4154 4547 4f52 4943 414c 5f4d 554c 5449  ATEGORICAL_MULTI
+00008e40: 2c0a 2020 2020 2020 2020 2020 2020 290a  ,.            ).
+00008e50: 2020 2020 2020 2020 6c6f 675f 6572 726f          log_erro
+00008e60: 7228 0a20 2020 2020 2020 2020 2020 206c  r(.            l
+00008e70: 6f67 6765 722c 2066 2246 6965 6c64 2074  ogger, f"Field t
+00008e80: 7970 6520 7b73 6572 6965 735f 6e61 6d65  ype {series_name
+00008e90: 7d20 6973 206e 6f74 2073 7570 706f 7274  } is not support
+00008ea0: 6564 222c 204e 6f74 496d 706c 656d 656e  ed", NotImplemen
+00008eb0: 7465 6445 7272 6f72 0a20 2020 2020 2020  tedError.       
+00008ec0: 2029 0a0a 2020 2020 4061 6464 5f74 6f5f   )..    @add_to_
+00008ed0: 6765 6e65 7261 6c5f 6173 796e 635f 6772  general_async_gr
+00008ee0: 6f75 700a 2020 2020 6173 796e 6320 6465  oup.    async de
+00008ef0: 6620 6669 6c74 6572 280a 2020 2020 2020  f filter(.      
+00008f00: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
+00008f10: 6f72 6465 723a 2069 6e74 2c0a 2020 2020  order: int,.    
+00008f20: 2020 2020 6461 7461 3a20 7374 722c 0a20      data: str,. 
+00008f30: 2020 2020 2020 2066 6965 6c64 3a20 7374         field: st
+00008f40: 722c 0a20 2020 2020 2020 206d 756c 7469  r,.        multi
+00008f50: 5f73 656c 6563 743a 2062 6f6f 6c20 3d20  _select: bool = 
+00008f60: 4661 6c73 652c 0a20 2020 2020 2020 2063  False,.        c
+00008f70: 6f6c 735f 7369 7a65 3a20 696e 7420 3d20  ols_size: int = 
+00008f80: 342c 0a20 2020 2020 2020 2072 6f77 735f  4,.        rows_
+00008f90: 7369 7a65 3a20 696e 7420 3d20 312c 0a20  size: int = 1,. 
+00008fa0: 2020 2020 2020 2070 6164 6469 6e67 3a20         padding: 
+00008fb0: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
+00008fc0: 4e6f 6e65 2c0a 2020 2020 293a 0a20 2020  None,.    ):.   
+00008fd0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00008fe0: 2046 696c 7465 7220 7468 6520 6461 7461   Filter the data
+00008ff0: 2073 6574 2e0a 2020 2020 2020 2020 3a70   set..        :p
+00009000: 6172 616d 206f 7264 6572 3a20 7468 6520  aram order: the 
+00009010: 6f72 6465 7220 6f66 2074 6865 2063 6861  order of the cha
+00009020: 7274 0a20 2020 2020 2020 203a 7061 7261  rt.        :para
+00009030: 6d20 6461 7461 3a20 7468 6520 6461 7461  m data: the data
+00009040: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+00009050: 6669 656c 643a 2074 6865 2066 6965 6c64  field: the field
+00009060: 2074 6f20 6669 6c74 6572 0a20 2020 2020   to filter.     
+00009070: 2020 203a 7061 7261 6d20 6d75 6c74 695f     :param multi_
+00009080: 7365 6c65 6374 3a20 7768 6574 6865 7220  select: whether 
+00009090: 746f 2061 6c6c 6f77 206d 756c 7469 2073  to allow multi s
+000090a0: 656c 6563 740a 2020 2020 2020 2020 3a70  elect.        :p
+000090b0: 6172 616d 2063 6f6c 735f 7369 7a65 3a20  aram cols_size: 
+000090c0: 7468 6520 7369 7a65 206f 6620 7468 6520  the size of the 
+000090d0: 636f 6c75 6d6e 730a 2020 2020 2020 2020  columns.        
+000090e0: 3a70 6172 616d 2072 6f77 735f 7369 7a65  :param rows_size
+000090f0: 3a20 7468 6520 7369 7a65 206f 6620 7468  : the size of th
+00009100: 6520 726f 7773 0a20 2020 2020 2020 203a  e rows.        :
+00009110: 7061 7261 6d20 7061 6464 696e 673a 2074  param padding: t
+00009120: 6865 2070 6164 6469 6e67 0a20 2020 2020  he padding.     
+00009130: 2020 2022 2222 0a0a 2020 2020 2020 2020     """..        
+00009140: 6966 206e 6f74 2069 7369 6e73 7461 6e63  if not isinstanc
+00009150: 6528 6461 7461 2c20 7374 7229 3a0a 2020  e(data, str):.  
+00009160: 2020 2020 2020 2020 2020 6c6f 675f 6572            log_er
+00009170: 726f 7228 0a20 2020 2020 2020 2020 2020  ror(.           
+00009180: 2020 2020 206c 6f67 6765 722c 0a20 2020       logger,.   
+00009190: 2020 2020 2020 2020 2020 2020 2022 546f               "To
+000091a0: 2066 696c 7465 7220 6120 6461 7461 2073   filter a data s
+000091b0: 6574 2c20 7468 6520 6461 7461 206d 7573  et, the data mus
+000091c0: 7420 6265 2061 2073 6861 7265 6420 6461  t be a shared da
+000091d0: 7461 2065 6e74 7279 222c 0a20 2020 2020  ta entry",.     
+000091e0: 2020 2020 2020 2020 2020 2044 6174 6145             DataE
+000091f0: 7272 6f72 2c0a 2020 2020 2020 2020 2020  rror,.          
+00009200: 2020 290a 0a20 2020 2020 2020 2069 6620    )..        if 
+00009210: 6461 7461 206e 6f74 2069 6e20 7365 6c66  data not in self
+00009220: 2e5f 7368 6172 6564 5f64 6174 615f 6d61  ._shared_data_ma
+00009230: 703a 0a20 2020 2020 2020 2020 2020 206c  p:.            l
+00009240: 6f67 5f65 7272 6f72 286c 6f67 6765 722c  og_error(logger,
+00009250: 2066 224e 6f20 7368 6172 6564 2064 6174   f"No shared dat
+00009260: 6120 7769 7468 206e 616d 6520 7b64 6174  a with name {dat
+00009270: 617d 2066 6f75 6e64 222c 2044 6174 6145  a} found", DataE
+00009280: 7272 6f72 290a 0a20 2020 2020 2020 205f  rror)..        _
+00009290: 2c20 6461 7461 5f73 6574 2c20 5f20 3d20  , data_set, _ = 
+000092a0: 7365 6c66 2e5f 7368 6172 6564 5f64 6174  self._shared_dat
+000092b0: 615f 6d61 705b 6461 7461 5d5b 6669 656c  a_map[data][fiel
+000092c0: 645d 0a20 2020 2020 2020 2064 6174 6120  d].        data 
+000092d0: 3d20 7365 6c66 2e5f 7368 6172 6564 5f64  = self._shared_d
+000092e0: 6174 615b 6461 7461 5d0a 0a20 2020 2020  ata[data]..     
+000092f0: 2020 2063 6f6e 7665 7274 6564 5f64 6174     converted_dat
+00009300: 612c 2073 6572 6965 735f 6e61 6d65 203d  a, series_name =
+00009310: 2063 6f6e 7665 7274 5f64 6174 615f 616e   convert_data_an
+00009320: 645f 6765 745f 7365 7269 6573 5f6e 616d  d_get_series_nam
+00009330: 6528 6461 7461 2c20 6669 656c 6429 0a20  e(data, field). 
+00009340: 2020 2020 2020 206f 7074 696f 6e73 2c20         options, 
+00009350: 6f70 6572 6174 696f 6e73 2c20 696e 7075  operations, inpu
+00009360: 745f 7479 7065 203d 2073 656c 662e 5f67  t_type = self._g
+00009370: 6574 5f66 696c 7465 725f 7072 6f70 6572  et_filter_proper
+00009380: 7469 6573 280a 2020 2020 2020 2020 2020  ties(.          
+00009390: 2020 7365 7269 6573 5f6e 616d 652c 2063    series_name, c
+000093a0: 6f6e 7665 7274 6564 5f64 6174 612c 206d  onverted_data, m
+000093b0: 756c 7469 5f73 656c 6563 740a 2020 2020  ulti_select.    
+000093c0: 2020 2020 290a 0a20 2020 2020 2020 2070      )..        p
+000093d0: 726f 7065 7274 6965 7320 3d20 7b0a 2020  roperties = {.  
+000093e0: 2020 2020 2020 2020 2020 2266 696c 7465            "filte
+000093f0: 7222 3a20 5b0a 2020 2020 2020 2020 2020  r": [.          
+00009400: 2020 2020 2020 7b0a 2020 2020 2020 2020        {.        
+00009410: 2020 2020 2020 2020 2020 2020 2266 6965              "fie
+00009420: 6c64 223a 2066 6965 6c64 2c0a 2020 2020  ld": field,.    
+00009430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009440: 2269 6e70 7574 5479 7065 223a 2069 6e70  "inputType": inp
+00009450: 7574 5f74 7970 652e 7661 6c75 652c 0a20  ut_type.value,. 
+00009460: 2020 2020 2020 2020 2020 2020 2020 207d                 }
+00009470: 0a20 2020 2020 2020 2020 2020 205d 2c0a  .            ],.
+00009480: 2020 2020 2020 2020 2020 2020 226d 6170              "map
+00009490: 7069 6e67 223a 205b 7b66 6965 6c64 3a20  ping": [{field: 
+000094a0: 7365 7269 6573 5f6e 616d 652c 2022 6964  series_name, "id
+000094b0: 223a 2064 6174 615f 7365 745b 2269 6422  ": data_set["id"
+000094c0: 5d7d 5d2c 0a20 2020 2020 2020 207d 0a0a  ]}],.        }..
+000094d0: 2020 2020 2020 2020 6966 206f 7065 7261          if opera
+000094e0: 7469 6f6e 733a 0a20 2020 2020 2020 2020  tions:.         
+000094f0: 2020 2070 726f 7065 7274 6965 735b 2266     properties["f
+00009500: 696c 7465 7222 5d5b 305d 5b22 6f70 6572  ilter"][0]["oper
+00009510: 6174 696f 6e73 225d 203d 206f 7065 7261  ations"] = opera
+00009520: 7469 6f6e 730a 2020 2020 2020 2020 6966  tions.        if
+00009530: 206f 7074 696f 6e73 3a0a 2020 2020 2020   options:.      
+00009540: 2020 2020 2020 7072 6f70 6572 7469 6573        properties
+00009550: 5b22 6669 6c74 6572 225d 5b30 5d5b 226f  ["filter"][0]["o
+00009560: 7074 696f 6e73 225d 203d 206f 7074 696f  ptions"] = optio
+00009570: 6e73 0a0a 2020 2020 2020 2020 6177 6169  ns..        awai
+00009580: 7420 7365 6c66 2e5f 6372 6561 7465 5f63  t self._create_c
+00009590: 6861 7274 280a 2020 2020 2020 2020 2020  hart(.          
+000095a0: 2020 6368 6172 745f 636c 6173 733d 4669    chart_class=Fi
+000095b0: 6c74 6572 4461 7461 5365 742c 0a20 2020  lterDataSet,.   
+000095c0: 2020 2020 2020 2020 206f 7264 6572 3d6f           order=o
+000095d0: 7264 6572 2c0a 2020 2020 2020 2020 2020  rder,.          
+000095e0: 2020 7469 746c 653d 2222 2c0a 2020 2020    title="",.    
+000095f0: 2020 2020 2020 2020 7369 7a65 526f 7773          sizeRows
+00009600: 3d72 6f77 735f 7369 7a65 2c0a 2020 2020  =rows_size,.    
+00009610: 2020 2020 2020 2020 7369 7a65 436f 6c75          sizeColu
+00009620: 6d6e 733d 636f 6c73 5f73 697a 652c 0a20  mns=cols_size,. 
+00009630: 2020 2020 2020 2020 2020 2073 697a 6550             sizeP
+00009640: 6164 6469 6e67 3d70 6164 6469 6e67 2c0a  adding=padding,.
+00009650: 2020 2020 2020 2020 2020 2020 7072 6f70              prop
+00009660: 6572 7469 6573 3d70 726f 7065 7274 6965  erties=propertie
+00009670: 732c 0a20 2020 2020 2020 2029 0a0a 2020  s,.        )..  
+00009680: 2020 4061 6464 5f74 6f5f 6765 6e65 7261    @add_to_genera
+00009690: 6c5f 6173 796e 635f 6772 6f75 700a 2020  l_async_group.  
+000096a0: 2020 6173 796e 6320 6465 6620 6966 7261    async def ifra
+000096b0: 6d65 280a 2020 2020 2020 2020 7365 6c66  me(.        self
+000096c0: 2c0a 2020 2020 2020 2020 7572 6c3a 2073  ,.        url: s
+000096d0: 7472 2c0a 2020 2020 2020 2020 6f72 6465  tr,.        orde
+000096e0: 723a 2069 6e74 2c0a 2020 2020 2020 2020  r: int,.        
+000096f0: 6865 6967 6874 3a20 696e 7420 3d20 3634  height: int = 64
+00009700: 302c 0a20 2020 2020 2020 2063 6f6c 735f  0,.        cols_
+00009710: 7369 7a65 3a20 4f70 7469 6f6e 616c 5b69  size: Optional[i
+00009720: 6e74 5d20 3d20 4e6f 6e65 2c0a 2020 2020  nt] = None,.    
+00009730: 2020 2020 7061 6464 696e 673a 204f 7074      padding: Opt
+00009740: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
+00009750: 652c 0a20 2020 2029 3a0a 2020 2020 2020  e,.    ):.      
+00009760: 2020 2222 2243 7265 6174 6520 616e 2069    """Create an i
+00009770: 6672 616d 6520 7265 706f 7274 2069 6e20  frame report in 
+00009780: 7468 6520 6461 7368 626f 6172 642e 0a20  the dashboard.. 
+00009790: 2020 2020 2020 203a 7061 7261 6d20 7572         :param ur
+000097a0: 6c3a 2074 6865 2075 726c 206f 6620 7468  l: the url of th
+000097b0: 6520 6966 7261 6d65 0a20 2020 2020 2020  e iframe.       
+000097c0: 203a 7061 7261 6d20 6f72 6465 723a 2074   :param order: t
+000097d0: 6865 206f 7264 6572 206f 6620 7468 6520  he order of the 
+000097e0: 6966 7261 6d65 0a20 2020 2020 2020 203a  iframe.        :
+000097f0: 7061 7261 6d20 6865 6967 6874 3a20 7468  param height: th
+00009800: 6520 6865 6967 6874 206f 6620 7468 6520  e height of the 
+00009810: 6966 7261 6d65 0a20 2020 2020 2020 203a  iframe.        :
+00009820: 7061 7261 6d20 636f 6c73 5f73 697a 653a  param cols_size:
+00009830: 2074 6865 2063 6f6c 756d 6e73 2074 6861   the columns tha
+00009840: 7420 7468 6520 6966 7261 6d65 206f 6363  t the iframe occ
+00009850: 7570 6965 730a 2020 2020 2020 2020 3a70  upies.        :p
+00009860: 6172 616d 2070 6164 6469 6e67 3a20 7061  aram padding: pa
+00009870: 6464 696e 670a 2020 2020 2020 2020 2222  dding.        ""
+00009880: 220a 2020 2020 2020 2020 6177 6169 7420  ".        await 
+00009890: 7365 6c66 2e5f 6372 6561 7465 5f63 6861  self._create_cha
+000098a0: 7274 280a 2020 2020 2020 2020 2020 2020  rt(.            
+000098b0: 6368 6172 745f 636c 6173 733d 4946 7261  chart_class=IFra
+000098c0: 6d65 2c0a 2020 2020 2020 2020 2020 2020  me,.            
+000098d0: 6f72 6465 723d 6f72 6465 722c 0a20 2020  order=order,.   
+000098e0: 2020 2020 2020 2020 2064 6174 6146 6965           dataFie
+000098f0: 6c64 733d 6469 6374 280a 2020 2020 2020  lds=dict(.      
+00009900: 2020 2020 2020 2020 2020 7572 6c3d 7572            url=ur
+00009910: 6c2c 0a20 2020 2020 2020 2020 2020 2020  l,.             
+00009920: 2020 2068 6569 6768 743d 6865 6967 6874     height=height
+00009930: 2c0a 2020 2020 2020 2020 2020 2020 292c  ,.            ),
+00009940: 0a20 2020 2020 2020 2020 2020 2073 697a  .            siz
+00009950: 6550 6164 6469 6e67 3d70 6164 6469 6e67  ePadding=padding
+00009960: 2c0a 2020 2020 2020 2020 2020 2020 7369  ,.            si
+00009970: 7a65 436f 6c75 6d6e 733d 636f 6c73 5f73  zeColumns=cols_s
+00009980: 697a 652c 0a20 2020 2020 2020 2020 2020  ize,.           
+00009990: 2073 697a 6552 6f77 733d 6365 696c 2868   sizeRows=ceil(h
+000099a0: 6569 6768 7420 2f20 3234 3029 2c0a 2020  eight / 240),.  
+000099b0: 2020 2020 2020 290a 0a20 2020 2061 7379        )..    asy
+000099c0: 6e63 2064 6566 205f 6874 6d6c 280a 2020  nc def _html(.  
+000099d0: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
+000099e0: 2020 2020 6874 6d6c 3a20 7374 722c 0a20      html: str,. 
+000099f0: 2020 2020 2020 206f 7264 6572 3a20 696e         order: in
+00009a00: 742c 0a20 2020 2020 2020 2063 6f6c 735f  t,.        cols_
+00009a10: 7369 7a65 3a20 4f70 7469 6f6e 616c 5b69  size: Optional[i
+00009a20: 6e74 5d20 3d20 4e6f 6e65 2c0a 2020 2020  nt] = None,.    
+00009a30: 2020 2020 726f 7773 5f73 697a 653a 204f      rows_size: O
+00009a40: 7074 696f 6e61 6c5b 696e 745d 203d 204e  ptional[int] = N
+00009a50: 6f6e 652c 0a20 2020 2020 2020 2070 6164  one,.        pad
+00009a60: 6469 6e67 3a20 4f70 7469 6f6e 616c 5b73  ding: Optional[s
+00009a70: 7472 5d20 3d20 4e6f 6e65 2c0a 2020 2020  tr] = None,.    
+00009a80: 293a 0a20 2020 2020 2020 2022 2222 6874  ):.        """ht
+00009a90: 6d6c 2066 6f72 2069 6e74 6572 6e61 6c20  ml for internal 
+00009aa0: 7573 6522 2222 0a20 2020 2020 2020 2061  use""".        a
+00009ab0: 7761 6974 2073 656c 662e 5f63 7265 6174  wait self._creat
+00009ac0: 655f 6368 6172 7428 0a20 2020 2020 2020  e_chart(.       
+00009ad0: 2020 2020 2063 6861 7274 5f63 6c61 7373       chart_class
+00009ae0: 3d48 544d 4c2c 0a20 2020 2020 2020 2020  =HTML,.         
+00009af0: 2020 206f 7264 6572 3d6f 7264 6572 2c0a     order=order,.
+00009b00: 2020 2020 2020 2020 2020 2020 6368 6172              char
+00009b10: 7444 6174 613d 5b7b 2276 616c 7565 223a  tData=[{"value":
+00009b20: 2068 746d 6c7d 5d2c 0a20 2020 2020 2020   html}],.       
+00009b30: 2020 2020 2073 697a 6550 6164 6469 6e67       sizePadding
+00009b40: 3d70 6164 6469 6e67 2c0a 2020 2020 2020  =padding,.      
+00009b50: 2020 2020 2020 7369 7a65 436f 6c75 6d6e        sizeColumn
+00009b60: 733d 636f 6c73 5f73 697a 652c 0a20 2020  s=cols_size,.   
+00009b70: 2020 2020 2020 2020 2073 697a 6552 6f77           sizeRow
+00009b80: 733d 726f 7773 5f73 697a 652c 0a20 2020  s=rows_size,.   
+00009b90: 2020 2020 2029 0a0a 2020 2020 4061 6464       )..    @add
+00009ba0: 5f74 6f5f 6765 6e65 7261 6c5f 6173 796e  _to_general_asyn
+00009bb0: 635f 6772 6f75 700a 2020 2020 6173 796e  c_group.    asyn
+00009bc0: 6320 6465 6620 6874 6d6c 280a 2020 2020  c def html(.    
+00009bd0: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
+00009be0: 2020 6874 6d6c 3a20 7374 722c 0a20 2020    html: str,.   
+00009bf0: 2020 2020 206f 7264 6572 3a20 696e 742c       order: int,
+00009c00: 0a20 2020 2020 2020 2063 6f6c 735f 7369  .        cols_si
+00009c10: 7a65 3a20 4f70 7469 6f6e 616c 5b69 6e74  ze: Optional[int
+00009c20: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
+00009c30: 2020 726f 7773 5f73 697a 653a 204f 7074    rows_size: Opt
+00009c40: 696f 6e61 6c5b 696e 745d 203d 204e 6f6e  ional[int] = Non
+00009c50: 652c 0a20 2020 2020 2020 2070 6164 6469  e,.        paddi
+00009c60: 6e67 3a20 4f70 7469 6f6e 616c 5b73 7472  ng: Optional[str
+00009c70: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 293a  ] = None,.    ):
+00009c80: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00009c90: 2020 2020 2043 7265 6174 6520 616e 2068       Create an h
+00009ca0: 746d 6c20 7265 706f 7274 2069 6e20 7468  tml report in th
+00009cb0: 6520 6461 7368 626f 6172 642e 0a20 2020  e dashboard..   
+00009cc0: 2020 2020 203a 7061 7261 6d20 6874 6d6c       :param html
+00009cd0: 3a20 7468 6520 6874 6d6c 2063 6f64 650a  : the html code.
+00009ce0: 2020 2020 2020 2020 3a70 6172 616d 206f          :param o
+00009cf0: 7264 6572 3a20 7468 6520 6f72 6465 7220  rder: the order 
+00009d00: 6f66 2074 6865 2068 746d 6c0a 2020 2020  of the html.    
+00009d10: 2020 2020 3a63 6f6c 735f 7369 7a65 3a20      :cols_size: 
+00009d20: 7468 6520 636f 6c75 6d6e 7320 7468 6174  the columns that
+00009d30: 2074 6865 2068 746d 6c20 6f63 6375 7069   the html occupi
+00009d40: 6573 0a20 2020 2020 2020 203a 726f 7773  es.        :rows
+00009d50: 5f73 697a 653a 2074 6865 2072 6f77 7320  _size: the rows 
+00009d60: 7468 6174 2074 6865 2068 746d 6c20 6f63  that the html oc
+00009d70: 6375 7069 6573 0a20 2020 2020 2020 203a  cupies.        :
+00009d80: 7061 6464 696e 673a 2070 6164 6469 6e67  padding: padding
+00009d90: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00009da0: 2020 2020 2061 7761 6974 2073 656c 662e       await self.
+00009db0: 5f68 746d 6c28 6874 6d6c 2c20 6f72 6465  _html(html, orde
+00009dc0: 722c 2063 6f6c 735f 7369 7a65 2c20 726f  r, cols_size, ro
+00009dd0: 7773 5f73 697a 652c 2070 6164 6469 6e67  ws_size, padding
+00009de0: 290a 0a20 2020 2040 6164 645f 746f 5f67  )..    @add_to_g
+00009df0: 656e 6572 616c 5f61 7379 6e63 5f67 726f  eneral_async_gro
+00009e00: 7570 0a20 2020 2061 7379 6e63 2064 6566  up.    async def
+00009e10: 2073 696e 676c 655f 696e 6469 6361 746f   single_indicato
+00009e20: 7228 0a20 2020 2020 2020 2073 656c 662c  r(.        self,
+00009e30: 0a20 2020 2020 2020 2064 6174 613a 2064  .        data: d
+00009e40: 6963 742c 0a20 2020 2020 2020 206f 7264  ict,.        ord
+00009e50: 6572 3a20 696e 742c 0a20 2020 2020 2020  er: int,.       
+00009e60: 2063 6f6c 735f 7369 7a65 3a20 4f70 7469   cols_size: Opti
+00009e70: 6f6e 616c 5b69 6e74 5d20 3d20 4e6f 6e65  onal[int] = None
+00009e80: 2c0a 2020 2020 2020 2020 726f 7773 5f73  ,.        rows_s
+00009e90: 697a 653a 204f 7074 696f 6e61 6c5b 696e  ize: Optional[in
+00009ea0: 745d 203d 204e 6f6e 652c 0a20 2020 2020  t] = None,.     
+00009eb0: 2020 2070 6164 6469 6e67 3a20 4f70 7469     padding: Opti
+00009ec0: 6f6e 616c 5b73 7472 5d20 3d20 4e6f 6e65  onal[str] = None
+00009ed0: 2c0a 2020 2020 293a 0a20 2020 2020 2020  ,.    ):.       
+00009ee0: 2022 2222 0a20 2020 2020 2020 2043 7265   """.        Cre
+00009ef0: 6174 6520 616e 2069 6e64 6963 6174 6f72  ate an indicator
+00009f00: 2072 6570 6f72 7420 696e 2074 6865 2064   report in the d
+00009f10: 6173 6862 6f61 7264 2e0a 2020 2020 2020  ashboard..      
+00009f20: 2020 3a70 6172 616d 2064 6174 613a 2074    :param data: t
+00009f30: 6865 2064 6174 6120 6f66 2074 6865 2069  he data of the i
+00009f40: 6e64 6963 6174 6f72 0a20 2020 2020 2020  ndicator.       
+00009f50: 203a 7061 7261 6d20 6f72 6465 723a 2074   :param order: t
+00009f60: 6865 206f 7264 6572 206f 6620 7468 6520  he order of the 
+00009f70: 696e 6469 6361 746f 720a 2020 2020 2020  indicator.      
+00009f80: 2020 3a63 6f6c 735f 7369 7a65 3a20 7468    :cols_size: th
+00009f90: 6520 636f 6c75 6d6e 7320 7468 6174 2074  e columns that t
+00009fa0: 6865 2069 6e64 6963 6174 6f72 206f 6363  he indicator occ
+00009fb0: 7570 6965 730a 2020 2020 2020 2020 3a72  upies.        :r
+00009fc0: 6f77 735f 7369 7a65 3a20 7468 6520 726f  ows_size: the ro
+00009fd0: 7773 2074 6861 7420 7468 6520 696e 6469  ws that the indi
+00009fe0: 6361 746f 7220 6f63 6375 7069 6573 0a20  cator occupies. 
+00009ff0: 2020 2020 2020 203a 7061 6464 696e 673a         :padding:
+0000a000: 2070 6164 6469 6e67 0a20 2020 2020 2020   padding.       
+0000a010: 2022 2222 0a20 2020 2020 2020 2061 7761   """.        awa
+0000a020: 6974 2073 656c 662e 5f63 7265 6174 655f  it self._create_
+0000a030: 6368 6172 7428 0a20 2020 2020 2020 2020  chart(.         
+0000a040: 2020 2063 6861 7274 5f63 6c61 7373 3d49     chart_class=I
+0000a050: 6e64 6963 6174 6f72 2c0a 2020 2020 2020  ndicator,.      
+0000a060: 2020 2020 2020 7061 7468 3d73 656c 662e        path=self.
+0000a070: 5f63 7572 7265 6e74 5f70 6174 682c 0a20  _current_path,. 
+0000a080: 2020 2020 2020 2020 2020 206f 7264 6572             order
+0000a090: 3d6f 7264 6572 2c0a 2020 2020 2020 2020  =order,.        
+0000a0a0: 2020 2020 7369 7a65 5061 6464 696e 673d      sizePadding=
+0000a0b0: 7061 6464 696e 672c 0a20 2020 2020 2020  padding,.       
+0000a0c0: 2020 2020 2073 697a 6552 6f77 733d 726f       sizeRows=ro
+0000a0d0: 7773 5f73 697a 652c 0a20 2020 2020 2020  ws_size,.       
+0000a0e0: 2020 2020 2073 697a 6543 6f6c 756d 6e73       sizeColumns
+0000a0f0: 3d63 6f6c 735f 7369 7a65 2c0a 2020 2020  =cols_size,.    
+0000a100: 2020 2020 2020 2020 7072 6f70 6572 7469          properti
+0000a110: 6573 3d64 6174 612c 0a20 2020 2020 2020  es=data,.       
+0000a120: 2029 0a0a 2020 2020 6465 6620 696e 6469   )..    def indi
+0000a130: 6361 746f 7228 0a20 2020 2020 2020 2073  cator(.        s
+0000a140: 656c 662c 0a20 2020 2020 2020 2064 6174  elf,.        dat
+0000a150: 613a 2055 6e69 6f6e 5b73 7472 2c20 7064  a: Union[str, pd
+0000a160: 2e44 6174 6146 7261 6d65 2c20 6c69 7374  .DataFrame, list
+0000a170: 5b64 6963 745d 2c20 6469 6374 5d2c 0a20  [dict], dict],. 
+0000a180: 2020 2020 2020 206f 7264 6572 3a20 696e         order: in
+0000a190: 742c 0a20 2020 2020 2020 2076 6572 7469  t,.        verti
+0000a1a0: 6361 6c3a 2055 6e69 6f6e 5b62 6f6f 6c2c  cal: Union[bool,
+0000a1b0: 2073 7472 5d20 3d20 4661 6c73 652c 0a20   str] = False,. 
+0000a1c0: 2020 2020 2020 2063 6f6c 6f72 5f62 795f         color_by_
+0000a1d0: 7661 6c75 653a 2062 6f6f 6c20 3d20 4661  value: bool = Fa
+0000a1e0: 6c73 652c 0a20 2020 2020 2020 2063 6f6c  lse,.        col
+0000a1f0: 735f 7369 7a65 3a20 696e 7420 3d20 3132  s_size: int = 12
+0000a200: 2c0a 2020 2020 2020 2020 726f 7773 5f73  ,.        rows_s
+0000a210: 697a 653a 2069 6e74 203d 2031 2c0a 2020  ize: int = 1,.  
+0000a220: 2020 2020 2020 7061 6464 696e 673a 204f        padding: O
+0000a230: 7074 696f 6e61 6c5b 7374 725d 203d 204e  ptional[str] = N
+0000a240: 6f6e 652c 0a20 2020 2020 2020 202a 2a6b  one,.        **k
+0000a250: 7761 7267 732c 2020 2320 6d61 6b65 7320  wargs,  # makes 
+0000a260: 6261 636b 7761 7264 7320 636f 6d70 6174  backwards compat
+0000a270: 6962 696c 6974 7920 6561 7369 6572 0a20  ibility easier. 
+0000a280: 2020 2029 3a0a 2020 2020 2020 2020 2222     ):.        ""
+0000a290: 220a 2020 2020 2020 2020 4372 6561 7465  ".        Create
+0000a2a0: 2061 6e20 696e 6469 6361 746f 7220 7265   an indicator re
+0000a2b0: 706f 7274 2069 6e20 7468 6520 6461 7368  port in the dash
+0000a2c0: 626f 6172 642e 0a20 2020 2020 2020 203a  board..        :
+0000a2d0: 7061 7261 6d20 6461 7461 3a20 7468 6520  param data: the 
+0000a2e0: 6461 7461 206f 6620 7468 6520 696e 6469  data of the indi
+0000a2f0: 6361 746f 720a 2020 2020 2020 2020 3a70  cator.        :p
+0000a300: 6172 616d 206f 7264 6572 3a20 7468 6520  aram order: the 
+0000a310: 6f72 6465 7220 6f66 2074 6865 2069 6e64  order of the ind
+0000a320: 6963 6174 6f72 0a20 2020 2020 2020 203a  icator.        :
+0000a330: 7061 7261 6d20 7665 7274 6963 616c 3a20  param vertical: 
+0000a340: 7768 6574 6865 7220 7468 6520 696e 6469  whether the indi
+0000a350: 6361 746f 7220 6973 2076 6572 7469 6361  cator is vertica
+0000a360: 6c0a 2020 2020 2020 2020 3a70 6172 616d  l.        :param
+0000a370: 2063 6f6c 6f72 5f62 795f 7661 6c75 653a   color_by_value:
+0000a380: 2077 6865 7468 6572 2074 6f20 636f 6c6f   whether to colo
+0000a390: 7220 7468 6520 696e 6469 6361 746f 7220  r the indicator 
+0000a3a0: 6279 2076 616c 7565 0a20 2020 2020 2020  by value.       
+0000a3b0: 203a 636f 6c73 5f73 697a 653a 2074 6865   :cols_size: the
+0000a3c0: 2063 6f6c 756d 6e73 2074 6861 7420 7468   columns that th
+0000a3d0: 6520 696e 6469 6361 746f 7220 6f63 6375  e indicator occu
+0000a3e0: 7069 6573 0a20 2020 2020 2020 203a 726f  pies.        :ro
+0000a3f0: 7773 5f73 697a 653a 2074 6865 2072 6f77  ws_size: the row
+0000a400: 7320 7468 6174 2074 6865 2069 6e64 6963  s that the indic
+0000a410: 6174 6f72 206f 6363 7570 6965 730a 2020  ator occupies.  
+0000a420: 2020 2020 2020 3a70 6164 6469 6e67 3a20        :padding: 
+0000a430: 7061 6464 696e 670a 2020 2020 2020 2020  padding.        
+0000a440: 3a74 6974 6c65 3a20 7468 6520 7469 746c  :title: the titl
+0000a450: 6520 6f66 2074 6865 2069 6e64 6963 6174  e of the indicat
+0000a460: 6f72 0a20 2020 2020 2020 2022 2222 0a20  or.        """. 
+0000a470: 2020 2020 2020 2064 6620 3d20 7064 2e44         df = pd.D
+0000a480: 6174 6146 7261 6d65 2864 6174 6120 6966  ataFrame(data if
+0000a490: 2069 7369 6e73 7461 6e63 6528 6461 7461   isinstance(data
+0000a4a0: 2c20 6c69 7374 2920 656c 7365 205b 6461  , list) else [da
+0000a4b0: 7461 5d29 0a20 2020 2020 2020 206b 6565  ta]).        kee
+0000a4c0: 705f 636f 6c75 6d6e 7320 3d20 5b0a 2020  p_columns = [.  
+0000a4d0: 2020 2020 2020 2020 2020 6b20 666f 7220            k for 
+0000a4e0: 6b20 696e 2064 662e 636f 6c75 6d6e 7320  k in df.columns 
+0000a4f0: 6966 206b 2069 6e20 6c69 7374 2849 6e64  if k in list(Ind
+0000a500: 6963 6174 6f72 2e64 6566 6175 6c74 5f70  icator.default_p
+0000a510: 726f 7065 7274 6965 732e 6b65 7973 2829  roperties.keys()
+0000a520: 290a 2020 2020 2020 2020 5d0a 2020 2020  ).        ].    
+0000a530: 2020 2020 6466 203d 2064 665b 6b65 6570      df = df[keep
+0000a540: 5f63 6f6c 756d 6e73 5d0a 0a20 2020 2020  _columns]..     
+0000a550: 2020 206f 7269 6769 6e61 6c5f 7061 6464     original_padd
+0000a560: 696e 6720 3d20 7061 6464 696e 670a 0a20  ing = padding.. 
+0000a570: 2020 2020 2020 206c 656e 5f64 6620 3d20         len_df = 
+0000a580: 6c65 6e28 6466 290a 2020 2020 2020 2020  len(df).        
+0000a590: 6966 2076 6572 7469 6361 6c20 616e 6420  if vertical and 
+0000a5a0: 286c 656e 5f64 6620 3e20 3120 6f72 2069  (len_df > 1 or i
+0000a5b0: 7369 6e73 7461 6e63 6528 7665 7274 6963  sinstance(vertic
+0000a5c0: 616c 2c20 7374 7229 293a 0a20 2020 2020  al, str)):.     
+0000a5d0: 2020 2020 2020 2069 6620 7365 6c66 2e5f         if self._
+0000a5e0: 6265 6e74 6f62 6f78 5f64 6174 613a 0a20  bentobox_data:. 
+0000a5f0: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+0000a600: 6f67 5f65 7272 6f72 280a 2020 2020 2020  og_error(.      
+0000a610: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
+0000a620: 6767 6572 2c0a 2020 2020 2020 2020 2020  gger,.          
+0000a630: 2020 2020 2020 2020 2020 2243 616e 6e6f            "Canno
+0000a640: 7420 6372 6561 7465 2076 6572 7469 6361  t create vertica
+0000a650: 6c20 696e 6469 6361 746f 7273 2069 6e20  l indicators in 
+0000a660: 6120 6265 6e74 6f62 6f78 222c 0a20 2020  a bentobox",.   
+0000a670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a680: 2052 756e 7469 6d65 4572 726f 722c 0a20   RuntimeError,. 
+0000a690: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+0000a6a0: 0a0a 2020 2020 2020 2020 2020 2020 7365  ..            se
+0000a6b0: 6c66 2e73 6574 5f62 656e 746f 626f 7828  lf.set_bentobox(
+0000a6c0: 636f 6c73 5f73 697a 653d 636f 6c73 5f73  cols_size=cols_s
+0000a6d0: 697a 652c 2072 6f77 735f 7369 7a65 3d72  ize, rows_size=r
+0000a6e0: 6f77 735f 7369 7a65 202a 206c 656e 5f64  ows_size * len_d
+0000a6f0: 6629 0a0a 2020 2020 2020 2020 2020 2020  f)..            
+0000a700: 2320 6669 7865 7864 2063 6f6c 735f 7369  # fixexd cols_si
+0000a710: 7a65 2066 6f72 2062 656e 746f 626f 7820  ze for bentobox 
+0000a720: 616e 6420 7661 7269 6162 6c65 2072 6f77  and variable row
+0000a730: 7320 7369 7a65 0a20 2020 2020 2020 2020  s size.         
+0000a740: 2020 2063 6f6c 735f 7369 7a65 203d 2032     cols_size = 2
+0000a750: 320a 2020 2020 2020 2020 2020 2020 726f  2.            ro
+0000a760: 7773 5f73 697a 6520 3d20 726f 7773 5f73  ws_size = rows_s
+0000a770: 697a 6520 2a20 3130 202d 2032 0a0a 2020  ize * 10 - 2..  
+0000a780: 2020 2020 2020 2020 2020 7061 6464 696e            paddin
+0000a790: 6720 3d20 2231 2c31 2c30 2c31 220a 2020  g = "1,1,0,1".  
+0000a7a0: 2020 2020 2020 2020 2020 6966 2069 7369            if isi
+0000a7b0: 6e73 7461 6e63 6528 7665 7274 6963 616c  nstance(vertical
+0000a7c0: 2c20 7374 7229 3a0a 2020 2020 2020 2020  , str):.        
+0000a7d0: 2020 2020 2020 2020 6874 6d6c 203d 2066          html = f
+0000a7e0: 223c 6835 2073 7479 6c65 3d27 666f 6e74  "<h5 style='font
+0000a7f0: 2d66 616d 696c 793a 2052 7562 696b 273e  -family: Rubik'>
+0000a800: 7b76 6572 7469 6361 6c7d 3c2f 6835 3e22  {vertical}</h5>"
+0000a810: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000a820: 2073 656c 662e 6874 6d6c 280a 2020 2020   self.html(.    
+0000a830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a840: 6874 6d6c 3d68 746d 6c2c 0a20 2020 2020  html=html,.     
+0000a850: 2020 2020 2020 2020 2020 2020 2020 206f                 o
+0000a860: 7264 6572 3d6f 7264 6572 2c0a 2020 2020  rder=order,.    
+0000a870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a880: 726f 7773 5f73 697a 653d 322c 0a20 2020  rows_size=2,.   
+0000a890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a8a0: 2063 6f6c 735f 7369 7a65 3d63 6f6c 735f   cols_size=cols_
+0000a8b0: 7369 7a65 2c0a 2020 2020 2020 2020 2020  size,.          
+0000a8c0: 2020 2020 2020 2020 2020 7061 6464 696e            paddin
+0000a8d0: 673d 7061 6464 696e 672c 0a20 2020 2020  g=padding,.     
+0000a8e0: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+0000a8f0: 2020 2020 2020 2020 2020 2020 206f 7264               ord
+0000a900: 6572 202b 3d20 310a 2020 2020 2020 2020  er += 1.        
+0000a910: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+0000a920: 2020 6265 6e74 6f62 6f78 5f64 6174 6120    bentobox_data 
+0000a930: 3d20 7365 6c66 2e5f 6265 6e74 6f62 6f78  = self._bentobox
+0000a940: 5f64 6174 610a 2020 2020 2020 2020 2020  _data.          
+0000a950: 2020 6966 2070 6164 6469 6e67 2069 7320    if padding is 
+0000a960: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0000a970: 2020 2020 2020 7061 6464 696e 6720 3d20        padding = 
+0000a980: 2230 2c30 2c30 2c30 220a 0a20 2020 2020  "0,0,0,0"..     
+0000a990: 2020 2020 2020 2070 6164 6469 6e67 203d         padding =
+0000a9a0: 2070 6164 6469 6e67 2e72 6570 6c61 6365   padding.replace
+0000a9b0: 2822 2022 2c20 2222 290a 0a20 2020 2020  (" ", "")..     
+0000a9c0: 2020 2020 2020 2072 656d 6169 6e69 6e67         remaining
+0000a9d0: 5f63 6f6c 7320 3d20 636f 6c73 5f73 697a  _cols = cols_siz
+0000a9e0: 6520 2520 6c65 6e5f 6466 0a0a 2020 2020  e % len_df..    
+0000a9f0: 2020 2020 2020 2020 6578 7472 615f 7061          extra_pa
+0000aa00: 6464 696e 6720 3d20 7265 6d61 696e 696e  dding = remainin
+0000aa10: 675f 636f 6c73 202f 2f20 320a 2020 2020  g_cols // 2.    
+0000aa20: 2020 2020 2020 2020 7061 6464 696e 675f          padding_
+0000aa30: 6c65 6674 5f69 6e74 203d 2069 6e74 2870  left_int = int(p
+0000aa40: 6164 6469 6e67 5b36 5d29 202b 2065 7874  adding[6]) + ext
+0000aa50: 7261 5f70 6164 6469 6e67 0a20 2020 2020  ra_padding.     
+0000aa60: 2020 2020 2020 2070 6164 6469 6e67 5f72         padding_r
+0000aa70: 6967 6874 5f69 6e74 203d 2069 6e74 2870  ight_int = int(p
+0000aa80: 6164 6469 6e67 5b32 5d29 202b 2065 7874  adding[2]) + ext
+0000aa90: 7261 5f70 6164 6469 6e67 202b 2072 656d  ra_padding + rem
+0000aaa0: 6169 6e69 6e67 5f63 6f6c 7320 2520 320a  aining_cols % 2.
+0000aab0: 0a20 2020 2020 2020 2020 2020 2070 6164  .            pad
+0000aac0: 6469 6e67 5f6c 6566 7420 3d20 6622 7b70  ding_left = f"{p
+0000aad0: 6164 6469 6e67 5b30 5d7d 2c30 2c7b 7061  adding[0]},0,{pa
+0000aae0: 6464 696e 675b 345d 7d2c 7b70 6164 6469  dding[4]},{paddi
+0000aaf0: 6e67 5f6c 6566 745f 696e 747d 220a 2020  ng_left_int}".  
+0000ab00: 2020 2020 2020 2020 2020 7061 6464 696e            paddin
+0000ab10: 675f 7269 6768 7420 3d20 6622 7b70 6164  g_right = f"{pad
+0000ab20: 6469 6e67 5b30 5d7d 2c7b 7061 6464 696e  ding[0]},{paddin
+0000ab30: 675f 7269 6768 745f 696e 747d 2c7b 7061  g_right_int},{pa
+0000ab40: 6464 696e 675b 345d 7d2c 7b69 6e74 2862  dding[4]},{int(b
+0000ab50: 6f6f 6c28 6265 6e74 6f62 6f78 5f64 6174  ool(bentobox_dat
+0000ab60: 6129 297d 220a 2020 2020 2020 2020 2020  a))}".          
+0000ab70: 2020 7061 6464 696e 675f 656c 7365 203d    padding_else =
+0000ab80: 2066 227b 7061 6464 696e 675b 305d 7d2c   f"{padding[0]},
+0000ab90: 302c 7b70 6164 6469 6e67 5b34 5d7d 2c7b  0,{padding[4]},{
+0000aba0: 696e 7428 626f 6f6c 2862 656e 746f 626f  int(bool(bentobo
+0000abb0: 785f 6461 7461 2929 7d22 0a0a 2020 2020  x_data))}"..    
+0000abc0: 2020 2020 2020 2020 636f 6c73 5f73 697a          cols_siz
+0000abd0: 6520 3d20 636f 6c73 5f73 697a 6520 2f2f  e = cols_size //
+0000abe0: 206c 656e 5f64 6620 2d20 696e 7428 626f   len_df - int(bo
+0000abf0: 6f6c 2862 656e 746f 626f 785f 6461 7461  ol(bentobox_data
+0000ac00: 2929 0a20 2020 2020 2020 2020 2020 2069  )).            i
+0000ac10: 6620 636f 6c73 5f73 697a 6520 3c20 323a  f cols_size < 2:
+0000ac20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000ac30: 206c 6f67 5f65 7272 6f72 280a 2020 2020   log_error(.    
+0000ac40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ac50: 6c6f 6767 6572 2c0a 2020 2020 2020 2020  logger,.        
+0000ac60: 2020 2020 2020 2020 2020 2020 6622 5468              f"Th
+0000ac70: 6520 6361 6c63 756c 6174 696f 6e20 6f66  e calculation of
+0000ac80: 2074 6865 2069 6e64 6976 6964 7561 6c20   the individual 
+0000ac90: 636f 6c73 5f73 697a 6520 666f 7220 6561  cols_size for ea
+0000aca0: 6368 2069 6e64 6963 6174 6f72 2022 0a20  ch indicator ". 
+0000acb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000acc0: 2020 2066 2269 7320 746f 6f20 736d 616c     f"is too smal
+0000acd0: 6c20 2863 6f6c 735f 7369 7a65 2f6c 656e  l (cols_size/len
+0000ace0: 2864 6629 293a 207b 636f 6c73 5f73 697a  (df)): {cols_siz
+0000acf0: 657d 222c 0a20 2020 2020 2020 2020 2020  e}",.           
+0000ad00: 2020 2020 2020 2020 2056 616c 7565 4572           ValueEr
+0000ad10: 726f 722c 0a20 2020 2020 2020 2020 2020  ror,.           
+0000ad20: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
+0000ad30: 6c61 7374 5f69 6e64 6578 203d 2064 662e  last_index = df.
+0000ad40: 696e 6465 785b 2d31 5d0a 2020 2020 2020  index[-1].      
+0000ad50: 2020 6669 7273 745f 696e 6465 7820 3d20    first_index = 
+0000ad60: 6466 2e69 6e64 6578 5b30 5d0a 0a20 2020  df.index[0]..   
+0000ad70: 2020 2020 2066 6f72 2069 6e64 6578 2c20       for index, 
+0000ad80: 6466 5f72 6f77 2069 6e20 6466 2e69 7465  df_row in df.ite
+0000ad90: 7272 6f77 7328 293a 0a20 2020 2020 2020  rrows():.       
+0000ada0: 2020 2020 2069 6620 6e6f 7420 7665 7274       if not vert
+0000adb0: 6963 616c 3a0a 2020 2020 2020 2020 2020  ical:.          
+0000adc0: 2020 2020 2020 6966 2069 6e64 6578 203d        if index =
+0000add0: 3d20 6669 7273 745f 696e 6465 7820 616e  = first_index an
+0000ade0: 6420 696e 6465 7820 3d3d 206c 6173 745f  d index == last_
+0000adf0: 696e 6465 783a 0a20 2020 2020 2020 2020  index:.         
+0000ae00: 2020 2020 2020 2020 2020 2070 6164 6469             paddi
+0000ae10: 6e67 203d 206f 7269 6769 6e61 6c5f 7061  ng = original_pa
+0000ae20: 6464 696e 670a 2020 2020 2020 2020 2020  dding.          
+0000ae30: 2020 2020 2020 656c 6966 2069 6e64 6578        elif index
+0000ae40: 203d 3d20 6669 7273 745f 696e 6465 783a   == first_index:
+0000ae50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000ae60: 2020 2020 2070 6164 6469 6e67 203d 2070       padding = p
+0000ae70: 6164 6469 6e67 5f6c 6566 740a 2020 2020  adding_left.    
+0000ae80: 2020 2020 2020 2020 2020 2020 656c 6966              elif
+0000ae90: 2069 6e64 6578 203d 3d20 6c61 7374 5f69   index == last_i
+0000aea0: 6e64 6578 3a0a 2020 2020 2020 2020 2020  ndex:.          
+0000aeb0: 2020 2020 2020 2020 2020 7061 6464 696e            paddin
+0000aec0: 6720 3d20 7061 6464 696e 675f 7269 6768  g = padding_righ
+0000aed0: 740a 2020 2020 2020 2020 2020 2020 2020  t.              
+0000aee0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+0000aef0: 2020 2020 2020 2020 2020 2020 7061 6464              padd
+0000af00: 696e 6720 3d20 7061 6464 696e 675f 656c  ing = padding_el
+0000af10: 7365 0a20 2020 2020 2020 2020 2020 2065  se.            e
+0000af20: 6c69 6620 280a 2020 2020 2020 2020 2020  lif (.          
+0000af30: 2020 2020 2020 696e 6465 7820 3d3d 206c        index == l
+0000af40: 6173 745f 696e 6465 780a 2020 2020 2020  ast_index.      
+0000af50: 2020 2020 2020 2020 2020 616e 6420 7665            and ve
+0000af60: 7274 6963 616c 0a20 2020 2020 2020 2020  rtical.         
+0000af70: 2020 2020 2020 2061 6e64 2028 6c65 6e5f         and (len_
+0000af80: 6466 203e 2031 206f 7220 6973 696e 7374  df > 1 or isinst
+0000af90: 616e 6365 2876 6572 7469 6361 6c2c 2073  ance(vertical, s
+0000afa0: 7472 2929 0a20 2020 2020 2020 2020 2020  tr)).           
+0000afb0: 2029 3a0a 2020 2020 2020 2020 2020 2020   ):.            
+0000afc0: 2020 2020 7061 6464 696e 6720 3d20 2231      padding = "1
+0000afd0: 2c31 2c31 2c31 220a 0a20 2020 2020 2020  ,1,1,1"..       
+0000afe0: 2020 2020 2069 6620 636f 6c6f 725f 6279       if color_by
+0000aff0: 5f76 616c 7565 2061 6e64 2022 636f 6c6f  _value and "colo
+0000b000: 7222 206e 6f74 2069 6e20 6466 5f72 6f77  r" not in df_row
+0000b010: 2061 6e64 2022 6963 6f6e 2220 6e6f 7420   and "icon" not 
+0000b020: 696e 2064 665f 726f 773a 0a20 2020 2020  in df_row:.     
+0000b030: 2020 2020 2020 2020 2020 2064 665f 726f             df_ro
+0000b040: 775b 2263 6f6c 6f72 225d 203d 2028 0a20  w["color"] = (. 
+0000b050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b060: 2020 2022 7375 6363 6573 7322 0a20 2020     "success".   
+0000b070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b080: 2069 6620 6466 5f72 6f77 5b22 7661 6c75   if df_row["valu
+0000b090: 6522 5d20 3e20 300a 2020 2020 2020 2020  e"] > 0.        
+0000b0a0: 2020 2020 2020 2020 2020 2020 656c 7365              else
+0000b0b0: 2022 6572 726f 7222 0a20 2020 2020 2020   "error".       
+0000b0c0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+0000b0d0: 6466 5f72 6f77 5b22 7661 6c75 6522 5d20  df_row["value"] 
+0000b0e0: 3c20 300a 2020 2020 2020 2020 2020 2020  < 0.            
+0000b0f0: 2020 2020 2020 2020 656c 7365 2022 6e65          else "ne
+0000b100: 7574 7261 6c22 0a20 2020 2020 2020 2020  utral".         
+0000b110: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+0000b120: 2020 2020 2020 2020 2064 665f 726f 775b           df_row[
+0000b130: 2269 636f 6e22 5d20 3d20 280a 2020 2020  "icon"] = (.    
 0000b140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b150: 2020 6966 2064 665f 726f 775b 2276 616c    if df_row["val
-0000b160: 7565 225d 203e 2030 0a20 2020 2020 2020  ue"] > 0.       
-0000b170: 2020 2020 2020 2020 2020 2020 2065 6c73               els
-0000b180: 6520 224c 696e 652f 6172 726f 772d 646f  e "Line/arrow-do
-0000b190: 776e 220a 2020 2020 2020 2020 2020 2020  wn".            
-0000b1a0: 2020 2020 2020 2020 6966 2064 665f 726f          if df_ro
-0000b1b0: 775b 2276 616c 7565 225d 203c 2030 0a20  w["value"] < 0. 
-0000b1c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b1d0: 2020 2065 6c73 6520 226e 6f6e 6522 0a20     else "none". 
-0000b1e0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-0000b1f0: 0a0a 2020 2020 2020 2020 2020 2020 7365  ..            se
-0000b200: 6c66 2e73 696e 676c 655f 696e 6469 6361  lf.single_indica
-0000b210: 746f 7228 0a20 2020 2020 2020 2020 2020  tor(.           
-0000b220: 2020 2020 2064 6174 613d 6466 5f72 6f77       data=df_row
-0000b230: 2e64 726f 706e 6128 292e 746f 5f64 6963  .dropna().to_dic
-0000b240: 7428 292c 0a20 2020 2020 2020 2020 2020  t(),.           
-0000b250: 2020 2020 206f 7264 6572 3d6f 7264 6572       order=order
-0000b260: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000b270: 2020 636f 6c73 5f73 697a 653d 636f 6c73    cols_size=cols
-0000b280: 5f73 697a 652c 0a20 2020 2020 2020 2020  _size,.         
-0000b290: 2020 2020 2020 2072 6f77 735f 7369 7a65         rows_size
-0000b2a0: 3d72 6f77 735f 7369 7a65 2c0a 2020 2020  =rows_size,.    
-0000b2b0: 2020 2020 2020 2020 2020 2020 7061 6464              padd
-0000b2c0: 696e 673d 7061 6464 696e 672c 0a20 2020  ing=padding,.   
-0000b2d0: 2020 2020 2020 2020 2029 0a0a 2020 2020           )..    
-0000b2e0: 2020 2020 2020 2020 6966 2069 7369 6e73          if isins
-0000b2f0: 7461 6e63 6528 6f72 6465 722c 2069 6e74  tance(order, int
-0000b300: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-0000b310: 2020 206f 7264 6572 202b 3d20 310a 0a20     order += 1.. 
-0000b320: 2020 2020 2020 2069 6620 7665 7274 6963         if vertic
-0000b330: 616c 3a0a 2020 2020 2020 2020 2020 2020  al:.            
-0000b340: 7365 6c66 2e70 6f70 5f6f 7574 5f6f 665f  self.pop_out_of_
-0000b350: 6265 6e74 6f62 6f78 2829 0a0a 2020 2020  bentobox()..    
-0000b360: 2020 2020 7265 7475 726e 206f 7264 6572      return order
-0000b370: 0a0a 2020 2020 6173 796e 6320 6465 6620  ..    async def 
-0000b380: 5f62 7574 746f 6e28 0a20 2020 2020 2020  _button(.       
-0000b390: 2073 656c 662c 0a20 2020 2020 2020 206c   self,.        l
-0000b3a0: 6162 656c 3a20 7374 722c 0a20 2020 2020  abel: str,.     
-0000b3b0: 2020 206f 7264 6572 3a20 696e 742c 0a20     order: int,. 
-0000b3c0: 2020 2020 2020 2072 6f77 735f 7369 7a65         rows_size
-0000b3d0: 3a20 4f70 7469 6f6e 616c 5b69 6e74 5d20  : Optional[int] 
-0000b3e0: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-0000b3f0: 636f 6c73 5f73 697a 653a 204f 7074 696f  cols_size: Optio
-0000b400: 6e61 6c5b 696e 745d 203d 204e 6f6e 652c  nal[int] = None,
-0000b410: 0a20 2020 2020 2020 2061 6c69 676e 3a20  .        align: 
-0000b420: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
-0000b430: 2273 7472 6574 6368 222c 0a20 2020 2020  "stretch",.     
-0000b440: 2020 2070 6164 6469 6e67 3a20 4f70 7469     padding: Opti
-0000b450: 6f6e 616c 5b73 7472 5d20 3d20 4e6f 6e65  onal[str] = None
-0000b460: 2c0a 2020 2020 2020 2020 6f6e 5f63 6c69  ,.        on_cli
-0000b470: 636b 5f65 7665 6e74 733a 204f 7074 696f  ck_events: Optio
-0000b480: 6e61 6c5b 556e 696f 6e5b 6c69 7374 5b64  nal[Union[list[d
-0000b490: 6963 745d 2c20 6469 6374 5d5d 203d 204e  ict], dict]] = N
-0000b4a0: 6f6e 652c 0a20 2020 2029 3a0a 2020 2020  one,.    ):.    
-0000b4b0: 2020 2020 2222 2243 7265 6174 6520 6120      """Create a 
-0000b4c0: 6275 7474 6f6e 2069 6e20 7468 6520 6461  button in the da
-0000b4d0: 7368 626f 6172 642e 2222 220a 2020 2020  shboard.""".    
-0000b4e0: 2020 2020 6966 206e 6f74 206f 6e5f 636c      if not on_cl
-0000b4f0: 6963 6b5f 6576 656e 7473 3a0a 2020 2020  ick_events:.    
-0000b500: 2020 2020 2020 2020 6f6e 5f63 6c69 636b          on_click
-0000b510: 5f65 7665 6e74 7320 3d20 5b5d 0a20 2020  _events = [].   
-0000b520: 2020 2020 2065 6c69 6620 6973 696e 7374       elif isinst
-0000b530: 616e 6365 286f 6e5f 636c 6963 6b5f 6576  ance(on_click_ev
-0000b540: 656e 7473 2c20 6469 6374 293a 0a20 2020  ents, dict):.   
-0000b550: 2020 2020 2020 2020 206f 6e5f 636c 6963           on_clic
-0000b560: 6b5f 6576 656e 7473 203d 205b 6f6e 5f63  k_events = [on_c
-0000b570: 6c69 636b 5f65 7665 6e74 735d 0a0a 2020  lick_events]..  
-0000b580: 2020 2020 2020 6177 6169 7420 7365 6c66        await self
-0000b590: 2e5f 6372 6561 7465 5f63 6861 7274 280a  ._create_chart(.
-0000b5a0: 2020 2020 2020 2020 2020 2020 6368 6172              char
-0000b5b0: 745f 636c 6173 733d 4275 7474 6f6e 2c0a  t_class=Button,.
-0000b5c0: 2020 2020 2020 2020 2020 2020 6f72 6465              orde
-0000b5d0: 723d 6f72 6465 722c 0a20 2020 2020 2020  r=order,.       
-0000b5e0: 2020 2020 2073 697a 6550 6164 6469 6e67       sizePadding
-0000b5f0: 3d70 6164 6469 6e67 2c0a 2020 2020 2020  =padding,.      
-0000b600: 2020 2020 2020 7369 7a65 526f 7773 3d72        sizeRows=r
-0000b610: 6f77 735f 7369 7a65 2c0a 2020 2020 2020  ows_size,.      
-0000b620: 2020 2020 2020 7369 7a65 436f 6c75 6d6e        sizeColumn
-0000b630: 733d 636f 6c73 5f73 697a 652c 0a20 2020  s=cols_size,.   
-0000b640: 2020 2020 2020 2020 2070 726f 7065 7274           propert
-0000b650: 6965 733d 6469 6374 280a 2020 2020 2020  ies=dict(.      
-0000b660: 2020 2020 2020 2020 2020 7465 7874 3d6c            text=l
-0000b670: 6162 656c 2c20 616c 6967 6e3d 616c 6967  abel, align=alig
-0000b680: 6e2c 2065 7665 6e74 733d 6469 6374 286f  n, events=dict(o
-0000b690: 6e43 6c69 636b 3d6f 6e5f 636c 6963 6b5f  nClick=on_click_
-0000b6a0: 6576 656e 7473 290a 2020 2020 2020 2020  events).        
-0000b6b0: 2020 2020 292c 0a20 2020 2020 2020 2029      ),.        )
-0000b6c0: 0a0a 2020 2020 4061 6464 5f74 6f5f 6765  ..    @add_to_ge
-0000b6d0: 6e65 7261 6c5f 6173 796e 635f 6772 6f75  neral_async_grou
-0000b6e0: 700a 2020 2020 6173 796e 6320 6465 6620  p.    async def 
-0000b6f0: 6275 7474 6f6e 280a 2020 2020 2020 2020  button(.        
-0000b700: 7365 6c66 2c0a 2020 2020 2020 2020 6c61  self,.        la
-0000b710: 6265 6c3a 2073 7472 2c0a 2020 2020 2020  bel: str,.      
-0000b720: 2020 6f72 6465 723a 2069 6e74 2c0a 2020    order: int,.  
-0000b730: 2020 2020 2020 726f 7773 5f73 697a 653a        rows_size:
-0000b740: 204f 7074 696f 6e61 6c5b 696e 745d 203d   Optional[int] =
-0000b750: 2031 2c0a 2020 2020 2020 2020 636f 6c73   1,.        cols
-0000b760: 5f73 697a 653a 2069 6e74 203d 2032 2c0a  _size: int = 2,.
-0000b770: 2020 2020 2020 2020 616c 6967 6e3a 204f          align: O
-0000b780: 7074 696f 6e61 6c5b 7374 725d 203d 2022  ptional[str] = "
-0000b790: 7374 7265 7463 6822 2c0a 2020 2020 2020  stretch",.      
-0000b7a0: 2020 7061 6464 696e 673a 204f 7074 696f    padding: Optio
-0000b7b0: 6e61 6c5b 7374 725d 203d 204e 6f6e 652c  nal[str] = None,
-0000b7c0: 0a20 2020 2020 2020 206f 6e5f 636c 6963  .        on_clic
-0000b7d0: 6b5f 6576 656e 7473 3a20 4f70 7469 6f6e  k_events: Option
-0000b7e0: 616c 5b55 6e69 6f6e 5b6c 6973 745b 6469  al[Union[list[di
-0000b7f0: 6374 5d2c 2064 6963 745d 5d20 3d20 4e6f  ct], dict]] = No
-0000b800: 6e65 2c0a 2020 2020 293a 0a20 2020 2020  ne,.    ):.     
-0000b810: 2020 2022 2222 4372 6561 7465 2061 2062     """Create a b
-0000b820: 7574 746f 6e20 696e 2074 6865 2064 6173  utton in the das
-0000b830: 6862 6f61 7264 2e22 2222 0a20 2020 2020  hboard.""".     
-0000b840: 2020 2061 7761 6974 2073 656c 662e 5f62     await self._b
-0000b850: 7574 746f 6e28 0a20 2020 2020 2020 2020  utton(.         
-0000b860: 2020 206c 6162 656c 3d6c 6162 656c 2c0a     label=label,.
-0000b870: 2020 2020 2020 2020 2020 2020 6f72 6465              orde
-0000b880: 723d 6f72 6465 722c 0a20 2020 2020 2020  r=order,.       
-0000b890: 2020 2020 2072 6f77 735f 7369 7a65 3d72       rows_size=r
-0000b8a0: 6f77 735f 7369 7a65 2c0a 2020 2020 2020  ows_size,.      
-0000b8b0: 2020 2020 2020 636f 6c73 5f73 697a 653d        cols_size=
-0000b8c0: 636f 6c73 5f73 697a 652c 0a20 2020 2020  cols_size,.     
-0000b8d0: 2020 2020 2020 2061 6c69 676e 3d61 6c69         align=ali
-0000b8e0: 676e 2c0a 2020 2020 2020 2020 2020 2020  gn,.            
-0000b8f0: 7061 6464 696e 673d 7061 6464 696e 672c  padding=padding,
-0000b900: 0a20 2020 2020 2020 2020 2020 206f 6e5f  .            on_
-0000b910: 636c 6963 6b5f 6576 656e 7473 3d6f 6e5f  click_events=on_
-0000b920: 636c 6963 6b5f 6576 656e 7473 2c0a 2020  click_events,.  
-0000b930: 2020 2020 2020 290a 0a20 2020 2040 6164        )..    @ad
-0000b940: 645f 746f 5f67 656e 6572 616c 5f61 7379  d_to_general_asy
-0000b950: 6e63 5f67 726f 7570 0a20 2020 2061 7379  nc_group.    asy
-0000b960: 6e63 2064 6566 206d 6f64 616c 5f62 7574  nc def modal_but
-0000b970: 746f 6e28 0a20 2020 2020 2020 2073 656c  ton(.        sel
-0000b980: 662c 0a20 2020 2020 2020 206c 6162 656c  f,.        label
-0000b990: 3a20 7374 722c 0a20 2020 2020 2020 206f  : str,.        o
-0000b9a0: 7264 6572 3a20 696e 742c 0a20 2020 2020  rder: int,.     
-0000b9b0: 2020 206d 6f64 616c 3a20 7374 722c 0a20     modal: str,. 
-0000b9c0: 2020 2020 2020 2072 6f77 735f 7369 7a65         rows_size
-0000b9d0: 3a20 4f70 7469 6f6e 616c 5b69 6e74 5d20  : Optional[int] 
-0000b9e0: 3d20 312c 0a20 2020 2020 2020 2063 6f6c  = 1,.        col
-0000b9f0: 735f 7369 7a65 3a20 696e 7420 3d20 322c  s_size: int = 2,
-0000ba00: 0a20 2020 2020 2020 2061 6c69 676e 3a20  .        align: 
-0000ba10: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
-0000ba20: 2273 7472 6574 6368 222c 0a20 2020 2020  "stretch",.     
-0000ba30: 2020 2070 6164 6469 6e67 3a20 4f70 7469     padding: Opti
-0000ba40: 6f6e 616c 5b73 7472 5d20 3d20 4e6f 6e65  onal[str] = None
-0000ba50: 2c0a 2020 2020 293a 0a20 2020 2020 2020  ,.    ):.       
-0000ba60: 2022 2222 0a20 2020 2020 2020 2043 7265   """.        Cre
-0000ba70: 6174 6520 6120 6275 7474 6f6e 2069 6e20  ate a button in 
-0000ba80: 7468 6520 6461 7368 626f 6172 6420 7468  the dashboard th
-0000ba90: 6174 206f 7065 6e73 2061 206d 6f64 616c  at opens a modal
-0000baa0: 2e0a 2020 2020 2020 2020 3a70 6172 616d  ..        :param
-0000bab0: 206c 6162 656c 3a20 7468 6520 6c61 6265   label: the labe
-0000bac0: 6c20 6f66 2074 6865 2062 7574 746f 6e0a  l of the button.
-0000bad0: 2020 2020 2020 2020 3a70 6172 616d 206f          :param o
-0000bae0: 7264 6572 3a20 7468 6520 6f72 6465 7220  rder: the order 
-0000baf0: 6f66 2074 6865 2062 7574 746f 6e0a 2020  of the button.  
-0000bb00: 2020 2020 2020 3a70 6172 616d 206d 6f64        :param mod
-0000bb10: 616c 3a20 7468 6520 6e61 6d65 206f 6620  al: the name of 
-0000bb20: 7468 6520 6d6f 6461 6c0a 2020 2020 2020  the modal.      
-0000bb30: 2020 3a70 6172 616d 2072 6f77 735f 7369    :param rows_si
-0000bb40: 7a65 3a20 7468 6520 7369 7a65 206f 6620  ze: the size of 
-0000bb50: 7468 6520 726f 7773 2069 6e20 7468 6520  the rows in the 
-0000bb60: 6275 7474 6f6e 0a20 2020 2020 2020 203a  button.        :
-0000bb70: 7061 7261 6d20 636f 6c73 5f73 697a 653a  param cols_size:
-0000bb80: 2074 6865 2073 697a 6520 6f66 2074 6865   the size of the
-0000bb90: 2063 6f6c 756d 6e73 2069 6e20 7468 6520   columns in the 
-0000bba0: 6275 7474 6f6e 0a20 2020 2020 2020 203a  button.        :
-0000bbb0: 7061 7261 6d20 616c 6967 6e3a 2074 6865  param align: the
-0000bbc0: 2061 6c69 676e 6d65 6e74 206f 6620 7468   alignment of th
-0000bbd0: 6520 6275 7474 6f6e 0a20 2020 2020 2020  e button.       
-0000bbe0: 203a 7061 7261 6d20 7061 6464 696e 673a   :param padding:
-0000bbf0: 2074 6865 2070 6164 6469 6e67 206f 6620   the padding of 
-0000bc00: 7468 6520 6275 7474 6f6e 0a20 2020 2020  the button.     
-0000bc10: 2020 2022 2222 0a20 2020 2020 2020 206d     """.        m
-0000bc20: 6f64 616c 5f69 6420 3d20 2861 7761 6974  odal_id = (await
-0000bc30: 2073 656c 662e 5f67 6574 5f6d 6f64 616c   self._get_modal
-0000bc40: 286d 6f64 616c 2929 5b22 6964 225d 0a0a  (modal))["id"]..
-0000bc50: 2020 2020 2020 2020 6177 6169 7420 7365          await se
-0000bc60: 6c66 2e5f 6275 7474 6f6e 280a 2020 2020  lf._button(.    
-0000bc70: 2020 2020 2020 2020 6c61 6265 6c3d 6c61          label=la
-0000bc80: 6265 6c2c 0a20 2020 2020 2020 2020 2020  bel,.           
-0000bc90: 206f 7264 6572 3d6f 7264 6572 2c0a 2020   order=order,.  
-0000bca0: 2020 2020 2020 2020 2020 7061 6464 696e            paddin
-0000bcb0: 673d 7061 6464 696e 672c 0a20 2020 2020  g=padding,.     
-0000bcc0: 2020 2020 2020 2072 6f77 735f 7369 7a65         rows_size
-0000bcd0: 3d72 6f77 735f 7369 7a65 2c0a 2020 2020  =rows_size,.    
-0000bce0: 2020 2020 2020 2020 636f 6c73 5f73 697a          cols_siz
-0000bcf0: 653d 636f 6c73 5f73 697a 652c 0a20 2020  e=cols_size,.   
-0000bd00: 2020 2020 2020 2020 2061 6c69 676e 3d61           align=a
-0000bd10: 6c69 676e 2c0a 2020 2020 2020 2020 2020  lign,.          
-0000bd20: 2020 6f6e 5f63 6c69 636b 5f65 7665 6e74    on_click_event
-0000bd30: 733d 5b0a 2020 2020 2020 2020 2020 2020  s=[.            
-0000bd40: 2020 2020 6469 6374 280a 2020 2020 2020      dict(.      
-0000bd50: 2020 2020 2020 2020 2020 2020 2020 6163                ac
-0000bd60: 7469 6f6e 3d22 6f70 656e 4d6f 6461 6c22  tion="openModal"
-0000bd70: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000bd80: 2020 2020 2020 7061 7261 6d73 3d64 6963        params=dic
-0000bd90: 7428 0a20 2020 2020 2020 2020 2020 2020  t(.             
-0000bda0: 2020 2020 2020 2020 2020 206d 6f64 616c             modal
-0000bdb0: 4964 3d6d 6f64 616c 5f69 642c 0a20 2020  Id=modal_id,.   
-0000bdc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bdd0: 2029 2c0a 2020 2020 2020 2020 2020 2020   ),.            
-0000bde0: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-0000bdf0: 2020 5d2c 0a20 2020 2020 2020 2029 0a0a    ],.        )..
-0000be00: 2020 2020 4061 6464 5f74 6f5f 6765 6e65      @add_to_gene
-0000be10: 7261 6c5f 6173 796e 635f 6772 6f75 700a  ral_async_group.
-0000be20: 2020 2020 6173 796e 6320 6465 6620 6163      async def ac
-0000be30: 7469 7669 7479 5f62 7574 746f 6e28 0a20  tivity_button(. 
-0000be40: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
-0000be50: 2020 2020 206c 6162 656c 3a20 7374 722c       label: str,
-0000be60: 0a20 2020 2020 2020 206f 7264 6572 3a20  .        order: 
-0000be70: 696e 742c 0a20 2020 2020 2020 2072 6f77  int,.        row
-0000be80: 735f 7369 7a65 3a20 4f70 7469 6f6e 616c  s_size: Optional
-0000be90: 5b69 6e74 5d20 3d20 312c 0a20 2020 2020  [int] = 1,.     
-0000bea0: 2020 2063 6f6c 735f 7369 7a65 3a20 696e     cols_size: in
-0000beb0: 7420 3d20 322c 0a20 2020 2020 2020 2061  t = 2,.        a
-0000bec0: 6c69 676e 3a20 4f70 7469 6f6e 616c 5b73  lign: Optional[s
-0000bed0: 7472 5d20 3d20 2273 7472 6574 6368 222c  tr] = "stretch",
-0000bee0: 0a20 2020 2020 2020 2070 6164 6469 6e67  .        padding
-0000bef0: 3a20 4f70 7469 6f6e 616c 5b73 7472 5d20  : Optional[str] 
-0000bf00: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-0000bf10: 6163 7469 7669 7479 5f69 643a 204f 7074  activity_id: Opt
-0000bf20: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
-0000bf30: 652c 0a20 2020 2020 2020 2061 6374 6976  e,.        activ
-0000bf40: 6974 795f 6e61 6d65 3a20 4f70 7469 6f6e  ity_name: Option
-0000bf50: 616c 5b73 7472 5d20 3d20 4e6f 6e65 2c0a  al[str] = None,.
-0000bf60: 2020 2020 293a 0a20 2020 2020 2020 2022      ):.        "
-0000bf70: 2222 0a20 2020 2020 2020 2043 7265 6174  "".        Creat
-0000bf80: 6520 6120 6275 7474 6f6e 2069 6e20 7468  e a button in th
-0000bf90: 6520 6461 7368 626f 6172 6420 7468 6174  e dashboard that
-0000bfa0: 2065 7865 6375 7465 7320 616e 2061 6374   executes an act
-0000bfb0: 6976 6974 792e 0a20 2020 2020 2020 203a  ivity..        :
-0000bfc0: 7061 7261 6d20 6c61 6265 6c3a 2074 6865  param label: the
-0000bfd0: 206c 6162 656c 206f 6620 7468 6520 6275   label of the bu
-0000bfe0: 7474 6f6e 0a20 2020 2020 2020 203a 7061  tton.        :pa
-0000bff0: 7261 6d20 6f72 6465 723a 2074 6865 206f  ram order: the o
-0000c000: 7264 6572 206f 6620 7468 6520 6275 7474  rder of the butt
-0000c010: 6f6e 0a20 2020 2020 2020 203a 7061 7261  on.        :para
-0000c020: 6d20 726f 7773 5f73 697a 653a 2074 6865  m rows_size: the
-0000c030: 2073 697a 6520 6f66 2074 6865 2072 6f77   size of the row
-0000c040: 7320 696e 2074 6865 2062 7574 746f 6e0a  s in the button.
-0000c050: 2020 2020 2020 2020 3a70 6172 616d 2063          :param c
-0000c060: 6f6c 735f 7369 7a65 3a20 7468 6520 7369  ols_size: the si
-0000c070: 7a65 206f 6620 7468 6520 636f 6c75 6d6e  ze of the column
-0000c080: 7320 696e 2074 6865 2062 7574 746f 6e0a  s in the button.
-0000c090: 2020 2020 2020 2020 3a70 6172 616d 2061          :param a
-0000c0a0: 6c69 676e 3a20 7468 6520 616c 6967 6e6d  lign: the alignm
-0000c0b0: 656e 7420 6f66 2074 6865 2062 7574 746f  ent of the butto
-0000c0c0: 6e0a 2020 2020 2020 2020 3a70 6172 616d  n.        :param
-0000c0d0: 2070 6164 6469 6e67 3a20 7468 6520 7061   padding: the pa
-0000c0e0: 6464 696e 6720 6f66 2074 6865 2062 7574  dding of the but
-0000c0f0: 746f 6e0a 2020 2020 2020 2020 3a70 6172  ton.        :par
-0000c100: 616d 2061 6374 6976 6974 795f 6964 3a20  am activity_id: 
-0000c110: 7468 6520 6964 206f 6620 7468 6520 6163  the id of the ac
-0000c120: 7469 7669 7479 0a20 2020 2020 2020 203a  tivity.        :
-0000c130: 7061 7261 6d20 6163 7469 7669 7479 5f6e  param activity_n
-0000c140: 616d 653a 2074 6865 206e 616d 6520 6f66  ame: the name of
-0000c150: 2074 6865 2061 6374 6976 6974 790a 2020   the activity.  
-0000c160: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-0000c170: 2020 6163 7469 7669 7479 5f69 6420 3d20    activity_id = 
-0000c180: 2861 7761 6974 2073 656c 662e 5f61 7070  (await self._app
-0000c190: 2e67 6574 5f61 6374 6976 6974 7928 6163  .get_activity(ac
-0000c1a0: 7469 7669 7479 5f69 642c 2061 6374 6976  tivity_id, activ
-0000c1b0: 6974 795f 6e61 6d65 2929 5b22 6964 225d  ity_name))["id"]
-0000c1c0: 0a0a 2020 2020 2020 2020 6177 6169 7420  ..        await 
-0000c1d0: 7365 6c66 2e5f 6275 7474 6f6e 280a 2020  self._button(.  
-0000c1e0: 2020 2020 2020 2020 2020 6c61 6265 6c3d            label=
-0000c1f0: 6c61 6265 6c2c 0a20 2020 2020 2020 2020  label,.         
-0000c200: 2020 206f 7264 6572 3d6f 7264 6572 2c0a     order=order,.
-0000c210: 2020 2020 2020 2020 2020 2020 7061 6464              padd
-0000c220: 696e 673d 7061 6464 696e 672c 0a20 2020  ing=padding,.   
-0000c230: 2020 2020 2020 2020 2072 6f77 735f 7369           rows_si
-0000c240: 7a65 3d72 6f77 735f 7369 7a65 2c0a 2020  ze=rows_size,.  
-0000c250: 2020 2020 2020 2020 2020 636f 6c73 5f73            cols_s
-0000c260: 697a 653d 636f 6c73 5f73 697a 652c 0a20  ize=cols_size,. 
-0000c270: 2020 2020 2020 2020 2020 2061 6c69 676e             align
-0000c280: 3d61 6c69 676e 2c0a 2020 2020 2020 2020  =align,.        
-0000c290: 2020 2020 6f6e 5f63 6c69 636b 5f65 7665      on_click_eve
-0000c2a0: 6e74 733d 5b0a 2020 2020 2020 2020 2020  nts=[.          
-0000c2b0: 2020 2020 2020 6469 6374 280a 2020 2020        dict(.    
-0000c2c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c2d0: 6163 7469 6f6e 3d22 7275 6e41 6374 6976  action="runActiv
-0000c2e0: 6974 7922 2c0a 2020 2020 2020 2020 2020  ity",.          
-0000c2f0: 2020 2020 2020 2020 2020 7061 7261 6d73            params
-0000c300: 3d64 6963 7428 0a20 2020 2020 2020 2020  =dict(.         
-0000c310: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-0000c320: 6374 6976 6974 7949 643d 6163 7469 7669  ctivityId=activi
-0000c330: 7479 5f69 642c 0a20 2020 2020 2020 2020  ty_id,.         
-0000c340: 2020 2020 2020 2020 2020 2029 2c0a 2020             ),.  
-0000c350: 2020 2020 2020 2020 2020 2020 2020 290a                ).
-0000c360: 2020 2020 2020 2020 2020 2020 5d2c 0a20              ],. 
-0000c370: 2020 2020 2020 2029 0a0a 2020 2020 4061         )..    @a
-0000c380: 6464 5f74 6f5f 6765 6e65 7261 6c5f 6173  dd_to_general_as
-0000c390: 796e 635f 6772 6f75 700a 2020 2020 6173  ync_group.    as
-0000c3a0: 796e 6320 6465 6620 6163 7469 6f6e 5f62  ync def action_b
-0000c3b0: 7574 746f 6e28 0a20 2020 2020 2020 2073  utton(.        s
-0000c3c0: 656c 662c 0a20 2020 2020 2020 206c 6162  elf,.        lab
-0000c3d0: 656c 3a20 7374 722c 0a20 2020 2020 2020  el: str,.       
-0000c3e0: 206f 7264 6572 3a20 696e 742c 0a20 2020   order: int,.   
-0000c3f0: 2020 2020 2061 6374 696f 6e5f 6964 3a20       action_id: 
-0000c400: 7374 722c 0a20 2020 2020 2020 2072 6f77  str,.        row
-0000c410: 735f 7369 7a65 3a20 4f70 7469 6f6e 616c  s_size: Optional
-0000c420: 5b69 6e74 5d20 3d20 312c 0a20 2020 2020  [int] = 1,.     
-0000c430: 2020 2063 6f6c 735f 7369 7a65 3a20 696e     cols_size: in
-0000c440: 7420 3d20 322c 0a20 2020 2020 2020 2061  t = 2,.        a
-0000c450: 6c69 676e 3a20 4f70 7469 6f6e 616c 5b73  lign: Optional[s
-0000c460: 7472 5d20 3d20 2273 7472 6574 6368 222c  tr] = "stretch",
-0000c470: 0a20 2020 2020 2020 2070 6164 6469 6e67  .        padding
-0000c480: 3a20 4f70 7469 6f6e 616c 5b73 7472 5d20  : Optional[str] 
-0000c490: 3d20 4e6f 6e65 2c0a 2020 2020 293a 0a20  = None,.    ):. 
-0000c4a0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-0000c4b0: 2020 2043 7265 6174 6520 6120 6275 7474     Create a butt
-0000c4c0: 6f6e 2069 6e20 7468 6520 6461 7368 626f  on in the dashbo
-0000c4d0: 6172 6420 7468 6174 2065 7865 6375 7465  ard that execute
-0000c4e0: 7320 616e 2061 6374 696f 6e2e 0a20 2020  s an action..   
-0000c4f0: 2020 2020 203a 7061 7261 6d20 6c61 6265       :param labe
-0000c500: 6c3a 2074 6865 206c 6162 656c 206f 6620  l: the label of 
-0000c510: 7468 6520 6275 7474 6f6e 0a20 2020 2020  the button.     
-0000c520: 2020 203a 7061 7261 6d20 6f72 6465 723a     :param order:
-0000c530: 2074 6865 206f 7264 6572 206f 6620 7468   the order of th
-0000c540: 6520 6275 7474 6f6e 0a20 2020 2020 2020  e button.       
-0000c550: 203a 7061 7261 6d20 6163 7469 6f6e 5f69   :param action_i
-0000c560: 643a 2074 6865 2069 6420 6f66 2074 6865  d: the id of the
-0000c570: 2061 6374 696f 6e0a 2020 2020 2020 2020   action.        
-0000c580: 3a70 6172 616d 2072 6f77 735f 7369 7a65  :param rows_size
-0000c590: 3a20 7468 6520 7369 7a65 206f 6620 7468  : the size of th
-0000c5a0: 6520 726f 7773 2069 6e20 7468 6520 6275  e rows in the bu
-0000c5b0: 7474 6f6e 0a20 2020 2020 2020 203a 7061  tton.        :pa
-0000c5c0: 7261 6d20 636f 6c73 5f73 697a 653a 2074  ram cols_size: t
-0000c5d0: 6865 2073 697a 6520 6f66 2074 6865 2063  he size of the c
-0000c5e0: 6f6c 756d 6e73 2069 6e20 7468 6520 6275  olumns in the bu
-0000c5f0: 7474 6f6e 0a20 2020 2020 2020 203a 7061  tton.        :pa
-0000c600: 7261 6d20 616c 6967 6e3a 2074 6865 2061  ram align: the a
-0000c610: 6c69 676e 6d65 6e74 206f 6620 7468 6520  lignment of the 
-0000c620: 6275 7474 6f6e 0a20 2020 2020 2020 203a  button.        :
-0000c630: 7061 7261 6d20 7061 6464 696e 673a 2074  param padding: t
-0000c640: 6865 2070 6164 6469 6e67 206f 6620 7468  he padding of th
-0000c650: 6520 6275 7474 6f6e 0a20 2020 2020 2020  e button.       
-0000c660: 2022 2222 0a20 2020 2020 2020 2061 7761   """.        awa
-0000c670: 6974 2073 656c 662e 5f62 7574 746f 6e28  it self._button(
-0000c680: 0a20 2020 2020 2020 2020 2020 206c 6162  .            lab
-0000c690: 656c 3d6c 6162 656c 2c0a 2020 2020 2020  el=label,.      
-0000c6a0: 2020 2020 2020 6f72 6465 723d 6f72 6465        order=orde
-0000c6b0: 722c 0a20 2020 2020 2020 2020 2020 2070  r,.            p
-0000c6c0: 6164 6469 6e67 3d70 6164 6469 6e67 2c0a  adding=padding,.
-0000c6d0: 2020 2020 2020 2020 2020 2020 726f 7773              rows
-0000c6e0: 5f73 697a 653d 726f 7773 5f73 697a 652c  _size=rows_size,
-0000c6f0: 0a20 2020 2020 2020 2020 2020 2063 6f6c  .            col
-0000c700: 735f 7369 7a65 3d63 6f6c 735f 7369 7a65  s_size=cols_size
-0000c710: 2c0a 2020 2020 2020 2020 2020 2020 616c  ,.            al
-0000c720: 6967 6e3d 616c 6967 6e2c 0a20 2020 2020  ign=align,.     
-0000c730: 2020 2020 2020 206f 6e5f 636c 6963 6b5f         on_click_
-0000c740: 6576 656e 7473 3d5b 0a20 2020 2020 2020  events=[.       
-0000c750: 2020 2020 2020 2020 2064 6963 7428 0a20           dict(. 
-0000c760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c770: 2020 2061 6374 696f 6e3d 2272 756e 4163     action="runAc
-0000c780: 7469 6f6e 222c 0a20 2020 2020 2020 2020  tion",.         
-0000c790: 2020 2020 2020 2020 2020 2070 6172 616d             param
-0000c7a0: 733d 6469 6374 280a 2020 2020 2020 2020  s=dict(.        
-0000c7b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c7c0: 6163 7469 6f6e 4964 3d61 6374 696f 6e5f  actionId=action_
-0000c7d0: 6964 2c0a 2020 2020 2020 2020 2020 2020  id,.            
-0000c7e0: 2020 2020 2020 2020 292c 0a20 2020 2020          ),.     
-0000c7f0: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-0000c800: 2020 2020 2020 2020 205d 2c0a 2020 2020           ],.    
-0000c810: 2020 2020 290a 0a20 2020 2040 6164 645f      )..    @add_
-0000c820: 746f 5f67 656e 6572 616c 5f61 7379 6e63  to_general_async
-0000c830: 5f67 726f 7570 0a20 2020 2061 7379 6e63  _group.    async
-0000c840: 2064 6566 2074 6162 6c65 280a 2020 2020   def table(.    
-0000c850: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
-0000c860: 2020 6f72 6465 723a 2069 6e74 2c0a 2020    order: int,.  
-0000c870: 2020 2020 2020 6461 7461 3a20 556e 696f        data: Unio
-0000c880: 6e5b 7374 722c 2070 642e 4461 7461 4672  n[str, pd.DataFr
-0000c890: 616d 652c 206c 6973 745b 6469 6374 5d2c  ame, list[dict],
-0000c8a0: 2064 6963 745d 2c0a 2020 2020 2020 2020   dict],.        
-0000c8b0: 636f 6c75 6d6e 733a 204f 7074 696f 6e61  columns: Optiona
-0000c8c0: 6c5b 6c69 7374 5b73 7472 5d5d 203d 204e  l[list[str]] = N
-0000c8d0: 6f6e 652c 0a20 2020 2020 2020 2063 6f6c  one,.        col
-0000c8e0: 756d 6e73 5f62 7574 746f 6e3a 2062 6f6f  umns_button: boo
-0000c8f0: 6c20 3d20 5472 7565 2c0a 2020 2020 2020  l = True,.      
-0000c900: 2020 6669 6c74 6572 733a 2062 6f6f 6c20    filters: bool 
-0000c910: 3d20 5472 7565 2c0a 2020 2020 2020 2020  = True,.        
-0000c920: 6578 706f 7274 5f74 6f5f 6373 763a 2062  export_to_csv: b
-0000c930: 6f6f 6c20 3d20 5472 7565 2c0a 2020 2020  ool = True,.    
-0000c940: 2020 2020 7365 6172 6368 3a20 626f 6f6c      search: bool
-0000c950: 203d 2054 7275 652c 0a20 2020 2020 2020   = True,.       
-0000c960: 2070 6167 655f 7369 7a65 3a20 696e 7420   page_size: int 
-0000c970: 3d20 3130 2c0a 2020 2020 2020 2020 7061  = 10,.        pa
-0000c980: 6765 5f73 697a 655f 6f70 7469 6f6e 733a  ge_size_options:
-0000c990: 204f 7074 696f 6e61 6c5b 6c69 7374 5b69   Optional[list[i
-0000c9a0: 6e74 5d5d 203d 204e 6f6e 652c 0a20 2020  nt]] = None,.   
-0000c9b0: 2020 2020 2069 6e69 7469 616c 5f73 6f72       initial_sor
-0000c9c0: 745f 636f 6c75 6d6e 3a20 4f70 7469 6f6e  t_column: Option
-0000c9d0: 616c 5b73 7472 5d20 3d20 4e6f 6e65 2c0a  al[str] = None,.
-0000c9e0: 2020 2020 2020 2020 736f 7274 5f64 6573          sort_des
-0000c9f0: 6365 6e64 696e 673a 2062 6f6f 6c20 3d20  cending: bool = 
-0000ca00: 4661 6c73 652c 0a20 2020 2020 2020 2063  False,.        c
-0000ca10: 6f6c 756d 6e73 5f6f 7074 696f 6e73 3a20  olumns_options: 
-0000ca20: 4f70 7469 6f6e 616c 5b64 6963 745d 203d  Optional[dict] =
-0000ca30: 204e 6f6e 652c 0a20 2020 2020 2020 2063   None,.        c
-0000ca40: 6174 6567 6f72 6963 616c 5f63 6f6c 756d  ategorical_colum
-0000ca50: 6e73 3a20 4f70 7469 6f6e 616c 5b6c 6973  ns: Optional[lis
-0000ca60: 745b 7374 725d 5d20 3d20 4e6f 6e65 2c0a  t[str]] = None,.
-0000ca70: 2020 2020 2020 2020 6c61 6265 6c5f 636f          label_co
-0000ca80: 6c75 6d6e 733a 204f 7074 696f 6e61 6c5b  lumns: Optional[
-0000ca90: 6469 6374 5d20 3d20 4e6f 6e65 2c0a 2020  dict] = None,.  
-0000caa0: 2020 2020 2020 7765 625f 6c69 6e6b 5f63        web_link_c
-0000cab0: 6f6c 756d 6e3a 204f 7074 696f 6e61 6c5b  olumn: Optional[
-0000cac0: 7374 725d 203d 204e 6f6e 652c 0a20 2020  str] = None,.   
-0000cad0: 2020 2020 206f 7065 6e5f 6c69 6e6b 5f69       open_link_i
-0000cae0: 6e5f 6e65 775f 7461 623a 2062 6f6f 6c20  n_new_tab: bool 
-0000caf0: 3d20 4661 6c73 652c 0a20 2020 2020 2020  = False,.       
-0000cb00: 2074 6974 6c65 3a20 4f70 7469 6f6e 616c   title: Optional
-0000cb10: 5b73 7472 5d20 3d20 4e6f 6e65 2c0a 2020  [str] = None,.  
-0000cb20: 2020 2020 2020 7061 6464 696e 673a 204f        padding: O
-0000cb30: 7074 696f 6e61 6c5b 7374 725d 203d 204e  ptional[str] = N
-0000cb40: 6f6e 652c 0a20 2020 2020 2020 2072 6f77  one,.        row
-0000cb50: 735f 7369 7a65 3a20 4f70 7469 6f6e 616c  s_size: Optional
-0000cb60: 5b69 6e74 5d20 3d20 4e6f 6e65 2c0a 2020  [int] = None,.  
-0000cb70: 2020 2020 2020 636f 6c73 5f73 697a 653a        cols_size:
-0000cb80: 204f 7074 696f 6e61 6c5b 696e 745d 203d   Optional[int] =
-0000cb90: 204e 6f6e 652c 0a20 2020 2029 3a0a 2020   None,.    ):.  
-0000cba0: 2020 2020 2020 2222 2243 7265 6174 6520        """Create 
-0000cbb0: 6120 7461 626c 6520 7265 706f 7274 2069  a table report i
-0000cbc0: 6e20 7468 6520 6461 7368 626f 6172 642e  n the dashboard.
-0000cbd0: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-0000cbe0: 6f72 6465 723a 2074 6865 206f 7264 6572  order: the order
-0000cbf0: 206f 6620 7468 6520 7461 626c 650a 2020   of the table.  
-0000cc00: 2020 2020 2020 3a70 6172 616d 2064 6174        :param dat
-0000cc10: 613a 2074 6865 2064 6174 6120 6f66 2074  a: the data of t
-0000cc20: 6865 2074 6162 6c65 0a20 2020 2020 2020  he table.       
-0000cc30: 203a 7061 7261 6d20 636f 6c75 6d6e 733a   :param columns:
-0000cc40: 2074 6865 2063 6f6c 756d 6e73 206f 6620   the columns of 
-0000cc50: 7468 6520 7461 626c 650a 2020 2020 2020  the table.      
-0000cc60: 2020 3a70 6172 616d 2063 6f6c 756d 6e73    :param columns
-0000cc70: 5f62 7574 746f 6e3a 2077 6865 7468 6572  _button: whether
-0000cc80: 2074 6f20 7368 6f77 2074 6865 2063 6f6c   to show the col
-0000cc90: 756d 6e73 2062 7574 746f 6e0a 2020 2020  umns button.    
-0000cca0: 2020 2020 3a70 6172 616d 2066 696c 7465      :param filte
-0000ccb0: 7273 3a20 7768 6574 6865 7220 746f 2073  rs: whether to s
-0000ccc0: 686f 7720 7468 6520 6669 6c74 6572 7320  how the filters 
-0000ccd0: 6275 7474 6f6e 0a20 2020 2020 2020 203a  button.        :
-0000cce0: 7061 7261 6d20 6578 706f 7274 5f74 6f5f  param export_to_
-0000ccf0: 6373 763a 2077 6865 7468 6572 2074 6f20  csv: whether to 
-0000cd00: 7368 6f77 2074 6865 2065 7870 6f72 7420  show the export 
-0000cd10: 746f 2063 7376 2062 7574 746f 6e0a 2020  to csv button.  
-0000cd20: 2020 2020 2020 3a70 6172 616d 2073 6561        :param sea
-0000cd30: 7263 683a 2077 6865 7468 6572 2074 6f20  rch: whether to 
-0000cd40: 7368 6f77 2074 6865 2073 6561 7263 6820  show the search 
-0000cd50: 6261 720a 2020 2020 2020 2020 3a70 6172  bar.        :par
-0000cd60: 616d 2070 6167 655f 7369 7a65 3a20 7468  am page_size: th
-0000cd70: 6520 6e75 6d62 6572 206f 6620 726f 7773  e number of rows
-0000cd80: 2070 6572 2070 6167 650a 2020 2020 2020   per page.      
-0000cd90: 2020 3a70 6172 616d 2070 6167 655f 7369    :param page_si
-0000cda0: 7a65 5f6f 7074 696f 6e73 3a20 7468 6520  ze_options: the 
-0000cdb0: 6f70 7469 6f6e 7320 666f 7220 7468 6520  options for the 
-0000cdc0: 6e75 6d62 6572 206f 6620 726f 7773 2070  number of rows p
-0000cdd0: 6572 2070 6167 650a 2020 2020 2020 2020  er page.        
-0000cde0: 3a70 6172 616d 2069 6e69 7469 616c 5f73  :param initial_s
-0000cdf0: 6f72 745f 636f 6c75 6d6e 3a20 7468 6520  ort_column: the 
-0000ce00: 696e 6974 6961 6c20 736f 7274 696e 6720  initial sorting 
-0000ce10: 636f 6c75 6d6e 0a20 2020 2020 2020 203a  column.        :
-0000ce20: 7061 7261 6d20 736f 7274 5f64 6573 6365  param sort_desce
-0000ce30: 6e64 696e 673a 2077 6865 7468 6572 2074  nding: whether t
-0000ce40: 6f20 736f 7274 2064 6573 6365 6e64 696e  o sort descendin
-0000ce50: 6720 6279 2074 6865 2069 6e69 7469 616c  g by the initial
-0000ce60: 2073 6f72 7469 6e67 2063 6f6c 756d 6e0a   sorting column.
-0000ce70: 2020 2020 2020 2020 3a70 6172 616d 2063          :param c
-0000ce80: 6f6c 756d 6e73 5f6f 7074 696f 6e73 3a20  olumns_options: 
-0000ce90: 7468 6520 6f70 7469 6f6e 7320 666f 7220  the options for 
-0000cea0: 7468 6520 636f 6c75 6d6e 730a 2020 2020  the columns.    
-0000ceb0: 2020 2020 3a70 6172 616d 2063 6174 6567      :param categ
-0000cec0: 6f72 6963 616c 5f63 6f6c 756d 6e73 3a20  orical_columns: 
-0000ced0: 7468 6520 6361 7465 676f 7269 6361 6c20  the categorical 
-0000cee0: 636f 6c75 6d6e 730a 2020 2020 2020 2020  columns.        
-0000cef0: 3a70 6172 616d 206c 6162 656c 5f63 6f6c  :param label_col
-0000cf00: 756d 6e73 3a20 7468 6520 6c61 6265 6c20  umns: the label 
-0000cf10: 636f 6c75 6d6e 730a 2020 2020 2020 2020  columns.        
-0000cf20: 3a70 6172 616d 2072 6570 6f72 745f 7061  :param report_pa
-0000cf30: 7261 6d73 3a20 6164 6469 7469 6f6e 616c  rams: additional
-0000cf40: 2072 6570 6f72 7420 7061 7261 6d65 7465   report paramete
-0000cf50: 7273 2061 7320 6b65 792d 7661 6c75 6520  rs as key-value 
-0000cf60: 7061 6972 730a 2020 2020 2020 2020 3a70  pairs.        :p
-0000cf70: 6172 616d 2077 6562 5f6c 696e 6b5f 636f  aram web_link_co
-0000cf80: 6c75 6d6e 3a20 7468 6520 636f 6c75 6d6e  lumn: the column
-0000cf90: 2074 6f20 7573 6520 6173 2077 6562 206c   to use as web l
-0000cfa0: 696e 6b0a 2020 2020 2020 2020 3a70 6172  ink.        :par
-0000cfb0: 616d 206f 7065 6e5f 6c69 6e6b 5f69 6e5f  am open_link_in_
-0000cfc0: 6e65 775f 7461 623a 2077 6865 7468 6572  new_tab: whether
-0000cfd0: 2074 6f20 6f70 656e 2074 6865 2077 6562   to open the web
-0000cfe0: 206c 696e 6b20 696e 2061 206e 6577 2074   link in a new t
-0000cff0: 6162 0a20 2020 2020 2020 203a 7061 7261  ab.        :para
-0000d000: 6d20 7469 746c 653a 2074 6865 2074 6974  m title: the tit
-0000d010: 6c65 206f 6620 7468 6520 7461 626c 650a  le of the table.
-0000d020: 2020 2020 2020 2020 3a70 6172 616d 2070          :param p
-0000d030: 6164 6469 6e67 3a20 7468 6520 7061 6464  adding: the padd
-0000d040: 696e 6720 6f66 2074 6865 2074 6162 6c65  ing of the table
-0000d050: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-0000d060: 726f 7773 5f73 697a 653a 2074 6865 2072  rows_size: the r
-0000d070: 6f77 7320 7369 7a65 206f 6620 7468 6520  ows size of the 
-0000d080: 7461 626c 650a 2020 2020 2020 2020 3a70  table.        :p
-0000d090: 6172 616d 2063 6f6c 735f 7369 7a65 3a20  aram cols_size: 
-0000d0a0: 7468 6520 636f 6c75 6d6e 7320 7369 7a65  the columns size
-0000d0b0: 206f 6620 7468 6520 7461 626c 650a 2020   of the table.  
-0000d0c0: 2020 2020 2020 2222 220a 0a20 2020 2020        """..     
-0000d0d0: 2020 2064 6174 615f 6d61 7070 696e 6773     data_mappings
-0000d0e0: 5f74 6f5f 7475 706c 6573 203d 2061 7761  _to_tuples = awa
-0000d0f0: 6974 2073 656c 662e 5f63 686f 6f73 655f  it self._choose_
-0000d100: 6461 7461 286f 7264 6572 2c20 6461 7461  data(order, data
-0000d110: 2c20 5461 626c 6529 0a20 2020 2020 2020  , Table).       
-0000d120: 2069 6620 6973 696e 7374 616e 6365 2864   if isinstance(d
-0000d130: 6174 612c 2073 7472 293a 0a20 2020 2020  ata, str):.     
-0000d140: 2020 2020 2020 2064 6174 6120 3d20 7365         data = se
-0000d150: 6c66 2e5f 7368 6172 6564 5f64 6174 615b  lf._shared_data[
-0000d160: 6461 7461 5d0a 0a20 2020 2020 2020 2064  data]..        d
-0000d170: 6620 3d20 7661 6c69 6461 7465 5f64 6174  f = validate_dat
-0000d180: 615f 6973 5f70 616e 6461 7261 626c 6528  a_is_pandarable(
-0000d190: 6461 7461 290a 0a20 2020 2020 2020 2069  data)..        i
-0000d1a0: 6620 6e6f 7420 636f 6c75 6d6e 733a 0a20  f not columns:. 
-0000d1b0: 2020 2020 2020 2020 2020 2063 6f6c 756d             colum
-0000d1c0: 6e73 203d 206c 6973 7428 6461 7461 5f6d  ns = list(data_m
-0000d1d0: 6170 7069 6e67 735f 746f 5f74 7570 6c65  appings_to_tuple
-0000d1e0: 732e 6b65 7973 2829 290a 2020 2020 2020  s.keys()).      
-0000d1f0: 2020 6966 206e 6f74 2063 6f6c 756d 6e73    if not columns
-0000d200: 5f6f 7074 696f 6e73 3a0a 2020 2020 2020  _options:.      
-0000d210: 2020 2020 2020 636f 6c75 6d6e 735f 6f70        columns_op
-0000d220: 7469 6f6e 7320 3d20 7b7d 0a20 2020 2020  tions = {}.     
-0000d230: 2020 2069 6620 6e6f 7420 6361 7465 676f     if not catego
-0000d240: 7269 6361 6c5f 636f 6c75 6d6e 733a 0a20  rical_columns:. 
-0000d250: 2020 2020 2020 2020 2020 2063 6174 6567             categ
-0000d260: 6f72 6963 616c 5f63 6f6c 756d 6e73 203d  orical_columns =
-0000d270: 205b 5d0a 2020 2020 2020 2020 6966 206e   [].        if n
-0000d280: 6f74 206c 6162 656c 5f63 6f6c 756d 6e73  ot label_columns
-0000d290: 3a0a 2020 2020 2020 2020 2020 2020 6c61  :.            la
-0000d2a0: 6265 6c5f 636f 6c75 6d6e 7320 3d20 7b7d  bel_columns = {}
-0000d2b0: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
-0000d2c0: 2020 2020 2020 2020 2020 2061 7578 5f6c             aux_l
-0000d2d0: 6162 656c 5f63 6f6c 756d 6e73 203d 206c  abel_columns = l
-0000d2e0: 6162 656c 5f63 6f6c 756d 6e73 0a20 2020  abel_columns.   
-0000d2f0: 2020 2020 2020 2020 206c 6162 656c 5f63           label_c
-0000d300: 6f6c 756d 6e73 203d 207b 7d0a 2020 2020  olumns = {}.    
-0000d310: 2020 2020 2020 2020 666f 7220 6861 735f          for has_
-0000d320: 746f 5f62 655f 7475 706c 6520 696e 2061  to_be_tuple in a
-0000d330: 7578 5f6c 6162 656c 5f63 6f6c 756d 6e73  ux_label_columns
-0000d340: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000d350: 2020 7620 3d20 6175 785f 6c61 6265 6c5f    v = aux_label_
-0000d360: 636f 6c75 6d6e 735b 6861 735f 746f 5f62  columns[has_to_b
-0000d370: 655f 7475 706c 655d 0a20 2020 2020 2020  e_tuple].       
-0000d380: 2020 2020 2020 2020 2069 6620 6973 696e           if isin
-0000d390: 7374 616e 6365 2868 6173 5f74 6f5f 6265  stance(has_to_be
-0000d3a0: 5f74 7570 6c65 2c20 7374 7229 3a0a 2020  _tuple, str):.  
-0000d3b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d3c0: 2020 6c61 6265 6c5f 636f 6c75 6d6e 735b    label_columns[
-0000d3d0: 2868 6173 5f74 6f5f 6265 5f74 7570 6c65  (has_to_be_tuple
-0000d3e0: 2c20 2266 696c 6c65 6422 295d 203d 2076  , "filled")] = v
-0000d3f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000d400: 2065 6c69 6620 6973 696e 7374 616e 6365   elif isinstance
-0000d410: 2868 6173 5f74 6f5f 6265 5f74 7570 6c65  (has_to_be_tuple
-0000d420: 2c20 7475 706c 6529 3a0a 2020 2020 2020  , tuple):.      
-0000d430: 2020 2020 2020 2020 2020 2020 2020 6c61                la
-0000d440: 6265 6c5f 636f 6c75 6d6e 735b 6861 735f  bel_columns[has_
-0000d450: 746f 5f62 655f 7475 706c 655d 203d 2076  to_be_tuple] = v
-0000d460: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000d470: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-0000d480: 2020 2020 2020 2020 2020 206c 6f67 5f65             log_e
-0000d490: 7272 6f72 280a 2020 2020 2020 2020 2020  rror(.          
-0000d4a0: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
-0000d4b0: 6767 6572 2c0a 2020 2020 2020 2020 2020  gger,.          
-0000d4c0: 2020 2020 2020 2020 2020 2020 2020 6622                f"
-0000d4d0: 496e 7661 6c69 6420 6c61 6265 6c5f 636f  Invalid label_co
-0000d4e0: 6c75 6d6e 7320 6b65 793a 207b 6861 735f  lumns key: {has_
-0000d4f0: 746f 5f62 655f 7475 706c 657d 222c 0a20  to_be_tuple}",. 
-0000d500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d510: 2020 2020 2020 2056 616c 7565 4572 726f         ValueErro
-0000d520: 722c 0a20 2020 2020 2020 2020 2020 2020  r,.             
-0000d530: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-0000d540: 206c 6162 656c 5f6a 7573 745f 636f 6c75   label_just_colu
-0000d550: 6d6e 7320 3d20 5b78 5b30 5d20 666f 7220  mns = [x[0] for 
-0000d560: 7820 696e 206c 6162 656c 5f63 6f6c 756d  x in label_colum
-0000d570: 6e73 2e6b 6579 7328 295d 0a0a 2020 2020  ns.keys()]..    
-0000d580: 2020 2020 5f2c 2064 6174 615f 7365 742c      _, data_set,
-0000d590: 205f 203d 2064 6174 615f 6d61 7070 696e   _ = data_mappin
-0000d5a0: 6773 5f74 6f5f 7475 706c 6573 5b63 6f6c  gs_to_tuples[col
-0000d5b0: 756d 6e73 5b30 5d5d 0a20 2020 2020 2020  umns[0]].       
-0000d5c0: 2063 6f6c 756d 6e73 5f64 6963 7473 203d   columns_dicts =
-0000d5d0: 205b 5d0a 2020 2020 2020 2020 726f 7773   [].        rows
-0000d5e0: 5f64 6963 7420 3d20 7b22 6d61 7070 696e  _dict = {"mappin
-0000d5f0: 6722 3a20 7b7d 7d0a 2020 2020 2020 2020  g": {}}.        
-0000d600: 666f 7220 692c 206e 616d 6520 696e 2065  for i, name in e
-0000d610: 6e75 6d65 7261 7465 2863 6f6c 756d 6e73  numerate(columns
-0000d620: 293a 0a20 2020 2020 2020 2020 2020 2063  ):.            c
-0000d630: 6f6c 756d 6e5f 6f70 7469 6f6e 7320 3d20  olumn_options = 
-0000d640: 7b22 6669 656c 6422 3a20 6e61 6d65 2c20  {"field": name, 
-0000d650: 2268 6561 6465 724e 616d 6522 3a20 6e61  "headerName": na
-0000d660: 6d65 2c20 226f 7264 6572 223a 2069 7d0a  me, "order": i}.
-0000d670: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-0000d680: 6e61 6d65 2069 6e20 636f 6c75 6d6e 735f  name in columns_
-0000d690: 6f70 7469 6f6e 733a 0a20 2020 2020 2020  options:.       
-0000d6a0: 2020 2020 2020 2020 2063 6f6c 756d 6e5f           column_
-0000d6b0: 6f70 7469 6f6e 732e 7570 6461 7465 2863  options.update(c
-0000d6c0: 6f6c 756d 6e73 5f6f 7074 696f 6e73 5b6e  olumns_options[n
-0000d6d0: 616d 655d 290a 0a20 2020 2020 2020 2020  ame])..         
-0000d6e0: 2020 2069 6620 6e61 6d65 2069 6e20 6361     if name in ca
-0000d6f0: 7465 676f 7269 6361 6c5f 636f 6c75 6d6e  tegorical_column
-0000d700: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
-0000d710: 2020 2069 6620 6e61 6d65 2069 6e20 6c61     if name in la
-0000d720: 6265 6c5f 636f 6c75 6d6e 733a 0a20 2020  bel_columns:.   
-0000d730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d740: 206c 6f67 5f65 7272 6f72 280a 2020 2020   log_error(.    
-0000d750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d760: 2020 2020 6c6f 6767 6572 2c0a 2020 2020      logger,.    
-0000d770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d780: 2020 2020 6622 436f 6c75 6d6e 7320 6361      f"Columns ca
-0000d790: 6e6e 6f74 2062 6520 626f 7468 2069 6e63  nnot be both inc
-0000d7a0: 6c75 6465 6420 696e 2063 6174 6567 6f72  luded in categor
-0000d7b0: 6963 616c 5f63 6f6c 756d 6e73 2061 6e64  ical_columns and
-0000d7c0: 206c 6162 656c 5f63 6f6c 756d 6e73 3a20   label_columns: 
-0000d7d0: 7b6e 616d 657d 222c 0a20 2020 2020 2020  {name}",.       
-0000d7e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d7f0: 2056 616c 7565 4572 726f 722c 0a20 2020   ValueError,.   
-0000d800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d810: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
-0000d820: 2020 2063 6f6c 756d 6e5f 6f70 7469 6f6e     column_option
-0000d830: 735b 2274 7970 6522 5d20 3d20 2273 696e  s["type"] = "sin
-0000d840: 676c 6553 656c 6563 7422 0a20 2020 2020  gleSelect".     
-0000d850: 2020 2020 2020 2020 2020 2063 6f6c 756d             colum
-0000d860: 6e5f 6f70 7469 6f6e 735b 226f 7074 696f  n_options["optio
-0000d870: 6e73 225d 203d 2064 665b 6e61 6d65 5d2e  ns"] = df[name].
-0000d880: 756e 6971 7565 2829 2e74 6f6c 6973 7428  unique().tolist(
-0000d890: 290a 0a20 2020 2020 2020 2020 2020 2069  )..            i
-0000d8a0: 6620 6e61 6d65 2069 6e20 6c61 6265 6c5f  f name in label_
-0000d8b0: 6a75 7374 5f63 6f6c 756d 6e73 3a0a 2020  just_columns:.  
-0000d8c0: 2020 2020 2020 2020 2020 2020 2020 696e                in
-0000d8d0: 6465 7820 3d20 6c61 6265 6c5f 6a75 7374  dex = label_just
-0000d8e0: 5f63 6f6c 756d 6e73 2e69 6e64 6578 286e  _columns.index(n
-0000d8f0: 616d 6529 0a20 2020 2020 2020 2020 2020  ame).           
-0000d900: 2020 2020 2028 5f2c 2076 6172 6961 6e74       (_, variant
-0000d910: 292c 206c 6162 656c 5f6f 7074 696f 6e73  ), label_options
-0000d920: 203d 206c 6973 7428 6c61 6265 6c5f 636f   = list(label_co
-0000d930: 6c75 6d6e 732e 6974 656d 7328 2929 5b69  lumns.items())[i
-0000d940: 6e64 6578 5d0a 2020 2020 2020 2020 2020  ndex].          
-0000d950: 2020 2020 2020 636f 6c75 6d6e 5f6f 7074        column_opt
-0000d960: 696f 6e73 5b22 6368 6970 7322 5d20 3d20  ions["chips"] = 
-0000d970: 7b7d 0a20 2020 2020 2020 2020 2020 2020  {}.             
-0000d980: 2020 2063 6f6c 756d 6e5f 6f70 7469 6f6e     column_option
-0000d990: 735b 2263 6869 7073 225d 5b22 7661 7269  s["chips"]["vari
-0000d9a0: 616e 7422 5d20 3d20 7661 7269 616e 740a  ant"] = variant.
-0000d9b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d9c0: 636f 6c75 6d6e 5f6f 7074 696f 6e73 5b22  column_options["
-0000d9d0: 6368 6970 7322 5d5b 226f 7074 696f 6e73  chips"]["options
-0000d9e0: 225d 203d 2069 6e74 6572 7072 6574 5f6c  "] = interpret_l
-0000d9f0: 6162 656c 5f69 6e66 6f28 0a20 2020 2020  abel_info(.     
-0000da00: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-0000da10: 662c 206e 616d 652c 206c 6162 656c 5f6f  f, name, label_o
-0000da20: 7074 696f 6e73 2c20 7661 7269 616e 740a  ptions, variant.
-0000da30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000da40: 290a 0a20 2020 2020 2020 2020 2020 2069  )..            i
-0000da50: 6620 6e61 6d65 203d 3d20 7765 625f 6c69  f name == web_li
-0000da60: 6e6b 5f63 6f6c 756d 6e3a 0a20 2020 2020  nk_column:.     
-0000da70: 2020 2020 2020 2020 2020 2063 6f6c 756d             colum
-0000da80: 6e5f 6f70 7469 6f6e 735b 226c 696e 6b22  n_options["link"
-0000da90: 5d20 3d20 7b0a 2020 2020 2020 2020 2020  ] = {.          
-0000daa0: 2020 2020 2020 2020 2020 2275 726c 223a            "url":
-0000dab0: 2022 7765 624c 696e 6b22 2c0a 2020 2020   "webLink",.    
-0000dac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dad0: 226f 7065 6e4e 6577 5461 6222 3a20 6f70  "openNewTab": op
-0000dae0: 656e 5f6c 696e 6b5f 696e 5f6e 6577 5f74  en_link_in_new_t
-0000daf0: 6162 2c0a 2020 2020 2020 2020 2020 2020  ab,.            
-0000db00: 2020 2020 7d0a 0a20 2020 2020 2020 2020      }..         
-0000db10: 2020 2063 6f6c 756d 6e73 5f64 6963 7473     columns_dicts
-0000db20: 2e61 7070 656e 6428 636f 6c75 6d6e 5f6f  .append(column_o
-0000db30: 7074 696f 6e73 290a 2020 2020 2020 2020  ptions).        
-0000db40: 2020 2020 726f 7773 5f64 6963 745b 226d      rows_dict["m
-0000db50: 6170 7069 6e67 225d 5b6e 616d 655d 203d  apping"][name] =
-0000db60: 2064 6174 615f 6d61 7070 696e 6773 5f74   data_mappings_t
-0000db70: 6f5f 7475 706c 6573 5b6e 616d 655d 5b30  o_tuples[name][0
-0000db80: 5d0a 0a20 2020 2020 2020 2069 6620 7765  ]..        if we
-0000db90: 625f 6c69 6e6b 5f63 6f6c 756d 6e3a 0a20  b_link_column:. 
-0000dba0: 2020 2020 2020 2020 2020 2072 6f77 735f             rows_
-0000dbb0: 6469 6374 5b22 6d61 7070 696e 6722 5d5b  dict["mapping"][
-0000dbc0: 2277 6562 225d 203d 2064 6174 615f 6d61  "web"] = data_ma
-0000dbd0: 7070 696e 6773 5f74 6f5f 7475 706c 6573  ppings_to_tuples
-0000dbe0: 5b77 6562 5f6c 696e 6b5f 636f 6c75 6d6e  [web_link_column
-0000dbf0: 5d5b 305d 0a20 2020 2020 2020 2020 2020  ][0].           
-0000dc00: 2072 6f77 735f 6469 6374 5b22 6d61 7070   rows_dict["mapp
-0000dc10: 696e 6722 5d5b 2277 6562 4c69 6e6b 225d  ing"]["webLink"]
-0000dc20: 203d 2064 6174 615f 6d61 7070 696e 6773   = data_mappings
-0000dc30: 5f74 6f5f 7475 706c 6573 5b77 6562 5f6c  _to_tuples[web_l
-0000dc40: 696e 6b5f 636f 6c75 6d6e 5d5b 0a20 2020  ink_column][.   
-0000dc50: 2020 2020 2020 2020 2020 2020 2030 0a20               0. 
-0000dc60: 2020 2020 2020 2020 2020 205d 0a0a 2020             ]..  
-0000dc70: 2020 2020 2020 5f2c 2072 6570 6f72 7420        _, report 
-0000dc80: 3d20 6177 6169 7420 7365 6c66 2e5f 6765  = await self._ge
-0000dc90: 745f 6368 6172 745f 7265 706f 7274 286f  t_chart_report(o
-0000dca0: 7264 6572 2c20 5461 626c 6529 0a0a 2020  rder, Table)..  
-0000dcb0: 2020 2020 2020 7264 7320 3d20 6177 6169        rds = awai
-0000dcc0: 7420 7265 706f 7274 2e67 6574 5f72 6570  t report.get_rep
-0000dcd0: 6f72 745f 6461 7461 5f73 6574 7328 290a  ort_data_sets().
-0000dce0: 0a20 2020 2020 2020 2069 6620 280a 2020  .        if (.  
-0000dcf0: 2020 2020 2020 2020 2020 7365 6c66 2e72            self.r
-0000dd00: 6575 7365 5f64 6174 615f 7365 7473 0a20  euse_data_sets. 
-0000dd10: 2020 2020 2020 2020 2020 2061 6e64 2072             and r
-0000dd20: 6570 6f72 745b 2270 726f 7065 7274 6965  eport["propertie
-0000dd30: 7322 5d2e 6765 7428 2263 6f6c 756d 6e73  s"].get("columns
-0000dd40: 2229 0a20 2020 2020 2020 2020 2020 2061  ").            a
-0000dd50: 6e64 2072 6570 6f72 745b 2270 726f 7065  nd report["prope
-0000dd60: 7274 6965 7322 5d5b 2263 6f6c 756d 6e73  rties"]["columns
-0000dd70: 225d 2021 3d20 636f 6c75 6d6e 735f 6469  "] != columns_di
-0000dd80: 6374 730a 2020 2020 2020 2020 293a 0a20  cts.        ):. 
-0000dd90: 2020 2020 2020 2020 2020 206c 6f67 5f65             log_e
-0000dda0: 7272 6f72 280a 2020 2020 2020 2020 2020  rror(.          
-0000ddb0: 2020 2020 2020 6c6f 6767 6572 2c0a 2020        logger,.  
-0000ddc0: 2020 2020 2020 2020 2020 2020 2020 2243                "C
-0000ddd0: 6f6c 756d 6e73 206f 7074 696f 6e73 2064  olumns options d
-0000dde0: 6f20 6e6f 7420 6d61 7463 6820 7468 6520  o not match the 
-0000ddf0: 7072 6576 696f 7573 2063 6f6c 756d 6e73  previous columns
-0000de00: 2c20 6d6f 7374 206c 696b 656c 7920 6461  , most likely da
-0000de10: 7461 2068 6173 2063 6861 6e67 6564 2c22  ta has changed,"
-0000de20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000de30: 2022 2064 6f6e 2774 2075 7365 2074 6865   " don't use the
-0000de40: 2072 6575 7365 5f64 6174 615f 7365 7473   reuse_data_sets
-0000de50: 206f 7074 696f 6e20 696e 2074 6869 7320   option in this 
-0000de60: 6361 7365 222c 0a20 2020 2020 2020 2020  case",.         
-0000de70: 2020 2020 2020 2044 6174 6145 7272 6f72         DataError
-0000de80: 2c0a 2020 2020 2020 2020 2020 2020 290a  ,.            ).
-0000de90: 0a20 2020 2020 2020 2069 6620 7264 7320  .        if rds 
-0000dea0: 616e 6420 280a 2020 2020 2020 2020 2020  and (.          
-0000deb0: 2020 6e6f 7420 7365 6c66 2e72 6575 7365    not self.reuse
-0000dec0: 5f64 6174 615f 7365 7473 0a20 2020 2020  _data_sets.     
-0000ded0: 2020 2020 2020 206f 7220 616e 7928 7264         or any(rd
-0000dee0: 5b22 6461 7461 5365 7449 6422 5d20 213d  ["dataSetId"] !=
-0000def0: 2064 6174 615f 7365 745b 2269 6422 5d20   data_set["id"] 
-0000df00: 666f 7220 7264 2069 6e20 7264 7329 0a20  for rd in rds). 
-0000df10: 2020 2020 2020 2029 3a0a 2020 2020 2020         ):.      
-0000df20: 2020 2020 2020 6177 6169 7420 7265 706f        await repo
-0000df30: 7274 2e64 656c 6574 655f 7265 706f 7274  rt.delete_report
-0000df40: 5f64 6174 615f 7365 7473 286c 6f67 3d54  _data_sets(log=T
-0000df50: 7275 6529 0a20 2020 2020 2020 2020 2020  rue).           
-0000df60: 2072 6473 203d 205b 5d0a 0a20 2020 2020   rds = []..     
-0000df70: 2020 2069 6620 6e6f 7420 7264 733a 0a20     if not rds:. 
-0000df80: 2020 2020 2020 2020 2020 2061 7761 6974             await
-0000df90: 2072 6570 6f72 742e 6372 6561 7465 5f72   report.create_r
-0000dfa0: 6570 6f72 745f 6461 7461 5f73 6574 2828  eport_data_set((
-0000dfb0: 4e6f 6e65 2c20 6461 7461 5f73 6574 2c20  None, data_set, 
-0000dfc0: 4e6f 6e65 2929 0a0a 2020 2020 2020 2020  None))..        
-0000dfd0: 7061 6769 6e61 7469 6f6e 203d 207b 2270  pagination = {"p
-0000dfe0: 6167 6553 697a 6522 3a20 7061 6765 5f73  ageSize": page_s
-0000dff0: 697a 657d 0a20 2020 2020 2020 2069 6620  ize}.        if 
-0000e000: 7061 6765 5f73 697a 655f 6f70 7469 6f6e  page_size_option
-0000e010: 733a 0a20 2020 2020 2020 2020 2020 2070  s:.            p
-0000e020: 6167 696e 6174 696f 6e5b 2270 6167 6553  agination["pageS
-0000e030: 697a 654f 7074 696f 6e73 225d 203d 2070  izeOptions"] = p
-0000e040: 6167 655f 7369 7a65 5f6f 7074 696f 6e73  age_size_options
-0000e050: 0a0a 2020 2020 2020 2020 736f 7274 203d  ..        sort =
-0000e060: 207b 7d0a 2020 2020 2020 2020 6966 2069   {}.        if i
-0000e070: 6e69 7469 616c 5f73 6f72 745f 636f 6c75  nitial_sort_colu
-0000e080: 6d6e 3a0a 2020 2020 2020 2020 2020 2020  mn:.            
-0000e090: 736f 7274 5b22 6669 656c 6422 5d20 3d20  sort["field"] = 
-0000e0a0: 6461 7461 5f6d 6170 7069 6e67 735f 746f  data_mappings_to
-0000e0b0: 5f74 7570 6c65 735b 696e 6974 6961 6c5f  _tuples[initial_
-0000e0c0: 736f 7274 5f63 6f6c 756d 6e5d 5b30 5d0a  sort_column][0].
-0000e0d0: 2020 2020 2020 2020 2020 2020 736f 7274              sort
-0000e0e0: 5b22 6469 7265 6374 696f 6e22 5d20 3d20  ["direction"] = 
-0000e0f0: 2261 7363 2220 6966 206e 6f74 2073 6f72  "asc" if not sor
-0000e100: 745f 6465 7363 656e 6469 6e67 2065 6c73  t_descending els
-0000e110: 6520 2264 6573 6322 0a0a 2020 2020 2020  e "desc"..      
-0000e120: 2020 6177 6169 7420 7365 6c66 2e5f 6372    await self._cr
-0000e130: 6561 7465 5f63 6861 7274 280a 2020 2020  eate_chart(.    
-0000e140: 2020 2020 2020 2020 6368 6172 745f 636c          chart_cl
-0000e150: 6173 733d 5461 626c 652c 0a20 2020 2020  ass=Table,.     
-0000e160: 2020 2020 2020 206f 7264 6572 3d6f 7264         order=ord
-0000e170: 6572 2c0a 2020 2020 2020 2020 2020 2020  er,.            
-0000e180: 7369 7a65 5061 6464 696e 673d 7061 6464  sizePadding=padd
-0000e190: 696e 672c 0a20 2020 2020 2020 2020 2020  ing,.           
-0000e1a0: 2073 697a 6552 6f77 733d 726f 7773 5f73   sizeRows=rows_s
-0000e1b0: 697a 652c 0a20 2020 2020 2020 2020 2020  ize,.           
-0000e1c0: 2073 697a 6543 6f6c 756d 6e73 3d63 6f6c   sizeColumns=col
-0000e1d0: 735f 7369 7a65 2c0a 2020 2020 2020 2020  s_size,.        
-0000e1e0: 2020 2020 7469 746c 653d 7469 746c 652c      title=title,
-0000e1f0: 0a20 2020 2020 2020 2020 2020 2070 726f  .            pro
-0000e200: 7065 7274 6965 733d 6469 6374 280a 2020  perties=dict(.  
-0000e210: 2020 2020 2020 2020 2020 2020 2020 636f                co
-0000e220: 6c75 6d6e 733d 636f 6c75 6d6e 735f 6469  lumns=columns_di
-0000e230: 6374 732c 0a20 2020 2020 2020 2020 2020  cts,.           
-0000e240: 2020 2020 2072 6f77 733d 726f 7773 5f64       rows=rows_d
-0000e250: 6963 742c 0a20 2020 2020 2020 2020 2020  ict,.           
-0000e260: 2020 2020 2063 6f6c 756d 6e73 4275 7474       columnsButt
-0000e270: 6f6e 3d63 6f6c 756d 6e73 5f62 7574 746f  on=columns_butto
-0000e280: 6e2c 0a20 2020 2020 2020 2020 2020 2020  n,.             
-0000e290: 2020 2066 696c 7465 7273 4275 7474 6f6e     filtersButton
-0000e2a0: 3d66 696c 7465 7273 2c0a 2020 2020 2020  =filters,.      
-0000e2b0: 2020 2020 2020 2020 2020 6578 706f 7274            export
-0000e2c0: 4275 7474 6f6e 3d65 7870 6f72 745f 746f  Button=export_to
-0000e2d0: 5f63 7376 2c0a 2020 2020 2020 2020 2020  _csv,.          
-0000e2e0: 2020 2020 2020 7365 6172 6368 3d73 6561        search=sea
-0000e2f0: 7263 682c 0a20 2020 2020 2020 2020 2020  rch,.           
-0000e300: 2020 2020 2070 6167 696e 6174 696f 6e3d       pagination=
-0000e310: 7061 6769 6e61 7469 6f6e 2c0a 2020 2020  pagination,.    
-0000e320: 2020 2020 2020 2020 2020 2020 736f 7274              sort
-0000e330: 3d73 6f72 742c 0a20 2020 2020 2020 2020  =sort,.         
-0000e340: 2020 2029 2c0a 2020 2020 2020 2020 290a     ),.        ).
-0000e350: 0a20 2020 2040 6164 645f 746f 5f67 656e  .    @add_to_gen
-0000e360: 6572 616c 5f61 7379 6e63 5f67 726f 7570  eral_async_group
-0000e370: 0a20 2020 2061 7379 6e63 2064 6566 2069  .    async def i
-0000e380: 6e70 7574 5f66 6f72 6d28 0a20 2020 2020  nput_form(.     
-0000e390: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
-0000e3a0: 206f 7074 696f 6e73 3a20 6469 6374 2c0a   options: dict,.
-0000e3b0: 2020 2020 2020 2020 6f72 6465 723a 2069          order: i
-0000e3c0: 6e74 2c0a 2020 2020 2020 2020 7061 6464  nt,.        padd
-0000e3d0: 696e 673a 204f 7074 696f 6e61 6c5b 7374  ing: Optional[st
-0000e3e0: 725d 203d 204e 6f6e 652c 0a20 2020 2020  r] = None,.     
-0000e3f0: 2020 2072 6f77 735f 7369 7a65 3a20 4f70     rows_size: Op
-0000e400: 7469 6f6e 616c 5b69 6e74 5d20 3d20 4e6f  tional[int] = No
-0000e410: 6e65 2c0a 2020 2020 2020 2020 636f 6c73  ne,.        cols
-0000e420: 5f73 697a 653a 204f 7074 696f 6e61 6c5b  _size: Optional[
-0000e430: 696e 745d 203d 204e 6f6e 652c 0a20 2020  int] = None,.   
-0000e440: 2020 2020 206d 6f64 616c 3a20 4f70 7469       modal: Opti
-0000e450: 6f6e 616c 5b73 7472 5d20 3d20 4e6f 6e65  onal[str] = None
-0000e460: 2c0a 2020 2020 2020 2020 6163 7469 7669  ,.        activi
-0000e470: 7479 5f69 643a 204f 7074 696f 6e61 6c5b  ty_id: Optional[
-0000e480: 7374 725d 203d 204e 6f6e 652c 0a20 2020  str] = None,.   
-0000e490: 2020 2020 2061 6374 6976 6974 795f 6e61       activity_na
-0000e4a0: 6d65 3a20 4f70 7469 6f6e 616c 5b73 7472  me: Optional[str
-0000e4b0: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
-0000e4c0: 2020 6163 7469 6f6e 5f69 643a 204f 7074    action_id: Opt
-0000e4d0: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
-0000e4e0: 652c 0a20 2020 2020 2020 206f 6e5f 7375  e,.        on_su
-0000e4f0: 626d 6974 5f65 7665 6e74 733a 204f 7074  bmit_events: Opt
-0000e500: 696f 6e61 6c5b 6c69 7374 5b64 6963 745d  ional[list[dict]
-0000e510: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 293a  ] = None,.    ):
-0000e520: 0a20 2020 2020 2020 2022 2222 4372 6561  .        """Crea
-0000e530: 7465 7320 616e 2069 6e70 7574 2066 6f72  tes an input for
-0000e540: 6d2e 0a20 2020 2020 2020 203a 7061 7261  m..        :para
-0000e550: 6d20 6f70 7469 6f6e 733a 2074 6865 206f  m options: the o
-0000e560: 7074 696f 6e73 2066 6f72 2074 6865 2069  ptions for the i
-0000e570: 6e70 7574 2066 6f72 6d0a 2020 2020 2020  nput form.      
-0000e580: 2020 3a70 6172 616d 206f 7264 6572 3a20    :param order: 
-0000e590: 7468 6520 6f72 6465 7220 6f66 2074 6865  the order of the
-0000e5a0: 2069 6e70 7574 2066 6f72 6d0a 2020 2020   input form.    
-0000e5b0: 2020 2020 3a70 6172 616d 2070 6164 6469      :param paddi
-0000e5c0: 6e67 3a20 7468 6520 7061 6464 696e 6720  ng: the padding 
-0000e5d0: 6f66 2074 6865 2069 6e70 7574 2066 6f72  of the input for
-0000e5e0: 6d0a 2020 2020 2020 2020 3a70 6172 616d  m.        :param
-0000e5f0: 2072 6f77 735f 7369 7a65 3a20 7468 6520   rows_size: the 
-0000e600: 726f 7773 2073 697a 6520 6f66 2074 6865  rows size of the
-0000e610: 2069 6e70 7574 2066 6f72 6d0a 2020 2020   input form.    
-0000e620: 2020 2020 3a70 6172 616d 2063 6f6c 735f      :param cols_
-0000e630: 7369 7a65 3a20 7468 6520 636f 6c75 6d6e  size: the column
-0000e640: 7320 7369 7a65 206f 6620 7468 6520 696e  s size of the in
-0000e650: 7075 7420 666f 726d 0a20 2020 2020 2020  put form.       
-0000e660: 203a 7061 7261 6d20 6d6f 6461 6c3a 2074   :param modal: t
-0000e670: 6865 206d 6f64 616c 2074 6f20 6f70 656e  he modal to open
-0000e680: 2061 6674 6572 2073 7562 6d69 7474 696e   after submittin
-0000e690: 6720 7468 6520 666f 726d 0a20 2020 2020  g the form.     
-0000e6a0: 2020 203a 7061 7261 6d20 6163 7469 7669     :param activi
-0000e6b0: 7479 5f69 643a 2074 6865 2061 6374 6976  ty_id: the activ
-0000e6c0: 6974 7920 6964 2074 6f20 7275 6e20 6166  ity id to run af
-0000e6d0: 7465 7220 7375 626d 6974 7469 6e67 2074  ter submitting t
-0000e6e0: 6865 2066 6f72 6d0a 2020 2020 2020 2020  he form.        
-0000e6f0: 3a70 6172 616d 2061 6374 6976 6974 795f  :param activity_
-0000e700: 6e61 6d65 3a20 7468 6520 6163 7469 7669  name: the activi
-0000e710: 7479 206e 616d 6520 746f 2072 756e 2061  ty name to run a
-0000e720: 6674 6572 2073 7562 6d69 7474 696e 6720  fter submitting 
-0000e730: 7468 6520 666f 726d 0a20 2020 2020 2020  the form.       
-0000e740: 203a 7061 7261 6d20 6163 7469 6f6e 5f69   :param action_i
-0000e750: 643a 2074 6865 2061 6374 696f 6e20 6964  d: the action id
-0000e760: 2074 6f20 7275 6e20 6166 7465 7220 7375   to run after su
-0000e770: 626d 6974 7469 6e67 2074 6865 2066 6f72  bmitting the for
-0000e780: 6d0a 2020 2020 2020 2020 3a70 6172 616d  m.        :param
-0000e790: 206f 6e5f 7375 626d 6974 5f65 7665 6e74   on_submit_event
-0000e7a0: 733a 2074 6865 2065 7665 6e74 7320 746f  s: the events to
-0000e7b0: 2072 756e 2061 6674 6572 2073 7562 6d69   run after submi
-0000e7c0: 7474 696e 6720 7468 6520 666f 726d 0a20  tting the form. 
-0000e7d0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-0000e7e0: 2020 2076 616c 6964 6174 655f 696e 7075     validate_inpu
-0000e7f0: 745f 666f 726d 5f64 6174 6128 7365 6c66  t_form_data(self
-0000e800: 2c20 6f70 7469 6f6e 7329 0a0a 2020 2020  , options)..    
-0000e810: 2020 2020 6966 206f 6e5f 7375 626d 6974      if on_submit
-0000e820: 5f65 7665 6e74 7320 6973 204e 6f6e 653a  _events is None:
-0000e830: 0a20 2020 2020 2020 2020 2020 206f 6e5f  .            on_
-0000e840: 7375 626d 6974 5f65 7665 6e74 7320 3d20  submit_events = 
-0000e850: 5b5d 0a0a 2020 2020 2020 2020 6966 206d  []..        if m
-0000e860: 6f64 616c 3a0a 2020 2020 2020 2020 2020  odal:.          
-0000e870: 2020 6d6f 6461 6c5f 6964 203d 2028 6177    modal_id = (aw
-0000e880: 6169 7420 7365 6c66 2e5f 6765 745f 6d6f  ait self._get_mo
-0000e890: 6461 6c28 6d6f 6461 6c29 295b 2269 6422  dal(modal))["id"
-0000e8a0: 5d0a 2020 2020 2020 2020 2020 2020 6f6e  ].            on
-0000e8b0: 5f73 7562 6d69 745f 6576 656e 7473 2e61  _submit_events.a
-0000e8c0: 7070 656e 6428 0a20 2020 2020 2020 2020  ppend(.         
-0000e8d0: 2020 2020 2020 207b 2261 6374 696f 6e22         {"action"
-0000e8e0: 3a20 226f 7065 6e4d 6f64 616c 222c 2022  : "openModal", "
-0000e8f0: 7061 7261 6d73 223a 207b 226d 6f64 616c  params": {"modal
-0000e900: 4964 223a 206d 6f64 616c 5f69 647d 7d0a  Id": modal_id}}.
-0000e910: 2020 2020 2020 2020 2020 2020 290a 0a20              ).. 
-0000e920: 2020 2020 2020 2069 6620 6163 7469 7669         if activi
-0000e930: 7479 5f69 6420 6f72 2061 6374 6976 6974  ty_id or activit
-0000e940: 795f 6e61 6d65 3a0a 2020 2020 2020 2020  y_name:.        
-0000e950: 2020 2020 6163 7469 7669 7479 5f69 6420      activity_id 
-0000e960: 3d20 2861 7761 6974 2073 656c 662e 5f61  = (await self._a
-0000e970: 7070 2e67 6574 5f61 6374 6976 6974 7928  pp.get_activity(
-0000e980: 6163 7469 7669 7479 5f69 642c 2061 6374  activity_id, act
-0000e990: 6976 6974 795f 6e61 6d65 2929 5b0a 2020  ivity_name))[.  
-0000e9a0: 2020 2020 2020 2020 2020 2020 2020 2269                "i
-0000e9b0: 6422 0a20 2020 2020 2020 2020 2020 205d  d".            ]
-0000e9c0: 0a0a 2020 2020 2020 2020 2020 2020 6f6e  ..            on
-0000e9d0: 5f73 7562 6d69 745f 6576 656e 7473 2e61  _submit_events.a
-0000e9e0: 7070 656e 6428 0a20 2020 2020 2020 2020  ppend(.         
-0000e9f0: 2020 2020 2020 207b 0a20 2020 2020 2020         {.       
-0000ea00: 2020 2020 2020 2020 2020 2020 2022 6163               "ac
-0000ea10: 7469 6f6e 223a 2022 7275 6e41 6374 6976  tion": "runActiv
-0000ea20: 6974 7922 2c0a 2020 2020 2020 2020 2020  ity",.          
-0000ea30: 2020 2020 2020 2020 2020 2270 6172 616d            "param
-0000ea40: 7322 3a20 7b0a 2020 2020 2020 2020 2020  s": {.          
-0000ea50: 2020 2020 2020 2020 2020 2020 2020 2261                "a
-0000ea60: 6374 6976 6974 7949 6422 3a20 6163 7469  ctivityId": acti
-0000ea70: 7669 7479 5f69 642c 0a20 2020 2020 2020  vity_id,.       
-0000ea80: 2020 2020 2020 2020 2020 2020 207d 2c0a               },.
-0000ea90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eaa0: 7d0a 2020 2020 2020 2020 2020 2020 290a  }.            ).
-0000eab0: 0a20 2020 2020 2020 2069 6620 6163 7469  .        if acti
-0000eac0: 6f6e 5f69 643a 0a20 2020 2020 2020 2020  on_id:.         
-0000ead0: 2020 206f 6e5f 7375 626d 6974 5f65 7665     on_submit_eve
-0000eae0: 6e74 732e 6170 7065 6e64 280a 2020 2020  nts.append(.    
-0000eaf0: 2020 2020 2020 2020 2020 2020 7b0a 2020              {.  
-0000eb00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eb10: 2020 2261 6374 696f 6e22 3a20 2272 756e    "action": "run
-0000eb20: 4163 7469 6f6e 222c 0a20 2020 2020 2020  Action",.       
-0000eb30: 2020 2020 2020 2020 2020 2020 2022 7061               "pa
-0000eb40: 7261 6d73 223a 207b 0a20 2020 2020 2020  rams": {.       
-0000eb50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eb60: 2022 6163 7469 6f6e 4964 223a 2061 6374   "actionId": act
-0000eb70: 696f 6e5f 6964 2c0a 2020 2020 2020 2020  ion_id,.        
-0000eb80: 2020 2020 2020 2020 2020 2020 7d2c 0a20              },. 
-0000eb90: 2020 2020 2020 2020 2020 2020 2020 207d                 }
-0000eba0: 0a20 2020 2020 2020 2020 2020 2029 0a0a  .            )..
-0000ebb0: 2020 2020 2020 2020 696e 6974 6961 6c5f          initial_
-0000ebc0: 6461 7461 3a20 6469 6374 203d 207b 7d0a  data: dict = {}.
-0000ebd0: 2020 2020 2020 2020 666f 7220 6669 656c          for fiel
-0000ebe0: 6473 2069 6e20 6f70 7469 6f6e 735b 2266  ds in options["f
-0000ebf0: 6965 6c64 7322 5d3a 0a20 2020 2020 2020  ields"]:.       
-0000ec00: 2020 2020 2066 6f72 2066 6965 6c64 2069       for field i
-0000ec10: 6e20 6669 656c 6473 5b22 6669 656c 6473  n fields["fields
-0000ec20: 225d 3a0a 2020 2020 2020 2020 2020 2020  "]:.            
-0000ec30: 2020 2020 6669 656c 645f 6e61 6d65 3a20      field_name: 
-0000ec40: 7374 7220 3d20 6669 656c 645b 2266 6965  str = field["fie
-0000ec50: 6c64 4e61 6d65 225d 0a20 2020 2020 2020  ldName"].       
-0000ec60: 2020 2020 2020 2020 2069 6e70 7574 5f74           input_t
-0000ec70: 7970 653a 204f 7074 696f 6e61 6c5b 7374  ype: Optional[st
-0000ec80: 725d 203d 2066 6965 6c64 2e67 6574 2822  r] = field.get("
-0000ec90: 696e 7075 7454 7970 6522 290a 2020 2020  inputType").    
-0000eca0: 2020 2020 2020 2020 2020 2020 6966 2069              if i
-0000ecb0: 6e70 7574 5f74 7970 6520 3d3d 2022 636f  nput_type == "co
-0000ecc0: 6c6f 7222 3a0a 2020 2020 2020 2020 2020  lor":.          
-0000ecd0: 2020 2020 2020 2020 2020 696e 6974 6961            initia
-0000ece0: 6c5f 6461 7461 5b66 6965 6c64 5f6e 616d  l_data[field_nam
-0000ecf0: 655d 203d 2022 2330 3030 3030 3022 0a20  e] = "#000000". 
-0000ed00: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-0000ed10: 6c69 6620 696e 7075 745f 7479 7065 203d  lif input_type =
-0000ed20: 3d20 226e 756d 6265 7222 3a0a 2020 2020  = "number":.    
-0000ed30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ed40: 696e 6974 6961 6c5f 6461 7461 5b66 6965  initial_data[fie
-0000ed50: 6c64 5f6e 616d 655d 203d 2030 0a20 2020  ld_name] = 0.   
-0000ed60: 2020 2020 2020 2020 2020 2020 2065 6c73               els
-0000ed70: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-0000ed80: 2020 2020 2020 2069 6e69 7469 616c 5f64         initial_d
-0000ed90: 6174 615b 6669 656c 645f 6e61 6d65 5d20  ata[field_name] 
-0000eda0: 3d20 2222 0a0a 2020 2020 2020 2020 725f  = ""..        r_
-0000edb0: 6861 7368 2c20 7265 706f 7274 203d 2061  hash, report = a
-0000edc0: 7761 6974 2073 656c 662e 5f67 6574 5f63  wait self._get_c
-0000edd0: 6861 7274 5f72 6570 6f72 7428 6f72 6465  hart_report(orde
-0000ede0: 722c 2049 6e70 7574 466f 726d 290a 2020  r, InputForm).  
-0000edf0: 2020 2020 2020 5f2c 2064 6174 615f 7365        _, data_se
-0000ee00: 742c 205f 203d 206c 6973 7428 0a20 2020  t, _ = list(.   
-0000ee10: 2020 2020 2020 2020 2028 0a20 2020 2020           (.     
-0000ee20: 2020 2020 2020 2020 2020 2061 7761 6974             await
-0000ee30: 2073 656c 662e 5f63 7265 6174 655f 6461   self._create_da
-0000ee40: 7461 5f73 6574 2872 6570 6f72 745b 2269  ta_set(report["i
-0000ee50: 6422 5d2c 2069 6e69 7469 616c 5f64 6174  d"], initial_dat
-0000ee60: 612c 2064 756d 705f 7768 6f6c 653d 5472  a, dump_whole=Tr
-0000ee70: 7565 290a 2020 2020 2020 2020 2020 2020  ue).            
-0000ee80: 292e 7661 6c75 6573 2829 0a20 2020 2020  ).values().     
-0000ee90: 2020 2029 5b30 5d0a 0a20 2020 2020 2020     )[0]..       
-0000eea0: 2072 6473 203d 2061 7761 6974 2072 6570   rds = await rep
-0000eeb0: 6f72 742e 6765 745f 7265 706f 7274 5f64  ort.get_report_d
-0000eec0: 6174 615f 7365 7473 2829 0a20 2020 2020  ata_sets().     
-0000eed0: 2020 2069 6620 6c65 6e28 7264 7329 203e     if len(rds) >
-0000eee0: 2031 3a0a 2020 2020 2020 2020 2020 2020   1:.            
-0000eef0: 6c6f 675f 6572 726f 7228 0a20 2020 2020  log_error(.     
-0000ef00: 2020 2020 2020 2020 2020 206c 6f67 6765             logge
-0000ef10: 722c 0a20 2020 2020 2020 2020 2020 2020  r,.             
-0000ef20: 2020 2022 496e 7075 7420 666f 726d 2063     "Input form c
-0000ef30: 616e 206f 6e6c 7920 6861 7665 206f 6e65  an only have one
-0000ef40: 2063 6f6d 706f 6e65 6e74 2064 6174 6120   component data 
-0000ef50: 7365 7420 6c69 6e6b 2c20 220a 2020 2020  set link, ".    
-0000ef60: 2020 2020 2020 2020 2020 2020 2274 6869              "thi
-0000ef70: 7320 6973 2061 6e20 5344 4b20 6275 6720  s is an SDK bug 
-0000ef80: 706c 6561 7365 2072 6570 6f72 7420 6974  please report it
-0000ef90: 2061 6e64 2022 0a20 2020 2020 2020 2020   and ".         
-0000efa0: 2020 2020 2020 2022 6465 6c65 7465 2074         "delete t
-0000efb0: 6865 2066 6f72 6d20 746f 2073 6f6c 7665  he form to solve
-0000efc0: 2074 6865 2069 7373 7565 222c 0a20 2020   the issue",.   
-0000efd0: 2020 2020 2020 2020 2020 2020 2044 6174               Dat
-0000efe0: 6145 7272 6f72 2c0a 2020 2020 2020 2020  aError,.        
-0000eff0: 2020 2020 290a 0a20 2020 2020 2020 2069      )..        i
-0000f000: 6620 7264 7320 616e 6420 280a 2020 2020  f rds and (.    
-0000f010: 2020 2020 2020 2020 6e6f 7420 7365 6c66          not self
-0000f020: 2e72 6575 7365 5f64 6174 615f 7365 7473  .reuse_data_sets
-0000f030: 0a20 2020 2020 2020 2020 2020 206f 7220  .            or 
-0000f040: 7264 735b 305d 5b22 6461 7461 5365 7449  rds[0]["dataSetI
-0000f050: 6422 5d20 213d 2064 6174 615f 7365 745b  d"] != data_set[
-0000f060: 2269 6422 5d0a 2020 2020 2020 2020 2020  "id"].          
-0000f070: 2020 6f72 2072 6473 5b30 5d5b 2270 726f    or rds[0]["pro
-0000f080: 7065 7274 6965 7322 5d5b 2266 6965 6c64  perties"]["field
-0000f090: 7322 5d20 213d 206f 7074 696f 6e73 5b22  s"] != options["
-0000f0a0: 6669 656c 6473 225d 0a20 2020 2020 2020  fields"].       
-0000f0b0: 2029 3a0a 2020 2020 2020 2020 2020 2020   ):.            
-0000f0c0: 6177 6169 7420 7265 706f 7274 2e64 656c  await report.del
-0000f0d0: 6574 655f 7265 706f 7274 5f64 6174 615f  ete_report_data_
-0000f0e0: 7365 7473 286c 6f67 3d54 7275 6529 0a20  sets(log=True). 
-0000f0f0: 2020 2020 2020 2020 2020 2072 6473 203d             rds =
-0000f100: 205b 5d0a 0a20 2020 2020 2020 2069 6620   []..        if 
-0000f110: 6e6f 7420 7264 733a 0a20 2020 2020 2020  not rds:.       
-0000f120: 2020 2020 2061 7761 6974 2072 6570 6f72       await repor
-0000f130: 742e 6372 6561 7465 5f72 6570 6f72 745f  t.create_report_
-0000f140: 6461 7461 5f73 6574 280a 2020 2020 2020  data_set(.      
-0000f150: 2020 2020 2020 2020 2020 2822 6375 7374            ("cust
-0000f160: 6f6d 4669 656c 6431 222c 2064 6174 615f  omField1", data_
-0000f170: 7365 742c 204e 6f6e 6529 2c20 7072 6f70  set, None), prop
-0000f180: 6572 7469 6573 3d6f 7074 696f 6e73 0a20  erties=options. 
-0000f190: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-0000f1a0: 2020 2020 2020 2020 206c 6f67 6765 722e           logger.
-0000f1b0: 696e 666f 2866 2243 7265 6174 6564 2031  info(f"Created 1
-0000f1c0: 2063 6f6d 706f 6e65 6e74 2064 6174 6120   component data 
-0000f1d0: 7365 7420 6c69 6e6b 2066 6f72 2069 6e70  set link for inp
-0000f1e0: 7574 2066 6f72 6d20 6174 207b 725f 6861  ut form at {r_ha
-0000f1f0: 7368 7d22 290a 0a20 2020 2020 2020 2061  sh}")..        a
-0000f200: 7761 6974 2073 656c 662e 5f63 7265 6174  wait self._creat
-0000f210: 655f 6368 6172 7428 0a20 2020 2020 2020  e_chart(.       
-0000f220: 2020 2020 2063 6861 7274 5f63 6c61 7373       chart_class
-0000f230: 3d49 6e70 7574 466f 726d 2c0a 2020 2020  =InputForm,.    
-0000f240: 2020 2020 2020 2020 6f72 6465 723d 6f72          order=or
-0000f250: 6465 722c 0a20 2020 2020 2020 2020 2020  der,.           
-0000f260: 2073 697a 6550 6164 6469 6e67 3d70 6164   sizePadding=pad
-0000f270: 6469 6e67 2c0a 2020 2020 2020 2020 2020  ding,.          
-0000f280: 2020 7369 7a65 526f 7773 3d72 6f77 735f    sizeRows=rows_
-0000f290: 7369 7a65 2c0a 2020 2020 2020 2020 2020  size,.          
-0000f2a0: 2020 7369 7a65 436f 6c75 6d6e 733d 636f    sizeColumns=co
-0000f2b0: 6c73 5f73 697a 652c 0a20 2020 2020 2020  ls_size,.       
-0000f2c0: 2020 2020 2070 726f 7065 7274 6965 733d       properties=
-0000f2d0: 7b22 6576 656e 7473 223a 207b 226f 6e53  {"events": {"onS
-0000f2e0: 7562 6d69 7422 3a20 6f6e 5f73 7562 6d69  ubmit": on_submi
-0000f2f0: 745f 6576 656e 7473 7d7d 2c0a 2020 2020  t_events}},.    
-0000f300: 2020 2020 290a 0a20 2020 2064 6566 2067      )..    def g
-0000f310: 656e 6572 6174 655f 696e 7075 745f 666f  enerate_input_fo
-0000f320: 726d 5f67 726f 7570 7328 0a20 2020 2020  rm_groups(.     
-0000f330: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
-0000f340: 206f 7264 6572 3a20 696e 742c 0a20 2020   order: int,.   
-0000f350: 2020 2020 2066 6f72 6d5f 6772 6f75 7073       form_groups
-0000f360: 3a20 6469 6374 2c0a 2020 2020 2020 2020  : dict,.        
-0000f370: 6479 6e61 6d69 635f 7365 7175 656e 7469  dynamic_sequenti
-0000f380: 616c 5f73 686f 773a 204f 7074 696f 6e61  al_show: Optiona
-0000f390: 6c5b 626f 6f6c 5d20 3d20 4661 6c73 652c  l[bool] = False,
-0000f3a0: 0a20 2020 2020 2020 2061 7574 6f5f 7365  .        auto_se
-0000f3b0: 6e64 3a20 4f70 7469 6f6e 616c 5b62 6f6f  nd: Optional[boo
-0000f3c0: 6c5d 203d 2046 616c 7365 2c0a 2020 2020  l] = False,.    
-0000f3d0: 2020 2020 6e65 7874 5f67 726f 7570 5f6c      next_group_l
-0000f3e0: 6162 656c 3a20 4f70 7469 6f6e 616c 5b73  abel: Optional[s
-0000f3f0: 7472 5d20 3d20 224e 6578 7422 2c0a 2020  tr] = "Next",.  
-0000f400: 2020 2020 2020 726f 7773 5f73 697a 653a        rows_size:
-0000f410: 204f 7074 696f 6e61 6c5b 696e 745d 203d   Optional[int] =
-0000f420: 2033 2c0a 2020 2020 2020 2020 636f 6c73   3,.        cols
-0000f430: 5f73 697a 653a 2069 6e74 203d 2031 322c  _size: int = 12,
-0000f440: 0a20 2020 2020 2020 2070 6164 6469 6e67  .        padding
-0000f450: 3a20 4f70 7469 6f6e 616c 5b73 7472 5d20  : Optional[str] 
-0000f460: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-0000f470: 6d6f 6461 6c3a 204f 7074 696f 6e61 6c5b  modal: Optional[
-0000f480: 7374 725d 203d 204e 6f6e 652c 0a20 2020  str] = None,.   
-0000f490: 2020 2020 2061 6374 6976 6974 795f 6964       activity_id
-0000f4a0: 3a20 4f70 7469 6f6e 616c 5b73 7472 5d20  : Optional[str] 
-0000f4b0: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-0000f4c0: 6163 7469 7669 7479 5f6e 616d 653a 204f  activity_name: O
-0000f4d0: 7074 696f 6e61 6c5b 7374 725d 203d 204e  ptional[str] = N
-0000f4e0: 6f6e 652c 0a20 2020 2020 2020 2061 6374  one,.        act
-0000f4f0: 696f 6e5f 6964 3a20 4f70 7469 6f6e 616c  ion_id: Optional
-0000f500: 5b73 7472 5d20 3d20 4e6f 6e65 2c0a 2020  [str] = None,.  
-0000f510: 2020 2020 2020 6f6e 5f73 7562 6d69 745f        on_submit_
-0000f520: 6576 656e 7473 3a20 4f70 7469 6f6e 616c  events: Optional
-0000f530: 5b6c 6973 745b 6469 6374 5d5d 203d 204e  [list[dict]] = N
-0000f540: 6f6e 652c 0a20 2020 2029 3a0a 2020 2020  one,.    ):.    
-0000f550: 2020 2020 2222 2245 6173 6965 7220 7761      """Easier wa
-0000f560: 7920 746f 2063 7265 6174 6520 616e 2069  y to create an i
-0000f570: 6e70 7574 2066 6f72 6d2e 0a20 2020 2020  nput form..     
-0000f580: 2020 203a 7061 7261 6d20 6d65 6e75 5f70     :param menu_p
-0000f590: 6174 683a 2074 6865 206d 656e 7520 7061  ath: the menu pa
-0000f5a0: 7468 206f 6620 7468 6520 696e 7075 7420  th of the input 
-0000f5b0: 666f 726d 0a20 2020 2020 2020 203a 7061  form.        :pa
-0000f5c0: 7261 6d20 6f72 6465 723a 2074 6865 206f  ram order: the o
-0000f5d0: 7264 6572 206f 6620 7468 6520 696e 7075  rder of the inpu
-0000f5e0: 7420 666f 726d 0a20 2020 2020 2020 203a  t form.        :
-0000f5f0: 7061 7261 6d20 666f 726d 5f67 726f 7570  param form_group
-0000f600: 733a 2074 6865 2066 6f72 6d20 6772 6f75  s: the form grou
-0000f610: 7073 206f 6620 7468 6520 696e 7075 7420  ps of the input 
-0000f620: 666f 726d 0a20 2020 2020 2020 203a 7061  form.        :pa
-0000f630: 7261 6d20 6479 6e61 6d69 635f 7365 7175  ram dynamic_sequ
-0000f640: 656e 7469 616c 5f73 686f 773a 2077 6865  ential_show: whe
-0000f650: 7468 6572 2074 6f20 7368 6f77 2074 6865  ther to show the
-0000f660: 206e 6578 7420 6772 6f75 7020 6166 7465   next group afte
-0000f670: 7220 7375 626d 6974 7469 6e67 2074 6865  r submitting the
-0000f680: 2063 7572 7265 6e74 2067 726f 7570 0a20   current group. 
-0000f690: 2020 2020 2020 203a 7061 7261 6d20 6175         :param au
-0000f6a0: 746f 5f73 656e 643a 2077 6865 7468 6572  to_send: whether
-0000f6b0: 2074 6f20 6175 746f 6d61 7469 6361 6c6c   to automaticall
-0000f6c0: 7920 7365 6e64 2074 6865 2066 6f72 6d20  y send the form 
-0000f6d0: 6166 7465 7220 7468 6520 6c61 7374 2067  after the last g
-0000f6e0: 726f 7570 0a20 2020 2020 2020 203a 7061  roup.        :pa
-0000f6f0: 7261 6d20 6e65 7874 5f67 726f 7570 5f6c  ram next_group_l
-0000f700: 6162 656c 3a20 7468 6520 6c61 6265 6c20  abel: the label 
-0000f710: 6f66 2074 6865 206e 6578 7420 6772 6f75  of the next grou
-0000f720: 7020 6275 7474 6f6e 0a20 2020 2020 2020  p button.       
-0000f730: 203a 7061 7261 6d20 726f 7773 5f73 697a   :param rows_siz
-0000f740: 653a 2074 6865 2072 6f77 7320 7369 7a65  e: the rows size
-0000f750: 206f 6620 7468 6520 696e 7075 7420 666f   of the input fo
-0000f760: 726d 0a20 2020 2020 2020 203a 7061 7261  rm.        :para
-0000f770: 6d20 636f 6c73 5f73 697a 653a 2074 6865  m cols_size: the
-0000f780: 2063 6f6c 756d 6e73 2073 697a 6520 6f66   columns size of
-0000f790: 2074 6865 2069 6e70 7574 2066 6f72 6d0a   the input form.
-0000f7a0: 2020 2020 2020 2020 3a70 6172 616d 2070          :param p
-0000f7b0: 6164 6469 6e67 3a20 7468 6520 7061 6464  adding: the padd
-0000f7c0: 696e 6720 6f66 2074 6865 2069 6e70 7574  ing of the input
-0000f7d0: 2066 6f72 6d0a 2020 2020 2020 2020 3a70   form.        :p
-0000f7e0: 6172 616d 206d 6f64 616c 3a20 7468 6520  aram modal: the 
-0000f7f0: 6d6f 6461 6c20 746f 206f 7065 6e20 6166  modal to open af
-0000f800: 7465 7220 7375 626d 6974 7469 6e67 2074  ter submitting t
-0000f810: 6865 2066 6f72 6d0a 2020 2020 2020 2020  he form.        
-0000f820: 3a70 6172 616d 2061 6374 6976 6974 795f  :param activity_
-0000f830: 6964 3a20 7468 6520 6163 7469 7669 7479  id: the activity
-0000f840: 2069 6420 746f 2072 756e 2061 6674 6572   id to run after
-0000f850: 2073 7562 6d69 7474 696e 6720 7468 6520   submitting the 
-0000f860: 666f 726d 0a20 2020 2020 2020 203a 7061  form.        :pa
-0000f870: 7261 6d20 6163 7469 7669 7479 5f6e 616d  ram activity_nam
-0000f880: 653a 2074 6865 2061 6374 6976 6974 7920  e: the activity 
-0000f890: 6e61 6d65 2074 6f20 7275 6e20 6166 7465  name to run afte
-0000f8a0: 7220 7375 626d 6974 7469 6e67 2074 6865  r submitting the
-0000f8b0: 2066 6f72 6d0a 2020 2020 2020 2020 3a70   form.        :p
-0000f8c0: 6172 616d 2061 6374 696f 6e5f 6964 3a20  aram action_id: 
-0000f8d0: 7468 6520 6163 7469 6f6e 2069 6420 746f  the action id to
-0000f8e0: 2072 756e 2061 6674 6572 2073 7562 6d69   run after submi
-0000f8f0: 7474 696e 6720 7468 6520 666f 726d 0a20  tting the form. 
-0000f900: 2020 2020 2020 203a 7061 7261 6d20 6f6e         :param on
-0000f910: 5f73 7562 6d69 745f 6576 656e 7473 3a20  _submit_events: 
-0000f920: 7468 6520 6576 656e 7473 2074 6f20 7275  the events to ru
-0000f930: 6e20 6166 7465 7220 7375 626d 6974 7469  n after submitti
-0000f940: 6e67 2074 6865 2066 6f72 6d0a 2020 2020  ng the form.    
-0000f950: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-0000f960: 7265 706f 7274 5f64 6174 615f 7365 745f  report_data_set_
-0000f970: 7072 6f70 6572 7469 6573 203d 207b 2266  properties = {"f
-0000f980: 6965 6c64 7322 3a20 5b5d 7d0a 2020 2020  ields": []}.    
-0000f990: 2020 2020 6966 2061 7574 6f5f 7365 6e64      if auto_send
-0000f9a0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-0000f9b0: 706f 7274 5f64 6174 615f 7365 745f 7072  port_data_set_pr
-0000f9c0: 6f70 6572 7469 6573 5b22 7661 7269 616e  operties["varian
-0000f9d0: 7422 5d20 3d20 2261 7574 6f53 656e 6422  t"] = "autoSend"
-0000f9e0: 0a0a 2020 2020 2020 2020 725f 6861 7368  ..        r_hash
-0000f9f0: 203d 2073 656c 662e 5f67 6574 5f63 6861   = self._get_cha
-0000fa00: 7274 5f68 6173 6828 6f72 6465 7229 0a0a  rt_hash(order)..
-0000fa10: 2020 2020 2020 2020 6e65 7874 5f69 6420          next_id 
-0000fa20: 3d20 6622 7b72 5f68 6173 687d 5f30 2220  = f"{r_hash}_0" 
-0000fa30: 6966 2064 796e 616d 6963 5f73 6571 7565  if dynamic_seque
-0000fa40: 6e74 6961 6c5f 7368 6f77 2065 6c73 6520  ntial_show else 
-0000fa50: 4e6f 6e65 0a0a 2020 2020 2020 2020 6e65  None..        ne
-0000fa60: 7874 5f67 726f 7570 5f69 6e64 6578 203d  xt_group_index =
-0000fa70: 2031 0a20 2020 2020 2020 2066 6f72 2066   1.        for f
-0000fa80: 6f72 6d5f 6772 6f75 705f 6e61 6d65 2c20  orm_group_name, 
-0000fa90: 666f 726d 5f67 726f 7570 2069 6e20 666f  form_group in fo
-0000faa0: 726d 5f67 726f 7570 732e 6974 656d 7328  rm_groups.items(
-0000fab0: 293a 0a20 2020 2020 2020 2020 2020 2066  ):.            f
-0000fac0: 6f72 6d5f 6772 6f75 705f 6a73 6f6e 203d  orm_group_json =
-0000fad0: 207b 2274 6974 6c65 223a 2066 6f72 6d5f   {"title": form_
-0000fae0: 6772 6f75 705f 6e61 6d65 2c20 2266 6965  group_name, "fie
-0000faf0: 6c64 7322 3a20 666f 726d 5f67 726f 7570  lds": form_group
-0000fb00: 7d0a 2020 2020 2020 2020 2020 2020 6966  }.            if
-0000fb10: 206e 6578 745f 6964 3a0a 2020 2020 2020   next_id:.      
-0000fb20: 2020 2020 2020 2020 2020 666f 726d 5f67            form_g
-0000fb30: 726f 7570 5f6a 736f 6e5b 2269 6422 5d20  roup_json["id"] 
-0000fb40: 3d20 6e65 7874 5f69 640a 2020 2020 2020  = next_id.      
-0000fb50: 2020 2020 2020 2020 2020 6e65 7874 5f69            next_i
-0000fb60: 6420 3d20 6622 7b72 5f68 6173 687d 5f7b  d = f"{r_hash}_{
-0000fb70: 6e65 7874 5f67 726f 7570 5f69 6e64 6578  next_group_index
-0000fb80: 7d22 0a20 2020 2020 2020 2020 2020 2020  }".             
-0000fb90: 2020 2066 6f72 6d5f 6772 6f75 705f 6a73     form_group_js
-0000fba0: 6f6e 5b22 6e65 7874 466f 726d 4772 6f75  on["nextFormGrou
-0000fbb0: 7022 5d20 3d20 7b0a 2020 2020 2020 2020  p"] = {.        
-0000fbc0: 2020 2020 2020 2020 2020 2020 2269 6422              "id"
-0000fbd0: 3a20 6e65 7874 5f69 642c 0a20 2020 2020  : next_id,.     
-0000fbe0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-0000fbf0: 6c61 6265 6c22 3a20 6e65 7874 5f67 726f  label": next_gro
-0000fc00: 7570 5f6c 6162 656c 2c0a 2020 2020 2020  up_label,.      
-0000fc10: 2020 2020 2020 2020 2020 7d0a 2020 2020            }.    
-0000fc20: 2020 2020 2020 2020 2020 2020 6e65 7874              next
-0000fc30: 5f67 726f 7570 5f69 6e64 6578 202b 3d20  _group_index += 
-0000fc40: 310a 2020 2020 2020 2020 2020 2020 7265  1.            re
-0000fc50: 706f 7274 5f64 6174 615f 7365 745f 7072  port_data_set_pr
-0000fc60: 6f70 6572 7469 6573 5b22 6669 656c 6473  operties["fields
-0000fc70: 225d 202b 3d20 5b66 6f72 6d5f 6772 6f75  "] += [form_grou
-0000fc80: 705f 6a73 6f6e 5d0a 0a20 2020 2020 2020  p_json]..       
-0000fc90: 2069 6620 6e65 7874 5f69 643a 0a20 2020   if next_id:.   
-0000fca0: 2020 2020 2020 2020 2064 656c 2072 6570           del rep
-0000fcb0: 6f72 745f 6461 7461 5f73 6574 5f70 726f  ort_data_set_pro
-0000fcc0: 7065 7274 6965 735b 2266 6965 6c64 7322  perties["fields"
-0000fcd0: 5d5b 2d31 5d5b 226e 6578 7446 6f72 6d47  ][-1]["nextFormG
-0000fce0: 726f 7570 225d 0a0a 2020 2020 2020 2020  roup"]..        
-0000fcf0: 7365 6c66 2e69 6e70 7574 5f66 6f72 6d28  self.input_form(
-0000fd00: 0a20 2020 2020 2020 2020 2020 206f 7074  .            opt
-0000fd10: 696f 6e73 3d72 6570 6f72 745f 6461 7461  ions=report_data
-0000fd20: 5f73 6574 5f70 726f 7065 7274 6965 732c  _set_properties,
-0000fd30: 0a20 2020 2020 2020 2020 2020 206f 7264  .            ord
-0000fd40: 6572 3d6f 7264 6572 2c0a 2020 2020 2020  er=order,.      
-0000fd50: 2020 2020 2020 726f 7773 5f73 697a 653d        rows_size=
-0000fd60: 726f 7773 5f73 697a 652c 0a20 2020 2020  rows_size,.     
-0000fd70: 2020 2020 2020 2063 6f6c 735f 7369 7a65         cols_size
-0000fd80: 3d63 6f6c 735f 7369 7a65 2c0a 2020 2020  =cols_size,.    
-0000fd90: 2020 2020 2020 2020 7061 6464 696e 673d          padding=
-0000fda0: 7061 6464 696e 672c 0a20 2020 2020 2020  padding,.       
-0000fdb0: 2020 2020 206d 6f64 616c 3d6d 6f64 616c       modal=modal
-0000fdc0: 2c0a 2020 2020 2020 2020 2020 2020 6163  ,.            ac
-0000fdd0: 7469 7669 7479 5f69 643d 6163 7469 7669  tivity_id=activi
-0000fde0: 7479 5f69 642c 0a20 2020 2020 2020 2020  ty_id,.         
-0000fdf0: 2020 2061 6374 6976 6974 795f 6e61 6d65     activity_name
-0000fe00: 3d61 6374 6976 6974 795f 6e61 6d65 2c0a  =activity_name,.
-0000fe10: 2020 2020 2020 2020 2020 2020 6f6e 5f73              on_s
-0000fe20: 7562 6d69 745f 6576 656e 7473 3d6f 6e5f  ubmit_events=on_
-0000fe30: 7375 626d 6974 5f65 7665 6e74 732c 0a20  submit_events,. 
-0000fe40: 2020 2020 2020 2020 2020 2061 6374 696f             actio
-0000fe50: 6e5f 6964 3d61 6374 696f 6e5f 6964 2c0a  n_id=action_id,.
-0000fe60: 2020 2020 2020 2020 290a 0a20 2020 2061          )..    a
-0000fe70: 7379 6e63 2064 6566 205f 6765 745f 696e  sync def _get_in
-0000fe80: 7075 745f 666f 726d 5f64 6174 6128 7365  put_form_data(se
-0000fe90: 6c66 2c20 696e 7075 745f 666f 726d 3a20  lf, input_form: 
-0000fea0: 496e 7075 7446 6f72 6d29 202d 3e20 6469  InputForm) -> di
-0000feb0: 6374 3a0a 2020 2020 2020 2020 2222 2247  ct:.        """G
-0000fec0: 6574 2074 6865 2069 6e70 7574 2066 6f72  et the input for
-0000fed0: 6d20 6461 7461 2e22 2222 0a20 2020 2020  m data.""".     
-0000fee0: 2020 2072 6570 6f72 745f 6461 7461 5f73     report_data_s
-0000fef0: 6574 203d 2028 6177 6169 7420 696e 7075  et = (await inpu
-0000ff00: 745f 666f 726d 2e67 6574 5f72 6570 6f72  t_form.get_repor
-0000ff10: 745f 6461 7461 5f73 6574 7328 2929 5b30  t_data_sets())[0
-0000ff20: 5d0a 2020 2020 2020 2020 6461 7461 5f73  ].        data_s
-0000ff30: 6574 203d 2061 7761 6974 2073 656c 662e  et = await self.
-0000ff40: 5f61 7070 2e67 6574 5f64 6174 615f 7365  _app.get_data_se
-0000ff50: 7428 7265 706f 7274 5f64 6174 615f 7365  t(report_data_se
-0000ff60: 745b 2264 6174 6153 6574 4964 225d 290a  t["dataSetId"]).
-0000ff70: 2020 2020 2020 2020 6461 7461 5f70 6f69          data_poi
-0000ff80: 6e74 203d 2061 7761 6974 2064 6174 615f  nt = await data_
-0000ff90: 7365 742e 6765 745f 6f6e 655f 6461 7461  set.get_one_data
-0000ffa0: 5f70 6f69 6e74 2829 0a20 2020 2020 2020  _point().       
-0000ffb0: 206c 6f67 6765 722e 696e 666f 2866 2247   logger.info(f"G
-0000ffc0: 6f74 2069 6e70 7574 2066 6f72 6d20 6461  ot input form da
-0000ffd0: 7461 2066 6f72 207b 7374 7228 696e 7075  ta for {str(inpu
-0000ffe0: 745f 666f 726d 297d 2229 0a20 2020 2020  t_form)}").     
-0000fff0: 2020 2072 6574 7572 6e20 7b0a 2020 2020     return {.    
-00010000: 2020 2020 2020 2020 2272 6570 6f72 7449          "reportI
-00010010: 6422 3a20 696e 7075 745f 666f 726d 5b22  d": input_form["
-00010020: 6964 225d 2c0a 2020 2020 2020 2020 2020  id"],.          
-00010030: 2020 226f 7264 6572 223a 2069 6e70 7574    "order": input
-00010040: 5f66 6f72 6d5b 226f 7264 6572 225d 2c0a  _form["order"],.
-00010050: 2020 2020 2020 2020 2020 2020 2264 6174              "dat
-00010060: 6122 3a20 6461 7461 5f70 6f69 6e74 5b22  a": data_point["
-00010070: 6375 7374 6f6d 4669 656c 6431 225d 2069  customField1"] i
-00010080: 6620 6461 7461 5f70 6f69 6e74 2065 6c73  f data_point els
-00010090: 6520 4e6f 6e65 2c0a 2020 2020 2020 2020  e None,.        
-000100a0: 7d0a 0a20 2020 2061 7379 6e63 2064 6566  }..    async def
-000100b0: 2067 6574 5f69 6e70 7574 5f66 6f72 6d73   get_input_forms
-000100c0: 2873 656c 6629 202d 3e20 6c69 7374 5b64  (self) -> list[d
-000100d0: 6963 745d 3a0a 2020 2020 2020 2020 2222  ict]:.        ""
-000100e0: 2247 6574 2061 6c6c 2074 6865 2069 6e70  "Get all the inp
-000100f0: 7574 2066 6f72 6d73 2069 6e20 7468 6520  ut forms in the 
-00010100: 6375 7272 656e 7420 6d65 6e75 5f70 6174  current menu_pat
-00010110: 682e 2222 220a 2020 2020 2020 2020 7265  h.""".        re
-00010120: 706f 7274 733a 206c 6973 7420 3d20 5b0a  ports: list = [.
-00010130: 2020 2020 2020 2020 2020 2020 7265 706f              repo
-00010140: 7274 0a20 2020 2020 2020 2020 2020 2066  rt.            f
-00010150: 6f72 2072 6570 6f72 7420 696e 2061 7761  or report in awa
-00010160: 6974 2073 656c 662e 5f61 7070 2e67 6574  it self._app.get
-00010170: 5f72 6570 6f72 7473 2829 0a20 2020 2020  _reports().     
-00010180: 2020 2020 2020 2069 6620 7265 706f 7274         if report
-00010190: 5b22 7265 706f 7274 5479 7065 225d 203d  ["reportType"] =
-000101a0: 3d20 2246 4f52 4d22 0a20 2020 2020 2020  = "FORM".       
-000101b0: 2020 2020 2061 6e64 2028 7265 706f 7274       and (report
-000101c0: 5b22 7061 7468 225d 203d 3d20 7365 6c66  ["path"] == self
-000101d0: 2e5f 6375 7272 656e 745f 7061 7468 206f  ._current_path o
-000101e0: 7220 6e6f 7420 7365 6c66 2e5f 6375 7272  r not self._curr
-000101f0: 656e 745f 7061 7468 290a 2020 2020 2020  ent_path).      
-00010200: 2020 5d0a 2020 2020 2020 2020 7265 7475    ].        retu
-00010210: 726e 206c 6973 7428 0a20 2020 2020 2020  rn list(.       
-00010220: 2020 2020 2061 7761 6974 2061 7379 6e63       await async
-00010230: 696f 2e67 6174 6865 7228 0a20 2020 2020  io.gather(.     
-00010240: 2020 2020 2020 2020 2020 202a 5b73 656c             *[sel
-00010250: 662e 5f67 6574 5f69 6e70 7574 5f66 6f72  f._get_input_for
-00010260: 6d5f 6461 7461 2872 6570 6f72 7429 2066  m_data(report) f
-00010270: 6f72 2072 6570 6f72 7420 696e 2072 6570  or report in rep
-00010280: 6f72 7473 5d0a 2020 2020 2020 2020 2020  orts].          
-00010290: 2020 290a 2020 2020 2020 2020 290a 0a20    ).        ).. 
-000102a0: 2020 2040 6164 645f 746f 5f67 656e 6572     @add_to_gener
-000102b0: 616c 5f61 7379 6e63 5f67 726f 7570 0a20  al_async_group. 
-000102c0: 2020 2061 7379 6e63 2064 6566 2061 6e6e     async def ann
-000102d0: 6f74 6174 6564 5f63 6861 7274 280a 2020  otated_chart(.  
-000102e0: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
-000102f0: 2020 2020 6461 7461 3a20 556e 696f 6e5b      data: Union[
-00010300: 6c69 7374 5b44 6174 6146 7261 6d65 5d2c  list[DataFrame],
-00010310: 206c 6973 745b 6c69 7374 5b64 6963 745d   list[list[dict]
-00010320: 5d5d 2c0a 2020 2020 2020 2020 6f72 6465  ]],.        orde
-00010330: 723a 2069 6e74 2c0a 2020 2020 2020 2020  r: int,.        
-00010340: 783a 2073 7472 2c0a 2020 2020 2020 2020  x: str,.        
-00010350: 793a 2055 6e69 6f6e 5b73 7472 2c20 6c69  y: Union[str, li
-00010360: 7374 5b73 7472 5d5d 2c0a 2020 2020 2020  st[str]],.      
-00010370: 2020 616e 6e6f 7461 7469 6f6e 733a 2073    annotations: s
-00010380: 7472 203d 2022 616e 6e6f 7461 7469 6f6e  tr = "annotation
-00010390: 222c 0a20 2020 2020 2020 2072 6f77 735f  ",.        rows_
-000103a0: 7369 7a65 3a20 4f70 7469 6f6e 616c 5b69  size: Optional[i
-000103b0: 6e74 5d20 3d20 4e6f 6e65 2c0a 2020 2020  nt] = None,.    
-000103c0: 2020 2020 636f 6c73 5f73 697a 653a 204f      cols_size: O
-000103d0: 7074 696f 6e61 6c5b 696e 745d 203d 204e  ptional[int] = N
-000103e0: 6f6e 652c 0a20 2020 2020 2020 2070 6164  one,.        pad
-000103f0: 6469 6e67 3a20 4f70 7469 6f6e 616c 5b73  ding: Optional[s
-00010400: 7472 5d20 3d20 4e6f 6e65 2c0a 2020 2020  tr] = None,.    
-00010410: 2020 2020 7469 746c 653a 204f 7074 696f      title: Optio
-00010420: 6e61 6c5b 7374 725d 203d 204e 6f6e 652c  nal[str] = None,
-00010430: 0a20 2020 2020 2020 2079 5f61 7869 735f  .        y_axis_
-00010440: 6e61 6d65 3a20 4f70 7469 6f6e 616c 5b73  name: Optional[s
-00010450: 7472 5d20 3d20 4e6f 6e65 2c0a 2020 2020  tr] = None,.    
-00010460: 2020 2020 736c 6964 6572 5f63 6f6e 6669      slider_confi
-00010470: 673a 204f 7074 696f 6e61 6c5b 6469 6374  g: Optional[dict
-00010480: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
-00010490: 2020 736c 6964 6572 5f6d 6172 6b73 3a20    slider_marks: 
-000104a0: 4f70 7469 6f6e 616c 5b6c 6973 745b 7475  Optional[list[tu
-000104b0: 706c 655d 5d20 3d20 4e6f 6e65 2c0a 2020  ple]] = None,.  
-000104c0: 2020 293a 0a20 2020 2020 2020 2022 2222    ):.        """
-000104d0: 0a20 2020 2020 2020 2043 7265 6174 6520  .        Create 
-000104e0: 616e 2061 6e6e 6f74 6174 6564 2063 6861  an annotated cha
-000104f0: 7274 2069 6e20 7468 6520 6d65 6e75 2070  rt in the menu p
-00010500: 6174 682e 0a20 2020 2020 2020 203a 7061  ath..        :pa
-00010510: 7261 6d20 6461 7461 3a20 7468 6520 6461  ram data: the da
-00010520: 7461 206f 6620 7468 6520 6368 6172 740a  ta of the chart.
-00010530: 2020 2020 2020 2020 3a70 6172 616d 206f          :param o
-00010540: 7264 6572 3a20 7468 6520 6f72 6465 7220  rder: the order 
-00010550: 6f66 2074 6865 2063 6861 7274 0a20 2020  of the chart.   
-00010560: 2020 2020 203a 7061 7261 6d20 783a 2074       :param x: t
-00010570: 6865 2078 2061 7869 730a 2020 2020 2020  he x axis.      
-00010580: 2020 3a70 6172 616d 2079 3a20 7468 6520    :param y: the 
-00010590: 7920 6178 6973 0a20 2020 2020 2020 203a  y axis.        :
-000105a0: 7061 7261 6d20 616e 6e6f 7461 7469 6f6e  param annotation
-000105b0: 733a 2074 6865 2061 6e6e 6f74 6174 696f  s: the annotatio
-000105c0: 6e73 0a20 2020 2020 2020 203a 7061 7261  ns.        :para
-000105d0: 6d20 726f 7773 5f73 697a 653a 2074 6865  m rows_size: the
-000105e0: 2072 6f77 7320 7369 7a65 206f 6620 7468   rows size of th
-000105f0: 6520 6368 6172 740a 2020 2020 2020 2020  e chart.        
-00010600: 3a70 6172 616d 2063 6f6c 735f 7369 7a65  :param cols_size
-00010610: 3a20 7468 6520 636f 6c75 6d6e 7320 7369  : the columns si
-00010620: 7a65 206f 6620 7468 6520 6368 6172 740a  ze of the chart.
-00010630: 2020 2020 2020 2020 3a70 6172 616d 2070          :param p
-00010640: 6164 6469 6e67 3a20 7468 6520 7061 6464  adding: the padd
-00010650: 696e 6720 6f66 2074 6865 2063 6861 7274  ing of the chart
-00010660: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-00010670: 7469 746c 653a 2074 6865 2074 6974 6c65  title: the title
-00010680: 206f 6620 7468 6520 6368 6172 740a 2020   of the chart.  
-00010690: 2020 2020 2020 3a70 6172 616d 2079 5f61        :param y_a
-000106a0: 7869 735f 6e61 6d65 3a20 7468 6520 6e61  xis_name: the na
-000106b0: 6d65 206f 6620 7468 6520 7920 6178 6973  me of the y axis
-000106c0: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-000106d0: 736c 6964 6572 5f63 6f6e 6669 673a 2074  slider_config: t
-000106e0: 6865 2073 6c69 6465 7220 636f 6e66 6967  he slider config
-000106f0: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-00010700: 736c 6964 6572 5f6d 6172 6b73 3a20 7468  slider_marks: th
-00010710: 6520 736c 6964 6572 206d 6172 6b73 0a20  e slider marks. 
-00010720: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00010730: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
-00010740: 2864 6174 612c 2073 7472 293a 0a20 2020  (data, str):.   
-00010750: 2020 2020 2020 2020 206c 6f67 5f65 7272           log_err
-00010760: 6f72 280a 2020 2020 2020 2020 2020 2020  or(.            
-00010770: 2020 2020 6c6f 6767 6572 2c0a 2020 2020      logger,.    
-00010780: 2020 2020 2020 2020 2020 2020 2241 6e6e              "Ann
-00010790: 6f74 6174 6564 2063 6861 7274 2064 6f65  otated chart doe
-000107a0: 7320 6e6f 7420 7375 7070 6f72 7420 7468  s not support th
-000107b0: 6520 7573 6520 6f66 2073 6861 7265 6420  e use of shared 
-000107c0: 6461 7461 222c 0a20 2020 2020 2020 2020  data",.         
-000107d0: 2020 2020 2020 2044 6174 6145 7272 6f72         DataError
-000107e0: 2c0a 2020 2020 2020 2020 2020 2020 290a  ,.            ).
-000107f0: 0a20 2020 2020 2020 2069 6620 736c 6964  .        if slid
-00010800: 6572 5f63 6f6e 6669 6720 6973 204e 6f6e  er_config is Non
-00010810: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-00010820: 6c69 6465 725f 636f 6e66 6967 203d 207b  lider_config = {
-00010830: 7d0a 0a20 2020 2020 2020 2069 6620 736c  }..        if sl
-00010840: 6964 6572 5f6d 6172 6b73 3a0a 2020 2020  ider_marks:.    
-00010850: 2020 2020 2020 2020 736c 6964 6572 5f63          slider_c
-00010860: 6f6e 6669 675b 226d 6172 6b73 225d 203d  onfig["marks"] =
-00010870: 205b 0a20 2020 2020 2020 2020 2020 2020   [.             
-00010880: 2020 207b 226c 6162 656c 223a 206d 6172     {"label": mar
-00010890: 6b5b 305d 2c20 2276 616c 7565 223a 206d  k[0], "value": m
-000108a0: 6172 6b5b 315d 7d20 666f 7220 6d61 726b  ark[1]} for mark
-000108b0: 2069 6e20 736c 6964 6572 5f6d 6172 6b73   in slider_marks
-000108c0: 0a20 2020 2020 2020 2020 2020 205d 0a0a  .            ]..
-000108d0: 2020 2020 2020 2020 6966 2069 7369 6e73          if isins
-000108e0: 7461 6e63 6528 792c 2073 7472 293a 0a20  tance(y, str):. 
-000108f0: 2020 2020 2020 2020 2020 2079 203d 205b             y = [
-00010900: 795d 0a0a 2020 2020 2020 2020 6966 206e  y]..        if n
-00010910: 6f74 206c 656e 2879 2920 3d3d 206c 656e  ot len(y) == len
-00010920: 2864 6174 6129 3a0a 2020 2020 2020 2020  (data):.        
-00010930: 2020 2020 6c6f 675f 6572 726f 7228 0a20      log_error(. 
-00010940: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-00010950: 6f67 6765 722c 0a20 2020 2020 2020 2020  ogger,.         
-00010960: 2020 2020 2020 2066 224e 756d 6265 7220         f"Number 
-00010970: 6f66 2079 2076 616c 7565 7320 287b 6c65  of y values ({le
-00010980: 6e28 7929 7d29 2064 6f65 7320 6e6f 7420  n(y)}) does not 
-00010990: 6d61 7463 6820 6e75 6d62 6572 206f 6620  match number of 
-000109a0: 6461 7461 6672 616d 6573 2028 7b6c 656e  dataframes ({len
-000109b0: 2864 6174 6129 7d29 222c 0a20 2020 2020  (data)})",.     
-000109c0: 2020 2020 2020 2020 2020 2044 6174 6145             DataE
-000109d0: 7272 6f72 2c0a 2020 2020 2020 2020 2020  rror,.          
-000109e0: 2020 290a 0a20 2020 2020 2020 205f 2c20    )..        _, 
-000109f0: 7265 706f 7274 203d 2061 7761 6974 2073  report = await s
-00010a00: 656c 662e 5f67 6574 5f63 6861 7274 5f72  elf._get_chart_r
-00010a10: 6570 6f72 7428 6f72 6465 722c 2041 6e6e  eport(order, Ann
-00010a20: 6f74 6174 6564 4543 6861 7274 290a 0a20  otatedEChart).. 
-00010a30: 2020 2020 2020 2064 6673 203d 205b 7661         dfs = [va
-00010a40: 6c69 6461 7465 5f64 6174 615f 6973 5f70  lidate_data_is_p
-00010a50: 616e 6461 7261 626c 6528 6466 2920 666f  andarable(df) fo
-00010a60: 7220 6466 2069 6e20 6461 7461 5d0a 2020  r df in data].  
-00010a70: 2020 2020 2020 6461 7461 5f73 6574 5f74        data_set_t
-00010a80: 6173 6b73 203d 205b 5d0a 2020 2020 2020  asks = [].      
-00010a90: 2020 666f 7220 6466 2c20 795f 7661 6c20    for df, y_val 
-00010aa0: 696e 207a 6970 2864 6673 2c20 7929 3a0a  in zip(dfs, y):.
-00010ab0: 2020 2020 2020 2020 2020 2020 6466 5b78              df[x
-00010ac0: 5d20 3d20 7064 2e74 6f5f 6461 7465 7469  ] = pd.to_dateti
-00010ad0: 6d65 2864 665b 785d 290a 2020 2020 2020  me(df[x]).      
-00010ae0: 2020 2020 2020 6966 2061 6e6e 6f74 6174        if annotat
-00010af0: 696f 6e73 2069 6e20 6466 3a0a 2020 2020  ions in df:.    
-00010b00: 2020 2020 2020 2020 2020 2020 6466 5b61              df[a
-00010b10: 6e6e 6f74 6174 696f 6e73 5d20 3d20 280a  nnotations] = (.
-00010b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010b30: 2020 2020 6466 5b61 6e6e 6f74 6174 696f      df[annotatio
-00010b40: 6e73 5d2e 7265 706c 6163 6528 6e70 2e6e  ns].replace(np.n
-00010b50: 616e 2c20 2222 2c20 7265 6765 783d 5472  an, "", regex=Tr
-00010b60: 7565 292e 6173 7479 7065 2873 7472 290a  ue).astype(str).
-00010b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010b80: 290a 2020 2020 2020 2020 2020 2020 6461  ).            da
-00010b90: 7461 5f73 6574 5f74 6173 6b73 2e61 7070  ta_set_tasks.app
-00010ba0: 656e 6428 0a20 2020 2020 2020 2020 2020  end(.           
-00010bb0: 2020 2020 2073 656c 662e 5f63 7265 6174       self._creat
-00010bc0: 655f 6461 7461 5f73 6574 286e 616d 653d  e_data_set(name=
-00010bd0: 6622 7b72 6570 6f72 745b 2769 6427 5d7d  f"{report['id']}
-00010be0: 5f7b 795f 7661 6c7d 222c 2064 6174 613d  _{y_val}", data=
-00010bf0: 6466 290a 2020 2020 2020 2020 2020 2020  df).            
-00010c00: 290a 0a20 2020 2020 2020 2064 6174 615f  )..        data_
-00010c10: 7365 745f 6469 6374 7320 3d20 6177 6169  set_dicts = awai
-00010c20: 7420 6173 796e 6369 6f2e 6761 7468 6572  t asyncio.gather
-00010c30: 282a 6461 7461 5f73 6574 5f74 6173 6b73  (*data_set_tasks
-00010c40: 290a 2020 2020 2020 2020 6461 7461 5f73  ).        data_s
-00010c50: 6574 7320 3d20 5b64 735b 795f 7661 6c5d  ets = [ds[y_val]
-00010c60: 5b31 5d20 666f 7220 6473 2c20 795f 7661  [1] for ds, y_va
-00010c70: 6c20 696e 207a 6970 2864 6174 615f 7365  l in zip(data_se
-00010c80: 745f 6469 6374 732c 2079 295d 0a0a 2020  t_dicts, y)]..  
-00010c90: 2020 2020 2020 7264 5f69 6473 203d 204e        rd_ids = N
-00010ca0: 6f6e 650a 2020 2020 2020 2020 6966 2073  one.        if s
-00010cb0: 656c 662e 7265 7573 655f 6461 7461 5f73  elf.reuse_data_s
-00010cc0: 6574 733a 0a20 2020 2020 2020 2020 2020  ets:.           
-00010cd0: 2072 645f 6964 7320 3d20 6765 745f 7575   rd_ids = get_uu
-00010ce0: 6964 735f 6672 6f6d 5f64 6963 7428 7265  ids_from_dict(re
-00010cf0: 706f 7274 5b22 7072 6f70 6572 7469 6573  port["properties
-00010d00: 225d 5b22 6f70 7469 6f6e 225d 290a 2020  "]["option"]).  
-00010d10: 2020 2020 2020 2020 2020 6966 206c 656e            if len
-00010d20: 2872 645f 6964 7329 203d 3d20 6c65 6e28  (rd_ids) == len(
-00010d30: 7929 3a0a 2020 2020 2020 2020 2020 2020  y):.            
-00010d40: 2020 2020 7265 705f 6473 3a20 6c69 7374      rep_ds: list
-00010d50: 5b52 6570 6f72 742e 5265 706f 7274 4461  [Report.ReportDa
-00010d60: 7461 5365 745d 203d 2061 7761 6974 2072  taSet] = await r
-00010d70: 6570 6f72 742e 6765 745f 7265 706f 7274  eport.get_report
-00010d80: 5f64 6174 615f 7365 7473 2829 0a20 2020  _data_sets().   
-00010d90: 2020 2020 2020 2020 2020 2020 2072 6570               rep
-00010da0: 5f64 7320 3d20 5b0a 2020 2020 2020 2020  _ds = [.        
-00010db0: 2020 2020 2020 2020 2020 2020 6e65 7874              next
-00010dc0: 2828 7264 2066 6f72 2072 6420 696e 2072  ((rd for rd in r
-00010dd0: 6570 5f64 7320 6966 2072 645b 2269 6422  ep_ds if rd["id"
-00010de0: 5d20 3d3d 2072 645f 6964 292c 204e 6f6e  ] == rd_id), Non
-00010df0: 6529 0a20 2020 2020 2020 2020 2020 2020  e).             
-00010e00: 2020 2020 2020 2066 6f72 2072 645f 6964         for rd_id
-00010e10: 2069 6e20 7264 5f69 6473 0a20 2020 2020   in rd_ids.     
-00010e20: 2020 2020 2020 2020 2020 205d 0a20 2020             ].   
-00010e30: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00010e40: 616e 7928 0a20 2020 2020 2020 2020 2020  any(.           
-00010e50: 2020 2020 2020 2020 2072 645b 2264 6174           rd["dat
-00010e60: 6153 6574 4964 225d 2021 3d20 6473 5b22  aSetId"] != ds["
-00010e70: 6964 225d 0a20 2020 2020 2020 2020 2020  id"].           
-00010e80: 2020 2020 2020 2020 206f 7220 7264 5b22           or rd["
-00010e90: 7072 6f70 6572 7469 6573 225d 5b22 6d61  properties"]["ma
-00010ea0: 7070 696e 6722 5d0a 2020 2020 2020 2020  pping"].        
-00010eb0: 2020 2020 2020 2020 2020 2020 213d 207b              != {
-00010ec0: 2276 616c 7565 7322 3a20 5b22 6461 7465  "values": ["date
-00010ed0: 4669 656c 6431 222c 2022 696e 7446 6965  Field1", "intFie
-00010ee0: 6c64 3122 5d2c 2022 6c61 6265 6c22 3a20  ld1"], "label": 
-00010ef0: 2273 7472 696e 6746 6965 6c64 3122 7d0a  "stringField1"}.
-00010f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010f10: 2020 2020 666f 7220 7264 2c20 6473 2069      for rd, ds i
-00010f20: 6e20 7a69 7028 7265 705f 6473 2c20 6461  n zip(rep_ds, da
-00010f30: 7461 5f73 6574 7329 0a20 2020 2020 2020  ta_sets).       
-00010f40: 2020 2020 2020 2020 2029 3a0a 2020 2020           ):.    
-00010f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010f60: 7264 5f69 6473 203d 204e 6f6e 650a 0a20  rd_ids = None.. 
-00010f70: 2020 2020 2020 2069 6620 6e6f 7420 7264         if not rd
-00010f80: 5f69 6473 3a0a 2020 2020 2020 2020 2020  _ids:.          
-00010f90: 2020 6177 6169 7420 7265 706f 7274 2e64    await report.d
-00010fa0: 656c 6574 655f 7265 706f 7274 5f64 6174  elete_report_dat
-00010fb0: 615f 7365 7473 286c 6f67 3d54 7275 6529  a_sets(log=True)
-00010fc0: 0a20 2020 2020 2020 2020 2020 206d 6170  .            map
-00010fd0: 7069 6e67 3a20 4d61 7070 696e 6720 3d20  ping: Mapping = 
-00010fe0: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
-00010ff0: 2020 2276 616c 7565 7322 3a20 5b22 6461    "values": ["da
-00011000: 7465 4669 656c 6431 222c 2022 696e 7446  teField1", "intF
-00011010: 6965 6c64 3122 5d2c 0a20 2020 2020 2020  ield1"],.       
-00011020: 2020 2020 2020 2020 2022 6c61 6265 6c22           "label"
-00011030: 3a20 2273 7472 696e 6746 6965 6c64 3122  : "stringField1"
-00011040: 2c0a 2020 2020 2020 2020 2020 2020 7d0a  ,.            }.
-00011050: 2020 2020 2020 2020 2020 2020 7265 706f              repo
-00011060: 7274 5f64 6174 615f 7365 7473 203d 2061  rt_data_sets = a
-00011070: 7761 6974 2061 7379 6e63 696f 2e67 6174  wait asyncio.gat
-00011080: 6865 7228 0a20 2020 2020 2020 2020 2020  her(.           
-00011090: 2020 2020 202a 5b0a 2020 2020 2020 2020       *[.        
-000110a0: 2020 2020 2020 2020 2020 2020 7265 706f              repo
-000110b0: 7274 2e63 7265 6174 655f 7265 706f 7274  rt.create_report
-000110c0: 5f64 6174 615f 7365 7428 286d 6170 7069  _data_set((mappi
-000110d0: 6e67 2c20 6461 7461 5f73 6574 2c20 4e6f  ng, data_set, No
-000110e0: 6e65 2929 0a20 2020 2020 2020 2020 2020  ne)).           
-000110f0: 2020 2020 2020 2020 2066 6f72 2064 6174           for dat
-00011100: 615f 7365 7420 696e 2064 6174 615f 7365  a_set in data_se
-00011110: 7473 0a20 2020 2020 2020 2020 2020 2020  ts.             
-00011120: 2020 205d 0a20 2020 2020 2020 2020 2020     ].           
-00011130: 2029 0a20 2020 2020 2020 2020 2020 2072   ).            r
-00011140: 645f 6964 7320 3d20 5b72 645b 2269 6422  d_ids = [rd["id"
-00011150: 5d20 666f 7220 7264 2069 6e20 7265 706f  ] for rd in repo
-00011160: 7274 5f64 6174 615f 7365 7473 5d0a 0a20  rt_data_sets].. 
-00011170: 2020 2020 2020 2063 6861 7274 5f6f 7074         chart_opt
-00011180: 696f 6e73 203d 207b 0a20 2020 2020 2020  ions = {.       
-00011190: 2020 2020 2022 7941 7869 7322 3a20 7b0a       "yAxis": {.
-000111a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000111b0: 226e 616d 6522 3a20 795f 6178 6973 5f6e  "name": y_axis_n
-000111c0: 616d 6520 6f72 2022 222c 0a20 2020 2020  ame or "",.     
-000111d0: 2020 2020 2020 2020 2020 2022 666f 6e74             "font
-000111e0: 2220 2274 7970 6522 3a20 2276 616c 7565  " "type": "value
-000111f0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-00011200: 2020 2022 6e61 6d65 4c6f 6361 7469 6f6e     "nameLocation
-00011210: 223a 2022 6d69 6464 6c65 222c 0a20 2020  ": "middle",.   
-00011220: 2020 2020 2020 2020 2020 2020 2022 6e61               "na
-00011230: 6d65 4761 7022 3a20 3330 2c0a 2020 2020  meGap": 30,.    
-00011240: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
-00011250: 2020 2020 2020 2022 7841 7869 7322 3a20         "xAxis": 
-00011260: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
-00011270: 2020 2274 7970 6522 3a20 2274 696d 6522    "type": "time"
-00011280: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00011290: 2020 226e 616d 654c 6f63 6174 696f 6e22    "nameLocation"
-000112a0: 3a20 226d 6964 646c 6522 2c0a 2020 2020  : "middle",.    
-000112b0: 2020 2020 2020 2020 2020 2020 226e 616d              "nam
-000112c0: 6547 6170 223a 2033 302c 0a20 2020 2020  eGap": 30,.     
-000112d0: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
-000112e0: 2020 2020 2020 2273 6572 6965 7322 3a20        "series": 
-000112f0: 5b0a 2020 2020 2020 2020 2020 2020 2020  [.              
-00011300: 2020 7b0a 2020 2020 2020 2020 2020 2020    {.            
-00011310: 2020 2020 2020 2020 2264 6174 6122 3a20          "data": 
-00011320: 2223 7b22 202b 2072 645f 6964 202b 2022  "#{" + rd_id + "
-00011330: 7d22 2c0a 2020 2020 2020 2020 2020 2020  }",.            
-00011340: 2020 2020 2020 2020 2274 7970 6522 3a20          "type": 
-00011350: 226c 696e 6522 2c0a 2020 2020 2020 2020  "line",.        
-00011360: 2020 2020 2020 2020 2020 2020 226e 616d              "nam
-00011370: 6522 3a20 795f 6e61 6d65 2c0a 2020 2020  e": y_name,.    
-00011380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011390: 2269 7465 6d53 7479 6c65 223a 207b 0a20  "itemStyle": {. 
-000113a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000113b0: 2020 2020 2020 2022 626f 7264 6572 5261         "borderRa
-000113c0: 6469 7573 223a 205b 392c 2039 2c20 302c  dius": [9, 9, 0,
-000113d0: 2030 5d2c 0a20 2020 2020 2020 2020 2020   0],.           
-000113e0: 2020 2020 2020 2020 207d 2c0a 2020 2020           },.    
-000113f0: 2020 2020 2020 2020 2020 2020 7d0a 2020              }.  
-00011400: 2020 2020 2020 2020 2020 2020 2020 666f                fo
-00011410: 7220 795f 6e61 6d65 2c20 7264 5f69 6420  r y_name, rd_id 
-00011420: 696e 207a 6970 2879 2c20 7264 5f69 6473  in zip(y, rd_ids
-00011430: 290a 2020 2020 2020 2020 2020 2020 5d2c  ).            ],
-00011440: 0a20 2020 2020 2020 207d 0a20 2020 2020  .        }.     
-00011450: 2020 2061 7761 6974 2073 656c 662e 5f63     await self._c
-00011460: 7265 6174 655f 6368 6172 7428 0a20 2020  reate_chart(.   
-00011470: 2020 2020 2020 2020 2063 6861 7274 5f63           chart_c
-00011480: 6c61 7373 3d41 6e6e 6f74 6174 6564 4543  lass=AnnotatedEC
-00011490: 6861 7274 2c0a 2020 2020 2020 2020 2020  hart,.          
-000114a0: 2020 6f72 6465 723d 6f72 6465 722c 0a20    order=order,. 
-000114b0: 2020 2020 2020 2020 2020 2073 697a 6550             sizeP
-000114c0: 6164 6469 6e67 3d70 6164 6469 6e67 2c0a  adding=padding,.
-000114d0: 2020 2020 2020 2020 2020 2020 7369 7a65              size
-000114e0: 526f 7773 3d72 6f77 735f 7369 7a65 2c0a  Rows=rows_size,.
-000114f0: 2020 2020 2020 2020 2020 2020 7369 7a65              size
-00011500: 436f 6c75 6d6e 733d 636f 6c73 5f73 697a  Columns=cols_siz
-00011510: 652c 0a20 2020 2020 2020 2020 2020 2074  e,.            t
-00011520: 6974 6c65 3d74 6974 6c65 2c0a 2020 2020  itle=title,.    
-00011530: 2020 2020 2020 2020 7072 6f70 6572 7469          properti
-00011540: 6573 3d64 6963 7428 0a20 2020 2020 2020  es=dict(.       
-00011550: 2020 2020 2020 2020 2073 6c69 6465 723d           slider=
-00011560: 736c 6964 6572 5f63 6f6e 6669 672c 0a20  slider_config,. 
-00011570: 2020 2020 2020 2020 2020 2020 2020 206f                 o
-00011580: 7074 696f 6e3d 6368 6172 745f 6f70 7469  ption=chart_opti
-00011590: 6f6e 732c 0a20 2020 2020 2020 2020 2020  ons,.           
-000115a0: 2029 2c0a 2020 2020 2020 2020 290a 0a20   ),.        ).. 
-000115b0: 2020 2061 7379 6e63 2064 6566 205f 6765     async def _ge
-000115c0: 745f 7265 706f 7274 5f64 6174 615f 7365  t_report_data_se
-000115d0: 7473 5f70 6572 5f6d 6170 7069 6e67 280a  ts_per_mapping(.
-000115e0: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
-000115f0: 2020 2020 2020 7265 706f 7274 3a20 5265        report: Re
-00011600: 706f 7274 2c0a 2020 2020 2020 2020 6461  port,.        da
-00011610: 7461 5f6d 6170 7069 6e67 5f74 6f5f 7475  ta_mapping_to_tu
-00011620: 706c 653a 2064 6963 742c 0a20 2020 2020  ple: dict,.     
-00011630: 2020 2066 6965 6c64 733a 206c 6973 745b     fields: list[
-00011640: 556e 696f 6e5b 7475 706c 652c 2064 6963  Union[tuple, dic
-00011650: 745d 5d2c 0a20 2020 2029 202d 3e20 6c69  t]],.    ) -> li
-00011660: 7374 5b52 6570 6f72 742e 5265 706f 7274  st[Report.Report
-00011670: 4461 7461 5365 745d 3a0a 2020 2020 2020  DataSet]:.      
-00011680: 2020 2222 2243 7265 6174 6520 6120 6461    """Create a da
-00011690: 7461 5f73 6574 2070 6572 2066 6965 6c64  ta_set per field
-000116a0: 206f 6620 6120 6461 7461 6672 616d 652e   of a dataframe.
-000116b0: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-000116c0: 7265 706f 7274 3a20 7468 6520 7265 706f  report: the repo
-000116d0: 7274 0a20 2020 2020 2020 203a 7061 7261  rt.        :para
-000116e0: 6d20 6461 7461 5f6d 6170 7069 6e67 5f74  m data_mapping_t
-000116f0: 6f5f 7475 706c 653a 2074 6865 206d 6170  o_tuple: the map
-00011700: 7069 6e67 206f 6620 7468 6520 6461 7461  ping of the data
-00011710: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-00011720: 6669 656c 6473 3a20 7468 6520 6669 656c  fields: the fiel
-00011730: 6473 206f 6620 7468 6520 6461 7461 2074  ds of the data t
-00011740: 6f20 6265 2075 7365 640a 2020 2020 2020  o be used.      
-00011750: 2020 3a72 6574 7572 6e3a 2074 6865 206c    :return: the l
-00011760: 6973 7420 6f66 2064 6174 6120 7365 7473  ist of data sets
-00011770: 2070 6172 7469 7469 6f6e 6564 2062 7920   partitioned by 
-00011780: 6178 6973 2061 6e64 2066 6965 6c64 730a  axis and fields.
-00011790: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-000117a0: 2020 2020 7461 736b 7320 3d20 5b5d 0a20      tasks = []. 
-000117b0: 2020 2020 2020 2066 6965 6c64 7320 3d20         fields = 
-000117c0: 6669 656c 6473 2069 6620 6669 656c 6473  fields if fields
-000117d0: 2065 6c73 6520 5b5d 0a20 2020 2020 2020   else [].       
-000117e0: 2066 6f72 2069 2c20 6620 696e 2065 6e75   for i, f in enu
-000117f0: 6d65 7261 7465 2866 6965 6c64 7329 3a0a  merate(fields):.
-00011800: 2020 2020 2020 2020 2020 2020 6d61 7070              mapp
-00011810: 696e 6720 3d20 5b5d 0a20 2020 2020 2020  ing = [].       
-00011820: 2020 2020 2064 6174 615f 7365 7420 3d20       data_set = 
-00011830: 4e6f 6e65 0a20 2020 2020 2020 2020 2020  None.           
-00011840: 2072 6573 5f73 6f72 7420 3d20 4e6f 6e65   res_sort = None
-00011850: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00011860: 6973 696e 7374 616e 6365 2866 2c20 7374  isinstance(f, st
-00011870: 7229 3a0a 2020 2020 2020 2020 2020 2020  r):.            
-00011880: 2020 2020 6966 2066 206e 6f74 2069 6e20      if f not in 
-00011890: 6461 7461 5f6d 6170 7069 6e67 5f74 6f5f  data_mapping_to_
-000118a0: 7475 706c 653a 0a20 2020 2020 2020 2020  tuple:.         
-000118b0: 2020 2020 2020 2020 2020 206c 6f67 5f65             log_e
-000118c0: 7272 6f72 286c 6f67 6765 722c 2066 2246  rror(logger, f"F
-000118d0: 6965 6c64 207b 667d 206e 6f74 2066 6f75  ield {f} not fou
-000118e0: 6e64 2069 6e20 6461 7461 222c 2044 6174  nd in data", Dat
-000118f0: 6145 7272 6f72 290a 2020 2020 2020 2020  aError).        
-00011900: 2020 2020 2020 2020 6d61 7070 696e 672c          mapping,
-00011910: 2064 6174 615f 7365 742c 2072 6573 5f73   data_set, res_s
-00011920: 6f72 7420 3d20 6461 7461 5f6d 6170 7069  ort = data_mappi
-00011930: 6e67 5f74 6f5f 7475 706c 655b 665d 0a20  ng_to_tuple[f]. 
-00011940: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
-00011950: 6973 696e 7374 616e 6365 2866 2c20 2874  isinstance(f, (t
-00011960: 7570 6c65 2c20 6c69 7374 2929 3a0a 2020  uple, list)):.  
-00011970: 2020 2020 2020 2020 2020 2020 2020 666f                fo
-00011980: 7220 665f 2069 6e20 663a 0a20 2020 2020  r f_ in f:.     
-00011990: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-000119a0: 6620 665f 206e 6f74 2069 6e20 6461 7461  f f_ not in data
-000119b0: 5f6d 6170 7069 6e67 5f74 6f5f 7475 706c  _mapping_to_tupl
-000119c0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-000119d0: 2020 2020 2020 2020 2020 206c 6f67 5f65             log_e
-000119e0: 7272 6f72 286c 6f67 6765 722c 2066 2246  rror(logger, f"F
-000119f0: 6965 6c64 207b 665f 7d20 6e6f 7420 666f  ield {f_} not fo
-00011a00: 756e 6420 696e 2064 6174 6122 2c20 4461  und in data", Da
-00011a10: 7461 4572 726f 7229 0a20 2020 2020 2020  taError).       
-00011a20: 2020 2020 2020 2020 2020 2020 206d 6170               map
-00011a30: 7069 6e67 5f2c 2064 6174 615f 7365 745f  ping_, data_set_
-00011a40: 2c20 7265 735f 736f 7274 5f20 3d20 6461  , res_sort_ = da
-00011a50: 7461 5f6d 6170 7069 6e67 5f74 6f5f 7475  ta_mapping_to_tu
-00011a60: 706c 655b 665f 5d0a 2020 2020 2020 2020  ple[f_].        
-00011a70: 2020 2020 2020 2020 2020 2020 6d61 7070              mapp
-00011a80: 696e 672e 6170 7065 6e64 286d 6170 7069  ing.append(mappi
-00011a90: 6e67 5f29 0a20 2020 2020 2020 2020 2020  ng_).           
-00011aa0: 2020 2020 2020 2020 2064 6174 615f 7365           data_se
-00011ab0: 7420 3d20 6461 7461 5f73 6574 2069 6620  t = data_set if 
-00011ac0: 6461 7461 5f73 6574 2065 6c73 6520 6461  data_set else da
-00011ad0: 7461 5f73 6574 5f0a 2020 2020 2020 2020  ta_set_.        
-00011ae0: 2020 2020 2020 2020 2020 2020 7265 735f              res_
-00011af0: 736f 7274 203d 2072 6573 5f73 6f72 7420  sort = res_sort 
-00011b00: 6966 2072 6573 5f73 6f72 7420 656c 7365  if res_sort else
-00011b10: 2072 6573 5f73 6f72 745f 0a20 2020 2020   res_sort_.     
-00011b20: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-00011b30: 7373 6572 7420 6461 7461 5f73 6574 203d  ssert data_set =
-00011b40: 3d20 6461 7461 5f73 6574 5f0a 2020 2020  = data_set_.    
-00011b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011b60: 6173 7365 7274 2072 6573 5f73 6f72 7420  assert res_sort 
-00011b70: 3d3d 2072 6573 5f73 6f72 745f 0a20 2020  == res_sort_.   
-00011b80: 2020 2020 2020 2020 2065 6c69 6620 6973           elif is
-00011b90: 696e 7374 616e 6365 2866 2c20 6469 6374  instance(f, dict
-00011ba0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00011bb0: 2020 206d 6170 7069 6e67 203d 207b 6b3a     mapping = {k:
-00011bc0: 205b 5d20 666f 7220 6b20 696e 2066 2e6b   [] for k in f.k
-00011bd0: 6579 7328 297d 0a20 2020 2020 2020 2020  eys()}.         
-00011be0: 2020 2020 2020 2066 6f72 206b 2c20 665f         for k, f_
-00011bf0: 2069 6e20 662e 6974 656d 7328 293a 0a20   in f.items():. 
-00011c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011c10: 2020 2069 6620 665f 206e 6f74 2069 6e20     if f_ not in 
-00011c20: 6461 7461 5f6d 6170 7069 6e67 5f74 6f5f  data_mapping_to_
-00011c30: 7475 706c 653a 0a20 2020 2020 2020 2020  tuple:.         
-00011c40: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-00011c50: 6f67 5f65 7272 6f72 286c 6f67 6765 722c  og_error(logger,
-00011c60: 2066 2246 6965 6c64 207b 665f 7d20 6e6f   f"Field {f_} no
-00011c70: 7420 666f 756e 6420 696e 2064 6174 6122  t found in data"
-00011c80: 2c20 4461 7461 4572 726f 7229 0a20 2020  , DataError).   
-00011c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011ca0: 206d 6170 7069 6e67 5f2c 2064 6174 615f   mapping_, data_
-00011cb0: 7365 745f 2c20 7265 735f 736f 7274 5f20  set_, res_sort_ 
-00011cc0: 3d20 6461 7461 5f6d 6170 7069 6e67 5f74  = data_mapping_t
-00011cd0: 6f5f 7475 706c 655b 665f 5d0a 2020 2020  o_tuple[f_].    
-00011ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011cf0: 6d61 7070 696e 675b 6b5d 203d 206d 6170  mapping[k] = map
-00011d00: 7069 6e67 5f0a 2020 2020 2020 2020 2020  ping_.          
-00011d10: 2020 2020 2020 2020 2020 6461 7461 5f73            data_s
-00011d20: 6574 203d 2064 6174 615f 7365 7420 6966  et = data_set if
-00011d30: 2064 6174 615f 7365 7420 656c 7365 2064   data_set else d
-00011d40: 6174 615f 7365 745f 0a20 2020 2020 2020  ata_set_.       
-00011d50: 2020 2020 2020 2020 2020 2020 2072 6573               res
-00011d60: 5f73 6f72 7420 3d20 7265 735f 736f 7274  _sort = res_sort
-00011d70: 2069 6620 7265 735f 736f 7274 2065 6c73   if res_sort els
-00011d80: 6520 7265 735f 736f 7274 5f0a 2020 2020  e res_sort_.    
-00011d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011da0: 6173 7365 7274 2064 6174 615f 7365 7420  assert data_set 
-00011db0: 3d3d 2064 6174 615f 7365 745f 0a20 2020  == data_set_.   
-00011dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011dd0: 2061 7373 6572 7420 7265 735f 736f 7274   assert res_sort
-00011de0: 203d 3d20 7265 735f 736f 7274 5f0a 2020   == res_sort_.  
-00011df0: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
-00011e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011e10: 6c6f 675f 6572 726f 7228 0a20 2020 2020  log_error(.     
-00011e20: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-00011e30: 6f67 6765 722c 2066 2246 6965 6c64 207b  ogger, f"Field {
-00011e40: 667d 2069 7320 6e6f 7420 6120 7374 7269  f} is not a stri
-00011e50: 6e67 2c20 7475 706c 652c 206c 6973 7420  ng, tuple, list 
-00011e60: 6f72 2064 6963 7422 2c20 4461 7461 4572  or dict", DataEr
-00011e70: 726f 720a 2020 2020 2020 2020 2020 2020  ror.            
-00011e80: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-00011e90: 2020 7461 736b 732e 6170 7065 6e64 280a    tasks.append(.
-00011ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011eb0: 7265 706f 7274 2e63 7265 6174 655f 7265  report.create_re
-00011ec0: 706f 7274 5f64 6174 615f 7365 7428 0a20  port_data_set(. 
-00011ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011ee0: 2020 206d 6170 7069 6e67 5f64 6174 615f     mapping_data_
-00011ef0: 7365 745f 736f 7274 3d28 6d61 7070 696e  set_sort=(mappin
-00011f00: 672c 2064 6174 615f 7365 742c 2072 6573  g, data_set, res
-00011f10: 5f73 6f72 7429 0a20 2020 2020 2020 2020  _sort).         
-00011f20: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-00011f30: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
-00011f40: 7265 706f 7274 5f64 6174 615f 7365 7473  report_data_sets
-00011f50: 203d 2061 7761 6974 2061 7379 6e63 696f   = await asyncio
-00011f60: 2e67 6174 6865 7228 2a74 6173 6b73 290a  .gather(*tasks).
-00011f70: 2020 2020 2020 2020 6c6f 6767 6572 2e69          logger.i
-00011f80: 6e66 6f28 0a20 2020 2020 2020 2020 2020  nfo(.           
-00011f90: 2066 2243 7265 6174 6564 207b 6c65 6e28   f"Created {len(
-00011fa0: 7265 706f 7274 5f64 6174 615f 7365 7473  report_data_sets
-00011fb0: 297d 2063 6f6d 706f 6e65 6e74 2064 6174  )} component dat
-00011fc0: 6120 7365 7420 6c69 6e6b 7320 666f 7220  a set links for 
-00011fd0: 636f 6d70 6f6e 656e 7420 7b73 7472 2872  component {str(r
-00011fe0: 6570 6f72 7429 7d22 0a20 2020 2020 2020  eport)}".       
-00011ff0: 2029 0a20 2020 2020 2020 2072 6574 7572   ).        retur
-00012000: 6e20 7265 706f 7274 5f64 6174 615f 7365  n report_data_se
-00012010: 7473 0a0a 2020 2020 6465 6620 5f75 7064  ts..    def _upd
-00012020: 6174 655f 6f70 7469 6f6e 7328 7365 6c66  ate_options(self
-00012030: 2c20 6f70 7469 6f6e 733a 2064 6963 742c  , options: dict,
-00012040: 206f 7074 696f 6e5f 6d6f 6469 6669 6361   option_modifica
-00012050: 7469 6f6e 733a 204f 7074 696f 6e61 6c5b  tions: Optional[
-00012060: 6469 6374 5d29 3a0a 2020 2020 2020 2020  dict]):.        
-00012070: 2222 2255 7064 6174 6520 7468 6520 6f70  """Update the op
-00012080: 7469 6f6e 7320 6f66 2061 6e20 6563 6861  tions of an echa
-00012090: 7274 2e0a 2020 2020 2020 2020 3a70 6172  rt..        :par
-000120a0: 616d 206f 7074 696f 6e73 3a20 7468 6520  am options: the 
-000120b0: 6f70 7469 6f6e 7320 6f66 2074 6865 2065  options of the e
-000120c0: 6368 6172 740a 2020 2020 2020 2020 3a70  chart.        :p
-000120d0: 6172 616d 206f 7074 696f 6e5f 6d6f 6469  aram option_modi
-000120e0: 6669 6361 7469 6f6e 733a 2074 6865 206d  fications: the m
-000120f0: 6f64 6966 6963 6174 696f 6e73 2074 6f20  odifications to 
-00012100: 6170 706c 7920 746f 2074 6865 206f 7074  apply to the opt
-00012110: 696f 6e73 0a20 2020 2020 2020 2022 2222  ions.        """
-00012120: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
-00012130: 6f70 7469 6f6e 5f6d 6f64 6966 6963 6174  option_modificat
-00012140: 696f 6e73 3a0a 2020 2020 2020 2020 2020  ions:.          
-00012150: 2020 7265 7475 726e 0a20 2020 2020 2020    return.       
-00012160: 2066 6f72 206b 2c20 7620 696e 206f 7074   for k, v in opt
-00012170: 696f 6e5f 6d6f 6469 6669 6361 7469 6f6e  ion_modification
-00012180: 732e 6974 656d 7328 293a 0a20 2020 2020  s.items():.     
-00012190: 2020 2020 2020 2069 6620 6b20 3d3d 2022         if k == "
-000121a0: 7365 7269 6573 223a 0a20 2020 2020 2020  series":.       
-000121b0: 2020 2020 2020 2020 206c 6f67 5f65 7272           log_err
-000121c0: 6f72 286c 6f67 6765 722c 2022 5365 7269  or(logger, "Seri
-000121d0: 6573 2063 616e 6e6f 7420 6265 206d 6f64  es cannot be mod
-000121e0: 6966 6965 6422 2c20 4461 7461 4572 726f  ified", DataErro
-000121f0: 7229 0a20 2020 2020 2020 2020 2020 2069  r).            i
-00012200: 6620 6b20 3d3d 2022 7841 7869 7322 206f  f k == "xAxis" o
-00012210: 7220 6b20 3d3d 2022 7941 7869 7322 3a0a  r k == "yAxis":.
-00012220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012230: 6966 2069 7369 6e73 7461 6e63 6528 762c  if isinstance(v,
-00012240: 2064 6963 7429 3a0a 2020 2020 2020 2020   dict):.        
-00012250: 2020 2020 2020 2020 2020 2020 7620 3d20              v = 
-00012260: 5b76 5d0a 2020 2020 2020 2020 2020 2020  [v].            
-00012270: 2020 2020 6966 206c 656e 2876 2920 213d      if len(v) !=
-00012280: 206c 656e 286f 7074 696f 6e73 5b6b 5d29   len(options[k])
-00012290: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-000122a0: 2020 2020 2020 6c6f 675f 6572 726f 7228        log_error(
-000122b0: 6c6f 6767 6572 2c20 6622 5468 6520 6e75  logger, f"The nu
-000122c0: 6d62 6572 206f 6620 7b6b 7d20 6d75 7374  mber of {k} must
-000122d0: 2062 6520 7b6c 656e 2876 297d 222c 2044   be {len(v)}", D
-000122e0: 6174 6145 7272 6f72 290a 2020 2020 2020  ataError).      
-000122f0: 2020 2020 2020 2020 2020 666f 7220 692c            for i,
-00012300: 2076 5f20 696e 2065 6e75 6d65 7261 7465   v_ in enumerate
-00012310: 2876 293a 0a20 2020 2020 2020 2020 2020  (v):.           
-00012320: 2020 2020 2020 2020 206f 7074 696f 6e73           options
-00012330: 5b6b 5d5b 695d 2e75 7064 6174 6528 765f  [k][i].update(v_
-00012340: 290a 2020 2020 2020 2020 2020 2020 656c  ).            el
-00012350: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-00012360: 2020 2020 6f70 7469 6f6e 735b 6b5d 203d      options[k] =
-00012370: 2076 0a0a 2020 2020 6173 796e 6320 6465   v..    async de
-00012380: 6620 5f63 7265 6174 655f 6563 6861 7274  f _create_echart
-00012390: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
-000123a0: 2020 2020 2020 2020 6f70 7469 6f6e 733a          options:
-000123b0: 2064 6963 742c 0a20 2020 2020 2020 206f   dict,.        o
-000123c0: 7264 6572 3a20 696e 742c 0a20 2020 2020  rder: int,.     
-000123d0: 2020 2066 6965 6c64 733a 206c 6973 745b     fields: list[
-000123e0: 556e 696f 6e5b 7374 722c 2074 7570 6c65  Union[str, tuple
-000123f0: 2c20 6469 6374 5d5d 2c0a 2020 2020 2020  , dict]],.      
-00012400: 2020 6461 7461 5f6d 6170 7069 6e67 5f74    data_mapping_t
-00012410: 6f5f 7475 706c 6573 3a20 4f70 7469 6f6e  o_tuples: Option
-00012420: 616c 5b64 6963 745d 203d 204e 6f6e 652c  al[dict] = None,
-00012430: 0a20 2020 2020 2020 2064 6174 613a 204f  .        data: O
-00012440: 7074 696f 6e61 6c5b 556e 696f 6e5b 7374  ptional[Union[st
-00012450: 722c 2070 642e 4461 7461 4672 616d 655d  r, pd.DataFrame]
-00012460: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
-00012470: 2020 6475 6d70 5f77 686f 6c65 3a20 626f    dump_whole: bo
-00012480: 6f6c 203d 2046 616c 7365 2c0a 2020 2020  ol = False,.    
-00012490: 2020 2020 6f70 7469 6f6e 5f6d 6f64 6966      option_modif
-000124a0: 6963 6174 696f 6e73 3a20 4f70 7469 6f6e  ications: Option
-000124b0: 616c 5b64 6963 745d 203d 204e 6f6e 652c  al[dict] = None,
-000124c0: 0a20 2020 2020 2020 2074 6974 6c65 3a20  .        title: 
-000124d0: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
-000124e0: 4e6f 6e65 2c0a 2020 2020 2020 2020 726f  None,.        ro
-000124f0: 7773 5f73 697a 653a 204f 7074 696f 6e61  ws_size: Optiona
-00012500: 6c5b 696e 745d 203d 204e 6f6e 652c 0a20  l[int] = None,. 
-00012510: 2020 2020 2020 2063 6f6c 735f 7369 7a65         cols_size
-00012520: 3a20 4f70 7469 6f6e 616c 5b69 6e74 5d20  : Optional[int] 
-00012530: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-00012540: 7061 6464 696e 673a 204f 7074 696f 6e61  padding: Optiona
-00012550: 6c5b 7374 725d 203d 204e 6f6e 652c 0a20  l[str] = None,. 
-00012560: 2020 2029 3a0a 2020 2020 2020 2020 2222     ):.        ""
-00012570: 220a 2020 2020 2020 2020 4372 6561 7465  ".        Create
-00012580: 2061 6e20 6563 6861 7274 2069 6e20 7468   an echart in th
-00012590: 6520 6461 7368 626f 6172 642c 2066 696c  e dashboard, fil
-000125a0: 6c20 696e 2074 6865 2064 6174 6120 7265  l in the data re
-000125b0: 6665 7265 6e63 6564 2069 6e20 7468 6520  ferenced in the 
-000125c0: 6563 6861 7274 5f6f 7074 696f 6e73 2061  echart_options a
-000125d0: 6e64 2063 7265 6174 6520 6f72 0a20 2020  nd create or.   
-000125e0: 2020 2020 2075 7064 6174 6520 7468 6520       update the 
-000125f0: 6368 6172 7420 616e 6420 6461 7461 2073  chart and data s
-00012600: 6574 206c 696e 6b73 2e0a 2020 2020 2020  et links..      
-00012610: 2020 3a70 6172 616d 206f 7074 696f 6e73    :param options
-00012620: 3a20 7468 6520 6f70 7469 6f6e 7320 6f66  : the options of
-00012630: 2074 6865 2065 6368 6172 740a 2020 2020   the echart.    
-00012640: 2020 2020 3a70 6172 616d 2064 6174 615f      :param data_
-00012650: 6d61 7070 696e 675f 746f 5f74 7570 6c65  mapping_to_tuple
-00012660: 733a 2074 6865 206d 6170 7069 6e67 206f  s: the mapping o
-00012670: 6620 7468 6520 6461 7461 2074 6f20 7468  f the data to th
-00012680: 6520 7475 706c 6573 0a20 2020 2020 2020  e tuples.       
-00012690: 203a 7061 7261 6d20 6461 7461 3a20 7468   :param data: th
-000126a0: 6520 6461 7461 206f 6620 7468 6520 6563  e data of the ec
-000126b0: 6861 7274 0a20 2020 2020 2020 203a 7061  hart.        :pa
-000126c0: 7261 6d20 6475 6d70 5f77 686f 6c65 3a20  ram dump_whole: 
-000126d0: 7768 6574 6865 7220 746f 2064 756d 7020  whether to dump 
-000126e0: 7468 6520 7768 6f6c 6520 6461 7461 0a20  the whole data. 
-000126f0: 2020 2020 2020 203a 7061 7261 6d20 6f70         :param op
-00012700: 7469 6f6e 5f6d 6f64 6966 6963 6174 696f  tion_modificatio
-00012710: 6e73 3a20 7468 6520 6d6f 6469 6669 6361  ns: the modifica
-00012720: 7469 6f6e 7320 746f 2061 7070 6c79 2074  tions to apply t
-00012730: 6f20 7468 6520 6f70 7469 6f6e 730a 2020  o the options.  
-00012740: 2020 2020 2020 3a70 6172 616d 2074 6974        :param tit
-00012750: 6c65 3a20 7468 6520 7469 746c 6520 6f66  le: the title of
-00012760: 2074 6865 2065 6368 6172 740a 2020 2020   the echart.    
-00012770: 2020 2020 3a70 6172 616d 2072 6f77 735f      :param rows_
-00012780: 7369 7a65 3a20 7468 6520 726f 7773 2073  size: the rows s
-00012790: 697a 6520 6f66 2074 6865 2065 6368 6172  ize of the echar
-000127a0: 740a 2020 2020 2020 2020 3a70 6172 616d  t.        :param
-000127b0: 2063 6f6c 735f 7369 7a65 3a20 7468 6520   cols_size: the 
-000127c0: 636f 6c75 6d6e 7320 7369 7a65 206f 6620  columns size of 
-000127d0: 7468 6520 6563 6861 7274 0a20 2020 2020  the echart.     
-000127e0: 2020 203a 7061 7261 6d20 7061 6464 696e     :param paddin
-000127f0: 673a 2074 6865 2070 6164 6469 6e67 206f  g: the padding o
-00012800: 6620 7468 6520 6563 6861 7274 0a20 2020  f the echart.   
-00012810: 2020 2020 2022 2222 0a0a 2020 2020 2020       """..      
-00012820: 2020 6966 2064 6174 6120 6973 206e 6f74    if data is not
-00012830: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00012840: 2020 2064 6174 615f 6d61 7070 696e 675f     data_mapping_
-00012850: 746f 5f74 7570 6c65 7320 3d20 6177 6169  to_tuples = awai
-00012860: 7420 7365 6c66 2e5f 6368 6f6f 7365 5f64  t self._choose_d
-00012870: 6174 6128 0a20 2020 2020 2020 2020 2020  ata(.           
-00012880: 2020 2020 206f 7264 6572 2c20 6461 7461       order, data
-00012890: 2c20 6475 6d70 5f77 686f 6c65 3d64 756d  , dump_whole=dum
-000128a0: 705f 7768 6f6c 650a 2020 2020 2020 2020  p_whole.        
-000128b0: 2020 2020 290a 0a20 2020 2020 2020 2064      )..        d
-000128c0: 6174 615f 6b65 795f 656e 7472 6965 7320  ata_key_entries 
-000128d0: 3d20 6765 745f 6461 7461 5f72 6566 6572  = get_data_refer
-000128e0: 656e 6365 735f 6672 6f6d 5f64 6963 7428  ences_from_dict(
-000128f0: 6f70 7469 6f6e 7329 0a20 2020 2020 2020  options).       
-00012900: 205f 2c20 7265 706f 7274 203d 2061 7761   _, report = awa
-00012910: 6974 2073 656c 662e 5f67 6574 5f63 6861  it self._get_cha
-00012920: 7274 5f72 6570 6f72 7428 6f72 6465 722c  rt_report(order,
-00012930: 2045 4368 6172 7429 0a0a 2020 2020 2020   EChart)..      
-00012940: 2020 7264 5f69 6473 203d 204e 6f6e 650a    rd_ids = None.
-00012950: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00012960: 7265 7573 655f 6461 7461 5f73 6574 733a  reuse_data_sets:
-00012970: 0a20 2020 2020 2020 2020 2020 2072 645f  .            rd_
-00012980: 6964 7320 3d20 6765 745f 7575 6964 735f  ids = get_uuids_
-00012990: 6672 6f6d 5f64 6963 7428 7265 706f 7274  from_dict(report
-000129a0: 5b22 7072 6f70 6572 7469 6573 225d 5b22  ["properties"]["
-000129b0: 6f70 7469 6f6e 225d 290a 2020 2020 2020  option"]).      
-000129c0: 2020 2020 2020 6966 206c 656e 2872 645f        if len(rd_
-000129d0: 6964 7329 203d 3d20 6c65 6e28 6669 656c  ids) == len(fiel
-000129e0: 6473 293a 0a20 2020 2020 2020 2020 2020  ds):.           
-000129f0: 2020 2020 2072 6570 5f64 733a 206c 6973       rep_ds: lis
-00012a00: 745b 5265 706f 7274 2e52 6570 6f72 7444  t[Report.ReportD
-00012a10: 6174 6153 6574 5d20 3d20 6177 6169 7420  ataSet] = await 
-00012a20: 7265 706f 7274 2e67 6574 5f72 6570 6f72  report.get_repor
-00012a30: 745f 6461 7461 5f73 6574 7328 290a 2020  t_data_sets().  
-00012a40: 2020 2020 2020 2020 2020 2020 2020 6d61                ma
-00012a50: 7070 6564 5f66 203d 205b 0a20 2020 2020  pped_f = [.     
-00012a60: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00012a70: 656c 662e 5f67 6574 5f66 6965 6c64 5f6d  elf._get_field_m
-00012a80: 6170 7069 6e67 2866 6965 6c64 2c20 6461  apping(field, da
-00012a90: 7461 5f6d 6170 7069 6e67 5f74 6f5f 7475  ta_mapping_to_tu
-00012aa0: 706c 6573 290a 2020 2020 2020 2020 2020  ples).          
-00012ab0: 2020 2020 2020 2020 2020 666f 7220 6669            for fi
-00012ac0: 656c 6420 696e 2066 6965 6c64 730a 2020  eld in fields.  
-00012ad0: 2020 2020 2020 2020 2020 2020 2020 5d0a                ].
-00012ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012af0: 666f 7220 692c 2072 645f 6964 2069 6e20  for i, rd_id in 
-00012b00: 656e 756d 6572 6174 6528 7264 5f69 6473  enumerate(rd_ids
-00012b10: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00012b20: 2020 2020 2020 2072 6570 6f72 745f 6461         report_da
-00012b30: 7461 5f73 6574 203d 206e 6578 7428 0a20  ta_set = next(. 
-00012b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012b50: 2020 2020 2020 2028 7264 2066 6f72 2072         (rd for r
-00012b60: 6420 696e 2072 6570 5f64 7320 6966 2072  d in rep_ds if r
-00012b70: 645b 2269 6422 5d20 3d3d 2072 645f 6964  d["id"] == rd_id
-00012b80: 292c 204e 6f6e 650a 2020 2020 2020 2020  ), None.        
-00012b90: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-00012ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012bb0: 2020 6966 2028 0a20 2020 2020 2020 2020    if (.         
-00012bc0: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-00012bd0: 6f74 2072 6570 6f72 745f 6461 7461 5f73  ot report_data_s
-00012be0: 6574 0a20 2020 2020 2020 2020 2020 2020  et.             
-00012bf0: 2020 2020 2020 2020 2020 206f 7220 6e6f             or no
-00012c00: 7420 7365 6c66 2e5f 6368 6563 6b5f 6d61  t self._check_ma
-00012c10: 7070 696e 675f 696e 5f72 6570 6f72 745f  pping_in_report_
-00012c20: 6461 7461 5f73 6574 280a 2020 2020 2020  data_set(.      
-00012c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012c40: 2020 2020 2020 7265 706f 7274 5f64 6174        report_dat
-00012c50: 615f 7365 742c 206d 6170 7065 645f 665b  a_set, mapped_f[
-00012c60: 695d 0a20 2020 2020 2020 2020 2020 2020  i].             
-00012c70: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-00012c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012c90: 2029 3a0a 2020 2020 2020 2020 2020 2020   ):.            
-00012ca0: 2020 2020 2020 2020 2020 2020 7264 5f69              rd_i
-00012cb0: 6473 203d 204e 6f6e 650a 2020 2020 2020  ds = None.      
-00012cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012cd0: 2020 6272 6561 6b0a 2020 2020 2020 2020    break.        
-00012ce0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00012cf0: 2020 2020 2020 2020 2020 7264 5f69 6473            rd_ids
-00012d00: 203d 204e 6f6e 650a 0a20 2020 2020 2020   = None..       
-00012d10: 2069 6620 6e6f 7420 7264 5f69 6473 3a0a   if not rd_ids:.
-00012d20: 2020 2020 2020 2020 2020 2020 6177 6169              awai
-00012d30: 7420 7265 706f 7274 2e64 656c 6574 655f  t report.delete_
-00012d40: 7265 706f 7274 5f64 6174 615f 7365 7473  report_data_sets
-00012d50: 286c 6f67 3d54 7275 6529 0a20 2020 2020  (log=True).     
-00012d60: 2020 2020 2020 2072 6570 6f72 745f 6461         report_da
-00012d70: 7461 5f73 6574 7320 3d20 6177 6169 7420  ta_sets = await 
-00012d80: 7365 6c66 2e5f 6765 745f 7265 706f 7274  self._get_report
-00012d90: 5f64 6174 615f 7365 7473 5f70 6572 5f6d  _data_sets_per_m
-00012da0: 6170 7069 6e67 280a 2020 2020 2020 2020  apping(.        
-00012db0: 2020 2020 2020 2020 7265 706f 7274 2c20          report, 
-00012dc0: 6461 7461 5f6d 6170 7069 6e67 5f74 6f5f  data_mapping_to_
-00012dd0: 7475 706c 6573 2c20 6669 656c 6473 0a20  tuples, fields. 
-00012de0: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-00012df0: 2020 2020 2020 2020 2072 645f 6964 7320           rd_ids 
-00012e00: 3d20 5b72 645b 2269 6422 5d20 666f 7220  = [rd["id"] for 
-00012e10: 7264 2069 6e20 7265 706f 7274 5f64 6174  rd in report_dat
-00012e20: 615f 7365 7473 5d0a 0a20 2020 2020 2020  a_sets]..       
-00012e30: 2073 656c 662e 5f75 7064 6174 655f 6f70   self._update_op
-00012e40: 7469 6f6e 7328 6f70 7469 6f6e 732c 206f  tions(options, o
-00012e50: 7074 696f 6e5f 6d6f 6469 6669 6361 7469  ption_modificati
-00012e60: 6f6e 7329 0a0a 2020 2020 2020 2020 6966  ons)..        if
-00012e70: 206c 656e 2872 645f 6964 7329 2021 3d20   len(rd_ids) != 
-00012e80: 6c65 6e28 6461 7461 5f6b 6579 5f65 6e74  len(data_key_ent
-00012e90: 7269 6573 293a 0a20 2020 2020 2020 2020  ries):.         
-00012ea0: 2020 206c 6f67 5f65 7272 6f72 280a 2020     log_error(.  
-00012eb0: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
-00012ec0: 6767 6572 2c0a 2020 2020 2020 2020 2020  gger,.          
-00012ed0: 2020 2020 2020 6622 5468 6520 6e75 6d62        f"The numb
-00012ee0: 6572 206f 6620 6461 7461 2072 6566 6572  er of data refer
-00012ef0: 656e 6365 7320 616e 6420 6669 656c 6473  ences and fields
-00012f00: 206d 7573 7420 6265 2065 7175 616c 2c20   must be equal, 
-00012f10: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-00012f20: 2020 6622 7468 6579 2061 7265 207b 6c65    f"they are {le
-00012f30: 6e28 6461 7461 5f6b 6579 5f65 6e74 7269  n(data_key_entri
-00012f40: 6573 297d 2061 6e64 207b 6c65 6e28 7264  es)} and {len(rd
-00012f50: 5f69 6473 297d 2072 6573 7065 6374 6976  _ids)} respectiv
-00012f60: 656c 792e 222c 0a20 2020 2020 2020 2020  ely.",.         
-00012f70: 2020 2020 2020 2044 6174 6145 7272 6f72         DataError
-00012f80: 2c0a 2020 2020 2020 2020 2020 2020 290a  ,.            ).
-00012f90: 0a20 2020 2020 2020 2066 6f72 2069 2c20  .        for i, 
-00012fa0: 6461 7461 5f6b 6579 5f65 6e74 7279 2069  data_key_entry i
-00012fb0: 6e20 656e 756d 6572 6174 6528 6461 7461  n enumerate(data
-00012fc0: 5f6b 6579 5f65 6e74 7269 6573 293a 0a20  _key_entries):. 
-00012fd0: 2020 2020 2020 2020 2020 2064 6174 6120             data 
-00012fe0: 3d20 6f70 7469 6f6e 730a 2020 2020 2020  = options.      
-00012ff0: 2020 2020 2020 666f 7220 6b65 7920 696e        for key in
-00013000: 2064 6174 615f 6b65 795f 656e 7472 795b   data_key_entry[
-00013010: 3a2d 315d 3a0a 2020 2020 2020 2020 2020  :-1]:.          
-00013020: 2020 2020 2020 6461 7461 203d 2064 6174        data = dat
-00013030: 615b 6b65 795d 0a20 2020 2020 2020 2020  a[key].         
-00013040: 2020 2064 6174 615b 6461 7461 5f6b 6579     data[data_key
-00013050: 5f65 6e74 7279 5b2d 315d 5d20 3d20 2223  _entry[-1]] = "#
-00013060: 7b22 202b 2072 645f 6964 735b 695d 202b  {" + rd_ids[i] +
-00013070: 2022 7d22 0a0a 2020 2020 2020 2020 6177   "}"..        aw
-00013080: 6169 7420 7365 6c66 2e5f 6372 6561 7465  ait self._create
-00013090: 5f63 6861 7274 280a 2020 2020 2020 2020  _chart(.        
-000130a0: 2020 2020 6368 6172 745f 636c 6173 733d      chart_class=
-000130b0: 4543 6861 7274 2c0a 2020 2020 2020 2020  EChart,.        
-000130c0: 2020 2020 7072 6f70 6572 7469 6573 3d7b      properties={
-000130d0: 226f 7074 696f 6e22 3a20 6f70 7469 6f6e  "option": option
-000130e0: 737d 2c0a 2020 2020 2020 2020 2020 2020  s},.            
-000130f0: 6f72 6465 723d 6f72 6465 722c 0a20 2020  order=order,.   
-00013100: 2020 2020 2020 2020 2074 6974 6c65 3d74           title=t
-00013110: 6974 6c65 2c0a 2020 2020 2020 2020 2020  itle,.          
-00013120: 2020 7369 7a65 5061 6464 696e 673d 7061    sizePadding=pa
-00013130: 6464 696e 672c 0a20 2020 2020 2020 2020  dding,.         
-00013140: 2020 2073 697a 6552 6f77 733d 726f 7773     sizeRows=rows
-00013150: 5f73 697a 652c 0a20 2020 2020 2020 2020  _size,.         
-00013160: 2020 2073 697a 6543 6f6c 756d 6e73 3d63     sizeColumns=c
-00013170: 6f6c 735f 7369 7a65 2c0a 2020 2020 2020  ols_size,.      
-00013180: 2020 290a 0a20 2020 2040 7374 6174 6963    )..    @static
-00013190: 6d65 7468 6f64 0a20 2020 2064 6566 205f  method.    def _
-000131a0: 6170 706c 795f 7661 7269 616e 7428 6563  apply_variant(ec
-000131b0: 6861 7274 5f6f 7074 696f 6e73 3a20 6469  hart_options: di
-000131c0: 6374 2c20 7661 7269 616e 743a 204f 7074  ct, variant: Opt
-000131d0: 696f 6e61 6c5b 7374 725d 293a 0a20 2020  ional[str]):.   
-000131e0: 2020 2020 2069 6620 7661 7269 616e 7420       if variant 
-000131f0: 3d3d 2022 636c 6561 6e22 3a0a 2020 2020  == "clean":.    
-00013200: 2020 2020 2020 2020 6563 6861 7274 5f6f          echart_o
-00013210: 7074 696f 6e73 2e75 7064 6174 6528 0a20  ptions.update(. 
-00013220: 2020 2020 2020 2020 2020 2020 2020 207b                 {
-00013230: 2274 6f6f 6c62 6f78 223a 207b 2273 686f  "toolbox": {"sho
-00013240: 7722 3a20 4661 6c73 657d 2c20 226c 6567  w": False}, "leg
-00013250: 656e 6422 3a20 7b22 7368 6f77 223a 2046  end": {"show": F
-00013260: 616c 7365 7d2c 2022 6772 6964 223a 207b  alse}, "grid": {
-00013270: 7d7d 0a20 2020 2020 2020 2020 2020 2029  }}.            )
-00013280: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
-00013290: 2061 7869 736c 6973 7420 696e 205b 6563   axislist in [ec
-000132a0: 6861 7274 5f6f 7074 696f 6e73 5b22 7841  hart_options["xA
-000132b0: 7869 7322 5d2c 2065 6368 6172 745f 6f70  xis"], echart_op
-000132c0: 7469 6f6e 735b 2279 4178 6973 225d 5d3a  tions["yAxis"]]:
-000132d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000132e0: 2066 6f72 2061 7869 7320 696e 2061 7869   for axis in axi
-000132f0: 736c 6973 743a 0a20 2020 2020 2020 2020  slist:.         
-00013300: 2020 2020 2020 2020 2020 2061 7869 732e             axis.
-00013310: 7570 6461 7465 280a 2020 2020 2020 2020  update(.        
-00013320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013330: 7b22 6178 6973 4c69 6e65 223a 207b 2273  {"axisLine": {"s
-00013340: 686f 7722 3a20 4661 6c73 657d 2c20 2261  how": False}, "a
-00013350: 7869 7354 6963 6b22 3a20 7b22 7368 6f77  xisTick": {"show
-00013360: 223a 2046 616c 7365 7d7d 0a20 2020 2020  ": False}}.     
-00013370: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-00013380: 0a20 2020 2020 2020 2065 6c69 6620 7661  .        elif va
-00013390: 7269 616e 7420 3d3d 2022 6d69 6e69 6d61  riant == "minima
-000133a0: 6c22 3a0a 2020 2020 2020 2020 2020 2020  l":.            
-000133b0: 6563 6861 7274 5f6f 7074 696f 6e73 2e75  echart_options.u
-000133c0: 7064 6174 6528 0a20 2020 2020 2020 2020  pdate(.         
-000133d0: 2020 2020 2020 207b 0a20 2020 2020 2020         {.       
-000133e0: 2020 2020 2020 2020 2020 2020 2022 746f               "to
-000133f0: 6f6c 626f 7822 3a20 7b22 7368 6f77 223a  olbox": {"show":
-00013400: 2046 616c 7365 7d2c 0a20 2020 2020 2020   False},.       
-00013410: 2020 2020 2020 2020 2020 2020 2022 6c65               "le
-00013420: 6765 6e64 223a 207b 2273 686f 7722 3a20  gend": {"show": 
-00013430: 4661 6c73 657d 2c0a 2020 2020 2020 2020  False},.        
-00013440: 2020 2020 2020 2020 2020 2020 2267 7269              "gri
-00013450: 6422 3a20 7b22 6c65 6674 223a 2022 3125  d": {"left": "1%
-00013460: 222c 2022 7269 6768 7422 3a20 2231 2522  ", "right": "1%"
-00013470: 2c20 2274 6f70 223a 2022 3125 222c 2022  , "top": "1%", "
-00013480: 626f 7474 6f6d 223a 2022 3125 227d 2c0a  bottom": "1%"},.
-00013490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000134a0: 2020 2020 2274 6f6f 6c74 6970 223a 207b      "tooltip": {
-000134b0: 2273 686f 7722 3a20 4661 6c73 657d 2c0a  "show": False},.
-000134c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000134d0: 7d0a 2020 2020 2020 2020 2020 2020 290a  }.            ).
-000134e0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-000134f0: 6178 6973 6c69 7374 2069 6e20 5b65 6368  axislist in [ech
-00013500: 6172 745f 6f70 7469 6f6e 735b 2278 4178  art_options["xAx
-00013510: 6973 225d 2c20 6563 6861 7274 5f6f 7074  is"], echart_opt
-00013520: 696f 6e73 5b22 7941 7869 7322 5d5d 3a0a  ions["yAxis"]]:.
-00013530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013540: 666f 7220 6178 6973 2069 6e20 6178 6973  for axis in axis
-00013550: 6c69 7374 3a0a 2020 2020 2020 2020 2020  list:.          
-00013560: 2020 2020 2020 2020 2020 6178 6973 2e75            axis.u
-00013570: 7064 6174 6528 0a20 2020 2020 2020 2020  pdate(.         
-00013580: 2020 2020 2020 2020 2020 2020 2020 207b                 {
-00013590: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000135a0: 2020 2020 2020 2020 2020 2020 2022 6178               "ax
-000135b0: 6973 4c69 6e65 223a 207b 2273 686f 7722  isLine": {"show"
-000135c0: 3a20 4661 6c73 657d 2c0a 2020 2020 2020  : False},.      
-000135d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000135e0: 2020 2020 2020 2261 7869 7354 6963 6b22        "axisTick"
-000135f0: 3a20 7b22 7368 6f77 223a 2046 616c 7365  : {"show": False
-00013600: 7d2c 0a20 2020 2020 2020 2020 2020 2020  },.             
-00013610: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00013620: 7370 6c69 744c 696e 6522 3a20 7b22 7368  splitLine": {"sh
-00013630: 6f77 223a 2046 616c 7365 7d2c 0a20 2020  ow": False},.   
-00013640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013650: 2020 2020 2020 2020 2022 6178 6973 4c61           "axisLa
-00013660: 6265 6c22 3a20 7b22 7368 6f77 223a 2046  bel": {"show": F
-00013670: 616c 7365 7d2c 0a20 2020 2020 2020 2020  alse},.         
-00013680: 2020 2020 2020 2020 2020 2020 2020 207d                 }
-00013690: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000136a0: 2020 2020 2029 0a0a 2020 2020 6173 796e       )..    asyn
-000136b0: 6320 6465 6620 5f63 7265 6174 655f 7472  c def _create_tr
-000136c0: 656e 645f 6368 6172 7428 0a20 2020 2020  end_chart(.     
-000136d0: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
-000136e0: 2061 7865 733a 2055 6e69 6f6e 5b6c 6973   axes: Union[lis
-000136f0: 745b 7374 725d 2c20 7374 725d 2c0a 2020  t[str], str],.  
-00013700: 2020 2020 2020 6f72 6465 723a 2069 6e74        order: int
-00013710: 2c0a 2020 2020 2020 2020 6461 7461 5f6d  ,.        data_m
-00013720: 6170 7069 6e67 5f74 6f5f 7475 706c 6573  apping_to_tuples
-00013730: 3a20 4f70 7469 6f6e 616c 5b64 6963 745d  : Optional[dict]
-00013740: 2c0a 2020 2020 2020 2020 6563 6861 7274  ,.        echart
-00013750: 5f6f 7074 696f 6e73 3a20 6469 6374 2c0a  _options: dict,.
-00013760: 2020 2020 2020 2020 7365 7269 6573 5f6f          series_o
-00013770: 7074 696f 6e73 3a20 556e 696f 6e5b 6469  ptions: Union[di
-00013780: 6374 2c20 6c69 7374 5b64 6963 745d 5d2c  ct, list[dict]],
-00013790: 0a20 2020 2020 2020 2076 616c 7565 733a  .        values:
-000137a0: 204f 7074 696f 6e61 6c5b 556e 696f 6e5b   Optional[Union[
-000137b0: 6c69 7374 5b55 6e69 6f6e 5b73 7472 2c20  list[Union[str, 
-000137c0: 7475 706c 655d 5d2c 2073 7472 2c20 7475  tuple]], str, tu
-000137d0: 706c 655d 5d20 3d20 4e6f 6e65 2c0a 2020  ple]] = None,.  
-000137e0: 2020 2020 2020 785f 6178 6973 5f6e 616d        x_axis_nam
-000137f0: 6573 3a20 4f70 7469 6f6e 616c 5b55 6e69  es: Optional[Uni
-00013800: 6f6e 5b73 7472 2c20 6c69 7374 5b73 7472  on[str, list[str
-00013810: 5d5d 5d20 3d20 4e6f 6e65 2c0a 2020 2020  ]]] = None,.    
-00013820: 2020 2020 795f 6178 6973 5f6e 616d 6573      y_axis_names
-00013830: 3a20 4f70 7469 6f6e 616c 5b55 6e69 6f6e  : Optional[Union
-00013840: 5b73 7472 2c20 6c69 7374 5b73 7472 5d5d  [str, list[str]]
-00013850: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
-00013860: 2020 7368 6f77 5f76 616c 7565 733a 204f    show_values: O
-00013870: 7074 696f 6e61 6c5b 556e 696f 6e5b 6c69  ptional[Union[li
-00013880: 7374 5b73 7472 5d2c 2073 7472 5d5d 203d  st[str], str]] =
-00013890: 204e 6f6e 652c 0a20 2020 2020 2020 2076   None,.        v
-000138a0: 6172 6961 6e74 3a20 4f70 7469 6f6e 616c  ariant: Optional
-000138b0: 5b73 7472 5d20 3d20 4e6f 6e65 2c0a 2020  [str] = None,.  
-000138c0: 2020 2020 2020 2a2a 7265 706f 7274 5f70        **report_p
-000138d0: 6172 616d 732c 0a20 2020 2029 3a0a 2020  arams,.    ):.  
-000138e0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-000138f0: 2020 4372 6561 7465 2061 206c 696e 6520    Create a line 
-00013900: 6368 6172 7420 696e 2074 6865 2064 6173  chart in the das
-00013910: 6862 6f61 7264 2e0a 2020 2020 2020 2020  hboard..        
-00013920: 3a70 6172 616d 2064 6174 613a 2074 6865  :param data: the
-00013930: 2064 6174 6120 6f66 2074 6865 2063 6861   data of the cha
-00013940: 7274 0a20 2020 2020 2020 203a 7061 7261  rt.        :para
-00013950: 6d20 6178 6573 3a20 7468 6520 6e61 6d65  m axes: the name
-00013960: 7320 6f66 2074 6865 2063 6f6c 756d 6e73  s of the columns
-00013970: 2074 6f20 6265 2075 7365 6420 6173 2061   to be used as a
-00013980: 7869 730a 2020 2020 2020 2020 3a70 6172  xis.        :par
-00013990: 616d 2076 616c 7565 733a 2074 6865 206e  am values: the n
-000139a0: 616d 6573 206f 6620 7468 6520 636f 6c75  ames of the colu
-000139b0: 6d6e 7320 746f 2062 6520 7573 6564 2061  mns to be used a
-000139c0: 7320 7661 6c75 6573 0a20 2020 2020 2020  s values.       
-000139d0: 203a 7061 7261 6d20 785f 6178 6973 5f6e   :param x_axis_n
-000139e0: 616d 6573 3a20 7468 6520 6e61 6d65 206f  ames: the name o
-000139f0: 6620 7468 6520 7820 6178 6573 0a20 2020  f the x axes.   
-00013a00: 2020 2020 203a 7061 7261 6d20 795f 6178       :param y_ax
-00013a10: 6973 5f6e 616d 6573 3a20 7468 6520 6e61  is_names: the na
-00013a20: 6d65 206f 6620 7468 6520 7920 6178 6573  me of the y axes
-00013a30: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-00013a40: 6563 6861 7274 5f6f 7074 696f 6e73 3a20  echart_options: 
-00013a50: 7468 6520 6f70 7469 6f6e 7320 6f66 2074  the options of t
-00013a60: 6865 2063 6861 7274 0a20 2020 2020 2020  he chart.       
-00013a70: 203a 7061 7261 6d20 7365 7269 6573 5f6f   :param series_o
-00013a80: 7074 696f 6e73 3a20 7468 6520 6f70 7469  ptions: the opti
-00013a90: 6f6e 7320 6f66 2074 6865 2073 6572 6965  ons of the serie
-00013aa0: 7320 6f66 2074 6865 2063 6861 7274 0a20  s of the chart. 
-00013ab0: 2020 2020 2020 203a 7061 7261 6d20 626f         :param bo
-00013ac0: 7474 6f6d 5f74 6f6f 6c62 6f78 3a20 7768  ttom_toolbox: wh
-00013ad0: 6574 6865 7220 746f 2073 686f 7720 7468  ether to show th
-00013ae0: 6520 746f 6f6c 626f 7820 6f6e 2074 6f70  e toolbox on top
-00013af0: 206f 6620 7468 6520 6368 6172 740a 2020   of the chart.  
-00013b00: 2020 2020 2020 3a70 6172 616d 206f 7264        :param ord
-00013b10: 6572 3a20 7468 6520 6f72 6465 7220 6f66  er: the order of
-00013b20: 2074 6865 2063 6861 7274 2069 6e20 7468   the chart in th
-00013b30: 6520 6461 7368 626f 6172 640a 2020 2020  e dashboard.    
-00013b40: 2020 2020 3a70 6172 616d 2072 6570 6f72      :param repor
-00013b50: 745f 7061 7261 6d73 3a20 6164 6469 7469  t_params: additi
-00013b60: 6f6e 616c 2072 6570 6f72 7420 7061 7261  onal report para
-00013b70: 6d65 7465 7273 2061 7320 6b65 792d 7661  meters as key-va
-00013b80: 6c75 6520 7061 6972 730a 2020 2020 2020  lue pairs.      
-00013b90: 2020 2222 220a 2020 2020 2020 2020 7365    """.        se
-00013ba0: 6c66 2e5f 6170 706c 795f 7661 7269 616e  lf._apply_varian
-00013bb0: 7428 6563 6861 7274 5f6f 7074 696f 6e73  t(echart_options
-00013bc0: 2c20 7661 7269 616e 7429 0a20 2020 2020  , variant).     
-00013bd0: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
-00013be0: 2861 7865 732c 2073 7472 293a 0a20 2020  (axes, str):.   
-00013bf0: 2020 2020 2020 2020 2061 7865 7320 3d20           axes = 
-00013c00: 5b61 7865 735d 0a20 2020 2020 2020 2069  [axes].        i
-00013c10: 6620 6973 696e 7374 616e 6365 2876 616c  f isinstance(val
-00013c20: 7565 732c 2073 7472 2920 6f72 2069 7369  ues, str) or isi
-00013c30: 6e73 7461 6e63 6528 7661 6c75 6573 2c20  nstance(values, 
-00013c40: 7475 706c 6529 3a0a 2020 2020 2020 2020  tuple):.        
-00013c50: 2020 2020 7661 6c75 6573 203d 205b 7661      values = [va
-00013c60: 6c75 6573 5d0a 2020 2020 2020 2020 6966  lues].        if
-00013c70: 2073 686f 775f 7661 6c75 6573 2069 7320   show_values is 
-00013c80: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00013c90: 2020 7368 6f77 5f76 616c 7565 7320 3d20    show_values = 
-00013ca0: 5b5d 0a0a 2020 2020 2020 2020 6966 2022  []..        if "
-00013cb0: 785f 6178 6973 5f6e 616d 6522 2069 6e20  x_axis_name" in 
-00013cc0: 7265 706f 7274 5f70 6172 616d 733a 0a20  report_params:. 
-00013cd0: 2020 2020 2020 2020 2020 2078 5f61 7869             x_axi
-00013ce0: 735f 6e61 6d65 7320 3d20 5b72 6570 6f72  s_names = [repor
-00013cf0: 745f 7061 7261 6d73 5b22 785f 6178 6973  t_params["x_axis
-00013d00: 5f6e 616d 6522 5d5d 0a20 2020 2020 2020  _name"]].       
-00013d10: 2065 6c69 6620 6973 696e 7374 616e 6365   elif isinstance
-00013d20: 2878 5f61 7869 735f 6e61 6d65 732c 2073  (x_axis_names, s
-00013d30: 7472 293a 0a20 2020 2020 2020 2020 2020  tr):.           
-00013d40: 2078 5f61 7869 735f 6e61 6d65 7320 3d20   x_axis_names = 
-00013d50: 5b78 5f61 7869 735f 6e61 6d65 735d 0a20  [x_axis_names]. 
-00013d60: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-00013d70: 2020 2020 2020 2020 2078 5f61 7869 735f           x_axis_
-00013d80: 6e61 6d65 7320 3d20 5b5d 0a0a 2020 2020  names = []..    
-00013d90: 2020 2020 6966 2022 795f 6178 6973 5f6e      if "y_axis_n
-00013da0: 616d 6522 2069 6e20 7265 706f 7274 5f70  ame" in report_p
-00013db0: 6172 616d 733a 0a20 2020 2020 2020 2020  arams:.         
-00013dc0: 2020 2079 5f61 7869 735f 6e61 6d65 7320     y_axis_names 
-00013dd0: 3d20 5b72 6570 6f72 745f 7061 7261 6d73  = [report_params
-00013de0: 5b22 795f 6178 6973 5f6e 616d 6522 5d5d  ["y_axis_name"]]
-00013df0: 0a20 2020 2020 2020 2065 6c69 6620 6973  .        elif is
-00013e00: 696e 7374 616e 6365 2879 5f61 7869 735f  instance(y_axis_
-00013e10: 6e61 6d65 732c 2073 7472 293a 0a20 2020  names, str):.   
-00013e20: 2020 2020 2020 2020 2079 5f61 7869 735f           y_axis_
-00013e30: 6e61 6d65 7320 3d20 5b79 5f61 7869 735f  names = [y_axis_
-00013e40: 6e61 6d65 735d 0a20 2020 2020 2020 2065  names].        e
-00013e50: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-00013e60: 2079 5f61 7869 735f 6e61 6d65 7320 3d20   y_axis_names = 
-00013e70: 5b5d 0a0a 2020 2020 2020 2020 7661 6c75  []..        valu
-00013e80: 6573 203d 2028 0a20 2020 2020 2020 2020  es = (.         
-00013e90: 2020 205b 7620 666f 7220 7620 696e 2064     [v for v in d
-00013ea0: 6174 615f 6d61 7070 696e 675f 746f 5f74  ata_mapping_to_t
-00013eb0: 7570 6c65 732e 6b65 7973 2829 2069 6620  uples.keys() if 
-00013ec0: 7620 6e6f 7420 696e 2061 7865 735d 0a20  v not in axes]. 
-00013ed0: 2020 2020 2020 2020 2020 2069 6620 7661             if va
-00013ee0: 6c75 6573 2069 7320 4e6f 6e65 0a20 2020  lues is None.   
-00013ef0: 2020 2020 2020 2020 2065 6c73 6520 7661           else va
-00013f00: 6c75 6573 0a20 2020 2020 2020 2029 0a20  lues.        ). 
-00013f10: 2020 2020 2020 2069 6620 6973 696e 7374         if isinst
-00013f20: 616e 6365 2873 6572 6965 735f 6f70 7469  ance(series_opti
-00013f30: 6f6e 732c 2064 6963 7429 3a0a 2020 2020  ons, dict):.    
-00013f40: 2020 2020 2020 2020 7365 7269 6573 5f6f          series_o
-00013f50: 7074 696f 6e73 203d 205b 7365 7269 6573  ptions = [series
-00013f60: 5f6f 7074 696f 6e73 5d20 2a20 6c65 6e28  _options] * len(
-00013f70: 7661 6c75 6573 290a 2020 2020 2020 2020  values).        
-00013f80: 656c 6966 206c 656e 2873 6572 6965 735f  elif len(series_
-00013f90: 6f70 7469 6f6e 7329 203c 206c 656e 2876  options) < len(v
-00013fa0: 616c 7565 7329 3a0a 2020 2020 2020 2020  alues):.        
-00013fb0: 2020 2020 7365 7269 6573 5f6f 7074 696f      series_optio
-00013fc0: 6e73 203d 2073 6572 6965 735f 6f70 7469  ns = series_opti
-00013fd0: 6f6e 7320 2b20 5b73 6572 6965 735f 6f70  ons + [series_op
-00013fe0: 7469 6f6e 735b 2d31 5d5d 202a 2028 0a20  tions[-1]] * (. 
-00013ff0: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-00014000: 656e 2876 616c 7565 7329 202d 206c 656e  en(values) - len
-00014010: 2873 6572 6965 735f 6f70 7469 6f6e 7329  (series_options)
-00014020: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
-00014030: 2020 2020 2020 2065 6c69 6620 6c65 6e28         elif len(
-00014040: 7365 7269 6573 5f6f 7074 696f 6e73 2920  series_options) 
-00014050: 3e20 6c65 6e28 7661 6c75 6573 293a 0a20  > len(values):. 
-00014060: 2020 2020 2020 2020 2020 2073 6572 6965             serie
-00014070: 735f 6f70 7469 6f6e 7320 3d20 7365 7269  s_options = seri
-00014080: 6573 5f6f 7074 696f 6e73 5b3a 206c 656e  es_options[: len
-00014090: 2876 616c 7565 7329 5d0a 0a20 2020 2020  (values)]..     
-000140a0: 2020 2065 6368 6172 745f 6f70 7469 6f6e     echart_option
-000140b0: 735b 2273 6572 6965 7322 5d20 3d20 5b0a  s["series"] = [.
-000140c0: 2020 2020 2020 2020 2020 2020 6465 6570              deep
-000140d0: 5f75 7064 6174 6528 0a20 2020 2020 2020  _update(.       
-000140e0: 2020 2020 2020 2020 207b 0a20 2020 2020           {.     
-000140f0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00014100: 6e61 6d65 223a 206e 616d 6520 6966 2069  name": name if i
-00014110: 7369 6e73 7461 6e63 6528 6e61 6d65 2c20  sinstance(name, 
-00014120: 7374 7229 2065 6c73 6520 2220 c397 2022  str) else " .. "
-00014130: 2e6a 6f69 6e28 6e61 6d65 292c 0a20 2020  .join(name),.   
-00014140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014150: 2022 6c61 6265 6c22 3a20 7b22 7368 6f77   "label": {"show
-00014160: 223a 2073 686f 775f 7661 6c75 6573 203d  ": show_values =
-00014170: 3d20 2261 6c6c 2220 6f72 206e 616d 6520  = "all" or name 
-00014180: 696e 2073 686f 775f 7661 6c75 6573 7d2c  in show_values},
-00014190: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000141a0: 207d 2c0a 2020 2020 2020 2020 2020 2020   },.            
-000141b0: 2020 2020 7365 7269 6573 5f6f 7074 696f      series_optio
-000141c0: 6e73 5b69 5d2c 0a20 2020 2020 2020 2020  ns[i],.         
-000141d0: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
-000141e0: 2066 6f72 2069 2c20 6e61 6d65 2069 6e20   for i, name in 
-000141f0: 656e 756d 6572 6174 6528 7661 6c75 6573  enumerate(values
-00014200: 290a 2020 2020 2020 2020 5d0a 0a20 2020  ).        ]..   
-00014210: 2020 2020 2066 6f72 2069 2c20 6178 6973       for i, axis
-00014220: 5f6f 7074 696f 6e73 2069 6e20 656e 756d  _options in enum
-00014230: 6572 6174 6528 6563 6861 7274 5f6f 7074  erate(echart_opt
-00014240: 696f 6e73 5b22 7841 7869 7322 5d29 3a0a  ions["xAxis"]):.
-00014250: 2020 2020 2020 2020 2020 2020 6178 6973              axis
-00014260: 5f6f 7074 696f 6e73 5b22 6e61 6d65 225d  _options["name"]
-00014270: 203d 2078 5f61 7869 735f 6e61 6d65 735b   = x_axis_names[
-00014280: 695d 2069 6620 6920 3c20 6c65 6e28 785f  i] if i < len(x_
-00014290: 6178 6973 5f6e 616d 6573 2920 656c 7365  axis_names) else
-000142a0: 204e 6f6e 650a 2020 2020 2020 2020 2020   None.          
-000142b0: 2020 6966 2061 7869 735f 6f70 7469 6f6e    if axis_option
-000142c0: 735b 226e 616d 6522 5d20 616e 6420 226e  s["name"] and "n
-000142d0: 616d 6547 6170 2220 6e6f 7420 696e 2061  ameGap" not in a
-000142e0: 7869 735f 6f70 7469 6f6e 733a 0a20 2020  xis_options:.   
-000142f0: 2020 2020 2020 2020 2020 2020 2061 7869               axi
-00014300: 735f 6f70 7469 6f6e 735b 226e 616d 6547  s_options["nameG
-00014310: 6170 225d 203d 2033 320a 0a20 2020 2020  ap"] = 32..     
-00014320: 2020 2066 6f72 2069 2c20 6178 6973 5f6f     for i, axis_o
-00014330: 7074 696f 6e73 2069 6e20 656e 756d 6572  ptions in enumer
-00014340: 6174 6528 6563 6861 7274 5f6f 7074 696f  ate(echart_optio
-00014350: 6e73 5b22 7941 7869 7322 5d29 3a0a 2020  ns["yAxis"]):.  
-00014360: 2020 2020 2020 2020 2020 6178 6973 5f6f            axis_o
-00014370: 7074 696f 6e73 5b22 6e61 6d65 225d 203d  ptions["name"] =
-00014380: 2079 5f61 7869 735f 6e61 6d65 735b 695d   y_axis_names[i]
-00014390: 2069 6620 6920 3c20 6c65 6e28 795f 6178   if i < len(y_ax
-000143a0: 6973 5f6e 616d 6573 2920 656c 7365 204e  is_names) else N
-000143b0: 6f6e 650a 2020 2020 2020 2020 2020 2020  one.            
-000143c0: 6966 2061 7869 735f 6f70 7469 6f6e 735b  if axis_options[
-000143d0: 226e 616d 6522 5d20 616e 6420 226e 616d  "name"] and "nam
-000143e0: 6547 6170 2220 6e6f 7420 696e 2061 7869  eGap" not in axi
-000143f0: 735f 6f70 7469 6f6e 733a 0a20 2020 2020  s_options:.     
-00014400: 2020 2020 2020 2020 2020 2061 7869 735f             axis_
-00014410: 6f70 7469 6f6e 735b 226e 616d 6547 6170  options["nameGap
-00014420: 225d 203d 202d 3234 0a20 2020 2020 2020  "] = -24.       
-00014430: 2020 2020 2020 2020 2061 7869 735f 6f70           axis_op
-00014440: 7469 6f6e 735b 226f 6666 7365 7422 5d20  tions["offset"] 
-00014450: 3d20 3336 0a20 2020 2020 2020 2020 2020  = 36.           
-00014460: 2020 2020 2065 6368 6172 745f 6f70 7469       echart_opti
-00014470: 6f6e 735b 2267 7269 6422 5d5b 226c 6566  ons["grid"]["lef
-00014480: 7422 5d20 3d20 2234 2522 0a20 2020 2020  t"] = "4%".     
-00014490: 2020 2020 2020 2020 2020 2061 7869 735f             axis_
-000144a0: 6f70 7469 6f6e 735b 2261 7869 7354 6963  options["axisTic
-000144b0: 6b22 5d20 3d20 7b22 7368 6f77 223a 2046  k"] = {"show": F
-000144c0: 616c 7365 7d0a 2020 2020 2020 2020 2020  alse}.          
-000144d0: 2020 2020 2020 6178 6973 5f6f 7074 696f        axis_optio
-000144e0: 6e73 5b22 6178 6973 4c69 6e65 225d 203d  ns["axisLine"] =
-000144f0: 207b 2273 686f 7722 3a20 4661 6c73 657d   {"show": False}
-00014500: 0a0a 2020 2020 2020 2020 6177 6169 7420  ..        await 
-00014510: 7365 6c66 2e5f 6372 6561 7465 5f65 6368  self._create_ech
-00014520: 6172 7428 0a20 2020 2020 2020 2020 2020  art(.           
-00014530: 206f 7264 6572 3d6f 7264 6572 2c0a 2020   order=order,.  
-00014540: 2020 2020 2020 2020 2020 6f70 7469 6f6e            option
-00014550: 733d 6563 6861 7274 5f6f 7074 696f 6e73  s=echart_options
-00014560: 2c0a 2020 2020 2020 2020 2020 2020 6461  ,.            da
-00014570: 7461 5f6d 6170 7069 6e67 5f74 6f5f 7475  ta_mapping_to_tu
-00014580: 706c 6573 3d64 6174 615f 6d61 7070 696e  ples=data_mappin
-00014590: 675f 746f 5f74 7570 6c65 732c 0a20 2020  g_to_tuples,.   
-000145a0: 2020 2020 2020 2020 2066 6965 6c64 733d           fields=
-000145b0: 6178 6573 202b 2076 616c 7565 732c 0a20  axes + values,. 
-000145c0: 2020 2020 2020 2020 2020 202a 2a72 6570             **rep
-000145d0: 6f72 745f 7061 7261 6d73 2c0a 2020 2020  ort_params,.    
-000145e0: 2020 2020 290a 0a20 2020 2040 6164 645f      )..    @add_
-000145f0: 746f 5f67 656e 6572 616c 5f61 7379 6e63  to_general_async
-00014600: 5f67 726f 7570 0a20 2020 2061 7379 6e63  _group.    async
-00014610: 2064 6566 2066 7265 655f 6563 6861 7274   def free_echart
-00014620: 7328 0a20 2020 2020 2020 2073 656c 662c  s(.        self,
-00014630: 0a20 2020 2020 2020 2064 6174 613a 204f  .        data: O
-00014640: 7074 696f 6e61 6c5b 556e 696f 6e5b 7374  ptional[Union[st
-00014650: 722c 2044 6174 6146 7261 6d65 2c20 6c69  r, DataFrame, li
-00014660: 7374 5b64 6963 745d 5d5d 203d 204e 6f6e  st[dict]]] = Non
-00014670: 652c 0a20 2020 2020 2020 206f 7074 696f  e,.        optio
-00014680: 6e73 3a20 4f70 7469 6f6e 616c 5b64 6963  ns: Optional[dic
-00014690: 745d 203d 204e 6f6e 652c 0a20 2020 2020  t] = None,.     
-000146a0: 2020 2072 6177 5f6f 7074 696f 6e73 3a20     raw_options: 
-000146b0: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
-000146c0: 4e6f 6e65 2c0a 2020 2020 2020 2020 6f72  None,.        or
-000146d0: 6465 723a 204f 7074 696f 6e61 6c5b 696e  der: Optional[in
-000146e0: 745d 203d 204e 6f6e 652c 0a20 2020 2020  t] = None,.     
-000146f0: 2020 2074 6974 6c65 3a20 4f70 7469 6f6e     title: Option
-00014700: 616c 5b73 7472 5d20 3d20 4e6f 6e65 2c0a  al[str] = None,.
-00014710: 2020 2020 2020 2020 726f 7773 5f73 697a          rows_siz
-00014720: 653a 204f 7074 696f 6e61 6c5b 696e 745d  e: Optional[int]
-00014730: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-00014740: 2063 6f6c 735f 7369 7a65 3a20 4f70 7469   cols_size: Opti
-00014750: 6f6e 616c 5b69 6e74 5d20 3d20 4e6f 6e65  onal[int] = None
-00014760: 2c0a 2020 2020 2020 2020 7061 6464 696e  ,.        paddin
-00014770: 673a 204f 7074 696f 6e61 6c5b 7374 725d  g: Optional[str]
-00014780: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-00014790: 2066 6965 6c64 733a 204f 7074 696f 6e61   fields: Optiona
-000147a0: 6c5b 6c69 7374 5d20 3d20 4e6f 6e65 2c0a  l[list] = None,.
-000147b0: 2020 2020 2020 2020 6461 7461 5f69 735f          data_is_
-000147c0: 6e6f 745f 6466 3a20 626f 6f6c 203d 2046  not_df: bool = F
-000147d0: 616c 7365 2c0a 2020 2020 293a 0a20 2020  alse,.    ):.   
-000147e0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-000147f0: 2043 7265 6174 6520 616e 2065 6368 6172   Create an echar
-00014800: 7473 2063 6861 7274 2077 6974 6820 6375  ts chart with cu
-00014810: 7374 6f6d 206f 7074 696f 6e73 2e0a 2020  stom options..  
-00014820: 2020 2020 2020 3a70 6172 616d 2064 6174        :param dat
-00014830: 613a 2074 6865 2064 6174 6120 6f66 2074  a: the data of t
-00014840: 6865 2063 6861 7274 0a20 2020 2020 2020  he chart.       
-00014850: 203a 7061 7261 6d20 6f70 7469 6f6e 733a   :param options:
-00014860: 2074 6865 206f 7074 696f 6e73 206f 6620   the options of 
-00014870: 7468 6520 6368 6172 740a 2020 2020 2020  the chart.      
-00014880: 2020 3a70 6172 616d 2072 6177 5f6f 7074    :param raw_opt
-00014890: 696f 6e73 3a20 7468 6520 7261 7720 6f70  ions: the raw op
-000148a0: 7469 6f6e 7320 6f66 2074 6865 2063 6861  tions of the cha
-000148b0: 7274 0a20 2020 2020 2020 203a 7061 7261  rt.        :para
-000148c0: 6d20 6f72 6465 723a 2074 6865 206f 7264  m order: the ord
-000148d0: 6572 206f 6620 7468 6520 6368 6172 7420  er of the chart 
-000148e0: 696e 2074 6865 2064 6173 6862 6f61 7264  in the dashboard
-000148f0: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-00014900: 7469 746c 653a 2074 6865 2074 6974 6c65  title: the title
-00014910: 206f 6620 7468 6520 6368 6172 740a 2020   of the chart.  
-00014920: 2020 2020 2020 3a70 6172 616d 2072 6f77        :param row
-00014930: 735f 7369 7a65 3a20 7468 6520 726f 7773  s_size: the rows
-00014940: 2073 697a 6520 6f66 2074 6865 2063 6861   size of the cha
-00014950: 7274 0a20 2020 2020 2020 203a 7061 7261  rt.        :para
-00014960: 6d20 636f 6c73 5f73 697a 653a 2074 6865  m cols_size: the
-00014970: 2063 6f6c 756d 6e73 2073 697a 6520 6f66   columns size of
-00014980: 2074 6865 2063 6861 7274 0a20 2020 2020   the chart.     
-00014990: 2020 203a 7061 7261 6d20 7061 6464 696e     :param paddin
-000149a0: 673a 2074 6865 2070 6164 6469 6e67 206f  g: the padding o
-000149b0: 6620 7468 6520 6368 6172 740a 2020 2020  f the chart.    
-000149c0: 2020 2020 3a70 6172 616d 2066 6965 6c64      :param field
-000149d0: 733a 2074 6865 2066 6965 6c64 7320 6f66  s: the fields of
-000149e0: 2074 6865 2063 6861 7274 0a20 2020 2020   the chart.     
-000149f0: 2020 203a 7061 7261 6d20 6461 7461 5f69     :param data_i
-00014a00: 735f 6e6f 745f 6466 3a20 7768 6574 6865  s_not_df: whethe
-00014a10: 7220 7468 6520 6461 7461 2069 7320 6e6f  r the data is no
-00014a20: 7420 6120 6461 7461 6672 616d 650a 2020  t a dataframe.  
-00014a30: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00014a40: 2020 6966 206e 6f74 206f 7074 696f 6e73    if not options
-00014a50: 2061 6e64 206e 6f74 2072 6177 5f6f 7074   and not raw_opt
-00014a60: 696f 6e73 3a0a 2020 2020 2020 2020 2020  ions:.          
-00014a70: 2020 6c6f 675f 6572 726f 7228 0a20 2020    log_error(.   
-00014a80: 2020 2020 2020 2020 2020 2020 206c 6f67               log
-00014a90: 6765 722c 2022 4569 7468 6572 206f 7074  ger, "Either opt
-00014aa0: 696f 6e73 206f 7220 7261 775f 6f70 7469  ions or raw_opti
-00014ab0: 6f6e 7320 6d75 7374 2062 6520 7072 6f76  ons must be prov
-00014ac0: 6964 6564 222c 2056 616c 7565 4572 726f  ided", ValueErro
-00014ad0: 720a 2020 2020 2020 2020 2020 2020 290a  r.            ).
-00014ae0: 2020 2020 2020 2020 6966 206f 7074 696f          if optio
-00014af0: 6e73 2061 6e64 206e 6f74 2069 7369 6e73  ns and not isins
-00014b00: 7461 6e63 6528 6461 7461 2c20 4461 7461  tance(data, Data
-00014b10: 4672 616d 6529 2061 6e64 2064 6174 6120  Frame) and data 
-00014b20: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
-00014b30: 2020 2020 206c 6f67 5f65 7272 6f72 280a       log_error(.
-00014b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014b50: 6c6f 6767 6572 2c20 2264 6174 6120 6d75  logger, "data mu
-00014b60: 7374 2062 6520 7072 6f76 6964 6564 2077  st be provided w
-00014b70: 6865 6e20 6f70 7469 6f6e 7320 6973 2070  hen options is p
-00014b80: 726f 7669 6465 6422 2c20 4461 7461 4572  rovided", DataEr
-00014b90: 726f 720a 2020 2020 2020 2020 2020 2020  ror.            
-00014ba0: 290a 2020 2020 2020 2020 6966 206f 7074  ).        if opt
-00014bb0: 696f 6e73 2061 6e64 2072 6177 5f6f 7074  ions and raw_opt
-00014bc0: 696f 6e73 3a0a 2020 2020 2020 2020 2020  ions:.          
-00014bd0: 2020 6c6f 675f 6572 726f 7228 0a20 2020    log_error(.   
-00014be0: 2020 2020 2020 2020 2020 2020 206c 6f67               log
-00014bf0: 6765 722c 0a20 2020 2020 2020 2020 2020  ger,.           
-00014c00: 2020 2020 2022 4f6e 6c79 206f 6e65 206f       "Only one o
-00014c10: 6620 6f70 7469 6f6e 7320 616e 6420 7261  f options and ra
-00014c20: 775f 6f70 7469 6f6e 7320 6361 6e20 6265  w_options can be
-00014c30: 2070 726f 7669 6465 6422 2c0a 2020 2020   provided",.    
-00014c40: 2020 2020 2020 2020 2020 2020 5661 6c75              Valu
-00014c50: 6545 7272 6f72 2c0a 2020 2020 2020 2020  eError,.        
-00014c60: 2020 2020 290a 0a20 2020 2020 2020 2069      )..        i
-00014c70: 6620 7261 775f 6f70 7469 6f6e 733a 0a20  f raw_options:. 
-00014c80: 2020 2020 2020 2020 2020 206f 7074 696f             optio
-00014c90: 6e73 203d 2074 7261 6e73 666f 726d 5f64  ns = transform_d
-00014ca0: 6963 745f 6a73 5f74 6f5f 7079 2872 6177  ict_js_to_py(raw
-00014cb0: 5f6f 7074 696f 6e73 290a 2020 2020 2020  _options).      
-00014cc0: 2020 2020 2020 6461 7461 203d 2072 6574        data = ret
-00014cd0: 7269 6576 655f 6461 7461 5f66 726f 6d5f  rieve_data_from_
-00014ce0: 6f70 7469 6f6e 7328 6f70 7469 6f6e 7329  options(options)
-00014cf0: 0a20 2020 2020 2020 2020 2020 206f 7074  .            opt
-00014d00: 696f 6e73 5b22 6461 7461 7365 7422 5d20  ions["dataset"] 
-00014d10: 3d20 7b22 736f 7572 6365 223a 2022 2373  = {"source": "#s
-00014d20: 6574 5f64 6174 6123 227d 0a20 2020 2020  et_data#"}.     
-00014d30: 2020 2020 2020 2066 6965 6c64 7320 3d20         fields = 
-00014d40: 5b6c 6973 7428 6461 7461 5b30 5d2e 6b65  [list(data[0].ke
-00014d50: 7973 2829 295d 0a20 2020 2020 2020 2065  ys())].        e
-00014d60: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-00014d70: 206f 7074 696f 6e73 203d 2064 6565 7063   options = deepc
-00014d80: 6f70 7928 6f70 7469 6f6e 7329 0a0a 2020  opy(options)..  
-00014d90: 2020 2020 2020 6177 6169 7420 7365 6c66        await self
-00014da0: 2e5f 6372 6561 7465 5f65 6368 6172 7428  ._create_echart(
-00014db0: 0a20 2020 2020 2020 2020 2020 206f 7264  .            ord
-00014dc0: 6572 3d6f 7264 6572 2c0a 2020 2020 2020  er=order,.      
-00014dd0: 2020 2020 2020 6461 7461 5f6d 6170 7069        data_mappi
-00014de0: 6e67 5f74 6f5f 7475 706c 6573 3d61 7761  ng_to_tuples=awa
-00014df0: 6974 2073 656c 662e 5f63 686f 6f73 655f  it self._choose_
-00014e00: 6461 7461 280a 2020 2020 2020 2020 2020  data(.          
-00014e10: 2020 2020 2020 6f72 6465 722c 2064 6174        order, dat
-00014e20: 612c 2064 756d 705f 7768 6f6c 653d 6461  a, dump_whole=da
-00014e30: 7461 5f69 735f 6e6f 745f 6466 0a20 2020  ta_is_not_df.   
-00014e40: 2020 2020 2020 2020 2029 2c0a 2020 2020           ),.    
-00014e50: 2020 2020 2020 2020 6669 656c 6473 3d66          fields=f
-00014e60: 6965 6c64 732c 0a20 2020 2020 2020 2020  ields,.         
-00014e70: 2020 206f 7074 696f 6e73 3d6f 7074 696f     options=optio
-00014e80: 6e73 2c0a 2020 2020 2020 2020 2020 2020  ns,.            
-00014e90: 7469 746c 653d 7469 746c 652c 0a20 2020  title=title,.   
-00014ea0: 2020 2020 2020 2020 2072 6f77 735f 7369           rows_si
-00014eb0: 7a65 3d72 6f77 735f 7369 7a65 2c0a 2020  ze=rows_size,.  
-00014ec0: 2020 2020 2020 2020 2020 636f 6c73 5f73            cols_s
-00014ed0: 697a 653d 636f 6c73 5f73 697a 652c 0a20  ize=cols_size,. 
-00014ee0: 2020 2020 2020 2020 2020 2070 6164 6469             paddi
-00014ef0: 6e67 3d70 6164 6469 6e67 2c0a 2020 2020  ng=padding,.    
-00014f00: 2020 2020 290a 0a20 2020 2023 2045 4368      )..    # ECh
-00014f10: 6172 7473 0a20 2020 206c 696e 6520 3d20  arts.    line = 
-00014f20: 6164 645f 746f 5f67 656e 6572 616c 5f61  add_to_general_a
-00014f30: 7379 6e63 5f67 726f 7570 286c 696e 655f  sync_group(line_
-00014f40: 6368 6172 7429 0a20 2020 2062 6172 203d  chart).    bar =
-00014f50: 2061 6464 5f74 6f5f 6765 6e65 7261 6c5f   add_to_general_
-00014f60: 6173 796e 635f 6772 6f75 7028 6261 725f  async_group(bar_
-00014f70: 6368 6172 7429 0a20 2020 2073 7461 636b  chart).    stack
-00014f80: 6564 5f62 6172 203d 2061 6464 5f74 6f5f  ed_bar = add_to_
-00014f90: 6765 6e65 7261 6c5f 6173 796e 635f 6772  general_async_gr
-00014fa0: 6f75 7028 7374 6163 6b65 645f 6261 725f  oup(stacked_bar_
-00014fb0: 6368 6172 7429 0a20 2020 2061 7265 6120  chart).    area 
-00014fc0: 3d20 6164 645f 746f 5f67 656e 6572 616c  = add_to_general
-00014fd0: 5f61 7379 6e63 5f67 726f 7570 2861 7265  _async_group(are
-00014fe0: 615f 6368 6172 7429 0a20 2020 2073 7461  a_chart).    sta
-00014ff0: 636b 6564 5f61 7265 6120 3d20 6164 645f  cked_area = add_
-00015000: 746f 5f67 656e 6572 616c 5f61 7379 6e63  to_general_async
-00015010: 5f67 726f 7570 2873 7461 636b 6564 5f61  _group(stacked_a
-00015020: 7265 615f 6368 6172 7429 0a20 2020 2073  rea_chart).    s
-00015030: 6361 7474 6572 203d 2061 6464 5f74 6f5f  catter = add_to_
-00015040: 6765 6e65 7261 6c5f 6173 796e 635f 6772  general_async_gr
-00015050: 6f75 7028 7363 6174 7465 725f 6368 6172  oup(scatter_char
-00015060: 7429 0a20 2020 2068 6f72 697a 6f6e 7461  t).    horizonta
-00015070: 6c5f 6261 7220 3d20 6164 645f 746f 5f67  l_bar = add_to_g
-00015080: 656e 6572 616c 5f61 7379 6e63 5f67 726f  eneral_async_gro
-00015090: 7570 2868 6f72 697a 6f6e 7461 6c5f 6261  up(horizontal_ba
-000150a0: 725f 6368 6172 7429 0a20 2020 2073 7461  r_chart).    sta
-000150b0: 636b 6564 5f68 6f72 697a 6f6e 7461 6c5f  cked_horizontal_
-000150c0: 6261 7220 3d20 6164 645f 746f 5f67 656e  bar = add_to_gen
-000150d0: 6572 616c 5f61 7379 6e63 5f67 726f 7570  eral_async_group
-000150e0: 2873 7461 636b 6564 5f68 6f72 697a 6f6e  (stacked_horizon
-000150f0: 7461 6c5f 6261 725f 6368 6172 7429 0a20  tal_bar_chart). 
-00015100: 2020 207a 6572 6f5f 6365 6e74 6572 6564     zero_centered
-00015110: 5f62 6172 203d 2061 6464 5f74 6f5f 6765  _bar = add_to_ge
-00015120: 6e65 7261 6c5f 6173 796e 635f 6772 6f75  neral_async_grou
-00015130: 7028 7a65 726f 5f63 656e 7465 7265 645f  p(zero_centered_
-00015140: 6261 725f 6368 6172 7429 0a20 2020 2066  bar_chart).    f
-00015150: 756e 6e65 6c20 3d20 6164 645f 746f 5f67  unnel = add_to_g
-00015160: 656e 6572 616c 5f61 7379 6e63 5f67 726f  eneral_async_gro
-00015170: 7570 2866 756e 6e65 6c5f 6368 6172 7429  up(funnel_chart)
-00015180: 0a20 2020 2074 7265 6520 3d20 6164 645f  .    tree = add_
-00015190: 746f 5f67 656e 6572 616c 5f61 7379 6e63  to_general_async
-000151a0: 5f67 726f 7570 2874 7265 655f 6368 6172  _group(tree_char
-000151b0: 7429 0a20 2020 2072 6164 6172 203d 2061  t).    radar = a
-000151c0: 6464 5f74 6f5f 6765 6e65 7261 6c5f 6173  dd_to_general_as
-000151d0: 796e 635f 6772 6f75 7028 7261 6461 725f  ync_group(radar_
-000151e0: 6368 6172 7429 0a20 2020 2070 6965 203d  chart).    pie =
-000151f0: 2061 6464 5f74 6f5f 6765 6e65 7261 6c5f   add_to_general_
-00015200: 6173 796e 635f 6772 6f75 7028 7069 655f  async_group(pie_
-00015210: 6368 6172 7429 0a20 2020 2064 6f75 6768  chart).    dough
-00015220: 6e75 7420 3d20 6164 645f 746f 5f67 656e  nut = add_to_gen
-00015230: 6572 616c 5f61 7379 6e63 5f67 726f 7570  eral_async_group
-00015240: 2864 6f75 6768 6e75 745f 6368 6172 7429  (doughnut_chart)
-00015250: 0a20 2020 2072 6f73 6520 3d20 6164 645f  .    rose = add_
-00015260: 746f 5f67 656e 6572 616c 5f61 7379 6e63  to_general_async
-00015270: 5f67 726f 7570 2872 6f73 655f 6368 6172  _group(rose_char
-00015280: 7429 0a20 2020 2073 756e 6275 7273 7420  t).    sunburst 
-00015290: 3d20 6164 645f 746f 5f67 656e 6572 616c  = add_to_general
-000152a0: 5f61 7379 6e63 5f67 726f 7570 2873 756e  _async_group(sun
-000152b0: 6275 7273 745f 6368 6172 7429 0a20 2020  burst_chart).   
-000152c0: 2074 7265 656d 6170 203d 2061 6464 5f74   treemap = add_t
-000152d0: 6f5f 6765 6e65 7261 6c5f 6173 796e 635f  o_general_async_
-000152e0: 6772 6f75 7028 7472 6565 6d61 705f 6368  group(treemap_ch
-000152f0: 6172 7429 0a20 2020 2073 616e 6b65 7920  art).    sankey 
-00015300: 3d20 6164 645f 746f 5f67 656e 6572 616c  = add_to_general
-00015310: 5f61 7379 6e63 5f67 726f 7570 2873 616e  _async_group(san
-00015320: 6b65 795f 6368 6172 7429 0a20 2020 2068  key_chart).    h
-00015330: 6561 746d 6170 203d 2061 6464 5f74 6f5f  eatmap = add_to_
-00015340: 6765 6e65 7261 6c5f 6173 796e 635f 6772  general_async_gr
-00015350: 6f75 7028 6865 6174 6d61 705f 6368 6172  oup(heatmap_char
-00015360: 7429 0a20 2020 2070 7265 6469 6374 6976  t).    predictiv
-00015370: 655f 6c69 6e65 203d 2061 6464 5f74 6f5f  e_line = add_to_
-00015380: 6765 6e65 7261 6c5f 6173 796e 635f 6772  general_async_gr
-00015390: 6f75 7028 7072 6564 6963 7469 7665 5f6c  oup(predictive_l
-000153a0: 696e 655f 6368 6172 7429 0a20 2020 2073  ine_chart).    s
-000153b0: 7065 6564 5f67 6175 6765 203d 2061 6464  peed_gauge = add
-000153c0: 5f74 6f5f 6765 6e65 7261 6c5f 6173 796e  _to_general_asyn
-000153d0: 635f 6772 6f75 7028 7370 6565 645f 6761  c_group(speed_ga
-000153e0: 7567 655f 6368 6172 7429 0a20 2020 2073  uge_chart).    s
-000153f0: 6869 6d6f 6b75 5f67 6175 6765 203d 2061  himoku_gauge = a
-00015400: 6464 5f74 6f5f 6765 6e65 7261 6c5f 6173  dd_to_general_as
-00015410: 796e 635f 6772 6f75 7028 7368 696d 6f6b  ync_group(shimok
-00015420: 755f 6761 7567 655f 6368 6172 7429 0a20  u_gauge_chart). 
-00015430: 2020 2073 6869 6d6f 6b75 5f67 6175 6765     shimoku_gauge
-00015440: 735f 6772 6f75 7020 3d20 6164 645f 746f  s_group = add_to
-00015450: 5f67 656e 6572 616c 5f61 7379 6e63 5f67  _general_async_g
-00015460: 726f 7570 2873 6869 6d6f 6b75 5f67 6175  roup(shimoku_gau
-00015470: 6765 735f 6772 6f75 7029 0a20 2020 2067  ges_group).    g
-00015480: 6175 6765 5f69 6e64 6963 6174 6f72 203d  auge_indicator =
-00015490: 2061 6464 5f74 6f5f 6765 6e65 7261 6c5f   add_to_general_
-000154a0: 6173 796e 635f 6772 6f75 7028 6761 7567  async_group(gaug
-000154b0: 655f 696e 6469 6361 746f 7229 0a20 2020  e_indicator).   
-000154c0: 2074 6f70 5f62 6f74 746f 6d5f 6172 6561   top_bottom_area
-000154d0: 203d 2061 6464 5f74 6f5f 6765 6e65 7261   = add_to_genera
-000154e0: 6c5f 6173 796e 635f 6772 6f75 7028 746f  l_async_group(to
-000154f0: 705f 626f 7474 6f6d 5f61 7265 615f 6368  p_bottom_area_ch
-00015500: 6172 7473 290a 2020 2020 746f 705f 626f  arts).    top_bo
-00015510: 7474 6f6d 5f6c 696e 6520 3d20 6164 645f  ttom_line = add_
-00015520: 746f 5f67 656e 6572 616c 5f61 7379 6e63  to_general_async
-00015530: 5f67 726f 7570 2874 6f70 5f62 6f74 746f  _group(top_botto
-00015540: 6d5f 6c69 6e65 5f63 6861 7274 7329 0a20  m_line_charts). 
-00015550: 2020 206c 696e 655f 7769 7468 5f63 6f6e     line_with_con
-00015560: 6669 6465 6e63 655f 6172 6561 203d 2061  fidence_area = a
-00015570: 6464 5f74 6f5f 6765 6e65 7261 6c5f 6173  dd_to_general_as
-00015580: 796e 635f 6772 6f75 7028 0a20 2020 2020  ync_group(.     
-00015590: 2020 206c 696e 655f 7769 7468 5f63 6f6e     line_with_con
-000155a0: 6669 6465 6e63 655f 6172 6561 5f63 6861  fidence_area_cha
-000155b0: 7274 0a20 2020 2029 0a20 2020 2073 6361  rt.    ).    sca
-000155c0: 7474 6572 5f77 6974 685f 6566 6665 6374  tter_with_effect
-000155d0: 203d 2061 6464 5f74 6f5f 6765 6e65 7261   = add_to_genera
-000155e0: 6c5f 6173 796e 635f 6772 6f75 7028 7363  l_async_group(sc
-000155f0: 6174 7465 725f 7769 7468 5f65 6666 6563  atter_with_effec
-00015600: 745f 6368 6172 7429 0a20 2020 2077 6174  t_chart).    wat
-00015610: 6572 6661 6c6c 203d 2061 6464 5f74 6f5f  erfall = add_to_
-00015620: 6765 6e65 7261 6c5f 6173 796e 635f 6772  general_async_gr
-00015630: 6f75 7028 7761 7465 7266 616c 6c5f 6368  oup(waterfall_ch
-00015640: 6172 7429 0a20 2020 206c 696e 655f 616e  art).    line_an
-00015650: 645f 6261 725f 6368 6172 7473 203d 2061  d_bar_charts = a
-00015660: 6464 5f74 6f5f 6765 6e65 7261 6c5f 6173  dd_to_general_as
-00015670: 796e 635f 6772 6f75 7028 6c69 6e65 5f61  ync_group(line_a
-00015680: 6e64 5f62 6172 5f63 6861 7274 7329 0a20  nd_bar_charts). 
-00015690: 2020 2073 6567 6d65 6e74 6564 5f6c 696e     segmented_lin
-000156a0: 6520 3d20 6164 645f 746f 5f67 656e 6572  e = add_to_gener
-000156b0: 616c 5f61 7379 6e63 5f67 726f 7570 2873  al_async_group(s
-000156c0: 6567 6d65 6e74 6564 5f6c 696e 655f 6368  egmented_line_ch
-000156d0: 6172 7429 0a20 2020 206d 6172 6b65 645f  art).    marked_
-000156e0: 6c69 6e65 203d 2061 6464 5f74 6f5f 6765  line = add_to_ge
-000156f0: 6e65 7261 6c5f 6173 796e 635f 6772 6f75  neral_async_grou
-00015700: 7028 6d61 726b 6564 5f6c 696e 655f 6368  p(marked_line_ch
-00015710: 6172 7429 0a20 2020 2073 6567 6d65 6e74  art).    segment
-00015720: 6564 5f61 7265 6120 3d20 6164 645f 746f  ed_area = add_to
-00015730: 5f67 656e 6572 616c 5f61 7379 6e63 5f67  _general_async_g
-00015740: 726f 7570 2873 6567 6d65 6e74 6564 5f61  roup(segmented_a
-00015750: 7265 615f 6368 6172 7429 0a0a 2020 2020  rea_chart)..    
-00015760: 2320 4265 6e74 6f62 6f78 2063 6861 7274  # Bentobox chart
-00015770: 7320 6465 6669 6e65 6420 696e 2074 6865  s defined in the
-00015780: 2062 656e 746f 626f 785f 6368 6172 7473   bentobox_charts
-00015790: 2e70 7920 6669 6c65 0a20 2020 2069 6e66  .py file.    inf
-000157a0: 6f67 7261 7068 6963 735f 7465 7874 5f62  ographics_text_b
-000157b0: 7562 626c 6520 3d20 6164 645f 746f 5f67  ubble = add_to_g
-000157c0: 656e 6572 616c 5f61 7379 6e63 5f67 726f  eneral_async_gro
-000157d0: 7570 2869 6e66 6f67 7261 7068 6963 735f  up(infographics_
-000157e0: 7465 7874 5f62 7562 626c 6529 0a20 2020  text_bubble).   
-000157f0: 2063 6861 7274 5f61 6e64 5f6d 6f64 616c   chart_and_modal
-00015800: 5f62 7574 746f 6e20 3d20 6164 645f 746f  _button = add_to
-00015810: 5f67 656e 6572 616c 5f61 7379 6e63 5f67  _general_async_g
-00015820: 726f 7570 2863 6861 7274 5f61 6e64 5f6d  roup(chart_and_m
-00015830: 6f64 616c 5f62 7574 746f 6e29 0a20 2020  odal_button).   
-00015840: 2063 6861 7274 5f61 6e64 5f69 6e64 6963   chart_and_indic
-00015850: 6174 6f72 7320 3d20 6164 645f 746f 5f67  ators = add_to_g
-00015860: 656e 6572 616c 5f61 7379 6e63 5f67 726f  eneral_async_gro
-00015870: 7570 2863 6861 7274 5f61 6e64 5f69 6e64  up(chart_and_ind
-00015880: 6963 6174 6f72 7329 0a20 2020 2069 6e64  icators).    ind
-00015890: 6963 6174 6f72 735f 7769 7468 5f68 6561  icators_with_hea
-000158a0: 6465 7220 3d20 6164 645f 746f 5f67 656e  der = add_to_gen
-000158b0: 6572 616c 5f61 7379 6e63 5f67 726f 7570  eral_async_group
-000158c0: 2869 6e64 6963 6174 6f72 735f 7769 7468  (indicators_with
-000158d0: 5f68 6561 6465 7229 0a20 2020 206c 696e  _header).    lin
-000158e0: 655f 7769 7468 5f73 756d 6d61 7279 203d  e_with_summary =
-000158f0: 2061 6464 5f74 6f5f 6765 6e65 7261 6c5f   add_to_general_
-00015900: 6173 796e 635f 6772 6f75 7028 6c69 6e65  async_group(line
-00015910: 5f77 6974 685f 7375 6d6d 6172 7929 0a    _with_summary).
+0000b150: 224c 696e 652f 6172 726f 772d 7570 220a  "Line/arrow-up".
+0000b160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b170: 2020 2020 6966 2064 665f 726f 775b 2276      if df_row["v
+0000b180: 616c 7565 225d 203e 2030 0a20 2020 2020  alue"] > 0.     
+0000b190: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+0000b1a0: 6c73 6520 224c 696e 652f 6172 726f 772d  lse "Line/arrow-
+0000b1b0: 646f 776e 220a 2020 2020 2020 2020 2020  down".          
+0000b1c0: 2020 2020 2020 2020 2020 6966 2064 665f            if df_
+0000b1d0: 726f 775b 2276 616c 7565 225d 203c 2030  row["value"] < 0
+0000b1e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000b1f0: 2020 2020 2065 6c73 6520 226e 6f6e 6522       else "none"
+0000b200: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000b210: 2029 0a0a 2020 2020 2020 2020 2020 2020   )..            
+0000b220: 7365 6c66 2e73 696e 676c 655f 696e 6469  self.single_indi
+0000b230: 6361 746f 7228 0a20 2020 2020 2020 2020  cator(.         
+0000b240: 2020 2020 2020 2064 6174 613d 6466 5f72         data=df_r
+0000b250: 6f77 2e64 726f 706e 6128 292e 746f 5f64  ow.dropna().to_d
+0000b260: 6963 7428 292c 0a20 2020 2020 2020 2020  ict(),.         
+0000b270: 2020 2020 2020 206f 7264 6572 3d6f 7264         order=ord
+0000b280: 6572 2c0a 2020 2020 2020 2020 2020 2020  er,.            
+0000b290: 2020 2020 636f 6c73 5f73 697a 653d 636f      cols_size=co
+0000b2a0: 6c73 5f73 697a 652c 0a20 2020 2020 2020  ls_size,.       
+0000b2b0: 2020 2020 2020 2020 2072 6f77 735f 7369           rows_si
+0000b2c0: 7a65 3d72 6f77 735f 7369 7a65 2c0a 2020  ze=rows_size,.  
+0000b2d0: 2020 2020 2020 2020 2020 2020 2020 7061                pa
+0000b2e0: 6464 696e 673d 7061 6464 696e 672c 0a20  dding=padding,. 
+0000b2f0: 2020 2020 2020 2020 2020 2029 0a0a 2020             )..  
+0000b300: 2020 2020 2020 2020 2020 6966 2069 7369            if isi
+0000b310: 6e73 7461 6e63 6528 6f72 6465 722c 2069  nstance(order, i
+0000b320: 6e74 293a 0a20 2020 2020 2020 2020 2020  nt):.           
+0000b330: 2020 2020 206f 7264 6572 202b 3d20 310a       order += 1.
+0000b340: 0a20 2020 2020 2020 2069 6620 7665 7274  .        if vert
+0000b350: 6963 616c 3a0a 2020 2020 2020 2020 2020  ical:.          
+0000b360: 2020 7365 6c66 2e70 6f70 5f6f 7574 5f6f    self.pop_out_o
+0000b370: 665f 6265 6e74 6f62 6f78 2829 0a0a 2020  f_bentobox()..  
+0000b380: 2020 2020 2020 7265 7475 726e 206f 7264        return ord
+0000b390: 6572 0a0a 2020 2020 6173 796e 6320 6465  er..    async de
+0000b3a0: 6620 5f62 7574 746f 6e28 0a20 2020 2020  f _button(.     
+0000b3b0: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
+0000b3c0: 206c 6162 656c 3a20 7374 722c 0a20 2020   label: str,.   
+0000b3d0: 2020 2020 206f 7264 6572 3a20 696e 742c       order: int,
+0000b3e0: 0a20 2020 2020 2020 2072 6f77 735f 7369  .        rows_si
+0000b3f0: 7a65 3a20 4f70 7469 6f6e 616c 5b69 6e74  ze: Optional[int
+0000b400: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
+0000b410: 2020 636f 6c73 5f73 697a 653a 204f 7074    cols_size: Opt
+0000b420: 696f 6e61 6c5b 696e 745d 203d 204e 6f6e  ional[int] = Non
+0000b430: 652c 0a20 2020 2020 2020 2061 6c69 676e  e,.        align
+0000b440: 3a20 4f70 7469 6f6e 616c 5b73 7472 5d20  : Optional[str] 
+0000b450: 3d20 2273 7472 6574 6368 222c 0a20 2020  = "stretch",.   
+0000b460: 2020 2020 2070 6164 6469 6e67 3a20 4f70       padding: Op
+0000b470: 7469 6f6e 616c 5b73 7472 5d20 3d20 4e6f  tional[str] = No
+0000b480: 6e65 2c0a 2020 2020 2020 2020 6f6e 5f63  ne,.        on_c
+0000b490: 6c69 636b 5f65 7665 6e74 733a 204f 7074  lick_events: Opt
+0000b4a0: 696f 6e61 6c5b 556e 696f 6e5b 6c69 7374  ional[Union[list
+0000b4b0: 5b64 6963 745d 2c20 6469 6374 5d5d 203d  [dict], dict]] =
+0000b4c0: 204e 6f6e 652c 0a20 2020 2029 3a0a 2020   None,.    ):.  
+0000b4d0: 2020 2020 2020 2222 2243 7265 6174 6520        """Create 
+0000b4e0: 6120 6275 7474 6f6e 2069 6e20 7468 6520  a button in the 
+0000b4f0: 6461 7368 626f 6172 642e 2222 220a 2020  dashboard.""".  
+0000b500: 2020 2020 2020 6966 206e 6f74 206f 6e5f        if not on_
+0000b510: 636c 6963 6b5f 6576 656e 7473 3a0a 2020  click_events:.  
+0000b520: 2020 2020 2020 2020 2020 6f6e 5f63 6c69            on_cli
+0000b530: 636b 5f65 7665 6e74 7320 3d20 5b5d 0a20  ck_events = []. 
+0000b540: 2020 2020 2020 2065 6c69 6620 6973 696e         elif isin
+0000b550: 7374 616e 6365 286f 6e5f 636c 6963 6b5f  stance(on_click_
+0000b560: 6576 656e 7473 2c20 6469 6374 293a 0a20  events, dict):. 
+0000b570: 2020 2020 2020 2020 2020 206f 6e5f 636c             on_cl
+0000b580: 6963 6b5f 6576 656e 7473 203d 205b 6f6e  ick_events = [on
+0000b590: 5f63 6c69 636b 5f65 7665 6e74 735d 0a0a  _click_events]..
+0000b5a0: 2020 2020 2020 2020 6177 6169 7420 7365          await se
+0000b5b0: 6c66 2e5f 6372 6561 7465 5f63 6861 7274  lf._create_chart
+0000b5c0: 280a 2020 2020 2020 2020 2020 2020 6368  (.            ch
+0000b5d0: 6172 745f 636c 6173 733d 4275 7474 6f6e  art_class=Button
+0000b5e0: 2c0a 2020 2020 2020 2020 2020 2020 6f72  ,.            or
+0000b5f0: 6465 723d 6f72 6465 722c 0a20 2020 2020  der=order,.     
+0000b600: 2020 2020 2020 2073 697a 6550 6164 6469         sizePaddi
+0000b610: 6e67 3d70 6164 6469 6e67 2c0a 2020 2020  ng=padding,.    
+0000b620: 2020 2020 2020 2020 7369 7a65 526f 7773          sizeRows
+0000b630: 3d72 6f77 735f 7369 7a65 2c0a 2020 2020  =rows_size,.    
+0000b640: 2020 2020 2020 2020 7369 7a65 436f 6c75          sizeColu
+0000b650: 6d6e 733d 636f 6c73 5f73 697a 652c 0a20  mns=cols_size,. 
+0000b660: 2020 2020 2020 2020 2020 2070 726f 7065             prope
+0000b670: 7274 6965 733d 6469 6374 280a 2020 2020  rties=dict(.    
+0000b680: 2020 2020 2020 2020 2020 2020 7465 7874              text
+0000b690: 3d6c 6162 656c 2c20 616c 6967 6e3d 616c  =label, align=al
+0000b6a0: 6967 6e2c 2065 7665 6e74 733d 6469 6374  ign, events=dict
+0000b6b0: 286f 6e43 6c69 636b 3d6f 6e5f 636c 6963  (onClick=on_clic
+0000b6c0: 6b5f 6576 656e 7473 290a 2020 2020 2020  k_events).      
+0000b6d0: 2020 2020 2020 292c 0a20 2020 2020 2020        ),.       
+0000b6e0: 2029 0a0a 2020 2020 4061 6464 5f74 6f5f   )..    @add_to_
+0000b6f0: 6765 6e65 7261 6c5f 6173 796e 635f 6772  general_async_gr
+0000b700: 6f75 700a 2020 2020 6173 796e 6320 6465  oup.    async de
+0000b710: 6620 6275 7474 6f6e 280a 2020 2020 2020  f button(.      
+0000b720: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
+0000b730: 6c61 6265 6c3a 2073 7472 2c0a 2020 2020  label: str,.    
+0000b740: 2020 2020 6f72 6465 723a 2069 6e74 2c0a      order: int,.
+0000b750: 2020 2020 2020 2020 726f 7773 5f73 697a          rows_siz
+0000b760: 653a 204f 7074 696f 6e61 6c5b 696e 745d  e: Optional[int]
+0000b770: 203d 2031 2c0a 2020 2020 2020 2020 636f   = 1,.        co
+0000b780: 6c73 5f73 697a 653a 2069 6e74 203d 2032  ls_size: int = 2
+0000b790: 2c0a 2020 2020 2020 2020 616c 6967 6e3a  ,.        align:
+0000b7a0: 204f 7074 696f 6e61 6c5b 7374 725d 203d   Optional[str] =
+0000b7b0: 2022 7374 7265 7463 6822 2c0a 2020 2020   "stretch",.    
+0000b7c0: 2020 2020 7061 6464 696e 673a 204f 7074      padding: Opt
+0000b7d0: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
+0000b7e0: 652c 0a20 2020 2020 2020 206f 6e5f 636c  e,.        on_cl
+0000b7f0: 6963 6b5f 6576 656e 7473 3a20 4f70 7469  ick_events: Opti
+0000b800: 6f6e 616c 5b55 6e69 6f6e 5b6c 6973 745b  onal[Union[list[
+0000b810: 6469 6374 5d2c 2064 6963 745d 5d20 3d20  dict], dict]] = 
+0000b820: 4e6f 6e65 2c0a 2020 2020 293a 0a20 2020  None,.    ):.   
+0000b830: 2020 2020 2022 2222 4372 6561 7465 2061       """Create a
+0000b840: 2062 7574 746f 6e20 696e 2074 6865 2064   button in the d
+0000b850: 6173 6862 6f61 7264 2e22 2222 0a20 2020  ashboard.""".   
+0000b860: 2020 2020 2061 7761 6974 2073 656c 662e       await self.
+0000b870: 5f62 7574 746f 6e28 0a20 2020 2020 2020  _button(.       
+0000b880: 2020 2020 206c 6162 656c 3d6c 6162 656c       label=label
+0000b890: 2c0a 2020 2020 2020 2020 2020 2020 6f72  ,.            or
+0000b8a0: 6465 723d 6f72 6465 722c 0a20 2020 2020  der=order,.     
+0000b8b0: 2020 2020 2020 2072 6f77 735f 7369 7a65         rows_size
+0000b8c0: 3d72 6f77 735f 7369 7a65 2c0a 2020 2020  =rows_size,.    
+0000b8d0: 2020 2020 2020 2020 636f 6c73 5f73 697a          cols_siz
+0000b8e0: 653d 636f 6c73 5f73 697a 652c 0a20 2020  e=cols_size,.   
+0000b8f0: 2020 2020 2020 2020 2061 6c69 676e 3d61           align=a
+0000b900: 6c69 676e 2c0a 2020 2020 2020 2020 2020  lign,.          
+0000b910: 2020 7061 6464 696e 673d 7061 6464 696e    padding=paddin
+0000b920: 672c 0a20 2020 2020 2020 2020 2020 206f  g,.            o
+0000b930: 6e5f 636c 6963 6b5f 6576 656e 7473 3d6f  n_click_events=o
+0000b940: 6e5f 636c 6963 6b5f 6576 656e 7473 2c0a  n_click_events,.
+0000b950: 2020 2020 2020 2020 290a 0a20 2020 2040          )..    @
+0000b960: 6164 645f 746f 5f67 656e 6572 616c 5f61  add_to_general_a
+0000b970: 7379 6e63 5f67 726f 7570 0a20 2020 2061  sync_group.    a
+0000b980: 7379 6e63 2064 6566 206d 6f64 616c 5f62  sync def modal_b
+0000b990: 7574 746f 6e28 0a20 2020 2020 2020 2073  utton(.        s
+0000b9a0: 656c 662c 0a20 2020 2020 2020 206c 6162  elf,.        lab
+0000b9b0: 656c 3a20 7374 722c 0a20 2020 2020 2020  el: str,.       
+0000b9c0: 206f 7264 6572 3a20 696e 742c 0a20 2020   order: int,.   
+0000b9d0: 2020 2020 206d 6f64 616c 3a20 7374 722c       modal: str,
+0000b9e0: 0a20 2020 2020 2020 2072 6f77 735f 7369  .        rows_si
+0000b9f0: 7a65 3a20 4f70 7469 6f6e 616c 5b69 6e74  ze: Optional[int
+0000ba00: 5d20 3d20 312c 0a20 2020 2020 2020 2063  ] = 1,.        c
+0000ba10: 6f6c 735f 7369 7a65 3a20 696e 7420 3d20  ols_size: int = 
+0000ba20: 322c 0a20 2020 2020 2020 2061 6c69 676e  2,.        align
+0000ba30: 3a20 4f70 7469 6f6e 616c 5b73 7472 5d20  : Optional[str] 
+0000ba40: 3d20 2273 7472 6574 6368 222c 0a20 2020  = "stretch",.   
+0000ba50: 2020 2020 2070 6164 6469 6e67 3a20 4f70       padding: Op
+0000ba60: 7469 6f6e 616c 5b73 7472 5d20 3d20 4e6f  tional[str] = No
+0000ba70: 6e65 2c0a 2020 2020 293a 0a20 2020 2020  ne,.    ):.     
+0000ba80: 2020 2022 2222 0a20 2020 2020 2020 2043     """.        C
+0000ba90: 7265 6174 6520 6120 6275 7474 6f6e 2069  reate a button i
+0000baa0: 6e20 7468 6520 6461 7368 626f 6172 6420  n the dashboard 
+0000bab0: 7468 6174 206f 7065 6e73 2061 206d 6f64  that opens a mod
+0000bac0: 616c 2e0a 2020 2020 2020 2020 3a70 6172  al..        :par
+0000bad0: 616d 206c 6162 656c 3a20 7468 6520 6c61  am label: the la
+0000bae0: 6265 6c20 6f66 2074 6865 2062 7574 746f  bel of the butto
+0000baf0: 6e0a 2020 2020 2020 2020 3a70 6172 616d  n.        :param
+0000bb00: 206f 7264 6572 3a20 7468 6520 6f72 6465   order: the orde
+0000bb10: 7220 6f66 2074 6865 2062 7574 746f 6e0a  r of the button.
+0000bb20: 2020 2020 2020 2020 3a70 6172 616d 206d          :param m
+0000bb30: 6f64 616c 3a20 7468 6520 6e61 6d65 206f  odal: the name o
+0000bb40: 6620 7468 6520 6d6f 6461 6c0a 2020 2020  f the modal.    
+0000bb50: 2020 2020 3a70 6172 616d 2072 6f77 735f      :param rows_
+0000bb60: 7369 7a65 3a20 7468 6520 7369 7a65 206f  size: the size o
+0000bb70: 6620 7468 6520 726f 7773 2069 6e20 7468  f the rows in th
+0000bb80: 6520 6275 7474 6f6e 0a20 2020 2020 2020  e button.       
+0000bb90: 203a 7061 7261 6d20 636f 6c73 5f73 697a   :param cols_siz
+0000bba0: 653a 2074 6865 2073 697a 6520 6f66 2074  e: the size of t
+0000bbb0: 6865 2063 6f6c 756d 6e73 2069 6e20 7468  he columns in th
+0000bbc0: 6520 6275 7474 6f6e 0a20 2020 2020 2020  e button.       
+0000bbd0: 203a 7061 7261 6d20 616c 6967 6e3a 2074   :param align: t
+0000bbe0: 6865 2061 6c69 676e 6d65 6e74 206f 6620  he alignment of 
+0000bbf0: 7468 6520 6275 7474 6f6e 0a20 2020 2020  the button.     
+0000bc00: 2020 203a 7061 7261 6d20 7061 6464 696e     :param paddin
+0000bc10: 673a 2074 6865 2070 6164 6469 6e67 206f  g: the padding o
+0000bc20: 6620 7468 6520 6275 7474 6f6e 0a20 2020  f the button.   
+0000bc30: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+0000bc40: 206d 6f64 616c 5f69 6420 3d20 2861 7761   modal_id = (awa
+0000bc50: 6974 2073 656c 662e 5f67 6574 5f6d 6f64  it self._get_mod
+0000bc60: 616c 286d 6f64 616c 2929 5b22 6964 225d  al(modal))["id"]
+0000bc70: 0a0a 2020 2020 2020 2020 6177 6169 7420  ..        await 
+0000bc80: 7365 6c66 2e5f 6275 7474 6f6e 280a 2020  self._button(.  
+0000bc90: 2020 2020 2020 2020 2020 6c61 6265 6c3d            label=
+0000bca0: 6c61 6265 6c2c 0a20 2020 2020 2020 2020  label,.         
+0000bcb0: 2020 206f 7264 6572 3d6f 7264 6572 2c0a     order=order,.
+0000bcc0: 2020 2020 2020 2020 2020 2020 7061 6464              padd
+0000bcd0: 696e 673d 7061 6464 696e 672c 0a20 2020  ing=padding,.   
+0000bce0: 2020 2020 2020 2020 2072 6f77 735f 7369           rows_si
+0000bcf0: 7a65 3d72 6f77 735f 7369 7a65 2c0a 2020  ze=rows_size,.  
+0000bd00: 2020 2020 2020 2020 2020 636f 6c73 5f73            cols_s
+0000bd10: 697a 653d 636f 6c73 5f73 697a 652c 0a20  ize=cols_size,. 
+0000bd20: 2020 2020 2020 2020 2020 2061 6c69 676e             align
+0000bd30: 3d61 6c69 676e 2c0a 2020 2020 2020 2020  =align,.        
+0000bd40: 2020 2020 6f6e 5f63 6c69 636b 5f65 7665      on_click_eve
+0000bd50: 6e74 733d 5b0a 2020 2020 2020 2020 2020  nts=[.          
+0000bd60: 2020 2020 2020 6469 6374 280a 2020 2020        dict(.    
+0000bd70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bd80: 6163 7469 6f6e 3d22 6f70 656e 4d6f 6461  action="openModa
+0000bd90: 6c22 2c0a 2020 2020 2020 2020 2020 2020  l",.            
+0000bda0: 2020 2020 2020 2020 7061 7261 6d73 3d64          params=d
+0000bdb0: 6963 7428 0a20 2020 2020 2020 2020 2020  ict(.           
+0000bdc0: 2020 2020 2020 2020 2020 2020 206d 6f64               mod
+0000bdd0: 616c 4964 3d6d 6f64 616c 5f69 642c 0a20  alId=modal_id,. 
+0000bde0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bdf0: 2020 2029 2c0a 2020 2020 2020 2020 2020     ),.          
+0000be00: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+0000be10: 2020 2020 5d2c 0a20 2020 2020 2020 2029      ],.        )
+0000be20: 0a0a 2020 2020 4061 6464 5f74 6f5f 6765  ..    @add_to_ge
+0000be30: 6e65 7261 6c5f 6173 796e 635f 6772 6f75  neral_async_grou
+0000be40: 700a 2020 2020 6173 796e 6320 6465 6620  p.    async def 
+0000be50: 6163 7469 7669 7479 5f62 7574 746f 6e28  activity_button(
+0000be60: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
+0000be70: 2020 2020 2020 206c 6162 656c 3a20 7374         label: st
+0000be80: 722c 0a20 2020 2020 2020 206f 7264 6572  r,.        order
+0000be90: 3a20 696e 742c 0a20 2020 2020 2020 2072  : int,.        r
+0000bea0: 6f77 735f 7369 7a65 3a20 4f70 7469 6f6e  ows_size: Option
+0000beb0: 616c 5b69 6e74 5d20 3d20 312c 0a20 2020  al[int] = 1,.   
+0000bec0: 2020 2020 2063 6f6c 735f 7369 7a65 3a20       cols_size: 
+0000bed0: 696e 7420 3d20 322c 0a20 2020 2020 2020  int = 2,.       
+0000bee0: 2061 6c69 676e 3a20 4f70 7469 6f6e 616c   align: Optional
+0000bef0: 5b73 7472 5d20 3d20 2273 7472 6574 6368  [str] = "stretch
+0000bf00: 222c 0a20 2020 2020 2020 2070 6164 6469  ",.        paddi
+0000bf10: 6e67 3a20 4f70 7469 6f6e 616c 5b73 7472  ng: Optional[str
+0000bf20: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
+0000bf30: 2020 6163 7469 7669 7479 5f69 643a 204f    activity_id: O
+0000bf40: 7074 696f 6e61 6c5b 7374 725d 203d 204e  ptional[str] = N
+0000bf50: 6f6e 652c 0a20 2020 2020 2020 2061 6374  one,.        act
+0000bf60: 6976 6974 795f 6e61 6d65 3a20 4f70 7469  ivity_name: Opti
+0000bf70: 6f6e 616c 5b73 7472 5d20 3d20 4e6f 6e65  onal[str] = None
+0000bf80: 2c0a 2020 2020 293a 0a20 2020 2020 2020  ,.    ):.       
+0000bf90: 2022 2222 0a20 2020 2020 2020 2043 7265   """.        Cre
+0000bfa0: 6174 6520 6120 6275 7474 6f6e 2069 6e20  ate a button in 
+0000bfb0: 7468 6520 6461 7368 626f 6172 6420 7468  the dashboard th
+0000bfc0: 6174 2065 7865 6375 7465 7320 616e 2061  at executes an a
+0000bfd0: 6374 6976 6974 792e 0a20 2020 2020 2020  ctivity..       
+0000bfe0: 203a 7061 7261 6d20 6c61 6265 6c3a 2074   :param label: t
+0000bff0: 6865 206c 6162 656c 206f 6620 7468 6520  he label of the 
+0000c000: 6275 7474 6f6e 0a20 2020 2020 2020 203a  button.        :
+0000c010: 7061 7261 6d20 6f72 6465 723a 2074 6865  param order: the
+0000c020: 206f 7264 6572 206f 6620 7468 6520 6275   order of the bu
+0000c030: 7474 6f6e 0a20 2020 2020 2020 203a 7061  tton.        :pa
+0000c040: 7261 6d20 726f 7773 5f73 697a 653a 2074  ram rows_size: t
+0000c050: 6865 2073 697a 6520 6f66 2074 6865 2072  he size of the r
+0000c060: 6f77 7320 696e 2074 6865 2062 7574 746f  ows in the butto
+0000c070: 6e0a 2020 2020 2020 2020 3a70 6172 616d  n.        :param
+0000c080: 2063 6f6c 735f 7369 7a65 3a20 7468 6520   cols_size: the 
+0000c090: 7369 7a65 206f 6620 7468 6520 636f 6c75  size of the colu
+0000c0a0: 6d6e 7320 696e 2074 6865 2062 7574 746f  mns in the butto
+0000c0b0: 6e0a 2020 2020 2020 2020 3a70 6172 616d  n.        :param
+0000c0c0: 2061 6c69 676e 3a20 7468 6520 616c 6967   align: the alig
+0000c0d0: 6e6d 656e 7420 6f66 2074 6865 2062 7574  nment of the but
+0000c0e0: 746f 6e0a 2020 2020 2020 2020 3a70 6172  ton.        :par
+0000c0f0: 616d 2070 6164 6469 6e67 3a20 7468 6520  am padding: the 
+0000c100: 7061 6464 696e 6720 6f66 2074 6865 2062  padding of the b
+0000c110: 7574 746f 6e0a 2020 2020 2020 2020 3a70  utton.        :p
+0000c120: 6172 616d 2061 6374 6976 6974 795f 6964  aram activity_id
+0000c130: 3a20 7468 6520 6964 206f 6620 7468 6520  : the id of the 
+0000c140: 6163 7469 7669 7479 0a20 2020 2020 2020  activity.       
+0000c150: 203a 7061 7261 6d20 6163 7469 7669 7479   :param activity
+0000c160: 5f6e 616d 653a 2074 6865 206e 616d 6520  _name: the name 
+0000c170: 6f66 2074 6865 2061 6374 6976 6974 790a  of the activity.
+0000c180: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+0000c190: 2020 2020 6163 7469 7669 7479 5f69 6420      activity_id 
+0000c1a0: 3d20 2861 7761 6974 2073 656c 662e 5f61  = (await self._a
+0000c1b0: 7070 2e67 6574 5f61 6374 6976 6974 7928  pp.get_activity(
+0000c1c0: 6163 7469 7669 7479 5f69 642c 2061 6374  activity_id, act
+0000c1d0: 6976 6974 795f 6e61 6d65 2929 5b22 6964  ivity_name))["id
+0000c1e0: 225d 0a0a 2020 2020 2020 2020 6177 6169  "]..        awai
+0000c1f0: 7420 7365 6c66 2e5f 6275 7474 6f6e 280a  t self._button(.
+0000c200: 2020 2020 2020 2020 2020 2020 6c61 6265              labe
+0000c210: 6c3d 6c61 6265 6c2c 0a20 2020 2020 2020  l=label,.       
+0000c220: 2020 2020 206f 7264 6572 3d6f 7264 6572       order=order
+0000c230: 2c0a 2020 2020 2020 2020 2020 2020 7061  ,.            pa
+0000c240: 6464 696e 673d 7061 6464 696e 672c 0a20  dding=padding,. 
+0000c250: 2020 2020 2020 2020 2020 2072 6f77 735f             rows_
+0000c260: 7369 7a65 3d72 6f77 735f 7369 7a65 2c0a  size=rows_size,.
+0000c270: 2020 2020 2020 2020 2020 2020 636f 6c73              cols
+0000c280: 5f73 697a 653d 636f 6c73 5f73 697a 652c  _size=cols_size,
+0000c290: 0a20 2020 2020 2020 2020 2020 2061 6c69  .            ali
+0000c2a0: 676e 3d61 6c69 676e 2c0a 2020 2020 2020  gn=align,.      
+0000c2b0: 2020 2020 2020 6f6e 5f63 6c69 636b 5f65        on_click_e
+0000c2c0: 7665 6e74 733d 5b0a 2020 2020 2020 2020  vents=[.        
+0000c2d0: 2020 2020 2020 2020 6469 6374 280a 2020          dict(.  
+0000c2e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c2f0: 2020 6163 7469 6f6e 3d22 7275 6e41 6374    action="runAct
+0000c300: 6976 6974 7922 2c0a 2020 2020 2020 2020  ivity",.        
+0000c310: 2020 2020 2020 2020 2020 2020 7061 7261              para
+0000c320: 6d73 3d64 6963 7428 0a20 2020 2020 2020  ms=dict(.       
+0000c330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c340: 2061 6374 6976 6974 7949 643d 6163 7469   activityId=acti
+0000c350: 7669 7479 5f69 642c 0a20 2020 2020 2020  vity_id,.       
+0000c360: 2020 2020 2020 2020 2020 2020 2029 2c0a               ),.
+0000c370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c380: 290a 2020 2020 2020 2020 2020 2020 5d2c  ).            ],
+0000c390: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
+0000c3a0: 4061 6464 5f74 6f5f 6765 6e65 7261 6c5f  @add_to_general_
+0000c3b0: 6173 796e 635f 6772 6f75 700a 2020 2020  async_group.    
+0000c3c0: 6173 796e 6320 6465 6620 6163 7469 6f6e  async def action
+0000c3d0: 5f62 7574 746f 6e28 0a20 2020 2020 2020  _button(.       
+0000c3e0: 2073 656c 662c 0a20 2020 2020 2020 206c   self,.        l
+0000c3f0: 6162 656c 3a20 7374 722c 0a20 2020 2020  abel: str,.     
+0000c400: 2020 206f 7264 6572 3a20 696e 742c 0a20     order: int,. 
+0000c410: 2020 2020 2020 2061 6374 696f 6e5f 6964         action_id
+0000c420: 3a20 7374 722c 0a20 2020 2020 2020 2072  : str,.        r
+0000c430: 6f77 735f 7369 7a65 3a20 4f70 7469 6f6e  ows_size: Option
+0000c440: 616c 5b69 6e74 5d20 3d20 312c 0a20 2020  al[int] = 1,.   
+0000c450: 2020 2020 2063 6f6c 735f 7369 7a65 3a20       cols_size: 
+0000c460: 696e 7420 3d20 322c 0a20 2020 2020 2020  int = 2,.       
+0000c470: 2061 6c69 676e 3a20 4f70 7469 6f6e 616c   align: Optional
+0000c480: 5b73 7472 5d20 3d20 2273 7472 6574 6368  [str] = "stretch
+0000c490: 222c 0a20 2020 2020 2020 2070 6164 6469  ",.        paddi
+0000c4a0: 6e67 3a20 4f70 7469 6f6e 616c 5b73 7472  ng: Optional[str
+0000c4b0: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 293a  ] = None,.    ):
+0000c4c0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+0000c4d0: 2020 2020 2043 7265 6174 6520 6120 6275       Create a bu
+0000c4e0: 7474 6f6e 2069 6e20 7468 6520 6461 7368  tton in the dash
+0000c4f0: 626f 6172 6420 7468 6174 2065 7865 6375  board that execu
+0000c500: 7465 7320 616e 2061 6374 696f 6e2e 0a20  tes an action.. 
+0000c510: 2020 2020 2020 203a 7061 7261 6d20 6c61         :param la
+0000c520: 6265 6c3a 2074 6865 206c 6162 656c 206f  bel: the label o
+0000c530: 6620 7468 6520 6275 7474 6f6e 0a20 2020  f the button.   
+0000c540: 2020 2020 203a 7061 7261 6d20 6f72 6465       :param orde
+0000c550: 723a 2074 6865 206f 7264 6572 206f 6620  r: the order of 
+0000c560: 7468 6520 6275 7474 6f6e 0a20 2020 2020  the button.     
+0000c570: 2020 203a 7061 7261 6d20 6163 7469 6f6e     :param action
+0000c580: 5f69 643a 2074 6865 2069 6420 6f66 2074  _id: the id of t
+0000c590: 6865 2061 6374 696f 6e0a 2020 2020 2020  he action.      
+0000c5a0: 2020 3a70 6172 616d 2072 6f77 735f 7369    :param rows_si
+0000c5b0: 7a65 3a20 7468 6520 7369 7a65 206f 6620  ze: the size of 
+0000c5c0: 7468 6520 726f 7773 2069 6e20 7468 6520  the rows in the 
+0000c5d0: 6275 7474 6f6e 0a20 2020 2020 2020 203a  button.        :
+0000c5e0: 7061 7261 6d20 636f 6c73 5f73 697a 653a  param cols_size:
+0000c5f0: 2074 6865 2073 697a 6520 6f66 2074 6865   the size of the
+0000c600: 2063 6f6c 756d 6e73 2069 6e20 7468 6520   columns in the 
+0000c610: 6275 7474 6f6e 0a20 2020 2020 2020 203a  button.        :
+0000c620: 7061 7261 6d20 616c 6967 6e3a 2074 6865  param align: the
+0000c630: 2061 6c69 676e 6d65 6e74 206f 6620 7468   alignment of th
+0000c640: 6520 6275 7474 6f6e 0a20 2020 2020 2020  e button.       
+0000c650: 203a 7061 7261 6d20 7061 6464 696e 673a   :param padding:
+0000c660: 2074 6865 2070 6164 6469 6e67 206f 6620   the padding of 
+0000c670: 7468 6520 6275 7474 6f6e 0a20 2020 2020  the button.     
+0000c680: 2020 2022 2222 0a20 2020 2020 2020 2061     """.        a
+0000c690: 7761 6974 2073 656c 662e 5f62 7574 746f  wait self._butto
+0000c6a0: 6e28 0a20 2020 2020 2020 2020 2020 206c  n(.            l
+0000c6b0: 6162 656c 3d6c 6162 656c 2c0a 2020 2020  abel=label,.    
+0000c6c0: 2020 2020 2020 2020 6f72 6465 723d 6f72          order=or
+0000c6d0: 6465 722c 0a20 2020 2020 2020 2020 2020  der,.           
+0000c6e0: 2070 6164 6469 6e67 3d70 6164 6469 6e67   padding=padding
+0000c6f0: 2c0a 2020 2020 2020 2020 2020 2020 726f  ,.            ro
+0000c700: 7773 5f73 697a 653d 726f 7773 5f73 697a  ws_size=rows_siz
+0000c710: 652c 0a20 2020 2020 2020 2020 2020 2063  e,.            c
+0000c720: 6f6c 735f 7369 7a65 3d63 6f6c 735f 7369  ols_size=cols_si
+0000c730: 7a65 2c0a 2020 2020 2020 2020 2020 2020  ze,.            
+0000c740: 616c 6967 6e3d 616c 6967 6e2c 0a20 2020  align=align,.   
+0000c750: 2020 2020 2020 2020 206f 6e5f 636c 6963           on_clic
+0000c760: 6b5f 6576 656e 7473 3d5b 0a20 2020 2020  k_events=[.     
+0000c770: 2020 2020 2020 2020 2020 2064 6963 7428             dict(
+0000c780: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000c790: 2020 2020 2061 6374 696f 6e3d 2272 756e       action="run
+0000c7a0: 4163 7469 6f6e 222c 0a20 2020 2020 2020  Action",.       
+0000c7b0: 2020 2020 2020 2020 2020 2020 2070 6172               par
+0000c7c0: 616d 733d 6469 6374 280a 2020 2020 2020  ams=dict(.      
+0000c7d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c7e0: 2020 6163 7469 6f6e 4964 3d61 6374 696f    actionId=actio
+0000c7f0: 6e5f 6964 2c0a 2020 2020 2020 2020 2020  n_id,.          
+0000c800: 2020 2020 2020 2020 2020 292c 0a20 2020            ),.   
+0000c810: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
+0000c820: 2020 2020 2020 2020 2020 205d 2c0a 2020             ],.  
+0000c830: 2020 2020 2020 290a 0a20 2020 2040 6461        )..    @da
+0000c840: 7461 636c 6173 730a 2020 2020 636c 6173  taclass.    clas
+0000c850: 7320 5461 626c 6542 7574 746f 6e43 6f6c  s TableButtonCol
+0000c860: 756d 6e44 6566 696e 6974 696f 6e3a 0a20  umnDefinition:. 
+0000c870: 2020 2020 2020 2063 6f6c 756d 6e5f 6e61         column_na
+0000c880: 6d65 3a20 7374 720a 2020 2020 2020 2020  me: str.        
+0000c890: 6c61 6265 6c3a 2073 7472 0a20 2020 2020  label: str.     
+0000c8a0: 2020 206d 6f64 616c 735f 636f 6c75 6d6e     modals_column
+0000c8b0: 3a20 4f70 7469 6f6e 616c 5b73 7472 5d20  : Optional[str] 
+0000c8c0: 3d20 4e6f 6e65 0a20 2020 2020 2020 2061  = None.        a
+0000c8d0: 6374 6976 6974 6965 735f 636f 6c75 6d6e  ctivities_column
+0000c8e0: 3a20 4f70 7469 6f6e 616c 5b73 7472 5d20  : Optional[str] 
+0000c8f0: 3d20 4e6f 6e65 0a20 2020 2020 2020 2061  = None.        a
+0000c900: 6374 696f 6e73 5f63 6f6c 756d 6e3a 204f  ctions_column: O
+0000c910: 7074 696f 6e61 6c5b 7374 725d 203d 204e  ptional[str] = N
+0000c920: 6f6e 650a 0a20 2020 2061 7379 6e63 2064  one..    async d
+0000c930: 6566 205f 6164 645f 6275 7474 6f6e 735f  ef _add_buttons_
+0000c940: 746f 5f74 6162 6c65 5f64 6174 6128 0a20  to_table_data(. 
+0000c950: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
+0000c960: 2020 2020 2064 6174 613a 2055 6e69 6f6e       data: Union
+0000c970: 5b73 7472 2c20 7064 2e44 6174 6146 7261  [str, pd.DataFra
+0000c980: 6d65 2c20 6c69 7374 5b64 6963 745d 5d2c  me, list[dict]],
+0000c990: 0a20 2020 2020 2020 2062 7574 746f 6e73  .        buttons
+0000c9a0: 5f63 6f6c 756d 6e5f 6465 6669 6e69 7469  _column_definiti
+0000c9b0: 6f6e 3a20 5461 626c 6542 7574 746f 6e43  on: TableButtonC
+0000c9c0: 6f6c 756d 6e44 6566 696e 6974 696f 6e2c  olumnDefinition,
+0000c9d0: 0a20 2020 2029 202d 3e20 7064 2e44 6174  .    ) -> pd.Dat
+0000c9e0: 6146 7261 6d65 3a0a 2020 2020 2020 2020  aFrame:.        
+0000c9f0: 6966 206e 6f74 2069 7369 6e73 7461 6e63  if not isinstanc
+0000ca00: 6528 6461 7461 2c20 2870 642e 4461 7461  e(data, (pd.Data
+0000ca10: 4672 616d 652c 206c 6973 7429 293a 0a20  Frame, list)):. 
+0000ca20: 2020 2020 2020 2020 2020 206c 6f67 5f65             log_e
+0000ca30: 7272 6f72 280a 2020 2020 2020 2020 2020  rror(.          
+0000ca40: 2020 2020 2020 6c6f 6767 6572 2c0a 2020        logger,.  
+0000ca50: 2020 2020 2020 2020 2020 2020 2020 2254                "T
+0000ca60: 6f20 6372 6561 7465 2061 2074 6162 6c65  o create a table
+0000ca70: 2077 6974 6820 6275 7474 6f6e 732c 2074   with buttons, t
+0000ca80: 6865 2064 6174 6120 6d75 7374 206e 6f74  he data must not
+0000ca90: 2022 0a20 2020 2020 2020 2020 2020 2020   ".             
+0000caa0: 2020 2022 6265 2061 2073 6861 7265 6420     "be a shared 
+0000cab0: 6461 7461 2065 6e74 7279 2e20 5468 6520  data entry. The 
+0000cac0: 7265 6173 6f6e 2069 7320 7468 6174 2074  reason is that t
+0000cad0: 6865 2064 6174 6120 6d75 7374 2062 6520  he data must be 
+0000cae0: 6d6f 6469 6669 6564 2074 6f20 696e 636c  modified to incl
+0000caf0: 7564 6520 220a 2020 2020 2020 2020 2020  ude ".          
+0000cb00: 2020 2020 2020 2274 6865 2062 7574 746f        "the butto
+0000cb10: 6e73 2e22 2c0a 2020 2020 2020 2020 2020  ns.",.          
+0000cb20: 2020 2020 2020 4461 7461 4572 726f 722c        DataError,
+0000cb30: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
+0000cb40: 2020 2020 2020 206d 6f64 616c 735f 636f         modals_co
+0000cb50: 6c75 6d6e 203d 2062 7574 746f 6e73 5f63  lumn = buttons_c
+0000cb60: 6f6c 756d 6e5f 6465 6669 6e69 7469 6f6e  olumn_definition
+0000cb70: 2e6d 6f64 616c 735f 636f 6c75 6d6e 0a20  .modals_column. 
+0000cb80: 2020 2020 2020 2061 6374 6976 6974 6965         activitie
+0000cb90: 735f 636f 6c75 6d6e 203d 2062 7574 746f  s_column = butto
+0000cba0: 6e73 5f63 6f6c 756d 6e5f 6465 6669 6e69  ns_column_defini
+0000cbb0: 7469 6f6e 2e61 6374 6976 6974 6965 735f  tion.activities_
+0000cbc0: 636f 6c75 6d6e 0a20 2020 2020 2020 2061  column.        a
+0000cbd0: 6374 696f 6e73 5f63 6f6c 756d 6e20 3d20  ctions_column = 
+0000cbe0: 6275 7474 6f6e 735f 636f 6c75 6d6e 5f64  buttons_column_d
+0000cbf0: 6566 696e 6974 696f 6e2e 6163 7469 6f6e  efinition.action
+0000cc00: 735f 636f 6c75 6d6e 0a0a 2020 2020 2020  s_column..      
+0000cc10: 2020 6461 7461 203d 2044 6174 6146 7261    data = DataFra
+0000cc20: 6d65 2864 6174 6129 0a20 2020 2020 2020  me(data).       
+0000cc30: 2062 7574 746f 6e73 5f63 6f6c 756d 6e73   buttons_columns
+0000cc40: 203d 205b 636f 6c20 666f 7220 636f 6c20   = [col for col 
+0000cc50: 696e 205b 6d6f 6461 6c73 5f63 6f6c 756d  in [modals_colum
+0000cc60: 6e2c 2061 6374 6976 6974 6965 735f 636f  n, activities_co
+0000cc70: 6c75 6d6e 2c20 6163 7469 6f6e 735f 636f  lumn, actions_co
+0000cc80: 6c75 6d6e 5d20 6966 2063 6f6c 5d0a 2020  lumn] if col].  
+0000cc90: 2020 2020 2020 6275 7474 6f6e 735f 6461        buttons_da
+0000cca0: 7461 203d 2064 6174 615b 6275 7474 6f6e  ta = data[button
+0000ccb0: 735f 636f 6c75 6d6e 735d 0a20 2020 2020  s_columns].     
+0000ccc0: 2020 2064 6174 6120 3d20 6461 7461 5b5b     data = data[[
+0000ccd0: 636f 6c20 666f 7220 636f 6c20 696e 2064  col for col in d
+0000cce0: 6174 612e 636f 6c75 6d6e 7320 6966 2063  ata.columns if c
+0000ccf0: 6f6c 206e 6f74 2069 6e20 6275 7474 6f6e  ol not in button
+0000cd00: 735f 636f 6c75 6d6e 735d 5d0a 2020 2020  s_columns]].    
+0000cd10: 2020 2020 6d6f 6461 6c5f 6964 7320 3d20      modal_ids = 
+0000cd20: 5b5d 0a20 2020 2020 2020 2069 6620 6d6f  [].        if mo
+0000cd30: 6461 6c73 5f63 6f6c 756d 6e3a 0a20 2020  dals_column:.   
+0000cd40: 2020 2020 2020 2020 2023 2043 616e 7420           # Cant 
+0000cd50: 7573 6520 6170 706c 7920 6265 6361 7573  use apply becaus
+0000cd60: 6520 6f66 2074 6865 2061 7379 6e63 0a20  e of the async. 
+0000cd70: 2020 2020 2020 2020 2020 2066 6f72 2069             for i
+0000cd80: 2c20 726f 7720 696e 2062 7574 746f 6e73  , row in buttons
+0000cd90: 5f64 6174 612e 6974 6572 726f 7773 2829  _data.iterrows()
+0000cda0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000cdb0: 2020 6d6f 6461 6c5f 6964 732e 6170 7065    modal_ids.appe
+0000cdc0: 6e64 2828 6177 6169 7420 7365 6c66 2e5f  nd((await self._
+0000cdd0: 6765 745f 6d6f 6461 6c28 726f 775b 6d6f  get_modal(row[mo
+0000cde0: 6461 6c73 5f63 6f6c 756d 6e5d 2929 5b22  dals_column]))["
+0000cdf0: 6964 225d 290a 2020 2020 2020 2020 2020  id"]).          
+0000ce00: 2020 6275 7474 6f6e 735f 6461 7461 5b22    buttons_data["
+0000ce10: 6d6f 6461 6c49 6422 5d20 3d20 6d6f 6461  modalId"] = moda
+0000ce20: 6c5f 6964 730a 0a20 2020 2020 2020 2064  l_ids..        d
+0000ce30: 6174 615b 6275 7474 6f6e 735f 636f 6c75  ata[buttons_colu
+0000ce40: 6d6e 5f64 6566 696e 6974 696f 6e2e 636f  mn_definition.co
+0000ce50: 6c75 6d6e 5f6e 616d 655d 203d 2062 7574  lumn_name] = but
+0000ce60: 746f 6e73 5f64 6174 612e 6170 706c 7928  tons_data.apply(
+0000ce70: 0a20 2020 2020 2020 2020 2020 206c 616d  .            lam
+0000ce80: 6264 6120 783a 207b 0a20 2020 2020 2020  bda x: {.       
+0000ce90: 2020 2020 2020 2020 2022 7265 706f 7274           "report
+0000cea0: 5479 7065 223a 2022 4255 5454 4f4e 222c  Type": "BUTTON",
+0000ceb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000cec0: 2022 7265 706f 7274 5072 6f70 6572 7469   "reportProperti
+0000ced0: 6573 223a 207b 0a20 2020 2020 2020 2020  es": {.         
+0000cee0: 2020 2020 2020 2020 2020 2022 7465 7874             "text
+0000cef0: 223a 2062 7574 746f 6e73 5f63 6f6c 756d  ": buttons_colum
+0000cf00: 6e5f 6465 6669 6e69 7469 6f6e 2e6c 6162  n_definition.lab
+0000cf10: 656c 2c0a 2020 2020 2020 2020 2020 2020  el,.            
+0000cf20: 2020 2020 2020 2020 2265 7665 6e74 7322          "events"
+0000cf30: 3a20 7b0a 2020 2020 2020 2020 2020 2020  : {.            
+0000cf40: 2020 2020 2020 2020 2020 2020 226f 6e43              "onC
+0000cf50: 6c69 636b 223a 205b 0a20 2020 2020 2020  lick": [.       
+0000cf60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cf70: 2020 2020 207b 0a20 2020 2020 2020 2020       {.         
+0000cf80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cf90: 2020 2020 2020 2022 6163 7469 6f6e 223a         "action":
+0000cfa0: 2022 6f70 656e 4d6f 6461 6c22 2c0a 2020   "openModal",.  
+0000cfb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cfc0: 2020 2020 2020 2020 2020 2020 2020 2270                "p
+0000cfd0: 6172 616d 7322 3a20 7b0a 2020 2020 2020  arams": {.      
+0000cfe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cff0: 2020 2020 2020 2020 2020 2020 2020 226d                "m
+0000d000: 6f64 616c 4964 223a 2078 5b22 6d6f 6461  odalId": x["moda
+0000d010: 6c49 6422 5d0a 2020 2020 2020 2020 2020  lId"].          
+0000d020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d030: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
+0000d040: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d050: 2020 2020 7d20 6966 206d 6f64 616c 735f      } if modals_
+0000d060: 636f 6c75 6d6e 2065 6c73 6520 7b7d 2c0a  column else {},.
+0000d070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d080: 2020 2020 2020 2020 2020 2020 7b0a 2020              {.  
+0000d090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d0a0: 2020 2020 2020 2020 2020 2020 2020 2261                "a
+0000d0b0: 6374 696f 6e22 3a20 2272 756e 4163 7469  ction": "runActi
+0000d0c0: 7669 7479 222c 0a20 2020 2020 2020 2020  vity",.         
+0000d0d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d0e0: 2020 2020 2020 2022 7061 7261 6d73 223a         "params":
+0000d0f0: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
+0000d100: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d110: 2020 2020 2020 2022 6163 7469 7669 7479         "activity
+0000d120: 4964 223a 2078 5b61 6374 6976 6974 6965  Id": x[activitie
+0000d130: 735f 636f 6c75 6d6e 5d0a 2020 2020 2020  s_column].      
+0000d140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d150: 2020 2020 2020 2020 2020 7d0a 2020 2020            }.    
+0000d160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d170: 2020 2020 2020 2020 7d20 6966 2061 6374          } if act
+0000d180: 6976 6974 6965 735f 636f 6c75 6d6e 2065  ivities_column e
+0000d190: 6c73 6520 7b7d 2c0a 2020 2020 2020 2020  lse {},.        
+0000d1a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d1b0: 2020 2020 7b0a 2020 2020 2020 2020 2020      {.          
+0000d1c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d1d0: 2020 2020 2020 2261 6374 696f 6e22 3a20        "action": 
+0000d1e0: 2272 756e 4163 7469 6f6e 222c 0a20 2020  "runAction",.   
+0000d1f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d200: 2020 2020 2020 2020 2020 2020 2022 7061               "pa
+0000d210: 7261 6d73 223a 207b 0a20 2020 2020 2020  rams": {.       
+0000d220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d230: 2020 2020 2020 2020 2020 2020 2022 6163               "ac
+0000d240: 7469 6f6e 4964 223a 2078 5b61 6374 696f  tionId": x[actio
+0000d250: 6e73 5f63 6f6c 756d 6e5d 0a20 2020 2020  ns_column].     
+0000d260: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d270: 2020 2020 2020 2020 2020 207d 0a20 2020             }.   
+0000d280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d290: 2020 2020 2020 2020 207d 2069 6620 6163           } if ac
+0000d2a0: 7469 6f6e 735f 636f 6c75 6d6e 2065 6c73  tions_column els
+0000d2b0: 6520 7b7d 0a20 2020 2020 2020 2020 2020  e {}.           
+0000d2c0: 2020 2020 2020 2020 2020 2020 205d 0a20               ]. 
+0000d2d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d2e0: 2020 207d 0a20 2020 2020 2020 2020 2020     }.           
+0000d2f0: 2020 2020 207d 0a20 2020 2020 2020 2020       }.         
+0000d300: 2020 207d 2c0a 2020 2020 2020 2020 2020     },.          
+0000d310: 2020 6178 6973 3d31 0a20 2020 2020 2020    axis=1.       
+0000d320: 2029 0a0a 2020 2020 2020 2020 7265 7475   )..        retu
+0000d330: 726e 2064 6174 610a 0a20 2020 2040 6164  rn data..    @ad
+0000d340: 645f 746f 5f67 656e 6572 616c 5f61 7379  d_to_general_asy
+0000d350: 6e63 5f67 726f 7570 0a20 2020 2061 7379  nc_group.    asy
+0000d360: 6e63 2064 6566 2074 6162 6c65 280a 2020  nc def table(.  
+0000d370: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
+0000d380: 2020 2020 6f72 6465 723a 2069 6e74 2c0a      order: int,.
+0000d390: 2020 2020 2020 2020 6461 7461 3a20 556e          data: Un
+0000d3a0: 696f 6e5b 7374 722c 2070 642e 4461 7461  ion[str, pd.Data
+0000d3b0: 4672 616d 652c 206c 6973 745b 6469 6374  Frame, list[dict
+0000d3c0: 5d5d 2c0a 2020 2020 2020 2020 636f 6c75  ]],.        colu
+0000d3d0: 6d6e 733a 204f 7074 696f 6e61 6c5b 6c69  mns: Optional[li
+0000d3e0: 7374 5b73 7472 5d5d 203d 204e 6f6e 652c  st[str]] = None,
+0000d3f0: 0a20 2020 2020 2020 2063 6f6c 756d 6e73  .        columns
+0000d400: 5f62 7574 746f 6e3a 2062 6f6f 6c20 3d20  _button: bool = 
+0000d410: 5472 7565 2c0a 2020 2020 2020 2020 6669  True,.        fi
+0000d420: 6c74 6572 733a 2062 6f6f 6c20 3d20 5472  lters: bool = Tr
+0000d430: 7565 2c0a 2020 2020 2020 2020 6578 706f  ue,.        expo
+0000d440: 7274 5f74 6f5f 6373 763a 2062 6f6f 6c20  rt_to_csv: bool 
+0000d450: 3d20 5472 7565 2c0a 2020 2020 2020 2020  = True,.        
+0000d460: 7365 6172 6368 3a20 626f 6f6c 203d 2054  search: bool = T
+0000d470: 7275 652c 0a20 2020 2020 2020 2070 6167  rue,.        pag
+0000d480: 655f 7369 7a65 3a20 696e 7420 3d20 3130  e_size: int = 10
+0000d490: 2c0a 2020 2020 2020 2020 7061 6765 5f73  ,.        page_s
+0000d4a0: 697a 655f 6f70 7469 6f6e 733a 204f 7074  ize_options: Opt
+0000d4b0: 696f 6e61 6c5b 6c69 7374 5b69 6e74 5d5d  ional[list[int]]
+0000d4c0: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
+0000d4d0: 2062 7574 746f 6e73 5f63 6f6c 756d 6e5f   buttons_column_
+0000d4e0: 6465 6669 6e69 7469 6f6e 3a20 4f70 7469  definition: Opti
+0000d4f0: 6f6e 616c 5b54 6162 6c65 4275 7474 6f6e  onal[TableButton
+0000d500: 436f 6c75 6d6e 4465 6669 6e69 7469 6f6e  ColumnDefinition
+0000d510: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
+0000d520: 2020 696e 6974 6961 6c5f 736f 7274 5f63    initial_sort_c
+0000d530: 6f6c 756d 6e3a 204f 7074 696f 6e61 6c5b  olumn: Optional[
+0000d540: 7374 725d 203d 204e 6f6e 652c 0a20 2020  str] = None,.   
+0000d550: 2020 2020 2073 6f72 745f 6465 7363 656e       sort_descen
+0000d560: 6469 6e67 3a20 626f 6f6c 203d 2046 616c  ding: bool = Fal
+0000d570: 7365 2c0a 2020 2020 2020 2020 636f 6c75  se,.        colu
+0000d580: 6d6e 735f 6f70 7469 6f6e 733a 204f 7074  mns_options: Opt
+0000d590: 696f 6e61 6c5b 6469 6374 5d20 3d20 4e6f  ional[dict] = No
+0000d5a0: 6e65 2c0a 2020 2020 2020 2020 6361 7465  ne,.        cate
+0000d5b0: 676f 7269 6361 6c5f 636f 6c75 6d6e 733a  gorical_columns:
+0000d5c0: 204f 7074 696f 6e61 6c5b 6c69 7374 5b73   Optional[list[s
+0000d5d0: 7472 5d5d 203d 204e 6f6e 652c 0a20 2020  tr]] = None,.   
+0000d5e0: 2020 2020 206c 6162 656c 5f63 6f6c 756d       label_colum
+0000d5f0: 6e73 3a20 4f70 7469 6f6e 616c 5b64 6963  ns: Optional[dic
+0000d600: 745d 203d 204e 6f6e 652c 0a20 2020 2020  t] = None,.     
+0000d610: 2020 2077 6562 5f6c 696e 6b5f 636f 6c75     web_link_colu
+0000d620: 6d6e 3a20 4f70 7469 6f6e 616c 5b73 7472  mn: Optional[str
+0000d630: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
+0000d640: 2020 6f70 656e 5f6c 696e 6b5f 696e 5f6e    open_link_in_n
+0000d650: 6577 5f74 6162 3a20 626f 6f6c 203d 2046  ew_tab: bool = F
+0000d660: 616c 7365 2c0a 2020 2020 2020 2020 7469  alse,.        ti
+0000d670: 746c 653a 204f 7074 696f 6e61 6c5b 7374  tle: Optional[st
+0000d680: 725d 203d 204e 6f6e 652c 0a20 2020 2020  r] = None,.     
+0000d690: 2020 2070 6164 6469 6e67 3a20 4f70 7469     padding: Opti
+0000d6a0: 6f6e 616c 5b73 7472 5d20 3d20 4e6f 6e65  onal[str] = None
+0000d6b0: 2c0a 2020 2020 2020 2020 726f 7773 5f73  ,.        rows_s
+0000d6c0: 697a 653a 204f 7074 696f 6e61 6c5b 696e  ize: Optional[in
+0000d6d0: 745d 203d 204e 6f6e 652c 0a20 2020 2020  t] = None,.     
+0000d6e0: 2020 2063 6f6c 735f 7369 7a65 3a20 4f70     cols_size: Op
+0000d6f0: 7469 6f6e 616c 5b69 6e74 5d20 3d20 4e6f  tional[int] = No
+0000d700: 6e65 2c0a 2020 2020 293a 0a20 2020 2020  ne,.    ):.     
+0000d710: 2020 2022 2222 4372 6561 7465 2061 2074     """Create a t
+0000d720: 6162 6c65 2072 6570 6f72 7420 696e 2074  able report in t
+0000d730: 6865 2064 6173 6862 6f61 7264 2e0a 2020  he dashboard..  
+0000d740: 2020 2020 2020 3a70 6172 616d 206f 7264        :param ord
+0000d750: 6572 3a20 7468 6520 6f72 6465 7220 6f66  er: the order of
+0000d760: 2074 6865 2074 6162 6c65 0a20 2020 2020   the table.     
+0000d770: 2020 203a 7061 7261 6d20 6461 7461 3a20     :param data: 
+0000d780: 7468 6520 6461 7461 206f 6620 7468 6520  the data of the 
+0000d790: 7461 626c 650a 2020 2020 2020 2020 3a70  table.        :p
+0000d7a0: 6172 616d 2063 6f6c 756d 6e73 3a20 7468  aram columns: th
+0000d7b0: 6520 636f 6c75 6d6e 7320 6f66 2074 6865  e columns of the
+0000d7c0: 2074 6162 6c65 0a20 2020 2020 2020 203a   table.        :
+0000d7d0: 7061 7261 6d20 636f 6c75 6d6e 735f 6275  param columns_bu
+0000d7e0: 7474 6f6e 3a20 7768 6574 6865 7220 746f  tton: whether to
+0000d7f0: 2073 686f 7720 7468 6520 636f 6c75 6d6e   show the column
+0000d800: 7320 6275 7474 6f6e 0a20 2020 2020 2020  s button.       
+0000d810: 203a 7061 7261 6d20 6669 6c74 6572 733a   :param filters:
+0000d820: 2077 6865 7468 6572 2074 6f20 7368 6f77   whether to show
+0000d830: 2074 6865 2066 696c 7465 7273 2062 7574   the filters but
+0000d840: 746f 6e0a 2020 2020 2020 2020 3a70 6172  ton.        :par
+0000d850: 616d 2065 7870 6f72 745f 746f 5f63 7376  am export_to_csv
+0000d860: 3a20 7768 6574 6865 7220 746f 2073 686f  : whether to sho
+0000d870: 7720 7468 6520 6578 706f 7274 2074 6f20  w the export to 
+0000d880: 6373 7620 6275 7474 6f6e 0a20 2020 2020  csv button.     
+0000d890: 2020 203a 7061 7261 6d20 7365 6172 6368     :param search
+0000d8a0: 3a20 7768 6574 6865 7220 746f 2073 686f  : whether to sho
+0000d8b0: 7720 7468 6520 7365 6172 6368 2062 6172  w the search bar
+0000d8c0: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+0000d8d0: 7061 6765 5f73 697a 653a 2074 6865 206e  page_size: the n
+0000d8e0: 756d 6265 7220 6f66 2072 6f77 7320 7065  umber of rows pe
+0000d8f0: 7220 7061 6765 0a20 2020 2020 2020 203a  r page.        :
+0000d900: 7061 7261 6d20 7061 6765 5f73 697a 655f  param page_size_
+0000d910: 6f70 7469 6f6e 733a 2074 6865 206f 7074  options: the opt
+0000d920: 696f 6e73 2066 6f72 2074 6865 206e 756d  ions for the num
+0000d930: 6265 7220 6f66 2072 6f77 7320 7065 7220  ber of rows per 
+0000d940: 7061 6765 0a20 2020 2020 2020 203a 7061  page.        :pa
+0000d950: 7261 6d20 6275 7474 6f6e 735f 636f 6c75  ram buttons_colu
+0000d960: 6d6e 5f64 6566 696e 6974 696f 6e3a 2074  mn_definition: t
+0000d970: 6865 2064 6566 696e 6974 696f 6e20 6f66  he definition of
+0000d980: 2074 6865 2062 7574 746f 6e73 2063 6f6c   the buttons col
+0000d990: 756d 6e0a 2020 2020 2020 2020 3a70 6172  umn.        :par
+0000d9a0: 616d 2069 6e69 7469 616c 5f73 6f72 745f  am initial_sort_
+0000d9b0: 636f 6c75 6d6e 3a20 7468 6520 696e 6974  column: the init
+0000d9c0: 6961 6c20 736f 7274 696e 6720 636f 6c75  ial sorting colu
+0000d9d0: 6d6e 0a20 2020 2020 2020 203a 7061 7261  mn.        :para
+0000d9e0: 6d20 736f 7274 5f64 6573 6365 6e64 696e  m sort_descendin
+0000d9f0: 673a 2077 6865 7468 6572 2074 6f20 736f  g: whether to so
+0000da00: 7274 2064 6573 6365 6e64 696e 6720 6279  rt descending by
+0000da10: 2074 6865 2069 6e69 7469 616c 2073 6f72   the initial sor
+0000da20: 7469 6e67 2063 6f6c 756d 6e0a 2020 2020  ting column.    
+0000da30: 2020 2020 3a70 6172 616d 2063 6f6c 756d      :param colum
+0000da40: 6e73 5f6f 7074 696f 6e73 3a20 7468 6520  ns_options: the 
+0000da50: 6f70 7469 6f6e 7320 666f 7220 7468 6520  options for the 
+0000da60: 636f 6c75 6d6e 730a 2020 2020 2020 2020  columns.        
+0000da70: 3a70 6172 616d 2063 6174 6567 6f72 6963  :param categoric
+0000da80: 616c 5f63 6f6c 756d 6e73 3a20 7468 6520  al_columns: the 
+0000da90: 6361 7465 676f 7269 6361 6c20 636f 6c75  categorical colu
+0000daa0: 6d6e 730a 2020 2020 2020 2020 3a70 6172  mns.        :par
+0000dab0: 616d 206c 6162 656c 5f63 6f6c 756d 6e73  am label_columns
+0000dac0: 3a20 7468 6520 6c61 6265 6c20 636f 6c75  : the label colu
+0000dad0: 6d6e 730a 2020 2020 2020 2020 3a70 6172  mns.        :par
+0000dae0: 616d 2077 6562 5f6c 696e 6b5f 636f 6c75  am web_link_colu
+0000daf0: 6d6e 3a20 7468 6520 636f 6c75 6d6e 2074  mn: the column t
+0000db00: 6f20 7573 6520 6173 2077 6562 206c 696e  o use as web lin
+0000db10: 6b0a 2020 2020 2020 2020 3a70 6172 616d  k.        :param
+0000db20: 206f 7065 6e5f 6c69 6e6b 5f69 6e5f 6e65   open_link_in_ne
+0000db30: 775f 7461 623a 2077 6865 7468 6572 2074  w_tab: whether t
+0000db40: 6f20 6f70 656e 2074 6865 2077 6562 206c  o open the web l
+0000db50: 696e 6b20 696e 2061 206e 6577 2074 6162  ink in a new tab
+0000db60: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+0000db70: 7469 746c 653a 2074 6865 2074 6974 6c65  title: the title
+0000db80: 206f 6620 7468 6520 7461 626c 650a 2020   of the table.  
+0000db90: 2020 2020 2020 3a70 6172 616d 2070 6164        :param pad
+0000dba0: 6469 6e67 3a20 7468 6520 7061 6464 696e  ding: the paddin
+0000dbb0: 6720 6f66 2074 6865 2074 6162 6c65 0a20  g of the table. 
+0000dbc0: 2020 2020 2020 203a 7061 7261 6d20 726f         :param ro
+0000dbd0: 7773 5f73 697a 653a 2074 6865 2072 6f77  ws_size: the row
+0000dbe0: 7320 7369 7a65 206f 6620 7468 6520 7461  s size of the ta
+0000dbf0: 626c 650a 2020 2020 2020 2020 3a70 6172  ble.        :par
+0000dc00: 616d 2063 6f6c 735f 7369 7a65 3a20 7468  am cols_size: th
+0000dc10: 6520 636f 6c75 6d6e 7320 7369 7a65 206f  e columns size o
+0000dc20: 6620 7468 6520 7461 626c 650a 2020 2020  f the table.    
+0000dc30: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+0000dc40: 6966 2062 7574 746f 6e73 5f63 6f6c 756d  if buttons_colum
+0000dc50: 6e5f 6465 6669 6e69 7469 6f6e 3a0a 2020  n_definition:.  
+0000dc60: 2020 2020 2020 2020 2020 6461 7461 203d            data =
+0000dc70: 2061 7761 6974 2073 656c 662e 5f61 6464   await self._add
+0000dc80: 5f62 7574 746f 6e73 5f74 6f5f 7461 626c  _buttons_to_tabl
+0000dc90: 655f 6461 7461 2864 6174 612c 2062 7574  e_data(data, but
+0000dca0: 746f 6e73 5f63 6f6c 756d 6e5f 6465 6669  tons_column_defi
+0000dcb0: 6e69 7469 6f6e 290a 2020 2020 2020 2020  nition).        
+0000dcc0: 6461 7461 5f6d 6170 7069 6e67 735f 746f  data_mappings_to
+0000dcd0: 5f74 7570 6c65 7320 3d20 6177 6169 7420  _tuples = await 
+0000dce0: 7365 6c66 2e5f 6368 6f6f 7365 5f64 6174  self._choose_dat
+0000dcf0: 6128 6f72 6465 722c 2064 6174 612c 2054  a(order, data, T
+0000dd00: 6162 6c65 290a 2020 2020 2020 2020 6966  able).        if
+0000dd10: 2069 7369 6e73 7461 6e63 6528 6461 7461   isinstance(data
+0000dd20: 2c20 7374 7229 3a0a 2020 2020 2020 2020  , str):.        
+0000dd30: 2020 2020 6461 7461 203d 2073 656c 662e      data = self.
+0000dd40: 5f73 6861 7265 645f 6461 7461 5b64 6174  _shared_data[dat
+0000dd50: 615d 0a0a 2020 2020 2020 2020 6466 203d  a]..        df =
+0000dd60: 2076 616c 6964 6174 655f 6461 7461 5f69   validate_data_i
+0000dd70: 735f 7061 6e64 6172 6162 6c65 2864 6174  s_pandarable(dat
+0000dd80: 6129 0a0a 2020 2020 2020 2020 6966 206e  a)..        if n
+0000dd90: 6f74 2063 6f6c 756d 6e73 3a0a 2020 2020  ot columns:.    
+0000dda0: 2020 2020 2020 2020 636f 6c75 6d6e 7320          columns 
+0000ddb0: 3d20 6c69 7374 2864 6174 615f 6d61 7070  = list(data_mapp
+0000ddc0: 696e 6773 5f74 6f5f 7475 706c 6573 2e6b  ings_to_tuples.k
+0000ddd0: 6579 7328 2929 0a20 2020 2020 2020 2069  eys()).        i
+0000dde0: 6620 6e6f 7420 636f 6c75 6d6e 735f 6f70  f not columns_op
+0000ddf0: 7469 6f6e 733a 0a20 2020 2020 2020 2020  tions:.         
+0000de00: 2020 2063 6f6c 756d 6e73 5f6f 7074 696f     columns_optio
+0000de10: 6e73 203d 207b 7d0a 2020 2020 2020 2020  ns = {}.        
+0000de20: 6966 206e 6f74 2063 6174 6567 6f72 6963  if not categoric
+0000de30: 616c 5f63 6f6c 756d 6e73 3a0a 2020 2020  al_columns:.    
+0000de40: 2020 2020 2020 2020 6361 7465 676f 7269          categori
+0000de50: 6361 6c5f 636f 6c75 6d6e 7320 3d20 5b5d  cal_columns = []
+0000de60: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
+0000de70: 6c61 6265 6c5f 636f 6c75 6d6e 733a 0a20  label_columns:. 
+0000de80: 2020 2020 2020 2020 2020 206c 6162 656c             label
+0000de90: 5f63 6f6c 756d 6e73 203d 207b 7d0a 2020  _columns = {}.  
+0000dea0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+0000deb0: 2020 2020 2020 2020 6175 785f 6c61 6265          aux_labe
+0000dec0: 6c5f 636f 6c75 6d6e 7320 3d20 6c61 6265  l_columns = labe
+0000ded0: 6c5f 636f 6c75 6d6e 730a 2020 2020 2020  l_columns.      
+0000dee0: 2020 2020 2020 6c61 6265 6c5f 636f 6c75        label_colu
+0000def0: 6d6e 7320 3d20 7b7d 0a20 2020 2020 2020  mns = {}.       
+0000df00: 2020 2020 2066 6f72 2068 6173 5f74 6f5f       for has_to_
+0000df10: 6265 5f74 7570 6c65 2069 6e20 6175 785f  be_tuple in aux_
+0000df20: 6c61 6265 6c5f 636f 6c75 6d6e 733a 0a20  label_columns:. 
+0000df30: 2020 2020 2020 2020 2020 2020 2020 2076                 v
+0000df40: 203d 2061 7578 5f6c 6162 656c 5f63 6f6c   = aux_label_col
+0000df50: 756d 6e73 5b68 6173 5f74 6f5f 6265 5f74  umns[has_to_be_t
+0000df60: 7570 6c65 5d0a 2020 2020 2020 2020 2020  uple].          
+0000df70: 2020 2020 2020 6966 2069 7369 6e73 7461        if isinsta
+0000df80: 6e63 6528 6861 735f 746f 5f62 655f 7475  nce(has_to_be_tu
+0000df90: 706c 652c 2073 7472 293a 0a20 2020 2020  ple, str):.     
+0000dfa0: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+0000dfb0: 6162 656c 5f63 6f6c 756d 6e73 5b28 6861  abel_columns[(ha
+0000dfc0: 735f 746f 5f62 655f 7475 706c 652c 2022  s_to_be_tuple, "
+0000dfd0: 6669 6c6c 6564 2229 5d20 3d20 760a 2020  filled")] = v.  
+0000dfe0: 2020 2020 2020 2020 2020 2020 2020 656c                el
+0000dff0: 6966 2069 7369 6e73 7461 6e63 6528 6861  if isinstance(ha
+0000e000: 735f 746f 5f62 655f 7475 706c 652c 2074  s_to_be_tuple, t
+0000e010: 7570 6c65 293a 0a20 2020 2020 2020 2020  uple):.         
+0000e020: 2020 2020 2020 2020 2020 206c 6162 656c             label
+0000e030: 5f63 6f6c 756d 6e73 5b68 6173 5f74 6f5f  _columns[has_to_
+0000e040: 6265 5f74 7570 6c65 5d20 3d20 760a 2020  be_tuple] = v.  
+0000e050: 2020 2020 2020 2020 2020 2020 2020 656c                el
+0000e060: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+0000e070: 2020 2020 2020 2020 6c6f 675f 6572 726f          log_erro
+0000e080: 7228 0a20 2020 2020 2020 2020 2020 2020  r(.             
+0000e090: 2020 2020 2020 2020 2020 206c 6f67 6765             logge
+0000e0a0: 722c 0a20 2020 2020 2020 2020 2020 2020  r,.             
+0000e0b0: 2020 2020 2020 2020 2020 2066 2249 6e76             f"Inv
+0000e0c0: 616c 6964 206c 6162 656c 5f63 6f6c 756d  alid label_colum
+0000e0d0: 6e73 206b 6579 3a20 7b68 6173 5f74 6f5f  ns key: {has_to_
+0000e0e0: 6265 5f74 7570 6c65 7d22 2c0a 2020 2020  be_tuple}",.    
+0000e0f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e100: 2020 2020 5661 6c75 6545 7272 6f72 2c0a      ValueError,.
+0000e110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e120: 2020 2020 290a 2020 2020 2020 2020 6c61      ).        la
+0000e130: 6265 6c5f 6a75 7374 5f63 6f6c 756d 6e73  bel_just_columns
+0000e140: 203d 205b 785b 305d 2066 6f72 2078 2069   = [x[0] for x i
+0000e150: 6e20 6c61 6265 6c5f 636f 6c75 6d6e 732e  n label_columns.
+0000e160: 6b65 7973 2829 5d0a 0a20 2020 2020 2020  keys()]..       
+0000e170: 205f 2c20 6461 7461 5f73 6574 2c20 5f20   _, data_set, _ 
+0000e180: 3d20 6461 7461 5f6d 6170 7069 6e67 735f  = data_mappings_
+0000e190: 746f 5f74 7570 6c65 735b 636f 6c75 6d6e  to_tuples[column
+0000e1a0: 735b 305d 5d0a 2020 2020 2020 2020 636f  s[0]].        co
+0000e1b0: 6c75 6d6e 735f 6469 6374 7320 3d20 5b5d  lumns_dicts = []
+0000e1c0: 0a20 2020 2020 2020 2072 6f77 735f 6469  .        rows_di
+0000e1d0: 6374 203d 207b 226d 6170 7069 6e67 223a  ct = {"mapping":
+0000e1e0: 207b 7d7d 0a20 2020 2020 2020 2066 6f72   {}}.        for
+0000e1f0: 2069 2c20 6e61 6d65 2069 6e20 656e 756d   i, name in enum
+0000e200: 6572 6174 6528 636f 6c75 6d6e 7329 3a0a  erate(columns):.
+0000e210: 2020 2020 2020 2020 2020 2020 636f 6c75              colu
+0000e220: 6d6e 5f6f 7074 696f 6e73 203d 207b 2266  mn_options = {"f
+0000e230: 6965 6c64 223a 206e 616d 652c 2022 6865  ield": name, "he
+0000e240: 6164 6572 4e61 6d65 223a 206e 616d 652c  aderName": name,
+0000e250: 2022 6f72 6465 7222 3a20 697d 0a0a 2020   "order": i}..  
+0000e260: 2020 2020 2020 2020 2020 6966 2062 7574            if but
+0000e270: 746f 6e73 5f63 6f6c 756d 6e5f 6465 6669  tons_column_defi
+0000e280: 6e69 7469 6f6e 2061 6e64 206e 616d 6520  nition and name 
+0000e290: 3d3d 2062 7574 746f 6e73 5f63 6f6c 756d  == buttons_colum
+0000e2a0: 6e5f 6465 6669 6e69 7469 6f6e 2e63 6f6c  n_definition.col
+0000e2b0: 756d 6e5f 6e61 6d65 3a0a 2020 2020 2020  umn_name:.      
+0000e2c0: 2020 2020 2020 2020 2020 636f 6c75 6d6e            column
+0000e2d0: 5f6f 7074 696f 6e73 5b22 7479 7065 225d  _options["type"]
+0000e2e0: 203d 2022 6275 7474 6f6e 220a 0a20 2020   = "button"..   
+0000e2f0: 2020 2020 2020 2020 2069 6620 6e61 6d65           if name
+0000e300: 2069 6e20 636f 6c75 6d6e 735f 6f70 7469   in columns_opti
+0000e310: 6f6e 733a 0a20 2020 2020 2020 2020 2020  ons:.           
+0000e320: 2020 2020 2063 6f6c 756d 6e5f 6f70 7469       column_opti
+0000e330: 6f6e 732e 7570 6461 7465 2863 6f6c 756d  ons.update(colum
+0000e340: 6e73 5f6f 7074 696f 6e73 5b6e 616d 655d  ns_options[name]
+0000e350: 290a 0a20 2020 2020 2020 2020 2020 2069  )..            i
+0000e360: 6620 6e61 6d65 2069 6e20 6361 7465 676f  f name in catego
+0000e370: 7269 6361 6c5f 636f 6c75 6d6e 733a 0a20  rical_columns:. 
+0000e380: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0000e390: 6620 6e61 6d65 2069 6e20 6c61 6265 6c5f  f name in label_
+0000e3a0: 636f 6c75 6d6e 733a 0a20 2020 2020 2020  columns:.       
+0000e3b0: 2020 2020 2020 2020 2020 2020 206c 6f67               log
+0000e3c0: 5f65 7272 6f72 280a 2020 2020 2020 2020  _error(.        
+0000e3d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e3e0: 6c6f 6767 6572 2c0a 2020 2020 2020 2020  logger,.        
+0000e3f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e400: 6622 436f 6c75 6d6e 7320 6361 6e6e 6f74  f"Columns cannot
+0000e410: 2062 6520 626f 7468 2069 6e63 6c75 6465   be both include
+0000e420: 6420 696e 2063 6174 6567 6f72 6963 616c  d in categorical
+0000e430: 5f63 6f6c 756d 6e73 2061 6e64 206c 6162  _columns and lab
+0000e440: 656c 5f63 6f6c 756d 6e73 3a20 7b6e 616d  el_columns: {nam
+0000e450: 657d 222c 0a20 2020 2020 2020 2020 2020  e}",.           
+0000e460: 2020 2020 2020 2020 2020 2020 2056 616c               Val
+0000e470: 7565 4572 726f 722c 0a20 2020 2020 2020  ueError,.       
+0000e480: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
+0000e490: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+0000e4a0: 6f6c 756d 6e5f 6f70 7469 6f6e 735b 2274  olumn_options["t
+0000e4b0: 7970 6522 5d20 3d20 2273 696e 676c 6553  ype"] = "singleS
+0000e4c0: 656c 6563 7422 0a20 2020 2020 2020 2020  elect".         
+0000e4d0: 2020 2020 2020 2063 6f6c 756d 6e5f 6f70         column_op
+0000e4e0: 7469 6f6e 735b 226f 7074 696f 6e73 225d  tions["options"]
+0000e4f0: 203d 2064 665b 6e61 6d65 5d2e 756e 6971   = df[name].uniq
+0000e500: 7565 2829 2e74 6f6c 6973 7428 290a 0a20  ue().tolist().. 
+0000e510: 2020 2020 2020 2020 2020 2069 6620 6e61             if na
+0000e520: 6d65 2069 6e20 6c61 6265 6c5f 6a75 7374  me in label_just
+0000e530: 5f63 6f6c 756d 6e73 3a0a 2020 2020 2020  _columns:.      
+0000e540: 2020 2020 2020 2020 2020 696e 6465 7820            index 
+0000e550: 3d20 6c61 6265 6c5f 6a75 7374 5f63 6f6c  = label_just_col
+0000e560: 756d 6e73 2e69 6e64 6578 286e 616d 6529  umns.index(name)
+0000e570: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e580: 2028 5f2c 2076 6172 6961 6e74 292c 206c   (_, variant), l
+0000e590: 6162 656c 5f6f 7074 696f 6e73 203d 206c  abel_options = l
+0000e5a0: 6973 7428 6c61 6265 6c5f 636f 6c75 6d6e  ist(label_column
+0000e5b0: 732e 6974 656d 7328 2929 5b69 6e64 6578  s.items())[index
+0000e5c0: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
+0000e5d0: 2020 636f 6c75 6d6e 5f6f 7074 696f 6e73    column_options
+0000e5e0: 5b22 6368 6970 7322 5d20 3d20 7b7d 0a20  ["chips"] = {}. 
+0000e5f0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+0000e600: 6f6c 756d 6e5f 6f70 7469 6f6e 735b 2263  olumn_options["c
+0000e610: 6869 7073 225d 5b22 7661 7269 616e 7422  hips"]["variant"
+0000e620: 5d20 3d20 7661 7269 616e 740a 2020 2020  ] = variant.    
+0000e630: 2020 2020 2020 2020 2020 2020 636f 6c75              colu
+0000e640: 6d6e 5f6f 7074 696f 6e73 5b22 6368 6970  mn_options["chip
+0000e650: 7322 5d5b 226f 7074 696f 6e73 225d 203d  s"]["options"] =
+0000e660: 2069 6e74 6572 7072 6574 5f6c 6162 656c   interpret_label
+0000e670: 5f69 6e66 6f28 0a20 2020 2020 2020 2020  _info(.         
+0000e680: 2020 2020 2020 2020 2020 2064 662c 206e             df, n
+0000e690: 616d 652c 206c 6162 656c 5f6f 7074 696f  ame, label_optio
+0000e6a0: 6e73 2c20 7661 7269 616e 740a 2020 2020  ns, variant.    
+0000e6b0: 2020 2020 2020 2020 2020 2020 290a 0a20              ).. 
+0000e6c0: 2020 2020 2020 2020 2020 2069 6620 6e61             if na
+0000e6d0: 6d65 203d 3d20 7765 625f 6c69 6e6b 5f63  me == web_link_c
+0000e6e0: 6f6c 756d 6e3a 0a20 2020 2020 2020 2020  olumn:.         
+0000e6f0: 2020 2020 2020 2063 6f6c 756d 6e5f 6f70         column_op
+0000e700: 7469 6f6e 735b 226c 696e 6b22 5d20 3d20  tions["link"] = 
+0000e710: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
+0000e720: 2020 2020 2020 2275 726c 223a 2022 7765        "url": "we
+0000e730: 624c 696e 6b22 2c0a 2020 2020 2020 2020  bLink",.        
+0000e740: 2020 2020 2020 2020 2020 2020 226f 7065              "ope
+0000e750: 6e4e 6577 5461 6222 3a20 6f70 656e 5f6c  nNewTab": open_l
+0000e760: 696e 6b5f 696e 5f6e 6577 5f74 6162 2c0a  ink_in_new_tab,.
+0000e770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e780: 7d0a 0a20 2020 2020 2020 2020 2020 2063  }..            c
+0000e790: 6f6c 756d 6e73 5f64 6963 7473 2e61 7070  olumns_dicts.app
+0000e7a0: 656e 6428 636f 6c75 6d6e 5f6f 7074 696f  end(column_optio
+0000e7b0: 6e73 290a 2020 2020 2020 2020 2020 2020  ns).            
+0000e7c0: 726f 7773 5f64 6963 745b 226d 6170 7069  rows_dict["mappi
+0000e7d0: 6e67 225d 5b6e 616d 655d 203d 2064 6174  ng"][name] = dat
+0000e7e0: 615f 6d61 7070 696e 6773 5f74 6f5f 7475  a_mappings_to_tu
+0000e7f0: 706c 6573 5b6e 616d 655d 5b30 5d0a 0a20  ples[name][0].. 
+0000e800: 2020 2020 2020 2069 6620 7765 625f 6c69         if web_li
+0000e810: 6e6b 5f63 6f6c 756d 6e3a 0a20 2020 2020  nk_column:.     
+0000e820: 2020 2020 2020 2072 6f77 735f 6469 6374         rows_dict
+0000e830: 5b22 6d61 7070 696e 6722 5d5b 2277 6562  ["mapping"]["web
+0000e840: 225d 203d 2064 6174 615f 6d61 7070 696e  "] = data_mappin
+0000e850: 6773 5f74 6f5f 7475 706c 6573 5b77 6562  gs_to_tuples[web
+0000e860: 5f6c 696e 6b5f 636f 6c75 6d6e 5d5b 305d  _link_column][0]
+0000e870: 0a20 2020 2020 2020 2020 2020 2072 6f77  .            row
+0000e880: 735f 6469 6374 5b22 6d61 7070 696e 6722  s_dict["mapping"
+0000e890: 5d5b 2277 6562 4c69 6e6b 225d 203d 2064  ]["webLink"] = d
+0000e8a0: 6174 615f 6d61 7070 696e 6773 5f74 6f5f  ata_mappings_to_
+0000e8b0: 7475 706c 6573 5b77 6562 5f6c 696e 6b5f  tuples[web_link_
+0000e8c0: 636f 6c75 6d6e 5d5b 0a20 2020 2020 2020  column][.       
+0000e8d0: 2020 2020 2020 2020 2030 0a20 2020 2020           0.     
+0000e8e0: 2020 2020 2020 205d 0a0a 2020 2020 2020         ]..      
+0000e8f0: 2020 5f2c 2072 6570 6f72 7420 3d20 6177    _, report = aw
+0000e900: 6169 7420 7365 6c66 2e5f 6765 745f 6368  ait self._get_ch
+0000e910: 6172 745f 7265 706f 7274 286f 7264 6572  art_report(order
+0000e920: 2c20 5461 626c 6529 0a0a 2020 2020 2020  , Table)..      
+0000e930: 2020 7264 7320 3d20 6177 6169 7420 7265    rds = await re
+0000e940: 706f 7274 2e67 6574 5f72 6570 6f72 745f  port.get_report_
+0000e950: 6461 7461 5f73 6574 7328 290a 0a20 2020  data_sets()..   
+0000e960: 2020 2020 2069 6620 280a 2020 2020 2020       if (.      
+0000e970: 2020 2020 2020 7365 6c66 2e72 6575 7365        self.reuse
+0000e980: 5f64 6174 615f 7365 7473 0a20 2020 2020  _data_sets.     
+0000e990: 2020 2020 2020 2061 6e64 2072 6570 6f72         and repor
+0000e9a0: 745b 2270 726f 7065 7274 6965 7322 5d2e  t["properties"].
+0000e9b0: 6765 7428 2263 6f6c 756d 6e73 2229 0a20  get("columns"). 
+0000e9c0: 2020 2020 2020 2020 2020 2061 6e64 2072             and r
+0000e9d0: 6570 6f72 745b 2270 726f 7065 7274 6965  eport["propertie
+0000e9e0: 7322 5d5b 2263 6f6c 756d 6e73 225d 2021  s"]["columns"] !
+0000e9f0: 3d20 636f 6c75 6d6e 735f 6469 6374 730a  = columns_dicts.
+0000ea00: 2020 2020 2020 2020 293a 0a20 2020 2020          ):.     
+0000ea10: 2020 2020 2020 206c 6f67 5f65 7272 6f72         log_error
+0000ea20: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+0000ea30: 2020 6c6f 6767 6572 2c0a 2020 2020 2020    logger,.      
+0000ea40: 2020 2020 2020 2020 2020 2243 6f6c 756d            "Colum
+0000ea50: 6e73 206f 7074 696f 6e73 2064 6f20 6e6f  ns options do no
+0000ea60: 7420 6d61 7463 6820 7468 6520 7072 6576  t match the prev
+0000ea70: 696f 7573 2063 6f6c 756d 6e73 2c20 6d6f  ious columns, mo
+0000ea80: 7374 206c 696b 656c 7920 6461 7461 2068  st likely data h
+0000ea90: 6173 2063 6861 6e67 6564 2c22 0a20 2020  as changed,".   
+0000eaa0: 2020 2020 2020 2020 2020 2020 2022 2064               " d
+0000eab0: 6f6e 2774 2075 7365 2074 6865 2072 6575  on't use the reu
+0000eac0: 7365 5f64 6174 615f 7365 7473 206f 7074  se_data_sets opt
+0000ead0: 696f 6e20 696e 2074 6869 7320 6361 7365  ion in this case
+0000eae0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+0000eaf0: 2020 2044 6174 6145 7272 6f72 2c0a 2020     DataError,.  
+0000eb00: 2020 2020 2020 2020 2020 290a 0a20 2020            )..   
+0000eb10: 2020 2020 2069 6620 7264 7320 616e 6420       if rds and 
+0000eb20: 280a 2020 2020 2020 2020 2020 2020 6e6f  (.            no
+0000eb30: 7420 7365 6c66 2e72 6575 7365 5f64 6174  t self.reuse_dat
+0000eb40: 615f 7365 7473 0a20 2020 2020 2020 2020  a_sets.         
+0000eb50: 2020 206f 7220 616e 7928 7264 5b22 6461     or any(rd["da
+0000eb60: 7461 5365 7449 6422 5d20 213d 2064 6174  taSetId"] != dat
+0000eb70: 615f 7365 745b 2269 6422 5d20 666f 7220  a_set["id"] for 
+0000eb80: 7264 2069 6e20 7264 7329 0a20 2020 2020  rd in rds).     
+0000eb90: 2020 2029 3a0a 2020 2020 2020 2020 2020     ):.          
+0000eba0: 2020 6177 6169 7420 7265 706f 7274 2e64    await report.d
+0000ebb0: 656c 6574 655f 7265 706f 7274 5f64 6174  elete_report_dat
+0000ebc0: 615f 7365 7473 286c 6f67 3d54 7275 6529  a_sets(log=True)
+0000ebd0: 0a20 2020 2020 2020 2020 2020 2072 6473  .            rds
+0000ebe0: 203d 205b 5d0a 0a20 2020 2020 2020 2069   = []..        i
+0000ebf0: 6620 6e6f 7420 7264 733a 0a20 2020 2020  f not rds:.     
+0000ec00: 2020 2020 2020 2061 7761 6974 2072 6570         await rep
+0000ec10: 6f72 742e 6372 6561 7465 5f72 6570 6f72  ort.create_repor
+0000ec20: 745f 6461 7461 5f73 6574 2828 4e6f 6e65  t_data_set((None
+0000ec30: 2c20 6461 7461 5f73 6574 2c20 4e6f 6e65  , data_set, None
+0000ec40: 2929 0a0a 2020 2020 2020 2020 7061 6769  ))..        pagi
+0000ec50: 6e61 7469 6f6e 203d 207b 2270 6167 6553  nation = {"pageS
+0000ec60: 697a 6522 3a20 7061 6765 5f73 697a 657d  ize": page_size}
+0000ec70: 0a20 2020 2020 2020 2069 6620 7061 6765  .        if page
+0000ec80: 5f73 697a 655f 6f70 7469 6f6e 733a 0a20  _size_options:. 
+0000ec90: 2020 2020 2020 2020 2020 2070 6167 696e             pagin
+0000eca0: 6174 696f 6e5b 2270 6167 6553 697a 654f  ation["pageSizeO
+0000ecb0: 7074 696f 6e73 225d 203d 2070 6167 655f  ptions"] = page_
+0000ecc0: 7369 7a65 5f6f 7074 696f 6e73 0a0a 2020  size_options..  
+0000ecd0: 2020 2020 2020 736f 7274 203d 207b 7d0a        sort = {}.
+0000ece0: 2020 2020 2020 2020 6966 2069 6e69 7469          if initi
+0000ecf0: 616c 5f73 6f72 745f 636f 6c75 6d6e 3a0a  al_sort_column:.
+0000ed00: 2020 2020 2020 2020 2020 2020 736f 7274              sort
+0000ed10: 5b22 6669 656c 6422 5d20 3d20 6461 7461  ["field"] = data
+0000ed20: 5f6d 6170 7069 6e67 735f 746f 5f74 7570  _mappings_to_tup
+0000ed30: 6c65 735b 696e 6974 6961 6c5f 736f 7274  les[initial_sort
+0000ed40: 5f63 6f6c 756d 6e5d 5b30 5d0a 2020 2020  _column][0].    
+0000ed50: 2020 2020 2020 2020 736f 7274 5b22 6469          sort["di
+0000ed60: 7265 6374 696f 6e22 5d20 3d20 2261 7363  rection"] = "asc
+0000ed70: 2220 6966 206e 6f74 2073 6f72 745f 6465  " if not sort_de
+0000ed80: 7363 656e 6469 6e67 2065 6c73 6520 2264  scending else "d
+0000ed90: 6573 6322 0a0a 2020 2020 2020 2020 6177  esc"..        aw
+0000eda0: 6169 7420 7365 6c66 2e5f 6372 6561 7465  ait self._create
+0000edb0: 5f63 6861 7274 280a 2020 2020 2020 2020  _chart(.        
+0000edc0: 2020 2020 6368 6172 745f 636c 6173 733d      chart_class=
+0000edd0: 5461 626c 652c 0a20 2020 2020 2020 2020  Table,.         
+0000ede0: 2020 206f 7264 6572 3d6f 7264 6572 2c0a     order=order,.
+0000edf0: 2020 2020 2020 2020 2020 2020 7369 7a65              size
+0000ee00: 5061 6464 696e 673d 7061 6464 696e 672c  Padding=padding,
+0000ee10: 0a20 2020 2020 2020 2020 2020 2073 697a  .            siz
+0000ee20: 6552 6f77 733d 726f 7773 5f73 697a 652c  eRows=rows_size,
+0000ee30: 0a20 2020 2020 2020 2020 2020 2073 697a  .            siz
+0000ee40: 6543 6f6c 756d 6e73 3d63 6f6c 735f 7369  eColumns=cols_si
+0000ee50: 7a65 2c0a 2020 2020 2020 2020 2020 2020  ze,.            
+0000ee60: 7469 746c 653d 7469 746c 652c 0a20 2020  title=title,.   
+0000ee70: 2020 2020 2020 2020 2070 726f 7065 7274           propert
+0000ee80: 6965 733d 6469 6374 280a 2020 2020 2020  ies=dict(.      
+0000ee90: 2020 2020 2020 2020 2020 636f 6c75 6d6e            column
+0000eea0: 733d 636f 6c75 6d6e 735f 6469 6374 732c  s=columns_dicts,
+0000eeb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000eec0: 2072 6f77 733d 726f 7773 5f64 6963 742c   rows=rows_dict,
+0000eed0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000eee0: 2063 6f6c 756d 6e73 4275 7474 6f6e 3d63   columnsButton=c
+0000eef0: 6f6c 756d 6e73 5f62 7574 746f 6e2c 0a20  olumns_button,. 
+0000ef00: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+0000ef10: 696c 7465 7273 4275 7474 6f6e 3d66 696c  iltersButton=fil
+0000ef20: 7465 7273 2c0a 2020 2020 2020 2020 2020  ters,.          
+0000ef30: 2020 2020 2020 6578 706f 7274 4275 7474        exportButt
+0000ef40: 6f6e 3d65 7870 6f72 745f 746f 5f63 7376  on=export_to_csv
+0000ef50: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000ef60: 2020 7365 6172 6368 3d73 6561 7263 682c    search=search,
+0000ef70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000ef80: 2070 6167 696e 6174 696f 6e3d 7061 6769   pagination=pagi
+0000ef90: 6e61 7469 6f6e 2c0a 2020 2020 2020 2020  nation,.        
+0000efa0: 2020 2020 2020 2020 736f 7274 3d73 6f72          sort=sor
+0000efb0: 742c 0a20 2020 2020 2020 2020 2020 2029  t,.            )
+0000efc0: 2c0a 2020 2020 2020 2020 290a 0a20 2020  ,.        )..   
+0000efd0: 2040 6164 645f 746f 5f67 656e 6572 616c   @add_to_general
+0000efe0: 5f61 7379 6e63 5f67 726f 7570 0a20 2020  _async_group.   
+0000eff0: 2061 7379 6e63 2064 6566 2069 6e70 7574   async def input
+0000f000: 5f66 6f72 6d28 0a20 2020 2020 2020 2073  _form(.        s
+0000f010: 656c 662c 0a20 2020 2020 2020 206f 7074  elf,.        opt
+0000f020: 696f 6e73 3a20 6469 6374 2c0a 2020 2020  ions: dict,.    
+0000f030: 2020 2020 6f72 6465 723a 2069 6e74 2c0a      order: int,.
+0000f040: 2020 2020 2020 2020 7061 6464 696e 673a          padding:
+0000f050: 204f 7074 696f 6e61 6c5b 7374 725d 203d   Optional[str] =
+0000f060: 204e 6f6e 652c 0a20 2020 2020 2020 2072   None,.        r
+0000f070: 6f77 735f 7369 7a65 3a20 4f70 7469 6f6e  ows_size: Option
+0000f080: 616c 5b69 6e74 5d20 3d20 4e6f 6e65 2c0a  al[int] = None,.
+0000f090: 2020 2020 2020 2020 636f 6c73 5f73 697a          cols_siz
+0000f0a0: 653a 204f 7074 696f 6e61 6c5b 696e 745d  e: Optional[int]
+0000f0b0: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
+0000f0c0: 206d 6f64 616c 3a20 4f70 7469 6f6e 616c   modal: Optional
+0000f0d0: 5b73 7472 5d20 3d20 4e6f 6e65 2c0a 2020  [str] = None,.  
+0000f0e0: 2020 2020 2020 6163 7469 7669 7479 5f69        activity_i
+0000f0f0: 643a 204f 7074 696f 6e61 6c5b 7374 725d  d: Optional[str]
+0000f100: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
+0000f110: 2061 6374 6976 6974 795f 6e61 6d65 3a20   activity_name: 
+0000f120: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
+0000f130: 4e6f 6e65 2c0a 2020 2020 2020 2020 6163  None,.        ac
+0000f140: 7469 6f6e 5f69 643a 204f 7074 696f 6e61  tion_id: Optiona
+0000f150: 6c5b 7374 725d 203d 204e 6f6e 652c 0a20  l[str] = None,. 
+0000f160: 2020 2020 2020 206f 6e5f 7375 626d 6974         on_submit
+0000f170: 5f65 7665 6e74 733a 204f 7074 696f 6e61  _events: Optiona
+0000f180: 6c5b 6c69 7374 5b64 6963 745d 5d20 3d20  l[list[dict]] = 
+0000f190: 4e6f 6e65 2c0a 2020 2020 293a 0a20 2020  None,.    ):.   
+0000f1a0: 2020 2020 2022 2222 4372 6561 7465 7320       """Creates 
+0000f1b0: 616e 2069 6e70 7574 2066 6f72 6d2e 0a20  an input form.. 
+0000f1c0: 2020 2020 2020 203a 7061 7261 6d20 6f70         :param op
+0000f1d0: 7469 6f6e 733a 2074 6865 206f 7074 696f  tions: the optio
+0000f1e0: 6e73 2066 6f72 2074 6865 2069 6e70 7574  ns for the input
+0000f1f0: 2066 6f72 6d0a 2020 2020 2020 2020 3a70   form.        :p
+0000f200: 6172 616d 206f 7264 6572 3a20 7468 6520  aram order: the 
+0000f210: 6f72 6465 7220 6f66 2074 6865 2069 6e70  order of the inp
+0000f220: 7574 2066 6f72 6d0a 2020 2020 2020 2020  ut form.        
+0000f230: 3a70 6172 616d 2070 6164 6469 6e67 3a20  :param padding: 
+0000f240: 7468 6520 7061 6464 696e 6720 6f66 2074  the padding of t
+0000f250: 6865 2069 6e70 7574 2066 6f72 6d0a 2020  he input form.  
+0000f260: 2020 2020 2020 3a70 6172 616d 2072 6f77        :param row
+0000f270: 735f 7369 7a65 3a20 7468 6520 726f 7773  s_size: the rows
+0000f280: 2073 697a 6520 6f66 2074 6865 2069 6e70   size of the inp
+0000f290: 7574 2066 6f72 6d0a 2020 2020 2020 2020  ut form.        
+0000f2a0: 3a70 6172 616d 2063 6f6c 735f 7369 7a65  :param cols_size
+0000f2b0: 3a20 7468 6520 636f 6c75 6d6e 7320 7369  : the columns si
+0000f2c0: 7a65 206f 6620 7468 6520 696e 7075 7420  ze of the input 
+0000f2d0: 666f 726d 0a20 2020 2020 2020 203a 7061  form.        :pa
+0000f2e0: 7261 6d20 6d6f 6461 6c3a 2074 6865 206d  ram modal: the m
+0000f2f0: 6f64 616c 2074 6f20 6f70 656e 2061 6674  odal to open aft
+0000f300: 6572 2073 7562 6d69 7474 696e 6720 7468  er submitting th
+0000f310: 6520 666f 726d 0a20 2020 2020 2020 203a  e form.        :
+0000f320: 7061 7261 6d20 6163 7469 7669 7479 5f69  param activity_i
+0000f330: 643a 2074 6865 2061 6374 6976 6974 7920  d: the activity 
+0000f340: 6964 2074 6f20 7275 6e20 6166 7465 7220  id to run after 
+0000f350: 7375 626d 6974 7469 6e67 2074 6865 2066  submitting the f
+0000f360: 6f72 6d0a 2020 2020 2020 2020 3a70 6172  orm.        :par
+0000f370: 616d 2061 6374 6976 6974 795f 6e61 6d65  am activity_name
+0000f380: 3a20 7468 6520 6163 7469 7669 7479 206e  : the activity n
+0000f390: 616d 6520 746f 2072 756e 2061 6674 6572  ame to run after
+0000f3a0: 2073 7562 6d69 7474 696e 6720 7468 6520   submitting the 
+0000f3b0: 666f 726d 0a20 2020 2020 2020 203a 7061  form.        :pa
+0000f3c0: 7261 6d20 6163 7469 6f6e 5f69 643a 2074  ram action_id: t
+0000f3d0: 6865 2061 6374 696f 6e20 6964 2074 6f20  he action id to 
+0000f3e0: 7275 6e20 6166 7465 7220 7375 626d 6974  run after submit
+0000f3f0: 7469 6e67 2074 6865 2066 6f72 6d0a 2020  ting the form.  
+0000f400: 2020 2020 2020 3a70 6172 616d 206f 6e5f        :param on_
+0000f410: 7375 626d 6974 5f65 7665 6e74 733a 2074  submit_events: t
+0000f420: 6865 2065 7665 6e74 7320 746f 2072 756e  he events to run
+0000f430: 2061 6674 6572 2073 7562 6d69 7474 696e   after submittin
+0000f440: 6720 7468 6520 666f 726d 0a20 2020 2020  g the form.     
+0000f450: 2020 2022 2222 0a20 2020 2020 2020 2076     """.        v
+0000f460: 616c 6964 6174 655f 696e 7075 745f 666f  alidate_input_fo
+0000f470: 726d 5f64 6174 6128 7365 6c66 2c20 6f70  rm_data(self, op
+0000f480: 7469 6f6e 7329 0a0a 2020 2020 2020 2020  tions)..        
+0000f490: 6966 206f 6e5f 7375 626d 6974 5f65 7665  if on_submit_eve
+0000f4a0: 6e74 7320 6973 204e 6f6e 653a 0a20 2020  nts is None:.   
+0000f4b0: 2020 2020 2020 2020 206f 6e5f 7375 626d           on_subm
+0000f4c0: 6974 5f65 7665 6e74 7320 3d20 5b5d 0a0a  it_events = []..
+0000f4d0: 2020 2020 2020 2020 6966 206d 6f64 616c          if modal
+0000f4e0: 3a0a 2020 2020 2020 2020 2020 2020 6d6f  :.            mo
+0000f4f0: 6461 6c5f 6964 203d 2028 6177 6169 7420  dal_id = (await 
+0000f500: 7365 6c66 2e5f 6765 745f 6d6f 6461 6c28  self._get_modal(
+0000f510: 6d6f 6461 6c29 295b 2269 6422 5d0a 2020  modal))["id"].  
+0000f520: 2020 2020 2020 2020 2020 6f6e 5f73 7562            on_sub
+0000f530: 6d69 745f 6576 656e 7473 2e61 7070 656e  mit_events.appen
+0000f540: 6428 0a20 2020 2020 2020 2020 2020 2020  d(.             
+0000f550: 2020 207b 2261 6374 696f 6e22 3a20 226f     {"action": "o
+0000f560: 7065 6e4d 6f64 616c 222c 2022 7061 7261  penModal", "para
+0000f570: 6d73 223a 207b 226d 6f64 616c 4964 223a  ms": {"modalId":
+0000f580: 206d 6f64 616c 5f69 647d 7d0a 2020 2020   modal_id}}.    
+0000f590: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
+0000f5a0: 2020 2069 6620 6163 7469 7669 7479 5f69     if activity_i
+0000f5b0: 6420 6f72 2061 6374 6976 6974 795f 6e61  d or activity_na
+0000f5c0: 6d65 3a0a 2020 2020 2020 2020 2020 2020  me:.            
+0000f5d0: 6163 7469 7669 7479 5f69 6420 3d20 2861  activity_id = (a
+0000f5e0: 7761 6974 2073 656c 662e 5f61 7070 2e67  wait self._app.g
+0000f5f0: 6574 5f61 6374 6976 6974 7928 6163 7469  et_activity(acti
+0000f600: 7669 7479 5f69 642c 2061 6374 6976 6974  vity_id, activit
+0000f610: 795f 6e61 6d65 2929 5b0a 2020 2020 2020  y_name))[.      
+0000f620: 2020 2020 2020 2020 2020 2269 6422 0a20            "id". 
+0000f630: 2020 2020 2020 2020 2020 205d 0a0a 2020             ]..  
+0000f640: 2020 2020 2020 2020 2020 6f6e 5f73 7562            on_sub
+0000f650: 6d69 745f 6576 656e 7473 2e61 7070 656e  mit_events.appen
+0000f660: 6428 0a20 2020 2020 2020 2020 2020 2020  d(.             
+0000f670: 2020 207b 0a20 2020 2020 2020 2020 2020     {.           
+0000f680: 2020 2020 2020 2020 2022 6163 7469 6f6e           "action
+0000f690: 223a 2022 7275 6e41 6374 6976 6974 7922  ": "runActivity"
+0000f6a0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000f6b0: 2020 2020 2020 2270 6172 616d 7322 3a20        "params": 
+0000f6c0: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
+0000f6d0: 2020 2020 2020 2020 2020 2261 6374 6976            "activ
+0000f6e0: 6974 7949 6422 3a20 6163 7469 7669 7479  ityId": activity
+0000f6f0: 5f69 642c 0a20 2020 2020 2020 2020 2020  _id,.           
+0000f700: 2020 2020 2020 2020 207d 2c0a 2020 2020           },.    
+0000f710: 2020 2020 2020 2020 2020 2020 7d0a 2020              }.  
+0000f720: 2020 2020 2020 2020 2020 290a 0a20 2020            )..   
+0000f730: 2020 2020 2069 6620 6163 7469 6f6e 5f69       if action_i
+0000f740: 643a 0a20 2020 2020 2020 2020 2020 206f  d:.            o
+0000f750: 6e5f 7375 626d 6974 5f65 7665 6e74 732e  n_submit_events.
+0000f760: 6170 7065 6e64 280a 2020 2020 2020 2020  append(.        
+0000f770: 2020 2020 2020 2020 7b0a 2020 2020 2020          {.      
+0000f780: 2020 2020 2020 2020 2020 2020 2020 2261                "a
+0000f790: 6374 696f 6e22 3a20 2272 756e 4163 7469  ction": "runActi
+0000f7a0: 6f6e 222c 0a20 2020 2020 2020 2020 2020  on",.           
+0000f7b0: 2020 2020 2020 2020 2022 7061 7261 6d73           "params
+0000f7c0: 223a 207b 0a20 2020 2020 2020 2020 2020  ": {.           
+0000f7d0: 2020 2020 2020 2020 2020 2020 2022 6163               "ac
+0000f7e0: 7469 6f6e 4964 223a 2061 6374 696f 6e5f  tionId": action_
+0000f7f0: 6964 2c0a 2020 2020 2020 2020 2020 2020  id,.            
+0000f800: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
+0000f810: 2020 2020 2020 2020 2020 207d 0a20 2020             }.   
+0000f820: 2020 2020 2020 2020 2029 0a0a 2020 2020           )..    
+0000f830: 2020 2020 696e 6974 6961 6c5f 6461 7461      initial_data
+0000f840: 3a20 6469 6374 203d 207b 7d0a 2020 2020  : dict = {}.    
+0000f850: 2020 2020 666f 7220 6669 656c 6473 2069      for fields i
+0000f860: 6e20 6f70 7469 6f6e 735b 2266 6965 6c64  n options["field
+0000f870: 7322 5d3a 0a20 2020 2020 2020 2020 2020  s"]:.           
+0000f880: 2066 6f72 2066 6965 6c64 2069 6e20 6669   for field in fi
+0000f890: 656c 6473 5b22 6669 656c 6473 225d 3a0a  elds["fields"]:.
+0000f8a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f8b0: 6669 656c 645f 6e61 6d65 3a20 7374 7220  field_name: str 
+0000f8c0: 3d20 6669 656c 645b 2266 6965 6c64 4e61  = field["fieldNa
+0000f8d0: 6d65 225d 0a20 2020 2020 2020 2020 2020  me"].           
+0000f8e0: 2020 2020 2069 6e70 7574 5f74 7970 653a       input_type:
+0000f8f0: 204f 7074 696f 6e61 6c5b 7374 725d 203d   Optional[str] =
+0000f900: 2066 6965 6c64 2e67 6574 2822 696e 7075   field.get("inpu
+0000f910: 7454 7970 6522 290a 2020 2020 2020 2020  tType").        
+0000f920: 2020 2020 2020 2020 6966 2069 6e70 7574          if input
+0000f930: 5f74 7970 6520 3d3d 2022 636f 6c6f 7222  _type == "color"
+0000f940: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000f950: 2020 2020 2020 696e 6974 6961 6c5f 6461        initial_da
+0000f960: 7461 5b66 6965 6c64 5f6e 616d 655d 203d  ta[field_name] =
+0000f970: 2022 2330 3030 3030 3022 0a20 2020 2020   "#000000".     
+0000f980: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
+0000f990: 696e 7075 745f 7479 7065 203d 3d20 226e  input_type == "n
+0000f9a0: 756d 6265 7222 3a0a 2020 2020 2020 2020  umber":.        
+0000f9b0: 2020 2020 2020 2020 2020 2020 696e 6974              init
+0000f9c0: 6961 6c5f 6461 7461 5b66 6965 6c64 5f6e  ial_data[field_n
+0000f9d0: 616d 655d 203d 2030 0a20 2020 2020 2020  ame] = 0.       
+0000f9e0: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
+0000f9f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fa00: 2020 2069 6e69 7469 616c 5f64 6174 615b     initial_data[
+0000fa10: 6669 656c 645f 6e61 6d65 5d20 3d20 2222  field_name] = ""
+0000fa20: 0a0a 2020 2020 2020 2020 725f 6861 7368  ..        r_hash
+0000fa30: 2c20 7265 706f 7274 203d 2061 7761 6974  , report = await
+0000fa40: 2073 656c 662e 5f67 6574 5f63 6861 7274   self._get_chart
+0000fa50: 5f72 6570 6f72 7428 6f72 6465 722c 2049  _report(order, I
+0000fa60: 6e70 7574 466f 726d 290a 2020 2020 2020  nputForm).      
+0000fa70: 2020 5f2c 2064 6174 615f 7365 742c 205f    _, data_set, _
+0000fa80: 203d 206c 6973 7428 0a20 2020 2020 2020   = list(.       
+0000fa90: 2020 2020 2028 0a20 2020 2020 2020 2020       (.         
+0000faa0: 2020 2020 2020 2061 7761 6974 2073 656c         await sel
+0000fab0: 662e 5f63 7265 6174 655f 6461 7461 5f73  f._create_data_s
+0000fac0: 6574 2872 6570 6f72 745b 2269 6422 5d2c  et(report["id"],
+0000fad0: 2069 6e69 7469 616c 5f64 6174 612c 2064   initial_data, d
+0000fae0: 756d 705f 7768 6f6c 653d 5472 7565 290a  ump_whole=True).
+0000faf0: 2020 2020 2020 2020 2020 2020 292e 7661              ).va
+0000fb00: 6c75 6573 2829 0a20 2020 2020 2020 2029  lues().        )
+0000fb10: 5b30 5d0a 0a20 2020 2020 2020 2072 6473  [0]..        rds
+0000fb20: 203d 2061 7761 6974 2072 6570 6f72 742e   = await report.
+0000fb30: 6765 745f 7265 706f 7274 5f64 6174 615f  get_report_data_
+0000fb40: 7365 7473 2829 0a20 2020 2020 2020 2069  sets().        i
+0000fb50: 6620 6c65 6e28 7264 7329 203e 2031 3a0a  f len(rds) > 1:.
+0000fb60: 2020 2020 2020 2020 2020 2020 6c6f 675f              log_
+0000fb70: 6572 726f 7228 0a20 2020 2020 2020 2020  error(.         
+0000fb80: 2020 2020 2020 206c 6f67 6765 722c 0a20         logger,. 
+0000fb90: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+0000fba0: 496e 7075 7420 666f 726d 2063 616e 206f  Input form can o
+0000fbb0: 6e6c 7920 6861 7665 206f 6e65 2063 6f6d  nly have one com
+0000fbc0: 706f 6e65 6e74 2064 6174 6120 7365 7420  ponent data set 
+0000fbd0: 6c69 6e6b 2c20 220a 2020 2020 2020 2020  link, ".        
+0000fbe0: 2020 2020 2020 2020 2274 6869 7320 6973          "this is
+0000fbf0: 2061 6e20 5344 4b20 6275 6720 706c 6561   an SDK bug plea
+0000fc00: 7365 2072 6570 6f72 7420 6974 2061 6e64  se report it and
+0000fc10: 2022 0a20 2020 2020 2020 2020 2020 2020   ".             
+0000fc20: 2020 2022 6465 6c65 7465 2074 6865 2066     "delete the f
+0000fc30: 6f72 6d20 746f 2073 6f6c 7665 2074 6865  orm to solve the
+0000fc40: 2069 7373 7565 222c 0a20 2020 2020 2020   issue",.       
+0000fc50: 2020 2020 2020 2020 2044 6174 6145 7272           DataErr
+0000fc60: 6f72 2c0a 2020 2020 2020 2020 2020 2020  or,.            
+0000fc70: 290a 0a20 2020 2020 2020 2069 6620 7264  )..        if rd
+0000fc80: 7320 616e 6420 280a 2020 2020 2020 2020  s and (.        
+0000fc90: 2020 2020 6e6f 7420 7365 6c66 2e72 6575      not self.reu
+0000fca0: 7365 5f64 6174 615f 7365 7473 0a20 2020  se_data_sets.   
+0000fcb0: 2020 2020 2020 2020 206f 7220 7264 735b           or rds[
+0000fcc0: 305d 5b22 6461 7461 5365 7449 6422 5d20  0]["dataSetId"] 
+0000fcd0: 213d 2064 6174 615f 7365 745b 2269 6422  != data_set["id"
+0000fce0: 5d0a 2020 2020 2020 2020 2020 2020 6f72  ].            or
+0000fcf0: 2072 6473 5b30 5d5b 2270 726f 7065 7274   rds[0]["propert
+0000fd00: 6965 7322 5d5b 2266 6965 6c64 7322 5d20  ies"]["fields"] 
+0000fd10: 213d 206f 7074 696f 6e73 5b22 6669 656c  != options["fiel
+0000fd20: 6473 225d 0a20 2020 2020 2020 2029 3a0a  ds"].        ):.
+0000fd30: 2020 2020 2020 2020 2020 2020 6177 6169              awai
+0000fd40: 7420 7265 706f 7274 2e64 656c 6574 655f  t report.delete_
+0000fd50: 7265 706f 7274 5f64 6174 615f 7365 7473  report_data_sets
+0000fd60: 286c 6f67 3d54 7275 6529 0a20 2020 2020  (log=True).     
+0000fd70: 2020 2020 2020 2072 6473 203d 205b 5d0a         rds = [].
+0000fd80: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
+0000fd90: 7264 733a 0a20 2020 2020 2020 2020 2020  rds:.           
+0000fda0: 2061 7761 6974 2072 6570 6f72 742e 6372   await report.cr
+0000fdb0: 6561 7465 5f72 6570 6f72 745f 6461 7461  eate_report_data
+0000fdc0: 5f73 6574 280a 2020 2020 2020 2020 2020  _set(.          
+0000fdd0: 2020 2020 2020 2822 6375 7374 6f6d 4669        ("customFi
+0000fde0: 656c 6431 222c 2064 6174 615f 7365 742c  eld1", data_set,
+0000fdf0: 204e 6f6e 6529 2c20 7072 6f70 6572 7469   None), properti
+0000fe00: 6573 3d6f 7074 696f 6e73 0a20 2020 2020  es=options.     
+0000fe10: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+0000fe20: 2020 2020 206c 6f67 6765 722e 696e 666f       logger.info
+0000fe30: 2866 2243 7265 6174 6564 2031 2063 6f6d  (f"Created 1 com
+0000fe40: 706f 6e65 6e74 2064 6174 6120 7365 7420  ponent data set 
+0000fe50: 6c69 6e6b 2066 6f72 2069 6e70 7574 2066  link for input f
+0000fe60: 6f72 6d20 6174 207b 725f 6861 7368 7d22  orm at {r_hash}"
+0000fe70: 290a 0a20 2020 2020 2020 2061 7761 6974  )..        await
+0000fe80: 2073 656c 662e 5f63 7265 6174 655f 6368   self._create_ch
+0000fe90: 6172 7428 0a20 2020 2020 2020 2020 2020  art(.           
+0000fea0: 2063 6861 7274 5f63 6c61 7373 3d49 6e70   chart_class=Inp
+0000feb0: 7574 466f 726d 2c0a 2020 2020 2020 2020  utForm,.        
+0000fec0: 2020 2020 6f72 6465 723d 6f72 6465 722c      order=order,
+0000fed0: 0a20 2020 2020 2020 2020 2020 2073 697a  .            siz
+0000fee0: 6550 6164 6469 6e67 3d70 6164 6469 6e67  ePadding=padding
+0000fef0: 2c0a 2020 2020 2020 2020 2020 2020 7369  ,.            si
+0000ff00: 7a65 526f 7773 3d72 6f77 735f 7369 7a65  zeRows=rows_size
+0000ff10: 2c0a 2020 2020 2020 2020 2020 2020 7369  ,.            si
+0000ff20: 7a65 436f 6c75 6d6e 733d 636f 6c73 5f73  zeColumns=cols_s
+0000ff30: 697a 652c 0a20 2020 2020 2020 2020 2020  ize,.           
+0000ff40: 2070 726f 7065 7274 6965 733d 7b22 6576   properties={"ev
+0000ff50: 656e 7473 223a 207b 226f 6e53 7562 6d69  ents": {"onSubmi
+0000ff60: 7422 3a20 6f6e 5f73 7562 6d69 745f 6576  t": on_submit_ev
+0000ff70: 656e 7473 7d7d 2c0a 2020 2020 2020 2020  ents}},.        
+0000ff80: 290a 0a20 2020 2064 6566 2067 656e 6572  )..    def gener
+0000ff90: 6174 655f 696e 7075 745f 666f 726d 5f67  ate_input_form_g
+0000ffa0: 726f 7570 7328 0a20 2020 2020 2020 2073  roups(.        s
+0000ffb0: 656c 662c 0a20 2020 2020 2020 206f 7264  elf,.        ord
+0000ffc0: 6572 3a20 696e 742c 0a20 2020 2020 2020  er: int,.       
+0000ffd0: 2066 6f72 6d5f 6772 6f75 7073 3a20 6469   form_groups: di
+0000ffe0: 6374 2c0a 2020 2020 2020 2020 6479 6e61  ct,.        dyna
+0000fff0: 6d69 635f 7365 7175 656e 7469 616c 5f73  mic_sequential_s
+00010000: 686f 773a 204f 7074 696f 6e61 6c5b 626f  how: Optional[bo
+00010010: 6f6c 5d20 3d20 4661 6c73 652c 0a20 2020  ol] = False,.   
+00010020: 2020 2020 2061 7574 6f5f 7365 6e64 3a20       auto_send: 
+00010030: 4f70 7469 6f6e 616c 5b62 6f6f 6c5d 203d  Optional[bool] =
+00010040: 2046 616c 7365 2c0a 2020 2020 2020 2020   False,.        
+00010050: 6e65 7874 5f67 726f 7570 5f6c 6162 656c  next_group_label
+00010060: 3a20 4f70 7469 6f6e 616c 5b73 7472 5d20  : Optional[str] 
+00010070: 3d20 224e 6578 7422 2c0a 2020 2020 2020  = "Next",.      
+00010080: 2020 726f 7773 5f73 697a 653a 204f 7074    rows_size: Opt
+00010090: 696f 6e61 6c5b 696e 745d 203d 2033 2c0a  ional[int] = 3,.
+000100a0: 2020 2020 2020 2020 636f 6c73 5f73 697a          cols_siz
+000100b0: 653a 2069 6e74 203d 2031 322c 0a20 2020  e: int = 12,.   
+000100c0: 2020 2020 2070 6164 6469 6e67 3a20 4f70       padding: Op
+000100d0: 7469 6f6e 616c 5b73 7472 5d20 3d20 4e6f  tional[str] = No
+000100e0: 6e65 2c0a 2020 2020 2020 2020 6d6f 6461  ne,.        moda
+000100f0: 6c3a 204f 7074 696f 6e61 6c5b 7374 725d  l: Optional[str]
+00010100: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
+00010110: 2061 6374 6976 6974 795f 6964 3a20 4f70   activity_id: Op
+00010120: 7469 6f6e 616c 5b73 7472 5d20 3d20 4e6f  tional[str] = No
+00010130: 6e65 2c0a 2020 2020 2020 2020 6163 7469  ne,.        acti
+00010140: 7669 7479 5f6e 616d 653a 204f 7074 696f  vity_name: Optio
+00010150: 6e61 6c5b 7374 725d 203d 204e 6f6e 652c  nal[str] = None,
+00010160: 0a20 2020 2020 2020 2061 6374 696f 6e5f  .        action_
+00010170: 6964 3a20 4f70 7469 6f6e 616c 5b73 7472  id: Optional[str
+00010180: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
+00010190: 2020 6f6e 5f73 7562 6d69 745f 6576 656e    on_submit_even
+000101a0: 7473 3a20 4f70 7469 6f6e 616c 5b6c 6973  ts: Optional[lis
+000101b0: 745b 6469 6374 5d5d 203d 204e 6f6e 652c  t[dict]] = None,
+000101c0: 0a20 2020 2029 3a0a 2020 2020 2020 2020  .    ):.        
+000101d0: 2222 2245 6173 6965 7220 7761 7920 746f  """Easier way to
+000101e0: 2063 7265 6174 6520 616e 2069 6e70 7574   create an input
+000101f0: 2066 6f72 6d2e 0a20 2020 2020 2020 203a   form..        :
+00010200: 7061 7261 6d20 6d65 6e75 5f70 6174 683a  param menu_path:
+00010210: 2074 6865 206d 656e 7520 7061 7468 206f   the menu path o
+00010220: 6620 7468 6520 696e 7075 7420 666f 726d  f the input form
+00010230: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+00010240: 6f72 6465 723a 2074 6865 206f 7264 6572  order: the order
+00010250: 206f 6620 7468 6520 696e 7075 7420 666f   of the input fo
+00010260: 726d 0a20 2020 2020 2020 203a 7061 7261  rm.        :para
+00010270: 6d20 666f 726d 5f67 726f 7570 733a 2074  m form_groups: t
+00010280: 6865 2066 6f72 6d20 6772 6f75 7073 206f  he form groups o
+00010290: 6620 7468 6520 696e 7075 7420 666f 726d  f the input form
+000102a0: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+000102b0: 6479 6e61 6d69 635f 7365 7175 656e 7469  dynamic_sequenti
+000102c0: 616c 5f73 686f 773a 2077 6865 7468 6572  al_show: whether
+000102d0: 2074 6f20 7368 6f77 2074 6865 206e 6578   to show the nex
+000102e0: 7420 6772 6f75 7020 6166 7465 7220 7375  t group after su
+000102f0: 626d 6974 7469 6e67 2074 6865 2063 7572  bmitting the cur
+00010300: 7265 6e74 2067 726f 7570 0a20 2020 2020  rent group.     
+00010310: 2020 203a 7061 7261 6d20 6175 746f 5f73     :param auto_s
+00010320: 656e 643a 2077 6865 7468 6572 2074 6f20  end: whether to 
+00010330: 6175 746f 6d61 7469 6361 6c6c 7920 7365  automatically se
+00010340: 6e64 2074 6865 2066 6f72 6d20 6166 7465  nd the form afte
+00010350: 7220 7468 6520 6c61 7374 2067 726f 7570  r the last group
+00010360: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+00010370: 6e65 7874 5f67 726f 7570 5f6c 6162 656c  next_group_label
+00010380: 3a20 7468 6520 6c61 6265 6c20 6f66 2074  : the label of t
+00010390: 6865 206e 6578 7420 6772 6f75 7020 6275  he next group bu
+000103a0: 7474 6f6e 0a20 2020 2020 2020 203a 7061  tton.        :pa
+000103b0: 7261 6d20 726f 7773 5f73 697a 653a 2074  ram rows_size: t
+000103c0: 6865 2072 6f77 7320 7369 7a65 206f 6620  he rows size of 
+000103d0: 7468 6520 696e 7075 7420 666f 726d 0a20  the input form. 
+000103e0: 2020 2020 2020 203a 7061 7261 6d20 636f         :param co
+000103f0: 6c73 5f73 697a 653a 2074 6865 2063 6f6c  ls_size: the col
+00010400: 756d 6e73 2073 697a 6520 6f66 2074 6865  umns size of the
+00010410: 2069 6e70 7574 2066 6f72 6d0a 2020 2020   input form.    
+00010420: 2020 2020 3a70 6172 616d 2070 6164 6469      :param paddi
+00010430: 6e67 3a20 7468 6520 7061 6464 696e 6720  ng: the padding 
+00010440: 6f66 2074 6865 2069 6e70 7574 2066 6f72  of the input for
+00010450: 6d0a 2020 2020 2020 2020 3a70 6172 616d  m.        :param
+00010460: 206d 6f64 616c 3a20 7468 6520 6d6f 6461   modal: the moda
+00010470: 6c20 746f 206f 7065 6e20 6166 7465 7220  l to open after 
+00010480: 7375 626d 6974 7469 6e67 2074 6865 2066  submitting the f
+00010490: 6f72 6d0a 2020 2020 2020 2020 3a70 6172  orm.        :par
+000104a0: 616d 2061 6374 6976 6974 795f 6964 3a20  am activity_id: 
+000104b0: 7468 6520 6163 7469 7669 7479 2069 6420  the activity id 
+000104c0: 746f 2072 756e 2061 6674 6572 2073 7562  to run after sub
+000104d0: 6d69 7474 696e 6720 7468 6520 666f 726d  mitting the form
+000104e0: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+000104f0: 6163 7469 7669 7479 5f6e 616d 653a 2074  activity_name: t
+00010500: 6865 2061 6374 6976 6974 7920 6e61 6d65  he activity name
+00010510: 2074 6f20 7275 6e20 6166 7465 7220 7375   to run after su
+00010520: 626d 6974 7469 6e67 2074 6865 2066 6f72  bmitting the for
+00010530: 6d0a 2020 2020 2020 2020 3a70 6172 616d  m.        :param
+00010540: 2061 6374 696f 6e5f 6964 3a20 7468 6520   action_id: the 
+00010550: 6163 7469 6f6e 2069 6420 746f 2072 756e  action id to run
+00010560: 2061 6674 6572 2073 7562 6d69 7474 696e   after submittin
+00010570: 6720 7468 6520 666f 726d 0a20 2020 2020  g the form.     
+00010580: 2020 203a 7061 7261 6d20 6f6e 5f73 7562     :param on_sub
+00010590: 6d69 745f 6576 656e 7473 3a20 7468 6520  mit_events: the 
+000105a0: 6576 656e 7473 2074 6f20 7275 6e20 6166  events to run af
+000105b0: 7465 7220 7375 626d 6974 7469 6e67 2074  ter submitting t
+000105c0: 6865 2066 6f72 6d0a 2020 2020 2020 2020  he form.        
+000105d0: 2222 220a 2020 2020 2020 2020 7265 706f  """.        repo
+000105e0: 7274 5f64 6174 615f 7365 745f 7072 6f70  rt_data_set_prop
+000105f0: 6572 7469 6573 203d 207b 2266 6965 6c64  erties = {"field
+00010600: 7322 3a20 5b5d 7d0a 2020 2020 2020 2020  s": []}.        
+00010610: 6966 2061 7574 6f5f 7365 6e64 3a0a 2020  if auto_send:.  
+00010620: 2020 2020 2020 2020 2020 7265 706f 7274            report
+00010630: 5f64 6174 615f 7365 745f 7072 6f70 6572  _data_set_proper
+00010640: 7469 6573 5b22 7661 7269 616e 7422 5d20  ties["variant"] 
+00010650: 3d20 2261 7574 6f53 656e 6422 0a0a 2020  = "autoSend"..  
+00010660: 2020 2020 2020 725f 6861 7368 203d 2073        r_hash = s
+00010670: 656c 662e 5f67 6574 5f63 6861 7274 5f68  elf._get_chart_h
+00010680: 6173 6828 6f72 6465 7229 0a0a 2020 2020  ash(order)..    
+00010690: 2020 2020 6e65 7874 5f69 6420 3d20 6622      next_id = f"
+000106a0: 7b72 5f68 6173 687d 5f30 2220 6966 2064  {r_hash}_0" if d
+000106b0: 796e 616d 6963 5f73 6571 7565 6e74 6961  ynamic_sequentia
+000106c0: 6c5f 7368 6f77 2065 6c73 6520 4e6f 6e65  l_show else None
+000106d0: 0a0a 2020 2020 2020 2020 6e65 7874 5f67  ..        next_g
+000106e0: 726f 7570 5f69 6e64 6578 203d 2031 0a20  roup_index = 1. 
+000106f0: 2020 2020 2020 2066 6f72 2066 6f72 6d5f         for form_
+00010700: 6772 6f75 705f 6e61 6d65 2c20 666f 726d  group_name, form
+00010710: 5f67 726f 7570 2069 6e20 666f 726d 5f67  _group in form_g
+00010720: 726f 7570 732e 6974 656d 7328 293a 0a20  roups.items():. 
+00010730: 2020 2020 2020 2020 2020 2066 6f72 6d5f             form_
+00010740: 6772 6f75 705f 6a73 6f6e 203d 207b 2274  group_json = {"t
+00010750: 6974 6c65 223a 2066 6f72 6d5f 6772 6f75  itle": form_grou
+00010760: 705f 6e61 6d65 2c20 2266 6965 6c64 7322  p_name, "fields"
+00010770: 3a20 666f 726d 5f67 726f 7570 7d0a 2020  : form_group}.  
+00010780: 2020 2020 2020 2020 2020 6966 206e 6578            if nex
+00010790: 745f 6964 3a0a 2020 2020 2020 2020 2020  t_id:.          
+000107a0: 2020 2020 2020 666f 726d 5f67 726f 7570        form_group
+000107b0: 5f6a 736f 6e5b 2269 6422 5d20 3d20 6e65  _json["id"] = ne
+000107c0: 7874 5f69 640a 2020 2020 2020 2020 2020  xt_id.          
+000107d0: 2020 2020 2020 6e65 7874 5f69 6420 3d20        next_id = 
+000107e0: 6622 7b72 5f68 6173 687d 5f7b 6e65 7874  f"{r_hash}_{next
+000107f0: 5f67 726f 7570 5f69 6e64 6578 7d22 0a20  _group_index}". 
+00010800: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00010810: 6f72 6d5f 6772 6f75 705f 6a73 6f6e 5b22  orm_group_json["
+00010820: 6e65 7874 466f 726d 4772 6f75 7022 5d20  nextFormGroup"] 
+00010830: 3d20 7b0a 2020 2020 2020 2020 2020 2020  = {.            
+00010840: 2020 2020 2020 2020 2269 6422 3a20 6e65          "id": ne
+00010850: 7874 5f69 642c 0a20 2020 2020 2020 2020  xt_id,.         
+00010860: 2020 2020 2020 2020 2020 2022 6c61 6265             "labe
+00010870: 6c22 3a20 6e65 7874 5f67 726f 7570 5f6c  l": next_group_l
+00010880: 6162 656c 2c0a 2020 2020 2020 2020 2020  abel,.          
+00010890: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
+000108a0: 2020 2020 2020 2020 6e65 7874 5f67 726f          next_gro
+000108b0: 7570 5f69 6e64 6578 202b 3d20 310a 2020  up_index += 1.  
+000108c0: 2020 2020 2020 2020 2020 7265 706f 7274            report
+000108d0: 5f64 6174 615f 7365 745f 7072 6f70 6572  _data_set_proper
+000108e0: 7469 6573 5b22 6669 656c 6473 225d 202b  ties["fields"] +
+000108f0: 3d20 5b66 6f72 6d5f 6772 6f75 705f 6a73  = [form_group_js
+00010900: 6f6e 5d0a 0a20 2020 2020 2020 2069 6620  on]..        if 
+00010910: 6e65 7874 5f69 643a 0a20 2020 2020 2020  next_id:.       
+00010920: 2020 2020 2064 656c 2072 6570 6f72 745f       del report_
+00010930: 6461 7461 5f73 6574 5f70 726f 7065 7274  data_set_propert
+00010940: 6965 735b 2266 6965 6c64 7322 5d5b 2d31  ies["fields"][-1
+00010950: 5d5b 226e 6578 7446 6f72 6d47 726f 7570  ]["nextFormGroup
+00010960: 225d 0a0a 2020 2020 2020 2020 7365 6c66  "]..        self
+00010970: 2e69 6e70 7574 5f66 6f72 6d28 0a20 2020  .input_form(.   
+00010980: 2020 2020 2020 2020 206f 7074 696f 6e73           options
+00010990: 3d72 6570 6f72 745f 6461 7461 5f73 6574  =report_data_set
+000109a0: 5f70 726f 7065 7274 6965 732c 0a20 2020  _properties,.   
+000109b0: 2020 2020 2020 2020 206f 7264 6572 3d6f           order=o
+000109c0: 7264 6572 2c0a 2020 2020 2020 2020 2020  rder,.          
+000109d0: 2020 726f 7773 5f73 697a 653d 726f 7773    rows_size=rows
+000109e0: 5f73 697a 652c 0a20 2020 2020 2020 2020  _size,.         
+000109f0: 2020 2063 6f6c 735f 7369 7a65 3d63 6f6c     cols_size=col
+00010a00: 735f 7369 7a65 2c0a 2020 2020 2020 2020  s_size,.        
+00010a10: 2020 2020 7061 6464 696e 673d 7061 6464      padding=padd
+00010a20: 696e 672c 0a20 2020 2020 2020 2020 2020  ing,.           
+00010a30: 206d 6f64 616c 3d6d 6f64 616c 2c0a 2020   modal=modal,.  
+00010a40: 2020 2020 2020 2020 2020 6163 7469 7669            activi
+00010a50: 7479 5f69 643d 6163 7469 7669 7479 5f69  ty_id=activity_i
+00010a60: 642c 0a20 2020 2020 2020 2020 2020 2061  d,.            a
+00010a70: 6374 6976 6974 795f 6e61 6d65 3d61 6374  ctivity_name=act
+00010a80: 6976 6974 795f 6e61 6d65 2c0a 2020 2020  ivity_name,.    
+00010a90: 2020 2020 2020 2020 6f6e 5f73 7562 6d69          on_submi
+00010aa0: 745f 6576 656e 7473 3d6f 6e5f 7375 626d  t_events=on_subm
+00010ab0: 6974 5f65 7665 6e74 732c 0a20 2020 2020  it_events,.     
+00010ac0: 2020 2020 2020 2061 6374 696f 6e5f 6964         action_id
+00010ad0: 3d61 6374 696f 6e5f 6964 2c0a 2020 2020  =action_id,.    
+00010ae0: 2020 2020 290a 0a20 2020 2061 7379 6e63      )..    async
+00010af0: 2064 6566 205f 6765 745f 696e 7075 745f   def _get_input_
+00010b00: 666f 726d 5f64 6174 6128 7365 6c66 2c20  form_data(self, 
+00010b10: 696e 7075 745f 666f 726d 3a20 496e 7075  input_form: Inpu
+00010b20: 7446 6f72 6d29 202d 3e20 6469 6374 3a0a  tForm) -> dict:.
+00010b30: 2020 2020 2020 2020 2222 2247 6574 2074          """Get t
+00010b40: 6865 2069 6e70 7574 2066 6f72 6d20 6461  he input form da
+00010b50: 7461 2e22 2222 0a20 2020 2020 2020 2072  ta.""".        r
+00010b60: 6570 6f72 745f 6461 7461 5f73 6574 203d  eport_data_set =
+00010b70: 2028 6177 6169 7420 696e 7075 745f 666f   (await input_fo
+00010b80: 726d 2e67 6574 5f72 6570 6f72 745f 6461  rm.get_report_da
+00010b90: 7461 5f73 6574 7328 2929 5b30 5d0a 2020  ta_sets())[0].  
+00010ba0: 2020 2020 2020 6461 7461 5f73 6574 203d        data_set =
+00010bb0: 2061 7761 6974 2073 656c 662e 5f61 7070   await self._app
+00010bc0: 2e67 6574 5f64 6174 615f 7365 7428 7265  .get_data_set(re
+00010bd0: 706f 7274 5f64 6174 615f 7365 745b 2264  port_data_set["d
+00010be0: 6174 6153 6574 4964 225d 290a 2020 2020  ataSetId"]).    
+00010bf0: 2020 2020 6461 7461 5f70 6f69 6e74 203d      data_point =
+00010c00: 2061 7761 6974 2064 6174 615f 7365 742e   await data_set.
+00010c10: 6765 745f 6f6e 655f 6461 7461 5f70 6f69  get_one_data_poi
+00010c20: 6e74 2829 0a20 2020 2020 2020 206c 6f67  nt().        log
+00010c30: 6765 722e 696e 666f 2866 2247 6f74 2069  ger.info(f"Got i
+00010c40: 6e70 7574 2066 6f72 6d20 6461 7461 2066  nput form data f
+00010c50: 6f72 207b 7374 7228 696e 7075 745f 666f  or {str(input_fo
+00010c60: 726d 297d 2229 0a20 2020 2020 2020 2072  rm)}").        r
+00010c70: 6574 7572 6e20 7b0a 2020 2020 2020 2020  eturn {.        
+00010c80: 2020 2020 2272 6570 6f72 7449 6422 3a20      "reportId": 
+00010c90: 696e 7075 745f 666f 726d 5b22 6964 225d  input_form["id"]
+00010ca0: 2c0a 2020 2020 2020 2020 2020 2020 226f  ,.            "o
+00010cb0: 7264 6572 223a 2069 6e70 7574 5f66 6f72  rder": input_for
+00010cc0: 6d5b 226f 7264 6572 225d 2c0a 2020 2020  m["order"],.    
+00010cd0: 2020 2020 2020 2020 2264 6174 6122 3a20          "data": 
+00010ce0: 6461 7461 5f70 6f69 6e74 5b22 6375 7374  data_point["cust
+00010cf0: 6f6d 4669 656c 6431 225d 2069 6620 6461  omField1"] if da
+00010d00: 7461 5f70 6f69 6e74 2065 6c73 6520 4e6f  ta_point else No
+00010d10: 6e65 2c0a 2020 2020 2020 2020 7d0a 0a20  ne,.        }.. 
+00010d20: 2020 2061 7379 6e63 2064 6566 2067 6574     async def get
+00010d30: 5f69 6e70 7574 5f66 6f72 6d73 2873 656c  _input_forms(sel
+00010d40: 6629 202d 3e20 6c69 7374 5b64 6963 745d  f) -> list[dict]
+00010d50: 3a0a 2020 2020 2020 2020 2222 2247 6574  :.        """Get
+00010d60: 2061 6c6c 2074 6865 2069 6e70 7574 2066   all the input f
+00010d70: 6f72 6d73 2069 6e20 7468 6520 6375 7272  orms in the curr
+00010d80: 656e 7420 6d65 6e75 5f70 6174 682e 2222  ent menu_path.""
+00010d90: 220a 2020 2020 2020 2020 7265 706f 7274  ".        report
+00010da0: 733a 206c 6973 7420 3d20 5b0a 2020 2020  s: list = [.    
+00010db0: 2020 2020 2020 2020 7265 706f 7274 0a20          report. 
+00010dc0: 2020 2020 2020 2020 2020 2066 6f72 2072             for r
+00010dd0: 6570 6f72 7420 696e 2061 7761 6974 2073  eport in await s
+00010de0: 656c 662e 5f61 7070 2e67 6574 5f72 6570  elf._app.get_rep
+00010df0: 6f72 7473 2829 0a20 2020 2020 2020 2020  orts().         
+00010e00: 2020 2069 6620 7265 706f 7274 5b22 7265     if report["re
+00010e10: 706f 7274 5479 7065 225d 203d 3d20 2246  portType"] == "F
+00010e20: 4f52 4d22 0a20 2020 2020 2020 2020 2020  ORM".           
+00010e30: 2061 6e64 2028 7265 706f 7274 5b22 7061   and (report["pa
+00010e40: 7468 225d 203d 3d20 7365 6c66 2e5f 6375  th"] == self._cu
+00010e50: 7272 656e 745f 7061 7468 206f 7220 6e6f  rrent_path or no
+00010e60: 7420 7365 6c66 2e5f 6375 7272 656e 745f  t self._current_
+00010e70: 7061 7468 290a 2020 2020 2020 2020 5d0a  path).        ].
+00010e80: 2020 2020 2020 2020 7265 7475 726e 206c          return l
+00010e90: 6973 7428 0a20 2020 2020 2020 2020 2020  ist(.           
+00010ea0: 2061 7761 6974 2061 7379 6e63 696f 2e67   await asyncio.g
+00010eb0: 6174 6865 7228 0a20 2020 2020 2020 2020  ather(.         
+00010ec0: 2020 2020 2020 202a 5b73 656c 662e 5f67         *[self._g
+00010ed0: 6574 5f69 6e70 7574 5f66 6f72 6d5f 6461  et_input_form_da
+00010ee0: 7461 2872 6570 6f72 7429 2066 6f72 2072  ta(report) for r
+00010ef0: 6570 6f72 7420 696e 2072 6570 6f72 7473  eport in reports
+00010f00: 5d0a 2020 2020 2020 2020 2020 2020 290a  ].            ).
+00010f10: 2020 2020 2020 2020 290a 0a20 2020 2040          )..    @
+00010f20: 6164 645f 746f 5f67 656e 6572 616c 5f61  add_to_general_a
+00010f30: 7379 6e63 5f67 726f 7570 0a20 2020 2061  sync_group.    a
+00010f40: 7379 6e63 2064 6566 2061 6e6e 6f74 6174  sync def annotat
+00010f50: 6564 5f63 6861 7274 280a 2020 2020 2020  ed_chart(.      
+00010f60: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
+00010f70: 6461 7461 3a20 556e 696f 6e5b 6c69 7374  data: Union[list
+00010f80: 5b44 6174 6146 7261 6d65 5d2c 206c 6973  [DataFrame], lis
+00010f90: 745b 6c69 7374 5b64 6963 745d 5d5d 2c0a  t[list[dict]]],.
+00010fa0: 2020 2020 2020 2020 6f72 6465 723a 2069          order: i
+00010fb0: 6e74 2c0a 2020 2020 2020 2020 783a 2073  nt,.        x: s
+00010fc0: 7472 2c0a 2020 2020 2020 2020 793a 2055  tr,.        y: U
+00010fd0: 6e69 6f6e 5b73 7472 2c20 6c69 7374 5b73  nion[str, list[s
+00010fe0: 7472 5d5d 2c0a 2020 2020 2020 2020 616e  tr]],.        an
+00010ff0: 6e6f 7461 7469 6f6e 733a 2073 7472 203d  notations: str =
+00011000: 2022 616e 6e6f 7461 7469 6f6e 222c 0a20   "annotation",. 
+00011010: 2020 2020 2020 2072 6f77 735f 7369 7a65         rows_size
+00011020: 3a20 4f70 7469 6f6e 616c 5b69 6e74 5d20  : Optional[int] 
+00011030: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+00011040: 636f 6c73 5f73 697a 653a 204f 7074 696f  cols_size: Optio
+00011050: 6e61 6c5b 696e 745d 203d 204e 6f6e 652c  nal[int] = None,
+00011060: 0a20 2020 2020 2020 2070 6164 6469 6e67  .        padding
+00011070: 3a20 4f70 7469 6f6e 616c 5b73 7472 5d20  : Optional[str] 
+00011080: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+00011090: 7469 746c 653a 204f 7074 696f 6e61 6c5b  title: Optional[
+000110a0: 7374 725d 203d 204e 6f6e 652c 0a20 2020  str] = None,.   
+000110b0: 2020 2020 2079 5f61 7869 735f 6e61 6d65       y_axis_name
+000110c0: 3a20 4f70 7469 6f6e 616c 5b73 7472 5d20  : Optional[str] 
+000110d0: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+000110e0: 736c 6964 6572 5f63 6f6e 6669 673a 204f  slider_config: O
+000110f0: 7074 696f 6e61 6c5b 6469 6374 5d20 3d20  ptional[dict] = 
+00011100: 4e6f 6e65 2c0a 2020 2020 2020 2020 736c  None,.        sl
+00011110: 6964 6572 5f6d 6172 6b73 3a20 4f70 7469  ider_marks: Opti
+00011120: 6f6e 616c 5b6c 6973 745b 7475 706c 655d  onal[list[tuple]
+00011130: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 293a  ] = None,.    ):
+00011140: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00011150: 2020 2020 2043 7265 6174 6520 616e 2061       Create an a
+00011160: 6e6e 6f74 6174 6564 2063 6861 7274 2069  nnotated chart i
+00011170: 6e20 7468 6520 6d65 6e75 2070 6174 682e  n the menu path.
+00011180: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+00011190: 6461 7461 3a20 7468 6520 6461 7461 206f  data: the data o
+000111a0: 6620 7468 6520 6368 6172 740a 2020 2020  f the chart.    
+000111b0: 2020 2020 3a70 6172 616d 206f 7264 6572      :param order
+000111c0: 3a20 7468 6520 6f72 6465 7220 6f66 2074  : the order of t
+000111d0: 6865 2063 6861 7274 0a20 2020 2020 2020  he chart.       
+000111e0: 203a 7061 7261 6d20 783a 2074 6865 2078   :param x: the x
+000111f0: 2061 7869 730a 2020 2020 2020 2020 3a70   axis.        :p
+00011200: 6172 616d 2079 3a20 7468 6520 7920 6178  aram y: the y ax
+00011210: 6973 0a20 2020 2020 2020 203a 7061 7261  is.        :para
+00011220: 6d20 616e 6e6f 7461 7469 6f6e 733a 2074  m annotations: t
+00011230: 6865 2061 6e6e 6f74 6174 696f 6e73 0a20  he annotations. 
+00011240: 2020 2020 2020 203a 7061 7261 6d20 726f         :param ro
+00011250: 7773 5f73 697a 653a 2074 6865 2072 6f77  ws_size: the row
+00011260: 7320 7369 7a65 206f 6620 7468 6520 6368  s size of the ch
+00011270: 6172 740a 2020 2020 2020 2020 3a70 6172  art.        :par
+00011280: 616d 2063 6f6c 735f 7369 7a65 3a20 7468  am cols_size: th
+00011290: 6520 636f 6c75 6d6e 7320 7369 7a65 206f  e columns size o
+000112a0: 6620 7468 6520 6368 6172 740a 2020 2020  f the chart.    
+000112b0: 2020 2020 3a70 6172 616d 2070 6164 6469      :param paddi
+000112c0: 6e67 3a20 7468 6520 7061 6464 696e 6720  ng: the padding 
+000112d0: 6f66 2074 6865 2063 6861 7274 0a20 2020  of the chart.   
+000112e0: 2020 2020 203a 7061 7261 6d20 7469 746c       :param titl
+000112f0: 653a 2074 6865 2074 6974 6c65 206f 6620  e: the title of 
+00011300: 7468 6520 6368 6172 740a 2020 2020 2020  the chart.      
+00011310: 2020 3a70 6172 616d 2079 5f61 7869 735f    :param y_axis_
+00011320: 6e61 6d65 3a20 7468 6520 6e61 6d65 206f  name: the name o
+00011330: 6620 7468 6520 7920 6178 6973 0a20 2020  f the y axis.   
+00011340: 2020 2020 203a 7061 7261 6d20 736c 6964       :param slid
+00011350: 6572 5f63 6f6e 6669 673a 2074 6865 2073  er_config: the s
+00011360: 6c69 6465 7220 636f 6e66 6967 0a20 2020  lider config.   
+00011370: 2020 2020 203a 7061 7261 6d20 736c 6964       :param slid
+00011380: 6572 5f6d 6172 6b73 3a20 7468 6520 736c  er_marks: the sl
+00011390: 6964 6572 206d 6172 6b73 0a20 2020 2020  ider marks.     
+000113a0: 2020 2022 2222 0a20 2020 2020 2020 2069     """.        i
+000113b0: 6620 6973 696e 7374 616e 6365 2864 6174  f isinstance(dat
+000113c0: 612c 2073 7472 293a 0a20 2020 2020 2020  a, str):.       
+000113d0: 2020 2020 206c 6f67 5f65 7272 6f72 280a       log_error(.
+000113e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000113f0: 6c6f 6767 6572 2c0a 2020 2020 2020 2020  logger,.        
+00011400: 2020 2020 2020 2020 2241 6e6e 6f74 6174          "Annotat
+00011410: 6564 2063 6861 7274 2064 6f65 7320 6e6f  ed chart does no
+00011420: 7420 7375 7070 6f72 7420 7468 6520 7573  t support the us
+00011430: 6520 6f66 2073 6861 7265 6420 6461 7461  e of shared data
+00011440: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00011450: 2020 2044 6174 6145 7272 6f72 2c0a 2020     DataError,.  
+00011460: 2020 2020 2020 2020 2020 290a 0a20 2020            )..   
+00011470: 2020 2020 2069 6620 736c 6964 6572 5f63       if slider_c
+00011480: 6f6e 6669 6720 6973 204e 6f6e 653a 0a20  onfig is None:. 
+00011490: 2020 2020 2020 2020 2020 2073 6c69 6465             slide
+000114a0: 725f 636f 6e66 6967 203d 207b 7d0a 0a20  r_config = {}.. 
+000114b0: 2020 2020 2020 2069 6620 736c 6964 6572         if slider
+000114c0: 5f6d 6172 6b73 3a0a 2020 2020 2020 2020  _marks:.        
+000114d0: 2020 2020 736c 6964 6572 5f63 6f6e 6669      slider_confi
+000114e0: 675b 226d 6172 6b73 225d 203d 205b 0a20  g["marks"] = [. 
+000114f0: 2020 2020 2020 2020 2020 2020 2020 207b                 {
+00011500: 226c 6162 656c 223a 206d 6172 6b5b 305d  "label": mark[0]
+00011510: 2c20 2276 616c 7565 223a 206d 6172 6b5b  , "value": mark[
+00011520: 315d 7d20 666f 7220 6d61 726b 2069 6e20  1]} for mark in 
+00011530: 736c 6964 6572 5f6d 6172 6b73 0a20 2020  slider_marks.   
+00011540: 2020 2020 2020 2020 205d 0a0a 2020 2020           ]..    
+00011550: 2020 2020 6966 2069 7369 6e73 7461 6e63      if isinstanc
+00011560: 6528 792c 2073 7472 293a 0a20 2020 2020  e(y, str):.     
+00011570: 2020 2020 2020 2079 203d 205b 795d 0a0a         y = [y]..
+00011580: 2020 2020 2020 2020 6966 206e 6f74 206c          if not l
+00011590: 656e 2879 2920 3d3d 206c 656e 2864 6174  en(y) == len(dat
+000115a0: 6129 3a0a 2020 2020 2020 2020 2020 2020  a):.            
+000115b0: 6c6f 675f 6572 726f 7228 0a20 2020 2020  log_error(.     
+000115c0: 2020 2020 2020 2020 2020 206c 6f67 6765             logge
+000115d0: 722c 0a20 2020 2020 2020 2020 2020 2020  r,.             
+000115e0: 2020 2066 224e 756d 6265 7220 6f66 2079     f"Number of y
+000115f0: 2076 616c 7565 7320 287b 6c65 6e28 7929   values ({len(y)
+00011600: 7d29 2064 6f65 7320 6e6f 7420 6d61 7463  }) does not matc
+00011610: 6820 6e75 6d62 6572 206f 6620 6461 7461  h number of data
+00011620: 6672 616d 6573 2028 7b6c 656e 2864 6174  frames ({len(dat
+00011630: 6129 7d29 222c 0a20 2020 2020 2020 2020  a)})",.         
+00011640: 2020 2020 2020 2044 6174 6145 7272 6f72         DataError
+00011650: 2c0a 2020 2020 2020 2020 2020 2020 290a  ,.            ).
+00011660: 0a20 2020 2020 2020 205f 2c20 7265 706f  .        _, repo
+00011670: 7274 203d 2061 7761 6974 2073 656c 662e  rt = await self.
+00011680: 5f67 6574 5f63 6861 7274 5f72 6570 6f72  _get_chart_repor
+00011690: 7428 6f72 6465 722c 2041 6e6e 6f74 6174  t(order, Annotat
+000116a0: 6564 4543 6861 7274 290a 0a20 2020 2020  edEChart)..     
+000116b0: 2020 2064 6673 203d 205b 7661 6c69 6461     dfs = [valida
+000116c0: 7465 5f64 6174 615f 6973 5f70 616e 6461  te_data_is_panda
+000116d0: 7261 626c 6528 6466 2920 666f 7220 6466  rable(df) for df
+000116e0: 2069 6e20 6461 7461 5d0a 2020 2020 2020   in data].      
+000116f0: 2020 6461 7461 5f73 6574 5f74 6173 6b73    data_set_tasks
+00011700: 203d 205b 5d0a 2020 2020 2020 2020 666f   = [].        fo
+00011710: 7220 6466 2c20 795f 7661 6c20 696e 207a  r df, y_val in z
+00011720: 6970 2864 6673 2c20 7929 3a0a 2020 2020  ip(dfs, y):.    
+00011730: 2020 2020 2020 2020 6466 5b78 5d20 3d20          df[x] = 
+00011740: 7064 2e74 6f5f 6461 7465 7469 6d65 2864  pd.to_datetime(d
+00011750: 665b 785d 290a 2020 2020 2020 2020 2020  f[x]).          
+00011760: 2020 6966 2061 6e6e 6f74 6174 696f 6e73    if annotations
+00011770: 2069 6e20 6466 3a0a 2020 2020 2020 2020   in df:.        
+00011780: 2020 2020 2020 2020 6466 5b61 6e6e 6f74          df[annot
+00011790: 6174 696f 6e73 5d20 3d20 280a 2020 2020  ations] = (.    
+000117a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000117b0: 6466 5b61 6e6e 6f74 6174 696f 6e73 5d2e  df[annotations].
+000117c0: 7265 706c 6163 6528 6e70 2e6e 616e 2c20  replace(np.nan, 
+000117d0: 2222 2c20 7265 6765 783d 5472 7565 292e  "", regex=True).
+000117e0: 6173 7479 7065 2873 7472 290a 2020 2020  astype(str).    
+000117f0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+00011800: 2020 2020 2020 2020 2020 6461 7461 5f73            data_s
+00011810: 6574 5f74 6173 6b73 2e61 7070 656e 6428  et_tasks.append(
+00011820: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011830: 2073 656c 662e 5f63 7265 6174 655f 6461   self._create_da
+00011840: 7461 5f73 6574 286e 616d 653d 6622 7b72  ta_set(name=f"{r
+00011850: 6570 6f72 745b 2769 6427 5d7d 5f7b 795f  eport['id']}_{y_
+00011860: 7661 6c7d 222c 2064 6174 613d 6466 290a  val}", data=df).
+00011870: 2020 2020 2020 2020 2020 2020 290a 0a20              ).. 
+00011880: 2020 2020 2020 2064 6174 615f 7365 745f         data_set_
+00011890: 6469 6374 7320 3d20 6177 6169 7420 6173  dicts = await as
+000118a0: 796e 6369 6f2e 6761 7468 6572 282a 6461  yncio.gather(*da
+000118b0: 7461 5f73 6574 5f74 6173 6b73 290a 2020  ta_set_tasks).  
+000118c0: 2020 2020 2020 6461 7461 5f73 6574 7320        data_sets 
+000118d0: 3d20 5b64 735b 795f 7661 6c5d 5b31 5d20  = [ds[y_val][1] 
+000118e0: 666f 7220 6473 2c20 795f 7661 6c20 696e  for ds, y_val in
+000118f0: 207a 6970 2864 6174 615f 7365 745f 6469   zip(data_set_di
+00011900: 6374 732c 2079 295d 0a0a 2020 2020 2020  cts, y)]..      
+00011910: 2020 7264 5f69 6473 203d 204e 6f6e 650a    rd_ids = None.
+00011920: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00011930: 7265 7573 655f 6461 7461 5f73 6574 733a  reuse_data_sets:
+00011940: 0a20 2020 2020 2020 2020 2020 2072 645f  .            rd_
+00011950: 6964 7320 3d20 6765 745f 7575 6964 735f  ids = get_uuids_
+00011960: 6672 6f6d 5f64 6963 7428 7265 706f 7274  from_dict(report
+00011970: 5b22 7072 6f70 6572 7469 6573 225d 5b22  ["properties"]["
+00011980: 6f70 7469 6f6e 225d 290a 2020 2020 2020  option"]).      
+00011990: 2020 2020 2020 6966 206c 656e 2872 645f        if len(rd_
+000119a0: 6964 7329 203d 3d20 6c65 6e28 7929 3a0a  ids) == len(y):.
+000119b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000119c0: 7265 705f 6473 3a20 6c69 7374 5b52 6570  rep_ds: list[Rep
+000119d0: 6f72 742e 5265 706f 7274 4461 7461 5365  ort.ReportDataSe
+000119e0: 745d 203d 2061 7761 6974 2072 6570 6f72  t] = await repor
+000119f0: 742e 6765 745f 7265 706f 7274 5f64 6174  t.get_report_dat
+00011a00: 615f 7365 7473 2829 0a20 2020 2020 2020  a_sets().       
+00011a10: 2020 2020 2020 2020 2072 6570 5f64 7320           rep_ds 
+00011a20: 3d20 5b0a 2020 2020 2020 2020 2020 2020  = [.            
+00011a30: 2020 2020 2020 2020 6e65 7874 2828 7264          next((rd
+00011a40: 2066 6f72 2072 6420 696e 2072 6570 5f64   for rd in rep_d
+00011a50: 7320 6966 2072 645b 2269 6422 5d20 3d3d  s if rd["id"] ==
+00011a60: 2072 645f 6964 292c 204e 6f6e 6529 0a20   rd_id), None). 
+00011a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011a80: 2020 2066 6f72 2072 645f 6964 2069 6e20     for rd_id in 
+00011a90: 7264 5f69 6473 0a20 2020 2020 2020 2020  rd_ids.         
+00011aa0: 2020 2020 2020 205d 0a20 2020 2020 2020         ].       
+00011ab0: 2020 2020 2020 2020 2069 6620 616e 7928           if any(
+00011ac0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011ad0: 2020 2020 2072 645b 2264 6174 6153 6574       rd["dataSet
+00011ae0: 4964 225d 2021 3d20 6473 5b22 6964 225d  Id"] != ds["id"]
+00011af0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011b00: 2020 2020 206f 7220 7264 5b22 7072 6f70       or rd["prop
+00011b10: 6572 7469 6573 225d 5b22 6d61 7070 696e  erties"]["mappin
+00011b20: 6722 5d0a 2020 2020 2020 2020 2020 2020  g"].            
+00011b30: 2020 2020 2020 2020 213d 207b 2276 616c          != {"val
+00011b40: 7565 7322 3a20 5b22 6461 7465 4669 656c  ues": ["dateFiel
+00011b50: 6431 222c 2022 696e 7446 6965 6c64 3122  d1", "intField1"
+00011b60: 5d2c 2022 6c61 6265 6c22 3a20 2273 7472  ], "label": "str
+00011b70: 696e 6746 6965 6c64 3122 7d0a 2020 2020  ingField1"}.    
+00011b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011b90: 666f 7220 7264 2c20 6473 2069 6e20 7a69  for rd, ds in zi
+00011ba0: 7028 7265 705f 6473 2c20 6461 7461 5f73  p(rep_ds, data_s
+00011bb0: 6574 7329 0a20 2020 2020 2020 2020 2020  ets).           
+00011bc0: 2020 2020 2029 3a0a 2020 2020 2020 2020       ):.        
+00011bd0: 2020 2020 2020 2020 2020 2020 7264 5f69              rd_i
+00011be0: 6473 203d 204e 6f6e 650a 0a20 2020 2020  ds = None..     
+00011bf0: 2020 2069 6620 6e6f 7420 7264 5f69 6473     if not rd_ids
+00011c00: 3a0a 2020 2020 2020 2020 2020 2020 6177  :.            aw
+00011c10: 6169 7420 7265 706f 7274 2e64 656c 6574  ait report.delet
+00011c20: 655f 7265 706f 7274 5f64 6174 615f 7365  e_report_data_se
+00011c30: 7473 286c 6f67 3d54 7275 6529 0a20 2020  ts(log=True).   
+00011c40: 2020 2020 2020 2020 206d 6170 7069 6e67           mapping
+00011c50: 3a20 4d61 7070 696e 6720 3d20 7b0a 2020  : Mapping = {.  
+00011c60: 2020 2020 2020 2020 2020 2020 2020 2276                "v
+00011c70: 616c 7565 7322 3a20 5b22 6461 7465 4669  alues": ["dateFi
+00011c80: 656c 6431 222c 2022 696e 7446 6965 6c64  eld1", "intField
+00011c90: 3122 5d2c 0a20 2020 2020 2020 2020 2020  1"],.           
+00011ca0: 2020 2020 2022 6c61 6265 6c22 3a20 2273       "label": "s
+00011cb0: 7472 696e 6746 6965 6c64 3122 2c0a 2020  tringField1",.  
+00011cc0: 2020 2020 2020 2020 2020 7d0a 2020 2020            }.    
+00011cd0: 2020 2020 2020 2020 7265 706f 7274 5f64          report_d
+00011ce0: 6174 615f 7365 7473 203d 2061 7761 6974  ata_sets = await
+00011cf0: 2061 7379 6e63 696f 2e67 6174 6865 7228   asyncio.gather(
+00011d00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011d10: 202a 5b0a 2020 2020 2020 2020 2020 2020   *[.            
+00011d20: 2020 2020 2020 2020 7265 706f 7274 2e63          report.c
+00011d30: 7265 6174 655f 7265 706f 7274 5f64 6174  reate_report_dat
+00011d40: 615f 7365 7428 286d 6170 7069 6e67 2c20  a_set((mapping, 
+00011d50: 6461 7461 5f73 6574 2c20 4e6f 6e65 2929  data_set, None))
+00011d60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011d70: 2020 2020 2066 6f72 2064 6174 615f 7365       for data_se
+00011d80: 7420 696e 2064 6174 615f 7365 7473 0a20  t in data_sets. 
+00011d90: 2020 2020 2020 2020 2020 2020 2020 205d                 ]
+00011da0: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
+00011db0: 2020 2020 2020 2020 2020 2072 645f 6964             rd_id
+00011dc0: 7320 3d20 5b72 645b 2269 6422 5d20 666f  s = [rd["id"] fo
+00011dd0: 7220 7264 2069 6e20 7265 706f 7274 5f64  r rd in report_d
+00011de0: 6174 615f 7365 7473 5d0a 0a20 2020 2020  ata_sets]..     
+00011df0: 2020 2063 6861 7274 5f6f 7074 696f 6e73     chart_options
+00011e00: 203d 207b 0a20 2020 2020 2020 2020 2020   = {.           
+00011e10: 2022 7941 7869 7322 3a20 7b0a 2020 2020   "yAxis": {.    
+00011e20: 2020 2020 2020 2020 2020 2020 226e 616d              "nam
+00011e30: 6522 3a20 795f 6178 6973 5f6e 616d 6520  e": y_axis_name 
+00011e40: 6f72 2022 222c 0a20 2020 2020 2020 2020  or "",.         
+00011e50: 2020 2020 2020 2022 666f 6e74 2220 2274         "font" "t
+00011e60: 7970 6522 3a20 2276 616c 7565 222c 0a20  ype": "value",. 
+00011e70: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00011e80: 6e61 6d65 4c6f 6361 7469 6f6e 223a 2022  nameLocation": "
+00011e90: 6d69 6464 6c65 222c 0a20 2020 2020 2020  middle",.       
+00011ea0: 2020 2020 2020 2020 2022 6e61 6d65 4761           "nameGa
+00011eb0: 7022 3a20 3330 2c0a 2020 2020 2020 2020  p": 30,.        
+00011ec0: 2020 2020 7d2c 0a20 2020 2020 2020 2020      },.         
+00011ed0: 2020 2022 7841 7869 7322 3a20 7b0a 2020     "xAxis": {.  
+00011ee0: 2020 2020 2020 2020 2020 2020 2020 2274                "t
+00011ef0: 7970 6522 3a20 2274 696d 6522 2c0a 2020  ype": "time",.  
+00011f00: 2020 2020 2020 2020 2020 2020 2020 226e                "n
+00011f10: 616d 654c 6f63 6174 696f 6e22 3a20 226d  ameLocation": "m
+00011f20: 6964 646c 6522 2c0a 2020 2020 2020 2020  iddle",.        
+00011f30: 2020 2020 2020 2020 226e 616d 6547 6170          "nameGap
+00011f40: 223a 2033 302c 0a20 2020 2020 2020 2020  ": 30,.         
+00011f50: 2020 207d 2c0a 2020 2020 2020 2020 2020     },.          
+00011f60: 2020 2273 6572 6965 7322 3a20 5b0a 2020    "series": [.  
+00011f70: 2020 2020 2020 2020 2020 2020 2020 7b0a                {.
+00011f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011f90: 2020 2020 2264 6174 6122 3a20 2223 7b22      "data": "#{"
+00011fa0: 202b 2072 645f 6964 202b 2022 7d22 2c0a   + rd_id + "}",.
+00011fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011fc0: 2020 2020 2274 7970 6522 3a20 226c 696e      "type": "lin
+00011fd0: 6522 2c0a 2020 2020 2020 2020 2020 2020  e",.            
+00011fe0: 2020 2020 2020 2020 226e 616d 6522 3a20          "name": 
+00011ff0: 795f 6e61 6d65 2c0a 2020 2020 2020 2020  y_name,.        
+00012000: 2020 2020 2020 2020 2020 2020 2269 7465              "ite
+00012010: 6d53 7479 6c65 223a 207b 0a20 2020 2020  mStyle": {.     
+00012020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012030: 2020 2022 626f 7264 6572 5261 6469 7573     "borderRadius
+00012040: 223a 205b 392c 2039 2c20 302c 2030 5d2c  ": [9, 9, 0, 0],
+00012050: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012060: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
+00012070: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
+00012080: 2020 2020 2020 2020 2020 666f 7220 795f            for y_
+00012090: 6e61 6d65 2c20 7264 5f69 6420 696e 207a  name, rd_id in z
+000120a0: 6970 2879 2c20 7264 5f69 6473 290a 2020  ip(y, rd_ids).  
+000120b0: 2020 2020 2020 2020 2020 5d2c 0a20 2020            ],.   
+000120c0: 2020 2020 207d 0a20 2020 2020 2020 2061       }.        a
+000120d0: 7761 6974 2073 656c 662e 5f63 7265 6174  wait self._creat
+000120e0: 655f 6368 6172 7428 0a20 2020 2020 2020  e_chart(.       
+000120f0: 2020 2020 2063 6861 7274 5f63 6c61 7373       chart_class
+00012100: 3d41 6e6e 6f74 6174 6564 4543 6861 7274  =AnnotatedEChart
+00012110: 2c0a 2020 2020 2020 2020 2020 2020 6f72  ,.            or
+00012120: 6465 723d 6f72 6465 722c 0a20 2020 2020  der=order,.     
+00012130: 2020 2020 2020 2073 697a 6550 6164 6469         sizePaddi
+00012140: 6e67 3d70 6164 6469 6e67 2c0a 2020 2020  ng=padding,.    
+00012150: 2020 2020 2020 2020 7369 7a65 526f 7773          sizeRows
+00012160: 3d72 6f77 735f 7369 7a65 2c0a 2020 2020  =rows_size,.    
+00012170: 2020 2020 2020 2020 7369 7a65 436f 6c75          sizeColu
+00012180: 6d6e 733d 636f 6c73 5f73 697a 652c 0a20  mns=cols_size,. 
+00012190: 2020 2020 2020 2020 2020 2074 6974 6c65             title
+000121a0: 3d74 6974 6c65 2c0a 2020 2020 2020 2020  =title,.        
+000121b0: 2020 2020 7072 6f70 6572 7469 6573 3d64      properties=d
+000121c0: 6963 7428 0a20 2020 2020 2020 2020 2020  ict(.           
+000121d0: 2020 2020 2073 6c69 6465 723d 736c 6964       slider=slid
+000121e0: 6572 5f63 6f6e 6669 672c 0a20 2020 2020  er_config,.     
+000121f0: 2020 2020 2020 2020 2020 206f 7074 696f             optio
+00012200: 6e3d 6368 6172 745f 6f70 7469 6f6e 732c  n=chart_options,
+00012210: 0a20 2020 2020 2020 2020 2020 2029 2c0a  .            ),.
+00012220: 2020 2020 2020 2020 290a 0a20 2020 2061          )..    a
+00012230: 7379 6e63 2064 6566 205f 6765 745f 7265  sync def _get_re
+00012240: 706f 7274 5f64 6174 615f 7365 7473 5f70  port_data_sets_p
+00012250: 6572 5f6d 6170 7069 6e67 280a 2020 2020  er_mapping(.    
+00012260: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
+00012270: 2020 7265 706f 7274 3a20 5265 706f 7274    report: Report
+00012280: 2c0a 2020 2020 2020 2020 6461 7461 5f6d  ,.        data_m
+00012290: 6170 7069 6e67 5f74 6f5f 7475 706c 653a  apping_to_tuple:
+000122a0: 2064 6963 742c 0a20 2020 2020 2020 2066   dict,.        f
+000122b0: 6965 6c64 733a 206c 6973 745b 556e 696f  ields: list[Unio
+000122c0: 6e5b 7475 706c 652c 2064 6963 745d 5d2c  n[tuple, dict]],
+000122d0: 0a20 2020 2029 202d 3e20 6c69 7374 5b52  .    ) -> list[R
+000122e0: 6570 6f72 742e 5265 706f 7274 4461 7461  eport.ReportData
+000122f0: 5365 745d 3a0a 2020 2020 2020 2020 2222  Set]:.        ""
+00012300: 2243 7265 6174 6520 6120 6461 7461 5f73  "Create a data_s
+00012310: 6574 2070 6572 2066 6965 6c64 206f 6620  et per field of 
+00012320: 6120 6461 7461 6672 616d 652e 0a20 2020  a dataframe..   
+00012330: 2020 2020 203a 7061 7261 6d20 7265 706f       :param repo
+00012340: 7274 3a20 7468 6520 7265 706f 7274 0a20  rt: the report. 
+00012350: 2020 2020 2020 203a 7061 7261 6d20 6461         :param da
+00012360: 7461 5f6d 6170 7069 6e67 5f74 6f5f 7475  ta_mapping_to_tu
+00012370: 706c 653a 2074 6865 206d 6170 7069 6e67  ple: the mapping
+00012380: 206f 6620 7468 6520 6461 7461 0a20 2020   of the data.   
+00012390: 2020 2020 203a 7061 7261 6d20 6669 656c       :param fiel
+000123a0: 6473 3a20 7468 6520 6669 656c 6473 206f  ds: the fields o
+000123b0: 6620 7468 6520 6461 7461 2074 6f20 6265  f the data to be
+000123c0: 2075 7365 640a 2020 2020 2020 2020 3a72   used.        :r
+000123d0: 6574 7572 6e3a 2074 6865 206c 6973 7420  eturn: the list 
+000123e0: 6f66 2064 6174 6120 7365 7473 2070 6172  of data sets par
+000123f0: 7469 7469 6f6e 6564 2062 7920 6178 6973  titioned by axis
+00012400: 2061 6e64 2066 6965 6c64 730a 2020 2020   and fields.    
+00012410: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00012420: 7461 736b 7320 3d20 5b5d 0a20 2020 2020  tasks = [].     
+00012430: 2020 2066 6965 6c64 7320 3d20 6669 656c     fields = fiel
+00012440: 6473 2069 6620 6669 656c 6473 2065 6c73  ds if fields els
+00012450: 6520 5b5d 0a20 2020 2020 2020 2066 6f72  e [].        for
+00012460: 2069 2c20 6620 696e 2065 6e75 6d65 7261   i, f in enumera
+00012470: 7465 2866 6965 6c64 7329 3a0a 2020 2020  te(fields):.    
+00012480: 2020 2020 2020 2020 6d61 7070 696e 6720          mapping 
+00012490: 3d20 5b5d 0a20 2020 2020 2020 2020 2020  = [].           
+000124a0: 2064 6174 615f 7365 7420 3d20 4e6f 6e65   data_set = None
+000124b0: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+000124c0: 5f73 6f72 7420 3d20 4e6f 6e65 0a20 2020  _sort = None.   
+000124d0: 2020 2020 2020 2020 2069 6620 6973 696e           if isin
+000124e0: 7374 616e 6365 2866 2c20 7374 7229 3a0a  stance(f, str):.
+000124f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012500: 6966 2066 206e 6f74 2069 6e20 6461 7461  if f not in data
+00012510: 5f6d 6170 7069 6e67 5f74 6f5f 7475 706c  _mapping_to_tupl
+00012520: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+00012530: 2020 2020 2020 206c 6f67 5f65 7272 6f72         log_error
+00012540: 286c 6f67 6765 722c 2066 2246 6965 6c64  (logger, f"Field
+00012550: 207b 667d 206e 6f74 2066 6f75 6e64 2069   {f} not found i
+00012560: 6e20 6461 7461 222c 2044 6174 6145 7272  n data", DataErr
+00012570: 6f72 290a 2020 2020 2020 2020 2020 2020  or).            
+00012580: 2020 2020 6d61 7070 696e 672c 2064 6174      mapping, dat
+00012590: 615f 7365 742c 2072 6573 5f73 6f72 7420  a_set, res_sort 
+000125a0: 3d20 6461 7461 5f6d 6170 7069 6e67 5f74  = data_mapping_t
+000125b0: 6f5f 7475 706c 655b 665d 0a20 2020 2020  o_tuple[f].     
+000125c0: 2020 2020 2020 2065 6c69 6620 6973 696e         elif isin
+000125d0: 7374 616e 6365 2866 2c20 2874 7570 6c65  stance(f, (tuple
+000125e0: 2c20 6c69 7374 2929 3a0a 2020 2020 2020  , list)):.      
+000125f0: 2020 2020 2020 2020 2020 666f 7220 665f            for f_
+00012600: 2069 6e20 663a 0a20 2020 2020 2020 2020   in f:.         
+00012610: 2020 2020 2020 2020 2020 2069 6620 665f             if f_
+00012620: 206e 6f74 2069 6e20 6461 7461 5f6d 6170   not in data_map
+00012630: 7069 6e67 5f74 6f5f 7475 706c 653a 0a20  ping_to_tuple:. 
+00012640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012650: 2020 2020 2020 206c 6f67 5f65 7272 6f72         log_error
+00012660: 286c 6f67 6765 722c 2066 2246 6965 6c64  (logger, f"Field
+00012670: 207b 665f 7d20 6e6f 7420 666f 756e 6420   {f_} not found 
+00012680: 696e 2064 6174 6122 2c20 4461 7461 4572  in data", DataEr
+00012690: 726f 7229 0a20 2020 2020 2020 2020 2020  ror).           
+000126a0: 2020 2020 2020 2020 206d 6170 7069 6e67           mapping
+000126b0: 5f2c 2064 6174 615f 7365 745f 2c20 7265  _, data_set_, re
+000126c0: 735f 736f 7274 5f20 3d20 6461 7461 5f6d  s_sort_ = data_m
+000126d0: 6170 7069 6e67 5f74 6f5f 7475 706c 655b  apping_to_tuple[
+000126e0: 665f 5d0a 2020 2020 2020 2020 2020 2020  f_].            
+000126f0: 2020 2020 2020 2020 6d61 7070 696e 672e          mapping.
+00012700: 6170 7065 6e64 286d 6170 7069 6e67 5f29  append(mapping_)
+00012710: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012720: 2020 2020 2064 6174 615f 7365 7420 3d20       data_set = 
+00012730: 6461 7461 5f73 6574 2069 6620 6461 7461  data_set if data
+00012740: 5f73 6574 2065 6c73 6520 6461 7461 5f73  _set else data_s
+00012750: 6574 5f0a 2020 2020 2020 2020 2020 2020  et_.            
+00012760: 2020 2020 2020 2020 7265 735f 736f 7274          res_sort
+00012770: 203d 2072 6573 5f73 6f72 7420 6966 2072   = res_sort if r
+00012780: 6573 5f73 6f72 7420 656c 7365 2072 6573  es_sort else res
+00012790: 5f73 6f72 745f 0a20 2020 2020 2020 2020  _sort_.         
+000127a0: 2020 2020 2020 2020 2020 2061 7373 6572             asser
+000127b0: 7420 6461 7461 5f73 6574 203d 3d20 6461  t data_set == da
+000127c0: 7461 5f73 6574 5f0a 2020 2020 2020 2020  ta_set_.        
+000127d0: 2020 2020 2020 2020 2020 2020 6173 7365              asse
+000127e0: 7274 2072 6573 5f73 6f72 7420 3d3d 2072  rt res_sort == r
+000127f0: 6573 5f73 6f72 745f 0a20 2020 2020 2020  es_sort_.       
+00012800: 2020 2020 2065 6c69 6620 6973 696e 7374       elif isinst
+00012810: 616e 6365 2866 2c20 6469 6374 293a 0a20  ance(f, dict):. 
+00012820: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+00012830: 6170 7069 6e67 203d 207b 6b3a 205b 5d20  apping = {k: [] 
+00012840: 666f 7220 6b20 696e 2066 2e6b 6579 7328  for k in f.keys(
+00012850: 297d 0a20 2020 2020 2020 2020 2020 2020  )}.             
+00012860: 2020 2066 6f72 206b 2c20 665f 2069 6e20     for k, f_ in 
+00012870: 662e 6974 656d 7328 293a 0a20 2020 2020  f.items():.     
+00012880: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00012890: 6620 665f 206e 6f74 2069 6e20 6461 7461  f f_ not in data
+000128a0: 5f6d 6170 7069 6e67 5f74 6f5f 7475 706c  _mapping_to_tupl
+000128b0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+000128c0: 2020 2020 2020 2020 2020 206c 6f67 5f65             log_e
+000128d0: 7272 6f72 286c 6f67 6765 722c 2066 2246  rror(logger, f"F
+000128e0: 6965 6c64 207b 665f 7d20 6e6f 7420 666f  ield {f_} not fo
+000128f0: 756e 6420 696e 2064 6174 6122 2c20 4461  und in data", Da
+00012900: 7461 4572 726f 7229 0a20 2020 2020 2020  taError).       
+00012910: 2020 2020 2020 2020 2020 2020 206d 6170               map
+00012920: 7069 6e67 5f2c 2064 6174 615f 7365 745f  ping_, data_set_
+00012930: 2c20 7265 735f 736f 7274 5f20 3d20 6461  , res_sort_ = da
+00012940: 7461 5f6d 6170 7069 6e67 5f74 6f5f 7475  ta_mapping_to_tu
+00012950: 706c 655b 665f 5d0a 2020 2020 2020 2020  ple[f_].        
+00012960: 2020 2020 2020 2020 2020 2020 6d61 7070              mapp
+00012970: 696e 675b 6b5d 203d 206d 6170 7069 6e67  ing[k] = mapping
+00012980: 5f0a 2020 2020 2020 2020 2020 2020 2020  _.              
+00012990: 2020 2020 2020 6461 7461 5f73 6574 203d        data_set =
+000129a0: 2064 6174 615f 7365 7420 6966 2064 6174   data_set if dat
+000129b0: 615f 7365 7420 656c 7365 2064 6174 615f  a_set else data_
+000129c0: 7365 745f 0a20 2020 2020 2020 2020 2020  set_.           
+000129d0: 2020 2020 2020 2020 2072 6573 5f73 6f72           res_sor
+000129e0: 7420 3d20 7265 735f 736f 7274 2069 6620  t = res_sort if 
+000129f0: 7265 735f 736f 7274 2065 6c73 6520 7265  res_sort else re
+00012a00: 735f 736f 7274 5f0a 2020 2020 2020 2020  s_sort_.        
+00012a10: 2020 2020 2020 2020 2020 2020 6173 7365              asse
+00012a20: 7274 2064 6174 615f 7365 7420 3d3d 2064  rt data_set == d
+00012a30: 6174 615f 7365 745f 0a20 2020 2020 2020  ata_set_.       
+00012a40: 2020 2020 2020 2020 2020 2020 2061 7373               ass
+00012a50: 6572 7420 7265 735f 736f 7274 203d 3d20  ert res_sort == 
+00012a60: 7265 735f 736f 7274 5f0a 2020 2020 2020  res_sort_.      
+00012a70: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+00012a80: 2020 2020 2020 2020 2020 2020 6c6f 675f              log_
+00012a90: 6572 726f 7228 0a20 2020 2020 2020 2020  error(.         
+00012aa0: 2020 2020 2020 2020 2020 206c 6f67 6765             logge
+00012ab0: 722c 2066 2246 6965 6c64 207b 667d 2069  r, f"Field {f} i
+00012ac0: 7320 6e6f 7420 6120 7374 7269 6e67 2c20  s not a string, 
+00012ad0: 7475 706c 652c 206c 6973 7420 6f72 2064  tuple, list or d
+00012ae0: 6963 7422 2c20 4461 7461 4572 726f 720a  ict", DataError.
+00012af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012b00: 290a 2020 2020 2020 2020 2020 2020 7461  ).            ta
+00012b10: 736b 732e 6170 7065 6e64 280a 2020 2020  sks.append(.    
+00012b20: 2020 2020 2020 2020 2020 2020 7265 706f              repo
+00012b30: 7274 2e63 7265 6174 655f 7265 706f 7274  rt.create_report
+00012b40: 5f64 6174 615f 7365 7428 0a20 2020 2020  _data_set(.     
+00012b50: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+00012b60: 6170 7069 6e67 5f64 6174 615f 7365 745f  apping_data_set_
+00012b70: 736f 7274 3d28 6d61 7070 696e 672c 2064  sort=(mapping, d
+00012b80: 6174 615f 7365 742c 2072 6573 5f73 6f72  ata_set, res_sor
+00012b90: 7429 0a20 2020 2020 2020 2020 2020 2020  t).             
+00012ba0: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+00012bb0: 2029 0a0a 2020 2020 2020 2020 7265 706f   )..        repo
+00012bc0: 7274 5f64 6174 615f 7365 7473 203d 2061  rt_data_sets = a
+00012bd0: 7761 6974 2061 7379 6e63 696f 2e67 6174  wait asyncio.gat
+00012be0: 6865 7228 2a74 6173 6b73 290a 2020 2020  her(*tasks).    
+00012bf0: 2020 2020 6c6f 6767 6572 2e69 6e66 6f28      logger.info(
+00012c00: 0a20 2020 2020 2020 2020 2020 2066 2243  .            f"C
+00012c10: 7265 6174 6564 207b 6c65 6e28 7265 706f  reated {len(repo
+00012c20: 7274 5f64 6174 615f 7365 7473 297d 2063  rt_data_sets)} c
+00012c30: 6f6d 706f 6e65 6e74 2064 6174 6120 7365  omponent data se
+00012c40: 7420 6c69 6e6b 7320 666f 7220 636f 6d70  t links for comp
+00012c50: 6f6e 656e 7420 7b73 7472 2872 6570 6f72  onent {str(repor
+00012c60: 7429 7d22 0a20 2020 2020 2020 2029 0a20  t)}".        ). 
+00012c70: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
+00012c80: 706f 7274 5f64 6174 615f 7365 7473 0a0a  port_data_sets..
+00012c90: 2020 2020 6465 6620 5f75 7064 6174 655f      def _update_
+00012ca0: 6f70 7469 6f6e 7328 7365 6c66 2c20 6f70  options(self, op
+00012cb0: 7469 6f6e 733a 2064 6963 742c 206f 7074  tions: dict, opt
+00012cc0: 696f 6e5f 6d6f 6469 6669 6361 7469 6f6e  ion_modification
+00012cd0: 733a 204f 7074 696f 6e61 6c5b 6469 6374  s: Optional[dict
+00012ce0: 5d29 3a0a 2020 2020 2020 2020 2222 2255  ]):.        """U
+00012cf0: 7064 6174 6520 7468 6520 6f70 7469 6f6e  pdate the option
+00012d00: 7320 6f66 2061 6e20 6563 6861 7274 2e0a  s of an echart..
+00012d10: 2020 2020 2020 2020 3a70 6172 616d 206f          :param o
+00012d20: 7074 696f 6e73 3a20 7468 6520 6f70 7469  ptions: the opti
+00012d30: 6f6e 7320 6f66 2074 6865 2065 6368 6172  ons of the echar
+00012d40: 740a 2020 2020 2020 2020 3a70 6172 616d  t.        :param
+00012d50: 206f 7074 696f 6e5f 6d6f 6469 6669 6361   option_modifica
+00012d60: 7469 6f6e 733a 2074 6865 206d 6f64 6966  tions: the modif
+00012d70: 6963 6174 696f 6e73 2074 6f20 6170 706c  ications to appl
+00012d80: 7920 746f 2074 6865 206f 7074 696f 6e73  y to the options
+00012d90: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00012da0: 2020 2020 2069 6620 6e6f 7420 6f70 7469       if not opti
+00012db0: 6f6e 5f6d 6f64 6966 6963 6174 696f 6e73  on_modifications
+00012dc0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00012dd0: 7475 726e 0a20 2020 2020 2020 2066 6f72  turn.        for
+00012de0: 206b 2c20 7620 696e 206f 7074 696f 6e5f   k, v in option_
+00012df0: 6d6f 6469 6669 6361 7469 6f6e 732e 6974  modifications.it
+00012e00: 656d 7328 293a 0a20 2020 2020 2020 2020  ems():.         
+00012e10: 2020 2069 6620 6b20 3d3d 2022 7365 7269     if k == "seri
+00012e20: 6573 223a 0a20 2020 2020 2020 2020 2020  es":.           
+00012e30: 2020 2020 206c 6f67 5f65 7272 6f72 286c       log_error(l
+00012e40: 6f67 6765 722c 2022 5365 7269 6573 2063  ogger, "Series c
+00012e50: 616e 6e6f 7420 6265 206d 6f64 6966 6965  annot be modifie
+00012e60: 6422 2c20 4461 7461 4572 726f 7229 0a20  d", DataError). 
+00012e70: 2020 2020 2020 2020 2020 2069 6620 6b20             if k 
+00012e80: 3d3d 2022 7841 7869 7322 206f 7220 6b20  == "xAxis" or k 
+00012e90: 3d3d 2022 7941 7869 7322 3a0a 2020 2020  == "yAxis":.    
+00012ea0: 2020 2020 2020 2020 2020 2020 6966 2069              if i
+00012eb0: 7369 6e73 7461 6e63 6528 762c 2064 6963  sinstance(v, dic
+00012ec0: 7429 3a0a 2020 2020 2020 2020 2020 2020  t):.            
+00012ed0: 2020 2020 2020 2020 7620 3d20 5b76 5d0a          v = [v].
+00012ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012ef0: 6966 206c 656e 2876 2920 213d 206c 656e  if len(v) != len
+00012f00: 286f 7074 696f 6e73 5b6b 5d29 3a0a 2020  (options[k]):.  
+00012f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012f20: 2020 6c6f 675f 6572 726f 7228 6c6f 6767    log_error(logg
+00012f30: 6572 2c20 6622 5468 6520 6e75 6d62 6572  er, f"The number
+00012f40: 206f 6620 7b6b 7d20 6d75 7374 2062 6520   of {k} must be 
+00012f50: 7b6c 656e 2876 297d 222c 2044 6174 6145  {len(v)}", DataE
+00012f60: 7272 6f72 290a 2020 2020 2020 2020 2020  rror).          
+00012f70: 2020 2020 2020 666f 7220 692c 2076 5f20        for i, v_ 
+00012f80: 696e 2065 6e75 6d65 7261 7465 2876 293a  in enumerate(v):
+00012f90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012fa0: 2020 2020 206f 7074 696f 6e73 5b6b 5d5b       options[k][
+00012fb0: 695d 2e75 7064 6174 6528 765f 290a 2020  i].update(v_).  
+00012fc0: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
+00012fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012fe0: 6f70 7469 6f6e 735b 6b5d 203d 2076 0a0a  options[k] = v..
+00012ff0: 2020 2020 6173 796e 6320 6465 6620 5f63      async def _c
+00013000: 7265 6174 655f 6563 6861 7274 280a 2020  reate_echart(.  
+00013010: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
+00013020: 2020 2020 6f70 7469 6f6e 733a 2064 6963      options: dic
+00013030: 742c 0a20 2020 2020 2020 206f 7264 6572  t,.        order
+00013040: 3a20 696e 742c 0a20 2020 2020 2020 2066  : int,.        f
+00013050: 6965 6c64 733a 206c 6973 745b 556e 696f  ields: list[Unio
+00013060: 6e5b 7374 722c 2074 7570 6c65 2c20 6469  n[str, tuple, di
+00013070: 6374 5d5d 2c0a 2020 2020 2020 2020 6461  ct]],.        da
+00013080: 7461 5f6d 6170 7069 6e67 5f74 6f5f 7475  ta_mapping_to_tu
+00013090: 706c 6573 3a20 4f70 7469 6f6e 616c 5b64  ples: Optional[d
+000130a0: 6963 745d 203d 204e 6f6e 652c 0a20 2020  ict] = None,.   
+000130b0: 2020 2020 2064 6174 613a 204f 7074 696f       data: Optio
+000130c0: 6e61 6c5b 556e 696f 6e5b 7374 722c 2070  nal[Union[str, p
+000130d0: 642e 4461 7461 4672 616d 655d 5d20 3d20  d.DataFrame]] = 
+000130e0: 4e6f 6e65 2c0a 2020 2020 2020 2020 6475  None,.        du
+000130f0: 6d70 5f77 686f 6c65 3a20 626f 6f6c 203d  mp_whole: bool =
+00013100: 2046 616c 7365 2c0a 2020 2020 2020 2020   False,.        
+00013110: 6f70 7469 6f6e 5f6d 6f64 6966 6963 6174  option_modificat
+00013120: 696f 6e73 3a20 4f70 7469 6f6e 616c 5b64  ions: Optional[d
+00013130: 6963 745d 203d 204e 6f6e 652c 0a20 2020  ict] = None,.   
+00013140: 2020 2020 2074 6974 6c65 3a20 4f70 7469       title: Opti
+00013150: 6f6e 616c 5b73 7472 5d20 3d20 4e6f 6e65  onal[str] = None
+00013160: 2c0a 2020 2020 2020 2020 726f 7773 5f73  ,.        rows_s
+00013170: 697a 653a 204f 7074 696f 6e61 6c5b 696e  ize: Optional[in
+00013180: 745d 203d 204e 6f6e 652c 0a20 2020 2020  t] = None,.     
+00013190: 2020 2063 6f6c 735f 7369 7a65 3a20 4f70     cols_size: Op
+000131a0: 7469 6f6e 616c 5b69 6e74 5d20 3d20 4e6f  tional[int] = No
+000131b0: 6e65 2c0a 2020 2020 2020 2020 7061 6464  ne,.        padd
+000131c0: 696e 673a 204f 7074 696f 6e61 6c5b 7374  ing: Optional[st
+000131d0: 725d 203d 204e 6f6e 652c 0a20 2020 2029  r] = None,.    )
+000131e0: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+000131f0: 2020 2020 2020 4372 6561 7465 2061 6e20        Create an 
+00013200: 6563 6861 7274 2069 6e20 7468 6520 6461  echart in the da
+00013210: 7368 626f 6172 642c 2066 696c 6c20 696e  shboard, fill in
+00013220: 2074 6865 2064 6174 6120 7265 6665 7265   the data refere
+00013230: 6e63 6564 2069 6e20 7468 6520 6563 6861  nced in the echa
+00013240: 7274 5f6f 7074 696f 6e73 2061 6e64 2063  rt_options and c
+00013250: 7265 6174 6520 6f72 0a20 2020 2020 2020  reate or.       
+00013260: 2075 7064 6174 6520 7468 6520 6368 6172   update the char
+00013270: 7420 616e 6420 6461 7461 2073 6574 206c  t and data set l
+00013280: 696e 6b73 2e0a 2020 2020 2020 2020 3a70  inks..        :p
+00013290: 6172 616d 206f 7074 696f 6e73 3a20 7468  aram options: th
+000132a0: 6520 6f70 7469 6f6e 7320 6f66 2074 6865  e options of the
+000132b0: 2065 6368 6172 740a 2020 2020 2020 2020   echart.        
+000132c0: 3a70 6172 616d 2064 6174 615f 6d61 7070  :param data_mapp
+000132d0: 696e 675f 746f 5f74 7570 6c65 733a 2074  ing_to_tuples: t
+000132e0: 6865 206d 6170 7069 6e67 206f 6620 7468  he mapping of th
+000132f0: 6520 6461 7461 2074 6f20 7468 6520 7475  e data to the tu
+00013300: 706c 6573 0a20 2020 2020 2020 203a 7061  ples.        :pa
+00013310: 7261 6d20 6461 7461 3a20 7468 6520 6461  ram data: the da
+00013320: 7461 206f 6620 7468 6520 6563 6861 7274  ta of the echart
+00013330: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+00013340: 6475 6d70 5f77 686f 6c65 3a20 7768 6574  dump_whole: whet
+00013350: 6865 7220 746f 2064 756d 7020 7468 6520  her to dump the 
+00013360: 7768 6f6c 6520 6461 7461 0a20 2020 2020  whole data.     
+00013370: 2020 203a 7061 7261 6d20 6f70 7469 6f6e     :param option
+00013380: 5f6d 6f64 6966 6963 6174 696f 6e73 3a20  _modifications: 
+00013390: 7468 6520 6d6f 6469 6669 6361 7469 6f6e  the modification
+000133a0: 7320 746f 2061 7070 6c79 2074 6f20 7468  s to apply to th
+000133b0: 6520 6f70 7469 6f6e 730a 2020 2020 2020  e options.      
+000133c0: 2020 3a70 6172 616d 2074 6974 6c65 3a20    :param title: 
+000133d0: 7468 6520 7469 746c 6520 6f66 2074 6865  the title of the
+000133e0: 2065 6368 6172 740a 2020 2020 2020 2020   echart.        
+000133f0: 3a70 6172 616d 2072 6f77 735f 7369 7a65  :param rows_size
+00013400: 3a20 7468 6520 726f 7773 2073 697a 6520  : the rows size 
+00013410: 6f66 2074 6865 2065 6368 6172 740a 2020  of the echart.  
+00013420: 2020 2020 2020 3a70 6172 616d 2063 6f6c        :param col
+00013430: 735f 7369 7a65 3a20 7468 6520 636f 6c75  s_size: the colu
+00013440: 6d6e 7320 7369 7a65 206f 6620 7468 6520  mns size of the 
+00013450: 6563 6861 7274 0a20 2020 2020 2020 203a  echart.        :
+00013460: 7061 7261 6d20 7061 6464 696e 673a 2074  param padding: t
+00013470: 6865 2070 6164 6469 6e67 206f 6620 7468  he padding of th
+00013480: 6520 6563 6861 7274 0a20 2020 2020 2020  e echart.       
+00013490: 2022 2222 0a0a 2020 2020 2020 2020 6966   """..        if
+000134a0: 2064 6174 6120 6973 206e 6f74 204e 6f6e   data is not Non
+000134b0: 653a 0a20 2020 2020 2020 2020 2020 2064  e:.            d
+000134c0: 6174 615f 6d61 7070 696e 675f 746f 5f74  ata_mapping_to_t
+000134d0: 7570 6c65 7320 3d20 6177 6169 7420 7365  uples = await se
+000134e0: 6c66 2e5f 6368 6f6f 7365 5f64 6174 6128  lf._choose_data(
+000134f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00013500: 206f 7264 6572 2c20 6461 7461 2c20 6475   order, data, du
+00013510: 6d70 5f77 686f 6c65 3d64 756d 705f 7768  mp_whole=dump_wh
+00013520: 6f6c 650a 2020 2020 2020 2020 2020 2020  ole.            
+00013530: 290a 0a20 2020 2020 2020 2064 6174 615f  )..        data_
+00013540: 6b65 795f 656e 7472 6965 7320 3d20 6765  key_entries = ge
+00013550: 745f 6461 7461 5f72 6566 6572 656e 6365  t_data_reference
+00013560: 735f 6672 6f6d 5f64 6963 7428 6f70 7469  s_from_dict(opti
+00013570: 6f6e 7329 0a20 2020 2020 2020 205f 2c20  ons).        _, 
+00013580: 7265 706f 7274 203d 2061 7761 6974 2073  report = await s
+00013590: 656c 662e 5f67 6574 5f63 6861 7274 5f72  elf._get_chart_r
+000135a0: 6570 6f72 7428 6f72 6465 722c 2045 4368  eport(order, ECh
+000135b0: 6172 7429 0a0a 2020 2020 2020 2020 7264  art)..        rd
+000135c0: 5f69 6473 203d 204e 6f6e 650a 2020 2020  _ids = None.    
+000135d0: 2020 2020 6966 2073 656c 662e 7265 7573      if self.reus
+000135e0: 655f 6461 7461 5f73 6574 733a 0a20 2020  e_data_sets:.   
+000135f0: 2020 2020 2020 2020 2072 645f 6964 7320           rd_ids 
+00013600: 3d20 6765 745f 7575 6964 735f 6672 6f6d  = get_uuids_from
+00013610: 5f64 6963 7428 7265 706f 7274 5b22 7072  _dict(report["pr
+00013620: 6f70 6572 7469 6573 225d 5b22 6f70 7469  operties"]["opti
+00013630: 6f6e 225d 290a 2020 2020 2020 2020 2020  on"]).          
+00013640: 2020 6966 206c 656e 2872 645f 6964 7329    if len(rd_ids)
+00013650: 203d 3d20 6c65 6e28 6669 656c 6473 293a   == len(fields):
+00013660: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00013670: 2072 6570 5f64 733a 206c 6973 745b 5265   rep_ds: list[Re
+00013680: 706f 7274 2e52 6570 6f72 7444 6174 6153  port.ReportDataS
+00013690: 6574 5d20 3d20 6177 6169 7420 7265 706f  et] = await repo
+000136a0: 7274 2e67 6574 5f72 6570 6f72 745f 6461  rt.get_report_da
+000136b0: 7461 5f73 6574 7328 290a 2020 2020 2020  ta_sets().      
+000136c0: 2020 2020 2020 2020 2020 6d61 7070 6564            mapped
+000136d0: 5f66 203d 205b 0a20 2020 2020 2020 2020  _f = [.         
+000136e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000136f0: 5f67 6574 5f66 6965 6c64 5f6d 6170 7069  _get_field_mappi
+00013700: 6e67 2866 6965 6c64 2c20 6461 7461 5f6d  ng(field, data_m
+00013710: 6170 7069 6e67 5f74 6f5f 7475 706c 6573  apping_to_tuples
+00013720: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00013730: 2020 2020 2020 666f 7220 6669 656c 6420        for field 
+00013740: 696e 2066 6965 6c64 730a 2020 2020 2020  in fields.      
+00013750: 2020 2020 2020 2020 2020 5d0a 2020 2020            ].    
+00013760: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+00013770: 692c 2072 645f 6964 2069 6e20 656e 756d  i, rd_id in enum
+00013780: 6572 6174 6528 7264 5f69 6473 293a 0a20  erate(rd_ids):. 
+00013790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000137a0: 2020 2072 6570 6f72 745f 6461 7461 5f73     report_data_s
+000137b0: 6574 203d 206e 6578 7428 0a20 2020 2020  et = next(.     
+000137c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000137d0: 2020 2028 7264 2066 6f72 2072 6420 696e     (rd for rd in
+000137e0: 2072 6570 5f64 7320 6966 2072 645b 2269   rep_ds if rd["i
+000137f0: 6422 5d20 3d3d 2072 645f 6964 292c 204e  d"] == rd_id), N
+00013800: 6f6e 650a 2020 2020 2020 2020 2020 2020  one.            
+00013810: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+00013820: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00013830: 2028 0a20 2020 2020 2020 2020 2020 2020   (.             
+00013840: 2020 2020 2020 2020 2020 206e 6f74 2072             not r
+00013850: 6570 6f72 745f 6461 7461 5f73 6574 0a20  eport_data_set. 
+00013860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013870: 2020 2020 2020 206f 7220 6e6f 7420 7365         or not se
+00013880: 6c66 2e5f 6368 6563 6b5f 6d61 7070 696e  lf._check_mappin
+00013890: 675f 696e 5f72 6570 6f72 745f 6461 7461  g_in_report_data
+000138a0: 5f73 6574 280a 2020 2020 2020 2020 2020  _set(.          
+000138b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000138c0: 2020 7265 706f 7274 5f64 6174 615f 7365    report_data_se
+000138d0: 742c 206d 6170 7065 645f 665b 695d 0a20  t, mapped_f[i]. 
+000138e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000138f0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00013900: 2020 2020 2020 2020 2020 2020 2029 3a0a               ):.
+00013910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013920: 2020 2020 2020 2020 7264 5f69 6473 203d          rd_ids =
+00013930: 204e 6f6e 650a 2020 2020 2020 2020 2020   None.          
+00013940: 2020 2020 2020 2020 2020 2020 2020 6272                br
+00013950: 6561 6b0a 2020 2020 2020 2020 2020 2020  eak.            
+00013960: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+00013970: 2020 2020 2020 7264 5f69 6473 203d 204e        rd_ids = N
+00013980: 6f6e 650a 0a20 2020 2020 2020 2069 6620  one..        if 
+00013990: 6e6f 7420 7264 5f69 6473 3a0a 2020 2020  not rd_ids:.    
+000139a0: 2020 2020 2020 2020 6177 6169 7420 7265          await re
+000139b0: 706f 7274 2e64 656c 6574 655f 7265 706f  port.delete_repo
+000139c0: 7274 5f64 6174 615f 7365 7473 286c 6f67  rt_data_sets(log
+000139d0: 3d54 7275 6529 0a20 2020 2020 2020 2020  =True).         
+000139e0: 2020 2072 6570 6f72 745f 6461 7461 5f73     report_data_s
+000139f0: 6574 7320 3d20 6177 6169 7420 7365 6c66  ets = await self
+00013a00: 2e5f 6765 745f 7265 706f 7274 5f64 6174  ._get_report_dat
+00013a10: 615f 7365 7473 5f70 6572 5f6d 6170 7069  a_sets_per_mappi
+00013a20: 6e67 280a 2020 2020 2020 2020 2020 2020  ng(.            
+00013a30: 2020 2020 7265 706f 7274 2c20 6461 7461      report, data
+00013a40: 5f6d 6170 7069 6e67 5f74 6f5f 7475 706c  _mapping_to_tupl
+00013a50: 6573 2c20 6669 656c 6473 0a20 2020 2020  es, fields.     
+00013a60: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00013a70: 2020 2020 2072 645f 6964 7320 3d20 5b72       rd_ids = [r
+00013a80: 645b 2269 6422 5d20 666f 7220 7264 2069  d["id"] for rd i
+00013a90: 6e20 7265 706f 7274 5f64 6174 615f 7365  n report_data_se
+00013aa0: 7473 5d0a 0a20 2020 2020 2020 2073 656c  ts]..        sel
+00013ab0: 662e 5f75 7064 6174 655f 6f70 7469 6f6e  f._update_option
+00013ac0: 7328 6f70 7469 6f6e 732c 206f 7074 696f  s(options, optio
+00013ad0: 6e5f 6d6f 6469 6669 6361 7469 6f6e 7329  n_modifications)
+00013ae0: 0a0a 2020 2020 2020 2020 6966 206c 656e  ..        if len
+00013af0: 2872 645f 6964 7329 2021 3d20 6c65 6e28  (rd_ids) != len(
+00013b00: 6461 7461 5f6b 6579 5f65 6e74 7269 6573  data_key_entries
+00013b10: 293a 0a20 2020 2020 2020 2020 2020 206c  ):.            l
+00013b20: 6f67 5f65 7272 6f72 280a 2020 2020 2020  og_error(.      
+00013b30: 2020 2020 2020 2020 2020 6c6f 6767 6572            logger
+00013b40: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00013b50: 2020 6622 5468 6520 6e75 6d62 6572 206f    f"The number o
+00013b60: 6620 6461 7461 2072 6566 6572 656e 6365  f data reference
+00013b70: 7320 616e 6420 6669 656c 6473 206d 7573  s and fields mus
+00013b80: 7420 6265 2065 7175 616c 2c20 220a 2020  t be equal, ".  
+00013b90: 2020 2020 2020 2020 2020 2020 2020 6622                f"
+00013ba0: 7468 6579 2061 7265 207b 6c65 6e28 6461  they are {len(da
+00013bb0: 7461 5f6b 6579 5f65 6e74 7269 6573 297d  ta_key_entries)}
+00013bc0: 2061 6e64 207b 6c65 6e28 7264 5f69 6473   and {len(rd_ids
+00013bd0: 297d 2072 6573 7065 6374 6976 656c 792e  )} respectively.
+00013be0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00013bf0: 2020 2044 6174 6145 7272 6f72 2c0a 2020     DataError,.  
+00013c00: 2020 2020 2020 2020 2020 290a 0a20 2020            )..   
+00013c10: 2020 2020 2066 6f72 2069 2c20 6461 7461       for i, data
+00013c20: 5f6b 6579 5f65 6e74 7279 2069 6e20 656e  _key_entry in en
+00013c30: 756d 6572 6174 6528 6461 7461 5f6b 6579  umerate(data_key
+00013c40: 5f65 6e74 7269 6573 293a 0a20 2020 2020  _entries):.     
+00013c50: 2020 2020 2020 2064 6174 6120 3d20 6f70         data = op
+00013c60: 7469 6f6e 730a 2020 2020 2020 2020 2020  tions.          
+00013c70: 2020 666f 7220 6b65 7920 696e 2064 6174    for key in dat
+00013c80: 615f 6b65 795f 656e 7472 795b 3a2d 315d  a_key_entry[:-1]
+00013c90: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00013ca0: 2020 6461 7461 203d 2064 6174 615b 6b65    data = data[ke
+00013cb0: 795d 0a20 2020 2020 2020 2020 2020 2064  y].            d
+00013cc0: 6174 615b 6461 7461 5f6b 6579 5f65 6e74  ata[data_key_ent
+00013cd0: 7279 5b2d 315d 5d20 3d20 2223 7b22 202b  ry[-1]] = "#{" +
+00013ce0: 2072 645f 6964 735b 695d 202b 2022 7d22   rd_ids[i] + "}"
+00013cf0: 0a0a 2020 2020 2020 2020 6177 6169 7420  ..        await 
+00013d00: 7365 6c66 2e5f 6372 6561 7465 5f63 6861  self._create_cha
+00013d10: 7274 280a 2020 2020 2020 2020 2020 2020  rt(.            
+00013d20: 6368 6172 745f 636c 6173 733d 4543 6861  chart_class=ECha
+00013d30: 7274 2c0a 2020 2020 2020 2020 2020 2020  rt,.            
+00013d40: 7072 6f70 6572 7469 6573 3d7b 226f 7074  properties={"opt
+00013d50: 696f 6e22 3a20 6f70 7469 6f6e 737d 2c0a  ion": options},.
+00013d60: 2020 2020 2020 2020 2020 2020 6f72 6465              orde
+00013d70: 723d 6f72 6465 722c 0a20 2020 2020 2020  r=order,.       
+00013d80: 2020 2020 2074 6974 6c65 3d74 6974 6c65       title=title
+00013d90: 2c0a 2020 2020 2020 2020 2020 2020 7369  ,.            si
+00013da0: 7a65 5061 6464 696e 673d 7061 6464 696e  zePadding=paddin
+00013db0: 672c 0a20 2020 2020 2020 2020 2020 2073  g,.            s
+00013dc0: 697a 6552 6f77 733d 726f 7773 5f73 697a  izeRows=rows_siz
+00013dd0: 652c 0a20 2020 2020 2020 2020 2020 2073  e,.            s
+00013de0: 697a 6543 6f6c 756d 6e73 3d63 6f6c 735f  izeColumns=cols_
+00013df0: 7369 7a65 2c0a 2020 2020 2020 2020 290a  size,.        ).
+00013e00: 0a20 2020 2040 7374 6174 6963 6d65 7468  .    @staticmeth
+00013e10: 6f64 0a20 2020 2064 6566 205f 6170 706c  od.    def _appl
+00013e20: 795f 7661 7269 616e 7428 6563 6861 7274  y_variant(echart
+00013e30: 5f6f 7074 696f 6e73 3a20 6469 6374 2c20  _options: dict, 
+00013e40: 7661 7269 616e 743a 204f 7074 696f 6e61  variant: Optiona
+00013e50: 6c5b 7374 725d 293a 0a20 2020 2020 2020  l[str]):.       
+00013e60: 2069 6620 7661 7269 616e 7420 3d3d 2022   if variant == "
+00013e70: 636c 6561 6e22 3a0a 2020 2020 2020 2020  clean":.        
+00013e80: 2020 2020 6563 6861 7274 5f6f 7074 696f      echart_optio
+00013e90: 6e73 2e75 7064 6174 6528 0a20 2020 2020  ns.update(.     
+00013ea0: 2020 2020 2020 2020 2020 207b 2274 6f6f             {"too
+00013eb0: 6c62 6f78 223a 207b 2273 686f 7722 3a20  lbox": {"show": 
+00013ec0: 4661 6c73 657d 2c20 226c 6567 656e 6422  False}, "legend"
+00013ed0: 3a20 7b22 7368 6f77 223a 2046 616c 7365  : {"show": False
+00013ee0: 7d2c 2022 6772 6964 223a 207b 7d7d 0a20  }, "grid": {}}. 
+00013ef0: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+00013f00: 2020 2020 2020 2020 2066 6f72 2061 7869           for axi
+00013f10: 736c 6973 7420 696e 205b 6563 6861 7274  slist in [echart
+00013f20: 5f6f 7074 696f 6e73 5b22 7841 7869 7322  _options["xAxis"
+00013f30: 5d2c 2065 6368 6172 745f 6f70 7469 6f6e  ], echart_option
+00013f40: 735b 2279 4178 6973 225d 5d3a 0a20 2020  s["yAxis"]]:.   
+00013f50: 2020 2020 2020 2020 2020 2020 2066 6f72               for
+00013f60: 2061 7869 7320 696e 2061 7869 736c 6973   axis in axislis
+00013f70: 743a 0a20 2020 2020 2020 2020 2020 2020  t:.             
+00013f80: 2020 2020 2020 2061 7869 732e 7570 6461         axis.upda
+00013f90: 7465 280a 2020 2020 2020 2020 2020 2020  te(.            
+00013fa0: 2020 2020 2020 2020 2020 2020 7b22 6178              {"ax
+00013fb0: 6973 4c69 6e65 223a 207b 2273 686f 7722  isLine": {"show"
+00013fc0: 3a20 4661 6c73 657d 2c20 2261 7869 7354  : False}, "axisT
+00013fd0: 6963 6b22 3a20 7b22 7368 6f77 223a 2046  ick": {"show": F
+00013fe0: 616c 7365 7d7d 0a20 2020 2020 2020 2020  alse}}.         
+00013ff0: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+00014000: 2020 2020 2065 6c69 6620 7661 7269 616e       elif varian
+00014010: 7420 3d3d 2022 6d69 6e69 6d61 6c22 3a0a  t == "minimal":.
+00014020: 2020 2020 2020 2020 2020 2020 6563 6861              echa
+00014030: 7274 5f6f 7074 696f 6e73 2e75 7064 6174  rt_options.updat
+00014040: 6528 0a20 2020 2020 2020 2020 2020 2020  e(.             
+00014050: 2020 207b 0a20 2020 2020 2020 2020 2020     {.           
+00014060: 2020 2020 2020 2020 2022 746f 6f6c 626f           "toolbo
+00014070: 7822 3a20 7b22 7368 6f77 223a 2046 616c  x": {"show": Fal
+00014080: 7365 7d2c 0a20 2020 2020 2020 2020 2020  se},.           
+00014090: 2020 2020 2020 2020 2022 6c65 6765 6e64           "legend
+000140a0: 223a 207b 2273 686f 7722 3a20 4661 6c73  ": {"show": Fals
+000140b0: 657d 2c0a 2020 2020 2020 2020 2020 2020  e},.            
+000140c0: 2020 2020 2020 2020 2267 7269 6422 3a20          "grid": 
+000140d0: 7b22 6c65 6674 223a 2022 3125 222c 2022  {"left": "1%", "
+000140e0: 7269 6768 7422 3a20 2231 2522 2c20 2274  right": "1%", "t
+000140f0: 6f70 223a 2022 3125 222c 2022 626f 7474  op": "1%", "bott
+00014100: 6f6d 223a 2022 3125 227d 2c0a 2020 2020  om": "1%"},.    
+00014110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014120: 2274 6f6f 6c74 6970 223a 207b 2273 686f  "tooltip": {"sho
+00014130: 7722 3a20 4661 6c73 657d 2c0a 2020 2020  w": False},.    
+00014140: 2020 2020 2020 2020 2020 2020 7d0a 2020              }.  
+00014150: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+00014160: 2020 2020 2020 2020 666f 7220 6178 6973          for axis
+00014170: 6c69 7374 2069 6e20 5b65 6368 6172 745f  list in [echart_
+00014180: 6f70 7469 6f6e 735b 2278 4178 6973 225d  options["xAxis"]
+00014190: 2c20 6563 6861 7274 5f6f 7074 696f 6e73  , echart_options
+000141a0: 5b22 7941 7869 7322 5d5d 3a0a 2020 2020  ["yAxis"]]:.    
+000141b0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+000141c0: 6178 6973 2069 6e20 6178 6973 6c69 7374  axis in axislist
+000141d0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000141e0: 2020 2020 2020 6178 6973 2e75 7064 6174        axis.updat
+000141f0: 6528 0a20 2020 2020 2020 2020 2020 2020  e(.             
+00014200: 2020 2020 2020 2020 2020 207b 0a20 2020             {.   
+00014210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014220: 2020 2020 2020 2020 2022 6178 6973 4c69           "axisLi
+00014230: 6e65 223a 207b 2273 686f 7722 3a20 4661  ne": {"show": Fa
+00014240: 6c73 657d 2c0a 2020 2020 2020 2020 2020  lse},.          
+00014250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014260: 2020 2261 7869 7354 6963 6b22 3a20 7b22    "axisTick": {"
+00014270: 7368 6f77 223a 2046 616c 7365 7d2c 0a20  show": False},. 
+00014280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014290: 2020 2020 2020 2020 2020 2022 7370 6c69             "spli
+000142a0: 744c 696e 6522 3a20 7b22 7368 6f77 223a  tLine": {"show":
+000142b0: 2046 616c 7365 7d2c 0a20 2020 2020 2020   False},.       
+000142c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000142d0: 2020 2020 2022 6178 6973 4c61 6265 6c22       "axisLabel"
+000142e0: 3a20 7b22 7368 6f77 223a 2046 616c 7365  : {"show": False
+000142f0: 7d2c 0a20 2020 2020 2020 2020 2020 2020  },.             
+00014300: 2020 2020 2020 2020 2020 207d 0a20 2020             }.   
+00014310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014320: 2029 0a0a 2020 2020 6173 796e 6320 6465   )..    async de
+00014330: 6620 5f63 7265 6174 655f 7472 656e 645f  f _create_trend_
+00014340: 6368 6172 7428 0a20 2020 2020 2020 2073  chart(.        s
+00014350: 656c 662c 0a20 2020 2020 2020 2061 7865  elf,.        axe
+00014360: 733a 2055 6e69 6f6e 5b6c 6973 745b 7374  s: Union[list[st
+00014370: 725d 2c20 7374 725d 2c0a 2020 2020 2020  r], str],.      
+00014380: 2020 6f72 6465 723a 2069 6e74 2c0a 2020    order: int,.  
+00014390: 2020 2020 2020 6461 7461 5f6d 6170 7069        data_mappi
+000143a0: 6e67 5f74 6f5f 7475 706c 6573 3a20 4f70  ng_to_tuples: Op
+000143b0: 7469 6f6e 616c 5b64 6963 745d 2c0a 2020  tional[dict],.  
+000143c0: 2020 2020 2020 6563 6861 7274 5f6f 7074        echart_opt
+000143d0: 696f 6e73 3a20 6469 6374 2c0a 2020 2020  ions: dict,.    
+000143e0: 2020 2020 7365 7269 6573 5f6f 7074 696f      series_optio
+000143f0: 6e73 3a20 556e 696f 6e5b 6469 6374 2c20  ns: Union[dict, 
+00014400: 6c69 7374 5b64 6963 745d 5d2c 0a20 2020  list[dict]],.   
+00014410: 2020 2020 2076 616c 7565 733a 204f 7074       values: Opt
+00014420: 696f 6e61 6c5b 556e 696f 6e5b 6c69 7374  ional[Union[list
+00014430: 5b55 6e69 6f6e 5b73 7472 2c20 7475 706c  [Union[str, tupl
+00014440: 655d 5d2c 2073 7472 2c20 7475 706c 655d  e]], str, tuple]
+00014450: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
+00014460: 2020 785f 6178 6973 5f6e 616d 6573 3a20    x_axis_names: 
+00014470: 4f70 7469 6f6e 616c 5b55 6e69 6f6e 5b73  Optional[Union[s
+00014480: 7472 2c20 6c69 7374 5b73 7472 5d5d 5d20  tr, list[str]]] 
+00014490: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+000144a0: 795f 6178 6973 5f6e 616d 6573 3a20 4f70  y_axis_names: Op
+000144b0: 7469 6f6e 616c 5b55 6e69 6f6e 5b73 7472  tional[Union[str
+000144c0: 2c20 6c69 7374 5b73 7472 5d5d 5d20 3d20  , list[str]]] = 
+000144d0: 4e6f 6e65 2c0a 2020 2020 2020 2020 7368  None,.        sh
+000144e0: 6f77 5f76 616c 7565 733a 204f 7074 696f  ow_values: Optio
+000144f0: 6e61 6c5b 556e 696f 6e5b 6c69 7374 5b73  nal[Union[list[s
+00014500: 7472 5d2c 2073 7472 5d5d 203d 204e 6f6e  tr], str]] = Non
+00014510: 652c 0a20 2020 2020 2020 2076 6172 6961  e,.        varia
+00014520: 6e74 3a20 4f70 7469 6f6e 616c 5b73 7472  nt: Optional[str
+00014530: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
+00014540: 2020 2a2a 7265 706f 7274 5f70 6172 616d    **report_param
+00014550: 732c 0a20 2020 2029 3a0a 2020 2020 2020  s,.    ):.      
+00014560: 2020 2222 220a 2020 2020 2020 2020 4372    """.        Cr
+00014570: 6561 7465 2061 206c 696e 6520 6368 6172  eate a line char
+00014580: 7420 696e 2074 6865 2064 6173 6862 6f61  t in the dashboa
+00014590: 7264 2e0a 2020 2020 2020 2020 3a70 6172  rd..        :par
+000145a0: 616d 2064 6174 613a 2074 6865 2064 6174  am data: the dat
+000145b0: 6120 6f66 2074 6865 2063 6861 7274 0a20  a of the chart. 
+000145c0: 2020 2020 2020 203a 7061 7261 6d20 6178         :param ax
+000145d0: 6573 3a20 7468 6520 6e61 6d65 7320 6f66  es: the names of
+000145e0: 2074 6865 2063 6f6c 756d 6e73 2074 6f20   the columns to 
+000145f0: 6265 2075 7365 6420 6173 2061 7869 730a  be used as axis.
+00014600: 2020 2020 2020 2020 3a70 6172 616d 2076          :param v
+00014610: 616c 7565 733a 2074 6865 206e 616d 6573  alues: the names
+00014620: 206f 6620 7468 6520 636f 6c75 6d6e 7320   of the columns 
+00014630: 746f 2062 6520 7573 6564 2061 7320 7661  to be used as va
+00014640: 6c75 6573 0a20 2020 2020 2020 203a 7061  lues.        :pa
+00014650: 7261 6d20 785f 6178 6973 5f6e 616d 6573  ram x_axis_names
+00014660: 3a20 7468 6520 6e61 6d65 206f 6620 7468  : the name of th
+00014670: 6520 7820 6178 6573 0a20 2020 2020 2020  e x axes.       
+00014680: 203a 7061 7261 6d20 795f 6178 6973 5f6e   :param y_axis_n
+00014690: 616d 6573 3a20 7468 6520 6e61 6d65 206f  ames: the name o
+000146a0: 6620 7468 6520 7920 6178 6573 0a20 2020  f the y axes.   
+000146b0: 2020 2020 203a 7061 7261 6d20 6563 6861       :param echa
+000146c0: 7274 5f6f 7074 696f 6e73 3a20 7468 6520  rt_options: the 
+000146d0: 6f70 7469 6f6e 7320 6f66 2074 6865 2063  options of the c
+000146e0: 6861 7274 0a20 2020 2020 2020 203a 7061  hart.        :pa
+000146f0: 7261 6d20 7365 7269 6573 5f6f 7074 696f  ram series_optio
+00014700: 6e73 3a20 7468 6520 6f70 7469 6f6e 7320  ns: the options 
+00014710: 6f66 2074 6865 2073 6572 6965 7320 6f66  of the series of
+00014720: 2074 6865 2063 6861 7274 0a20 2020 2020   the chart.     
+00014730: 2020 203a 7061 7261 6d20 626f 7474 6f6d     :param bottom
+00014740: 5f74 6f6f 6c62 6f78 3a20 7768 6574 6865  _toolbox: whethe
+00014750: 7220 746f 2073 686f 7720 7468 6520 746f  r to show the to
+00014760: 6f6c 626f 7820 6f6e 2074 6f70 206f 6620  olbox on top of 
+00014770: 7468 6520 6368 6172 740a 2020 2020 2020  the chart.      
+00014780: 2020 3a70 6172 616d 206f 7264 6572 3a20    :param order: 
+00014790: 7468 6520 6f72 6465 7220 6f66 2074 6865  the order of the
+000147a0: 2063 6861 7274 2069 6e20 7468 6520 6461   chart in the da
+000147b0: 7368 626f 6172 640a 2020 2020 2020 2020  shboard.        
+000147c0: 3a70 6172 616d 2072 6570 6f72 745f 7061  :param report_pa
+000147d0: 7261 6d73 3a20 6164 6469 7469 6f6e 616c  rams: additional
+000147e0: 2072 6570 6f72 7420 7061 7261 6d65 7465   report paramete
+000147f0: 7273 2061 7320 6b65 792d 7661 6c75 6520  rs as key-value 
+00014800: 7061 6972 730a 2020 2020 2020 2020 2222  pairs.        ""
+00014810: 220a 2020 2020 2020 2020 7365 6c66 2e5f  ".        self._
+00014820: 6170 706c 795f 7661 7269 616e 7428 6563  apply_variant(ec
+00014830: 6861 7274 5f6f 7074 696f 6e73 2c20 7661  hart_options, va
+00014840: 7269 616e 7429 0a20 2020 2020 2020 2069  riant).        i
+00014850: 6620 6973 696e 7374 616e 6365 2861 7865  f isinstance(axe
+00014860: 732c 2073 7472 293a 0a20 2020 2020 2020  s, str):.       
+00014870: 2020 2020 2061 7865 7320 3d20 5b61 7865       axes = [axe
+00014880: 735d 0a20 2020 2020 2020 2069 6620 6973  s].        if is
+00014890: 696e 7374 616e 6365 2876 616c 7565 732c  instance(values,
+000148a0: 2073 7472 2920 6f72 2069 7369 6e73 7461   str) or isinsta
+000148b0: 6e63 6528 7661 6c75 6573 2c20 7475 706c  nce(values, tupl
+000148c0: 6529 3a0a 2020 2020 2020 2020 2020 2020  e):.            
+000148d0: 7661 6c75 6573 203d 205b 7661 6c75 6573  values = [values
+000148e0: 5d0a 2020 2020 2020 2020 6966 2073 686f  ].        if sho
+000148f0: 775f 7661 6c75 6573 2069 7320 4e6f 6e65  w_values is None
+00014900: 3a0a 2020 2020 2020 2020 2020 2020 7368  :.            sh
+00014910: 6f77 5f76 616c 7565 7320 3d20 5b5d 0a0a  ow_values = []..
+00014920: 2020 2020 2020 2020 6966 2022 785f 6178          if "x_ax
+00014930: 6973 5f6e 616d 6522 2069 6e20 7265 706f  is_name" in repo
+00014940: 7274 5f70 6172 616d 733a 0a20 2020 2020  rt_params:.     
+00014950: 2020 2020 2020 2078 5f61 7869 735f 6e61         x_axis_na
+00014960: 6d65 7320 3d20 5b72 6570 6f72 745f 7061  mes = [report_pa
+00014970: 7261 6d73 5b22 785f 6178 6973 5f6e 616d  rams["x_axis_nam
+00014980: 6522 5d5d 0a20 2020 2020 2020 2065 6c69  e"]].        eli
+00014990: 6620 6973 696e 7374 616e 6365 2878 5f61  f isinstance(x_a
+000149a0: 7869 735f 6e61 6d65 732c 2073 7472 293a  xis_names, str):
+000149b0: 0a20 2020 2020 2020 2020 2020 2078 5f61  .            x_a
+000149c0: 7869 735f 6e61 6d65 7320 3d20 5b78 5f61  xis_names = [x_a
+000149d0: 7869 735f 6e61 6d65 735d 0a20 2020 2020  xis_names].     
+000149e0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+000149f0: 2020 2020 2078 5f61 7869 735f 6e61 6d65       x_axis_name
+00014a00: 7320 3d20 5b5d 0a0a 2020 2020 2020 2020  s = []..        
+00014a10: 6966 2022 795f 6178 6973 5f6e 616d 6522  if "y_axis_name"
+00014a20: 2069 6e20 7265 706f 7274 5f70 6172 616d   in report_param
+00014a30: 733a 0a20 2020 2020 2020 2020 2020 2079  s:.            y
+00014a40: 5f61 7869 735f 6e61 6d65 7320 3d20 5b72  _axis_names = [r
+00014a50: 6570 6f72 745f 7061 7261 6d73 5b22 795f  eport_params["y_
+00014a60: 6178 6973 5f6e 616d 6522 5d5d 0a20 2020  axis_name"]].   
+00014a70: 2020 2020 2065 6c69 6620 6973 696e 7374       elif isinst
+00014a80: 616e 6365 2879 5f61 7869 735f 6e61 6d65  ance(y_axis_name
+00014a90: 732c 2073 7472 293a 0a20 2020 2020 2020  s, str):.       
+00014aa0: 2020 2020 2079 5f61 7869 735f 6e61 6d65       y_axis_name
+00014ab0: 7320 3d20 5b79 5f61 7869 735f 6e61 6d65  s = [y_axis_name
+00014ac0: 735d 0a20 2020 2020 2020 2065 6c73 653a  s].        else:
+00014ad0: 0a20 2020 2020 2020 2020 2020 2079 5f61  .            y_a
+00014ae0: 7869 735f 6e61 6d65 7320 3d20 5b5d 0a0a  xis_names = []..
+00014af0: 2020 2020 2020 2020 7661 6c75 6573 203d          values =
+00014b00: 2028 0a20 2020 2020 2020 2020 2020 205b   (.            [
+00014b10: 7620 666f 7220 7620 696e 2064 6174 615f  v for v in data_
+00014b20: 6d61 7070 696e 675f 746f 5f74 7570 6c65  mapping_to_tuple
+00014b30: 732e 6b65 7973 2829 2069 6620 7620 6e6f  s.keys() if v no
+00014b40: 7420 696e 2061 7865 735d 0a20 2020 2020  t in axes].     
+00014b50: 2020 2020 2020 2069 6620 7661 6c75 6573         if values
+00014b60: 2069 7320 4e6f 6e65 0a20 2020 2020 2020   is None.       
+00014b70: 2020 2020 2065 6c73 6520 7661 6c75 6573       else values
+00014b80: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
+00014b90: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
+00014ba0: 2873 6572 6965 735f 6f70 7469 6f6e 732c  (series_options,
+00014bb0: 2064 6963 7429 3a0a 2020 2020 2020 2020   dict):.        
+00014bc0: 2020 2020 7365 7269 6573 5f6f 7074 696f      series_optio
+00014bd0: 6e73 203d 205b 7365 7269 6573 5f6f 7074  ns = [series_opt
+00014be0: 696f 6e73 5d20 2a20 6c65 6e28 7661 6c75  ions] * len(valu
+00014bf0: 6573 290a 2020 2020 2020 2020 656c 6966  es).        elif
+00014c00: 206c 656e 2873 6572 6965 735f 6f70 7469   len(series_opti
+00014c10: 6f6e 7329 203c 206c 656e 2876 616c 7565  ons) < len(value
+00014c20: 7329 3a0a 2020 2020 2020 2020 2020 2020  s):.            
+00014c30: 7365 7269 6573 5f6f 7074 696f 6e73 203d  series_options =
+00014c40: 2073 6572 6965 735f 6f70 7469 6f6e 7320   series_options 
+00014c50: 2b20 5b73 6572 6965 735f 6f70 7469 6f6e  + [series_option
+00014c60: 735b 2d31 5d5d 202a 2028 0a20 2020 2020  s[-1]] * (.     
+00014c70: 2020 2020 2020 2020 2020 206c 656e 2876             len(v
+00014c80: 616c 7565 7329 202d 206c 656e 2873 6572  alues) - len(ser
+00014c90: 6965 735f 6f70 7469 6f6e 7329 0a20 2020  ies_options).   
+00014ca0: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+00014cb0: 2020 2065 6c69 6620 6c65 6e28 7365 7269     elif len(seri
+00014cc0: 6573 5f6f 7074 696f 6e73 2920 3e20 6c65  es_options) > le
+00014cd0: 6e28 7661 6c75 6573 293a 0a20 2020 2020  n(values):.     
+00014ce0: 2020 2020 2020 2073 6572 6965 735f 6f70         series_op
+00014cf0: 7469 6f6e 7320 3d20 7365 7269 6573 5f6f  tions = series_o
+00014d00: 7074 696f 6e73 5b3a 206c 656e 2876 616c  ptions[: len(val
+00014d10: 7565 7329 5d0a 0a20 2020 2020 2020 2065  ues)]..        e
+00014d20: 6368 6172 745f 6f70 7469 6f6e 735b 2273  chart_options["s
+00014d30: 6572 6965 7322 5d20 3d20 5b0a 2020 2020  eries"] = [.    
+00014d40: 2020 2020 2020 2020 6465 6570 5f75 7064          deep_upd
+00014d50: 6174 6528 0a20 2020 2020 2020 2020 2020  ate(.           
+00014d60: 2020 2020 207b 0a20 2020 2020 2020 2020       {.         
+00014d70: 2020 2020 2020 2020 2020 2022 6e61 6d65             "name
+00014d80: 223a 206e 616d 6520 6966 2069 7369 6e73  ": name if isins
+00014d90: 7461 6e63 6528 6e61 6d65 2c20 7374 7229  tance(name, str)
+00014da0: 2065 6c73 6520 2220 c397 2022 2e6a 6f69   else " .. ".joi
+00014db0: 6e28 6e61 6d65 292c 0a20 2020 2020 2020  n(name),.       
+00014dc0: 2020 2020 2020 2020 2020 2020 2022 6c61               "la
+00014dd0: 6265 6c22 3a20 7b22 7368 6f77 223a 2073  bel": {"show": s
+00014de0: 686f 775f 7661 6c75 6573 203d 3d20 2261  how_values == "a
+00014df0: 6c6c 2220 6f72 206e 616d 6520 696e 2073  ll" or name in s
+00014e00: 686f 775f 7661 6c75 6573 7d2c 0a20 2020  how_values},.   
+00014e10: 2020 2020 2020 2020 2020 2020 207d 2c0a               },.
+00014e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014e30: 7365 7269 6573 5f6f 7074 696f 6e73 5b69  series_options[i
+00014e40: 5d2c 0a20 2020 2020 2020 2020 2020 2029  ],.            )
+00014e50: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
+00014e60: 2069 2c20 6e61 6d65 2069 6e20 656e 756d   i, name in enum
+00014e70: 6572 6174 6528 7661 6c75 6573 290a 2020  erate(values).  
+00014e80: 2020 2020 2020 5d0a 0a20 2020 2020 2020        ]..       
+00014e90: 2066 6f72 2069 2c20 6178 6973 5f6f 7074   for i, axis_opt
+00014ea0: 696f 6e73 2069 6e20 656e 756d 6572 6174  ions in enumerat
+00014eb0: 6528 6563 6861 7274 5f6f 7074 696f 6e73  e(echart_options
+00014ec0: 5b22 7841 7869 7322 5d29 3a0a 2020 2020  ["xAxis"]):.    
+00014ed0: 2020 2020 2020 2020 6178 6973 5f6f 7074          axis_opt
+00014ee0: 696f 6e73 5b22 6e61 6d65 225d 203d 2078  ions["name"] = x
+00014ef0: 5f61 7869 735f 6e61 6d65 735b 695d 2069  _axis_names[i] i
+00014f00: 6620 6920 3c20 6c65 6e28 785f 6178 6973  f i < len(x_axis
+00014f10: 5f6e 616d 6573 2920 656c 7365 204e 6f6e  _names) else Non
+00014f20: 650a 2020 2020 2020 2020 2020 2020 6966  e.            if
+00014f30: 2061 7869 735f 6f70 7469 6f6e 735b 226e   axis_options["n
+00014f40: 616d 6522 5d20 616e 6420 226e 616d 6547  ame"] and "nameG
+00014f50: 6170 2220 6e6f 7420 696e 2061 7869 735f  ap" not in axis_
+00014f60: 6f70 7469 6f6e 733a 0a20 2020 2020 2020  options:.       
+00014f70: 2020 2020 2020 2020 2061 7869 735f 6f70           axis_op
+00014f80: 7469 6f6e 735b 226e 616d 6547 6170 225d  tions["nameGap"]
+00014f90: 203d 2033 320a 0a20 2020 2020 2020 2066   = 32..        f
+00014fa0: 6f72 2069 2c20 6178 6973 5f6f 7074 696f  or i, axis_optio
+00014fb0: 6e73 2069 6e20 656e 756d 6572 6174 6528  ns in enumerate(
+00014fc0: 6563 6861 7274 5f6f 7074 696f 6e73 5b22  echart_options["
+00014fd0: 7941 7869 7322 5d29 3a0a 2020 2020 2020  yAxis"]):.      
+00014fe0: 2020 2020 2020 6178 6973 5f6f 7074 696f        axis_optio
+00014ff0: 6e73 5b22 6e61 6d65 225d 203d 2079 5f61  ns["name"] = y_a
+00015000: 7869 735f 6e61 6d65 735b 695d 2069 6620  xis_names[i] if 
+00015010: 6920 3c20 6c65 6e28 795f 6178 6973 5f6e  i < len(y_axis_n
+00015020: 616d 6573 2920 656c 7365 204e 6f6e 650a  ames) else None.
+00015030: 2020 2020 2020 2020 2020 2020 6966 2061              if a
+00015040: 7869 735f 6f70 7469 6f6e 735b 226e 616d  xis_options["nam
+00015050: 6522 5d20 616e 6420 226e 616d 6547 6170  e"] and "nameGap
+00015060: 2220 6e6f 7420 696e 2061 7869 735f 6f70  " not in axis_op
+00015070: 7469 6f6e 733a 0a20 2020 2020 2020 2020  tions:.         
+00015080: 2020 2020 2020 2061 7869 735f 6f70 7469         axis_opti
+00015090: 6f6e 735b 226e 616d 6547 6170 225d 203d  ons["nameGap"] =
+000150a0: 202d 3234 0a20 2020 2020 2020 2020 2020   -24.           
+000150b0: 2020 2020 2061 7869 735f 6f70 7469 6f6e       axis_option
+000150c0: 735b 226f 6666 7365 7422 5d20 3d20 3336  s["offset"] = 36
+000150d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000150e0: 2065 6368 6172 745f 6f70 7469 6f6e 735b   echart_options[
+000150f0: 2267 7269 6422 5d5b 226c 6566 7422 5d20  "grid"]["left"] 
+00015100: 3d20 2234 2522 0a20 2020 2020 2020 2020  = "4%".         
+00015110: 2020 2020 2020 2061 7869 735f 6f70 7469         axis_opti
+00015120: 6f6e 735b 2261 7869 7354 6963 6b22 5d20  ons["axisTick"] 
+00015130: 3d20 7b22 7368 6f77 223a 2046 616c 7365  = {"show": False
+00015140: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
+00015150: 2020 6178 6973 5f6f 7074 696f 6e73 5b22    axis_options["
+00015160: 6178 6973 4c69 6e65 225d 203d 207b 2273  axisLine"] = {"s
+00015170: 686f 7722 3a20 4661 6c73 657d 0a0a 2020  how": False}..  
+00015180: 2020 2020 2020 6177 6169 7420 7365 6c66        await self
+00015190: 2e5f 6372 6561 7465 5f65 6368 6172 7428  ._create_echart(
+000151a0: 0a20 2020 2020 2020 2020 2020 206f 7264  .            ord
+000151b0: 6572 3d6f 7264 6572 2c0a 2020 2020 2020  er=order,.      
+000151c0: 2020 2020 2020 6f70 7469 6f6e 733d 6563        options=ec
+000151d0: 6861 7274 5f6f 7074 696f 6e73 2c0a 2020  hart_options,.  
+000151e0: 2020 2020 2020 2020 2020 6461 7461 5f6d            data_m
+000151f0: 6170 7069 6e67 5f74 6f5f 7475 706c 6573  apping_to_tuples
+00015200: 3d64 6174 615f 6d61 7070 696e 675f 746f  =data_mapping_to
+00015210: 5f74 7570 6c65 732c 0a20 2020 2020 2020  _tuples,.       
+00015220: 2020 2020 2066 6965 6c64 733d 6178 6573       fields=axes
+00015230: 202b 2076 616c 7565 732c 0a20 2020 2020   + values,.     
+00015240: 2020 2020 2020 202a 2a72 6570 6f72 745f         **report_
+00015250: 7061 7261 6d73 2c0a 2020 2020 2020 2020  params,.        
+00015260: 290a 0a20 2020 2040 6164 645f 746f 5f67  )..    @add_to_g
+00015270: 656e 6572 616c 5f61 7379 6e63 5f67 726f  eneral_async_gro
+00015280: 7570 0a20 2020 2061 7379 6e63 2064 6566  up.    async def
+00015290: 2066 7265 655f 6563 6861 7274 7328 0a20   free_echarts(. 
+000152a0: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
+000152b0: 2020 2020 2064 6174 613a 204f 7074 696f       data: Optio
+000152c0: 6e61 6c5b 556e 696f 6e5b 7374 722c 2044  nal[Union[str, D
+000152d0: 6174 6146 7261 6d65 2c20 6c69 7374 5b64  ataFrame, list[d
+000152e0: 6963 745d 5d5d 203d 204e 6f6e 652c 0a20  ict]]] = None,. 
+000152f0: 2020 2020 2020 206f 7074 696f 6e73 3a20         options: 
+00015300: 4f70 7469 6f6e 616c 5b64 6963 745d 203d  Optional[dict] =
+00015310: 204e 6f6e 652c 0a20 2020 2020 2020 2072   None,.        r
+00015320: 6177 5f6f 7074 696f 6e73 3a20 4f70 7469  aw_options: Opti
+00015330: 6f6e 616c 5b73 7472 5d20 3d20 4e6f 6e65  onal[str] = None
+00015340: 2c0a 2020 2020 2020 2020 6f72 6465 723a  ,.        order:
+00015350: 204f 7074 696f 6e61 6c5b 696e 745d 203d   Optional[int] =
+00015360: 204e 6f6e 652c 0a20 2020 2020 2020 2074   None,.        t
+00015370: 6974 6c65 3a20 4f70 7469 6f6e 616c 5b73  itle: Optional[s
+00015380: 7472 5d20 3d20 4e6f 6e65 2c0a 2020 2020  tr] = None,.    
+00015390: 2020 2020 726f 7773 5f73 697a 653a 204f      rows_size: O
+000153a0: 7074 696f 6e61 6c5b 696e 745d 203d 204e  ptional[int] = N
+000153b0: 6f6e 652c 0a20 2020 2020 2020 2063 6f6c  one,.        col
+000153c0: 735f 7369 7a65 3a20 4f70 7469 6f6e 616c  s_size: Optional
+000153d0: 5b69 6e74 5d20 3d20 4e6f 6e65 2c0a 2020  [int] = None,.  
+000153e0: 2020 2020 2020 7061 6464 696e 673a 204f        padding: O
+000153f0: 7074 696f 6e61 6c5b 7374 725d 203d 204e  ptional[str] = N
+00015400: 6f6e 652c 0a20 2020 2020 2020 2066 6965  one,.        fie
+00015410: 6c64 733a 204f 7074 696f 6e61 6c5b 6c69  lds: Optional[li
+00015420: 7374 5d20 3d20 4e6f 6e65 2c0a 2020 2020  st] = None,.    
+00015430: 2020 2020 6461 7461 5f69 735f 6e6f 745f      data_is_not_
+00015440: 6466 3a20 626f 6f6c 203d 2046 616c 7365  df: bool = False
+00015450: 2c0a 2020 2020 293a 0a20 2020 2020 2020  ,.    ):.       
+00015460: 2022 2222 0a20 2020 2020 2020 2043 7265   """.        Cre
+00015470: 6174 6520 616e 2065 6368 6172 7473 2063  ate an echarts c
+00015480: 6861 7274 2077 6974 6820 6375 7374 6f6d  hart with custom
+00015490: 206f 7074 696f 6e73 2e0a 2020 2020 2020   options..      
+000154a0: 2020 3a70 6172 616d 2064 6174 613a 2074    :param data: t
+000154b0: 6865 2064 6174 6120 6f66 2074 6865 2063  he data of the c
+000154c0: 6861 7274 0a20 2020 2020 2020 203a 7061  hart.        :pa
+000154d0: 7261 6d20 6f70 7469 6f6e 733a 2074 6865  ram options: the
+000154e0: 206f 7074 696f 6e73 206f 6620 7468 6520   options of the 
+000154f0: 6368 6172 740a 2020 2020 2020 2020 3a70  chart.        :p
+00015500: 6172 616d 2072 6177 5f6f 7074 696f 6e73  aram raw_options
+00015510: 3a20 7468 6520 7261 7720 6f70 7469 6f6e  : the raw option
+00015520: 7320 6f66 2074 6865 2063 6861 7274 0a20  s of the chart. 
+00015530: 2020 2020 2020 203a 7061 7261 6d20 6f72         :param or
+00015540: 6465 723a 2074 6865 206f 7264 6572 206f  der: the order o
+00015550: 6620 7468 6520 6368 6172 7420 696e 2074  f the chart in t
+00015560: 6865 2064 6173 6862 6f61 7264 0a20 2020  he dashboard.   
+00015570: 2020 2020 203a 7061 7261 6d20 7469 746c       :param titl
+00015580: 653a 2074 6865 2074 6974 6c65 206f 6620  e: the title of 
+00015590: 7468 6520 6368 6172 740a 2020 2020 2020  the chart.      
+000155a0: 2020 3a70 6172 616d 2072 6f77 735f 7369    :param rows_si
+000155b0: 7a65 3a20 7468 6520 726f 7773 2073 697a  ze: the rows siz
+000155c0: 6520 6f66 2074 6865 2063 6861 7274 0a20  e of the chart. 
+000155d0: 2020 2020 2020 203a 7061 7261 6d20 636f         :param co
+000155e0: 6c73 5f73 697a 653a 2074 6865 2063 6f6c  ls_size: the col
+000155f0: 756d 6e73 2073 697a 6520 6f66 2074 6865  umns size of the
+00015600: 2063 6861 7274 0a20 2020 2020 2020 203a   chart.        :
+00015610: 7061 7261 6d20 7061 6464 696e 673a 2074  param padding: t
+00015620: 6865 2070 6164 6469 6e67 206f 6620 7468  he padding of th
+00015630: 6520 6368 6172 740a 2020 2020 2020 2020  e chart.        
+00015640: 3a70 6172 616d 2066 6965 6c64 733a 2074  :param fields: t
+00015650: 6865 2066 6965 6c64 7320 6f66 2074 6865  he fields of the
+00015660: 2063 6861 7274 0a20 2020 2020 2020 203a   chart.        :
+00015670: 7061 7261 6d20 6461 7461 5f69 735f 6e6f  param data_is_no
+00015680: 745f 6466 3a20 7768 6574 6865 7220 7468  t_df: whether th
+00015690: 6520 6461 7461 2069 7320 6e6f 7420 6120  e data is not a 
+000156a0: 6461 7461 6672 616d 650a 2020 2020 2020  dataframe.      
+000156b0: 2020 2222 220a 2020 2020 2020 2020 6966    """.        if
+000156c0: 206e 6f74 206f 7074 696f 6e73 2061 6e64   not options and
+000156d0: 206e 6f74 2072 6177 5f6f 7074 696f 6e73   not raw_options
+000156e0: 3a0a 2020 2020 2020 2020 2020 2020 6c6f  :.            lo
+000156f0: 675f 6572 726f 7228 0a20 2020 2020 2020  g_error(.       
+00015700: 2020 2020 2020 2020 206c 6f67 6765 722c           logger,
+00015710: 2022 4569 7468 6572 206f 7074 696f 6e73   "Either options
+00015720: 206f 7220 7261 775f 6f70 7469 6f6e 7320   or raw_options 
+00015730: 6d75 7374 2062 6520 7072 6f76 6964 6564  must be provided
+00015740: 222c 2056 616c 7565 4572 726f 720a 2020  ", ValueError.  
+00015750: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+00015760: 2020 2020 6966 206f 7074 696f 6e73 2061      if options a
+00015770: 6e64 206e 6f74 2069 7369 6e73 7461 6e63  nd not isinstanc
+00015780: 6528 6461 7461 2c20 4461 7461 4672 616d  e(data, DataFram
+00015790: 6529 2061 6e64 2064 6174 6120 6973 204e  e) and data is N
+000157a0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+000157b0: 206c 6f67 5f65 7272 6f72 280a 2020 2020   log_error(.    
+000157c0: 2020 2020 2020 2020 2020 2020 6c6f 6767              logg
+000157d0: 6572 2c20 2264 6174 6120 6d75 7374 2062  er, "data must b
+000157e0: 6520 7072 6f76 6964 6564 2077 6865 6e20  e provided when 
+000157f0: 6f70 7469 6f6e 7320 6973 2070 726f 7669  options is provi
+00015800: 6465 6422 2c20 4461 7461 4572 726f 720a  ded", DataError.
+00015810: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+00015820: 2020 2020 2020 6966 206f 7074 696f 6e73        if options
+00015830: 2061 6e64 2072 6177 5f6f 7074 696f 6e73   and raw_options
+00015840: 3a0a 2020 2020 2020 2020 2020 2020 6c6f  :.            lo
+00015850: 675f 6572 726f 7228 0a20 2020 2020 2020  g_error(.       
+00015860: 2020 2020 2020 2020 206c 6f67 6765 722c           logger,
+00015870: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00015880: 2022 4f6e 6c79 206f 6e65 206f 6620 6f70   "Only one of op
+00015890: 7469 6f6e 7320 616e 6420 7261 775f 6f70  tions and raw_op
+000158a0: 7469 6f6e 7320 6361 6e20 6265 2070 726f  tions can be pro
+000158b0: 7669 6465 6422 2c0a 2020 2020 2020 2020  vided",.        
+000158c0: 2020 2020 2020 2020 5661 6c75 6545 7272          ValueErr
+000158d0: 6f72 2c0a 2020 2020 2020 2020 2020 2020  or,.            
+000158e0: 290a 0a20 2020 2020 2020 2069 6620 7261  )..        if ra
+000158f0: 775f 6f70 7469 6f6e 733a 0a20 2020 2020  w_options:.     
+00015900: 2020 2020 2020 206f 7074 696f 6e73 203d         options =
+00015910: 2074 7261 6e73 666f 726d 5f64 6963 745f   transform_dict_
+00015920: 6a73 5f74 6f5f 7079 2872 6177 5f6f 7074  js_to_py(raw_opt
+00015930: 696f 6e73 290a 2020 2020 2020 2020 2020  ions).          
+00015940: 2020 6461 7461 203d 2072 6574 7269 6576    data = retriev
+00015950: 655f 6461 7461 5f66 726f 6d5f 6f70 7469  e_data_from_opti
+00015960: 6f6e 7328 6f70 7469 6f6e 7329 0a20 2020  ons(options).   
+00015970: 2020 2020 2020 2020 206f 7074 696f 6e73           options
+00015980: 5b22 6461 7461 7365 7422 5d20 3d20 7b22  ["dataset"] = {"
+00015990: 736f 7572 6365 223a 2022 2373 6574 5f64  source": "#set_d
+000159a0: 6174 6123 227d 0a20 2020 2020 2020 2020  ata#"}.         
+000159b0: 2020 2066 6965 6c64 7320 3d20 5b6c 6973     fields = [lis
+000159c0: 7428 6461 7461 5b30 5d2e 6b65 7973 2829  t(data[0].keys()
+000159d0: 295d 0a20 2020 2020 2020 2065 6c73 653a  )].        else:
+000159e0: 0a20 2020 2020 2020 2020 2020 206f 7074  .            opt
+000159f0: 696f 6e73 203d 2064 6565 7063 6f70 7928  ions = deepcopy(
+00015a00: 6f70 7469 6f6e 7329 0a0a 2020 2020 2020  options)..      
+00015a10: 2020 6177 6169 7420 7365 6c66 2e5f 6372    await self._cr
+00015a20: 6561 7465 5f65 6368 6172 7428 0a20 2020  eate_echart(.   
+00015a30: 2020 2020 2020 2020 206f 7264 6572 3d6f           order=o
+00015a40: 7264 6572 2c0a 2020 2020 2020 2020 2020  rder,.          
+00015a50: 2020 6461 7461 5f6d 6170 7069 6e67 5f74    data_mapping_t
+00015a60: 6f5f 7475 706c 6573 3d61 7761 6974 2073  o_tuples=await s
+00015a70: 656c 662e 5f63 686f 6f73 655f 6461 7461  elf._choose_data
+00015a80: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00015a90: 2020 6f72 6465 722c 2064 6174 612c 2064    order, data, d
+00015aa0: 756d 705f 7768 6f6c 653d 6461 7461 5f69  ump_whole=data_i
+00015ab0: 735f 6e6f 745f 6466 0a20 2020 2020 2020  s_not_df.       
+00015ac0: 2020 2020 2029 2c0a 2020 2020 2020 2020       ),.        
+00015ad0: 2020 2020 6669 656c 6473 3d66 6965 6c64      fields=field
+00015ae0: 732c 0a20 2020 2020 2020 2020 2020 206f  s,.            o
+00015af0: 7074 696f 6e73 3d6f 7074 696f 6e73 2c0a  ptions=options,.
+00015b00: 2020 2020 2020 2020 2020 2020 7469 746c              titl
+00015b10: 653d 7469 746c 652c 0a20 2020 2020 2020  e=title,.       
+00015b20: 2020 2020 2072 6f77 735f 7369 7a65 3d72       rows_size=r
+00015b30: 6f77 735f 7369 7a65 2c0a 2020 2020 2020  ows_size,.      
+00015b40: 2020 2020 2020 636f 6c73 5f73 697a 653d        cols_size=
+00015b50: 636f 6c73 5f73 697a 652c 0a20 2020 2020  cols_size,.     
+00015b60: 2020 2020 2020 2070 6164 6469 6e67 3d70         padding=p
+00015b70: 6164 6469 6e67 2c0a 2020 2020 2020 2020  adding,.        
+00015b80: 290a 0a20 2020 2023 2045 4368 6172 7473  )..    # ECharts
+00015b90: 0a20 2020 206c 696e 6520 3d20 6164 645f  .    line = add_
+00015ba0: 746f 5f67 656e 6572 616c 5f61 7379 6e63  to_general_async
+00015bb0: 5f67 726f 7570 286c 696e 655f 6368 6172  _group(line_char
+00015bc0: 7429 0a20 2020 2062 6172 203d 2061 6464  t).    bar = add
+00015bd0: 5f74 6f5f 6765 6e65 7261 6c5f 6173 796e  _to_general_asyn
+00015be0: 635f 6772 6f75 7028 6261 725f 6368 6172  c_group(bar_char
+00015bf0: 7429 0a20 2020 2073 7461 636b 6564 5f62  t).    stacked_b
+00015c00: 6172 203d 2061 6464 5f74 6f5f 6765 6e65  ar = add_to_gene
+00015c10: 7261 6c5f 6173 796e 635f 6772 6f75 7028  ral_async_group(
+00015c20: 7374 6163 6b65 645f 6261 725f 6368 6172  stacked_bar_char
+00015c30: 7429 0a20 2020 2061 7265 6120 3d20 6164  t).    area = ad
+00015c40: 645f 746f 5f67 656e 6572 616c 5f61 7379  d_to_general_asy
+00015c50: 6e63 5f67 726f 7570 2861 7265 615f 6368  nc_group(area_ch
+00015c60: 6172 7429 0a20 2020 2073 7461 636b 6564  art).    stacked
+00015c70: 5f61 7265 6120 3d20 6164 645f 746f 5f67  _area = add_to_g
+00015c80: 656e 6572 616c 5f61 7379 6e63 5f67 726f  eneral_async_gro
+00015c90: 7570 2873 7461 636b 6564 5f61 7265 615f  up(stacked_area_
+00015ca0: 6368 6172 7429 0a20 2020 2073 6361 7474  chart).    scatt
+00015cb0: 6572 203d 2061 6464 5f74 6f5f 6765 6e65  er = add_to_gene
+00015cc0: 7261 6c5f 6173 796e 635f 6772 6f75 7028  ral_async_group(
+00015cd0: 7363 6174 7465 725f 6368 6172 7429 0a20  scatter_chart). 
+00015ce0: 2020 2068 6f72 697a 6f6e 7461 6c5f 6261     horizontal_ba
+00015cf0: 7220 3d20 6164 645f 746f 5f67 656e 6572  r = add_to_gener
+00015d00: 616c 5f61 7379 6e63 5f67 726f 7570 2868  al_async_group(h
+00015d10: 6f72 697a 6f6e 7461 6c5f 6261 725f 6368  orizontal_bar_ch
+00015d20: 6172 7429 0a20 2020 2073 7461 636b 6564  art).    stacked
+00015d30: 5f68 6f72 697a 6f6e 7461 6c5f 6261 7220  _horizontal_bar 
+00015d40: 3d20 6164 645f 746f 5f67 656e 6572 616c  = add_to_general
+00015d50: 5f61 7379 6e63 5f67 726f 7570 2873 7461  _async_group(sta
+00015d60: 636b 6564 5f68 6f72 697a 6f6e 7461 6c5f  cked_horizontal_
+00015d70: 6261 725f 6368 6172 7429 0a20 2020 207a  bar_chart).    z
+00015d80: 6572 6f5f 6365 6e74 6572 6564 5f62 6172  ero_centered_bar
+00015d90: 203d 2061 6464 5f74 6f5f 6765 6e65 7261   = add_to_genera
+00015da0: 6c5f 6173 796e 635f 6772 6f75 7028 7a65  l_async_group(ze
+00015db0: 726f 5f63 656e 7465 7265 645f 6261 725f  ro_centered_bar_
+00015dc0: 6368 6172 7429 0a20 2020 2066 756e 6e65  chart).    funne
+00015dd0: 6c20 3d20 6164 645f 746f 5f67 656e 6572  l = add_to_gener
+00015de0: 616c 5f61 7379 6e63 5f67 726f 7570 2866  al_async_group(f
+00015df0: 756e 6e65 6c5f 6368 6172 7429 0a20 2020  unnel_chart).   
+00015e00: 2074 7265 6520 3d20 6164 645f 746f 5f67   tree = add_to_g
+00015e10: 656e 6572 616c 5f61 7379 6e63 5f67 726f  eneral_async_gro
+00015e20: 7570 2874 7265 655f 6368 6172 7429 0a20  up(tree_chart). 
+00015e30: 2020 2072 6164 6172 203d 2061 6464 5f74     radar = add_t
+00015e40: 6f5f 6765 6e65 7261 6c5f 6173 796e 635f  o_general_async_
+00015e50: 6772 6f75 7028 7261 6461 725f 6368 6172  group(radar_char
+00015e60: 7429 0a20 2020 2070 6965 203d 2061 6464  t).    pie = add
+00015e70: 5f74 6f5f 6765 6e65 7261 6c5f 6173 796e  _to_general_asyn
+00015e80: 635f 6772 6f75 7028 7069 655f 6368 6172  c_group(pie_char
+00015e90: 7429 0a20 2020 2064 6f75 6768 6e75 7420  t).    doughnut 
+00015ea0: 3d20 6164 645f 746f 5f67 656e 6572 616c  = add_to_general
+00015eb0: 5f61 7379 6e63 5f67 726f 7570 2864 6f75  _async_group(dou
+00015ec0: 6768 6e75 745f 6368 6172 7429 0a20 2020  ghnut_chart).   
+00015ed0: 2072 6f73 6520 3d20 6164 645f 746f 5f67   rose = add_to_g
+00015ee0: 656e 6572 616c 5f61 7379 6e63 5f67 726f  eneral_async_gro
+00015ef0: 7570 2872 6f73 655f 6368 6172 7429 0a20  up(rose_chart). 
+00015f00: 2020 2073 756e 6275 7273 7420 3d20 6164     sunburst = ad
+00015f10: 645f 746f 5f67 656e 6572 616c 5f61 7379  d_to_general_asy
+00015f20: 6e63 5f67 726f 7570 2873 756e 6275 7273  nc_group(sunburs
+00015f30: 745f 6368 6172 7429 0a20 2020 2074 7265  t_chart).    tre
+00015f40: 656d 6170 203d 2061 6464 5f74 6f5f 6765  emap = add_to_ge
+00015f50: 6e65 7261 6c5f 6173 796e 635f 6772 6f75  neral_async_grou
+00015f60: 7028 7472 6565 6d61 705f 6368 6172 7429  p(treemap_chart)
+00015f70: 0a20 2020 2073 616e 6b65 7920 3d20 6164  .    sankey = ad
+00015f80: 645f 746f 5f67 656e 6572 616c 5f61 7379  d_to_general_asy
+00015f90: 6e63 5f67 726f 7570 2873 616e 6b65 795f  nc_group(sankey_
+00015fa0: 6368 6172 7429 0a20 2020 2068 6561 746d  chart).    heatm
+00015fb0: 6170 203d 2061 6464 5f74 6f5f 6765 6e65  ap = add_to_gene
+00015fc0: 7261 6c5f 6173 796e 635f 6772 6f75 7028  ral_async_group(
+00015fd0: 6865 6174 6d61 705f 6368 6172 7429 0a20  heatmap_chart). 
+00015fe0: 2020 2070 7265 6469 6374 6976 655f 6c69     predictive_li
+00015ff0: 6e65 203d 2061 6464 5f74 6f5f 6765 6e65  ne = add_to_gene
+00016000: 7261 6c5f 6173 796e 635f 6772 6f75 7028  ral_async_group(
+00016010: 7072 6564 6963 7469 7665 5f6c 696e 655f  predictive_line_
+00016020: 6368 6172 7429 0a20 2020 2073 7065 6564  chart).    speed
+00016030: 5f67 6175 6765 203d 2061 6464 5f74 6f5f  _gauge = add_to_
+00016040: 6765 6e65 7261 6c5f 6173 796e 635f 6772  general_async_gr
+00016050: 6f75 7028 7370 6565 645f 6761 7567 655f  oup(speed_gauge_
+00016060: 6368 6172 7429 0a20 2020 2073 6869 6d6f  chart).    shimo
+00016070: 6b75 5f67 6175 6765 203d 2061 6464 5f74  ku_gauge = add_t
+00016080: 6f5f 6765 6e65 7261 6c5f 6173 796e 635f  o_general_async_
+00016090: 6772 6f75 7028 7368 696d 6f6b 755f 6761  group(shimoku_ga
+000160a0: 7567 655f 6368 6172 7429 0a20 2020 2073  uge_chart).    s
+000160b0: 6869 6d6f 6b75 5f67 6175 6765 735f 6772  himoku_gauges_gr
+000160c0: 6f75 7020 3d20 6164 645f 746f 5f67 656e  oup = add_to_gen
+000160d0: 6572 616c 5f61 7379 6e63 5f67 726f 7570  eral_async_group
+000160e0: 2873 6869 6d6f 6b75 5f67 6175 6765 735f  (shimoku_gauges_
+000160f0: 6772 6f75 7029 0a20 2020 2067 6175 6765  group).    gauge
+00016100: 5f69 6e64 6963 6174 6f72 203d 2061 6464  _indicator = add
+00016110: 5f74 6f5f 6765 6e65 7261 6c5f 6173 796e  _to_general_asyn
+00016120: 635f 6772 6f75 7028 6761 7567 655f 696e  c_group(gauge_in
+00016130: 6469 6361 746f 7229 0a20 2020 2074 6f70  dicator).    top
+00016140: 5f62 6f74 746f 6d5f 6172 6561 203d 2061  _bottom_area = a
+00016150: 6464 5f74 6f5f 6765 6e65 7261 6c5f 6173  dd_to_general_as
+00016160: 796e 635f 6772 6f75 7028 746f 705f 626f  ync_group(top_bo
+00016170: 7474 6f6d 5f61 7265 615f 6368 6172 7473  ttom_area_charts
+00016180: 290a 2020 2020 746f 705f 626f 7474 6f6d  ).    top_bottom
+00016190: 5f6c 696e 6520 3d20 6164 645f 746f 5f67  _line = add_to_g
+000161a0: 656e 6572 616c 5f61 7379 6e63 5f67 726f  eneral_async_gro
+000161b0: 7570 2874 6f70 5f62 6f74 746f 6d5f 6c69  up(top_bottom_li
+000161c0: 6e65 5f63 6861 7274 7329 0a20 2020 206c  ne_charts).    l
+000161d0: 696e 655f 7769 7468 5f63 6f6e 6669 6465  ine_with_confide
+000161e0: 6e63 655f 6172 6561 203d 2061 6464 5f74  nce_area = add_t
+000161f0: 6f5f 6765 6e65 7261 6c5f 6173 796e 635f  o_general_async_
+00016200: 6772 6f75 7028 0a20 2020 2020 2020 206c  group(.        l
+00016210: 696e 655f 7769 7468 5f63 6f6e 6669 6465  ine_with_confide
+00016220: 6e63 655f 6172 6561 5f63 6861 7274 0a20  nce_area_chart. 
+00016230: 2020 2029 0a20 2020 2073 6361 7474 6572     ).    scatter
+00016240: 5f77 6974 685f 6566 6665 6374 203d 2061  _with_effect = a
+00016250: 6464 5f74 6f5f 6765 6e65 7261 6c5f 6173  dd_to_general_as
+00016260: 796e 635f 6772 6f75 7028 7363 6174 7465  ync_group(scatte
+00016270: 725f 7769 7468 5f65 6666 6563 745f 6368  r_with_effect_ch
+00016280: 6172 7429 0a20 2020 2077 6174 6572 6661  art).    waterfa
+00016290: 6c6c 203d 2061 6464 5f74 6f5f 6765 6e65  ll = add_to_gene
+000162a0: 7261 6c5f 6173 796e 635f 6772 6f75 7028  ral_async_group(
+000162b0: 7761 7465 7266 616c 6c5f 6368 6172 7429  waterfall_chart)
+000162c0: 0a20 2020 206c 696e 655f 616e 645f 6261  .    line_and_ba
+000162d0: 725f 6368 6172 7473 203d 2061 6464 5f74  r_charts = add_t
+000162e0: 6f5f 6765 6e65 7261 6c5f 6173 796e 635f  o_general_async_
+000162f0: 6772 6f75 7028 6c69 6e65 5f61 6e64 5f62  group(line_and_b
+00016300: 6172 5f63 6861 7274 7329 0a20 2020 2073  ar_charts).    s
+00016310: 6567 6d65 6e74 6564 5f6c 696e 6520 3d20  egmented_line = 
+00016320: 6164 645f 746f 5f67 656e 6572 616c 5f61  add_to_general_a
+00016330: 7379 6e63 5f67 726f 7570 2873 6567 6d65  sync_group(segme
+00016340: 6e74 6564 5f6c 696e 655f 6368 6172 7429  nted_line_chart)
+00016350: 0a20 2020 206d 6172 6b65 645f 6c69 6e65  .    marked_line
+00016360: 203d 2061 6464 5f74 6f5f 6765 6e65 7261   = add_to_genera
+00016370: 6c5f 6173 796e 635f 6772 6f75 7028 6d61  l_async_group(ma
+00016380: 726b 6564 5f6c 696e 655f 6368 6172 7429  rked_line_chart)
+00016390: 0a20 2020 2073 6567 6d65 6e74 6564 5f61  .    segmented_a
+000163a0: 7265 6120 3d20 6164 645f 746f 5f67 656e  rea = add_to_gen
+000163b0: 6572 616c 5f61 7379 6e63 5f67 726f 7570  eral_async_group
+000163c0: 2873 6567 6d65 6e74 6564 5f61 7265 615f  (segmented_area_
+000163d0: 6368 6172 7429 0a0a 2020 2020 2320 4265  chart)..    # Be
+000163e0: 6e74 6f62 6f78 2063 6861 7274 7320 6465  ntobox charts de
+000163f0: 6669 6e65 6420 696e 2074 6865 2062 656e  fined in the ben
+00016400: 746f 626f 785f 6368 6172 7473 2e70 7920  tobox_charts.py 
+00016410: 6669 6c65 0a20 2020 2069 6e66 6f67 7261  file.    infogra
+00016420: 7068 6963 735f 7465 7874 5f62 7562 626c  phics_text_bubbl
+00016430: 6520 3d20 6164 645f 746f 5f67 656e 6572  e = add_to_gener
+00016440: 616c 5f61 7379 6e63 5f67 726f 7570 2869  al_async_group(i
+00016450: 6e66 6f67 7261 7068 6963 735f 7465 7874  nfographics_text
+00016460: 5f62 7562 626c 6529 0a20 2020 2063 6861  _bubble).    cha
+00016470: 7274 5f61 6e64 5f6d 6f64 616c 5f62 7574  rt_and_modal_but
+00016480: 746f 6e20 3d20 6164 645f 746f 5f67 656e  ton = add_to_gen
+00016490: 6572 616c 5f61 7379 6e63 5f67 726f 7570  eral_async_group
+000164a0: 2863 6861 7274 5f61 6e64 5f6d 6f64 616c  (chart_and_modal
+000164b0: 5f62 7574 746f 6e29 0a20 2020 2063 6861  _button).    cha
+000164c0: 7274 5f61 6e64 5f69 6e64 6963 6174 6f72  rt_and_indicator
+000164d0: 7320 3d20 6164 645f 746f 5f67 656e 6572  s = add_to_gener
+000164e0: 616c 5f61 7379 6e63 5f67 726f 7570 2863  al_async_group(c
+000164f0: 6861 7274 5f61 6e64 5f69 6e64 6963 6174  hart_and_indicat
+00016500: 6f72 7329 0a20 2020 2069 6e64 6963 6174  ors).    indicat
+00016510: 6f72 735f 7769 7468 5f68 6561 6465 7220  ors_with_header 
+00016520: 3d20 6164 645f 746f 5f67 656e 6572 616c  = add_to_general
+00016530: 5f61 7379 6e63 5f67 726f 7570 2869 6e64  _async_group(ind
+00016540: 6963 6174 6f72 735f 7769 7468 5f68 6561  icators_with_hea
+00016550: 6465 7229 0a20 2020 206c 696e 655f 7769  der).    line_wi
+00016560: 7468 5f73 756d 6d61 7279 203d 2061 6464  th_summary = add
+00016570: 5f74 6f5f 6765 6e65 7261 6c5f 6173 796e  _to_general_asyn
+00016580: 635f 6772 6f75 7028 6c69 6e65 5f77 6974  c_group(line_wit
+00016590: 685f 7375 6d6d 6172 7929 0a              h_summary).
```

### Comparing `shimoku-browser-2.3.1/src/shimoku/plt/utils.py` & `shimoku_browser-2.4.0/src/shimoku/plt/utils.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/src/shimoku/utils.py` & `shimoku_browser-2.4.0/src/shimoku/utils.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/src/shimoku_browser.egg-info/PKG-INFO` & `shimoku_browser-2.4.0/src/shimoku_browser.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shimoku-browser
-Version: 2.3.1
+Version: 2.4.0
 Summary: Shimoku enables you to build Data Products in just hours and allows you to create Predictive Analytics Products with Artificial Intelligence capabilities.
 Home-page: https://github.com/shimoku-tech/shimoku-api-python
 Author: Shimoku
 Author-email: contact@shimoku.com
 License: MIT
 Project-URL: Documentation, https://docs.shimoku.com/
 Platform: any
```

### Comparing `shimoku-browser-2.3.1/src/shimoku_browser.egg-info/SOURCES.txt` & `shimoku_browser-2.4.0/src/shimoku_browser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/tests/Jupyter_notebook_test.ipynb` & `shimoku_browser-2.4.0/tests/Jupyter_notebook_test.ipynb`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/tests/mockable_tests/correct_action_scripts/correct_action.py` & `shimoku_browser-2.4.0/tests/mockable_tests/correct_action_scripts/correct_action.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/tests/mockable_tests/mock_classes.py` & `shimoku_browser-2.4.0/tests/mockable_tests/mock_classes.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/tests/mockable_tests/test_actions.py` & `shimoku_browser-2.4.0/tests/mockable_tests/test_actions.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/tests/mockable_tests/test_activity_metadata_api.py` & `shimoku_browser-2.4.0/tests/mockable_tests/test_activity_metadata_api.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/tests/mockable_tests/test_app_metadata_api.py` & `shimoku_browser-2.4.0/tests/mockable_tests/test_app_metadata_api.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/tests/mockable_tests/test_business_metadata_api.py` & `shimoku_browser-2.4.0/tests/mockable_tests/test_business_metadata_api.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/tests/mockable_tests/test_code_generation.py` & `shimoku_browser-2.4.0/tests/mockable_tests/test_code_generation.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/tests/mockable_tests/test_dashboard_metadata_api.py` & `shimoku_browser-2.4.0/tests/mockable_tests/test_dashboard_metadata_api.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api.py` & `shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/annotation_chart.py` & `shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/annotation_chart.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/bar_and_line_chart.py` & `shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/bar_and_line_chart.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/bentobox.py` & `shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/bentobox.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/chart_and_indicators.py` & `shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/chart_and_indicators.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/data/annotation_chart.py` & `shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/data/annotation_chart.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/data/bar_and_line.py` & `shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/data/bar_and_line.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/data/dynamic_conditional_and_auto_send_input_form.py` & `shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/data/dynamic_conditional_and_auto_send_input_form.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/data/flow_and_rainfall.py` & `shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/data/flow_and_rainfall.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/data/free_echarts.py` & `shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/data/free_echarts.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/data/free_echarts_raw.py` & `shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/data/free_echarts_raw.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/data/heatmap.py` & `shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/data/heatmap.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/data/indicator.py` & `shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/data/indicator.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/data/input_form.py` & `shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/data/input_form.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/data/noise.py` & `shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/data/noise.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/data/scatter_test.csv` & `shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/data/scatter_test.csv`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/data/scatter_with_effect.py` & `shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/data/scatter_with_effect.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/data/stacked_area.py` & `shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/data/stacked_area.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/data/suburst.py` & `shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/data/suburst.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/data/table_with_labels.py` & `shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/data/table_with_labels.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/data/tree.py` & `shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/data/tree.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/data/waterfall.py` & `shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/data/waterfall.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/doughnut.py` & `shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/doughnut.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/dynamic_conditional_and_auto_send_input_form.py` & `shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/dynamic_conditional_and_auto_send_input_form.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/gauge_indicator.py` & `shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/gauge_indicator.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/heatmap.py` & `shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/heatmap.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/horizontal_bar.py` & `shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/horizontal_bar.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/indicator.py` & `shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/indicator.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/infographics.py` & `shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/infographics.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/line_with_confidence_area.py` & `shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/line_with_confidence_area.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/modal.py` & `shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/modal.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/radar.py` & `shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/radar.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/rainfall_area.py` & `shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/rainfall_area.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/rainfall_line.py` & `shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/rainfall_line.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/rose.py` & `shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/rose.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/scatter.py` & `shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/scatter.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/segmented_area_chart.py` & `shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/segmented_area_chart.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/segmented_line_chart.py` & `shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/segmented_line_chart.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/shimoku_gauges.py` & `shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/shimoku_gauges.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/table_with_lables.py` & `shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/table_with_lables.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/tabs.py` & `shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/tabs.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/tree.py` & `shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/tree.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/variants.py` & `shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/variants.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/waterfall.py` & `shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/waterfall.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/tests/mockable_tests/test_plot_api_functions/zero_centered_bar.py` & `shimoku_browser-2.4.0/tests/mockable_tests/test_plot_api_functions/zero_centered_bar.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/tests/mockable_tests/test_report_metadata_api.py` & `shimoku_browser-2.4.0/tests/mockable_tests/test_report_metadata_api.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/tests/mockable_tests/test_roles.py` & `shimoku_browser-2.4.0/tests/mockable_tests/test_roles.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/tests/mockable_tests/utils.py` & `shimoku_browser-2.4.0/tests/mockable_tests/utils.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/tests/test_ai_api.py` & `shimoku_browser-2.4.0/tests/test_ai_api.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/tests/test_components_catalog.py` & `shimoku_browser-2.4.0/tests/test_components_catalog.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/tests/test_data_managing_api.py` & `shimoku_browser-2.4.0/tests/test_data_managing_api.py`

 * *Files identical despite different names*

### Comparing `shimoku-browser-2.3.1/tests/test_file_metadata_api.py` & `shimoku_browser-2.4.0/tests/test_file_metadata_api.py`

 * *Files identical despite different names*

