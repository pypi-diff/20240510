# Comparing `tmp/pulumi_signalfx-7.2.0a1715236218.tar.gz` & `tmp/pulumi_signalfx-7.2.0a1715305180.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_signalfx-7.2.0a1715236218.tar", last modified: Thu May  9 06:38:50 2024, max compression
+gzip compressed data, was "pulumi_signalfx-7.2.0a1715305180.tar", last modified: Fri May 10 01:52:59 2024, max compression
```

## Comparing `pulumi_signalfx-7.2.0a1715236218.tar` & `pulumi_signalfx-7.2.0a1715305180.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:38:50.509876 pulumi_signalfx-7.2.0a1715236218/
--rw-r--r--   0 runner    (1001) docker     (127)     3024 2024-05-09 06:38:50.509876 pulumi_signalfx-7.2.0a1715236218/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2570 2024-05-09 06:38:44.000000 pulumi_signalfx-7.2.0a1715236218/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:38:50.501876 pulumi_signalfx-7.2.0a1715236218/pulumi_signalfx/
--rw-r--r--   0 runner    (1001) docker     (127)     7521 2024-05-09 06:38:44.000000 pulumi_signalfx-7.2.0a1715236218/pulumi_signalfx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   153334 2024-05-09 06:38:44.000000 pulumi_signalfx-7.2.0a1715236218/pulumi_signalfx/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-05-09 06:38:44.000000 pulumi_signalfx-7.2.0a1715236218/pulumi_signalfx/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    19007 2024-05-09 06:38:44.000000 pulumi_signalfx-7.2.0a1715236218/pulumi_signalfx/alert_muting_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:38:50.501876 pulumi_signalfx-7.2.0a1715236218/pulumi_signalfx/aws/
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-09 06:38:44.000000 pulumi_signalfx-7.2.0a1715236218/pulumi_signalfx/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10415 2024-05-09 06:38:44.000000 pulumi_signalfx-7.2.0a1715236218/pulumi_signalfx/aws/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    10582 2024-05-09 06:38:44.000000 pulumi_signalfx-7.2.0a1715236218/pulumi_signalfx/aws/external_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)    82908 2024-05-09 06:38:44.000000 pulumi_signalfx-7.2.0a1715236218/pulumi_signalfx/aws/integration.py
--rw-r--r--   0 runner    (1001) docker     (127)     9992 2024-05-09 06:38:44.000000 pulumi_signalfx-7.2.0a1715236218/pulumi_signalfx/aws/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    10114 2024-05-09 06:38:44.000000 pulumi_signalfx-7.2.0a1715236218/pulumi_signalfx/aws/token_integration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:38:50.505876 pulumi_signalfx-7.2.0a1715236218/pulumi_signalfx/azure/
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-09 06:38:44.000000 pulumi_signalfx-7.2.0a1715236218/pulumi_signalfx/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-05-09 06:38:44.000000 pulumi_signalfx-7.2.0a1715236218/pulumi_signalfx/azure/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    56590 2024-05-09 06:38:44.000000 pulumi_signalfx-7.2.0a1715236218/pulumi_signalfx/azure/integration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-05-09 06:38:44.000000 pulumi_signalfx-7.2.0a1715236218/pulumi_signalfx/azure/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:38:50.505876 pulumi_signalfx-7.2.0a1715236218/pulumi_signalfx/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-09 06:38:44.000000 pulumi_signalfx-7.2.0a1715236218/pulumi_signalfx/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-09 06:38:44.000000 pulumi_signalfx-7.2.0a1715236218/pulumi_signalfx/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-05-09 06:38:44.000000 pulumi_signalfx-7.2.0a1715236218/pulumi_signalfx/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    54932 2024-05-09 06:38:44.000000 pulumi_signalfx-7.2.0a1715236218/pulumi_signalfx/dashboard.py
--rw-r--r--   0 runner    (1001) docker     (127)    33368 2024-05-09 06:38:44.000000 pulumi_signalfx-7.2.0a1715236218/pulumi_signalfx/dashboard_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    26221 2024-05-09 06:38:44.000000 pulumi_signalfx-7.2.0a1715236218/pulumi_signalfx/data_link.py
--rw-r--r--   0 runner    (1001) docker     (127)    65421 2024-05-09 06:38:44.000000 pulumi_signalfx-7.2.0a1715236218/pulumi_signalfx/detector.py
--rw-r--r--   0 runner    (1001) docker     (127)    18692 2024-05-09 06:38:44.000000 pulumi_signalfx-7.2.0a1715236218/pulumi_signalfx/event_feed_chart.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:38:50.505876 pulumi_signalfx-7.2.0a1715236218/pulumi_signalfx/gcp/
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-09 06:38:44.000000 pulumi_signalfx-7.2.0a1715236218/pulumi_signalfx/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-05-09 06:38:44.000000 pulumi_signalfx-7.2.0a1715236218/pulumi_signalfx/gcp/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    34998 2024-05-09 06:38:44.000000 pulumi_signalfx-7.2.0a1715236218/pulumi_signalfx/gcp/integration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-05-09 06:38:44.000000 pulumi_signalfx-7.2.0a1715236218/pulumi_signalfx/gcp/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-05-09 06:38:44.000000 pulumi_signalfx-7.2.0a1715236218/pulumi_signalfx/get_dimension_values.py
--rw-r--r--   0 runner    (1001) docker     (127)    44252 2024-05-09 06:38:44.000000 pulumi_signalfx-7.2.0a1715236218/pulumi_signalfx/heatmap_chart.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:38:50.505876 pulumi_signalfx-7.2.0a1715236218/pulumi_signalfx/jira/
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-09 06:38:44.000000 pulumi_signalfx-7.2.0a1715236218/pulumi_signalfx/jira/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    34217 2024-05-09 06:38:44.000000 pulumi_signalfx-7.2.0a1715236218/pulumi_signalfx/jira/integration.py
--rw-r--r--   0 runner    (1001) docker     (127)    65676 2024-05-09 06:38:44.000000 pulumi_signalfx-7.2.0a1715236218/pulumi_signalfx/list_chart.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:38:50.505876 pulumi_signalfx-7.2.0a1715236218/pulumi_signalfx/log/
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-09 06:38:44.000000 pulumi_signalfx-7.2.0a1715236218/pulumi_signalfx/log/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-05-09 06:38:44.000000 pulumi_signalfx-7.2.0a1715236218/pulumi_signalfx/log/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-05-09 06:38:44.000000 pulumi_signalfx-7.2.0a1715236218/pulumi_signalfx/log/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    21446 2024-05-09 06:38:44.000000 pulumi_signalfx-7.2.0a1715236218/pulumi_signalfx/log/timeline.py
--rw-r--r--   0 runner    (1001) docker     (127)    26770 2024-05-09 06:38:44.000000 pulumi_signalfx-7.2.0a1715236218/pulumi_signalfx/log/view.py
--rw-r--r--   0 runner    (1001) docker     (127)    21744 2024-05-09 06:38:44.000000 pulumi_signalfx-7.2.0a1715236218/pulumi_signalfx/metric_ruleset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:38:50.505876 pulumi_signalfx-7.2.0a1715236218/pulumi_signalfx/opsgenie/
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-09 06:38:44.000000 pulumi_signalfx-7.2.0a1715236218/pulumi_signalfx/opsgenie/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12501 2024-05-09 06:38:44.000000 pulumi_signalfx-7.2.0a1715236218/pulumi_signalfx/opsgenie/integration.py
--rw-r--r--   0 runner    (1001) docker     (127)    24829 2024-05-09 06:38:44.000000 pulumi_signalfx-7.2.0a1715236218/pulumi_signalfx/org_token.py
--rw-r--r--   0 runner    (1001) docker     (127)   138325 2024-05-09 06:38:44.000000 pulumi_signalfx-7.2.0a1715236218/pulumi_signalfx/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:38:50.509876 pulumi_signalfx-7.2.0a1715236218/pulumi_signalfx/pagerduty/
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-09 06:38:44.000000 pulumi_signalfx-7.2.0a1715236218/pulumi_signalfx/pagerduty/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3712 2024-05-09 06:38:44.000000 pulumi_signalfx-7.2.0a1715236218/pulumi_signalfx/pagerduty/get_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)    10441 2024-05-09 06:38:44.000000 pulumi_signalfx-7.2.0a1715236218/pulumi_signalfx/pagerduty/integration.py
--rw-r--r--   0 runner    (1001) docker     (127)    11882 2024-05-09 06:38:44.000000 pulumi_signalfx-7.2.0a1715236218/pulumi_signalfx/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-09 06:38:44.000000 pulumi_signalfx-7.2.0a1715236218/pulumi_signalfx/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 06:38:44.000000 pulumi_signalfx-7.2.0a1715236218/pulumi_signalfx/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:38:50.509876 pulumi_signalfx-7.2.0a1715236218/pulumi_signalfx/servicenow/
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-09 06:38:44.000000 pulumi_signalfx-7.2.0a1715236218/pulumi_signalfx/servicenow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28846 2024-05-09 06:38:44.000000 pulumi_signalfx-7.2.0a1715236218/pulumi_signalfx/servicenow/integration.py
--rw-r--r--   0 runner    (1001) docker     (127)    44927 2024-05-09 06:38:44.000000 pulumi_signalfx-7.2.0a1715236218/pulumi_signalfx/single_value_chart.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:38:50.509876 pulumi_signalfx-7.2.0a1715236218/pulumi_signalfx/slack/
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-09 06:38:44.000000 pulumi_signalfx-7.2.0a1715236218/pulumi_signalfx/slack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10698 2024-05-09 06:38:44.000000 pulumi_signalfx-7.2.0a1715236218/pulumi_signalfx/slack/integration.py
--rw-r--r--   0 runner    (1001) docker     (127)    30506 2024-05-09 06:38:44.000000 pulumi_signalfx-7.2.0a1715236218/pulumi_signalfx/slo.py
--rw-r--r--   0 runner    (1001) docker     (127)    32559 2024-05-09 06:38:44.000000 pulumi_signalfx-7.2.0a1715236218/pulumi_signalfx/table_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)    29851 2024-05-09 06:38:44.000000 pulumi_signalfx-7.2.0a1715236218/pulumi_signalfx/team.py
--rw-r--r--   0 runner    (1001) docker     (127)    11236 2024-05-09 06:38:44.000000 pulumi_signalfx-7.2.0a1715236218/pulumi_signalfx/text_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)    85614 2024-05-09 06:38:44.000000 pulumi_signalfx-7.2.0a1715236218/pulumi_signalfx/time_chart.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:38:50.509876 pulumi_signalfx-7.2.0a1715236218/pulumi_signalfx/victorops/
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-09 06:38:44.000000 pulumi_signalfx-7.2.0a1715236218/pulumi_signalfx/victorops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10363 2024-05-09 06:38:44.000000 pulumi_signalfx-7.2.0a1715236218/pulumi_signalfx/victorops/integration.py
--rw-r--r--   0 runner    (1001) docker     (127)    14929 2024-05-09 06:38:44.000000 pulumi_signalfx-7.2.0a1715236218/pulumi_signalfx/webhook_integration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:38:50.509876 pulumi_signalfx-7.2.0a1715236218/pulumi_signalfx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3024 2024-05-09 06:38:50.000000 pulumi_signalfx-7.2.0a1715236218/pulumi_signalfx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-05-09 06:38:50.000000 pulumi_signalfx-7.2.0a1715236218/pulumi_signalfx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 06:38:50.000000 pulumi_signalfx-7.2.0a1715236218/pulumi_signalfx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-09 06:38:50.000000 pulumi_signalfx-7.2.0a1715236218/pulumi_signalfx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-09 06:38:50.000000 pulumi_signalfx-7.2.0a1715236218/pulumi_signalfx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-09 06:38:44.000000 pulumi_signalfx-7.2.0a1715236218/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 06:38:50.509876 pulumi_signalfx-7.2.0a1715236218/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 01:52:59.339127 pulumi_signalfx-7.2.0a1715305180/
+-rw-r--r--   0 runner    (1001) docker     (127)     3024 2024-05-10 01:52:59.339127 pulumi_signalfx-7.2.0a1715305180/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2570 2024-05-10 01:52:52.000000 pulumi_signalfx-7.2.0a1715305180/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 01:52:59.331127 pulumi_signalfx-7.2.0a1715305180/pulumi_signalfx/
+-rw-r--r--   0 runner    (1001) docker     (127)     7521 2024-05-10 01:52:52.000000 pulumi_signalfx-7.2.0a1715305180/pulumi_signalfx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   153334 2024-05-10 01:52:52.000000 pulumi_signalfx-7.2.0a1715305180/pulumi_signalfx/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-05-10 01:52:52.000000 pulumi_signalfx-7.2.0a1715305180/pulumi_signalfx/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19007 2024-05-10 01:52:52.000000 pulumi_signalfx-7.2.0a1715305180/pulumi_signalfx/alert_muting_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 01:52:59.335127 pulumi_signalfx-7.2.0a1715305180/pulumi_signalfx/aws/
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-10 01:52:52.000000 pulumi_signalfx-7.2.0a1715305180/pulumi_signalfx/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10415 2024-05-10 01:52:52.000000 pulumi_signalfx-7.2.0a1715305180/pulumi_signalfx/aws/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10582 2024-05-10 01:52:52.000000 pulumi_signalfx-7.2.0a1715305180/pulumi_signalfx/aws/external_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    82462 2024-05-10 01:52:52.000000 pulumi_signalfx-7.2.0a1715305180/pulumi_signalfx/aws/integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9992 2024-05-10 01:52:52.000000 pulumi_signalfx-7.2.0a1715305180/pulumi_signalfx/aws/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10114 2024-05-10 01:52:52.000000 pulumi_signalfx-7.2.0a1715305180/pulumi_signalfx/aws/token_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 01:52:59.335127 pulumi_signalfx-7.2.0a1715305180/pulumi_signalfx/azure/
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-10 01:52:52.000000 pulumi_signalfx-7.2.0a1715305180/pulumi_signalfx/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-05-10 01:52:52.000000 pulumi_signalfx-7.2.0a1715305180/pulumi_signalfx/azure/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56590 2024-05-10 01:52:52.000000 pulumi_signalfx-7.2.0a1715305180/pulumi_signalfx/azure/integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-05-10 01:52:52.000000 pulumi_signalfx-7.2.0a1715305180/pulumi_signalfx/azure/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 01:52:59.335127 pulumi_signalfx-7.2.0a1715305180/pulumi_signalfx/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-10 01:52:52.000000 pulumi_signalfx-7.2.0a1715305180/pulumi_signalfx/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-10 01:52:52.000000 pulumi_signalfx-7.2.0a1715305180/pulumi_signalfx/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-05-10 01:52:52.000000 pulumi_signalfx-7.2.0a1715305180/pulumi_signalfx/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54932 2024-05-10 01:52:52.000000 pulumi_signalfx-7.2.0a1715305180/pulumi_signalfx/dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33368 2024-05-10 01:52:52.000000 pulumi_signalfx-7.2.0a1715305180/pulumi_signalfx/dashboard_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26221 2024-05-10 01:52:52.000000 pulumi_signalfx-7.2.0a1715305180/pulumi_signalfx/data_link.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65421 2024-05-10 01:52:52.000000 pulumi_signalfx-7.2.0a1715305180/pulumi_signalfx/detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18692 2024-05-10 01:52:52.000000 pulumi_signalfx-7.2.0a1715305180/pulumi_signalfx/event_feed_chart.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 01:52:59.335127 pulumi_signalfx-7.2.0a1715305180/pulumi_signalfx/gcp/
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-10 01:52:52.000000 pulumi_signalfx-7.2.0a1715305180/pulumi_signalfx/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-05-10 01:52:52.000000 pulumi_signalfx-7.2.0a1715305180/pulumi_signalfx/gcp/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34998 2024-05-10 01:52:52.000000 pulumi_signalfx-7.2.0a1715305180/pulumi_signalfx/gcp/integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-05-10 01:52:52.000000 pulumi_signalfx-7.2.0a1715305180/pulumi_signalfx/gcp/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-05-10 01:52:52.000000 pulumi_signalfx-7.2.0a1715305180/pulumi_signalfx/get_dimension_values.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44252 2024-05-10 01:52:52.000000 pulumi_signalfx-7.2.0a1715305180/pulumi_signalfx/heatmap_chart.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 01:52:59.339127 pulumi_signalfx-7.2.0a1715305180/pulumi_signalfx/jira/
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-10 01:52:52.000000 pulumi_signalfx-7.2.0a1715305180/pulumi_signalfx/jira/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34217 2024-05-10 01:52:52.000000 pulumi_signalfx-7.2.0a1715305180/pulumi_signalfx/jira/integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65676 2024-05-10 01:52:52.000000 pulumi_signalfx-7.2.0a1715305180/pulumi_signalfx/list_chart.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 01:52:59.339127 pulumi_signalfx-7.2.0a1715305180/pulumi_signalfx/log/
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-10 01:52:52.000000 pulumi_signalfx-7.2.0a1715305180/pulumi_signalfx/log/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-05-10 01:52:52.000000 pulumi_signalfx-7.2.0a1715305180/pulumi_signalfx/log/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-05-10 01:52:52.000000 pulumi_signalfx-7.2.0a1715305180/pulumi_signalfx/log/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21446 2024-05-10 01:52:52.000000 pulumi_signalfx-7.2.0a1715305180/pulumi_signalfx/log/timeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26770 2024-05-10 01:52:52.000000 pulumi_signalfx-7.2.0a1715305180/pulumi_signalfx/log/view.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21744 2024-05-10 01:52:52.000000 pulumi_signalfx-7.2.0a1715305180/pulumi_signalfx/metric_ruleset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 01:52:59.339127 pulumi_signalfx-7.2.0a1715305180/pulumi_signalfx/opsgenie/
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-10 01:52:52.000000 pulumi_signalfx-7.2.0a1715305180/pulumi_signalfx/opsgenie/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12501 2024-05-10 01:52:52.000000 pulumi_signalfx-7.2.0a1715305180/pulumi_signalfx/opsgenie/integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24829 2024-05-10 01:52:52.000000 pulumi_signalfx-7.2.0a1715305180/pulumi_signalfx/org_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)   138325 2024-05-10 01:52:52.000000 pulumi_signalfx-7.2.0a1715305180/pulumi_signalfx/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 01:52:59.339127 pulumi_signalfx-7.2.0a1715305180/pulumi_signalfx/pagerduty/
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-10 01:52:52.000000 pulumi_signalfx-7.2.0a1715305180/pulumi_signalfx/pagerduty/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3712 2024-05-10 01:52:52.000000 pulumi_signalfx-7.2.0a1715305180/pulumi_signalfx/pagerduty/get_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10441 2024-05-10 01:52:52.000000 pulumi_signalfx-7.2.0a1715305180/pulumi_signalfx/pagerduty/integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11882 2024-05-10 01:52:52.000000 pulumi_signalfx-7.2.0a1715305180/pulumi_signalfx/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-10 01:52:52.000000 pulumi_signalfx-7.2.0a1715305180/pulumi_signalfx/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 01:52:52.000000 pulumi_signalfx-7.2.0a1715305180/pulumi_signalfx/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 01:52:59.339127 pulumi_signalfx-7.2.0a1715305180/pulumi_signalfx/servicenow/
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-10 01:52:52.000000 pulumi_signalfx-7.2.0a1715305180/pulumi_signalfx/servicenow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28846 2024-05-10 01:52:52.000000 pulumi_signalfx-7.2.0a1715305180/pulumi_signalfx/servicenow/integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44927 2024-05-10 01:52:52.000000 pulumi_signalfx-7.2.0a1715305180/pulumi_signalfx/single_value_chart.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 01:52:59.339127 pulumi_signalfx-7.2.0a1715305180/pulumi_signalfx/slack/
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-10 01:52:52.000000 pulumi_signalfx-7.2.0a1715305180/pulumi_signalfx/slack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10698 2024-05-10 01:52:52.000000 pulumi_signalfx-7.2.0a1715305180/pulumi_signalfx/slack/integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30506 2024-05-10 01:52:52.000000 pulumi_signalfx-7.2.0a1715305180/pulumi_signalfx/slo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32559 2024-05-10 01:52:52.000000 pulumi_signalfx-7.2.0a1715305180/pulumi_signalfx/table_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29851 2024-05-10 01:52:52.000000 pulumi_signalfx-7.2.0a1715305180/pulumi_signalfx/team.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11236 2024-05-10 01:52:52.000000 pulumi_signalfx-7.2.0a1715305180/pulumi_signalfx/text_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)    85614 2024-05-10 01:52:52.000000 pulumi_signalfx-7.2.0a1715305180/pulumi_signalfx/time_chart.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 01:52:59.339127 pulumi_signalfx-7.2.0a1715305180/pulumi_signalfx/victorops/
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-10 01:52:52.000000 pulumi_signalfx-7.2.0a1715305180/pulumi_signalfx/victorops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10363 2024-05-10 01:52:52.000000 pulumi_signalfx-7.2.0a1715305180/pulumi_signalfx/victorops/integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14929 2024-05-10 01:52:52.000000 pulumi_signalfx-7.2.0a1715305180/pulumi_signalfx/webhook_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 01:52:59.339127 pulumi_signalfx-7.2.0a1715305180/pulumi_signalfx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3024 2024-05-10 01:52:59.000000 pulumi_signalfx-7.2.0a1715305180/pulumi_signalfx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-05-10 01:52:59.000000 pulumi_signalfx-7.2.0a1715305180/pulumi_signalfx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 01:52:59.000000 pulumi_signalfx-7.2.0a1715305180/pulumi_signalfx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-10 01:52:59.000000 pulumi_signalfx-7.2.0a1715305180/pulumi_signalfx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-10 01:52:59.000000 pulumi_signalfx-7.2.0a1715305180/pulumi_signalfx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-10 01:52:52.000000 pulumi_signalfx-7.2.0a1715305180/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 01:52:59.339127 pulumi_signalfx-7.2.0a1715305180/setup.cfg
```

### Comparing `pulumi_signalfx-7.2.0a1715236218/PKG-INFO` & `pulumi_signalfx-7.2.0a1715305180/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_signalfx
-Version: 7.2.0a1715236218
+Version: 7.2.0a1715305180
 Summary: A Pulumi package for creating and managing SignalFx resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-signalfx
 Keywords: pulumi,signalfx
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_signalfx-7.2.0a1715236218/README.md` & `pulumi_signalfx-7.2.0a1715305180/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1715236218/pulumi_signalfx/__init__.py` & `pulumi_signalfx-7.2.0a1715305180/pulumi_signalfx/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1715236218/pulumi_signalfx/_inputs.py` & `pulumi_signalfx-7.2.0a1715305180/pulumi_signalfx/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1715236218/pulumi_signalfx/_utilities.py` & `pulumi_signalfx-7.2.0a1715305180/pulumi_signalfx/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1715236218/pulumi_signalfx/alert_muting_rule.py` & `pulumi_signalfx-7.2.0a1715305180/pulumi_signalfx/alert_muting_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1715236218/pulumi_signalfx/aws/_inputs.py` & `pulumi_signalfx-7.2.0a1715305180/pulumi_signalfx/aws/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1715236218/pulumi_signalfx/aws/external_integration.py` & `pulumi_signalfx-7.2.0a1715305180/pulumi_signalfx/aws/external_integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1715236218/pulumi_signalfx/aws/integration.py` & `pulumi_signalfx-7.2.0a1715305180/pulumi_signalfx/aws/integration.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,33 +46,33 @@
         :param pulumi.Input[Sequence[pulumi.Input['IntegrationCustomNamespaceSyncRuleArgs']]] custom_namespace_sync_rules: Each element controls the data collected by Splunk Observability for the specified namespace. If you specify this
                property, Splunk Observability ignores values in the "custom_cloudwatch_namespaces" property.
         :param pulumi.Input[bool] enable_aws_usage: Flag that controls how Splunk Observability imports usage metrics from AWS to use with AWS Cost Optimizer. If `true`,
                Splunk Observability imports the metrics.
         :param pulumi.Input[bool] enable_check_large_volume: Controls how Splunk Observability checks for large amounts of data for this AWS integration. If true, Splunk
                Observability monitors the amount of data coming in from the integration.
         :param pulumi.Input[bool] enable_logs_sync: Enables AWS logs synchronization.
