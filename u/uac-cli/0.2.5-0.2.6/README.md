# Comparing `tmp/uac-cli-0.2.5.tar.gz` & `tmp/uac-cli-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uac-cli-0.2.5.tar", last modified: Wed May  8 05:35:43 2024, max compression
+gzip compressed data, was "uac-cli-0.2.6.tar", last modified: Fri May 10 17:14:44 2024, max compression
```

## Comparing `uac-cli-0.2.5.tar` & `uac-cli-0.2.6.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-05-08 05:35:43.253610 uac-cli-0.2.5/
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     9672 2024-05-08 05:35:43.253316 uac-cli-0.2.5/PKG-INFO
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     9041 2024-05-07 21:43:44.000000 uac-cli-0.2.5/README.md
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      405 2024-05-07 21:45:43.000000 uac-cli-0.2.5/pyproject.toml
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)       38 2024-05-08 05:35:43.253661 uac-cli-0.2.5/setup.cfg
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     1185 2024-05-08 02:51:37.000000 uac-cli-0.2.5/setup.py
-drwxr-xr-x   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-05-08 05:35:43.238652 uac-cli-0.2.5/uac_cli/
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      145 2024-05-08 05:35:39.000000 uac-cli-0.2.5/uac_cli/__init__.py
-drwxr-xr-x   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-05-08 05:35:43.251488 uac-cli-0.2.5/uac_cli/commands/
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-05-05 17:55:51.000000 uac-cli-0.2.5/uac_cli/commands/__init__.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     5545 2024-05-07 20:59:24.000000 uac-cli-0.2.5/uac_cli/commands/agent.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     6346 2024-05-07 21:00:04.000000 uac-cli-0.2.5/uac_cli/commands/agent_cluster.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      918 2024-05-07 15:20:53.000000 uac-cli-0.2.5/uac_cli/commands/audit.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     9331 2024-05-07 15:20:53.000000 uac-cli-0.2.5/uac_cli/commands/bundle.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2994 2024-05-07 15:20:53.000000 uac-cli-0.2.5/uac_cli/commands/business_service.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     5357 2024-05-07 15:20:53.000000 uac-cli-0.2.5/uac_cli/commands/calendar.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     1188 2024-05-07 15:20:53.000000 uac-cli-0.2.5/uac_cli/commands/cluster_node.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2183 2024-05-07 15:20:53.000000 uac-cli-0.2.5/uac_cli/commands/config.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)    11836 2024-05-07 15:20:53.000000 uac-cli-0.2.5/uac_cli/commands/connection.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     3875 2024-05-07 15:20:53.000000 uac-cli-0.2.5/uac_cli/commands/credential.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     3434 2024-05-07 15:20:53.000000 uac-cli-0.2.5/uac_cli/commands/custom_day.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2929 2024-05-07 15:20:53.000000 uac-cli-0.2.5/uac_cli/commands/email_template.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     1491 2024-05-07 15:20:53.000000 uac-cli-0.2.5/uac_cli/commands/ldap.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      756 2024-05-07 15:20:53.000000 uac-cli-0.2.5/uac_cli/commands/metric.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2954 2024-05-07 15:20:53.000000 uac-cli-0.2.5/uac_cli/commands/oauth_client.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     3023 2024-05-07 15:20:53.000000 uac-cli-0.2.5/uac_cli/commands/oms_server.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     1616 2024-05-08 03:23:56.000000 uac-cli-0.2.5/uac_cli/commands/property.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      958 2024-05-07 15:20:53.000000 uac-cli-0.2.5/uac_cli/commands/report.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2527 2024-05-07 15:20:53.000000 uac-cli-0.2.5/uac_cli/commands/script.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     3134 2024-05-08 03:49:16.000000 uac-cli-0.2.5/uac_cli/commands/server_operation.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2993 2024-05-07 15:20:53.000000 uac-cli-0.2.5/uac_cli/commands/simulation.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      726 2024-05-07 15:20:53.000000 uac-cli-0.2.5/uac_cli/commands/system.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     9664 2024-05-07 15:20:53.000000 uac-cli-0.2.5/uac_cli/commands/task.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)    19049 2024-05-08 04:47:43.000000 uac-cli-0.2.5/uac_cli/commands/task_instance.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     6392 2024-05-07 15:20:53.000000 uac-cli-0.2.5/uac_cli/commands/trigger.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     1499 2024-05-07 15:20:53.000000 uac-cli-0.2.5/uac_cli/commands/universal_event.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     3084 2024-05-07 15:20:53.000000 uac-cli-0.2.5/uac_cli/commands/universal_event_template.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     6950 2024-05-08 05:29:26.000000 uac-cli-0.2.5/uac_cli/commands/universal_template.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     4716 2024-05-07 15:20:53.000000 uac-cli-0.2.5/uac_cli/commands/user.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2678 2024-05-07 15:20:53.000000 uac-cli-0.2.5/uac_cli/commands/user_group.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     3495 2024-05-07 15:20:53.000000 uac-cli-0.2.5/uac_cli/commands/variable.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     3691 2024-05-07 15:20:53.000000 uac-cli-0.2.5/uac_cli/commands/virtual_resource.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     4208 2024-05-07 15:20:53.000000 uac-cli-0.2.5/uac_cli/commands/webhook.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     5716 2024-05-08 04:31:39.000000 uac-cli-0.2.5/uac_cli/commands/workflow.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     4504 2024-05-07 19:37:27.000000 uac-cli-0.2.5/uac_cli/main.py
-drwxr-xr-x   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-05-08 05:35:43.252905 uac-cli-0.2.5/uac_cli/utils/
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-05-05 17:56:14.000000 uac-cli-0.2.5/uac_cli/utils/__init__.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2922 2024-05-05 22:04:40.000000 uac-cli-0.2.5/uac_cli/utils/config.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      573 2024-05-08 05:25:10.000000 uac-cli-0.2.5/uac_cli/utils/options.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2223 2024-05-08 05:27:25.000000 uac-cli-0.2.5/uac_cli/utils/process.py
-drwxr-xr-x   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-05-08 05:35:43.240275 uac-cli-0.2.5/uac_cli.egg-info/
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     9672 2024-05-08 05:35:43.000000 uac-cli-0.2.5/uac_cli.egg-info/PKG-INFO
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     1433 2024-05-08 05:35:43.000000 uac-cli-0.2.5/uac_cli.egg-info/SOURCES.txt
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        1 2024-05-08 05:35:43.000000 uac-cli-0.2.5/uac_cli.egg-info/dependency_links.txt
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)       41 2024-05-08 05:35:43.000000 uac-cli-0.2.5/uac_cli.egg-info/entry_points.txt
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)       66 2024-05-08 05:35:43.000000 uac-cli-0.2.5/uac_cli.egg-info/requires.txt
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        8 2024-05-08 05:35:43.000000 uac-cli-0.2.5/uac_cli.egg-info/top_level.txt
+drwxr-xr-x   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-05-10 17:14:44.237628 uac-cli-0.2.6/
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     9672 2024-05-10 17:14:44.237279 uac-cli-0.2.6/PKG-INFO
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     9041 2024-05-07 21:43:44.000000 uac-cli-0.2.6/README.md
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      405 2024-05-07 21:45:43.000000 uac-cli-0.2.6/pyproject.toml
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)       38 2024-05-10 17:14:44.237684 uac-cli-0.2.6/setup.cfg
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     1185 2024-05-08 02:51:37.000000 uac-cli-0.2.6/setup.py
+drwxr-xr-x   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-05-10 17:14:44.213675 uac-cli-0.2.6/uac_cli/
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      145 2024-05-10 17:10:20.000000 uac-cli-0.2.6/uac_cli/__init__.py
+drwxr-xr-x   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-05-10 17:14:44.234890 uac-cli-0.2.6/uac_cli/commands/
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-05-05 17:55:51.000000 uac-cli-0.2.6/uac_cli/commands/__init__.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     5545 2024-05-07 20:59:24.000000 uac-cli-0.2.6/uac_cli/commands/agent.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     6346 2024-05-07 21:00:04.000000 uac-cli-0.2.6/uac_cli/commands/agent_cluster.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      918 2024-05-07 15:20:53.000000 uac-cli-0.2.6/uac_cli/commands/audit.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     9331 2024-05-07 15:20:53.000000 uac-cli-0.2.6/uac_cli/commands/bundle.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2994 2024-05-07 15:20:53.000000 uac-cli-0.2.6/uac_cli/commands/business_service.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     5357 2024-05-07 15:20:53.000000 uac-cli-0.2.6/uac_cli/commands/calendar.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     1188 2024-05-07 15:20:53.000000 uac-cli-0.2.6/uac_cli/commands/cluster_node.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2891 2024-05-10 16:40:07.000000 uac-cli-0.2.6/uac_cli/commands/config.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)    11836 2024-05-07 15:20:53.000000 uac-cli-0.2.6/uac_cli/commands/connection.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     3875 2024-05-07 15:20:53.000000 uac-cli-0.2.6/uac_cli/commands/credential.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     3434 2024-05-07 15:20:53.000000 uac-cli-0.2.6/uac_cli/commands/custom_day.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2929 2024-05-07 15:20:53.000000 uac-cli-0.2.6/uac_cli/commands/email_template.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     1491 2024-05-07 15:20:53.000000 uac-cli-0.2.6/uac_cli/commands/ldap.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      756 2024-05-07 15:20:53.000000 uac-cli-0.2.6/uac_cli/commands/metric.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2954 2024-05-07 15:20:53.000000 uac-cli-0.2.6/uac_cli/commands/oauth_client.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     3023 2024-05-07 15:20:53.000000 uac-cli-0.2.6/uac_cli/commands/oms_server.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     1616 2024-05-08 03:23:56.000000 uac-cli-0.2.6/uac_cli/commands/property.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      958 2024-05-07 15:20:53.000000 uac-cli-0.2.6/uac_cli/commands/report.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2527 2024-05-07 15:20:53.000000 uac-cli-0.2.6/uac_cli/commands/script.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     3134 2024-05-08 03:49:16.000000 uac-cli-0.2.6/uac_cli/commands/server_operation.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2993 2024-05-07 15:20:53.000000 uac-cli-0.2.6/uac_cli/commands/simulation.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      726 2024-05-07 15:20:53.000000 uac-cli-0.2.6/uac_cli/commands/system.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     9664 2024-05-07 15:20:53.000000 uac-cli-0.2.6/uac_cli/commands/task.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)    19049 2024-05-08 04:47:43.000000 uac-cli-0.2.6/uac_cli/commands/task_instance.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     6392 2024-05-07 15:20:53.000000 uac-cli-0.2.6/uac_cli/commands/trigger.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     1499 2024-05-07 15:20:53.000000 uac-cli-0.2.6/uac_cli/commands/universal_event.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     3084 2024-05-07 15:20:53.000000 uac-cli-0.2.6/uac_cli/commands/universal_event_template.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     6950 2024-05-08 05:29:26.000000 uac-cli-0.2.6/uac_cli/commands/universal_template.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     4716 2024-05-07 15:20:53.000000 uac-cli-0.2.6/uac_cli/commands/user.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2678 2024-05-07 15:20:53.000000 uac-cli-0.2.6/uac_cli/commands/user_group.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     3495 2024-05-07 15:20:53.000000 uac-cli-0.2.6/uac_cli/commands/variable.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     3691 2024-05-07 15:20:53.000000 uac-cli-0.2.6/uac_cli/commands/virtual_resource.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     4208 2024-05-07 15:20:53.000000 uac-cli-0.2.6/uac_cli/commands/webhook.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     5716 2024-05-08 04:31:39.000000 uac-cli-0.2.6/uac_cli/commands/workflow.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     6719 2024-05-10 17:08:47.000000 uac-cli-0.2.6/uac_cli/main.py
+drwxr-xr-x   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-05-10 17:14:44.236755 uac-cli-0.2.6/uac_cli/utils/
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-05-05 17:56:14.000000 uac-cli-0.2.6/uac_cli/utils/__init__.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2970 2024-05-10 16:44:39.000000 uac-cli-0.2.6/uac_cli/utils/config.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      573 2024-05-08 05:25:10.000000 uac-cli-0.2.6/uac_cli/utils/options.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2736 2024-05-10 16:09:14.000000 uac-cli-0.2.6/uac_cli/utils/process.py
+drwxr-xr-x   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-05-10 17:14:44.216435 uac-cli-0.2.6/uac_cli.egg-info/
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     9672 2024-05-10 17:14:44.000000 uac-cli-0.2.6/uac_cli.egg-info/PKG-INFO
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     1433 2024-05-10 17:14:44.000000 uac-cli-0.2.6/uac_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        1 2024-05-10 17:14:44.000000 uac-cli-0.2.6/uac_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)       41 2024-05-10 17:14:44.000000 uac-cli-0.2.6/uac_cli.egg-info/entry_points.txt
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)       66 2024-05-10 17:14:44.000000 uac-cli-0.2.6/uac_cli.egg-info/requires.txt
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        8 2024-05-10 17:14:44.000000 uac-cli-0.2.6/uac_cli.egg-info/top_level.txt
```

### Comparing `uac-cli-0.2.5/PKG-INFO` & `uac-cli-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uac-cli
-Version: 0.2.5
+Version: 0.2.6
 Summary: A CLI tool for executing commands against the Stonebranch UAC API
 Author: Stonebranch
 Author-email: "Huseyin G." <huseyim@gmail.com>
 License: CC BY-NC 4.0
 Project-URL: Homepage, https://github.com/gomleksiz/uac-cli
 Project-URL: Issues, https://github.com/gomleksiz/uac-cli/issues
 Project-URL: Documentation, https://uac-cli.readthedocs.io/en/latest/index.html
