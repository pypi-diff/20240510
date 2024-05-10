# Comparing `tmp/insightconnect_plugin_runtime-5.4.8.tar.gz` & `tmp/insightconnect_plugin_runtime-5.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "insightconnect_plugin_runtime-5.4.8.tar", last modified: Wed May  1 10:15:18 2024, max compression
+gzip compressed data, was "insightconnect_plugin_runtime-5.4.9.tar", last modified: Fri May 10 10:27:31 2024, max compression
```

## Comparing `insightconnect_plugin_runtime-5.4.8.tar` & `insightconnect_plugin_runtime-5.4.9.tar`

### file list

```diff
@@ -1,116 +1,116 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 10:15:18.672598 insightconnect_plugin_runtime-5.4.8/
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-01 10:13:47.000000 insightconnect_plugin_runtime-5.4.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    13054 2024-05-01 10:15:18.672598 insightconnect_plugin_runtime-5.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11989 2024-05-01 10:13:47.000000 insightconnect_plugin_runtime-5.4.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    17439 2024-05-01 10:14:40.000000 insightconnect_plugin_runtime-5.4.8/insightconnect-plugin-swagger.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 10:15:18.656598 insightconnect_plugin_runtime-5.4.8/insightconnect_plugin_runtime/
--rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-05-01 10:13:47.000000 insightconnect_plugin_runtime-5.4.8/insightconnect_plugin_runtime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-01 10:13:47.000000 insightconnect_plugin_runtime-5.4.8/insightconnect_plugin_runtime/action.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 10:15:18.660598 insightconnect_plugin_runtime-5.4.8/insightconnect_plugin_runtime/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 10:13:47.000000 insightconnect_plugin_runtime-5.4.8/insightconnect_plugin_runtime/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31445 2024-05-01 10:13:47.000000 insightconnect_plugin_runtime-5.4.8/insightconnect_plugin_runtime/api/endpoints.py
--rw-r--r--   0 runner    (1001) docker     (127)     2754 2024-05-01 10:13:47.000000 insightconnect_plugin_runtime-5.4.8/insightconnect_plugin_runtime/api/schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)     8939 2024-05-01 10:13:47.000000 insightconnect_plugin_runtime-5.4.8/insightconnect_plugin_runtime/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 10:15:18.660598 insightconnect_plugin_runtime-5.4.8/insightconnect_plugin_runtime/clients/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 10:13:47.000000 insightconnect_plugin_runtime-5.4.8/insightconnect_plugin_runtime/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20290 2024-05-01 10:13:47.000000 insightconnect_plugin_runtime-5.4.8/insightconnect_plugin_runtime/clients/aws_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-05-01 10:13:47.000000 insightconnect_plugin_runtime-5.4.8/insightconnect_plugin_runtime/clients/oauth.py
--rw-r--r--   0 runner    (1001) docker     (127)     2340 2024-05-01 10:13:47.000000 insightconnect_plugin_runtime-5.4.8/insightconnect_plugin_runtime/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 10:15:18.660598 insightconnect_plugin_runtime-5.4.8/insightconnect_plugin_runtime/data/
--rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-05-01 10:13:47.000000 insightconnect_plugin_runtime-5.4.8/insightconnect_plugin_runtime/data/input_message_schema.json
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-01 10:13:47.000000 insightconnect_plugin_runtime-5.4.8/insightconnect_plugin_runtime/data/output_message_schema.json
--rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-05-01 10:13:47.000000 insightconnect_plugin_runtime-5.4.8/insightconnect_plugin_runtime/dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     6507 2024-05-01 10:13:47.000000 insightconnect_plugin_runtime-5.4.8/insightconnect_plugin_runtime/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    21108 2024-05-01 10:13:47.000000 insightconnect_plugin_runtime-5.4.8/insightconnect_plugin_runtime/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     3186 2024-05-01 10:13:47.000000 insightconnect_plugin_runtime-5.4.8/insightconnect_plugin_runtime/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    23573 2024-05-01 10:13:47.000000 insightconnect_plugin_runtime-5.4.8/insightconnect_plugin_runtime/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-01 10:13:47.000000 insightconnect_plugin_runtime-5.4.8/insightconnect_plugin_runtime/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)    12195 2024-05-01 10:13:47.000000 insightconnect_plugin_runtime-5.4.8/insightconnect_plugin_runtime/server.py
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-05-01 10:13:47.000000 insightconnect_plugin_runtime-5.4.8/insightconnect_plugin_runtime/step.py
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-01 10:13:47.000000 insightconnect_plugin_runtime-5.4.8/insightconnect_plugin_runtime/task.py
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-05-01 10:13:47.000000 insightconnect_plugin_runtime-5.4.8/insightconnect_plugin_runtime/trigger.py
--rw-r--r--   0 runner    (1001) docker     (127)     8398 2024-05-01 10:13:47.000000 insightconnect_plugin_runtime-5.4.8/insightconnect_plugin_runtime/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-05-01 10:13:47.000000 insightconnect_plugin_runtime-5.4.8/insightconnect_plugin_runtime/variables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 10:15:18.672598 insightconnect_plugin_runtime-5.4.8/insightconnect_plugin_runtime.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13054 2024-05-01 10:15:18.000000 insightconnect_plugin_runtime-5.4.8/insightconnect_plugin_runtime.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4785 2024-05-01 10:15:18.000000 insightconnect_plugin_runtime-5.4.8/insightconnect_plugin_runtime.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 10:15:18.000000 insightconnect_plugin_runtime-5.4.8/insightconnect_plugin_runtime.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-01 10:15:18.000000 insightconnect_plugin_runtime-5.4.8/insightconnect_plugin_runtime.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-01 10:15:18.000000 insightconnect_plugin_runtime-5.4.8/insightconnect_plugin_runtime.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 10:15:18.672598 insightconnect_plugin_runtime-5.4.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-05-01 10:13:47.000000 insightconnect_plugin_runtime-5.4.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 10:15:18.660598 insightconnect_plugin_runtime-5.4.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-01 10:13:47.000000 insightconnect_plugin_runtime-5.4.8/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 10:15:18.660598 insightconnect_plugin_runtime-5.4.8/tests/plugin/
--rw-r--r--   0 runner    (1001) docker     (127)     2712 2024-05-01 10:13:47.000000 insightconnect_plugin_runtime-5.4.8/tests/plugin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 10:15:18.660598 insightconnect_plugin_runtime-5.4.8/tests/plugin/hello_world/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-01 10:13:47.000000 insightconnect_plugin_runtime-5.4.8/tests/plugin/hello_world/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 10:15:18.660598 insightconnect_plugin_runtime-5.4.8/tests/plugin/hello_world/hello_world/
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-05-01 10:13:47.000000 insightconnect_plugin_runtime-5.4.8/tests/plugin/hello_world/hello_world/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 10:15:18.660598 insightconnect_plugin_runtime-5.4.8/tests/plugin/hello_world/hello_world/komand_hello_world/
--rwxr-xr-x   0 runner    (1001) docker     (127)       40 2024-05-01 10:13:47.000000 insightconnect_plugin_runtime-5.4.8/tests/plugin/hello_world/hello_world/komand_hello_world/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 10:15:18.660598 insightconnect_plugin_runtime-5.4.8/tests/plugin/hello_world/hello_world/komand_hello_world/actions/
--rwxr-xr-x   0 runner    (1001) docker     (127)      173 2024-05-01 10:13:47.000000 insightconnect_plugin_runtime-5.4.8/tests/plugin/hello_world/hello_world/komand_hello_world/actions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 10:15:18.660598 insightconnect_plugin_runtime-5.4.8/tests/plugin/hello_world/hello_world/komand_hello_world/actions/hello/
--rwxr-xr-x   0 runner    (1001) docker     (127)       66 2024-05-01 10:13:47.000000 insightconnect_plugin_runtime-5.4.8/tests/plugin/hello_world/hello_world/komand_hello_world/actions/hello/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      642 2024-05-01 10:13:47.000000 insightconnect_plugin_runtime-5.4.8/tests/plugin/hello_world/hello_world/komand_hello_world/actions/hello/action.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      930 2024-05-01 10:13:47.000000 insightconnect_plugin_runtime-5.4.8/tests/plugin/hello_world/hello_world/komand_hello_world/actions/hello/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 10:15:18.660598 insightconnect_plugin_runtime-5.4.8/tests/plugin/hello_world/hello_world/komand_hello_world/actions/return_bad_json/
--rwxr-xr-x   0 runner    (1001) docker     (127)       74 2024-05-01 10:13:47.000000 insightconnect_plugin_runtime-5.4.8/tests/plugin/hello_world/hello_world/komand_hello_world/actions/return_bad_json/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      631 2024-05-01 10:13:47.000000 insightconnect_plugin_runtime-5.4.8/tests/plugin/hello_world/hello_world/komand_hello_world/actions/return_bad_json/action.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      946 2024-05-01 10:13:47.000000 insightconnect_plugin_runtime-5.4.8/tests/plugin/hello_world/hello_world/komand_hello_world/actions/return_bad_json/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 10:15:18.664599 insightconnect_plugin_runtime-5.4.8/tests/plugin/hello_world/hello_world/komand_hello_world/actions/throw_exception/
--rwxr-xr-x   0 runner    (1001) docker     (127)       75 2024-05-01 10:13:47.000000 insightconnect_plugin_runtime-5.4.8/tests/plugin/hello_world/hello_world/komand_hello_world/actions/throw_exception/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1077 2024-05-01 10:13:47.000000 insightconnect_plugin_runtime-5.4.8/tests/plugin/hello_world/hello_world/komand_hello_world/actions/throw_exception/action.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1101 2024-05-01 10:13:47.000000 insightconnect_plugin_runtime-5.4.8/tests/plugin/hello_world/hello_world/komand_hello_world/actions/throw_exception/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 10:15:18.664599 insightconnect_plugin_runtime-5.4.8/tests/plugin/hello_world/hello_world/komand_hello_world/connection/
--rwxr-xr-x   0 runner    (1001) docker     (127)       75 2024-05-01 10:13:47.000000 insightconnect_plugin_runtime-5.4.8/tests/plugin/hello_world/hello_world/komand_hello_world/connection/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      375 2024-05-01 10:13:47.000000 insightconnect_plugin_runtime-5.4.8/tests/plugin/hello_world/hello_world/komand_hello_world/connection/connection.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      517 2024-05-01 10:13:47.000000 insightconnect_plugin_runtime-5.4.8/tests/plugin/hello_world/hello_world/komand_hello_world/connection/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 10:15:18.664599 insightconnect_plugin_runtime-5.4.8/tests/plugin/hello_world/hello_world/komand_hello_world/tasks/
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-01 10:13:47.000000 insightconnect_plugin_runtime-5.4.8/tests/plugin/hello_world/hello_world/komand_hello_world/tasks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 10:15:18.664599 insightconnect_plugin_runtime-5.4.8/tests/plugin/hello_world/hello_world/komand_hello_world/tasks/monitor_events/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-01 10:13:47.000000 insightconnect_plugin_runtime-5.4.8/tests/plugin/hello_world/hello_world/komand_hello_world/tasks/monitor_events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-01 10:13:47.000000 insightconnect_plugin_runtime-5.4.8/tests/plugin/hello_world/hello_world/komand_hello_world/tasks/monitor_events/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-05-01 10:13:47.000000 insightconnect_plugin_runtime-5.4.8/tests/plugin/hello_world/hello_world/komand_hello_world/tasks/monitor_events/task.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 10:15:18.664599 insightconnect_plugin_runtime-5.4.8/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/
--rwxr-xr-x   0 runner    (1001) docker     (127)      221 2024-05-01 10:13:47.000000 insightconnect_plugin_runtime-5.4.8/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 10:15:18.664599 insightconnect_plugin_runtime-5.4.8/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/hello_trigger/
--rwxr-xr-x   0 runner    (1001) docker     (127)       74 2024-05-01 10:13:47.000000 insightconnect_plugin_runtime-5.4.8/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/hello_trigger/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      944 2024-05-01 10:13:47.000000 insightconnect_plugin_runtime-5.4.8/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/hello_trigger/schema.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1148 2024-05-01 10:13:47.000000 insightconnect_plugin_runtime-5.4.8/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/hello_trigger/trigger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 10:15:18.664599 insightconnect_plugin_runtime-5.4.8/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/return_bad_json_trigger/
--rwxr-xr-x   0 runner    (1001) docker     (127)       82 2024-05-01 10:13:47.000000 insightconnect_plugin_runtime-5.4.8/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/return_bad_json_trigger/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      960 2024-05-01 10:13:47.000000 insightconnect_plugin_runtime-5.4.8/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/return_bad_json_trigger/schema.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      717 2024-05-01 10:13:47.000000 insightconnect_plugin_runtime-5.4.8/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/return_bad_json_trigger/trigger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 10:15:18.664599 insightconnect_plugin_runtime-5.4.8/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/throw_exception_trigger/
--rwxr-xr-x   0 runner    (1001) docker     (127)       83 2024-05-01 10:13:47.000000 insightconnect_plugin_runtime-5.4.8/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/throw_exception_trigger/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      962 2024-05-01 10:13:47.000000 insightconnect_plugin_runtime-5.4.8/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/throw_exception_trigger/schema.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      696 2024-05-01 10:13:47.000000 insightconnect_plugin_runtime-5.4.8/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/throw_exception_trigger/trigger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 10:15:18.664599 insightconnect_plugin_runtime-5.4.8/tests/plugin/hello_world/hello_world/komand_hello_world/util/
--rwxr-xr-x   0 runner    (1001) docker     (127)       40 2024-05-01 10:13:47.000000 insightconnect_plugin_runtime-5.4.8/tests/plugin/hello_world/hello_world/komand_hello_world/util/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      467 2024-05-01 10:13:47.000000 insightconnect_plugin_runtime-5.4.8/tests/plugin/hello_world/hello_world/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 10:15:18.668599 insightconnect_plugin_runtime-5.4.8/tests/plugin/hello_world/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 10:13:47.000000 insightconnect_plugin_runtime-5.4.8/tests/plugin/hello_world/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-05-01 10:13:47.000000 insightconnect_plugin_runtime-5.4.8/tests/plugin/hello_world/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     4049 2024-05-01 10:13:47.000000 insightconnect_plugin_runtime-5.4.8/tests/plugin/hello_world/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-05-01 10:13:47.000000 insightconnect_plugin_runtime-5.4.8/tests/plugin/hello_world/tests/test_hello_world.py
--rw-r--r--   0 runner    (1001) docker     (127)     4071 2024-05-01 10:13:47.000000 insightconnect_plugin_runtime-5.4.8/tests/plugin/hello_world/tests/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 10:15:18.668599 insightconnect_plugin_runtime-5.4.8/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 10:13:47.000000 insightconnect_plugin_runtime-5.4.8/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-05-01 10:13:47.000000 insightconnect_plugin_runtime-5.4.8/tests/unit/test_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     4441 2024-05-01 10:13:47.000000 insightconnect_plugin_runtime-5.4.8/tests/unit/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     7952 2024-05-01 10:13:47.000000 insightconnect_plugin_runtime-5.4.8/tests/unit/test_aws_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     2207 2024-05-01 10:13:47.000000 insightconnect_plugin_runtime-5.4.8/tests/unit/test_custom_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     6401 2024-05-01 10:13:47.000000 insightconnect_plugin_runtime-5.4.8/tests/unit/test_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (127)     4668 2024-05-01 10:13:47.000000 insightconnect_plugin_runtime-5.4.8/tests/unit/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     8542 2024-05-01 10:13:47.000000 insightconnect_plugin_runtime-5.4.8/tests/unit/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7979 2024-05-01 10:13:47.000000 insightconnect_plugin_runtime-5.4.8/tests/unit/test_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-05-01 10:13:47.000000 insightconnect_plugin_runtime-5.4.8/tests/unit/test_oauth.py
--rw-r--r--   0 runner    (1001) docker     (127)     4160 2024-05-01 10:13:47.000000 insightconnect_plugin_runtime-5.4.8/tests/unit/test_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-05-01 10:13:47.000000 insightconnect_plugin_runtime-5.4.8/tests/unit/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     5096 2024-05-01 10:13:47.000000 insightconnect_plugin_runtime-5.4.8/tests/unit/test_server_cloud_plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-05-01 10:13:47.000000 insightconnect_plugin_runtime-5.4.8/tests/unit/test_server_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-05-01 10:13:47.000000 insightconnect_plugin_runtime-5.4.8/tests/unit/test_trigger.py
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-01 10:13:47.000000 insightconnect_plugin_runtime-5.4.8/tests/unit/test_variables.py
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-01 10:13:47.000000 insightconnect_plugin_runtime-5.4.8/tests/unit/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:27:31.855387 insightconnect_plugin_runtime-5.4.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-10 10:26:07.000000 insightconnect_plugin_runtime-5.4.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    13159 2024-05-10 10:27:31.855387 insightconnect_plugin_runtime-5.4.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12094 2024-05-10 10:26:07.000000 insightconnect_plugin_runtime-5.4.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    17439 2024-05-10 10:26:56.000000 insightconnect_plugin_runtime-5.4.9/insightconnect-plugin-swagger.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:27:31.843387 insightconnect_plugin_runtime-5.4.9/insightconnect_plugin_runtime/
+-rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-05-10 10:26:07.000000 insightconnect_plugin_runtime-5.4.9/insightconnect_plugin_runtime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-10 10:26:07.000000 insightconnect_plugin_runtime-5.4.9/insightconnect_plugin_runtime/action.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:27:31.843387 insightconnect_plugin_runtime-5.4.9/insightconnect_plugin_runtime/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 10:26:07.000000 insightconnect_plugin_runtime-5.4.9/insightconnect_plugin_runtime/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31445 2024-05-10 10:26:07.000000 insightconnect_plugin_runtime-5.4.9/insightconnect_plugin_runtime/api/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2754 2024-05-10 10:26:07.000000 insightconnect_plugin_runtime-5.4.9/insightconnect_plugin_runtime/api/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8939 2024-05-10 10:26:07.000000 insightconnect_plugin_runtime-5.4.9/insightconnect_plugin_runtime/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:27:31.847386 insightconnect_plugin_runtime-5.4.9/insightconnect_plugin_runtime/clients/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 10:26:07.000000 insightconnect_plugin_runtime-5.4.9/insightconnect_plugin_runtime/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20508 2024-05-10 10:26:07.000000 insightconnect_plugin_runtime-5.4.9/insightconnect_plugin_runtime/clients/aws_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-05-10 10:26:07.000000 insightconnect_plugin_runtime-5.4.9/insightconnect_plugin_runtime/clients/oauth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2340 2024-05-10 10:26:07.000000 insightconnect_plugin_runtime-5.4.9/insightconnect_plugin_runtime/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:27:31.847386 insightconnect_plugin_runtime-5.4.9/insightconnect_plugin_runtime/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-05-10 10:26:07.000000 insightconnect_plugin_runtime-5.4.9/insightconnect_plugin_runtime/data/input_message_schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-10 10:26:07.000000 insightconnect_plugin_runtime-5.4.9/insightconnect_plugin_runtime/data/output_message_schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-05-10 10:26:07.000000 insightconnect_plugin_runtime-5.4.9/insightconnect_plugin_runtime/dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6507 2024-05-10 10:26:07.000000 insightconnect_plugin_runtime-5.4.9/insightconnect_plugin_runtime/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21108 2024-05-10 10:26:07.000000 insightconnect_plugin_runtime-5.4.9/insightconnect_plugin_runtime/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3186 2024-05-10 10:26:07.000000 insightconnect_plugin_runtime-5.4.9/insightconnect_plugin_runtime/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23573 2024-05-10 10:26:07.000000 insightconnect_plugin_runtime-5.4.9/insightconnect_plugin_runtime/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-10 10:26:07.000000 insightconnect_plugin_runtime-5.4.9/insightconnect_plugin_runtime/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12195 2024-05-10 10:26:07.000000 insightconnect_plugin_runtime-5.4.9/insightconnect_plugin_runtime/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-05-10 10:26:07.000000 insightconnect_plugin_runtime-5.4.9/insightconnect_plugin_runtime/step.py
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-10 10:26:07.000000 insightconnect_plugin_runtime-5.4.9/insightconnect_plugin_runtime/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-05-10 10:26:07.000000 insightconnect_plugin_runtime-5.4.9/insightconnect_plugin_runtime/trigger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8398 2024-05-10 10:26:07.000000 insightconnect_plugin_runtime-5.4.9/insightconnect_plugin_runtime/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-05-10 10:26:07.000000 insightconnect_plugin_runtime-5.4.9/insightconnect_plugin_runtime/variables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:27:31.855387 insightconnect_plugin_runtime-5.4.9/insightconnect_plugin_runtime.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13159 2024-05-10 10:27:31.000000 insightconnect_plugin_runtime-5.4.9/insightconnect_plugin_runtime.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4785 2024-05-10 10:27:31.000000 insightconnect_plugin_runtime-5.4.9/insightconnect_plugin_runtime.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 10:27:31.000000 insightconnect_plugin_runtime-5.4.9/insightconnect_plugin_runtime.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-10 10:27:31.000000 insightconnect_plugin_runtime-5.4.9/insightconnect_plugin_runtime.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-10 10:27:31.000000 insightconnect_plugin_runtime-5.4.9/insightconnect_plugin_runtime.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 10:27:31.855387 insightconnect_plugin_runtime-5.4.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-05-10 10:26:07.000000 insightconnect_plugin_runtime-5.4.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:27:31.847386 insightconnect_plugin_runtime-5.4.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-10 10:26:07.000000 insightconnect_plugin_runtime-5.4.9/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:27:31.847386 insightconnect_plugin_runtime-5.4.9/tests/plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)     2712 2024-05-10 10:26:07.000000 insightconnect_plugin_runtime-5.4.9/tests/plugin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:27:31.847386 insightconnect_plugin_runtime-5.4.9/tests/plugin/hello_world/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-10 10:26:07.000000 insightconnect_plugin_runtime-5.4.9/tests/plugin/hello_world/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:27:31.847386 insightconnect_plugin_runtime-5.4.9/tests/plugin/hello_world/hello_world/
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-05-10 10:26:07.000000 insightconnect_plugin_runtime-5.4.9/tests/plugin/hello_world/hello_world/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:27:31.847386 insightconnect_plugin_runtime-5.4.9/tests/plugin/hello_world/hello_world/komand_hello_world/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       40 2024-05-10 10:26:07.000000 insightconnect_plugin_runtime-5.4.9/tests/plugin/hello_world/hello_world/komand_hello_world/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:27:31.847386 insightconnect_plugin_runtime-5.4.9/tests/plugin/hello_world/hello_world/komand_hello_world/actions/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      173 2024-05-10 10:26:07.000000 insightconnect_plugin_runtime-5.4.9/tests/plugin/hello_world/hello_world/komand_hello_world/actions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:27:31.847386 insightconnect_plugin_runtime-5.4.9/tests/plugin/hello_world/hello_world/komand_hello_world/actions/hello/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       66 2024-05-10 10:26:07.000000 insightconnect_plugin_runtime-5.4.9/tests/plugin/hello_world/hello_world/komand_hello_world/actions/hello/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      642 2024-05-10 10:26:07.000000 insightconnect_plugin_runtime-5.4.9/tests/plugin/hello_world/hello_world/komand_hello_world/actions/hello/action.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      930 2024-05-10 10:26:07.000000 insightconnect_plugin_runtime-5.4.9/tests/plugin/hello_world/hello_world/komand_hello_world/actions/hello/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:27:31.847386 insightconnect_plugin_runtime-5.4.9/tests/plugin/hello_world/hello_world/komand_hello_world/actions/return_bad_json/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       74 2024-05-10 10:26:07.000000 insightconnect_plugin_runtime-5.4.9/tests/plugin/hello_world/hello_world/komand_hello_world/actions/return_bad_json/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      631 2024-05-10 10:26:07.000000 insightconnect_plugin_runtime-5.4.9/tests/plugin/hello_world/hello_world/komand_hello_world/actions/return_bad_json/action.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      946 2024-05-10 10:26:07.000000 insightconnect_plugin_runtime-5.4.9/tests/plugin/hello_world/hello_world/komand_hello_world/actions/return_bad_json/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:27:31.847386 insightconnect_plugin_runtime-5.4.9/tests/plugin/hello_world/hello_world/komand_hello_world/actions/throw_exception/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       75 2024-05-10 10:26:07.000000 insightconnect_plugin_runtime-5.4.9/tests/plugin/hello_world/hello_world/komand_hello_world/actions/throw_exception/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1077 2024-05-10 10:26:07.000000 insightconnect_plugin_runtime-5.4.9/tests/plugin/hello_world/hello_world/komand_hello_world/actions/throw_exception/action.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1101 2024-05-10 10:26:07.000000 insightconnect_plugin_runtime-5.4.9/tests/plugin/hello_world/hello_world/komand_hello_world/actions/throw_exception/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:27:31.851387 insightconnect_plugin_runtime-5.4.9/tests/plugin/hello_world/hello_world/komand_hello_world/connection/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       75 2024-05-10 10:26:07.000000 insightconnect_plugin_runtime-5.4.9/tests/plugin/hello_world/hello_world/komand_hello_world/connection/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      375 2024-05-10 10:26:07.000000 insightconnect_plugin_runtime-5.4.9/tests/plugin/hello_world/hello_world/komand_hello_world/connection/connection.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      517 2024-05-10 10:26:07.000000 insightconnect_plugin_runtime-5.4.9/tests/plugin/hello_world/hello_world/komand_hello_world/connection/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:27:31.851387 insightconnect_plugin_runtime-5.4.9/tests/plugin/hello_world/hello_world/komand_hello_world/tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-10 10:26:07.000000 insightconnect_plugin_runtime-5.4.9/tests/plugin/hello_world/hello_world/komand_hello_world/tasks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:27:31.851387 insightconnect_plugin_runtime-5.4.9/tests/plugin/hello_world/hello_world/komand_hello_world/tasks/monitor_events/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-10 10:26:07.000000 insightconnect_plugin_runtime-5.4.9/tests/plugin/hello_world/hello_world/komand_hello_world/tasks/monitor_events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-10 10:26:07.000000 insightconnect_plugin_runtime-5.4.9/tests/plugin/hello_world/hello_world/komand_hello_world/tasks/monitor_events/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-05-10 10:26:07.000000 insightconnect_plugin_runtime-5.4.9/tests/plugin/hello_world/hello_world/komand_hello_world/tasks/monitor_events/task.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:27:31.851387 insightconnect_plugin_runtime-5.4.9/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      221 2024-05-10 10:26:07.000000 insightconnect_plugin_runtime-5.4.9/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:27:31.851387 insightconnect_plugin_runtime-5.4.9/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/hello_trigger/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       74 2024-05-10 10:26:07.000000 insightconnect_plugin_runtime-5.4.9/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/hello_trigger/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      944 2024-05-10 10:26:07.000000 insightconnect_plugin_runtime-5.4.9/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/hello_trigger/schema.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1148 2024-05-10 10:26:07.000000 insightconnect_plugin_runtime-5.4.9/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/hello_trigger/trigger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:27:31.851387 insightconnect_plugin_runtime-5.4.9/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/return_bad_json_trigger/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       82 2024-05-10 10:26:07.000000 insightconnect_plugin_runtime-5.4.9/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/return_bad_json_trigger/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      960 2024-05-10 10:26:07.000000 insightconnect_plugin_runtime-5.4.9/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/return_bad_json_trigger/schema.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      717 2024-05-10 10:26:07.000000 insightconnect_plugin_runtime-5.4.9/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/return_bad_json_trigger/trigger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:27:31.851387 insightconnect_plugin_runtime-5.4.9/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/throw_exception_trigger/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       83 2024-05-10 10:26:07.000000 insightconnect_plugin_runtime-5.4.9/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/throw_exception_trigger/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      962 2024-05-10 10:26:07.000000 insightconnect_plugin_runtime-5.4.9/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/throw_exception_trigger/schema.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      696 2024-05-10 10:26:07.000000 insightconnect_plugin_runtime-5.4.9/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/throw_exception_trigger/trigger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:27:31.851387 insightconnect_plugin_runtime-5.4.9/tests/plugin/hello_world/hello_world/komand_hello_world/util/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       40 2024-05-10 10:26:07.000000 insightconnect_plugin_runtime-5.4.9/tests/plugin/hello_world/hello_world/komand_hello_world/util/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      467 2024-05-10 10:26:07.000000 insightconnect_plugin_runtime-5.4.9/tests/plugin/hello_world/hello_world/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:27:31.851387 insightconnect_plugin_runtime-5.4.9/tests/plugin/hello_world/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 10:26:07.000000 insightconnect_plugin_runtime-5.4.9/tests/plugin/hello_world/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-05-10 10:26:07.000000 insightconnect_plugin_runtime-5.4.9/tests/plugin/hello_world/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4049 2024-05-10 10:26:07.000000 insightconnect_plugin_runtime-5.4.9/tests/plugin/hello_world/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-05-10 10:26:07.000000 insightconnect_plugin_runtime-5.4.9/tests/plugin/hello_world/tests/test_hello_world.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4071 2024-05-10 10:26:07.000000 insightconnect_plugin_runtime-5.4.9/tests/plugin/hello_world/tests/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:27:31.855387 insightconnect_plugin_runtime-5.4.9/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 10:26:07.000000 insightconnect_plugin_runtime-5.4.9/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-05-10 10:26:07.000000 insightconnect_plugin_runtime-5.4.9/tests/unit/test_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4441 2024-05-10 10:26:07.000000 insightconnect_plugin_runtime-5.4.9/tests/unit/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7952 2024-05-10 10:26:07.000000 insightconnect_plugin_runtime-5.4.9/tests/unit/test_aws_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2207 2024-05-10 10:26:07.000000 insightconnect_plugin_runtime-5.4.9/tests/unit/test_custom_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6401 2024-05-10 10:26:07.000000 insightconnect_plugin_runtime-5.4.9/tests/unit/test_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4668 2024-05-10 10:26:07.000000 insightconnect_plugin_runtime-5.4.9/tests/unit/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8542 2024-05-10 10:26:07.000000 insightconnect_plugin_runtime-5.4.9/tests/unit/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7979 2024-05-10 10:26:07.000000 insightconnect_plugin_runtime-5.4.9/tests/unit/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-05-10 10:26:07.000000 insightconnect_plugin_runtime-5.4.9/tests/unit/test_oauth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4160 2024-05-10 10:26:07.000000 insightconnect_plugin_runtime-5.4.9/tests/unit/test_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-05-10 10:26:07.000000 insightconnect_plugin_runtime-5.4.9/tests/unit/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5096 2024-05-10 10:26:07.000000 insightconnect_plugin_runtime-5.4.9/tests/unit/test_server_cloud_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-05-10 10:26:07.000000 insightconnect_plugin_runtime-5.4.9/tests/unit/test_server_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-05-10 10:26:07.000000 insightconnect_plugin_runtime-5.4.9/tests/unit/test_trigger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-10 10:26:07.000000 insightconnect_plugin_runtime-5.4.9/tests/unit/test_variables.py
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-10 10:26:07.000000 insightconnect_plugin_runtime-5.4.9/tests/unit/utils.py
```

### Comparing `insightconnect_plugin_runtime-5.4.8/PKG-INFO` & `insightconnect_plugin_runtime-5.4.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: insightconnect-plugin-runtime
-Version: 5.4.8
+Version: 5.4.9
 Summary: InsightConnect Plugin Runtime
 Home-page: https://github.com/rapid7/komand-plugin-sdk-python
 Author: Rapid7 Integrations Alliance
 Author-email: integrationalliance@rapid7.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