-        :param pulumi.Input[str] external_id: Used with `signalfx_aws_external_integration`. Use this property to specify the external id.
+        :param pulumi.Input[str] external_id: Used with `aws.ExternalIntegration`. Use this property to specify the external id.
         :param pulumi.Input[bool] import_cloud_watch: Flag that controls how Splunk Observability imports Cloud Watch metrics. If true, Splunk Observability imports Cloud
                Watch metrics from AWS.
-        :param pulumi.Input[str] key: Used with `signalfx_aws_token_integration`. Use this property to specify the token.
+        :param pulumi.Input[str] key: Used with `aws.TokenIntegration`. Use this property to specify the token.
         :param pulumi.Input[Sequence[pulumi.Input['IntegrationMetricStatsToSyncArgs']]] metric_stats_to_syncs: Each element in the array is an object that contains an AWS namespace name, AWS metric name and a list of statistics
                that Splunk Observability collects for this metric. If you specify this property, Splunk Observability retrieves only
                specified AWS statistics. If you don't specify this property, Splunk Observability retrieves the AWS standard set of
                statistics.
         :param pulumi.Input[str] named_token: A named token to use for ingest
         :param pulumi.Input[Sequence[pulumi.Input['IntegrationNamespaceSyncRuleArgs']]] namespace_sync_rules: Each element in the array is an object that contains an AWS namespace name and a filter that controls the data that
                Splunk Observability collects for the namespace. If you specify this property, Splunk Observability ignores the values
                in the AWS CloudWatch Integration Model "services" property. If you don't specify either property, Splunk Observability
                syncs all data in all AWS namespaces.
         :param pulumi.Input[int] poll_rate: AWS poll rate (in seconds). Between `60` and `600`.
