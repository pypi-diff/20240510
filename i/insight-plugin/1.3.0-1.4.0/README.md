# Comparing `tmp/insight_plugin-1.3.0.tar.gz` & `tmp/insight_plugin-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "insight_plugin-1.3.0.tar", last modified: Wed Apr 24 10:37:10 2024, max compression
+gzip compressed data, was "insight_plugin-1.4.0.tar", last modified: Fri May 10 09:40:01 2024, max compression
```

## Comparing `insight_plugin-1.3.0.tar` & `insight_plugin-1.4.0.tar`

### file list

```diff
@@ -1,183 +1,176 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:37:10.574485 insight_plugin-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-04-24 10:36:48.000000 insight_plugin-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-04-24 10:37:10.570485 insight_plugin-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-04-24 10:36:48.000000 insight_plugin-1.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:37:10.550485 insight_plugin-1.3.0/insight_plugin/
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-24 10:36:48.000000 insight_plugin-1.3.0/insight_plugin/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    18895 2024-04-24 10:36:48.000000 insight_plugin-1.3.0/insight_plugin/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:37:10.554485 insight_plugin-1.3.0/insight_plugin/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-24 10:37:10.000000 insight_plugin-1.3.0/insight_plugin/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-04-24 10:36:48.000000 insight_plugin-1.3.0/insight_plugin/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:37:10.554485 insight_plugin-1.3.0/insight_plugin/features/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 10:36:48.000000 insight_plugin-1.3.0/insight_plugin/features/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:37:10.554485 insight_plugin-1.3.0/insight_plugin/features/analysis/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 10:36:48.000000 insight_plugin-1.3.0/insight_plugin/features/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-04-24 10:36:48.000000 insight_plugin-1.3.0/insight_plugin/features/analysis/controller.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:37:10.554485 insight_plugin-1.3.0/insight_plugin/features/common/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 10:36:48.000000 insight_plugin-1.3.0/insight_plugin/features/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2916 2024-04-24 10:36:48.000000 insight_plugin-1.3.0/insight_plugin/features/common/builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     6553 2024-04-24 10:36:48.000000 insight_plugin-1.3.0/insight_plugin/features/common/checksum_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-04-24 10:36:48.000000 insight_plugin-1.3.0/insight_plugin/features/common/command_line_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-04-24 10:36:48.000000 insight_plugin-1.3.0/insight_plugin/features/common/common_feature.py
--rw-r--r--   0 runner    (1001) docker     (127)    12907 2024-04-24 10:36:48.000000 insight_plugin-1.3.0/insight_plugin/features/common/docker_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-04-24 10:36:48.000000 insight_plugin-1.3.0/insight_plugin/features/common/dockerspec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-24 10:36:48.000000 insight_plugin-1.3.0/insight_plugin/features/common/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-04-24 10:36:48.000000 insight_plugin-1.3.0/insight_plugin/features/common/logging_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     6465 2024-04-24 10:36:48.000000 insight_plugin-1.3.0/insight_plugin/features/common/plugin_spec_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    24186 2024-04-24 10:36:48.000000 insight_plugin-1.3.0/insight_plugin/features/common/schema_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3225 2024-04-24 10:36:48.000000 insight_plugin-1.3.0/insight_plugin/features/common/temp_file_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    10630 2024-04-24 10:36:48.000000 insight_plugin-1.3.0/insight_plugin/features/common/template_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:37:10.558485 insight_plugin-1.3.0/insight_plugin/features/create/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 10:36:48.000000 insight_plugin-1.3.0/insight_plugin/features/create/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5010 2024-04-24 10:36:48.000000 insight_plugin-1.3.0/insight_plugin/features/create/controller.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:37:10.558485 insight_plugin-1.3.0/insight_plugin/features/create/help/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 10:36:48.000000 insight_plugin-1.3.0/insight_plugin/features/create/help/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8215 2024-04-24 10:36:48.000000 insight_plugin-1.3.0/insight_plugin/features/create/help/components.py
--rw-r--r--   0 runner    (1001) docker     (127)     4121 2024-04-24 10:36:48.000000 insight_plugin-1.3.0/insight_plugin/features/create/help/connection_help.py
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-04-24 10:36:48.000000 insight_plugin-1.3.0/insight_plugin/features/create/help/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     4289 2024-04-24 10:36:48.000000 insight_plugin-1.3.0/insight_plugin/features/create/help/help_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     8684 2024-04-24 10:36:48.000000 insight_plugin-1.3.0/insight_plugin/features/create/help/input_output_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    15746 2024-04-24 10:36:48.000000 insight_plugin-1.3.0/insight_plugin/features/create/json_generation_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    10781 2024-04-24 10:36:48.000000 insight_plugin-1.3.0/insight_plugin/features/create/plugin_to_helpmd.py
--rw-r--r--   0 runner    (1001) docker     (127)    33526 2024-04-24 10:36:48.000000 insight_plugin-1.3.0/insight_plugin/features/create/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:37:10.558485 insight_plugin-1.3.0/insight_plugin/features/export/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 10:36:48.000000 insight_plugin-1.3.0/insight_plugin/features/export/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5241 2024-04-24 10:36:48.000000 insight_plugin-1.3.0/insight_plugin/features/export/controller.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:37:10.558485 insight_plugin-1.3.0/insight_plugin/features/export/util/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 10:36:48.000000 insight_plugin-1.3.0/insight_plugin/features/export/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 10:36:48.000000 insight_plugin-1.3.0/insight_plugin/features/export/util/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:37:10.558485 insight_plugin-1.3.0/insight_plugin/features/interactive/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 10:36:48.000000 insight_plugin-1.3.0/insight_plugin/features/interactive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7628 2024-04-24 10:36:48.000000 insight_plugin-1.3.0/insight_plugin/features/interactive/controller.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:37:10.558485 insight_plugin-1.3.0/insight_plugin/features/interactive/util/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 10:36:48.000000 insight_plugin-1.3.0/insight_plugin/features/interactive/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7027 2024-04-24 10:36:48.000000 insight_plugin-1.3.0/insight_plugin/features/interactive/util/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:37:10.558485 insight_plugin-1.3.0/insight_plugin/features/linter/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 10:36:48.000000 insight_plugin-1.3.0/insight_plugin/features/linter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-24 10:36:48.000000 insight_plugin-1.3.0/insight_plugin/features/linter/controller.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:37:10.558485 insight_plugin-1.3.0/insight_plugin/features/refresh/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 10:36:48.000000 insight_plugin-1.3.0/insight_plugin/features/refresh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3263 2024-04-24 10:36:48.000000 insight_plugin-1.3.0/insight_plugin/features/refresh/controller.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:37:10.558485 insight_plugin-1.3.0/insight_plugin/features/run/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 10:36:48.000000 insight_plugin-1.3.0/insight_plugin/features/run/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-04-24 10:36:48.000000 insight_plugin-1.3.0/insight_plugin/features/run/bash_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/insight_plugin/features/run/run_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/insight_plugin/features/run/server_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:37:10.558485 insight_plugin-1.3.0/insight_plugin/features/samples/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/insight_plugin/features/samples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/insight_plugin/features/samples/controller.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:37:10.562485 insight_plugin-1.3.0/insight_plugin/features/samples/util/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/insight_plugin/features/samples/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/insight_plugin/features/samples/util/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    12047 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/insight_plugin/features/samples/util/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:37:10.562485 insight_plugin-1.3.0/insight_plugin/features/validate/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/insight_plugin/features/validate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/insight_plugin/features/validate/controller.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:37:10.562485 insight_plugin-1.3.0/insight_plugin/features/version/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/insight_plugin/features/version/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/insight_plugin/features/version/controller.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:37:10.562485 insight_plugin-1.3.0/insight_plugin/features/version/util/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/insight_plugin/features/version/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/insight_plugin/features/version/util/helpmd_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/insight_plugin/features/version/util/input_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/insight_plugin/features/version/util/version_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/insight_plugin/features/version/util/yaml_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:37:10.562485 insight_plugin-1.3.0/insight_plugin/features/view/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/insight_plugin/features/view/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/insight_plugin/features/view/controller.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:37:10.562485 insight_plugin-1.3.0/insight_plugin/templates/
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/insight_plugin/templates/.dockerignore.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/insight_plugin/templates/Dockerfile.jinja
--rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/insight_plugin/templates/Makefile.jinja
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/insight_plugin/templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:37:10.562485 insight_plugin-1.3.0/insight_plugin/templates/assessment/
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/insight_plugin/templates/assessment/assessment.jinja
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:37:10.562485 insight_plugin-1.3.0/insight_plugin/templates/bin/
--rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/insight_plugin/templates/bin/plugin.jinja
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:37:10.562485 insight_plugin-1.3.0/insight_plugin/templates/plugin/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/insight_plugin/templates/plugin/__init__.py.jinja
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:37:10.562485 insight_plugin-1.3.0/insight_plugin/templates/plugin/actions/
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/insight_plugin/templates/plugin/actions/__init__.py.jinja
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:37:10.562485 insight_plugin-1.3.0/insight_plugin/templates/plugin/actions/action/
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/insight_plugin/templates/plugin/actions/action/__init__.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/insight_plugin/templates/plugin/actions/action/action.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/insight_plugin/templates/plugin/actions/action/schema.py.jinja
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:37:10.566485 insight_plugin-1.3.0/insight_plugin/templates/plugin/connection/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/insight_plugin/templates/plugin/connection/__init__.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/insight_plugin/templates/plugin/connection/connection.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/insight_plugin/templates/plugin/connection/schema.py.jinja
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:37:10.566485 insight_plugin-1.3.0/insight_plugin/templates/plugin/tasks/
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/insight_plugin/templates/plugin/tasks/__init__.py.jinja
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:37:10.566485 insight_plugin-1.3.0/insight_plugin/templates/plugin/tasks/task/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/insight_plugin/templates/plugin/tasks/task/__init__.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/insight_plugin/templates/plugin/tasks/task/schema.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/insight_plugin/templates/plugin/tasks/task/task.py.jinja
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:37:10.566485 insight_plugin-1.3.0/insight_plugin/templates/plugin/triggers/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/insight_plugin/templates/plugin/triggers/__init__.py.jinja
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:37:10.566485 insight_plugin-1.3.0/insight_plugin/templates/plugin/triggers/trigger/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/insight_plugin/templates/plugin/triggers/trigger/__init__.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      933 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/insight_plugin/templates/plugin/triggers/trigger/schema.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/insight_plugin/templates/plugin/triggers/trigger/trigger.py.jinja
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:37:10.566485 insight_plugin-1.3.0/insight_plugin/templates/plugin/util/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/insight_plugin/templates/plugin/util/__init__.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/insight_plugin/templates/requirements.txt.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/insight_plugin/templates/setup.py.jinja
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:37:10.566485 insight_plugin-1.3.0/insight_plugin/templates/unit_test/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/insight_plugin/templates/unit_test/__init__.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/insight_plugin/templates/unit_test/test_action.py.jinja
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:37:10.554485 insight_plugin-1.3.0/insight_plugin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-04-24 10:37:10.000000 insight_plugin-1.3.0/insight_plugin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6209 2024-04-24 10:37:10.000000 insight_plugin-1.3.0/insight_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 10:37:10.000000 insight_plugin-1.3.0/insight_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-24 10:37:10.000000 insight_plugin-1.3.0/insight_plugin.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-24 10:37:10.000000 insight_plugin-1.3.0/insight_plugin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-24 10:37:10.000000 insight_plugin-1.3.0/insight_plugin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 10:37:10.574485 insight_plugin-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:37:10.570485 insight_plugin-1.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:37:10.570485 insight_plugin-1.3.0/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/tests/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:37:10.570485 insight_plugin-1.3.0/tests/resources/export_test_base64/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/tests/resources/export_test_base64/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:37:10.570485 insight_plugin-1.3.0/tests/resources/export_test_base64/komand_base64/
--rwxr-xr-x   0 runner    (1001) docker     (127)       40 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/tests/resources/export_test_base64/komand_base64/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:37:10.570485 insight_plugin-1.3.0/tests/resources/export_test_base64/komand_base64/actions/
--rwxr-xr-x   0 runner    (1001) docker     (127)      108 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/tests/resources/export_test_base64/komand_base64/actions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:37:10.570485 insight_plugin-1.3.0/tests/resources/export_test_base64/komand_base64/actions/decode/
--rwxr-xr-x   0 runner    (1001) docker     (127)       67 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/tests/resources/export_test_base64/komand_base64/actions/decode/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1299 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/tests/resources/export_test_base64/komand_base64/actions/decode/action.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1430 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/tests/resources/export_test_base64/komand_base64/actions/decode/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:37:10.570485 insight_plugin-1.3.0/tests/resources/export_test_base64/komand_base64/actions/encode/
--rwxr-xr-x   0 runner    (1001) docker     (127)       67 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/tests/resources/export_test_base64/komand_base64/actions/encode/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      589 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/tests/resources/export_test_base64/komand_base64/actions/encode/action.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1142 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/tests/resources/export_test_base64/komand_base64/actions/encode/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:37:10.570485 insight_plugin-1.3.0/tests/resources/export_test_base64/komand_base64/connection/
--rwxr-xr-x   0 runner    (1001) docker     (127)       75 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/tests/resources/export_test_base64/komand_base64/connection/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      276 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/tests/resources/export_test_base64/komand_base64/connection/connection.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      316 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/tests/resources/export_test_base64/komand_base64/connection/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:37:10.570485 insight_plugin-1.3.0/tests/resources/export_test_base64/komand_base64/triggers/
--rwxr-xr-x   0 runner    (1001) docker     (127)       40 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/tests/resources/export_test_base64/komand_base64/triggers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:37:10.570485 insight_plugin-1.3.0/tests/resources/export_test_base64/komand_base64/util/
--rwxr-xr-x   0 runner    (1001) docker     (127)       40 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/tests/resources/export_test_base64/komand_base64/util/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      469 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/tests/resources/export_test_base64/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:37:10.570485 insight_plugin-1.3.0/tests/resources/export_test_base64/unit_test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/tests/resources/export_test_base64/unit_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/tests/resources/export_test_base64/unit_test/test_encode.py
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/tests/test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/tests/test_checksum.py
--rw-r--r--   0 runner    (1001) docker     (127)     6313 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/tests/test_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/tests/test_export.py
--rw-r--r--   0 runner    (1001) docker     (127)     4542 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/tests/test_gen_samples.py
--rw-r--r--   0 runner    (1001) docker     (127)     4083 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/tests/test_help_creation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/tests/test_interactive.py
--rw-r--r--   0 runner    (1001) docker     (127)     4190 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/tests/test_json_generate.py
--rw-r--r--   0 runner    (1001) docker     (127)     8797 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/tests/test_refresh.py
--rw-r--r--   0 runner    (1001) docker     (127)     4950 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/tests/test_run.py
--rw-r--r--   0 runner    (1001) docker     (127)     4410 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/tests/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     4523 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/tests/test_semver.py
--rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/tests/test_spec_order.py
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/tests/test_temp_file_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/tests/test_validate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/tests/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:40:01.456187 insight_plugin-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-10 09:39:44.000000 insight_plugin-1.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-05-10 09:40:01.456187 insight_plugin-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-05-10 09:39:44.000000 insight_plugin-1.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:40:01.428187 insight_plugin-1.4.0/insight_plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-10 09:39:44.000000 insight_plugin-1.4.0/insight_plugin/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    18701 2024-05-10 09:39:44.000000 insight_plugin-1.4.0/insight_plugin/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:40:01.432187 insight_plugin-1.4.0/insight_plugin/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-10 09:40:01.000000 insight_plugin-1.4.0/insight_plugin/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-05-10 09:39:44.000000 insight_plugin-1.4.0/insight_plugin/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:40:01.432187 insight_plugin-1.4.0/insight_plugin/features/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 09:39:44.000000 insight_plugin-1.4.0/insight_plugin/features/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:40:01.432187 insight_plugin-1.4.0/insight_plugin/features/analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 09:39:44.000000 insight_plugin-1.4.0/insight_plugin/features/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-05-10 09:39:44.000000 insight_plugin-1.4.0/insight_plugin/features/analysis/controller.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:40:01.432187 insight_plugin-1.4.0/insight_plugin/features/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 09:39:44.000000 insight_plugin-1.4.0/insight_plugin/features/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2916 2024-05-10 09:39:44.000000 insight_plugin-1.4.0/insight_plugin/features/common/builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6553 2024-05-10 09:39:44.000000 insight_plugin-1.4.0/insight_plugin/features/common/checksum_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-05-10 09:39:44.000000 insight_plugin-1.4.0/insight_plugin/features/common/command_line_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-05-10 09:39:44.000000 insight_plugin-1.4.0/insight_plugin/features/common/common_feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12907 2024-05-10 09:39:44.000000 insight_plugin-1.4.0/insight_plugin/features/common/docker_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-05-10 09:39:44.000000 insight_plugin-1.4.0/insight_plugin/features/common/dockerspec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-05-10 09:39:44.000000 insight_plugin-1.4.0/insight_plugin/features/common/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-05-10 09:39:44.000000 insight_plugin-1.4.0/insight_plugin/features/common/logging_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6433 2024-05-10 09:39:44.000000 insight_plugin-1.4.0/insight_plugin/features/common/plugin_spec_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24216 2024-05-10 09:39:44.000000 insight_plugin-1.4.0/insight_plugin/features/common/schema_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3225 2024-05-10 09:39:44.000000 insight_plugin-1.4.0/insight_plugin/features/common/temp_file_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10630 2024-05-10 09:39:44.000000 insight_plugin-1.4.0/insight_plugin/features/common/template_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:40:01.432187 insight_plugin-1.4.0/insight_plugin/features/create/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 09:39:44.000000 insight_plugin-1.4.0/insight_plugin/features/create/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4629 2024-05-10 09:39:44.000000 insight_plugin-1.4.0/insight_plugin/features/create/controller.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:40:01.436187 insight_plugin-1.4.0/insight_plugin/features/create/help/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 09:39:44.000000 insight_plugin-1.4.0/insight_plugin/features/create/help/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8215 2024-05-10 09:39:44.000000 insight_plugin-1.4.0/insight_plugin/features/create/help/components.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4121 2024-05-10 09:39:44.000000 insight_plugin-1.4.0/insight_plugin/features/create/help/connection_help.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-05-10 09:39:44.000000 insight_plugin-1.4.0/insight_plugin/features/create/help/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4290 2024-05-10 09:39:44.000000 insight_plugin-1.4.0/insight_plugin/features/create/help/help_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8684 2024-05-10 09:39:44.000000 insight_plugin-1.4.0/insight_plugin/features/create/help/input_output_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15746 2024-05-10 09:39:44.000000 insight_plugin-1.4.0/insight_plugin/features/create/json_generation_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10781 2024-05-10 09:39:44.000000 insight_plugin-1.4.0/insight_plugin/features/create/plugin_to_helpmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33526 2024-05-10 09:39:44.000000 insight_plugin-1.4.0/insight_plugin/features/create/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:40:01.436187 insight_plugin-1.4.0/insight_plugin/features/export/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 09:39:44.000000 insight_plugin-1.4.0/insight_plugin/features/export/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5241 2024-05-10 09:39:44.000000 insight_plugin-1.4.0/insight_plugin/features/export/controller.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:40:01.436187 insight_plugin-1.4.0/insight_plugin/features/export/util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 09:39:44.000000 insight_plugin-1.4.0/insight_plugin/features/export/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 09:39:44.000000 insight_plugin-1.4.0/insight_plugin/features/export/util/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:40:01.436187 insight_plugin-1.4.0/insight_plugin/features/linter/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 09:39:44.000000 insight_plugin-1.4.0/insight_plugin/features/linter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-10 09:39:44.000000 insight_plugin-1.4.0/insight_plugin/features/linter/controller.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:40:01.436187 insight_plugin-1.4.0/insight_plugin/features/refresh/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 09:39:44.000000 insight_plugin-1.4.0/insight_plugin/features/refresh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3263 2024-05-10 09:39:44.000000 insight_plugin-1.4.0/insight_plugin/features/refresh/controller.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:40:01.436187 insight_plugin-1.4.0/insight_plugin/features/run/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 09:39:44.000000 insight_plugin-1.4.0/insight_plugin/features/run/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-05-10 09:39:44.000000 insight_plugin-1.4.0/insight_plugin/features/run/bash_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-05-10 09:39:44.000000 insight_plugin-1.4.0/insight_plugin/features/run/run_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-05-10 09:39:44.000000 insight_plugin-1.4.0/insight_plugin/features/run/server_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:40:01.436187 insight_plugin-1.4.0/insight_plugin/features/samples/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 09:39:44.000000 insight_plugin-1.4.0/insight_plugin/features/samples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-05-10 09:39:44.000000 insight_plugin-1.4.0/insight_plugin/features/samples/controller.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:40:01.440187 insight_plugin-1.4.0/insight_plugin/features/samples/util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 09:39:44.000000 insight_plugin-1.4.0/insight_plugin/features/samples/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-10 09:39:44.000000 insight_plugin-1.4.0/insight_plugin/features/samples/util/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12047 2024-05-10 09:39:44.000000 insight_plugin-1.4.0/insight_plugin/features/samples/util/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:40:01.440187 insight_plugin-1.4.0/insight_plugin/features/validate/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 09:39:44.000000 insight_plugin-1.4.0/insight_plugin/features/validate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-10 09:39:44.000000 insight_plugin-1.4.0/insight_plugin/features/validate/controller.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:40:01.440187 insight_plugin-1.4.0/insight_plugin/features/version/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 09:39:44.000000 insight_plugin-1.4.0/insight_plugin/features/version/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-05-10 09:39:44.000000 insight_plugin-1.4.0/insight_plugin/features/version/controller.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:40:01.440187 insight_plugin-1.4.0/insight_plugin/features/version/util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 09:39:44.000000 insight_plugin-1.4.0/insight_plugin/features/version/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-05-10 09:39:44.000000 insight_plugin-1.4.0/insight_plugin/features/version/util/helpmd_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-05-10 09:39:44.000000 insight_plugin-1.4.0/insight_plugin/features/version/util/input_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-05-10 09:39:44.000000 insight_plugin-1.4.0/insight_plugin/features/version/util/version_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-05-10 09:39:44.000000 insight_plugin-1.4.0/insight_plugin/features/version/util/yaml_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:40:01.440187 insight_plugin-1.4.0/insight_plugin/features/view/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 09:39:44.000000 insight_plugin-1.4.0/insight_plugin/features/view/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-05-10 09:39:44.000000 insight_plugin-1.4.0/insight_plugin/features/view/controller.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:40:01.440187 insight_plugin-1.4.0/insight_plugin/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-10 09:39:44.000000 insight_plugin-1.4.0/insight_plugin/templates/.dockerignore.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-05-10 09:39:44.000000 insight_plugin-1.4.0/insight_plugin/templates/Dockerfile.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-05-10 09:39:44.000000 insight_plugin-1.4.0/insight_plugin/templates/Makefile.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 09:39:44.000000 insight_plugin-1.4.0/insight_plugin/templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:40:01.440187 insight_plugin-1.4.0/insight_plugin/templates/assessment/
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-10 09:39:44.000000 insight_plugin-1.4.0/insight_plugin/templates/assessment/assessment.jinja
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:40:01.440187 insight_plugin-1.4.0/insight_plugin/templates/bin/
+-rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-05-10 09:39:44.000000 insight_plugin-1.4.0/insight_plugin/templates/bin/plugin.jinja
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:40:01.440187 insight_plugin-1.4.0/insight_plugin/templates/plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-10 09:39:44.000000 insight_plugin-1.4.0/insight_plugin/templates/plugin/__init__.py.jinja
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:40:01.444187 insight_plugin-1.4.0/insight_plugin/templates/plugin/actions/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-10 09:39:44.000000 insight_plugin-1.4.0/insight_plugin/templates/plugin/actions/__init__.py.jinja
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:40:01.444187 insight_plugin-1.4.0/insight_plugin/templates/plugin/actions/action/
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-10 09:39:44.000000 insight_plugin-1.4.0/insight_plugin/templates/plugin/actions/action/__init__.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-10 09:39:44.000000 insight_plugin-1.4.0/insight_plugin/templates/plugin/actions/action/action.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-10 09:39:44.000000 insight_plugin-1.4.0/insight_plugin/templates/plugin/actions/action/schema.py.jinja
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:40:01.444187 insight_plugin-1.4.0/insight_plugin/templates/plugin/connection/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-10 09:39:44.000000 insight_plugin-1.4.0/insight_plugin/templates/plugin/connection/__init__.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-05-10 09:39:44.000000 insight_plugin-1.4.0/insight_plugin/templates/plugin/connection/connection.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-10 09:39:44.000000 insight_plugin-1.4.0/insight_plugin/templates/plugin/connection/schema.py.jinja
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:40:01.444187 insight_plugin-1.4.0/insight_plugin/templates/plugin/tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-10 09:39:44.000000 insight_plugin-1.4.0/insight_plugin/templates/plugin/tasks/__init__.py.jinja
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:40:01.444187 insight_plugin-1.4.0/insight_plugin/templates/plugin/tasks/task/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-10 09:39:44.000000 insight_plugin-1.4.0/insight_plugin/templates/plugin/tasks/task/__init__.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-05-10 09:39:44.000000 insight_plugin-1.4.0/insight_plugin/templates/plugin/tasks/task/schema.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-05-10 09:39:44.000000 insight_plugin-1.4.0/insight_plugin/templates/plugin/tasks/task/task.py.jinja
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:40:01.444187 insight_plugin-1.4.0/insight_plugin/templates/plugin/triggers/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-10 09:39:44.000000 insight_plugin-1.4.0/insight_plugin/templates/plugin/triggers/__init__.py.jinja
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:40:01.444187 insight_plugin-1.4.0/insight_plugin/templates/plugin/triggers/trigger/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-10 09:39:44.000000 insight_plugin-1.4.0/insight_plugin/templates/plugin/triggers/trigger/__init__.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-05-10 09:39:44.000000 insight_plugin-1.4.0/insight_plugin/templates/plugin/triggers/trigger/schema.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-10 09:39:44.000000 insight_plugin-1.4.0/insight_plugin/templates/plugin/triggers/trigger/trigger.py.jinja
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:40:01.444187 insight_plugin-1.4.0/insight_plugin/templates/plugin/util/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-10 09:39:44.000000 insight_plugin-1.4.0/insight_plugin/templates/plugin/util/__init__.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-10 09:39:44.000000 insight_plugin-1.4.0/insight_plugin/templates/requirements.txt.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-10 09:39:44.000000 insight_plugin-1.4.0/insight_plugin/templates/setup.py.jinja
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:40:01.444187 insight_plugin-1.4.0/insight_plugin/templates/unit_test/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-10 09:39:44.000000 insight_plugin-1.4.0/insight_plugin/templates/unit_test/__init__.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-10 09:39:44.000000 insight_plugin-1.4.0/insight_plugin/templates/unit_test/test_action.py.jinja
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:40:01.432187 insight_plugin-1.4.0/insight_plugin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-05-10 09:40:01.000000 insight_plugin-1.4.0/insight_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5983 2024-05-10 09:40:01.000000 insight_plugin-1.4.0/insight_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 09:40:01.000000 insight_plugin-1.4.0/insight_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-10 09:40:01.000000 insight_plugin-1.4.0/insight_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-10 09:40:01.000000 insight_plugin-1.4.0/insight_plugin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-10 09:40:01.000000 insight_plugin-1.4.0/insight_plugin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-10 09:39:44.000000 insight_plugin-1.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 09:40:01.456187 insight_plugin-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-05-10 09:39:44.000000 insight_plugin-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:40:01.452187 insight_plugin-1.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-10 09:39:44.000000 insight_plugin-1.4.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:40:01.452187 insight_plugin-1.4.0/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 09:39:44.000000 insight_plugin-1.4.0/tests/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:40:01.452187 insight_plugin-1.4.0/tests/resources/export_test_base64/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 09:39:44.000000 insight_plugin-1.4.0/tests/resources/export_test_base64/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:40:01.452187 insight_plugin-1.4.0/tests/resources/export_test_base64/komand_base64/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       40 2024-05-10 09:39:44.000000 insight_plugin-1.4.0/tests/resources/export_test_base64/komand_base64/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:40:01.452187 insight_plugin-1.4.0/tests/resources/export_test_base64/komand_base64/actions/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      108 2024-05-10 09:39:44.000000 insight_plugin-1.4.0/tests/resources/export_test_base64/komand_base64/actions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:40:01.452187 insight_plugin-1.4.0/tests/resources/export_test_base64/komand_base64/actions/decode/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       67 2024-05-10 09:39:44.000000 insight_plugin-1.4.0/tests/resources/export_test_base64/komand_base64/actions/decode/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1299 2024-05-10 09:39:44.000000 insight_plugin-1.4.0/tests/resources/export_test_base64/komand_base64/actions/decode/action.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1430 2024-05-10 09:39:44.000000 insight_plugin-1.4.0/tests/resources/export_test_base64/komand_base64/actions/decode/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:40:01.452187 insight_plugin-1.4.0/tests/resources/export_test_base64/komand_base64/actions/encode/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       67 2024-05-10 09:39:44.000000 insight_plugin-1.4.0/tests/resources/export_test_base64/komand_base64/actions/encode/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      589 2024-05-10 09:39:44.000000 insight_plugin-1.4.0/tests/resources/export_test_base64/komand_base64/actions/encode/action.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1142 2024-05-10 09:39:44.000000 insight_plugin-1.4.0/tests/resources/export_test_base64/komand_base64/actions/encode/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:40:01.452187 insight_plugin-1.4.0/tests/resources/export_test_base64/komand_base64/connection/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       75 2024-05-10 09:39:44.000000 insight_plugin-1.4.0/tests/resources/export_test_base64/komand_base64/connection/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      276 2024-05-10 09:39:44.000000 insight_plugin-1.4.0/tests/resources/export_test_base64/komand_base64/connection/connection.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      316 2024-05-10 09:39:44.000000 insight_plugin-1.4.0/tests/resources/export_test_base64/komand_base64/connection/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:40:01.456187 insight_plugin-1.4.0/tests/resources/export_test_base64/komand_base64/triggers/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       40 2024-05-10 09:39:44.000000 insight_plugin-1.4.0/tests/resources/export_test_base64/komand_base64/triggers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:40:01.456187 insight_plugin-1.4.0/tests/resources/export_test_base64/komand_base64/util/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       40 2024-05-10 09:39:44.000000 insight_plugin-1.4.0/tests/resources/export_test_base64/komand_base64/util/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      469 2024-05-10 09:39:44.000000 insight_plugin-1.4.0/tests/resources/export_test_base64/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:40:01.456187 insight_plugin-1.4.0/tests/resources/export_test_base64/unit_test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 09:39:44.000000 insight_plugin-1.4.0/tests/resources/export_test_base64/unit_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-10 09:39:44.000000 insight_plugin-1.4.0/tests/resources/export_test_base64/unit_test/test_encode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-10 09:39:44.000000 insight_plugin-1.4.0/tests/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-05-10 09:39:44.000000 insight_plugin-1.4.0/tests/test_checksum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6313 2024-05-10 09:39:44.000000 insight_plugin-1.4.0/tests/test_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-05-10 09:39:44.000000 insight_plugin-1.4.0/tests/test_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4542 2024-05-10 09:39:44.000000 insight_plugin-1.4.0/tests/test_gen_samples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4083 2024-05-10 09:39:44.000000 insight_plugin-1.4.0/tests/test_help_creation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4190 2024-05-10 09:39:44.000000 insight_plugin-1.4.0/tests/test_json_generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8797 2024-05-10 09:39:44.000000 insight_plugin-1.4.0/tests/test_refresh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4950 2024-05-10 09:39:44.000000 insight_plugin-1.4.0/tests/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4410 2024-05-10 09:39:44.000000 insight_plugin-1.4.0/tests/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4523 2024-05-10 09:39:44.000000 insight_plugin-1.4.0/tests/test_semver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-05-10 09:39:44.000000 insight_plugin-1.4.0/tests/test_spec_order.py
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-10 09:39:44.000000 insight_plugin-1.4.0/tests/test_temp_file_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-10 09:39:44.000000 insight_plugin-1.4.0/tests/test_validate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-05-10 09:39:44.000000 insight_plugin-1.4.0/tests/util.py
```

### Comparing `insight_plugin-1.3.0/LICENSE` & `insight_plugin-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.3.0/PKG-INFO` & `insight_plugin-1.4.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: insight_plugin
-Version: 1.3.0
+Version: 1.4.0
 Summary: Plugin tooling for the Rapid7 Insight platform
 Home-page: https://github.com/rapid7/insight-plugin
 Author: Rapid7 Integrations Alliance
 Author-email: integrationalliance@rapid7.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -16,14 +16,31 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Insight Plugin - CLI Tooling for plugin development
 
 ## Commands
 