```

### Comparing `uac-cli-0.2.5/README.md` & `uac-cli-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.5/setup.py` & `uac-cli-0.2.6/setup.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.5/uac_cli/commands/agent.py` & `uac-cli-0.2.6/uac_cli/commands/agent.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.5/uac_cli/commands/agent_cluster.py` & `uac-cli-0.2.6/uac_cli/commands/agent_cluster.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.5/uac_cli/commands/audit.py` & `uac-cli-0.2.6/uac_cli/commands/audit.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.5/uac_cli/commands/bundle.py` & `uac-cli-0.2.6/uac_cli/commands/bundle.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.5/uac_cli/commands/business_service.py` & `uac-cli-0.2.6/uac_cli/commands/business_service.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.5/uac_cli/commands/calendar.py` & `uac-cli-0.2.6/uac_cli/commands/calendar.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.5/uac_cli/commands/cluster_node.py` & `uac-cli-0.2.6/uac_cli/commands/cluster_node.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.5/uac_cli/commands/connection.py` & `uac-cli-0.2.6/uac_cli/commands/connection.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.5/uac_cli/commands/credential.py` & `uac-cli-0.2.6/uac_cli/commands/credential.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.5/uac_cli/commands/custom_day.py` & `uac-cli-0.2.6/uac_cli/commands/custom_day.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.5/uac_cli/commands/email_template.py` & `uac-cli-0.2.6/uac_cli/commands/email_template.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.5/uac_cli/commands/ldap.py` & `uac-cli-0.2.6/uac_cli/commands/ldap.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.5/uac_cli/commands/metric.py` & `uac-cli-0.2.6/uac_cli/commands/metric.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.5/uac_cli/commands/oauth_client.py` & `uac-cli-0.2.6/uac_cli/commands/oauth_client.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.5/uac_cli/commands/oms_server.py` & `uac-cli-0.2.6/uac_cli/commands/oms_server.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.5/uac_cli/commands/property.py` & `uac-cli-0.2.6/uac_cli/commands/property.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.5/uac_cli/commands/report.py` & `uac-cli-0.2.6/uac_cli/commands/report.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.5/uac_cli/commands/script.py` & `uac-cli-0.2.6/uac_cli/commands/script.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.5/uac_cli/commands/server_operation.py` & `uac-cli-0.2.6/uac_cli/commands/server_operation.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.5/uac_cli/commands/simulation.py` & `uac-cli-0.2.6/uac_cli/commands/simulation.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.5/uac_cli/commands/system.py` & `uac-cli-0.2.6/uac_cli/commands/system.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.5/uac_cli/commands/task.py` & `uac-cli-0.2.6/uac_cli/commands/task.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.5/uac_cli/commands/task_instance.py` & `uac-cli-0.2.6/uac_cli/commands/task_instance.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.5/uac_cli/commands/trigger.py` & `uac-cli-0.2.6/uac_cli/commands/trigger.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.5/uac_cli/commands/universal_event.py` & `uac-cli-0.2.6/uac_cli/commands/universal_event.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.5/uac_cli/commands/universal_event_template.py` & `uac-cli-0.2.6/uac_cli/commands/universal_event_template.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.5/uac_cli/commands/universal_template.py` & `uac-cli-0.2.6/uac_cli/commands/universal_template.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.5/uac_cli/commands/user.py` & `uac-cli-0.2.6/uac_cli/commands/user.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.5/uac_cli/commands/user_group.py` & `uac-cli-0.2.6/uac_cli/commands/user_group.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.5/uac_cli/commands/variable.py` & `uac-cli-0.2.6/uac_cli/commands/variable.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.5/uac_cli/commands/virtual_resource.py` & `uac-cli-0.2.6/uac_cli/commands/virtual_resource.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.5/uac_cli/commands/webhook.py` & `uac-cli-0.2.6/uac_cli/commands/webhook.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.5/uac_cli/commands/workflow.py` & `uac-cli-0.2.6/uac_cli/commands/workflow.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.5/uac_cli/utils/config.py` & `uac-cli-0.2.6/uac_cli/utils/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,17 @@
     
     # Encode the modified password with Base64
     encoded_password = base64.b64encode(modified_password.encode()).decode()
     
     return encoded_password
 
 def simple_decrypt(encrypted_password, key):