-        :param pulumi.Input[str] role_arn: Used with `signalfx_aws_external_integration`. Use this property to specify the AIM role ARN.
+        :param pulumi.Input[str] role_arn: Used with `aws.ExternalIntegration`. Use this property to specify the AIM role ARN.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] services: List of AWS services that you want Splunk Observability to monitor. Each element is a string designating an AWS service.
         :param pulumi.Input[bool] sync_custom_namespaces_only: Indicates that Splunk Observability should sync metrics and metadata from custom AWS namespaces only (see the
                `custom_namespace_sync_rule` field for details). Defaults to `false`.
-        :param pulumi.Input[str] token: Used with `signalfx_aws_token_integration`. Use this property to specify the token.
+        :param pulumi.Input[str] token: Used with `aws.TokenIntegration`. Use this property to specify the token.
         :param pulumi.Input[bool] use_metric_streams_sync: Enables the use of Cloudwatch Metric Streams for metrics synchronization.
         """
         pulumi.set(__self__, "enabled", enabled)
         pulumi.set(__self__, "integration_id", integration_id)
         pulumi.set(__self__, "regions", regions)
         if custom_cloudwatch_namespaces is not None:
             pulumi.set(__self__, "custom_cloudwatch_namespaces", custom_cloudwatch_namespaces)
@@ -209,15 +209,15 @@
     def enable_logs_sync(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "enable_logs_sync", value)
 
     @property
     @pulumi.getter(name="externalId")
     def external_id(self) -> Optional[pulumi.Input[str]]:
         """