+### Analysis
+Run Static Code Analysis on the plugin.
+
+This command will run the static code analysis check on the plugin.
+
+### Linter
+Run the linter check on the plugin.
+
+This command will run the `black` linter on the plugin and return any
+formatting issues with the plugin.
+
+### Checks
+Run analysis, linter and validate on the plugin.
+
+This will allow you to recreate, locally, all the github checks that get run
+on plugins.
+
 ### Create
 Create a new plugin.
 
 This command will generate the skeleton folder structure and 
 code for a new plugin, based on the provided plugin.spec.yaml file.
 
 ### Export
```

### Comparing `insight_plugin-1.3.0/README.md` & `insight_plugin-1.4.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,28 @@
 # Insight Plugin - CLI Tooling for plugin development
 
 ## Commands
 
+### Analysis
+Run Static Code Analysis on the plugin.
+
+This command will run the static code analysis check on the plugin.
+
+### Linter
+Run the linter check on the plugin.
+
+This command will run the `black` linter on the plugin and return any
+formatting issues with the plugin.
+
+### Checks
+Run analysis, linter and validate on the plugin.
+
+This will allow you to recreate, locally, all the github checks that get run
+on plugins.
+
 ### Create
 Create a new plugin.
 
 This command will generate the skeleton folder structure and 
 code for a new plugin, based on the provided plugin.spec.yaml file.
 
 ### Export