@@ -207,14 +207,15 @@
 
 Contributions for maintaining and enhancing the InsightConnect Python Plugin Runtime are appreciated. This project uses
 [Black](https://github.com/psf/black) for code formatting and includes a pre-commit hook to auto format code as it is
 contributed. Black is installed as a test dependency and the hook can be initialized by running `pre-commit install` 
 after cloning this repository.
 
 ## Changelog
+* 5.4.9 - Updated aws_client to clean assume role json object to remove any none or empty string values.
 * 5.4.8 - Address vulnerabilities within `gunicorn` and `idna` python packages.
 * 5.4.7 - Address vulnerabilities within `insightconnect-python-3-plugin` image.
 * 5.4.6 - Updated our cloud loggers to include the request path | Updated slim image to remediate vulnerabilities.
 * 5.4.5 - Updated base images to pull Python 3.9.19 | Alpine image: Updated expat package
 * 5.4.4 - Handling the 'Connection Refused' to cps (during startup) as an info instead of error log as this is an expected error.
 * 5.4.3 - Updated dependencies to the latest versions | Fixed issue related to logger `StreamHandlers`
 * 5.4.2 - Remove background scheduler to simplify when the server gets custom_config values | Revert to use `bullseye` for slim image.
```

### Comparing `insightconnect_plugin_runtime-5.4.8/README.md` & `insightconnect_plugin_runtime-5.4.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -178,14 +178,15 @@
 
 Contributions for maintaining and enhancing the InsightConnect Python Plugin Runtime are appreciated. This project uses
 [Black](https://github.com/psf/black) for code formatting and includes a pre-commit hook to auto format code as it is
 contributed. Black is installed as a test dependency and the hook can be initialized by running `pre-commit install` 
 after cloning this repository.
 
 ## Changelog
+* 5.4.9 - Updated aws_client to clean assume role json object to remove any none or empty string values.
 * 5.4.8 - Address vulnerabilities within `gunicorn` and `idna` python packages.
 * 5.4.7 - Address vulnerabilities within `insightconnect-python-3-plugin` image.
 * 5.4.6 - Updated our cloud loggers to include the request path | Updated slim image to remediate vulnerabilities.
 * 5.4.5 - Updated base images to pull Python 3.9.19 | Alpine image: Updated expat package
 * 5.4.4 - Handling the 'Connection Refused' to cps (during startup) as an info instead of error log as this is an expected error.
 * 5.4.3 - Updated dependencies to the latest versions | Fixed issue related to logger `StreamHandlers`
 * 5.4.2 - Remove background scheduler to simplify when the server gets custom_config values | Revert to use `bullseye` for slim image.
```

### Comparing `insightconnect_plugin_runtime-5.4.8/insightconnect-plugin-swagger.json` & `insightconnect_plugin_runtime-5.4.9/insightconnect-plugin-swagger.json`

 * *Files identical despite different names*

### Comparing `insightconnect_plugin_runtime-5.4.8/insightconnect_plugin_runtime/__init__.py` & `insightconnect_plugin_runtime-5.4.9/insightconnect_plugin_runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `insightconnect_plugin_runtime-5.4.8/insightconnect_plugin_runtime/api/endpoints.py` & `insightconnect_plugin_runtime-5.4.9/insightconnect_plugin_runtime/api/endpoints.py`

 * *Files identical despite different names*

### Comparing `insightconnect_plugin_runtime-5.4.8/insightconnect_plugin_runtime/api/schemas.py` & `insightconnect_plugin_runtime-5.4.9/insightconnect_plugin_runtime/api/schemas.py`

 * *Files identical despite different names*

### Comparing `insightconnect_plugin_runtime-5.4.8/insightconnect_plugin_runtime/cli.py` & `insightconnect_plugin_runtime-5.4.9/insightconnect_plugin_runtime/cli.py`

 * *Files identical despite different names*

### Comparing `insightconnect_plugin_runtime-5.4.8/insightconnect_plugin_runtime/clients/aws_client.py` & `insightconnect_plugin_runtime-5.4.9/insightconnect_plugin_runtime/clients/aws_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,34 +11,35 @@
 import botocore.session
 import requests
 from botocore.exceptions import ClientError
 
 import insightconnect_plugin_runtime
 from insightconnect_plugin_runtime.action import Action
 from insightconnect_plugin_runtime.exceptions import PluginException
+from insightconnect_plugin_runtime.helper import clean
 
 REGION = "region"
 EXTERNAL_ID = "external_id"
 ROLE_ARN = "role_arn"
 ASSUME_ROLE_PARAMETERS = "assume_role_params"
 
 
 class PaginationHelper:
     """
     A helper class for dealing with paginated requests.
     """
 
     def __init__(
-        self,
-        input_token: List[str],
-        output_token: List[str],
-        result_key: List[str],
-        limit_key: str = None,
-        more_results: str = None,
-        non_aggregate_keys: List[str] = None,
+            self,
+            input_token: List[str],
+            output_token: List[str],
+            result_key: List[str],
+            limit_key: str = None,
+            more_results: str = None,
+            non_aggregate_keys: List[str] = None,
     ):
         self.input_token = input_token
         self.output_token = output_token
         self.result_key = result_key
         self.limit_key = limit_key
         self.more_results = more_results
         self.non_aggregate_keys = non_aggregate_keys
@@ -65,32 +66,32 @@
         :param output: The output variables
         :return: True if more results are available, False otherwise
         """
 
         is_paginated = False
 
         if (
-            self.more_results
-            and self.more_results in output.keys()
-            and output[self.more_results]
+                self.more_results
+                and self.more_results in output.keys()
+                and output[self.more_results]
         ):
             is_paginated = True
 
         for idx, _ in enumerate(self.input_token):
             if self.output_token[idx] in output.keys():
                 input_[self.input_token[idx]] = output[self.output_token[idx]]
                 is_paginated = True
 
         return is_paginated
 
     def merge_responses(
-        self,
-        input_: Dict[str, Any],
-        response_1: Dict[str, Any],
-        response_2: Dict[str, Any],
+            self,
+            input_: Dict[str, Any],
+            response_1: Dict[str, Any],
+            response_2: Dict[str, Any],
     ) -> Tuple[Dict[str, Any], bool]:
         """
         Merges two output dictionaries together.
         :param input_: Input dictionary containing limit_key
         :type: Dict[str, Any]
         :param response_1: First input response
         :type: Dict[str, Any]
@@ -107,16 +108,15 @@
             response_1[response] = response_2[response]
             response_1[response].extend(temporary_1)
 
             if self.limit_key and self.limit_key in input_.keys():
                 if len(response_1[response]) >= input_[self.limit_key]:
                     max_hit = True
                     response_1[response] = response_1[response][
-                        : input_[self.limit_key]
-                    ]
+                                           : input_[self.limit_key]]
 
         return response_1, max_hit
 
 
 class ActionHelper:
     """
     Helper class for invoking AWS.
@@ -298,15 +298,15 @@
                 new_obj.append(new_list)
             return new_obj
         else:
             return obj
 
     @classmethod
     def format_output(
-        cls, output_schema: Union[Dict[str, Any], None], output: Dict[str, Any]
+            cls, output_schema: Union[Dict[str, Any], None], output: Dict[str, Any]
     ) -> Any:
         """
         Formats a botocore response into a correct Komand response.
 
         Keys are formatted to snake case.
 
         :param output_schema: The output json schema
@@ -329,22 +329,22 @@
 
 class AWSAction(Action):
     """
     Abstract class for handling any aws-cli request.
     """
 
     def __init__(
-        self,
-        name: str,
-        description: str,
-        input_: insightconnect_plugin_runtime.Input,
-        output: insightconnect_plugin_runtime.Output,
-        aws_service: str,
-        aws_command: str,
-        pagination_helper: PaginationHelper = None,
+            self,
+            name: str,
+            description: str,
+            input_: insightconnect_plugin_runtime.Input,
+            output: insightconnect_plugin_runtime.Output,
+            aws_service: str,
+            aws_command: str,
+            pagination_helper: PaginationHelper = None,
     ):
         """
 
         Initializes a new AwsAction object.
 
         :param name: The name of the action. Should be snake case.
         :param description: The description fo the action.
@@ -358,15 +358,15 @@
             name=name, description=description, input=input_, output=output
         )
         self.aws_service = aws_service
         self.aws_command = aws_command
         self.pagination_helper = pagination_helper
 
     def _handle_botocore_function(
-        self, client_function: Callable, params: Dict
+            self, client_function: Callable, params: Dict
     ) -> Dict:
         try:
             response = client_function(**params)
         except botocore.exceptions.NoRegionError as error:
             self.logger.error(
                 f"Error occurred when invoking the aws-cli. No region specified. Boto3 response: {error}"
             )
@@ -476,19 +476,19 @@
             )
 
         # There exists a function for each command in the service client object.
         try:
             client_function = getattr(client, self.aws_command)
         except AttributeError:
             error_message = (
-                'Unable to find the command "'
-                + self.aws_service
-                + " "
-                + self.aws_command
-                + '"'
+                    'Unable to find the command "'
+                    + self.aws_service
+                    + " "
+                    + self.aws_command
+                    + '"'
             )
             self.logger.error(error_message)
             raise PluginException(cause=error_message)
 
         response = self.handle_rest_call(client_function, params)
 
         # Handle possible pagination if this action supports pagination.
@@ -529,25 +529,25 @@
         else:
             response = helper.format_output(None, {})
 
         return response
 
     @staticmethod
     def try_to_assume_role(
-        service_name: str,
-        assume_role_params: Dict[str, str],
-        auth_params: Dict[str, str],
+            service_name: str,
+            assume_role_params: Dict[str, str],
+            auth_params: Dict[str, str],
     ):
         session_name = str(uuid.uuid1())
         sts_client = boto3.client("sts", **auth_params)
         try:
             assumed_role_object = sts_client.assume_role(
-                RoleArn=assume_role_params.get(ROLE_ARN),
-                RoleSessionName=session_name,
-                ExternalId=assume_role_params.get(EXTERNAL_ID),
+                **clean({"RoleArn": assume_role_params.get(ROLE_ARN),
+                         "RoleSessionName": session_name,
+                         "ExternalId": assume_role_params.get(EXTERNAL_ID)})
             )
         except ClientError as error:
             raise PluginException(
                 cause=f"Boto3 raised following error during assume role: {error.response['Error']['Code']}",
                 assistance="Please verify your role ARN and external ID are correct",
             )
         credentials = assumed_role_object["Credentials"]
```

### Comparing `insightconnect_plugin_runtime-5.4.8/insightconnect_plugin_runtime/clients/oauth.py` & `insightconnect_plugin_runtime-5.4.9/insightconnect_plugin_runtime/clients/oauth.py`

 * *Files identical despite different names*

### Comparing `insightconnect_plugin_runtime-5.4.8/insightconnect_plugin_runtime/connection.py` & `insightconnect_plugin_runtime-5.4.9/insightconnect_plugin_runtime/connection.py`

 * *Files identical despite different names*

### Comparing `insightconnect_plugin_runtime-5.4.8/insightconnect_plugin_runtime/data/input_message_schema.json` & `insightconnect_plugin_runtime-5.4.9/insightconnect_plugin_runtime/data/input_message_schema.json`

 * *Files identical despite different names*

### Comparing `insightconnect_plugin_runtime-5.4.8/insightconnect_plugin_runtime/data/output_message_schema.json` & `insightconnect_plugin_runtime-5.4.9/insightconnect_plugin_runtime/data/output_message_schema.json`

 * *Files identical despite different names*

### Comparing `insightconnect_plugin_runtime-5.4.8/insightconnect_plugin_runtime/dispatcher.py` & `insightconnect_plugin_runtime-5.4.9/insightconnect_plugin_runtime/dispatcher.py`

 * *Files identical despite different names*

### Comparing `insightconnect_plugin_runtime-5.4.8/insightconnect_plugin_runtime/exceptions.py` & `insightconnect_plugin_runtime-5.4.9/insightconnect_plugin_runtime/exceptions.py`

 * *Files identical despite different names*

### Comparing `insightconnect_plugin_runtime-5.4.8/insightconnect_plugin_runtime/helper.py` & `insightconnect_plugin_runtime-5.4.9/insightconnect_plugin_runtime/helper.py`

 * *Files identical despite different names*

### Comparing `insightconnect_plugin_runtime-5.4.8/insightconnect_plugin_runtime/metrics.py` & `insightconnect_plugin_runtime-5.4.9/insightconnect_plugin_runtime/metrics.py`

 * *Files identical despite different names*

### Comparing `insightconnect_plugin_runtime-5.4.8/insightconnect_plugin_runtime/plugin.py` & `insightconnect_plugin_runtime-5.4.9/insightconnect_plugin_runtime/plugin.py`

 * *Files identical despite different names*

### Comparing `insightconnect_plugin_runtime-5.4.8/insightconnect_plugin_runtime/schema.py` & `insightconnect_plugin_runtime-5.4.9/insightconnect_plugin_runtime/schema.py`

 * *Files identical despite different names*

### Comparing `insightconnect_plugin_runtime-5.4.8/insightconnect_plugin_runtime/server.py` & `insightconnect_plugin_runtime-5.4.9/insightconnect_plugin_runtime/server.py`

 * *Files identical despite different names*

### Comparing `insightconnect_plugin_runtime-5.4.8/insightconnect_plugin_runtime/step.py` & `insightconnect_plugin_runtime-5.4.9/insightconnect_plugin_runtime/step.py`

 * *Files identical despite different names*

### Comparing `insightconnect_plugin_runtime-5.4.8/insightconnect_plugin_runtime/trigger.py` & `insightconnect_plugin_runtime-5.4.9/insightconnect_plugin_runtime/trigger.py`

 * *Files identical despite different names*

### Comparing `insightconnect_plugin_runtime-5.4.8/insightconnect_plugin_runtime/util.py` & `insightconnect_plugin_runtime-5.4.9/insightconnect_plugin_runtime/util.py`

 * *Files identical despite different names*

### Comparing `insightconnect_plugin_runtime-5.4.8/insightconnect_plugin_runtime/variables.py` & `insightconnect_plugin_runtime-5.4.9/insightconnect_plugin_runtime/variables.py`

 * *Files identical despite different names*

### Comparing `insightconnect_plugin_runtime-5.4.8/insightconnect_plugin_runtime.egg-info/PKG-INFO` & `insightconnect_plugin_runtime-5.4.9/insightconnect_plugin_runtime.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: insightconnect-plugin-runtime
-Version: 5.4.8
+Version: 5.4.9
 Summary: InsightConnect Plugin Runtime
 Home-page: https://github.com/rapid7/komand-plugin-sdk-python
 Author: Rapid7 Integrations Alliance
 Author-email: integrationalliance@rapid7.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
@@ -207,14 +207,15 @@
 
 Contributions for maintaining and enhancing the InsightConnect Python Plugin Runtime are appreciated. This project uses
 [Black](https://github.com/psf/black) for code formatting and includes a pre-commit hook to auto format code as it is
 contributed. Black is installed as a test dependency and the hook can be initialized by running `pre-commit install` 
 after cloning this repository.
 
 ## Changelog
+* 5.4.9 - Updated aws_client to clean assume role json object to remove any none or empty string values.
 * 5.4.8 - Address vulnerabilities within `gunicorn` and `idna` python packages.
 * 5.4.7 - Address vulnerabilities within `insightconnect-python-3-plugin` image.
 * 5.4.6 - Updated our cloud loggers to include the request path | Updated slim image to remediate vulnerabilities.
 * 5.4.5 - Updated base images to pull Python 3.9.19 | Alpine image: Updated expat package
 * 5.4.4 - Handling the 'Connection Refused' to cps (during startup) as an info instead of error log as this is an expected error.
 * 5.4.3 - Updated dependencies to the latest versions | Fixed issue related to logger `StreamHandlers`
 * 5.4.2 - Remove background scheduler to simplify when the server gets custom_config values | Revert to use `bullseye` for slim image.
```

### Comparing `insightconnect_plugin_runtime-5.4.8/insightconnect_plugin_runtime.egg-info/SOURCES.txt` & `insightconnect_plugin_runtime-5.4.9/insightconnect_plugin_runtime.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `insightconnect_plugin_runtime-5.4.8/setup.py` & `insightconnect_plugin_runtime-5.4.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="insightconnect-plugin-runtime",
-    version="5.4.8",
+    version="5.4.9",
     description="InsightConnect Plugin Runtime",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Rapid7 Integrations Alliance",
     author_email="integrationalliance@rapid7.com",
     url="https://github.com/rapid7/komand-plugin-sdk-python",
     packages=find_packages(),
```

### Comparing `insightconnect_plugin_runtime-5.4.8/tests/plugin/__init__.py` & `insightconnect_plugin_runtime-5.4.9/tests/plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `insightconnect_plugin_runtime-5.4.8/tests/plugin/hello_world/hello_world/__init__.py` & `insightconnect_plugin_runtime-5.4.9/tests/plugin/hello_world/hello_world/__init__.py`

 * *Files identical despite different names*

### Comparing `insightconnect_plugin_runtime-5.4.8/tests/plugin/hello_world/hello_world/komand_hello_world/actions/hello/action.py` & `insightconnect_plugin_runtime-5.4.9/tests/plugin/hello_world/hello_world/komand_hello_world/actions/hello/action.py`

 * *Files identical despite different names*

### Comparing `insightconnect_plugin_runtime-5.4.8/tests/plugin/hello_world/hello_world/komand_hello_world/actions/hello/schema.py` & `insightconnect_plugin_runtime-5.4.9/tests/plugin/hello_world/hello_world/komand_hello_world/actions/hello/schema.py`

 * *Files identical despite different names*

### Comparing `insightconnect_plugin_runtime-5.4.8/tests/plugin/hello_world/hello_world/komand_hello_world/actions/return_bad_json/action.py` & `insightconnect_plugin_runtime-5.4.9/tests/plugin/hello_world/hello_world/komand_hello_world/actions/return_bad_json/action.py`

 * *Files identical despite different names*

### Comparing `insightconnect_plugin_runtime-5.4.8/tests/plugin/hello_world/hello_world/komand_hello_world/actions/return_bad_json/schema.py` & `insightconnect_plugin_runtime-5.4.9/tests/plugin/hello_world/hello_world/komand_hello_world/actions/return_bad_json/schema.py`

 * *Files identical despite different names*

### Comparing `insightconnect_plugin_runtime-5.4.8/tests/plugin/hello_world/hello_world/komand_hello_world/actions/throw_exception/action.py` & `insightconnect_plugin_runtime-5.4.9/tests/plugin/hello_world/hello_world/komand_hello_world/actions/throw_exception/action.py`

 * *Files identical despite different names*

### Comparing `insightconnect_plugin_runtime-5.4.8/tests/plugin/hello_world/hello_world/komand_hello_world/actions/throw_exception/schema.py` & `insightconnect_plugin_runtime-5.4.9/tests/plugin/hello_world/hello_world/komand_hello_world/actions/throw_exception/schema.py`

 * *Files identical despite different names*

### Comparing `insightconnect_plugin_runtime-5.4.8/tests/plugin/hello_world/hello_world/komand_hello_world/connection/schema.py` & `insightconnect_plugin_runtime-5.4.9/tests/plugin/hello_world/hello_world/komand_hello_world/connection/schema.py`

 * *Files identical despite different names*

### Comparing `insightconnect_plugin_runtime-5.4.8/tests/plugin/hello_world/hello_world/komand_hello_world/tasks/monitor_events/schema.py` & `insightconnect_plugin_runtime-5.4.9/tests/plugin/hello_world/hello_world/komand_hello_world/tasks/monitor_events/schema.py`

 * *Files identical despite different names*

### Comparing `insightconnect_plugin_runtime-5.4.8/tests/plugin/hello_world/hello_world/komand_hello_world/tasks/monitor_events/task.py` & `insightconnect_plugin_runtime-5.4.9/tests/plugin/hello_world/hello_world/komand_hello_world/tasks/monitor_events/task.py`

 * *Files identical despite different names*

### Comparing `insightconnect_plugin_runtime-5.4.8/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/hello_trigger/schema.py` & `insightconnect_plugin_runtime-5.4.9/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/hello_trigger/schema.py`

 * *Files identical despite different names*

### Comparing `insightconnect_plugin_runtime-5.4.8/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/hello_trigger/trigger.py` & `insightconnect_plugin_runtime-5.4.9/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/hello_trigger/trigger.py`

 * *Files identical despite different names*

### Comparing `insightconnect_plugin_runtime-5.4.8/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/return_bad_json_trigger/schema.py` & `insightconnect_plugin_runtime-5.4.9/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/return_bad_json_trigger/schema.py`

 * *Files identical despite different names*

### Comparing `insightconnect_plugin_runtime-5.4.8/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/return_bad_json_trigger/trigger.py` & `insightconnect_plugin_runtime-5.4.9/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/return_bad_json_trigger/trigger.py`

 * *Files identical despite different names*

### Comparing `insightconnect_plugin_runtime-5.4.8/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/throw_exception_trigger/schema.py` & `insightconnect_plugin_runtime-5.4.9/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/throw_exception_trigger/schema.py`

 * *Files identical despite different names*

### Comparing `insightconnect_plugin_runtime-5.4.8/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/throw_exception_trigger/trigger.py` & `insightconnect_plugin_runtime-5.4.9/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/throw_exception_trigger/trigger.py`

 * *Files identical despite different names*

### Comparing `insightconnect_plugin_runtime-5.4.8/tests/plugin/hello_world/tests/conftest.py` & `insightconnect_plugin_runtime-5.4.9/tests/plugin/hello_world/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `insightconnect_plugin_runtime-5.4.8/tests/plugin/hello_world/tests/test_cli.py` & `insightconnect_plugin_runtime-5.4.9/tests/plugin/hello_world/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `insightconnect_plugin_runtime-5.4.8/tests/plugin/hello_world/tests/test_hello_world.py` & `insightconnect_plugin_runtime-5.4.9/tests/plugin/hello_world/tests/test_hello_world.py`

 * *Files identical despite different names*

### Comparing `insightconnect_plugin_runtime-5.4.8/tests/plugin/hello_world/tests/test_server.py` & `insightconnect_plugin_runtime-5.4.9/tests/plugin/hello_world/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `insightconnect_plugin_runtime-5.4.8/tests/unit/test_action.py` & `insightconnect_plugin_runtime-5.4.9/tests/unit/test_action.py`

 * *Files identical despite different names*

### Comparing `insightconnect_plugin_runtime-5.4.8/tests/unit/test_api.py` & `insightconnect_plugin_runtime-5.4.9/tests/unit/test_api.py`

 * *Files identical despite different names*

### Comparing `insightconnect_plugin_runtime-5.4.8/tests/unit/test_aws_action.py` & `insightconnect_plugin_runtime-5.4.9/tests/unit/test_aws_action.py`

 * *Files identical despite different names*

### Comparing `insightconnect_plugin_runtime-5.4.8/tests/unit/test_custom_encoder.py` & `insightconnect_plugin_runtime-5.4.9/tests/unit/test_custom_encoder.py`

 * *Files identical despite different names*

### Comparing `insightconnect_plugin_runtime-5.4.8/tests/unit/test_endpoints.py` & `insightconnect_plugin_runtime-5.4.9/tests/unit/test_endpoints.py`

 * *Files identical despite different names*

### Comparing `insightconnect_plugin_runtime-5.4.8/tests/unit/test_exceptions.py` & `insightconnect_plugin_runtime-5.4.9/tests/unit/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `insightconnect_plugin_runtime-5.4.8/tests/unit/test_helpers.py` & `insightconnect_plugin_runtime-5.4.9/tests/unit/test_helpers.py`

 * *Files identical despite different names*

### Comparing `insightconnect_plugin_runtime-5.4.8/tests/unit/test_metrics.py` & `insightconnect_plugin_runtime-5.4.9/tests/unit/test_metrics.py`

 * *Files identical despite different names*

### Comparing `insightconnect_plugin_runtime-5.4.8/tests/unit/test_oauth.py` & `insightconnect_plugin_runtime-5.4.9/tests/unit/test_oauth.py`

 * *Files identical despite different names*

### Comparing `insightconnect_plugin_runtime-5.4.8/tests/unit/test_plugin.py` & `insightconnect_plugin_runtime-5.4.9/tests/unit/test_plugin.py`

 * *Files identical despite different names*

### Comparing `insightconnect_plugin_runtime-5.4.8/tests/unit/test_schema.py` & `insightconnect_plugin_runtime-5.4.9/tests/unit/test_schema.py`

 * *Files identical despite different names*

### Comparing `insightconnect_plugin_runtime-5.4.8/tests/unit/test_server_cloud_plugins.py` & `insightconnect_plugin_runtime-5.4.9/tests/unit/test_server_cloud_plugins.py`

 * *Files identical despite different names*

### Comparing `insightconnect_plugin_runtime-5.4.8/tests/unit/test_server_spec.py` & `insightconnect_plugin_runtime-5.4.9/tests/unit/test_server_spec.py`

 * *Files identical despite different names*

### Comparing `insightconnect_plugin_runtime-5.4.8/tests/unit/test_trigger.py` & `insightconnect_plugin_runtime-5.4.9/tests/unit/test_trigger.py`

 * *Files identical despite different names*