-        Used with `signalfx_aws_external_integration`. Use this property to specify the external id.
+        Used with `aws.ExternalIntegration`. Use this property to specify the external id.
         """
         return pulumi.get(self, "external_id")
 
     @external_id.setter
     def external_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "external_id", value)
 
@@ -234,15 +234,15 @@
     def import_cloud_watch(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "import_cloud_watch", value)
 
     @property
     @pulumi.getter
     def key(self) -> Optional[pulumi.Input[str]]:
         """
-        Used with `signalfx_aws_token_integration`. Use this property to specify the token.
+        Used with `aws.TokenIntegration`. Use this property to specify the token.
         """
         return pulumi.get(self, "key")
 
     @key.setter
     def key(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "key", value)
 
@@ -300,15 +300,15 @@
     def poll_rate(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "poll_rate", value)
 
     @property
     @pulumi.getter(name="roleArn")
     def role_arn(self) -> Optional[pulumi.Input[str]]:
         """
-        Used with `signalfx_aws_external_integration`. Use this property to specify the AIM role ARN.
+        Used with `aws.ExternalIntegration`. Use this property to specify the AIM role ARN.
         """
         return pulumi.get(self, "role_arn")
 
     @role_arn.setter
     def role_arn(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "role_arn", value)
 
@@ -337,15 +337,15 @@
     def sync_custom_namespaces_only(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "sync_custom_namespaces_only", value)
 
     @property
     @pulumi.getter
     def token(self) -> Optional[pulumi.Input[str]]:
         """