+    if not key:
+        return None
+    
     # Convert the key (username) into a shift value
     shift = sum(ord(c) for c in key) % 256
     
     # Decode the password from Base64
     decoded_password = base64.b64decode(encrypted_password).decode()
     
     # Reverse the modification using the shift value
@@ -49,16 +52,16 @@
     if not os.path.exists(Path.home() / '.uac' / 'profiles.yml'):
         return None
 
     with open(Path.home() / '.uac' / 'profiles.yml', 'r') as file:
         config = yaml.load(file, Loader=yaml.FullLoader)
         if profile_name in config:
             profile = config[profile_name]
-            if "password" in profile and len(profile.get('password')) > 0:
-                profile['password'] = simple_decrypt(profile['password'], profile['username'])
+            if "password" in profile and profile.get('password', None):
+                profile['password'] = simple_decrypt(profile['password'], profile.get('username', None))
         else:
             profile = None
     return profile
 
 def write_profile(profile_name, profile):
     config = read_config()
     if config is None:
```

### Comparing `uac-cli-0.2.5/uac_cli/utils/options.py` & `uac-cli-0.2.6/uac_cli/utils/options.py`

 * *Files identical despite different names*

### Comparing `uac-cli-0.2.5/uac_cli/utils/process.py` & `uac-cli-0.2.6/uac_cli/utils/process.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import json
 import click
 from jsonpath_ng import jsonpath, parse