```

### Comparing `insight_plugin-1.3.0/insight_plugin/__main__.py` & `insight_plugin-1.4.0/insight_plugin/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 from insight_plugin.features.export.controller import ExportController
 from insight_plugin.features.linter.controller import LinterController
 from insight_plugin.features.refresh.controller import RefreshController
 from insight_plugin.features.run.run_controller import RunController
 from insight_plugin.features.validate.controller import ValidateController
 from insight_plugin.features.run.server_controller import RunServerController
 from insight_plugin.features.run.bash_controller import RunShellController
-from insight_plugin.features.interactive.controller import InteractiveController
 from insight_plugin.features.common.exceptions import InsightException
 from insight_plugin.features.version.controller import VersionController
 from insight_plugin.features.view.controller import ViewController
 from typing import List
 from insight_plugin.constants import Color
 
 DEFAULT_JQ_STRING = ".body.output"
@@ -95,15 +94,15 @@
     else:
         # If an argument was given then execute that. If arguments fail, fall back to interactive session
         try:
             args.func(args)
         except InsightException as error:
             logging.exception(error)
         except AttributeError:
-            interactive()
+            print("try 'insight-plugin --help' for more information")
 
 
 def create_argparse(subparsers, parsers_list: List) -> None:
     """
     Handle the arg-parsing for the create subcommand
     :param subparsers: List to be filled with commands
     :param parsers_list: List to be appended with parsed commands
@@ -171,22 +170,14 @@
             "verbose": args.verbose,
             "target_dir": args.target_dir,
         }
     )
     controller.export()
 
 
-def interactive() -> None:
-    """
-    Start a general interactive session with the user
-    :return: None
-    """
-    InteractiveController.prompt_menu()
-
-
 def refresh_argparse(subparsers, parsers_list: List) -> None:
     """
     Handle the arg-parsing for the refresh subcommand
     :param subparsers: List to be filled with commands
     :param parsers_list: List to be appended with parsed commands
     :return: None
     """
```

### Comparing `insight_plugin-1.3.0/insight_plugin/__pycache__/__init__.cpython-39.pyc` & `insight_plugin-1.4.0/insight_plugin/__pycache__/__init__.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Apr 24 10:36:48 2024 UTC, .py size: 429 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-00000000: 610d 0d0a 0000 0000 c0e0 2866 ad01 0000  a.........(f....
+00000000: 610d 0d0a 0000 0000 60eb 3d66 ad01 0000  a.......`.=f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0007 0000 0040 0000 0073 6400 0000 6400  .....@...sd...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6402  d.l.Z.d.d.l.Z.d.
 00000040: 5a02 6500 6a03 a004 6500 6a03 a005 6506  Z.e.j...e.j...e.
 00000050: a101 a101 5a07 6403 5a08 6404 5a09 6405  ....Z.d.Z.d.Z.d.
 00000060: 5a0a 6406 5a0b 6407 5a0c 6408 5a0d 6408  Z.d.Z.d.Z.d.Z.d.
 00000070: 5a0e 6501 6a03 a00f 6500 6a03 a004 6500  Z.e.j...e.j...e.
 00000080: 6a03 a004 6506 a101 a101 a101 0100 6401  j...e.........d.
-00000090: 5300 2909 e900 0000 004e 7a05 312e 332e  S.)......Nz.1.3.
+00000090: 5300 2909 e900 0000 004e 7a05 312e 342e  S.)......Nz.1.4.
 000000a0: 305a 0664 6f63 6b65 727a 0575 7466 2d38  0Z.dockerz.utf-8
 000000b0: 5a04 6963 6f6e 5a1d 696e 7369 6768 7463  Z.iconZ.insightc
 000000c0: 6f6e 6e65 6374 5f70 6c75 6769 6e5f 7275  onnect_plugin_ru
 000000d0: 6e74 696d 657a 1d69 6e73 6967 6874 636f  ntimez.insightco
 000000e0: 6e6e 6563 742d 706c 7567 696e 2d72 756e  nnect-plugin-run
 000000f0: 7469 6d65 5a06 6b6f 6d61 6e64 2910 da02  timeZ.komand)...
 00000100: 6f73 da03 7379 73da 0756 4552 5349 4f4e  os..sys..VERSION
```

### Comparing `insight_plugin-1.3.0/insight_plugin/constants.py` & `insight_plugin-1.4.0/insight_plugin/constants.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.3.0/insight_plugin/features/analysis/controller.py` & `insight_plugin-1.4.0/insight_plugin/features/analysis/controller.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.3.0/insight_plugin/features/common/builder.py` & `insight_plugin-1.4.0/insight_plugin/features/common/builder.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.3.0/insight_plugin/features/common/checksum_util.py` & `insight_plugin-1.4.0/insight_plugin/features/common/checksum_util.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.3.0/insight_plugin/features/common/command_line_util.py` & `insight_plugin-1.4.0/insight_plugin/features/common/command_line_util.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.3.0/insight_plugin/features/common/common_feature.py` & `insight_plugin-1.4.0/insight_plugin/features/common/common_feature.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.3.0/insight_plugin/features/common/docker_util.py` & `insight_plugin-1.4.0/insight_plugin/features/common/docker_util.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.3.0/insight_plugin/features/common/dockerspec.py` & `insight_plugin-1.4.0/insight_plugin/features/common/dockerspec.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.3.0/insight_plugin/features/common/exceptions.py` & `insight_plugin-1.4.0/insight_plugin/features/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.3.0/insight_plugin/features/common/logging_util.py` & `insight_plugin-1.4.0/insight_plugin/features/common/logging_util.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.3.0/insight_plugin/features/common/plugin_spec_util.py` & `insight_plugin-1.4.0/insight_plugin/features/common/plugin_spec_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,15 +60,14 @@
     TRIGGER = PluginSpecConstants.TRIGGERS
     TASK = PluginSpecConstants.TASKS
 
 
 class PluginSpecUtilModes(Enum):
     # Class that would later support alternate ways of getting the spec file
     SPECFILE = f"{PluginSpecConstants.FILEPATH} mode"
-    INTERACTIVE = "interactive"
     GUI = "gui"
 
 
 class PluginSpecTypes:
     # Spec is an explicit type alias defining valid plugin spec values
     Spec = Dict[str, Union[str, bool, int, float, dict]]
```

### Comparing `insight_plugin-1.3.0/insight_plugin/features/common/schema_util.py` & `insight_plugin-1.4.0/insight_plugin/features/common/schema_util.py`

 * *Files 0% similar despite different names*

```diff
@@ -437,15 +437,17 @@
             # Set the current parameter description if one exists.
             SchemaUtil.try_add(
                 PluginSpecConstants.DESCRIPTION, items, parent_object[key]
             )
             # Set the current parameter default if one exists.
             SchemaUtil.try_add(PluginSpecConstants.DEFAULT, items, parent_object[key])
             # Set placeholder
-            SchemaUtil.try_add(PluginSpecConstants.PLACEHOLDER, items, parent_object[key])
+            SchemaUtil.try_add(
+                PluginSpecConstants.PLACEHOLDER, items, parent_object[key]
+            )
             # Set tooltip
             SchemaUtil.try_add(PluginSpecConstants.TOOLTIP, items, parent_object[key])
             # If the current parameter is an array (it has items contents), set the items object dict.
             if array_items[SchemaConstants.ITEMS]:
                 SchemaUtil.try_add(
                     SchemaConstants.ITEMS, array_items, parent_object[key]
                 )
```

### Comparing `insight_plugin-1.3.0/insight_plugin/features/common/temp_file_util.py` & `insight_plugin-1.4.0/insight_plugin/features/common/temp_file_util.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.3.0/insight_plugin/features/common/template_util.py` & `insight_plugin-1.4.0/insight_plugin/features/common/template_util.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.3.0/insight_plugin/features/create/controller.py` & `insight_plugin-1.4.0/insight_plugin/features/create/controller.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,22 +34,14 @@
         )
         return cls(
             kwargs.get("spec_path"),
             kwargs.get("verbose"),
             kwargs.get("target_dir"),
         )
 
-    def interactive_prompt_spec(self) -> PluginSpecTypes.Spec:
-        # TODO: Implement interactive create
-        self.logger.warning(
-            "Creating a plugin spec interactively is not yet supported. "
-            "Please create a plugin.spec.yaml"
-        )
-        return {"": ""}
-
     def spec_to_file(self, spec: PluginSpecTypes.Spec, plugin_dir: str):
         with open(
             os.path.join(plugin_dir, "plugin.spec.yaml"), "w", encoding=FILE_ENCODING
         ) as plugin_spec:
             plugin_spec.write(str(spec))  # This is formatted in JSON not YAML
 
     def create(self) -> None:
@@ -71,16 +63,15 @@
 
         # Check if a plugin.spec.yaml file path has been provided as a CLI argument
         if self._spec_path:
             # Load the plugin spec from file
             spec = PluginSpecUtil.get_spec_file(self._spec_path)
         else:
             # TODO
-            # Interactively prompt the user for plugin spec configuration values
-            spec = self.interactive_prompt_spec()
+            print("No spec file provided")
 
         # The target directory will CONTAIN the top-level directory containing all plugin content.
         # The target directory IS NOT the top-level plugin directory itself.
         # The top-level plugin directory WILL BE CREATED by this tool INSIDE the target directory.
         plugin_dir = os.path.join(target_dir, spec["name"])
 
         if not os.path.exists(plugin_dir):
```

### Comparing `insight_plugin-1.3.0/insight_plugin/features/create/help/components.py` & `insight_plugin-1.4.0/insight_plugin/features/create/help/components.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.3.0/insight_plugin/features/create/help/connection_help.py` & `insight_plugin-1.4.0/insight_plugin/features/create/help/connection_help.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.3.0/insight_plugin/features/create/help/constants.py` & `insight_plugin-1.4.0/insight_plugin/features/create/help/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         "Type",
         "Default",
         "Required",
         "Description",
         "Enum",
         "Example",
         "Placeholder",
-        "Tooltip"
+        "Tooltip",
     ]
     OUTPUT_HEADERS = [
         "Name",
         "Type",
         "Required",
         "Description",
         "Example",
```

### Comparing `insight_plugin-1.3.0/insight_plugin/features/create/help/help_util.py` & `insight_plugin-1.4.0/insight_plugin/features/create/help/help_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
                     item.get(PluginSpecConstants.TYPE, "None"),
                     item.get(PluginSpecConstants.DEFAULT, "None"),
                     item.get(PluginSpecConstants.REQUIRED, "None"),
                     item.get(PluginSpecConstants.DESCRIPTION, "None"),
                     item.get(PluginSpecConstants.ENUM, "None"),
                     item.get(PluginSpecConstants.EXAMPLE, "None"),
                     item.get(PluginSpecConstants.PLACEHOLDER, "None"),
-                    item.get(PluginSpecConstants.TOOLTIP, "None")
+                    item.get(PluginSpecConstants.TOOLTIP, "None"),
                 ]
             elif table_type == TableHeaders.OUTPUT_HEADERS:
                 next_row = [
                     key,
                     item.get(PluginSpecConstants.TYPE, "None"),
                     item.get(PluginSpecConstants.REQUIRED, "None"),
                     item.get(PluginSpecConstants.DESCRIPTION, "None"),
```

### Comparing `insight_plugin-1.3.0/insight_plugin/features/create/help/input_output_helpers.py` & `insight_plugin-1.4.0/insight_plugin/features/create/help/input_output_helpers.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.3.0/insight_plugin/features/create/json_generation_util.py` & `insight_plugin-1.4.0/insight_plugin/features/create/json_generation_util.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.3.0/insight_plugin/features/create/plugin_to_helpmd.py` & `insight_plugin-1.4.0/insight_plugin/features/create/plugin_to_helpmd.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.3.0/insight_plugin/features/create/util.py` & `insight_plugin-1.4.0/insight_plugin/features/create/util.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.3.0/insight_plugin/features/export/controller.py` & `insight_plugin-1.4.0/insight_plugin/features/export/controller.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.3.0/insight_plugin/features/linter/controller.py` & `insight_plugin-1.4.0/insight_plugin/features/linter/controller.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.3.0/insight_plugin/features/refresh/controller.py` & `insight_plugin-1.4.0/insight_plugin/features/refresh/controller.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.3.0/insight_plugin/features/run/bash_controller.py` & `insight_plugin-1.4.0/insight_plugin/features/run/bash_controller.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.3.0/insight_plugin/features/run/run_controller.py` & `insight_plugin-1.4.0/insight_plugin/features/run/run_controller.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.3.0/insight_plugin/features/run/server_controller.py` & `insight_plugin-1.4.0/insight_plugin/features/run/server_controller.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.3.0/insight_plugin/features/samples/controller.py` & `insight_plugin-1.4.0/insight_plugin/features/samples/controller.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.3.0/insight_plugin/features/samples/util/constants.py` & `insight_plugin-1.4.0/insight_plugin/features/samples/util/constants.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.3.0/insight_plugin/features/samples/util/util.py` & `insight_plugin-1.4.0/insight_plugin/features/samples/util/util.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.3.0/insight_plugin/features/validate/controller.py` & `insight_plugin-1.4.0/insight_plugin/features/validate/controller.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.3.0/insight_plugin/features/version/controller.py` & `insight_plugin-1.4.0/insight_plugin/features/version/controller.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.3.0/insight_plugin/features/version/util/helpmd_util.py` & `insight_plugin-1.4.0/insight_plugin/features/version/util/helpmd_util.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.3.0/insight_plugin/features/version/util/input_util.py` & `insight_plugin-1.4.0/insight_plugin/features/version/util/input_util.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.3.0/insight_plugin/features/version/util/version_util.py` & `insight_plugin-1.4.0/insight_plugin/features/version/util/version_util.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.3.0/insight_plugin/features/version/util/yaml_util.py` & `insight_plugin-1.4.0/insight_plugin/features/version/util/yaml_util.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.3.0/insight_plugin/features/view/controller.py` & `insight_plugin-1.4.0/insight_plugin/features/view/controller.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.3.0/insight_plugin/templates/Dockerfile.jinja` & `insight_plugin-1.4.0/insight_plugin/templates/Dockerfile.jinja`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.3.0/insight_plugin/templates/Makefile.jinja` & `insight_plugin-1.4.0/insight_plugin/templates/Makefile.jinja`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.3.0/insight_plugin/templates/assessment/assessment.jinja` & `insight_plugin-1.4.0/insight_plugin/templates/assessment/assessment.jinja`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.3.0/insight_plugin/templates/bin/plugin.jinja` & `insight_plugin-1.4.0/insight_plugin/templates/bin/plugin.jinja`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.3.0/insight_plugin/templates/plugin/actions/action/action.py.jinja` & `insight_plugin-1.4.0/insight_plugin/templates/plugin/actions/action/action.py.jinja`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.3.0/insight_plugin/templates/plugin/actions/action/schema.py.jinja` & `insight_plugin-1.4.0/insight_plugin/templates/plugin/actions/action/schema.py.jinja`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.3.0/insight_plugin/templates/plugin/connection/connection.py.jinja` & `insight_plugin-1.4.0/insight_plugin/templates/plugin/connection/connection.py.jinja`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.3.0/insight_plugin/templates/plugin/tasks/task/schema.py.jinja` & `insight_plugin-1.4.0/insight_plugin/templates/plugin/tasks/task/schema.py.jinja`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.3.0/insight_plugin/templates/plugin/tasks/task/task.py.jinja` & `insight_plugin-1.4.0/insight_plugin/templates/plugin/tasks/task/task.py.jinja`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.3.0/insight_plugin/templates/plugin/triggers/trigger/schema.py.jinja` & `insight_plugin-1.4.0/insight_plugin/templates/plugin/triggers/trigger/schema.py.jinja`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.3.0/insight_plugin/templates/plugin/triggers/trigger/trigger.py.jinja` & `insight_plugin-1.4.0/insight_plugin/templates/plugin/triggers/trigger/trigger.py.jinja`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.3.0/insight_plugin/templates/unit_test/test_action.py.jinja` & `insight_plugin-1.4.0/insight_plugin/templates/unit_test/test_action.py.jinja`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.3.0/insight_plugin.egg-info/PKG-INFO` & `insight_plugin-1.4.0/insight_plugin.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: insight-plugin
-Version: 1.3.0
+Version: 1.4.0
 Summary: Plugin tooling for the Rapid7 Insight platform
 Home-page: https://github.com/rapid7/insight-plugin
 Author: Rapid7 Integrations Alliance
 Author-email: integrationalliance@rapid7.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -16,14 +16,31 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Insight Plugin - CLI Tooling for plugin development
 
 ## Commands
 
+### Analysis
+Run Static Code Analysis on the plugin.
+
+This command will run the static code analysis check on the plugin.
+
+### Linter
+Run the linter check on the plugin.
+
+This command will run the `black` linter on the plugin and return any
+formatting issues with the plugin.
+
+### Checks
+Run analysis, linter and validate on the plugin.
+
+This will allow you to recreate, locally, all the github checks that get run
+on plugins.
+
 ### Create
 Create a new plugin.
 
 This command will generate the skeleton folder structure and 
 code for a new plugin, based on the provided plugin.spec.yaml file.
 
 ### Export
```

### Comparing `insight_plugin-1.3.0/insight_plugin.egg-info/SOURCES.txt` & `insight_plugin-1.4.0/insight_plugin.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -39,18 +39,14 @@
 insight_plugin/features/create/help/constants.py
 insight_plugin/features/create/help/help_util.py
 insight_plugin/features/create/help/input_output_helpers.py
 insight_plugin/features/export/__init__.py
 insight_plugin/features/export/controller.py
 insight_plugin/features/export/util/__init__.py
 insight_plugin/features/export/util/util.py
-insight_plugin/features/interactive/__init__.py
-insight_plugin/features/interactive/controller.py
-insight_plugin/features/interactive/util/__init__.py
-insight_plugin/features/interactive/util/util.py
 insight_plugin/features/linter/__init__.py
 insight_plugin/features/linter/controller.py
 insight_plugin/features/refresh/__init__.py
 insight_plugin/features/refresh/controller.py
 insight_plugin/features/run/__init__.py
 insight_plugin/features/run/bash_controller.py
 insight_plugin/features/run/run_controller.py
@@ -101,15 +97,14 @@
 tests/__init__.py
 tests/test.py
 tests/test_checksum.py
 tests/test_create.py
 tests/test_export.py
 tests/test_gen_samples.py
 tests/test_help_creation.py
-tests/test_interactive.py
 tests/test_json_generate.py
 tests/test_refresh.py
 tests/test_run.py
 tests/test_schema.py
 tests/test_semver.py
 tests/test_spec_order.py
 tests/test_temp_file_util.py
```

### Comparing `insight_plugin-1.3.0/pyproject.toml` & `insight_plugin-1.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.3.0/setup.py` & `insight_plugin-1.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.3.0/tests/resources/export_test_base64/komand_base64/actions/decode/action.py` & `insight_plugin-1.4.0/tests/resources/export_test_base64/komand_base64/actions/decode/action.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.3.0/tests/resources/export_test_base64/komand_base64/actions/decode/schema.py` & `insight_plugin-1.4.0/tests/resources/export_test_base64/komand_base64/actions/decode/schema.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.3.0/tests/resources/export_test_base64/komand_base64/actions/encode/action.py` & `insight_plugin-1.4.0/tests/resources/export_test_base64/komand_base64/actions/encode/action.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.3.0/tests/resources/export_test_base64/komand_base64/actions/encode/schema.py` & `insight_plugin-1.4.0/tests/resources/export_test_base64/komand_base64/actions/encode/schema.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.3.0/tests/test_checksum.py` & `insight_plugin-1.4.0/tests/test_checksum.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.3.0/tests/test_create.py` & `insight_plugin-1.4.0/tests/test_create.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.3.0/tests/test_export.py` & `insight_plugin-1.4.0/tests/test_export.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.3.0/tests/test_gen_samples.py` & `insight_plugin-1.4.0/tests/test_gen_samples.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.3.0/tests/test_help_creation.py` & `insight_plugin-1.4.0/tests/test_help_creation.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.3.0/tests/test_json_generate.py` & `insight_plugin-1.4.0/tests/test_json_generate.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.3.0/tests/test_refresh.py` & `insight_plugin-1.4.0/tests/test_refresh.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.3.0/tests/test_run.py` & `insight_plugin-1.4.0/tests/test_run.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.3.0/tests/test_schema.py` & `insight_plugin-1.4.0/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.3.0/tests/test_semver.py` & `insight_plugin-1.4.0/tests/test_semver.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.3.0/tests/test_spec_order.py` & `insight_plugin-1.4.0/tests/test_spec_order.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.3.0/tests/util.py` & `insight_plugin-1.4.0/tests/util.py`

 * *Files identical despite different names*