-        Used with `signalfx_aws_token_integration`. Use this property to specify the token.
+        Used with `aws.TokenIntegration`. Use this property to specify the token.
         """
         return pulumi.get(self, "token")
 
     @token.setter
     def token(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "token", value)
 
@@ -385,49 +385,48 @@
                  role_arn: Optional[pulumi.Input[str]] = None,
                  services: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  sync_custom_namespaces_only: Optional[pulumi.Input[bool]] = None,
                  token: Optional[pulumi.Input[str]] = None,
                  use_metric_streams_sync: Optional[pulumi.Input[bool]] = None):
         """
         Input properties used for looking up and filtering Integration resources.
-        :param pulumi.Input[str] auth_method: The mechanism used to authenticate with AWS. Use one of `signalfx_aws_external_integration` or
-               `signalfx_aws_token_integration` to define this
+        :param pulumi.Input[str] auth_method: The mechanism used to authenticate with AWS. Use one of `aws.ExternalIntegration` or `aws.TokenIntegration` to define
+               this
         :param pulumi.Input[Sequence[pulumi.Input[str]]] custom_cloudwatch_namespaces: List of custom AWS CloudWatch namespaces to monitor. Custom namespaces contain custom metrics that you define in AWS;
                Splunk Observability imports the metrics so you can monitor them.
         :param pulumi.Input[Sequence[pulumi.Input['IntegrationCustomNamespaceSyncRuleArgs']]] custom_namespace_sync_rules: Each element controls the data collected by Splunk Observability for the specified namespace. If you specify this
                property, Splunk Observability ignores values in the "custom_cloudwatch_namespaces" property.
         :param pulumi.Input[bool] enable_aws_usage: Flag that controls how Splunk Observability imports usage metrics from AWS to use with AWS Cost Optimizer. If `true`,
                Splunk Observability imports the metrics.
         :param pulumi.Input[bool] enable_check_large_volume: Controls how Splunk Observability checks for large amounts of data for this AWS integration. If true, Splunk
                Observability monitors the amount of data coming in from the integration.
         :param pulumi.Input[bool] enable_logs_sync: Enables AWS logs synchronization.
         :param pulumi.Input[bool] enabled: Whether the integration is enabled or not
-        :param pulumi.Input[str] external_id: Used with `signalfx_aws_external_integration`. Use this property to specify the external id.
+        :param pulumi.Input[str] external_id: Used with `aws.ExternalIntegration`. Use this property to specify the external id.
         :param pulumi.Input[bool] import_cloud_watch: Flag that controls how Splunk Observability imports Cloud Watch metrics. If true, Splunk Observability imports Cloud
                Watch metrics from AWS.
         :param pulumi.Input[str] integration_id: The ID of this integration
-        :param pulumi.Input[str] key: Used with `signalfx_aws_token_integration`. Use this property to specify the token.
+        :param pulumi.Input[str] key: Used with `aws.TokenIntegration`. Use this property to specify the token.
         :param pulumi.Input[Sequence[pulumi.Input['IntegrationMetricStatsToSyncArgs']]] metric_stats_to_syncs: Each element in the array is an object that contains an AWS namespace name, AWS metric name and a list of statistics
                that Splunk Observability collects for this metric. If you specify this property, Splunk Observability retrieves only
                specified AWS statistics. If you don't specify this property, Splunk Observability retrieves the AWS standard set of
                statistics.
-        :param pulumi.Input[str] name: Name of the integration. Please specify the name in `signalfx_aws_external_integration` or
-               `signalfx_aws_integration_token`
+        :param pulumi.Input[str] name: Name of the integration. Please specify the name in `aws.ExternalIntegration` or `signalfx_aws_integration_token`
         :param pulumi.Input[str] named_token: A named token to use for ingest
         :param pulumi.Input[Sequence[pulumi.Input['IntegrationNamespaceSyncRuleArgs']]] namespace_sync_rules: Each element in the array is an object that contains an AWS namespace name and a filter that controls the data that
                Splunk Observability collects for the namespace. If you specify this property, Splunk Observability ignores the values
                in the AWS CloudWatch Integration Model "services" property. If you don't specify either property, Splunk Observability
                syncs all data in all AWS namespaces.
         :param pulumi.Input[int] poll_rate: AWS poll rate (in seconds). Between `60` and `600`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] regions: List of AWS regions that Splunk Observability should monitor.
-        :param pulumi.Input[str] role_arn: Used with `signalfx_aws_external_integration`. Use this property to specify the AIM role ARN.
+        :param pulumi.Input[str] role_arn: Used with `aws.ExternalIntegration`. Use this property to specify the AIM role ARN.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] services: List of AWS services that you want Splunk Observability to monitor. Each element is a string designating an AWS service.
         :param pulumi.Input[bool] sync_custom_namespaces_only: Indicates that Splunk Observability should sync metrics and metadata from custom AWS namespaces only (see the
                `custom_namespace_sync_rule` field for details). Defaults to `false`.
-        :param pulumi.Input[str] token: Used with `signalfx_aws_token_integration`. Use this property to specify the token.
+        :param pulumi.Input[str] token: Used with `aws.TokenIntegration`. Use this property to specify the token.
         :param pulumi.Input[bool] use_metric_streams_sync: Enables the use of Cloudwatch Metric Streams for metrics synchronization.
         """
         if auth_method is not None:
             pulumi.set(__self__, "auth_method", auth_method)
         if custom_cloudwatch_namespaces is not None:
             pulumi.set(__self__, "custom_cloudwatch_namespaces", custom_cloudwatch_namespaces)
         if custom_namespace_sync_rules is not None:
@@ -471,16 +470,16 @@
         if use_metric_streams_sync is not None:
             pulumi.set(__self__, "use_metric_streams_sync", use_metric_streams_sync)
 
     @property
     @pulumi.getter(name="authMethod")
     def auth_method(self) -> Optional[pulumi.Input[str]]:
         """