+import re
 
 def snake_to_camel(snake_case_str):
     """Converts a snake_case string to camelCase.
 
     Args:
         snake_case_str: The string in snake_case format.
 
@@ -47,23 +48,44 @@
     if input:
         payload = input.read()
         if not binary:    
             if not isinstance(payload, dict):
                 payload = json.loads(payload)
             for var in vars_dict:
                 _var = snake_to_camel(var)
+                value = input_value_parsing(vars_dict[var])
                 if var in payload:
-                    payload[var] = vars_dict[var]
+                    payload[var] = value
                 elif _var in payload:
-                    payload[_var] = vars_dict[var]
+                    payload[_var] = value
             vars_dict["payload"] = payload
         else:
             vars_dict["data"] = payload
     return vars_dict
 
+def input_value_parsing(value):
+    if not isinstance(value, str):
+        return value
+    
+    if value.lower() == ":none:":
+        return None
+    elif value.lower() == ":false:":
+        return False
+    elif value.lower() == ":true:":
+        return True
+    elif value == ":[]:":
+        return []
+    elif value == ":{}:":
+        return {}
+    elif re.match(r'^:\d+:$', value):
+        return int(value.strip(":"))
+    else:
+        return value
+    
+
 def create_payload(args):
     vars_dict = dict(var.split('=') for var in args)
     payload = {}
     for k, v in vars_dict.items():
         payload[k] = v
     return payload
```

### Comparing `uac-cli-0.2.5/uac_cli.egg-info/PKG-INFO` & `uac-cli-0.2.6/uac_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uac-cli
-Version: 0.2.5
+Version: 0.2.6
 Summary: A CLI tool for executing commands against the Stonebranch UAC API
 Author: Stonebranch
 Author-email: "Huseyin G." <huseyim@gmail.com>
 License: CC BY-NC 4.0
 Project-URL: Homepage, https://github.com/gomleksiz/uac-cli
 Project-URL: Issues, https://github.com/gomleksiz/uac-cli/issues
 Project-URL: Documentation, https://uac-cli.readthedocs.io/en/latest/index.html
```

### Comparing `uac-cli-0.2.5/uac_cli.egg-info/SOURCES.txt` & `uac-cli-0.2.6/uac_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