-        The mechanism used to authenticate with AWS. Use one of `signalfx_aws_external_integration` or
-        `signalfx_aws_token_integration` to define this
+        The mechanism used to authenticate with AWS. Use one of `aws.ExternalIntegration` or `aws.TokenIntegration` to define
+        this
         """
         return pulumi.get(self, "auth_method")
 
     @auth_method.setter
     def auth_method(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "auth_method", value)
 
@@ -560,15 +559,15 @@
     def enabled(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "enabled", value)
 
     @property
     @pulumi.getter(name="externalId")
     def external_id(self) -> Optional[pulumi.Input[str]]:
         """
-        Used with `signalfx_aws_external_integration`. Use this property to specify the external id.
+        Used with `aws.ExternalIntegration`. Use this property to specify the external id.
         """
         return pulumi.get(self, "external_id")
 
     @external_id.setter
     def external_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "external_id", value)
 
@@ -597,15 +596,15 @@
     def integration_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "integration_id", value)
 
     @property
     @pulumi.getter
     def key(self) -> Optional[pulumi.Input[str]]:
         """
-        Used with `signalfx_aws_token_integration`. Use this property to specify the token.
+        Used with `aws.TokenIntegration`. Use this property to specify the token.
         """
         return pulumi.get(self, "key")
 
     @key.setter
     def key(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "key", value)
 
@@ -624,16 +623,15 @@
     def metric_stats_to_syncs(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['IntegrationMetricStatsToSyncArgs']]]]):
         pulumi.set(self, "metric_stats_to_syncs", value)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
-        Name of the integration. Please specify the name in `signalfx_aws_external_integration` or
-        `signalfx_aws_integration_token`
+        Name of the integration. Please specify the name in `aws.ExternalIntegration` or `signalfx_aws_integration_token`
         """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
@@ -688,15 +686,15 @@
     def regions(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "regions", value)
 
     @property
     @pulumi.getter(name="roleArn")
     def role_arn(self) -> Optional[pulumi.Input[str]]:
         """
-        Used with `signalfx_aws_external_integration`. Use this property to specify the AIM role ARN.
+        Used with `aws.ExternalIntegration`. Use this property to specify the AIM role ARN.
         """
         return pulumi.get(self, "role_arn")
 
     @role_arn.setter
     def role_arn(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "role_arn", value)
 
@@ -725,15 +723,15 @@
     def sync_custom_namespaces_only(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "sync_custom_namespaces_only", value)
 
     @property
     @pulumi.getter
     def token(self) -> Optional[pulumi.Input[str]]:
         """
-        Used with `signalfx_aws_token_integration`. Use this property to specify the token.
+        Used with `aws.TokenIntegration`. Use this property to specify the token.
         """
         return pulumi.get(self, "token")
 
     @token.setter
     def token(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "token", value)
 
@@ -830,35 +828,35 @@
                property, Splunk Observability ignores values in the "custom_cloudwatch_namespaces" property.
         :param pulumi.Input[bool] enable_aws_usage: Flag that controls how Splunk Observability imports usage metrics from AWS to use with AWS Cost Optimizer. If `true`,
                Splunk Observability imports the metrics.
         :param pulumi.Input[bool] enable_check_large_volume: Controls how Splunk Observability checks for large amounts of data for this AWS integration. If true, Splunk
                Observability monitors the amount of data coming in from the integration.
         :param pulumi.Input[bool] enable_logs_sync: Enables AWS logs synchronization.
         :param pulumi.Input[bool] enabled: Whether the integration is enabled or not
-        :param pulumi.Input[str] external_id: Used with `signalfx_aws_external_integration`. Use this property to specify the external id.
+        :param pulumi.Input[str] external_id: Used with `aws.ExternalIntegration`. Use this property to specify the external id.
         :param pulumi.Input[bool] import_cloud_watch: Flag that controls how Splunk Observability imports Cloud Watch metrics. If true, Splunk Observability imports Cloud
                Watch metrics from AWS.
         :param pulumi.Input[str] integration_id: The ID of this integration
-        :param pulumi.Input[str] key: Used with `signalfx_aws_token_integration`. Use this property to specify the token.
+        :param pulumi.Input[str] key: Used with `aws.TokenIntegration`. Use this property to specify the token.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['IntegrationMetricStatsToSyncArgs']]]] metric_stats_to_syncs: Each element in the array is an object that contains an AWS namespace name, AWS metric name and a list of statistics
                that Splunk Observability collects for this metric. If you specify this property, Splunk Observability retrieves only
                specified AWS statistics. If you don't specify this property, Splunk Observability retrieves the AWS standard set of
                statistics.
         :param pulumi.Input[str] named_token: A named token to use for ingest
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['IntegrationNamespaceSyncRuleArgs']]]] namespace_sync_rules: Each element in the array is an object that contains an AWS namespace name and a filter that controls the data that
                Splunk Observability collects for the namespace. If you specify this property, Splunk Observability ignores the values
                in the AWS CloudWatch Integration Model "services" property. If you don't specify either property, Splunk Observability
                syncs all data in all AWS namespaces.
         :param pulumi.Input[int] poll_rate: AWS poll rate (in seconds). Between `60` and `600`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] regions: List of AWS regions that Splunk Observability should monitor.
-        :param pulumi.Input[str] role_arn: Used with `signalfx_aws_external_integration`. Use this property to specify the AIM role ARN.
+        :param pulumi.Input[str] role_arn: Used with `aws.ExternalIntegration`. Use this property to specify the AIM role ARN.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] services: List of AWS services that you want Splunk Observability to monitor. Each element is a string designating an AWS service.
         :param pulumi.Input[bool] sync_custom_namespaces_only: Indicates that Splunk Observability should sync metrics and metadata from custom AWS namespaces only (see the
                `custom_namespace_sync_rule` field for details). Defaults to `false`.
-        :param pulumi.Input[str] token: Used with `signalfx_aws_token_integration`. Use this property to specify the token.
+        :param pulumi.Input[str] token: Used with `aws.TokenIntegration`. Use this property to specify the token.
         :param pulumi.Input[bool] use_metric_streams_sync: Enables the use of Cloudwatch Metric Streams for metrics synchronization.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: IntegrationArgs,
@@ -1018,49 +1016,48 @@
         """
         Get an existing Integration resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] auth_method: The mechanism used to authenticate with AWS. Use one of `signalfx_aws_external_integration` or
-               `signalfx_aws_token_integration` to define this
+        :param pulumi.Input[str] auth_method: The mechanism used to authenticate with AWS. Use one of `aws.ExternalIntegration` or `aws.TokenIntegration` to define
+               this
         :param pulumi.Input[Sequence[pulumi.Input[str]]] custom_cloudwatch_namespaces: List of custom AWS CloudWatch namespaces to monitor. Custom namespaces contain custom metrics that you define in AWS;
                Splunk Observability imports the metrics so you can monitor them.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['IntegrationCustomNamespaceSyncRuleArgs']]]] custom_namespace_sync_rules: Each element controls the data collected by Splunk Observability for the specified namespace. If you specify this
                property, Splunk Observability ignores values in the "custom_cloudwatch_namespaces" property.
         :param pulumi.Input[bool] enable_aws_usage: Flag that controls how Splunk Observability imports usage metrics from AWS to use with AWS Cost Optimizer. If `true`,
                Splunk Observability imports the metrics.
         :param pulumi.Input[bool] enable_check_large_volume: Controls how Splunk Observability checks for large amounts of data for this AWS integration. If true, Splunk
                Observability monitors the amount of data coming in from the integration.
         :param pulumi.Input[bool] enable_logs_sync: Enables AWS logs synchronization.
         :param pulumi.Input[bool] enabled: Whether the integration is enabled or not
-        :param pulumi.Input[str] external_id: Used with `signalfx_aws_external_integration`. Use this property to specify the external id.
+        :param pulumi.Input[str] external_id: Used with `aws.ExternalIntegration`. Use this property to specify the external id.
         :param pulumi.Input[bool] import_cloud_watch: Flag that controls how Splunk Observability imports Cloud Watch metrics. If true, Splunk Observability imports Cloud
                Watch metrics from AWS.
         :param pulumi.Input[str] integration_id: The ID of this integration
-        :param pulumi.Input[str] key: Used with `signalfx_aws_token_integration`. Use this property to specify the token.
+        :param pulumi.Input[str] key: Used with `aws.TokenIntegration`. Use this property to specify the token.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['IntegrationMetricStatsToSyncArgs']]]] metric_stats_to_syncs: Each element in the array is an object that contains an AWS namespace name, AWS metric name and a list of statistics
                that Splunk Observability collects for this metric. If you specify this property, Splunk Observability retrieves only
                specified AWS statistics. If you don't specify this property, Splunk Observability retrieves the AWS standard set of
                statistics.
-        :param pulumi.Input[str] name: Name of the integration. Please specify the name in `signalfx_aws_external_integration` or
-               `signalfx_aws_integration_token`
+        :param pulumi.Input[str] name: Name of the integration. Please specify the name in `aws.ExternalIntegration` or `signalfx_aws_integration_token`
         :param pulumi.Input[str] named_token: A named token to use for ingest
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['IntegrationNamespaceSyncRuleArgs']]]] namespace_sync_rules: Each element in the array is an object that contains an AWS namespace name and a filter that controls the data that
                Splunk Observability collects for the namespace. If you specify this property, Splunk Observability ignores the values
                in the AWS CloudWatch Integration Model "services" property. If you don't specify either property, Splunk Observability
                syncs all data in all AWS namespaces.
         :param pulumi.Input[int] poll_rate: AWS poll rate (in seconds). Between `60` and `600`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] regions: List of AWS regions that Splunk Observability should monitor.
-        :param pulumi.Input[str] role_arn: Used with `signalfx_aws_external_integration`. Use this property to specify the AIM role ARN.
+        :param pulumi.Input[str] role_arn: Used with `aws.ExternalIntegration`. Use this property to specify the AIM role ARN.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] services: List of AWS services that you want Splunk Observability to monitor. Each element is a string designating an AWS service.
         :param pulumi.Input[bool] sync_custom_namespaces_only: Indicates that Splunk Observability should sync metrics and metadata from custom AWS namespaces only (see the
                `custom_namespace_sync_rule` field for details). Defaults to `false`.
-        :param pulumi.Input[str] token: Used with `signalfx_aws_token_integration`. Use this property to specify the token.
+        :param pulumi.Input[str] token: Used with `aws.TokenIntegration`. Use this property to specify the token.
         :param pulumi.Input[bool] use_metric_streams_sync: Enables the use of Cloudwatch Metric Streams for metrics synchronization.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _IntegrationState.__new__(_IntegrationState)
 
         __props__.__dict__["auth_method"] = auth_method
@@ -1087,16 +1084,16 @@
         __props__.__dict__["use_metric_streams_sync"] = use_metric_streams_sync
         return Integration(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter(name="authMethod")
     def auth_method(self) -> pulumi.Output[str]:
         """
-        The mechanism used to authenticate with AWS. Use one of `signalfx_aws_external_integration` or
-        `signalfx_aws_token_integration` to define this
+        The mechanism used to authenticate with AWS. Use one of `aws.ExternalIntegration` or `aws.TokenIntegration` to define
+        this
         """
         return pulumi.get(self, "auth_method")
 
     @property
     @pulumi.getter(name="customCloudwatchNamespaces")
     def custom_cloudwatch_namespaces(self) -> pulumi.Output[Optional[Sequence[str]]]:
         """
@@ -1148,15 +1145,15 @@
         """
         return pulumi.get(self, "enabled")
 
     @property
     @pulumi.getter(name="externalId")
     def external_id(self) -> pulumi.Output[Optional[str]]:
         """
-        Used with `signalfx_aws_external_integration`. Use this property to specify the external id.
+        Used with `aws.ExternalIntegration`. Use this property to specify the external id.
         """
         return pulumi.get(self, "external_id")
 
     @property
     @pulumi.getter(name="importCloudWatch")
     def import_cloud_watch(self) -> pulumi.Output[Optional[bool]]:
         """
@@ -1173,15 +1170,15 @@
         """
         return pulumi.get(self, "integration_id")
 
     @property
     @pulumi.getter
     def key(self) -> pulumi.Output[Optional[str]]:
         """
-        Used with `signalfx_aws_token_integration`. Use this property to specify the token.
+        Used with `aws.TokenIntegration`. Use this property to specify the token.
         """
         return pulumi.get(self, "key")
 
     @property
     @pulumi.getter(name="metricStatsToSyncs")
     def metric_stats_to_syncs(self) -> pulumi.Output[Optional[Sequence['outputs.IntegrationMetricStatsToSync']]]:
         """
@@ -1192,16 +1189,15 @@
         """
         return pulumi.get(self, "metric_stats_to_syncs")
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Output[str]:
         """
-        Name of the integration. Please specify the name in `signalfx_aws_external_integration` or
-        `signalfx_aws_integration_token`
+        Name of the integration. Please specify the name in `aws.ExternalIntegration` or `signalfx_aws_integration_token`
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="namedToken")
     def named_token(self) -> pulumi.Output[Optional[str]]:
         """
@@ -1236,15 +1232,15 @@
         """
         return pulumi.get(self, "regions")
 
     @property
     @pulumi.getter(name="roleArn")
     def role_arn(self) -> pulumi.Output[Optional[str]]:
         """
-        Used with `signalfx_aws_external_integration`. Use this property to specify the AIM role ARN.
+        Used with `aws.ExternalIntegration`. Use this property to specify the AIM role ARN.
         """
         return pulumi.get(self, "role_arn")
 
     @property
     @pulumi.getter
     def services(self) -> pulumi.Output[Optional[Sequence[str]]]:
         """
@@ -1261,15 +1257,15 @@
         """
         return pulumi.get(self, "sync_custom_namespaces_only")
 
     @property
     @pulumi.getter
     def token(self) -> pulumi.Output[Optional[str]]:
         """
-        Used with `signalfx_aws_token_integration`. Use this property to specify the token.
+        Used with `aws.TokenIntegration`. Use this property to specify the token.
         """
         return pulumi.get(self, "token")
 
     @property
     @pulumi.getter(name="useMetricStreamsSync")
     def use_metric_streams_sync(self) -> pulumi.Output[bool]:
         """
```

### Comparing `pulumi_signalfx-7.2.0a1715236218/pulumi_signalfx/aws/outputs.py` & `pulumi_signalfx-7.2.0a1715305180/pulumi_signalfx/aws/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1715236218/pulumi_signalfx/aws/token_integration.py` & `pulumi_signalfx-7.2.0a1715305180/pulumi_signalfx/aws/token_integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1715236218/pulumi_signalfx/azure/_inputs.py` & `pulumi_signalfx-7.2.0a1715305180/pulumi_signalfx/azure/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1715236218/pulumi_signalfx/azure/integration.py` & `pulumi_signalfx-7.2.0a1715305180/pulumi_signalfx/azure/integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1715236218/pulumi_signalfx/azure/outputs.py` & `pulumi_signalfx-7.2.0a1715305180/pulumi_signalfx/azure/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1715236218/pulumi_signalfx/config/__init__.pyi` & `pulumi_signalfx-7.2.0a1715305180/pulumi_signalfx/config/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1715236218/pulumi_signalfx/config/vars.py` & `pulumi_signalfx-7.2.0a1715305180/pulumi_signalfx/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1715236218/pulumi_signalfx/dashboard.py` & `pulumi_signalfx-7.2.0a1715305180/pulumi_signalfx/dashboard.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1715236218/pulumi_signalfx/dashboard_group.py` & `pulumi_signalfx-7.2.0a1715305180/pulumi_signalfx/dashboard_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1715236218/pulumi_signalfx/data_link.py` & `pulumi_signalfx-7.2.0a1715305180/pulumi_signalfx/data_link.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1715236218/pulumi_signalfx/detector.py` & `pulumi_signalfx-7.2.0a1715305180/pulumi_signalfx/detector.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1715236218/pulumi_signalfx/event_feed_chart.py` & `pulumi_signalfx-7.2.0a1715305180/pulumi_signalfx/event_feed_chart.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1715236218/pulumi_signalfx/gcp/_inputs.py` & `pulumi_signalfx-7.2.0a1715305180/pulumi_signalfx/gcp/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1715236218/pulumi_signalfx/gcp/integration.py` & `pulumi_signalfx-7.2.0a1715305180/pulumi_signalfx/gcp/integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1715236218/pulumi_signalfx/gcp/outputs.py` & `pulumi_signalfx-7.2.0a1715305180/pulumi_signalfx/gcp/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1715236218/pulumi_signalfx/get_dimension_values.py` & `pulumi_signalfx-7.2.0a1715305180/pulumi_signalfx/get_dimension_values.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1715236218/pulumi_signalfx/heatmap_chart.py` & `pulumi_signalfx-7.2.0a1715305180/pulumi_signalfx/heatmap_chart.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1715236218/pulumi_signalfx/jira/integration.py` & `pulumi_signalfx-7.2.0a1715305180/pulumi_signalfx/jira/integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1715236218/pulumi_signalfx/list_chart.py` & `pulumi_signalfx-7.2.0a1715305180/pulumi_signalfx/list_chart.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1715236218/pulumi_signalfx/log/_inputs.py` & `pulumi_signalfx-7.2.0a1715305180/pulumi_signalfx/log/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1715236218/pulumi_signalfx/log/outputs.py` & `pulumi_signalfx-7.2.0a1715305180/pulumi_signalfx/log/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1715236218/pulumi_signalfx/log/timeline.py` & `pulumi_signalfx-7.2.0a1715305180/pulumi_signalfx/log/timeline.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1715236218/pulumi_signalfx/log/view.py` & `pulumi_signalfx-7.2.0a1715305180/pulumi_signalfx/log/view.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1715236218/pulumi_signalfx/metric_ruleset.py` & `pulumi_signalfx-7.2.0a1715305180/pulumi_signalfx/metric_ruleset.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1715236218/pulumi_signalfx/opsgenie/integration.py` & `pulumi_signalfx-7.2.0a1715305180/pulumi_signalfx/opsgenie/integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1715236218/pulumi_signalfx/org_token.py` & `pulumi_signalfx-7.2.0a1715305180/pulumi_signalfx/org_token.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1715236218/pulumi_signalfx/outputs.py` & `pulumi_signalfx-7.2.0a1715305180/pulumi_signalfx/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1715236218/pulumi_signalfx/pagerduty/get_integration.py` & `pulumi_signalfx-7.2.0a1715305180/pulumi_signalfx/pagerduty/get_integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1715236218/pulumi_signalfx/pagerduty/integration.py` & `pulumi_signalfx-7.2.0a1715305180/pulumi_signalfx/pagerduty/integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1715236218/pulumi_signalfx/provider.py` & `pulumi_signalfx-7.2.0a1715305180/pulumi_signalfx/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1715236218/pulumi_signalfx/servicenow/integration.py` & `pulumi_signalfx-7.2.0a1715305180/pulumi_signalfx/servicenow/integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1715236218/pulumi_signalfx/single_value_chart.py` & `pulumi_signalfx-7.2.0a1715305180/pulumi_signalfx/single_value_chart.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1715236218/pulumi_signalfx/slack/integration.py` & `pulumi_signalfx-7.2.0a1715305180/pulumi_signalfx/slack/integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1715236218/pulumi_signalfx/slo.py` & `pulumi_signalfx-7.2.0a1715305180/pulumi_signalfx/slo.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1715236218/pulumi_signalfx/table_chart.py` & `pulumi_signalfx-7.2.0a1715305180/pulumi_signalfx/table_chart.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1715236218/pulumi_signalfx/team.py` & `pulumi_signalfx-7.2.0a1715305180/pulumi_signalfx/team.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1715236218/pulumi_signalfx/text_chart.py` & `pulumi_signalfx-7.2.0a1715305180/pulumi_signalfx/text_chart.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1715236218/pulumi_signalfx/time_chart.py` & `pulumi_signalfx-7.2.0a1715305180/pulumi_signalfx/time_chart.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1715236218/pulumi_signalfx/victorops/integration.py` & `pulumi_signalfx-7.2.0a1715305180/pulumi_signalfx/victorops/integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1715236218/pulumi_signalfx/webhook_integration.py` & `pulumi_signalfx-7.2.0a1715305180/pulumi_signalfx/webhook_integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1715236218/pulumi_signalfx.egg-info/PKG-INFO` & `pulumi_signalfx-7.2.0a1715305180/pulumi_signalfx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_signalfx
-Version: 7.2.0a1715236218
+Version: 7.2.0a1715305180
 Summary: A Pulumi package for creating and managing SignalFx resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-signalfx
 Keywords: pulumi,signalfx
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_signalfx-7.2.0a1715236218/pulumi_signalfx.egg-info/SOURCES.txt` & `pulumi_signalfx-7.2.0a1715305180/pulumi_signalfx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1715236218/pyproject.toml` & `pulumi_signalfx-7.2.0a1715305180/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_signalfx"
   description = "A Pulumi package for creating and managing SignalFx resources."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "signalfx"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "7.2.0a1715236218"
+  version = "7.2.0a1715305180"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://pulumi.io"
     Repository = "https://github.com/pulumi/pulumi-signalfx"
 
 [build-system]
```

