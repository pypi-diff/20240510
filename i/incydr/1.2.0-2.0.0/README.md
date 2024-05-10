# Comparing `tmp/incydr-1.2.0.tar.gz` & `tmp/incydr-2.0.0.tar.gz`

## Comparing `incydr-1.2.0.tar` & `incydr-2.0.0.tar`

### file list

```diff
@@ -1,106 +1,116 @@
--rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 incydr-1.2.0/_incydr_cli/__init__.py
--rw-r--r--   0        0        0     5619 2020-02-02 00:00:00.000000 incydr-1.2.0/_incydr_cli/core.py
--rw-r--r--   0        0        0     3164 2020-02-02 00:00:00.000000 incydr-1.2.0/_incydr_cli/cursor.py
--rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 incydr-1.2.0/_incydr_cli/exceptions.py
--rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 incydr-1.2.0/_incydr_cli/file_readers.py
--rw-r--r--   0        0        0     2783 2020-02-02 00:00:00.000000 incydr-1.2.0/_incydr_cli/main.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 incydr-1.2.0/_incydr_cli/render.py
--rw-r--r--   0        0        0    22896 2020-02-02 00:00:00.000000 incydr-1.2.0/_incydr_cli/rich_utils.py
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 incydr-1.2.0/_incydr_cli/utils.py
--rw-r--r--   0        0        0     8994 2020-02-02 00:00:00.000000 incydr-1.2.0/_incydr_cli/cmds/agents.py
--rw-r--r--   0        0        0     6793 2020-02-02 00:00:00.000000 incydr-1.2.0/_incydr_cli/cmds/alert_rules.py
--rw-r--r--   0        0        0    12979 2020-02-02 00:00:00.000000 incydr-1.2.0/_incydr_cli/cmds/alerts.py
--rw-r--r--   0        0        0    10318 2020-02-02 00:00:00.000000 incydr-1.2.0/_incydr_cli/cmds/audit_log.py
--rw-r--r--   0        0        0    17742 2020-02-02 00:00:00.000000 incydr-1.2.0/_incydr_cli/cmds/cases.py
--rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 incydr-1.2.0/_incydr_cli/cmds/departments.py
--rw-r--r--   0        0        0     2755 2020-02-02 00:00:00.000000 incydr-1.2.0/_incydr_cli/cmds/devices.py
--rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 incydr-1.2.0/_incydr_cli/cmds/directory_groups.py
--rw-r--r--   0        0        0    10015 2020-02-02 00:00:00.000000 incydr-1.2.0/_incydr_cli/cmds/file_events.py
--rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 incydr-1.2.0/_incydr_cli/cmds/models.py
--rw-r--r--   0        0        0    12079 2020-02-02 00:00:00.000000 incydr-1.2.0/_incydr_cli/cmds/trusted_activities.py
--rw-r--r--   0        0        0    10965 2020-02-02 00:00:00.000000 incydr-1.2.0/_incydr_cli/cmds/user_risk_profiles.py
--rw-r--r--   0        0        0    15938 2020-02-02 00:00:00.000000 incydr-1.2.0/_incydr_cli/cmds/users.py
--rw-r--r--   0        0        0     2109 2020-02-02 00:00:00.000000 incydr-1.2.0/_incydr_cli/cmds/utils.py
--rw-r--r--   0        0        0    25269 2020-02-02 00:00:00.000000 incydr-1.2.0/_incydr_cli/cmds/watchlists.py
--rw-r--r--   0        0        0     3661 2020-02-02 00:00:00.000000 incydr-1.2.0/_incydr_cli/cmds/options/alert_filter_options.py
--rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 incydr-1.2.0/_incydr_cli/cmds/options/audit_log_filter_options.py
--rw-r--r--   0        0        0     5243 2020-02-02 00:00:00.000000 incydr-1.2.0/_incydr_cli/cmds/options/event_filter_options.py
--rw-r--r--   0        0        0     2683 2020-02-02 00:00:00.000000 incydr-1.2.0/_incydr_cli/cmds/options/output_options.py
--rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 incydr-1.2.0/_incydr_cli/cmds/options/profile_filter_options.py
--rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 incydr-1.2.0/_incydr_cli/cmds/options/utils.py
--rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 incydr-1.2.0/_incydr_cli/logger/__init__.py
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 incydr-1.2.0/_incydr_cli/logger/enums.py
--rw-r--r--   0        0        0     5016 2020-02-02 00:00:00.000000 incydr-1.2.0/_incydr_cli/logger/handlers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 incydr-1.2.0/_incydr_sdk/__init__.py
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 incydr-1.2.0/_incydr_sdk/__version__.py
--rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 incydr-1.2.0/_incydr_sdk/exceptions.py
--rw-r--r--   0        0        0     8485 2020-02-02 00:00:00.000000 incydr-1.2.0/_incydr_sdk/utils.py
--rw-r--r--   0        0        0     6274 2020-02-02 00:00:00.000000 incydr-1.2.0/_incydr_sdk/agents/client.py
--rw-r--r--   0        0        0     4165 2020-02-02 00:00:00.000000 incydr-1.2.0/_incydr_sdk/agents/models.py
--rw-r--r--   0        0        0     5971 2020-02-02 00:00:00.000000 incydr-1.2.0/_incydr_sdk/alert_rules/client.py
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 incydr-1.2.0/_incydr_sdk/alert_rules/models/request.py
--rw-r--r--   0        0        0    16555 2020-02-02 00:00:00.000000 incydr-1.2.0/_incydr_sdk/alert_rules/models/response.py
--rw-r--r--   0        0        0     5351 2020-02-02 00:00:00.000000 incydr-1.2.0/_incydr_sdk/alerts/client.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 incydr-1.2.0/_incydr_sdk/alerts/models/__init__.py
--rw-r--r--   0        0        0     9912 2020-02-02 00:00:00.000000 incydr-1.2.0/_incydr_sdk/alerts/models/alert.py
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 incydr-1.2.0/_incydr_sdk/alerts/models/enums.py
--rw-r--r--   0        0        0     1897 2020-02-02 00:00:00.000000 incydr-1.2.0/_incydr_sdk/alerts/models/request.py
--rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 incydr-1.2.0/_incydr_sdk/alerts/models/response.py
--rw-r--r--   0        0        0    11953 2020-02-02 00:00:00.000000 incydr-1.2.0/_incydr_sdk/audit_log/client.py
--rw-r--r--   0        0        0     2403 2020-02-02 00:00:00.000000 incydr-1.2.0/_incydr_sdk/audit_log/models.py
--rw-r--r--   0        0        0    15787 2020-02-02 00:00:00.000000 incydr-1.2.0/_incydr_sdk/cases/client.py
--rw-r--r--   0        0        0     8301 2020-02-02 00:00:00.000000 incydr-1.2.0/_incydr_sdk/cases/models.py
--rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 incydr-1.2.0/_incydr_sdk/core/auth.py
--rw-r--r--   0        0        0    10268 2020-02-02 00:00:00.000000 incydr-1.2.0/_incydr_sdk/core/client.py
--rw-r--r--   0        0        0     6599 2020-02-02 00:00:00.000000 incydr-1.2.0/_incydr_sdk/core/models.py
--rw-r--r--   0        0        0     9792 2020-02-02 00:00:00.000000 incydr-1.2.0/_incydr_sdk/core/settings.py
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 incydr-1.2.0/_incydr_sdk/core/utils.py
--rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 incydr-1.2.0/_incydr_sdk/customer/client.py
--rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 incydr-1.2.0/_incydr_sdk/customer/models.py
--rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 incydr-1.2.0/_incydr_sdk/departments/client.py
--rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 incydr-1.2.0/_incydr_sdk/departments/models.py
--rw-r--r--   0        0        0     3720 2020-02-02 00:00:00.000000 incydr-1.2.0/_incydr_sdk/devices/client.py
--rw-r--r--   0        0        0     7898 2020-02-02 00:00:00.000000 incydr-1.2.0/_incydr_sdk/devices/models.py
--rw-r--r--   0        0        0     2326 2020-02-02 00:00:00.000000 incydr-1.2.0/_incydr_sdk/directory_groups/client.py
--rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 incydr-1.2.0/_incydr_sdk/directory_groups/models.py
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 incydr-1.2.0/_incydr_sdk/enums/__init__.py
--rw-r--r--   0        0        0     1841 2020-02-02 00:00:00.000000 incydr-1.2.0/_incydr_sdk/enums/alerts.py
--rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 incydr-1.2.0/_incydr_sdk/enums/cases.py
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 incydr-1.2.0/_incydr_sdk/enums/devices.py
--rw-r--r--   0        0        0    20195 2020-02-02 00:00:00.000000 incydr-1.2.0/_incydr_sdk/enums/file_events.py
--rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 incydr-1.2.0/_incydr_sdk/enums/trusted_activities.py
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 incydr-1.2.0/_incydr_sdk/enums/watchlists.py
--rw-r--r--   0        0        0     5093 2020-02-02 00:00:00.000000 incydr-1.2.0/_incydr_sdk/file_events/client.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 incydr-1.2.0/_incydr_sdk/file_events/models/__init__.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 incydr-1.2.0/_incydr_sdk/file_events/models/enums.py
--rw-r--r--   0        0        0    32082 2020-02-02 00:00:00.000000 incydr-1.2.0/_incydr_sdk/file_events/models/event.py
--rw-r--r--   0        0        0     7490 2020-02-02 00:00:00.000000 incydr-1.2.0/_incydr_sdk/file_events/models/response.py
--rw-r--r--   0        0        0     9950 2020-02-02 00:00:00.000000 incydr-1.2.0/_incydr_sdk/queries/alerts.py
--rw-r--r--   0        0        0    12185 2020-02-02 00:00:00.000000 incydr-1.2.0/_incydr_sdk/queries/file_events.py
--rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 incydr-1.2.0/_incydr_sdk/queries/utils.py
--rw-r--r--   0        0        0    15252 2020-02-02 00:00:00.000000 incydr-1.2.0/_incydr_sdk/trusted_activities/client.py
--rw-r--r--   0        0        0     7109 2020-02-02 00:00:00.000000 incydr-1.2.0/_incydr_sdk/trusted_activities/models.py
--rw-r--r--   0        0        0     9299 2020-02-02 00:00:00.000000 incydr-1.2.0/_incydr_sdk/user_risk_profiles/client.py
--rw-r--r--   0        0        0     6251 2020-02-02 00:00:00.000000 incydr-1.2.0/_incydr_sdk/user_risk_profiles/models.py
--rw-r--r--   0        0        0    14133 2020-02-02 00:00:00.000000 incydr-1.2.0/_incydr_sdk/users/client.py
--rw-r--r--   0        0        0     8679 2020-02-02 00:00:00.000000 incydr-1.2.0/_incydr_sdk/users/models.py
--rw-r--r--   0        0        0    19422 2020-02-02 00:00:00.000000 incydr-1.2.0/_incydr_sdk/watchlists/client.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 incydr-1.2.0/_incydr_sdk/watchlists/models/__init__.py
--rw-r--r--   0        0        0     2079 2020-02-02 00:00:00.000000 incydr-1.2.0/_incydr_sdk/watchlists/models/requests.py
--rw-r--r--   0        0        0     9515 2020-02-02 00:00:00.000000 incydr-1.2.0/_incydr_sdk/watchlists/models/responses.py
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 incydr-1.2.0/incydr/__init__.py
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 incydr-1.2.0/incydr/__main__.py
--rw-r--r--   0        0        0     3437 2020-02-02 00:00:00.000000 incydr-1.2.0/incydr/models.py
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 incydr-1.2.0/incydr/enums/__init__.py
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 incydr-1.2.0/incydr/enums/agents.py
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 incydr-1.2.0/incydr/enums/alerts.py
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 incydr-1.2.0/incydr/enums/cases.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 incydr-1.2.0/incydr/enums/devices.py
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 incydr-1.2.0/incydr/enums/file_events.py
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 incydr-1.2.0/incydr/enums/trusted_activities.py
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 incydr-1.2.0/incydr/enums/watchlists.py
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 incydr-1.2.0/.gitignore
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 incydr-1.2.0/LICENSE.txt
--rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 incydr-1.2.0/README.md
--rw-r--r--   0        0        0     2644 2020-02-02 00:00:00.000000 incydr-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     2523 2020-02-02 00:00:00.000000 incydr-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 incydr-2.0.0/_incydr_cli/__init__.py
+-rw-r--r--   0        0        0     5619 2020-02-02 00:00:00.000000 incydr-2.0.0/_incydr_cli/core.py
+-rw-r--r--   0        0        0     3186 2020-02-02 00:00:00.000000 incydr-2.0.0/_incydr_cli/cursor.py
+-rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 incydr-2.0.0/_incydr_cli/exceptions.py
+-rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 incydr-2.0.0/_incydr_cli/file_readers.py
+-rw-r--r--   0        0        0     2924 2020-02-02 00:00:00.000000 incydr-2.0.0/_incydr_cli/main.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 incydr-2.0.0/_incydr_cli/render.py
+-rw-r--r--   0        0        0    22896 2020-02-02 00:00:00.000000 incydr-2.0.0/_incydr_cli/rich_utils.py
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 incydr-2.0.0/_incydr_cli/utils.py
+-rw-r--r--   0        0        0     6032 2020-02-02 00:00:00.000000 incydr-2.0.0/_incydr_cli/cmds/actors.py
+-rw-r--r--   0        0        0     8994 2020-02-02 00:00:00.000000 incydr-2.0.0/_incydr_cli/cmds/agents.py
+-rw-r--r--   0        0        0     6793 2020-02-02 00:00:00.000000 incydr-2.0.0/_incydr_cli/cmds/alert_rules.py
+-rw-r--r--   0        0        0    13224 2020-02-02 00:00:00.000000 incydr-2.0.0/_incydr_cli/cmds/alerts.py
+-rw-r--r--   0        0        0    10318 2020-02-02 00:00:00.000000 incydr-2.0.0/_incydr_cli/cmds/audit_log.py
+-rw-r--r--   0        0        0    17745 2020-02-02 00:00:00.000000 incydr-2.0.0/_incydr_cli/cmds/cases.py
+-rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 incydr-2.0.0/_incydr_cli/cmds/departments.py
+-rw-r--r--   0        0        0     2755 2020-02-02 00:00:00.000000 incydr-2.0.0/_incydr_cli/cmds/devices.py
+-rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 incydr-2.0.0/_incydr_cli/cmds/directory_groups.py
+-rw-r--r--   0        0        0    10015 2020-02-02 00:00:00.000000 incydr-2.0.0/_incydr_cli/cmds/file_events.py
+-rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 incydr-2.0.0/_incydr_cli/cmds/models.py
+-rw-r--r--   0        0        0     5872 2020-02-02 00:00:00.000000 incydr-2.0.0/_incydr_cli/cmds/risk_profiles.py
+-rw-r--r--   0        0        0    14266 2020-02-02 00:00:00.000000 incydr-2.0.0/_incydr_cli/cmds/sessions.py
+-rw-r--r--   0        0        0    12079 2020-02-02 00:00:00.000000 incydr-2.0.0/_incydr_cli/cmds/trusted_activities.py
+-rw-r--r--   0        0        0    15938 2020-02-02 00:00:00.000000 incydr-2.0.0/_incydr_cli/cmds/users.py
+-rw-r--r--   0        0        0     2207 2020-02-02 00:00:00.000000 incydr-2.0.0/_incydr_cli/cmds/utils.py
+-rw-r--r--   0        0        0    25269 2020-02-02 00:00:00.000000 incydr-2.0.0/_incydr_cli/cmds/watchlists.py
+-rw-r--r--   0        0        0     3661 2020-02-02 00:00:00.000000 incydr-2.0.0/_incydr_cli/cmds/options/alert_filter_options.py
+-rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 incydr-2.0.0/_incydr_cli/cmds/options/audit_log_filter_options.py
+-rw-r--r--   0        0        0     5243 2020-02-02 00:00:00.000000 incydr-2.0.0/_incydr_cli/cmds/options/event_filter_options.py
+-rw-r--r--   0        0        0     2683 2020-02-02 00:00:00.000000 incydr-2.0.0/_incydr_cli/cmds/options/output_options.py
+-rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 incydr-2.0.0/_incydr_cli/cmds/options/profile_filter_options.py
+-rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 incydr-2.0.0/_incydr_cli/cmds/options/utils.py
+-rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 incydr-2.0.0/_incydr_cli/logger/__init__.py
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 incydr-2.0.0/_incydr_cli/logger/enums.py
+-rw-r--r--   0        0        0     5016 2020-02-02 00:00:00.000000 incydr-2.0.0/_incydr_cli/logger/handlers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 incydr-2.0.0/_incydr_sdk/__init__.py
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 incydr-2.0.0/_incydr_sdk/__version__.py
+-rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 incydr-2.0.0/_incydr_sdk/exceptions.py
+-rw-r--r--   0        0        0     8485 2020-02-02 00:00:00.000000 incydr-2.0.0/_incydr_sdk/utils.py
+-rw-r--r--   0        0        0     6938 2020-02-02 00:00:00.000000 incydr-2.0.0/_incydr_sdk/actors/client.py
+-rw-r--r--   0        0        0     4908 2020-02-02 00:00:00.000000 incydr-2.0.0/_incydr_sdk/actors/models.py
+-rw-r--r--   0        0        0     6274 2020-02-02 00:00:00.000000 incydr-2.0.0/_incydr_sdk/agents/client.py
+-rw-r--r--   0        0        0     4165 2020-02-02 00:00:00.000000 incydr-2.0.0/_incydr_sdk/agents/models.py
+-rw-r--r--   0        0        0     5685 2020-02-02 00:00:00.000000 incydr-2.0.0/_incydr_sdk/alert_rules/client.py
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 incydr-2.0.0/_incydr_sdk/alert_rules/models/request.py
+-rw-r--r--   0        0        0    16555 2020-02-02 00:00:00.000000 incydr-2.0.0/_incydr_sdk/alert_rules/models/response.py
+-rw-r--r--   0        0        0     6092 2020-02-02 00:00:00.000000 incydr-2.0.0/_incydr_sdk/alerts/client.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 incydr-2.0.0/_incydr_sdk/alerts/models/__init__.py
+-rw-r--r--   0        0        0     9912 2020-02-02 00:00:00.000000 incydr-2.0.0/_incydr_sdk/alerts/models/alert.py
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 incydr-2.0.0/_incydr_sdk/alerts/models/enums.py
+-rw-r--r--   0        0        0     1897 2020-02-02 00:00:00.000000 incydr-2.0.0/_incydr_sdk/alerts/models/request.py
+-rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 incydr-2.0.0/_incydr_sdk/alerts/models/response.py
+-rw-r--r--   0        0        0    11953 2020-02-02 00:00:00.000000 incydr-2.0.0/_incydr_sdk/audit_log/client.py
+-rw-r--r--   0        0        0     2403 2020-02-02 00:00:00.000000 incydr-2.0.0/_incydr_sdk/audit_log/models.py
+-rw-r--r--   0        0        0    15787 2020-02-02 00:00:00.000000 incydr-2.0.0/_incydr_sdk/cases/client.py
+-rw-r--r--   0        0        0     8301 2020-02-02 00:00:00.000000 incydr-2.0.0/_incydr_sdk/cases/models.py
+-rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 incydr-2.0.0/_incydr_sdk/core/auth.py
+-rw-r--r--   0        0        0    10965 2020-02-02 00:00:00.000000 incydr-2.0.0/_incydr_sdk/core/client.py
+-rw-r--r--   0        0        0     6599 2020-02-02 00:00:00.000000 incydr-2.0.0/_incydr_sdk/core/models.py
+-rw-r--r--   0        0        0     9792 2020-02-02 00:00:00.000000 incydr-2.0.0/_incydr_sdk/core/settings.py
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 incydr-2.0.0/_incydr_sdk/core/utils.py
+-rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 incydr-2.0.0/_incydr_sdk/customer/client.py
+-rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 incydr-2.0.0/_incydr_sdk/customer/models.py
+-rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 incydr-2.0.0/_incydr_sdk/departments/client.py
+-rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 incydr-2.0.0/_incydr_sdk/departments/models.py
+-rw-r--r--   0        0        0     3720 2020-02-02 00:00:00.000000 incydr-2.0.0/_incydr_sdk/devices/client.py
+-rw-r--r--   0        0        0     7898 2020-02-02 00:00:00.000000 incydr-2.0.0/_incydr_sdk/devices/models.py
+-rw-r--r--   0        0        0     2326 2020-02-02 00:00:00.000000 incydr-2.0.0/_incydr_sdk/directory_groups/client.py
+-rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 incydr-2.0.0/_incydr_sdk/directory_groups/models.py
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 incydr-2.0.0/_incydr_sdk/enums/__init__.py
+-rw-r--r--   0        0        0     1841 2020-02-02 00:00:00.000000 incydr-2.0.0/_incydr_sdk/enums/alerts.py
+-rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 incydr-2.0.0/_incydr_sdk/enums/cases.py
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 incydr-2.0.0/_incydr_sdk/enums/devices.py
+-rw-r--r--   0        0        0    20195 2020-02-02 00:00:00.000000 incydr-2.0.0/_incydr_sdk/enums/file_events.py
+-rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 incydr-2.0.0/_incydr_sdk/enums/sessions.py
+-rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 incydr-2.0.0/_incydr_sdk/enums/trusted_activities.py
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 incydr-2.0.0/_incydr_sdk/enums/watchlists.py
+-rw-r--r--   0        0        0     5093 2020-02-02 00:00:00.000000 incydr-2.0.0/_incydr_sdk/file_events/client.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 incydr-2.0.0/_incydr_sdk/file_events/models/__init__.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 incydr-2.0.0/_incydr_sdk/file_events/models/enums.py
+-rw-r--r--   0        0        0    32082 2020-02-02 00:00:00.000000 incydr-2.0.0/_incydr_sdk/file_events/models/event.py
+-rw-r--r--   0        0        0     7490 2020-02-02 00:00:00.000000 incydr-2.0.0/_incydr_sdk/file_events/models/response.py
+-rw-r--r--   0        0        0     9950 2020-02-02 00:00:00.000000 incydr-2.0.0/_incydr_sdk/queries/alerts.py
+-rw-r--r--   0        0        0    12185 2020-02-02 00:00:00.000000 incydr-2.0.0/_incydr_sdk/queries/file_events.py
+-rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 incydr-2.0.0/_incydr_sdk/queries/utils.py
+-rw-r--r--   0        0        0     7614 2020-02-02 00:00:00.000000 incydr-2.0.0/_incydr_sdk/risk_profiles/client.py
+-rw-r--r--   0        0        0     6263 2020-02-02 00:00:00.000000 incydr-2.0.0/_incydr_sdk/risk_profiles/models.py
+-rw-r--r--   0        0        0    14804 2020-02-02 00:00:00.000000 incydr-2.0.0/_incydr_sdk/sessions/client.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 incydr-2.0.0/_incydr_sdk/sessions/models/__init__.py
+-rw-r--r--   0        0        0     2449 2020-02-02 00:00:00.000000 incydr-2.0.0/_incydr_sdk/sessions/models/models.py
+-rw-r--r--   0        0        0     4276 2020-02-02 00:00:00.000000 incydr-2.0.0/_incydr_sdk/sessions/models/response.py
+-rw-r--r--   0        0        0    15246 2020-02-02 00:00:00.000000 incydr-2.0.0/_incydr_sdk/trusted_activities/client.py
+-rw-r--r--   0        0        0     7109 2020-02-02 00:00:00.000000 incydr-2.0.0/_incydr_sdk/trusted_activities/models.py
+-rw-r--r--   0        0        0    14133 2020-02-02 00:00:00.000000 incydr-2.0.0/_incydr_sdk/users/client.py
+-rw-r--r--   0        0        0     8679 2020-02-02 00:00:00.000000 incydr-2.0.0/_incydr_sdk/users/models.py
+-rw-r--r--   0        0        0    19422 2020-02-02 00:00:00.000000 incydr-2.0.0/_incydr_sdk/watchlists/client.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 incydr-2.0.0/_incydr_sdk/watchlists/models/__init__.py
+-rw-r--r--   0        0        0     2079 2020-02-02 00:00:00.000000 incydr-2.0.0/_incydr_sdk/watchlists/models/requests.py
+-rw-r--r--   0        0        0     9515 2020-02-02 00:00:00.000000 incydr-2.0.0/_incydr_sdk/watchlists/models/responses.py
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 incydr-2.0.0/incydr/__init__.py
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 incydr-2.0.0/incydr/__main__.py
+-rw-r--r--   0        0        0     3758 2020-02-02 00:00:00.000000 incydr-2.0.0/incydr/models.py
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 incydr-2.0.0/incydr/enums/__init__.py
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 incydr-2.0.0/incydr/enums/agents.py
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 incydr-2.0.0/incydr/enums/alerts.py
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 incydr-2.0.0/incydr/enums/cases.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 incydr-2.0.0/incydr/enums/devices.py
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 incydr-2.0.0/incydr/enums/file_events.py
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 incydr-2.0.0/incydr/enums/sessions.py
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 incydr-2.0.0/incydr/enums/trusted_activities.py
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 incydr-2.0.0/incydr/enums/watchlists.py
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 incydr-2.0.0/.gitignore
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 incydr-2.0.0/LICENSE.txt
+-rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 incydr-2.0.0/README.md
+-rw-r--r--   0        0        0     2732 2020-02-02 00:00:00.000000 incydr-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     2625 2020-02-02 00:00:00.000000 incydr-2.0.0/PKG-INFO
```

### Comparing `incydr-1.2.0/_incydr_cli/__init__.py` & `incydr-2.0.0/_incydr_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `incydr-1.2.0/_incydr_cli/core.py` & `incydr-2.0.0/_incydr_cli/core.py`

 * *Files identical despite different names*

### Comparing `incydr-1.2.0/_incydr_cli/cursor.py` & `incydr-2.0.0/_incydr_cli/cursor.py`

 * *Files 9% similar despite different names*

```diff
@@ -73,23 +73,23 @@
         return [Cursor(f) for f in dir_contents if self._is_file(f)]
 
     def _is_file(self, node_name):
         return path.isfile(path.join(self._dir_path, node_name))
 
     def get_items(self, cursor_name):
         """
-        Used with alerts and audit_log events to avoid duplicates
+        Used with alerts, audit_log events, and sessions to avoid duplicates
         """
         try:
             location = path.join(self._dir_path, cursor_name) + f"_{self._event_key}"
             with open(location) as checkpoint:
                 return json.loads(checkpoint.read())
         except (FileNotFoundError, json.JSONDecodeError):
             return []
 
     def replace_items(self, cursor_name, new_events):
         """
-        Used with alerts and audit_log events to avoid duplicates
+        Used with alerts, audit_log events, and sessions to avoid duplicates
         """
         location = path.join(self._dir_path, cursor_name) + f"_{self._event_key}"
         with open(location, "w") as checkpoint:
             checkpoint.write(json.dumps(new_events))
```

### Comparing `incydr-1.2.0/_incydr_cli/exceptions.py` & `incydr-2.0.0/_incydr_cli/exceptions.py`

 * *Files identical despite different names*

### Comparing `incydr-1.2.0/_incydr_cli/file_readers.py` & `incydr-2.0.0/_incydr_cli/file_readers.py`

 * *Files identical despite different names*

### Comparing `incydr-1.2.0/_incydr_cli/main.py` & `incydr-2.0.0/_incydr_cli/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,25 +4,27 @@
 import sys
 
 import click
 from requests.exceptions import HTTPError
 
 from _incydr_cli import console
 from _incydr_cli import logging_options
+from _incydr_cli.cmds.actors import actors
 from _incydr_cli.cmds.agents import agents
 from _incydr_cli.cmds.alert_rules import alert_rules
 from _incydr_cli.cmds.alerts import alerts
 from _incydr_cli.cmds.audit_log import audit_log
 from _incydr_cli.cmds.cases import cases
 from _incydr_cli.cmds.departments import departments
 from _incydr_cli.cmds.devices import devices
 from _incydr_cli.cmds.directory_groups import directory_groups
 from _incydr_cli.cmds.file_events import file_events
+from _incydr_cli.cmds.risk_profiles import risk_profiles
+from _incydr_cli.cmds.sessions import sessions
 from _incydr_cli.cmds.trusted_activities import trusted_activities
-from _incydr_cli.cmds.user_risk_profiles import risk_profiles
 from _incydr_cli.cmds.users import users
 from _incydr_cli.cmds.watchlists import watchlists
 from _incydr_cli.core import ExceptionHandlingGroup
 from _incydr_sdk.__version__ import __version__
 
 if platform.system() in ("Darwin", "Linux"):
     os.environ["MANPAGER"] = "less -S"
@@ -63,24 +65,26 @@
 
         for root, _dirs, files in os.walk(site.USER_BASE):
             if "incydr" in files or "incydr.exe" in files:
                 console.print(root, highlight=False)
                 sys.exit(0)
 
 
+incydr.add_command(actors)
 incydr.add_command(agents)
 incydr.add_command(alerts)
 incydr.add_command(alert_rules)
 incydr.add_command(audit_log)
 incydr.add_command(departments)
 incydr.add_command(devices)
 incydr.add_command(directory_groups)
 incydr.add_command(file_events)
 incydr.add_command(cases)
 incydr.add_command(risk_profiles)
+incydr.add_command(sessions)
 incydr.add_command(trusted_activities)
 incydr.add_command(users)
 incydr.add_command(watchlists)
 
 if __name__ == "__main__":
     try:
         incydr()
```

### Comparing `incydr-1.2.0/_incydr_cli/render.py` & `incydr-2.0.0/_incydr_cli/render.py`

 * *Files identical despite different names*

### Comparing `incydr-1.2.0/_incydr_cli/rich_utils.py` & `incydr-2.0.0/_incydr_cli/rich_utils.py`

 * *Files identical despite different names*

### Comparing `incydr-1.2.0/_incydr_cli/utils.py` & `incydr-2.0.0/_incydr_cli/utils.py`

 * *Files identical despite different names*

### Comparing `incydr-1.2.0/_incydr_cli/cmds/agents.py` & `incydr-2.0.0/_incydr_cli/cmds/agents.py`

 * *Files identical despite different names*

### Comparing `incydr-1.2.0/_incydr_cli/cmds/alert_rules.py` & `incydr-2.0.0/_incydr_cli/cmds/alert_rules.py`

 * *Files identical despite different names*

### Comparing `incydr-1.2.0/_incydr_cli/cmds/alerts.py` & `incydr-2.0.0/_incydr_cli/cmds/alerts.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,32 +22,37 @@
 from _incydr_cli.cmds.options.output_options import input_format_option
 from _incydr_cli.cmds.options.output_options import output_options
 from _incydr_cli.cmds.options.output_options import single_format_option
 from _incydr_cli.cmds.options.output_options import SingleFormat
 from _incydr_cli.cmds.options.output_options import table_format_option
 from _incydr_cli.cmds.options.output_options import TableFormat
 from _incydr_cli.cmds.options.utils import checkpoint_option
+from _incydr_cli.cmds.utils import deprecation_warning
 from _incydr_cli.cmds.utils import warn_interrupt
 from _incydr_cli.core import IncydrCommand
 from _incydr_cli.core import IncydrGroup
 from _incydr_cli.cursor import CursorStore
 from _incydr_cli.file_readers import AutoDecodedFile
 from _incydr_cli.logger import get_server_logger
 from _incydr_sdk.alerts.models.alert import AlertSummary
 from _incydr_sdk.core.client import Client
 from _incydr_sdk.core.models import CSVModel
 from _incydr_sdk.core.models import Model
 from _incydr_sdk.queries.alerts import AlertQuery
 from _incydr_sdk.utils import model_as_card
 
+# Deprecated April 2024.
+DEPRECATION_TEXT = "DeprecationWarning: Alerts commands are deprecated. Use the 'incydr sessions' command group instead."
+
 
 @click.group(cls=IncydrGroup)
 @logging_options
 def alerts():
     """View and manage alerts."""
+    deprecation_warning(DEPRECATION_TEXT)
 
 
 @alerts.command(cls=IncydrCommand)
 @checkpoint_option
 @logging_options
 @columns_option
 @table_format_option
```

### Comparing `incydr-1.2.0/_incydr_cli/cmds/audit_log.py` & `incydr-2.0.0/_incydr_cli/cmds/audit_log.py`

 * *Files identical despite different names*

### Comparing `incydr-1.2.0/_incydr_cli/cmds/cases.py` & `incydr-2.0.0/_incydr_cli/cmds/cases.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,15 @@
     "--subject",
     help="User of the subject of the case.  Takes a user ID or a username.  Performs an additional lookup if a username is passed.",
     default=None,
     callback=user_lookup_callback,
 )
 @click.option(
     "--assignee",
-    help="User of the assignee of the case. Takes a user ID or a username.  Performs an additional lookup if a username is passed.",
+    help="User of the assignee of the case. Takes an actor ID or a username.  Performs an additional lookup if a username is passed.",
     default=None,
     callback=user_lookup_callback,
 )
 @click.option(
     "--findings", help="Markdown formatted details of case notes.", default=None
 )
 @logging_options
@@ -255,15 +255,15 @@
     Takes a single arg `FILE` which specifies the path to the file (use "-" to read from stdin).
 
     File format can either be CSV or [JSON Lines format](https://jsonlines.org) (Default is CSV).
 
     Valid CSV columns that correspond to update-able case fields include:
 
     * `number` (REQUIRED) - Case number.
-    * `assignee` - User ID or username of the administrator assigned to the case. Performs an additional lookup if a username is passed.
+    * `assignee` - actor ID or username of the administrator assigned to the case. Performs an additional lookup if a username is passed.
     * `description` - Brief optional description.
     * `findings` - Markdown formatted text summarizing the findings for a case.
     * `name` - Case name.
     * `status` - Case status. One of `ARCHIVED`, `CLOSED` or `OPEN`.
     * `subject` - User ID or username of the case subject. Performs an additional lookup if a username is passed.
     """
     client = Client()
```

### Comparing `incydr-1.2.0/_incydr_cli/cmds/departments.py` & `incydr-2.0.0/_incydr_cli/cmds/departments.py`

 * *Files identical despite different names*

### Comparing `incydr-1.2.0/_incydr_cli/cmds/devices.py` & `incydr-2.0.0/_incydr_cli/cmds/devices.py`

 * *Files identical despite different names*

### Comparing `incydr-1.2.0/_incydr_cli/cmds/directory_groups.py` & `incydr-2.0.0/_incydr_cli/cmds/directory_groups.py`

 * *Files identical despite different names*

### Comparing `incydr-1.2.0/_incydr_cli/cmds/file_events.py` & `incydr-2.0.0/_incydr_cli/cmds/file_events.py`

 * *Files identical despite different names*

### Comparing `incydr-1.2.0/_incydr_cli/cmds/models.py` & `incydr-2.0.0/_incydr_cli/cmds/models.py`

 * *Files identical despite different names*

### Comparing `incydr-1.2.0/_incydr_cli/cmds/trusted_activities.py` & `incydr-2.0.0/_incydr_cli/cmds/trusted_activities.py`

 * *Files identical despite different names*

### Comparing `incydr-1.2.0/_incydr_cli/cmds/user_risk_profiles.py` & `incydr-2.0.0/_incydr_cli/cmds/users.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from functools import lru_cache
 from pathlib import Path
 from typing import Optional
 
 import click
+from boltons.iterutils import bucketize
 from pydantic import Field
 from requests import HTTPError
 from rich.panel import Panel
 from rich.progress import track
 
 from _incydr_cli import console
 from _incydr_cli import logging_options
@@ -15,343 +16,530 @@
 from _incydr_cli.cmds.models import UserJSON
 from _incydr_cli.cmds.options.output_options import columns_option
 from _incydr_cli.cmds.options.output_options import input_format_option
 from _incydr_cli.cmds.options.output_options import single_format_option
 from _incydr_cli.cmds.options.output_options import SingleFormat
 from _incydr_cli.cmds.options.output_options import table_format_option
 from _incydr_cli.cmds.options.output_options import TableFormat
-from _incydr_cli.cmds.options.profile_filter_options import profile_filter_options
 from _incydr_cli.cmds.options.utils import user_lookup_callback
-from _incydr_cli.cmds.users import users
 from _incydr_cli.cmds.utils import user_lookup
-from _incydr_cli.core import incompatible_with
 from _incydr_cli.core import IncydrCommand
 from _incydr_cli.core import IncydrGroup
+from _incydr_cli.file_readers import AutoDecodedFile
 from _incydr_sdk.core.client import Client
-from _incydr_sdk.exceptions import DateParseError
-from _incydr_sdk.user_risk_profiles.models import UserRiskProfile
+from _incydr_sdk.devices.models import Device
+from _incydr_sdk.users.client import RoleNotFoundError
+from _incydr_sdk.users.client import RoleProcessingError
+from _incydr_sdk.users.client import UserNotAssignedRoleError
+from _incydr_sdk.users.models import Role
+from _incydr_sdk.users.models import User
+from _incydr_sdk.users.models import UserRole
 from _incydr_sdk.utils import model_as_card
 
+user_arg = click.argument("user", callback=user_lookup_callback)
 
-class UpdateCloudAliasesCSV(UserCSV):
-    cloud_alias: str = Field(csv_aliases=["cloudAlias", "cloud_alias", "alias"])
 
-
-class UpdateCloudAliasesJSON(UserJSON):
-    cloud_alias: str = Field(alias="cloudAlias")
-
-
-@users.group(cls=IncydrGroup)
+@click.group(cls=IncydrGroup)
 @logging_options
-def risk_profiles():
-    """View and manage user risk profiles."""
+def users():
+    """View and manage users and user roles."""
 
 
-@risk_profiles.command("list", cls=IncydrCommand)
+@users.command("list", cls=IncydrCommand)
+@click.option(
+    "--active/--inactive",
+    default=None,
+    help="Filter by active or inactive users. Defaults to returning both when when neither option is passed.",
+)
+@click.option(
+    "--blocked/--unblocked",
+    default=None,
+    help="Filter by blocked or unblocked users. Defaults to returning both when when neither option is passed.",
+)
+@click.option("--username", default=None)
 @table_format_option
 @columns_option
-@profile_filter_options
 @logging_options
 def list_(
+    active: Optional[bool],
+    blocked: Optional[bool],
+    username: Optional[str],
     format_: TableFormat,
     columns: Optional[str],
-    manager: Optional[str],
-    title: Optional[str],
-    division: Optional[str],
-    department: Optional[str],
-    employment_type: Optional[str],
-    country: Optional[str],
-    region: Optional[str],
-    locality: Optional[str],
-    active: Optional[bool],
-    deleted: Optional[bool],
-    support_user: Optional[bool],
 ):
     """
-    List user risk profiles.
+    List users.
     """
     client = Client()
-    profiles = client.user_risk_profiles.v1.iter_all(
-        manager_id=manager,
-        title=title,
-        division=division,
-        department=department,
-        employment_type=employment_type,
-        country=country,
-        region=region,
-        locality=locality,
-        active=active,
-        deleted=deleted,
-        support_user=support_user,
-    )
+    users_ = client.users.v1.iter_all(active=active, blocked=blocked, username=username)
 
     if format_ == TableFormat.csv:
-        render.csv(UserRiskProfile, profiles, columns=columns, flat=True)
+        render.csv(User, users_, columns=columns, flat=True)
     elif format_ == TableFormat.table:
         columns = columns or [
-            "username",
             "user_id",
-            "display_name",
-            "cloud_aliases",
+            "username",
+            "first_name",
+            "last_name",
+            "org_guid",
+            "org_name",
+            "notes",
             "active",
-            "start_date",
-            "end_date",
+            "blocked",
         ]
-        render.table(UserRiskProfile, profiles, columns=columns, flat=False)
+        render.table(User, users_, columns=columns, flat=False)
     else:
         printed = False
         if format_ == TableFormat.json_pretty:
-            for p in profiles:
+            for item in users_:
                 printed = True
-                console.print_json(p.json())
+                console.print_json(item.json())
         else:
-            for p in profiles:
+            for item in users_:
                 printed = True
-                click.echo(p.json())
+                click.echo(item.json())
         if not printed:
             console.print("No results found.")
 
 
-@risk_profiles.command(cls=IncydrCommand)
-@click.argument("user", callback=user_lookup_callback)
+@users.command(cls=IncydrCommand)
+@click.argument("user")  # don't need username callback, handled by client method
 @single_format_option
 @logging_options
 def show(
-    user: str,
+    user,
     format_: SingleFormat,
 ):
     """
-    Show details for a user risk profile.
+    Show details for a user.
 
-    Accepts a user ID or a username.  Performs an additional lookup if a username is passed.
+    Accepts a user ID or a username.  Performs an additional lookup if username is passed.
     """
     client = Client()
-    profile = client.user_risk_profiles.v1.get_user_risk_profile(user)
+    user = client.users.v1.get_user(user)
+
     if format_ == SingleFormat.rich and client.settings.use_rich:
-        console.print(
-            Panel.fit(model_as_card(profile), title=f"Risk Profile {profile.username}")
-        )
+        console.print(Panel.fit(model_as_card(user), title=f"User {user.username}"))
     elif format_ == SingleFormat.json_pretty:
-        console.print_json(profile.json())
+        console.print_json(user.json())
     else:
-        click.echo(profile.json())
+        click.echo(user.json())
 
 
-@risk_profiles.command(cls=IncydrCommand)
-@click.argument("user", callback=user_lookup_callback)
-@click.option(
-    "--start-date",
-    default=None,
-    help="Update a user's starting date. Accepts a date in yyyy-MM-dd (UTC) format.",
-)
-@click.option(
-    "--end-date",
-    default=None,
-    help="Update a user's departure date. Accepts a date in yyyy-MM-dd (UTC) format.",
-)
-@click.option(
-    "--notes", default=None, help="Update the optional notes on a user's profile."
-)
-@click.option(
-    "--clear-start-date",
-    is_flag=True,
-    default=False,
-    help="Clear the start date on a user's profile. Incompatible with --start-date.",
-    cls=incompatible_with("start_date"),
-)
-@click.option(
-    "--clear-end-date",
-    is_flag=True,
-    default=False,
-    help="Clear the end date on a user's profile. Incompatible with --end-date.",
-    cls=incompatible_with("end_date"),
-)
-@click.option(
-    "--clear-notes",
-    is_flag=True,
-    default=False,
-    help="Clear the notes on a user's profile. Incompatible with --notes.",
-    cls=incompatible_with("notes"),
-)
+@users.command(cls=IncydrCommand)
+@user_arg
+@table_format_option
+@columns_option
 @logging_options
-def update(
+def list_devices(
     user,
-    start_date=None,
-    end_date=None,
-    notes=None,
-    clear_start_date=None,
-    clear_end_date=None,
-    clear_notes=None,
-):
-    """
-    Update a user risk profile.
-
-    Accepts a user ID or a username.  Performs an additional lookup if a username is passed.
-    """
-    if not any(
-        [start_date, end_date, notes, clear_start_date, clear_end_date, clear_notes]
-    ):
-        raise click.UsageError(
-            "At least one of --start-date, --end-date, or --notes, or one of their corresponding clear flags, "
-            "is required to update a user risk profile."
-        )
+    format_: TableFormat,
+    columns: Optional[str],
+):
+    """
+    List devices associated with a particular user.
+    """
+    client = Client()
+    devices = client.users.v1.get_devices(user).devices
+
+    if format_ == TableFormat.csv:
+        render.csv(Device, devices, columns=columns, flat=True)
+    elif format_ == TableFormat.table:
+        columns = columns or [
+            "device_id",
+            "name",
+            "os_hostname",
+            "status",
+            "active",
+            "blocked",
+            "alert_state",
+            "org_guid",
+            "login_date",
+        ]
+        render.table(Device, devices, columns=columns, flat=False)
+    elif format_ == TableFormat.json_pretty:
+        for item in devices:
+            console.print_json(item.json())
+    else:
+        for item in devices:
+            click.echo(item.json())
 
+
+@users.command("list-roles", cls=IncydrCommand)
+@user_arg
+@table_format_option
+@columns_option
+@logging_options
+def list_user_roles(
+    user: str,
+    format_: TableFormat,
+    columns: Optional[str],
+):
+    """
+    List roles associated with a particular user.
+    """
+    client = Client()
+    roles = client.users.v1.list_user_roles(user)
+
+    if format_ == TableFormat.csv:
+        render.csv(UserRole, roles, columns=columns, flat=True)
+    elif format_ == TableFormat.table:
+        render.table(UserRole, roles, columns=columns, flat=False)
+    elif format_ == TableFormat.json_pretty:
+        for item in roles:
+            console.print_json(item.json())
+    else:
+        for item in roles:
+            click.echo(item.json())
+
+
+@users.command(cls=IncydrCommand)
+@user_arg
+@click.argument("roles")
+@click.option("--add", "update_method", flag_value="add", default=None)
+@click.option("--remove", "update_method", flag_value="remove", default=None)
+@logging_options
+def update_roles(
+    user,
+    roles: str,
+    update_method: str,
+):
+    """
+    Update roles associated with a particular user.
+
+    Usage:
+        users update-roles USER ROLES
+
+    USER is the user ID or username of the user whose roles will be updated.
+    Performs an additional lookup if username is passed.
+
+    ROLES is a comma-delimited list of role IDs and/or role names to replace that user's roles.
+
+    Use the `--remove` flag to remove the specified role(s) from a user's existing roles.
+
+    Alternatively, use the `--add` flag to assign additional roles to a user's existing roles.
+    """
     client = Client()
 
-    if clear_start_date:
-        start_date = ""
-    if clear_end_date:
-        end_date = ""
-    if clear_notes:
-        notes = ""
+    if update_method == "add":
+        update_func = client.users.v1.add_roles
+    elif update_method == "remove":
+        update_func = client.users.v1.remove_roles
+    else:
+        update_func = client.users.v1.update_roles
 
     try:
-        updated_profile = client.user_risk_profiles.v1.update(
-            user, notes, start_date, end_date
-        )
-        if client.settings.use_rich:
-            console.print(
-                Panel.fit(
-                    model_as_card(updated_profile), title="Updated User Risk Profile"
-                )
-            )
-        else:
-            console.print(updated_profile.json(), highlight=False)
-    except DateParseError as err:
-        raise err
+        update_func(user, [r.strip() for r in roles.split(",")])
+    except RoleNotFoundError as e:
+        raise e
+    except UserNotAssignedRoleError as e:
+        raise e
+    console.print(f"Roles successfully updated for user '{user}'")
 
 
-@risk_profiles.command(cls=IncydrCommand)
-@click.argument("user", callback=user_lookup_callback)
-@click.argument("cloud-alias")
+@users.command(cls=IncydrCommand)
+@user_arg
 @logging_options
-def add_cloud_alias(
-    user: str,
-    cloud_alias: str,
+def activate(
+    user,
 ):
     """
-    Add a cloud alias to a user risk profile.
+    Activate a user.
+    """
+    client = Client()
+    client.users.v1.activate(user)
+    console.print(f"User '{user}' successfully activated.")
 
-    Accepts a user ID or a username.  Performs an additional lookup if a username is passed.
 
-    A cloud alias is the username an employee uses to access cloud services such as Google Drive or Box.
-    Adding a cloud alias allows Incydr to link a user's cloud activity with their Code42 username.
-    Each user has a default cloud alias of their Code42 username. You can add one additional alias.
+@users.command(cls=IncydrCommand)
+@user_arg
+@logging_options
+def deactivate(
+    user,
+):
+    """
+    Deactivate a user.
     """
     client = Client()
-    client.user_risk_profiles.v1.add_cloud_alias(user, cloud_alias)
-    console.print(f"Cloud alias successfully added to user '{user}")
+    client.users.v1.deactivate(user)
+    console.print(f"User '{user}' successfully deactivated.")
 
 
-@risk_profiles.command(cls=IncydrCommand)
-@click.argument("user", callback=user_lookup_callback)
-@click.argument("cloud-alias")
+@users.command(cls=IncydrCommand)
+@user_arg
+@click.argument("org_guid")
 @logging_options
-def remove_cloud_alias(
-    user: str,
-    cloud_alias: str,
+def move(
+    user,
+    org_guid,
+):
+    """
+    Move a user to a specified organization.
+    """
+    client = Client()
+    client.users.v1.move(user, org_guid)
+    console.print(f"User '{user}' successfully moved to org '{org_guid}'.")
+
+
+@users.group("roles", cls=IncydrGroup)
+def roles_():
+    """View available roles."""
+
+
+@roles_.command("show", cls=IncydrCommand)
+@single_format_option
+@click.argument("role")
+@logging_options
+def show_role(
+    role,
+    format_: SingleFormat,
 ):
     """
-    Remove a cloud alias from a user risk profile.
+    Show details for a single role, specified by role name or role ID.
+    """
+    client = Client()
+    role = client.users.v1.get_role(role)
+    if format_ == SingleFormat.rich and client.settings.use_rich:
+        console.print(Panel.fit(model_as_card(role), title=role.role_name))
+    elif format_ == SingleFormat.json_pretty:
+        console.print_json(role.json())
+    else:
+        click.echo(role.json())
+
 
-    Accepts a user ID or a username.  Performs an additional lookup if a username is passed.
+@roles_.command("list", cls=IncydrCommand)
+@table_format_option
+@logging_options
+def list_roles(
+    format_: TableFormat,
+):
+    """
+    List all available roles that can be assigned by the current user.
     """
     client = Client()
-    client.user_risk_profiles.v1.delete_cloud_alias(user, cloud_alias)
-    console.print(f"Cloud alias successfully removed from user '{user}")
+    roles = client.users.v1.list_roles()
+    if format_ == TableFormat.csv:
+        render.csv(Role, roles, flat=True)
+    elif format_ == TableFormat.table:
+        render.table(Role, roles, flat=False)
+    elif format_ == TableFormat.json_pretty:
+        for item in roles:
+            console.print_json(item.json())
+    else:
+        for item in roles:
+            click.echo(item.json())
 
 
-@risk_profiles.command(cls=IncydrCommand)
-@click.argument("file", type=click.File())
+@users.command(cls=IncydrCommand)
+@click.argument("file", type=AutoDecodedFile())
 @input_format_option
+@click.option("--add", "update_method", flag_value="add", default=None)
+@click.option("--remove", "update_method", flag_value="remove", default=None)
 @logging_options
-def bulk_add_cloud_aliases(file: Path, format_: str):
+def bulk_update_roles(
+    file,
+    update_method: str,
+    format_: Optional[str],
+):
+    """
+    Bulk update roles associated with multiple users from a file.
+
+    By default, the provided roles will replace the specified user's existing roles.
+    Use the `--add` flag or the `--remove` flag to add or remove roles, respectively, from a user's existing roles.
+
+    Takes a single arg `FILE` which specifies the path to the file (use "-" to read from stdin).
+
+    File format can either be CSV or [JSON Lines format](https://jsonlines.org) (Default is CSV).
+
+    Requires the following CSV columns or JSON keys:
+
+    * `user` - User ID or username of the user whose roles will be updated. Performs an additional lookup if username is passed.
+    * `role` - Role ID and/or role name (case-sensitive) to assign to the new user.
+
+    Example:
+
+        The following command will add roles to users as specified in a JSON-lines formatted file:
+
+            incydr users bulk-update-roles path/to/file.json --add --format json-lines
+    """
+    client = Client()
+
+    @lru_cache()
+    def resolve_username(user):
+        if user is None:
+            return
+        elif "@" in user:
+            return user_lookup(client, user)
+        else:  # assume user_id
+            return user
+
+    class RoleUpdateCSV(UserCSV):
+        role: str = Field(
+            csv_aliases=["role", "role_id", "role_name", "roleId", "roleName"]
+        )
+
+    class RoleUpdateJSON(UserJSON):
+        role: str = Field(alias="roleId")
+
+    if format_ == "csv":
+        roles_file = RoleUpdateCSV.parse_csv(file)
+    else:
+        roles_file = RoleUpdateJSON.parse_json_lines(file)
+
+    if update_method == "add":
+        update_func = client.users.v1.add_roles
+    elif update_method == "remove":
+        update_func = client.users.v1.remove_roles
+    else:
+        update_func = client.users.v1.update_roles
+
+    # group updates by user
+    buckets = bucketize(
+        roles_file,
+        key=lambda role_update: role_update.user,
+        value_transform=lambda role_update: role_update.role,
+    )
+    for bucket in buckets:
+        user = bucket
+        roles = buckets[bucket]
+        try:
+            user = resolve_username(user)
+            update_func(user, roles)
+            console.print(f"Successfully updated roles for user {user}.'")
+        except RoleProcessingError as err:
+            console.print(
+                f"[red]Error! {str(err)} [/red]",
+                highlight=False,
+            )
+
 
+@users.command(cls=IncydrCommand)
+@click.argument("file", type=click.File())
+@input_format_option
+@logging_options
+def bulk_activate(file: Path, format_: str):
     """
-    Bulk add cloud aliases to user risk profiles.
+    Bulk activate users.
 
     Takes a single arg `FILE` which specifies the path to the file (use "-" to read from stdin).
 
     File format can either be CSV or [JSON Lines format](https://jsonlines.org) (Default is CSV).
 
-    Required CSV columns:
+    Requires a single `user` column or field that contains either the user IDs or the usernames of the users to be activated.
+    """
+    client = Client()
+
+    @lru_cache()
+    def resolve_username(user):
+        if user is None:
+            return
+        elif "@" in user:
+            return user_lookup(client, user)
+        else:  # assume user_id
+            return user
+
+    if format_ == "csv":
+        models = UserCSV.parse_csv(file)
+    else:
+        models = UserJSON.parse_json_lines(file)
+
+    try:
+        for row in track(
+            models,
+            description="Activating users...",
+            transient=True,
+        ):
+            client.users.v1.activate(resolve_username(row.user))
+    except HTTPError as err:
+        console.print(f"[red]Error:[/red] {err.response.text}")
+
+
+@users.command(cls=IncydrCommand)
+@click.argument("file", type=click.File())
+@input_format_option
+@logging_options
+def bulk_deactivate(file: Path, format_: str):
+    """
+    Bulk deactivate users.
+
+    Takes a single arg `FILE` which specifies the path to the file (use "-" to read from stdin).
+
+    File format can either be CSV or [JSON Lines format](https://jsonlines.org) (Default is CSV).
 
-     * `user` - User ID or username of the user risk profile. Performs an additional lookup if username is passed.
-     * `cloud_alias` - The cloud alias to remove from the profile.
+    Requires a single `user` column or field that contains either the user IDs or the usernames of the users to be deactivated.
     """
     client = Client()
 
     @lru_cache()
     def resolve_username(user):
         if user is None:
             return
         elif "@" in user:
             return user_lookup(client, user)
         else:  # assume user_id
             return user
 
     if format_ == "csv":
-        models = UpdateCloudAliasesCSV.parse_csv(file)
+        models = UserCSV.parse_csv(file)
     else:
-        models = UpdateCloudAliasesJSON.parse_json_lines(file)
+        models = UserJSON.parse_json_lines(file)
 
     try:
         for row in track(
             models,
-            description="Adding cloud aliases...",
+            description="Deactivating users...",
             transient=True,
         ):
-            client.user_risk_profiles.v1.add_cloud_alias(
-                resolve_username(row.user), row.cloud_alias
-            )
-    except ValueError as err:
-        console.print(f"[red]Error:[/red] {err}")
+            client.users.v1.deactivate(resolve_username(row.user))
     except HTTPError as err:
         console.print(f"[red]Error:[/red] {err.response.text}")
 
 
-@risk_profiles.command(cls=IncydrCommand)
+@users.command(cls=IncydrCommand)
 @click.argument("file", type=click.File())
 @input_format_option
 @logging_options
-def bulk_remove_cloud_aliases(file: Path, format_: str):
+def bulk_move(file: Path, format_: str):
+
     """
-    Bulk remove cloud aliases from user risk profiles.
+    Bulk move multiple users to specified organizations.
 
     Takes a single arg `FILE` which specifies the path to the file (use "-" to read from stdin).
 
     File format can either be CSV or [JSON Lines format](https://jsonlines.org) (Default is CSV).
 
-    Required CSV columns:
+    Requires the following columns:
 
-     * `user` - User ID or username of the user risk profile. Performs an additional lookup if username is passed.
-     * `cloud_alias` - The cloud alias to remove from the profile.
+    * `user` - User ID or username of the user who will be moved to the new organization. Performs an additional lookup if username is passed.
+    * `org_guid` - GUID for the user's new organization.
     """
     client = Client()
 
+    class UserMoveCSV(UserCSV):
+        org_guid: str = Field(csv_aliases=["org_guid", "orgGuid", "org"])
+
+    class UserMoveJSON(UserJSON):
+        org_guid: str = Field(alias="orgGuid")
+
     @lru_cache()
     def resolve_username(user):
         if user is None:
             return
         elif "@" in user:
             return user_lookup(client, user)
         else:  # assume user_id
             return user
 
     if format_ == "csv":
-        models = UpdateCloudAliasesCSV.parse_csv(file)
+        models = UserMoveCSV.parse_csv(file)
     else:
-        models = UpdateCloudAliasesJSON.parse_json_lines(file)
+        models = UserMoveJSON.parse_json_lines(file)
 
     try:
         for row in track(
             models,
-            description="Removing cloud aliases...",
+            description="Moving users...",
             transient=True,
         ):
-            client.user_risk_profiles.v1.delete_cloud_alias(
-                resolve_username(row.user), row.cloud_alias
-            )
-    except ValueError as err:
-        console.print(f"[red]Error:[/red] {err}")
+            client.users.v1.move(resolve_username(row.user), row.org_guid)
     except HTTPError as err:
         console.print(f"[red]Error:[/red] {err.response.text}")
```

### Comparing `incydr-1.2.0/_incydr_cli/cmds/users.py` & `incydr-2.0.0/_incydr_cli/cmds/sessions.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,545 +1,417 @@
-from functools import lru_cache
+import json
+from contextlib import nullcontext
 from pathlib import Path
+from typing import List
 from typing import Optional
 
 import click
-from boltons.iterutils import bucketize
 from pydantic import Field
 from requests import HTTPError
 from rich.panel import Panel
 from rich.progress import track
 
 from _incydr_cli import console
+from _incydr_cli import get_user_project_path
 from _incydr_cli import logging_options
 from _incydr_cli import render
-from _incydr_cli.cmds.models import UserCSV
-from _incydr_cli.cmds.models import UserJSON
 from _incydr_cli.cmds.options.output_options import columns_option
 from _incydr_cli.cmds.options.output_options import input_format_option
+from _incydr_cli.cmds.options.output_options import output_options
 from _incydr_cli.cmds.options.output_options import single_format_option
 from _incydr_cli.cmds.options.output_options import SingleFormat
 from _incydr_cli.cmds.options.output_options import table_format_option
 from _incydr_cli.cmds.options.output_options import TableFormat
-from _incydr_cli.cmds.options.utils import user_lookup_callback
-from _incydr_cli.cmds.utils import user_lookup
+from _incydr_cli.cmds.options.utils import checkpoint_option
+from _incydr_cli.cmds.utils import warn_interrupt
 from _incydr_cli.core import IncydrCommand
 from _incydr_cli.core import IncydrGroup
-from _incydr_cli.file_readers import AutoDecodedFile
+from _incydr_cli.cursor import CursorStore
+from _incydr_cli.logger import get_server_logger
 from _incydr_sdk.core.client import Client
-from _incydr_sdk.devices.models import Device
-from _incydr_sdk.users.client import RoleNotFoundError
-from _incydr_sdk.users.client import RoleProcessingError
-from _incydr_sdk.users.client import UserNotAssignedRoleError
-from _incydr_sdk.users.models import Role
-from _incydr_sdk.users.models import User
-from _incydr_sdk.users.models import UserRole
+from _incydr_sdk.core.models import CSVModel
+from _incydr_sdk.core.models import Model
+from _incydr_sdk.enums.sessions import ContentInspectionStatuses
+from _incydr_sdk.enums.sessions import SessionSeverities
+from _incydr_sdk.enums.sessions import SessionStates
+from _incydr_sdk.file_events.models.event import FileEventV2
+from _incydr_sdk.file_events.models.response import FileEventsPage
+from _incydr_sdk.sessions.models.response import Session
 from _incydr_sdk.utils import model_as_card
 
-user_arg = click.argument("user", callback=user_lookup_callback)
+SEVERITY_MAP = {"NO_RISK": 0, "LOW": 1, "MODERATE": 2, "HIGH": 3, "CRITICAL": 4}
 
 
 @click.group(cls=IncydrGroup)
 @logging_options
-def users():
-    """View and manage users and user roles."""
+def sessions():
+    """
+    View and manage Incydr Sessions, including Alerts.
+
+    Sessions group all Incydr activity for an individual actor within a specific time frame.
+    Sessions may include file events, alerts, Instructor lessons, and more. A single session can contain one or more alerts.
+
+    Alerts are triggered when user file activity matches criteria defined in your alert rules.
+    Alerts are included within sessions to group related activity and provide additional context.
+    """
 
 
-@users.command("list", cls=IncydrCommand)
+@sessions.command(cls=IncydrCommand)
+@checkpoint_option
 @click.option(
-    "--active/--inactive",
+    "--actor-id", default=None, help="Limit search to sessions generated by this actor."
+)
+@click.option(
+    "--start",
     default=None,
-    help="Filter by active or inactive users. Defaults to returning both when when neither option is passed.",
+    help="Limit search to sessions beginning on or after this date and time. "
+    "Accepts a date/time in yyyy-MM-dd (UTC) or yyyy-MM-dd HH:MM:SS (UTC+24-hr time) format.",
 )
 @click.option(
-    "--blocked/--unblocked",
+    "--end",
     default=None,
-    help="Filter by blocked or unblocked users. Defaults to returning both when when neither option is passed.",
+    help="Limit search to sessions beginning before this date and time. "
+    "Accepts a date/time in yyyy-MM-dd (UTC) or yyyy-MM-dd HH:MM:SS (UTC+24-hr time) format.",
+)
+@click.option(
+    "--no-alerts",
+    is_flag=True,
+    default=False,
+    help="Limit search to sessions that do NOT have alerts associated with them.",
+)
+@click.option(
+    "--risk-indicators",
+    default=None,
+    help="A CSV list of risk indicator IDs. Limit search to sessions that include these risk indicators.",
+)
+@click.option(
+    "--state",
+    type=click.Choice([e.value for e in SessionStates]),
+    default=[],
+    multiple=True,
+    help="Limit search to sessions with this state. Can be specified multiple times to include multiple values. ",
+)
+@click.option(
+    "--severity",
+    type=click.Choice([e.value for e in SessionSeverities]),
+    default=[],
+    multiple=True,
+    help="Specify one or more severity levels, can be specified multiple times to include multiple values. "
+    "Limit search to sessions that have the matching severity value(s). ",
+)
+@click.option(
+    "--rule-id",
+    default=[],
+    multiple=True,
+    help="A rule ID. Limit search to sessions associated with this rule. Can be specified multiple times to include multiple values. ",
+)
+@click.option(
+    "--watchlist-id",
+    default=[],
+    multiple=True,
+    help="A watchlist ID. Limit search to sessions associated with this watchlist. Can be specified multiple times to include multiple values. ",
+)
+@click.option(
+    "--content-inspection-status",
+    type=click.Choice([e.value for e in ContentInspectionStatuses]),
+    default=None,
+    help="Limit search to sessions with the given content inspection status.",
 )
-@click.option("--username", default=None)
 @table_format_option
 @columns_option
 @logging_options
-def list_(
-    active: Optional[bool],
-    blocked: Optional[bool],
-    username: Optional[str],
-    format_: TableFormat,
-    columns: Optional[str],
-):
-    """
-    List users.
-    """
-    client = Client()
-    users_ = client.users.v1.iter_all(active=active, blocked=blocked, username=username)
+def search(
+    actor_id: Optional[str] = None,
+    start: Optional[str] = None,
+    end: Optional[str] = None,
+    no_alerts: bool = False,
+    risk_indicators: Optional[str] = None,
+    state: Optional[List[str]] = None,
+    severity: Optional[List[str]] = None,
+    rule_id: Optional[List[str]] = None,
+    watchlist_id: Optional[List[str]] = None,
+    content_inspection_status: Optional[str] = None,
+    output: Optional[str] = None,
+    certs: Optional[str] = None,
+    ignore_cert_validation: Optional[bool] = None,
+    checkpoint_name: Optional[str] = None,
+    format_: Optional[TableFormat] = None,
+    columns: Optional[str] = None,
+):
+    """
+    Search sessions.
+
+    Defaults to only include sessions that have alerts associated with them.
+    Use the --no-alerts option to view sessions without any alerts.
+    """
+    client = Client()
+    cursor = _get_cursor_store(client.settings.api_client_id)
+
+    if output:
+        format_ = TableFormat.json_lines
+
+    # Use stored checkpoint timestamp for start filter if applicable
+    if checkpoint_name:
+        checkpoint = cursor.get(checkpoint_name)
+        if checkpoint:
+            start = int(checkpoint)
+
+    severity_values = []
+    for value in severity:
+        severity_values.append(SEVERITY_MAP[value])
+
+    sessions_gen = client.sessions.v1.iter_all(
+        actor_id=actor_id,
+        start_time=start,
+        end_time=end,
+        has_alerts=not no_alerts,
+        risk_indicators=risk_indicators.split(",") if risk_indicators else None,
+        states=[*state] if state else None,
+        severities=severity_values,
+        rule_ids=[*rule_id] if rule_id else None,
+        watchlist_ids=[*watchlist_id] if watchlist_id else None,
+        content_inspection_status=content_inspection_status,
+    )
+    if checkpoint_name:
+        sessions_gen = _update_checkpoint(cursor, checkpoint_name, sessions_gen)
 
-    if format_ == TableFormat.csv:
-        render.csv(User, users_, columns=columns, flat=True)
-    elif format_ == TableFormat.table:
-        columns = columns or [
-            "user_id",
-            "username",
-            "first_name",
-            "last_name",
-            "org_guid",
-            "org_name",
-            "notes",
-            "active",
-            "blocked",
-        ]
-        render.table(User, users_, columns=columns, flat=False)
-    else:
-        printed = False
-        if format_ == TableFormat.json_pretty:
-            for item in users_:
-                printed = True
-                console.print_json(item.json())
+    with warn_interrupt() if checkpoint_name else nullcontext():
+        if output:
+            logger = get_server_logger(output, certs, ignore_cert_validation)
+            for session in sessions_gen:
+                logger.info(session.json())
+            return
+
+        if format_ == TableFormat.table:
+            columns = columns or [
+                "session_id",
+                "begin_time",
+                "end_time",
+                "context_summary",
+                "exfiltration_summary",
+                "actor_id",
+                "low_events",
+                "moderate_events",
+                "high_events",
+                "states",
+                "notes",
+            ]
+            render.table(Session, sessions_gen, columns=columns, flat=False)
+        elif format_ == TableFormat.csv:
+            render.csv(Session, sessions_gen, columns=columns, flat=True)
         else:
-            for item in users_:
+            printed = False
+            for session in sessions_gen:
                 printed = True
-                click.echo(item.json())
-        if not printed:
-            console.print("No results found.")
+                if format_ == TableFormat.json_pretty:
+                    console.print_json(session.json())
+                else:
+                    click.echo(session.json())
+            if not printed:
+                console.print("No results found.")
 
 
-@users.command(cls=IncydrCommand)
-@click.argument("user")  # don't need username callback, handled by client method
-@single_format_option
+@sessions.command(cls=IncydrCommand)
+@click.argument("session-id")
 @logging_options
-def show(
-    user,
-    format_: SingleFormat,
-):
+@single_format_option
+def show(session_id: str, format_: SingleFormat):
     """
-    Show details for a user.
-
-    Accepts a user ID or a username.  Performs an additional lookup if username is passed.
+    Show the details of a single session.
     """
     client = Client()
-    user = client.users.v1.get_user(user)
+    session = client.sessions.v1.get_session_details(session_id)
 
-    if format_ == SingleFormat.rich and client.settings.use_rich:
-        console.print(Panel.fit(model_as_card(user), title=f"User {user.username}"))
+    if format_ == SingleFormat.rich:
+        console.print(Panel.fit(model_as_card(session)))
     elif format_ == SingleFormat.json_pretty:
-        console.print_json(user.json())
+        console.print_json(session.json())
     else:
-        click.echo(user.json())
+        click.echo(session.json())
 
 
-@users.command(cls=IncydrCommand)
-@user_arg
-@table_format_option
-@columns_option
+@sessions.command(cls=IncydrCommand)
 @logging_options
-def list_devices(
-    user,
-    format_: TableFormat,
+@columns_option
+@table_format_option
+@output_options
+@click.argument("session-id")
+def show_events(
+    session_id: str,
     columns: Optional[str],
+    output: Optional[str],
+    certs: Optional[str],
+    ignore_cert_validation: Optional[bool],
+    format_: SingleFormat,
 ):
     """
-    List devices associated with a particular user.
+    Show the details of a single session.
     """
     client = Client()
-    devices = client.users.v1.get_devices(user).devices
+    page = client.sessions.v1.get_session_events(session_id)
 
-    if format_ == TableFormat.csv:
-        render.csv(Device, devices, columns=columns, flat=True)
-    elif format_ == TableFormat.table:
-        columns = columns or [
-            "device_id",
-            "name",
-            "os_hostname",
-            "status",
-            "active",
-            "blocked",
-            "alert_state",
-            "org_guid",
-            "login_date",
-        ]
-        render.table(Device, devices, columns=columns, flat=False)
-    elif format_ == TableFormat.json_pretty:
-        for item in devices:
-            console.print_json(item.json())
-    else:
-        for item in devices:
-            click.echo(item.json())
+    def event_iterator(event_page: FileEventsPage):
+        yield from event_page.file_events
 
+    events = event_iterator(page)
 
-@users.command("list-roles", cls=IncydrCommand)
-@user_arg
-@table_format_option
-@columns_option
-@logging_options
-def list_user_roles(
-    user: str,
-    format_: TableFormat,
-    columns: Optional[str],
-):
-    """
-    List roles associated with a particular user.
-    """
-    client = Client()
-    roles = client.users.v1.list_user_roles(user)
+    if output:
+        logger = get_server_logger(output, certs, ignore_cert_validation)
+        for event_ in events:
+            logger.info(event_.json())
+        return
 
     if format_ == TableFormat.csv:
-        render.csv(UserRole, roles, columns=columns, flat=True)
+        render.csv(FileEventV2, events, columns=columns, flat=True)
     elif format_ == TableFormat.table:
-        render.table(UserRole, roles, columns=columns, flat=False)
-    elif format_ == TableFormat.json_pretty:
-        for item in roles:
-            console.print_json(item.json())
-    else:
-        for item in roles:
-            click.echo(item.json())
-
-
-@users.command(cls=IncydrCommand)
-@user_arg
-@click.argument("roles")
-@click.option("--add", "update_method", flag_value="add", default=None)
-@click.option("--remove", "update_method", flag_value="remove", default=None)
-@logging_options
-def update_roles(
-    user,
-    roles: str,
-    update_method: str,
-):
-    """
-    Update roles associated with a particular user.
-
-    Usage:
-        users update-roles USER ROLES
-
-    USER is the user ID or username of the user whose roles will be updated.
-    Performs an additional lookup if username is passed.
-
-    ROLES is a comma-delimited list of role IDs and/or role names to replace that user's roles.
-
-    Use the `--remove` flag to remove the specified role(s) from a user's existing roles.
-
-    Alternatively, use the `--add` flag to assign additional roles to a user's existing roles.
-    """
-    client = Client()
-
-    if update_method == "add":
-        update_func = client.users.v1.add_roles
-    elif update_method == "remove":
-        update_func = client.users.v1.remove_roles
-    else:
-        update_func = client.users.v1.update_roles
-
-    try:
-        update_func(user, [r.strip() for r in roles.split(",")])
-    except RoleNotFoundError as e:
-        raise e
-    except UserNotAssignedRoleError as e:
-        raise e
-    console.print(f"Roles successfully updated for user '{user}'")
-
-
-@users.command(cls=IncydrCommand)
-@user_arg
-@logging_options
-def activate(
-    user,
-):
-    """
-    Activate a user.
-    """
-    client = Client()
-    client.users.v1.activate(user)
-    console.print(f"User '{user}' successfully activated.")
-
-
-@users.command(cls=IncydrCommand)
-@user_arg
-@logging_options
-def deactivate(
-    user,
-):
-    """
-    Deactivate a user.
-    """
-    client = Client()
-    client.users.v1.deactivate(user)
-    console.print(f"User '{user}' successfully deactivated.")
-
-
-@users.command(cls=IncydrCommand)
-@user_arg
-@click.argument("org_guid")
-@logging_options
-def move(
-    user,
-    org_guid,
-):
-    """
-    Move a user to a specified organization.
-    """
-    client = Client()
-    client.users.v1.move(user, org_guid)
-    console.print(f"User '{user}' successfully moved to org '{org_guid}'.")
-
-
-@users.group("roles", cls=IncydrGroup)
-def roles_():
-    """View available roles."""
-
-
-@roles_.command("show", cls=IncydrCommand)
-@single_format_option
-@click.argument("role")
-@logging_options
-def show_role(
-    role,
-    format_: SingleFormat,
-):
-    """
-    Show details for a single role, specified by role name or role ID.
-    """
-    client = Client()
-    role = client.users.v1.get_role(role)
-    if format_ == SingleFormat.rich and client.settings.use_rich:
-        console.print(Panel.fit(model_as_card(role), title=role.role_name))
-    elif format_ == SingleFormat.json_pretty:
-        console.print_json(role.json())
+        render.table(FileEventV2, events, columns=columns, flat=False)
     else:
-        click.echo(role.json())
+        printed = False
+        for event in events:
+            printed = True
+            if format_ == TableFormat.json_pretty:
+                console.print_json(data=event)
+            else:
+                click.echo(json.dumps(event))
+        if not printed:
+            console.print("No results found.")
 
 
-@roles_.command("list", cls=IncydrCommand)
-@table_format_option
+@sessions.command(cls=IncydrCommand)
+@click.argument("session-id")
+@click.option(
+    "--state",
+    "-s",
+    type=click.Choice([e.value for e in SessionStates]),
+    help="Update a session's state.",
+)
+@click.option(
+    "--note",
+    help="Add a note to the session. Takes the notes content with a 2000 character max.",
+)
 @logging_options
-def list_roles(
-    format_: TableFormat,
-):
+def update(session_id: str, state: str = None, note: str = None):
     """
-    List all available roles that can be assigned by the current user.
+    Update the state of and/or the note attached to the session.
     """
     client = Client()
-    roles = client.users.v1.list_roles()
-    if format_ == TableFormat.csv:
-        render.csv(Role, roles, flat=True)
-    elif format_ == TableFormat.table:
-        render.table(Role, roles, flat=False)
-    elif format_ == TableFormat.json_pretty:
-        for item in roles:
-            console.print_json(item.json())
-    else:
-        for item in roles:
-            click.echo(item.json())
+    if state:
+        client.sessions.v1.update_state_by_id(session_id, state)
+        console.print(f"Successfully updated session {session_id} to {state}!")
+    if note:
+        client.sessions.v1.add_note(session_id, note)
+        console.print(f"Successfully added note to session {session_id}!")
 
 
-@users.command(cls=IncydrCommand)
-@click.argument("file", type=AutoDecodedFile())
+@sessions.command(cls=IncydrCommand)
+@click.argument("file", type=click.File())
+@click.option(
+    "--state",
+    type=click.Choice([e.value for e in SessionStates]),
+    help="Override CSV/JSON input's `state` value with this value.",
+)
+@click.option("--note", help="Override CSV/JSON input's `note` value with this value.")
 @input_format_option
-@click.option("--add", "update_method", flag_value="add", default=None)
-@click.option("--remove", "update_method", flag_value="remove", default=None)
 @logging_options
-def bulk_update_roles(
-    file,
-    update_method: str,
-    format_: Optional[str],
+def bulk_update_state(
+    file: Path,
+    state: Optional[str] = None,
+    note: Optional[str] = None,
+    format_: str = None,
 ):
     """
-    Bulk update roles associated with multiple users from a file.
+    Bulk update the state of multiple sessions. Optionally attach a note.
 
-    By default, the provided roles will replace the specified user's existing roles.
-    Use the `--add` flag or the `--remove` flag to add or remove roles, respectively, from a user's existing roles.
+    NEW_STATE specifies the new state to which sessions will be updated.
+    Must be one of the following: 'OPEN', 'IN_PROGRESS', 'CLOSED', 'CLOSED_TP', 'CLOSED_FP', 'OPEN_NEW_DATA'
 
     Takes a single arg `FILE` which specifies the path to the file (use "-" to read from stdin).
-
     File format can either be CSV or [JSON Lines format](https://jsonlines.org) (Default is CSV).
 
-    Requires the following CSV columns or JSON keys:
-
-    * `user` - User ID or username of the user whose roles will be updated. Performs an additional lookup if username is passed.
-    * `role` - Role ID and/or role name (case-sensitive) to assign to the new user.
-
-    Example:
-
-        The following command will add roles to users as specified in a JSON-lines formatted file:
-
-            incydr users bulk-update-roles path/to/file.json --add --format json-lines
-    """
-    client = Client()
-
-    @lru_cache()
-    def resolve_username(user):
-        if user is None:
-            return
-        elif "@" in user:
-            return user_lookup(client, user)
-        else:  # assume user_id
-            return user
-
-    class RoleUpdateCSV(UserCSV):
-        role: str = Field(
-            csv_aliases=["role", "role_id", "role_name", "roleId", "roleName"]
-        )
-
-    class RoleUpdateJSON(UserJSON):
-        role: str = Field(alias="roleId")
-
-    if format_ == "csv":
-        roles_file = RoleUpdateCSV.parse_csv(file)
-    else:
-        roles_file = RoleUpdateJSON.parse_json_lines(file)
+    The --state and --note options to this command will override respective columns/keys in the CSV/JSON input.
 
-    if update_method == "add":
-        update_func = client.users.v1.add_roles
-    elif update_method == "remove":
-        update_func = client.users.v1.remove_roles
-    else:
-        update_func = client.users.v1.update_roles
+    Accepts the following columns:
 
-    # group updates by user
-    buckets = bucketize(
-        roles_file,
-        key=lambda role_update: role_update.user,
-        value_transform=lambda role_update: role_update.role,
-    )
-    for bucket in buckets:
-        user = bucket
-        roles = buckets[bucket]
-        try:
-            user = resolve_username(user)
-            update_func(user, roles)
-            console.print(f"Successfully updated roles for user {user}.'")
-        except RoleProcessingError as err:
-            console.print(
-                f"[red]Error! {str(err)} [/red]",
-                highlight=False,
-            )
+    * `session_id` (required)
+    * `state` (required if --state option is not provided)
+    * `note` (optional)
 
+    If --state is not provided, the CSV/JSON input _must_ have a `state` column/key for each row/object.
 
-@users.command(cls=IncydrCommand)
-@click.argument("file", type=click.File())
-@input_format_option
-@logging_options
-def bulk_activate(file: Path, format_: str):
     """
-    Bulk activate users.
+    # if --state is provided, we want that column/key to be optional on input data, otherwise required
+    state_type = Optional[str] if state else str
 
-    Takes a single arg `FILE` which specifies the path to the file (use "-" to read from stdin).
+    # Validate input models
 
-    File format can either be CSV or [JSON Lines format](https://jsonlines.org) (Default is CSV).
+    class SessionCSV(CSVModel):
+        session_id: str = Field(csv_aliases=["session_id", "sessionId"])
+        state: state_type = Field(csv_aliases=["state"])
+        note: Optional[str]
 
-    Requires a single `user` column or field that contains either the user IDs or the usernames of the users to be activated.
-    """
-    client = Client()
-
-    @lru_cache()
-    def resolve_username(user):
-        if user is None:
-            return
-        elif "@" in user:
-            return user_lookup(client, user)
-        else:  # assume user_id
-            return user
+    class SessionJSON(Model):
+        session_id: str = Field(alias="sessionId")
+        state: state_type
+        note: Optional[str]
 
     if format_ == "csv":
-        models = UserCSV.parse_csv(file)
+        models = SessionCSV.parse_csv(file)
     else:
-        models = UserJSON.parse_json_lines(file)
-
-    try:
-        for row in track(
-            models,
-            description="Activating users...",
-            transient=True,
-        ):
-            client.users.v1.activate(resolve_username(row.user))
-    except HTTPError as err:
-        console.print(f"[red]Error:[/red] {err.response.text}")
-
-
-@users.command(cls=IncydrCommand)
-@click.argument("file", type=click.File())
-@input_format_option
-@logging_options
-def bulk_deactivate(file: Path, format_: str):
-    """
-    Bulk deactivate users.
+        models = SessionJSON.parse_json_lines(file)
 
-    Takes a single arg `FILE` which specifies the path to the file (use "-" to read from stdin).
-
-    File format can either be CSV or [JSON Lines format](https://jsonlines.org) (Default is CSV).
+    # Process input
 
-    Requires a single `user` column or field that contains either the user IDs or the usernames of the users to be deactivated.
-    """
     client = Client()
 
-    @lru_cache()
-    def resolve_username(user):
-        if user is None:
-            return
-        elif "@" in user:
-            return user_lookup(client, user)
-        else:  # assume user_id
-            return user
-
-    if format_ == "csv":
-        models = UserCSV.parse_csv(file)
-    else:
-        models = UserJSON.parse_json_lines(file)
+    # optimization: bucketize update state calls in batches of 100
 
     try:
         for row in track(
             models,
-            description="Deactivating users...",
+            description="Updating sessions...",
             transient=True,
         ):
-            client.users.v1.deactivate(resolve_username(row.user))
+            client.sessions.v1.update_state_by_id(row.session_id, state or row.state)
+            if note or row.note:
+                client.sessions.v1.add_note(row.session_id, note or row.note)
     except HTTPError as err:
         console.print(f"[red]Error:[/red] {err.response.text}")
 
 
-@users.command(cls=IncydrCommand)
-@click.argument("file", type=click.File())
-@input_format_option
-@logging_options
-def bulk_move(file: Path, format_: str):
-
+def _get_cursor_store(api_key):
     """
-    Bulk move multiple users to specified organizations.
-
-    Takes a single arg `FILE` which specifies the path to the file (use "-" to read from stdin).
-
-    File format can either be CSV or [JSON Lines format](https://jsonlines.org) (Default is CSV).
-
-    Requires the following columns:
-
-    * `user` - User ID or username of the user who will be moved to the new organization. Performs an additional lookup if username is passed.
-    * `org_guid` - GUID for the user's new organization.
+    Get cursor store for sessions search checkpoints.
     """
-    client = Client()
-
-    class UserMoveCSV(UserCSV):
-        org_guid: str = Field(csv_aliases=["org_guid", "orgGuid", "org"])
-
-    class UserMoveJSON(UserJSON):
-        org_guid: str = Field(alias="orgGuid")
+    dir_path = get_user_project_path(
+        "checkpoints",
+        api_key,
+        "session_checkpoints",
+    )
+    return CursorStore(dir_path, "sessions")
 
-    @lru_cache()
-    def resolve_username(user):
-        if user is None:
-            return
-        elif "@" in user:
-            return user_lookup(client, user)
-        else:  # assume user_id
-            return user
 
-    if format_ == "csv":
-        models = UserMoveCSV.parse_csv(file)
-    else:
-        models = UserMoveJSON.parse_json_lines(file)
+def _update_checkpoint(cursor, checkpoint_name, sessions_gen):
+    """
+    De-duplicates results across checkpointed runs.
 
-    try:
-        for row in track(
-            models,
-            description="Moving users...",
-            transient=True,
-        ):
-            client.users.v1.move(resolve_username(row.user), row.org_guid)
-    except HTTPError as err:
-        console.print(f"[red]Error:[/red] {err.response.text}")
+    Since using the timestamp of the last result
+    processed as the `--start` time of the next run causes the last event to show up again in the
+    next results, store the last session IDs in the cursor to
+    filter out on the next run.
+
+    It's also possible that two sessions have the exact same timestamp, so
+    `checkpoint_sessions` needs to be a list of session IDs so we can filter out everything that's actually
+    been processed.
+    """
+    checkpoint_sessions = cursor.get_items(checkpoint_name)
+    new_timestamp = None
+    new_sessions = []
+    for session in sessions_gen:
+        session_id = session.session_id
+        if session_id not in checkpoint_sessions:
+            if not new_timestamp or session.end_time > new_timestamp:
+                new_timestamp = session.end_time
+                new_sessions.clear()
+            new_sessions.append(session_id)
+            yield session
+            cursor.replace(checkpoint_name, new_timestamp)
+            cursor.replace_items(checkpoint_name, new_sessions)
```

### Comparing `incydr-1.2.0/_incydr_cli/cmds/utils.py` & `incydr-2.0.0/_incydr_cli/cmds/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 # CLI - specific utils.py file to avoid circular imports
 from functools import wraps
 from signal import getsignal
 from signal import SIGINT
 from signal import signal
 
 import click
+from click import echo
 from click import style
 
 
+def deprecation_warning(text):
+    echo(style(text, fg="red"), err=True)
+
+
 def user_lookup(client, value):
     """
     Returns the user ID for a given username, or returns the value unchanged if not a username.
 
     Used with the `user_lookup_callback` method on user args.
     """
     if "@" in str(value):
```

### Comparing `incydr-1.2.0/_incydr_cli/cmds/watchlists.py` & `incydr-2.0.0/_incydr_cli/cmds/watchlists.py`

 * *Files identical despite different names*

### Comparing `incydr-1.2.0/_incydr_cli/cmds/options/alert_filter_options.py` & `incydr-2.0.0/_incydr_cli/cmds/options/alert_filter_options.py`

 * *Files identical despite different names*

### Comparing `incydr-1.2.0/_incydr_cli/cmds/options/audit_log_filter_options.py` & `incydr-2.0.0/_incydr_cli/cmds/options/audit_log_filter_options.py`

 * *Files identical despite different names*

### Comparing `incydr-1.2.0/_incydr_cli/cmds/options/event_filter_options.py` & `incydr-2.0.0/_incydr_cli/cmds/options/event_filter_options.py`

 * *Files identical despite different names*

### Comparing `incydr-1.2.0/_incydr_cli/cmds/options/output_options.py` & `incydr-2.0.0/_incydr_cli/cmds/options/output_options.py`

 * *Files identical despite different names*

### Comparing `incydr-1.2.0/_incydr_cli/cmds/options/profile_filter_options.py` & `incydr-2.0.0/_incydr_cli/cmds/options/profile_filter_options.py`

 * *Files identical despite different names*

### Comparing `incydr-1.2.0/_incydr_cli/cmds/options/utils.py` & `incydr-2.0.0/_incydr_cli/cmds/options/utils.py`

 * *Files identical despite different names*

### Comparing `incydr-1.2.0/_incydr_cli/logger/__init__.py` & `incydr-2.0.0/_incydr_cli/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `incydr-1.2.0/_incydr_cli/logger/handlers.py` & `incydr-2.0.0/_incydr_cli/logger/handlers.py`

 * *Files identical despite different names*

### Comparing `incydr-1.2.0/_incydr_sdk/exceptions.py` & `incydr-2.0.0/_incydr_sdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `incydr-1.2.0/_incydr_sdk/utils.py` & `incydr-2.0.0/_incydr_sdk/utils.py`

 * *Files identical despite different names*

### Comparing `incydr-1.2.0/_incydr_sdk/agents/client.py` & `incydr-2.0.0/_incydr_sdk/agents/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,19 +48,19 @@
         **Parameters**:
 
         * **active**: `bool | None` - When `True`, return only active agents. When `False`, return only deactivated agents. Defaults to `None` (returning both).
         * **agent_type**: `AgentType | str | None` - Return only agents of given type.
         * **page_num**: `int` - Page number for results, starting at 1.
         * **page_size**: `int` - Max number of results to return per page.
         * **sort_dir**: `SortDirection` - `asc` or `desc`. The direction in which to sort the response based on the corresponding key. Defaults to `asc`.
-        * **sort_key**: `[SortKeys][agents-sort-keys]` - Values on which the response will be sorted. Defaults to agent name.
+        * **sort_key**: [`SortKeys`][agents-sort-keys] - Values on which the response will be sorted. Defaults to agent name.
         * **agent_healthy**: `bool | None` - Optionally retrieve agents with this health status. Agents that have no health issue types are considered healthy.
         * **agent_health_issue_types**: `List[str] | str` - Optionally retrieve agents that have (at least) any of the given issue type(s). Health issue types include the following: `NOT_CONNECTING`, `NOT_SENDING_SECURITY_EVENTS`.
 
-        **Returns**: An `[AgentsPage][agentspage-model]` object.
+        **Returns**: An [`AgentsPage`][agentspage-model] object.
         """
         data = QueryAgentsRequest(
             active=active,
             agentType=agent_type,
             agentHealthy=agent_healthy,
             anyOfAgentHealthIssueTypes=[agent_health_issue_types]
             if isinstance(agent_health_issue_types, str)
```

### Comparing `incydr-1.2.0/_incydr_sdk/agents/models.py` & `incydr-2.0.0/_incydr_sdk/agents/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     * **name**: `str` The editable name of the agent.
     * **user_id**: `str` The unique ID of the user the agent is assigned to.
     * **os_hostname**: `str` The hostname reported by the OS the agent is running on.
     * **os_name**: `str` The name of the OS the agent is running on.
     * **machine_id**: `str` Device machine ID.
     * **serial_number**: `str` Authenticated agent serial number.
     * **active**: `bool` If the agent status is active.
-    * **agent_type**: `[AgentType][agent-type]` The type of agent.
+    * **agent_type**: [`AgentType`][agent-type] The type of agent.
     * **agent_health_issue_types: `List[str]` List of health issues with the agent. Health issue types include the following: `NOT_CONNECTING`, `NOT_SENDING_SECURITY_EVENTS`.
     * **app_version**: `str` The app version of the agent.
     * **product_version**: `str` The product version of the agent.
     * **last_connected**: `datetime` The time the agent last connected to a Code42 Authority server.
     * **external_reference**: `str` Editable reference information (useful for identifying an agent in external systems).
     * **creation_date**: `datetime` The time the agent was first registered.
     * **modification_date**: `datetime` The time the agent's database entry was last updated.
```

### Comparing `incydr-1.2.0/_incydr_sdk/alert_rules/client.py` & `incydr-2.0.0/_incydr_sdk/alert_rules/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 from requests import HTTPError
 from requests import Response
 
 from _incydr_sdk.alert_rules.models.request import GetRulesRequest
 from _incydr_sdk.alert_rules.models.response import RuleDetails
 from _incydr_sdk.alert_rules.models.response import RuleUsersList
 from _incydr_sdk.exceptions import IncydrException
-from _incydr_sdk.user_risk_profiles.models import UserRiskProfile
 
 
 class MissingUsernameCriterionError(IncydrException):
     """An error raised if an alert rule has no username filter."""
 
     def __init__(self, rule_id):
         super().__init__(
@@ -168,12 +167,7 @@
         except HTTPError as e:
             # This endpoint doesn't have query params or a request body, so it should
             # only return a 400 if there is not username filter for the rule.
             if e.response.status_code == 400:
                 raise MissingUsernameCriterionError(rule_id)
             raise e
         return RuleUsersList.parse_response(response)
-
-    def _get_user_aliases(self, user_id):
-        response = self._parent.session.get(f"/v1/user-risk-profiles/{user_id}")
-        profile = UserRiskProfile.parse_response(response)
-        return profile.cloud_aliases
```

### Comparing `incydr-1.2.0/_incydr_sdk/alert_rules/models/response.py` & `incydr-2.0.0/_incydr_sdk/alert_rules/models/response.py`

 * *Files identical despite different names*

### Comparing `incydr-1.2.0/_incydr_sdk/alerts/client.py` & `incydr-2.0.0/_incydr_sdk/alerts/client.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import itertools
 from itertools import count
 from typing import Iterator
 from typing import List
 from typing import Union
+from warnings import warn
 
 import requests
 from pydantic import parse_obj_as
 
 from .models.alert import AlertSummary
 from .models.request import AddNoteRequest
 from .models.request import AlertDetailsRequest
@@ -38,14 +39,20 @@
 
         **Parameters**:
 
         * **query**: `AlertQuery` (required) - The query object to filter alerts by different fields.
 
         **Returns**: An [`AlertQueryPage`][alertquerypage-model] object.
         """
+        warn(
+            "Alerts are deprecated. Replaced by Sessions.",
+            DeprecationWarning,
+            stacklevel=2,
+        )
+
         if not isinstance(query, AlertQuery):
             raise ValueError("query must be an `incydr.AlertQuery` object.")
         query.tenant_id = self._parent.tenant_id
         response = self._parent.session.post(
             "/v1/alerts/query-alerts", json=query.dict()
         )
         return AlertQueryPage.parse_response(response)
@@ -54,14 +61,20 @@
         """
         Retrieve all alerts for a given query, automatically retrieving multiple pages if they exist.
 
         * **query**: `AlertQuery` (required) - The query object used to filter alerts by different fields.
 
         **Returns**: A generator yielding individual [`AlertSummary`][alertsummary-model] objects.
         """
+        warn(
+            "Alerts are deprecated. Replaced by Sessions.",
+            DeprecationWarning,
+            stacklevel=2,
+        )
+
         if not isinstance(query, AlertQuery):
             raise ValueError("query must be an `incydr.AlertQuery` object.")
         query.tenant_id = self._parent.tenant_id
         for page_num in count(0):
             query.page_num = page_num
             response = self._parent.session.post(
                 "/v1/alerts/query-alerts", json=query.dict()
@@ -80,14 +93,20 @@
 
         **Parameters**:
 
         * **alert_ids**: `str | List[str]` (required) - Single alertId or list of alertId strings.
 
         **Returns**: A list of [`AlertDetails`][alertdetails-model] objects.
         """
+        warn(
+            "Alerts are deprecated. Replaced by Sessions.",
+            DeprecationWarning,
+            stacklevel=2,
+        )
+
         if isinstance(alert_ids, str):
             alert_ids = [alert_ids]
         results = []
         ids = iter(alert_ids)
         while True:
             chunk = list(itertools.islice(ids, 100))
             if not chunk:
@@ -106,14 +125,20 @@
 
         **Parameters**:
 
         * **alert_id**: `List[str]` (required) -
 
         **Returns**: A `Response` object indicating success.
         """
+        warn(
+            "Alerts are deprecated. Replaced by Sessions.",
+            DeprecationWarning,
+            stacklevel=2,
+        )
+
         data = AddNoteRequest(
             alertId=alert_id,
             note=note,
             tenantId=self._parent.tenant_id,
         )
         return self._parent.session.post(
             "/v1/alerts/add-note", json=data.dict(by_alias=True)
@@ -129,14 +154,20 @@
 
         * **alert_id**: `str | List[str]` (required) - ID or list of IDs of the alert(s) to update.
         * **state**: [`AlertState`][alert-state] (required) - State to set alert(s) to.
         * **note**: `str` - Optional note text.
 
         **Returns**: A `Response` object indicating success.
         """
+        warn(
+            "Alerts are deprecated. Replaced by Sessions.",
+            DeprecationWarning,
+            stacklevel=2,
+        )
+
         if isinstance(alert_ids, str):
             alert_ids = [alert_ids]
         data = UpdateAlertStateRequest(
             tenantId=self._parent.tenant_id,
             alertIds=alert_ids,
             state=state,
             note=note,
```

### Comparing `incydr-1.2.0/_incydr_sdk/alerts/models/alert.py` & `incydr-2.0.0/_incydr_sdk/alerts/models/alert.py`

 * *Files identical despite different names*

### Comparing `incydr-1.2.0/_incydr_sdk/alerts/models/enums.py` & `incydr-2.0.0/_incydr_sdk/alerts/models/enums.py`

 * *Files identical despite different names*

### Comparing `incydr-1.2.0/_incydr_sdk/alerts/models/request.py` & `incydr-2.0.0/_incydr_sdk/alerts/models/request.py`

 * *Files identical despite different names*

### Comparing `incydr-1.2.0/_incydr_sdk/alerts/models/response.py` & `incydr-2.0.0/_incydr_sdk/alerts/models/response.py`

 * *Files identical despite different names*

### Comparing `incydr-1.2.0/_incydr_sdk/audit_log/client.py` & `incydr-2.0.0/_incydr_sdk/audit_log/client.py`

 * *Files identical despite different names*

### Comparing `incydr-1.2.0/_incydr_sdk/audit_log/models.py` & `incydr-2.0.0/_incydr_sdk/audit_log/models.py`

 * *Files identical despite different names*

### Comparing `incydr-1.2.0/_incydr_sdk/cases/client.py` & `incydr-2.0.0/_incydr_sdk/cases/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
         """
         Create a case.
 
         **Parameters:**
 
         * **name**: `str` (required) The unique name given to the case.
         * **subject**: `str` The user UID of the subject being investigated in this case.
-        * **assignee**: `str` The user UID of the administrator assigned to investigate the case.
+        * **assignee**: `str` The actor ID of the administrator assigned to investigate the case.
         * **findings**: `str` Markdown formatted text summarizing the findings for a case.
         * **description**: `str` Brief description providing context for a case.
 
         **Returns**: A [`Case`][case-model] object representing the newly created case.
         """
         data = CreateCaseRequest(
             name=name,
@@ -120,15 +120,15 @@
         """
         Get a page of cases.
 
         Filter results by passing appropriate parameters:
 
         **Parameters**:
 
-        * **assignee**: `str` - User UID of an assignee of a case on which to filter.
+        * **assignee**: `str` - Actor ID of an assignee of a case on which to filter.
         * **created_at**: `Tuple[datetime, datetime]` - Filter cases created between the supplied start and end times.
         * **is_assigned**: `bool` - Filter cases with an assignee (`True`) or without (`False`).
         * **last_modified_by**: `str` - User UID of the user who most recently modified the case.
         * **name**: str - Name of a case on which to filter; will include partial matches.
         * **status**: [`CaseStatus`][case-statuses] - One or more case statuses on which to filter. Available values: `OPEN`, `CLOSED`
         * **page_num**: `int` - Page number for results, starting at 1.
         * **page_size**: `int` - Max number of results to return for a page. Defaults to client's `page_size` setting.
```

### Comparing `incydr-1.2.0/_incydr_sdk/cases/models.py` & `incydr-2.0.0/_incydr_sdk/cases/models.py`

 * *Files identical despite different names*

### Comparing `incydr-1.2.0/_incydr_sdk/core/auth.py` & `incydr-2.0.0/_incydr_sdk/core/auth.py`

 * *Files identical despite different names*

### Comparing `incydr-1.2.0/_incydr_sdk/core/client.py` & `incydr-2.0.0/_incydr_sdk/core/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,29 +4,31 @@
 from collections import deque
 
 import pydantic
 from requests_toolbelt import user_agent
 from requests_toolbelt.sessions import BaseUrlSession
 
 from _incydr_sdk.__version__ import __version__
+from _incydr_sdk.actors.client import ActorsClient
 from _incydr_sdk.agents.client import AgentsClient
 from _incydr_sdk.alert_rules.client import AlertRulesClient
 from _incydr_sdk.alerts.client import AlertsClient
 from _incydr_sdk.audit_log.client import AuditLogClient
 from _incydr_sdk.cases.client import CasesClient
 from _incydr_sdk.core.auth import APIClientAuth
 from _incydr_sdk.core.settings import IncydrSettings
 from _incydr_sdk.customer.client import CustomerClient
 from _incydr_sdk.departments.client import DepartmentsClient
 from _incydr_sdk.devices.client import DevicesClient
 from _incydr_sdk.directory_groups.client import DirectoryGroupsClient
 from _incydr_sdk.exceptions import AuthMissingError
 from _incydr_sdk.file_events.client import FileEventsClient
+from _incydr_sdk.risk_profiles.client import RiskProfiles
+from _incydr_sdk.sessions.client import SessionsClient
 from _incydr_sdk.trusted_activities.client import TrustedActivitiesClient
-from _incydr_sdk.user_risk_profiles.client import UserRiskProfiles
 from _incydr_sdk.users.client import UsersClient
 from _incydr_sdk.watchlists.client import WatchlistsClient
 
 _base_user_agent = user_agent("incydr", __version__)
 
 
 class Client:
@@ -89,27 +91,29 @@
                 self.settings._log_response_debug(response)
 
             self._request_history.appendleft(response)
             response.raise_for_status()
 
         self._session.hooks["response"] = [response_hook]
 
+        self._actors = ActorsClient(self)
         self._agents = AgentsClient(self)
         self._alerts = AlertsClient(self)
         self._alert_rules = AlertRulesClient(self)
         self._audit_log = AuditLogClient(self)
         self._cases = CasesClient(self)
         self._customer = CustomerClient(self)
         self._departments = DepartmentsClient(self)
         self._devices = DevicesClient(self)
         self._directory_groups = DirectoryGroupsClient(self)
         self._file_events = FileEventsClient(self)
+        self._sessions = SessionsClient(self)
         self._trusted_activities = TrustedActivitiesClient(self)
         self._users = UsersClient(self)
-        self._user_risk_profiles = UserRiskProfiles(self)
+        self._risk_profiles = RiskProfiles(self)
         self._watchlists = WatchlistsClient(self)
 
         if not skip_auth:
             self._session.auth.refresh()
 
     @property
     def tenant_id(self):
@@ -153,27 +157,37 @@
             <Response [200]>
             >>> response.url
             'https://api.us.code42.com/v1/users'
         """
         return self._session
 
     @property
+    def actors(self):
+        """
+        Property returning an [`ActorsClient`](../actors) for interacting with `/v*/actors` API endpoints.
+
+        Usage:
+            >>> clients.actors.v1.get_page()
+        """
+        return self._actors
+
+    @property
     def agents(self):
         """
         Property returning an [`AgentsClient`](../agents) for interacting with
         `/v*/agents` API endpoints.
         Usage:
             >>> client.agents.v1.get_page()
         """
         return self._agents
 
     @property
     def alerts(self):
         """
-        Property returning an [`AlertsClient`](../alerts) for interacting with
+        (DEPRECATED) Property returning an [`AlertsClient`](../alerts) for interacting with
         `/v*/alerts` API endpoints.
         Usage:
             >>> client.alerts.v1.get_page()
         """
         return self._alerts
 
     @property
@@ -266,14 +280,25 @@
 
             >>> client.file_events.v2.search(query)
 
         """
         return self._file_events
 
     @property
+    def sessions(self):
+        """
+        Property returning a [`SessionsClient`](../sessions) for interacting with `/v*/sessions` API endpoints.
+        Usage:
+
+            >>> client.items.v1.get_page(has_alerts=True)
+
+        """
+        return self._sessions
+
+    @property
     def trusted_activities(self):
         """
         Property returning a [`TrustedActivitiesClient`](../trusted_activities) for interacting with
         `/v*/trusted-activities` API endpoints.
 
         Usage:
 
@@ -290,25 +315,25 @@
 
             >>> client.users.v1.get_page(active=True)
 
         """
         return self._users
 
     @property
-    def user_risk_profiles(self):
+    def risk_profiles(self):
         """
-        Property returning a [`UserRiskProfilesClient`](../user_risk_profiles) for interacting with
+        Property returning a [`RiskProfilesClient`](../risk_profiles) for interacting with
         `/v*/user_risk_profiles` API endpoints.
 
         Usage:
 
-            >>> client.user_risk_profiles.v1.get_user_risk_profile("23")
+            >>> client.risk_profiles.v1.get_risk_profile("23")
 
         """
-        return self._user_risk_profiles
+        return self._risk_profiles
 
     @property
     def watchlists(self):
         """
         Property returning a [`WatchlistsClient`](../watchlists) for interacting with `/v*/watchlists` API endpoints.
         Usage:
```

### Comparing `incydr-1.2.0/_incydr_sdk/core/models.py` & `incydr-2.0.0/_incydr_sdk/core/models.py`

 * *Files identical despite different names*

### Comparing `incydr-1.2.0/_incydr_sdk/core/settings.py` & `incydr-2.0.0/_incydr_sdk/core/settings.py`

 * *Files identical despite different names*

### Comparing `incydr-1.2.0/_incydr_sdk/customer/client.py` & `incydr-2.0.0/_incydr_sdk/customer/client.py`

 * *Files identical despite different names*

### Comparing `incydr-1.2.0/_incydr_sdk/customer/models.py` & `incydr-2.0.0/_incydr_sdk/customer/models.py`

 * *Files identical despite different names*

### Comparing `incydr-1.2.0/_incydr_sdk/departments/client.py` & `incydr-2.0.0/_incydr_sdk/departments/client.py`

 * *Files identical despite different names*

### Comparing `incydr-1.2.0/_incydr_sdk/departments/models.py` & `incydr-2.0.0/_incydr_sdk/departments/models.py`

 * *Files identical despite different names*

### Comparing `incydr-1.2.0/_incydr_sdk/devices/client.py` & `incydr-2.0.0/_incydr_sdk/devices/client.py`

 * *Files identical despite different names*

### Comparing `incydr-1.2.0/_incydr_sdk/devices/models.py` & `incydr-2.0.0/_incydr_sdk/devices/models.py`

 * *Files identical despite different names*

### Comparing `incydr-1.2.0/_incydr_sdk/directory_groups/client.py` & `incydr-2.0.0/_incydr_sdk/directory_groups/client.py`

 * *Files identical despite different names*

### Comparing `incydr-1.2.0/_incydr_sdk/directory_groups/models.py` & `incydr-2.0.0/_incydr_sdk/directory_groups/models.py`

 * *Files identical despite different names*

### Comparing `incydr-1.2.0/_incydr_sdk/enums/__init__.py` & `incydr-2.0.0/_incydr_sdk/enums/__init__.py`

 * *Files identical despite different names*

### Comparing `incydr-1.2.0/_incydr_sdk/enums/alerts.py` & `incydr-2.0.0/_incydr_sdk/enums/alerts.py`

 * *Files identical despite different names*

### Comparing `incydr-1.2.0/_incydr_sdk/enums/cases.py` & `incydr-2.0.0/_incydr_sdk/enums/cases.py`

 * *Files identical despite different names*

### Comparing `incydr-1.2.0/_incydr_sdk/enums/file_events.py` & `incydr-2.0.0/_incydr_sdk/enums/file_events.py`

 * *Files identical despite different names*

### Comparing `incydr-1.2.0/_incydr_sdk/enums/trusted_activities.py` & `incydr-2.0.0/_incydr_sdk/enums/trusted_activities.py`

 * *Files identical despite different names*

### Comparing `incydr-1.2.0/_incydr_sdk/enums/watchlists.py` & `incydr-2.0.0/_incydr_sdk/enums/watchlists.py`

 * *Files identical despite different names*

### Comparing `incydr-1.2.0/_incydr_sdk/file_events/client.py` & `incydr-2.0.0/_incydr_sdk/file_events/client.py`

 * *Files identical despite different names*

### Comparing `incydr-1.2.0/_incydr_sdk/file_events/models/event.py` & `incydr-2.0.0/_incydr_sdk/file_events/models/event.py`

 * *Files identical despite different names*

### Comparing `incydr-1.2.0/_incydr_sdk/file_events/models/response.py` & `incydr-2.0.0/_incydr_sdk/file_events/models/response.py`

 * *Files identical despite different names*

### Comparing `incydr-1.2.0/_incydr_sdk/queries/alerts.py` & `incydr-2.0.0/_incydr_sdk/queries/alerts.py`

 * *Files identical despite different names*

### Comparing `incydr-1.2.0/_incydr_sdk/queries/file_events.py` & `incydr-2.0.0/_incydr_sdk/queries/file_events.py`

 * *Files identical despite different names*

### Comparing `incydr-1.2.0/_incydr_sdk/queries/utils.py` & `incydr-2.0.0/_incydr_sdk/queries/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
     **Returns**:
         (str): A str representing the given timestamp. Example output looks like
         '2020-03-25T15:29:04.465Z'.
     """
     # convert str/int/float values to datetime
     if isinstance(timestamp, (int, float)):
-        timestamp = datetime.utcfromtimestamp(timestamp)
+        timestamp = datetime.fromtimestamp(timestamp, tz=timezone.utc)
     elif isinstance(timestamp, str):
         timestamp = parse_str_to_dt(timestamp)
     timestamp.replace(tzinfo=timezone.utc)
     # parse datetime to string
     return f"{timestamp.strftime(MICROSECOND_FORMAT)[:-4]}Z"
```

### Comparing `incydr-1.2.0/_incydr_sdk/trusted_activities/client.py` & `incydr-2.0.0/_incydr_sdk/trusted_activities/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 
         **Parameters**:
 
         * **page_num**: `int` - Page number for results, starting at 1.
         * **page_size**: `int` - Max number of results to return per page. Defaults to client's `page_size` setting.
         * **activity_type**: `ActivityType` - The type of the trusted activity.
         * **sort_key**: `SortKeys` - The key by which to sort the returned list.
-        * **sort_direction**: `SortDirection` - The order in which to sort the returned list.
+        * **sort_dir**: `SortDirection` - The order in which to sort the returned list.
 
         **Returns**: A [`TrustedActivitiesPage`][trustedactivitiespage-model] object.
         """
 
         page_size = page_size or self._parent.settings.page_size
         data = QueryTrustedActivitiesRequest(
             page_num=page_num,
```

### Comparing `incydr-1.2.0/_incydr_sdk/trusted_activities/models.py` & `incydr-2.0.0/_incydr_sdk/trusted_activities/models.py`

 * *Files identical despite different names*

### Comparing `incydr-1.2.0/_incydr_sdk/user_risk_profiles/client.py` & `incydr-2.0.0/_incydr_sdk/risk_profiles/client.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,61 +1,59 @@
 from datetime import datetime
 from itertools import count
 from typing import Iterator
 from typing import Union
 
-from requests import Response
-
 from _incydr_sdk.exceptions import DateParseError
 from _incydr_sdk.queries.utils import DATE_STR_FORMAT
-from _incydr_sdk.user_risk_profiles.models import Date
-from _incydr_sdk.user_risk_profiles.models import QueryUserRiskProfilesRequest
-from _incydr_sdk.user_risk_profiles.models import UpdateUserRiskProfileRequest
-from _incydr_sdk.user_risk_profiles.models import UserRiskProfile
-from _incydr_sdk.user_risk_profiles.models import UserRiskProfilesPage
+from _incydr_sdk.risk_profiles.models import Date
+from _incydr_sdk.risk_profiles.models import QueryRiskProfilesRequest
+from _incydr_sdk.risk_profiles.models import RiskProfile
+from _incydr_sdk.risk_profiles.models import RiskProfilesPage
+from _incydr_sdk.risk_profiles.models import UpdateRiskProfileRequest
 
 
-class UserRiskProfiles:
+class RiskProfiles:
     def __init__(self, parent):
         self._parent = parent
         self._v1 = None
 
     @property
     def v1(self):
         if self._v1 is None:
-            self._v1 = UserRiskProfilesV1(self._parent)
+            self._v1 = RiskProfilesV1(self._parent)
         return self._v1
 
 
-class UserRiskProfilesV1:
+class RiskProfilesV1:
     """
     Client for `/v1/user-risk-profiles` endpoints.
 
     Usage example:
 
         >>> import incydr
         >>> client = incydr.Client(**kwargs)
-        >>> client.user_risk_profiles.v1.get_page()
+        >>> client.risk_profiles.v1.get_page()
     """
 
     def __init__(self, parent):
         self._parent = parent
 
-    def get_user_risk_profile(self, user_id: str) -> UserRiskProfile:
+    def get_risk_profile(self, user_id: str) -> RiskProfile:
         """
-        Get a single user risk profile.
+        Get a single risk profile.
 
         **Parameters:**
 
         * **user_id**: `str` (required) - The unique ID for the user.
 
-        **Returns**: A [`UserRiskProfile`][userriskprofile-model] object representing the user risk profile.
+        **Returns**: A [`RiskProfile`][riskprofile-model] object representing the risk profile.
         """
         response = self._parent.session.get(f"/v1/user-risk-profiles/{user_id}")
-        return UserRiskProfile.parse_response(response)
+        return RiskProfile.parse_response(response)
 
     def get_page(
         self,
         page_num: int = 1,
         page_size: int = None,
         manager_id: str = None,
         title: str = None,
@@ -64,17 +62,17 @@
         employment_type: str = None,
         country: str = None,
         region: str = None,
         locality: str = None,
         active: bool = None,
         deleted: bool = None,
         support_user: bool = None,
-    ) -> UserRiskProfilesPage:
+    ) -> RiskProfilesPage:
         """
-        Get a page of user risk profiles.
+        Get a page of risk profiles.
 
         Filter results by passing the appropriate parameters:
 
         **Parameters**:
 
         * **page_num**: `int` - Page number for results, starting at 1.
         * **page_size**: `int` - Max number of results to return per page.
@@ -89,18 +87,18 @@
         ** **active**: `bool | None` - When true, return only active users. When false, return only inactive users.
                                        Defaults to `None` (returning both).
         * **deleted**: `bool | None` - When true, return only deleted users. When false, return only non-deleted users.
                                        Defaults to returning both.
         * **support_user**: `bool | None` - When true, return only support users. When false, return only non-support users.
                                             Defaults to returning both
 
-        **Returns**: A ['UserRiskProfilesPage'][userriskprofilespage-model] object.
+        **Returns**: A ['RiskProfilesPage'][riskprofilespage-model] object.
         """
         page_size = page_size or self._parent.settings.page_size
-        data = QueryUserRiskProfilesRequest(
+        data = QueryRiskProfilesRequest(
             page=page_num,
             page_size=page_size,
             manager_id=manager_id,
             title=title,
             division=division,
             department=department,
             employment_type=employment_type,
@@ -110,15 +108,15 @@
             active=active,
             deleted=deleted,
             support_user=support_user,
         )
         response = self._parent.session.get(
             "/v1/user-risk-profiles", params=data.dict()
         )
-        return UserRiskProfilesPage.parse_response(response)
+        return RiskProfilesPage.parse_response(response)
 
     def iter_all(
         self,
         page_size: int = None,
         manager_id: str = None,
         title: str = None,
         division: str = None,
@@ -126,21 +124,21 @@
         employment_type: str = None,
         country: str = None,
         region: str = None,
         locality: str = None,
         active: bool = None,
         deleted: bool = None,
         support_user: bool = None,
-    ) -> Iterator[UserRiskProfile]:
+    ) -> Iterator[RiskProfile]:
         """
-        Iterate over all user risk profiles.
+        Iterate over all risk profiles.
 
         Accepts the same parameters as `.get_page()` except `page_num`.
 
-        **Returns**: A generator yielding individual [`UserRiskProfile`][userriskprofile-model] objects.
+        **Returns**: A generator yielding individual [`RiskProfile`][riskprofile-model] objects.
         """
         page_size = page_size or self._parent.settings.page_size
         for page_num in count(1):
             page = self.get_page(
                 page_num=page_num,
                 page_size=page_size,
                 manager_id=manager_id,
@@ -161,86 +159,48 @@
 
     def update(
         self,
         user_id: str,
         notes: str = None,
         start_date: Union[datetime, str] = None,
         end_date: Union[datetime, str] = None,
-    ) -> UserRiskProfile:
+    ) -> RiskProfile:
         """
-        Updates a user risk profile.
+        Updates a risk profile.
 
         **Parameters**
 
-        * **notes**: `str` - Additional notes for the user risk profile.
+        * **notes**: `str` - Additional notes for the risk profile.
         * **start_date**: `datetime` - The starting date for the user. Accepts a datetime object or a string in the format yyyy-MM-dd (UTC) format. Pass an empty string to clear the field.
         * **end_date**: `datetime` - The departure date for the user.  Accepts a datetime object or a string in the format yyyy-MM-dd (UTC) format.  Pass an empty string to clear the field.
 
-        **Returns**: A [`UserRiskProfile`][userriskprofile-model] object.
+        **Returns**: A [`RiskProfile`][riskprofile-model] object.
         """
         paths = []
         if start_date is not None:
             paths += ["startDate"]
             start_date = None if start_date == "" else _create_date(start_date)
         if end_date is not None:
             paths += ["endDate"]
             end_date = None if end_date == "" else _create_date(end_date)
         if notes is not None:
             paths += ["notes"]
             if notes == "":
                 notes = None
 
-        data = UpdateUserRiskProfileRequest(
+        data = UpdateRiskProfileRequest(
             endDate=end_date, notes=notes, startDate=start_date
         )
 
         response = self._parent.session.patch(
             f"/v1/user-risk-profiles/{user_id}",
             params={"paths": paths},
             json=data.dict(),
         )
-        return UserRiskProfile.parse_response(response)
-
-    def add_cloud_alias(self, user_id: str, cloud_alias: str) -> Response:
-        """
-        Add cloud aliases to a user risk profile.
-
-        A cloud alias is the username an employee uses to access cloud services such as Google Drive or Box.
-        Adding a cloud alias allows Incydr to link a user's cloud activity with their Code42 username.
-        Each user has a default cloud alias of their Code42 username. You can add one additional alias.
-
-        **Parameters:**
-
-        * **user_id**: `str` - User ID of the profile to update.
-        * **cloud_alias**: `str` - The new cloud alias to add to the user risk profile.
-
-        **Returns**: A `requests.Response` indicating success.
-        """
-
-        return self._parent.session.post(
-            f"/v1/user-risk-profiles/{user_id}/add-cloud-aliases",
-            json={"userId": user_id, "cloudAliases": [cloud_alias]},
-        )
-
-    def delete_cloud_alias(self, user_id: str, cloud_alias: str) -> Response:
-        """
-        Delete a cloud alias from a user risk profile.
-
-        **Parameters:**
-
-        * **user_id**: `str` - User ID of the profile to update.
-        * **cloud_alias**: `str` - The cloud alias to remove from the user risk profile.
-
-        **Returns**: A `requests.Response` indicating success.
-        """
-
-        return self._parent.session.post(
-            f"/v1/user-risk-profiles/{user_id}/delete-cloud-aliases",
-            json={"userId": user_id, "cloudAliases": [cloud_alias]},
-        )
+        return RiskProfile.parse_response(response)
 
 
 def _create_date(date: Union[datetime, str]):
     if not isinstance(date, datetime):
         try:
             date = datetime.strptime(date, DATE_STR_FORMAT)
         except ValueError:
```

### Comparing `incydr-1.2.0/_incydr_sdk/user_risk_profiles/models.py` & `incydr-2.0.0/_incydr_sdk/risk_profiles/models.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,114 +22,116 @@
     day: Optional[int] = Field(
         None,
         description="Day of month. Must be from 1 to 31 and valid for the year and month, or 0\n if specifying a year "
         "by itself or a year and month where the day is not\n significant.",
     )
 
 
-class UserRiskProfile(ResponseModel):
-    """A model representing a user risk profile.
+class RiskProfile(ResponseModel):
+    """A model representing a risk profile.
 
     **Fields**:
 
-    * **active**: `bool` - Whether the user is active.
-    * **cloud_alias**: `List[str]` - List of cloud aliases for the user.
-    * **country**: `str` - The user's country.
-    * **deleted**: `bool` - Whether the user has been deleted.
-    * **department**: `str` - The user's department.
-    * **display_name**: `str` - The user's display name.
-    * **division**: `str` - The user's division.
-    * **employment_type**: `str` - The user's employment type.
-    * **end_date**: `Date` - Departure date for the user
-    * **locality**: `str` - The user's locality (city).
-    * **manager_display_name**: `str` - The user's manager's display name.
-    * **manager_id**: `str` - Unique user ID of the user's manager.
-    * **manager_username**: `str` - The Code42 username of the user's manager.
-    * **notes**: `str` - Additional notes about the user.
-    * **region**: `str` - The user's region (state).
-    * **start_date**: `Date` - Starting date for the user.
-    * **support_user**: `bool` - Whether the user is a support user.
+    * **active**: `bool` - Whether the actor is active.
+    * **cloud_alias**: `List[str]` - List of cloud aliases for the actor.
+    * **country**: `str` - The actor's country.
+    * **deleted**: `bool` - Whether the actor has been deleted.
+    * **department**: `str` - The actor's department.
+    * **display_name**: `str` - The actor's display name.
+    * **division**: `str` - The actor's division.
+    * **employment_type**: `str` - The actor's employment type.
+    * **end_date**: `Date` - Departure date for the actor
+    * **locality**: `str` - The actor's locality (city).
+    * **manager_display_name**: `str` - The actor's manager's display name.
+    * **manager_id**: `str` - Unique actor ID of the actor's manager.
+    * **manager_username**: `str` - The Code42 actorname of the actor's manager.
+    * **notes**: `str` - Additional notes about the actor.
+    * **region**: `str` - The actor's region (state).
+    * **start_date**: `Date` - Starting date for the actor.
+    * **support_user**: `bool` - Whether the actor is a support actor.
     * **tenant_id**: `str` - Unique tenant ID.
-    * **title**: `str` - The user's job title.
-    * **user_id**: `str` - Unique user ID.
-    * **username**: `str` - User's Code42 username.
+    * **title**: `str` - The actor's job title.
+    * **user_id**: `str` - Unique actor ID.
+    * **username**: `str` - actor's Code42 actorname.
     """
 
-    active: Optional[bool] = Field(None, description="Whether the user is active.")
+    active: Optional[bool] = Field(None, description="Whether the actor is active.")
     cloud_aliases: Optional[List[str]] = Field(
-        None, description="A list of cloud aliases for the user.", alias="cloudAliases"
+        None, description="A list of cloud aliases for the actor.", alias="cloudAliases"
     )
-    country: Optional[str] = Field(None, description="The user's country.")
-    deleted: Optional[bool] = Field(None, description="Whether the user is deleted.")
-    department: Optional[str] = Field(None, description="The user's department.")
+    country: Optional[str] = Field(None, description="The actor's country.")
+    deleted: Optional[bool] = Field(None, description="Whether the actor is deleted.")
+    department: Optional[str] = Field(None, description="The actor's department.")
     display_name: Optional[str] = Field(
-        None, description="The user's friendly display name.", alias="displayName"
+        None, description="The actor's friendly display name.", alias="displayName"
     )
-    division: Optional[str] = Field(None, description="The user's division.")
+    division: Optional[str] = Field(None, description="The actor's division.")
     employment_type: Optional[str] = Field(
-        None, description="The user's employment type.", alias="employmentType"
+        None, description="The actor's employment type.", alias="employmentType"
     )
     end_date: Optional[Date] = Field(None, alias="endDate")
-    locality: Optional[str] = Field(None, description="The user's locality (city).")
+    locality: Optional[str] = Field(None, description="The actor's locality (city).")
     manager_display_name: Optional[str] = Field(
         None,
-        description="The user's manager's friendly display name.",
+        description="The actor's manager's friendly display name.",
         alias="managerDisplayName",
     )
     manager_id: Optional[str] = Field(
-        None, description="The Code42 user ID of the user's manager.", alias="managerId"
+        None,
+        description="The Code42 actor ID of the actor's manager.",
+        alias="managerId",
     )
     manager_username: Optional[str] = Field(
         None,
-        description="The Code42 username of the user's manager.",
+        description="The Code42 actorname of the actor's manager.",
         alias="managerUsername",
     )
     notes: Optional[str] = Field(
         None,
-        description="Notes about the user.",
+        description="Notes about the actor.",
         table=lambda f: f if f is None else Markdown(f),
     )
-    region: Optional[str] = Field(None, description="The user's region (state).")
+    region: Optional[str] = Field(None, description="The actor's region (state).")
     start_date: Optional[Date] = Field(None, alias="startDate")
     support_user: Optional[bool] = Field(
-        None, description="Whether the user is a support user.", alias="supportUser"
+        None, description="Whether the actor is a support actor.", alias="supportUser"
     )
     tenant_id: Optional[str] = Field(
         None, description="A unique tenant ID.", alias="tenantId"
     )
-    title: Optional[str] = Field(None, description="The user's job title.")
+    title: Optional[str] = Field(None, description="The actor's job title.")
     user_id: Optional[str] = Field(
-        None, description="A unique user ID.", alias="userId"
+        None, description="A unique actor ID.", alias="userId"
     )
-    username: Optional[str] = Field(None, description="The user's Code42 username.")
+    username: Optional[str] = Field(None, description="The actor's Code42 actorname.")
 
 
-class UserRiskProfilesPage(ResponseModel):
+class RiskProfilesPage(ResponseModel):
     """
-    A model representing a page of `UserRiskProfile` objects.
+    A model representing a page of `RiskProfile` objects.
 
     **Fields**:
 
-    * **total_count**: `int` The total count of all user risk profiles.
-    * **user_risk_profiles**: `List[UserRiskProfile]` The list of `n` number of user risk profiles
+    * **total_count**: `int` The total count of all risk profiles.
+    * **user_risk_profiles**: `List[RiskProfile]` The list of `n` number of risk profiles
                             retrieved from the query, where `n=page_size`.
     """
 
     total_count: Optional[int] = Field(
         None,
-        description="The total count of all user risk profiles.",
+        description="The total count of all risk profiles.",
         example=10,
         alias="totalCount",
     )
-    user_risk_profiles: Optional[List[UserRiskProfile]] = Field(
+    user_risk_profiles: Optional[List[RiskProfile]] = Field(
         None, alias="userRiskProfiles"
     )
 
 
-class QueryUserRiskProfilesRequest(Model):
+class QueryRiskProfilesRequest(Model):
     page: Optional[int]
     page_size: Optional[int]
     manager_id: Optional[str]
     title: Optional[str]
     division: Optional[str]
     department: Optional[str]
     employment_type: Optional[str]
@@ -140,29 +142,29 @@
     deleted: Optional[bool]
     support_user: Optional[bool]
 
     class Config:
         use_enum_values = True
 
 
-class UpdateUserRiskProfileRequest(Model):
+class UpdateRiskProfileRequest(Model):
     endDate: Optional[Date] = None
     notes: Optional[str] = Field(
         None,
-        description="Notes to add to the user risk profile.",
+        description="Notes to add to the risk profile.",
         example="These are my notes",
     )
     startDate: Optional[Date] = None
 
 
 class AddCloudAliasesRequest(Model):
     cloudAliases: Optional[List[str]] = None
     userId: Optional[str] = Field(
-        None, description="The ID of the user to add cloud aliases.", example="123"
+        None, description="The ID of the actor to add cloud aliases.", example="123"
     )
 
 
 class DeleteCloudAliasesRequest(Model):
     cloudAliases: Optional[List[str]] = None
     userId: Optional[str] = Field(
-        None, description="The ID of the user to delete cloud aliases.", example="123"
+        None, description="The ID of the actor to delete cloud aliases.", example="123"
     )
```

### Comparing `incydr-1.2.0/_incydr_sdk/users/client.py` & `incydr-2.0.0/_incydr_sdk/users/client.py`

 * *Files identical despite different names*

### Comparing `incydr-1.2.0/_incydr_sdk/users/models.py` & `incydr-2.0.0/_incydr_sdk/users/models.py`

 * *Files identical despite different names*

### Comparing `incydr-1.2.0/_incydr_sdk/watchlists/client.py` & `incydr-2.0.0/_incydr_sdk/watchlists/client.py`

 * *Files identical despite different names*

### Comparing `incydr-1.2.0/_incydr_sdk/watchlists/models/requests.py` & `incydr-2.0.0/_incydr_sdk/watchlists/models/requests.py`

 * *Files identical despite different names*

### Comparing `incydr-1.2.0/_incydr_sdk/watchlists/models/responses.py` & `incydr-2.0.0/_incydr_sdk/watchlists/models/responses.py`

 * *Files identical despite different names*

### Comparing `incydr-1.2.0/incydr/__init__.py` & `incydr-2.0.0/incydr/__init__.py`

 * *Files identical despite different names*

### Comparing `incydr-1.2.0/incydr/models.py` & `incydr-2.0.0/incydr/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+from _incydr_sdk.actors.models import Actor
+from _incydr_sdk.actors.models import ActorFamily
+from _incydr_sdk.actors.models import ActorsPage
 from _incydr_sdk.agents.models import Agent
 from _incydr_sdk.agents.models import AgentsPage
 from _incydr_sdk.alert_rules.models.response import RuleDetails
 from _incydr_sdk.alert_rules.models.response import RuleUser
 from _incydr_sdk.alert_rules.models.response import RuleUsersList
 from _incydr_sdk.alerts.models.alert import AlertDetails
 from _incydr_sdk.alerts.models.alert import AlertSummary
@@ -16,18 +19,20 @@
 from _incydr_sdk.devices.models import DevicesPage
 from _incydr_sdk.directory_groups.models import DirectoryGroup
 from _incydr_sdk.directory_groups.models import DirectoryGroupsPage
 from _incydr_sdk.file_events.models.event import FileEventV2
 from _incydr_sdk.file_events.models.event import User
 from _incydr_sdk.file_events.models.response import FileEventsPage
 from _incydr_sdk.file_events.models.response import SavedSearch
+from _incydr_sdk.risk_profiles.models import RiskProfile
+from _incydr_sdk.risk_profiles.models import RiskProfilesPage
+from _incydr_sdk.sessions.models.response import Session
+from _incydr_sdk.sessions.models.response import SessionsPage
 from _incydr_sdk.trusted_activities.models import TrustedActivitiesPage
 from _incydr_sdk.trusted_activities.models import TrustedActivity
-from _incydr_sdk.user_risk_profiles.models import UserRiskProfile
-from _incydr_sdk.user_risk_profiles.models import UserRiskProfilesPage
 from _incydr_sdk.users.models import Role
 from _incydr_sdk.users.models import UpdateRolesResponse
 from _incydr_sdk.users.models import UserRole
 from _incydr_sdk.users.models import UsersPage
 from _incydr_sdk.watchlists.models.responses import ExcludedUsersList
 from _incydr_sdk.watchlists.models.responses import IncludedDepartment
 from _incydr_sdk.watchlists.models.responses import IncludedDepartmentsList
@@ -36,14 +41,17 @@
 from _incydr_sdk.watchlists.models.responses import IncludedUsersList
 from _incydr_sdk.watchlists.models.responses import Watchlist
 from _incydr_sdk.watchlists.models.responses import WatchlistMembersList
 from _incydr_sdk.watchlists.models.responses import WatchlistsPage
 from _incydr_sdk.watchlists.models.responses import WatchlistUser
 
 __all__ = [
+    "Actor",
+    "ActorFamily",
+    "ActorsPage",
     "Agent",
     "AgentsPage",
     "AlertDetails",
     "AlertSummary",
     "AlertQueryPage",
     "Case",
     "CaseFileEvents",
@@ -58,14 +66,16 @@
     "UsersPage",
     "UserRole",
     "Role",
     "UpdateRolesResponse",
     "RuleUsersList",
     "RuleUser",
     "RuleDetails",
+    "Session",
+    "SessionsPage",
     "TrustedActivity",
     "TrustedActivitiesPage",
     "DepartmentsPage",
     "DirectoryGroupsPage",
     "DirectoryGroup",
     "Watchlist",
     "WatchlistsPage",
@@ -74,16 +84,16 @@
     "IncludedUsersList",
     "WatchlistUser",
     "IncludedDepartmentsList",
     "IncludedDepartment",
     "IncludedDirectoryGroupsList",
     "IncludedDirectoryGroup",
     "AuditEventsPage",
-    "UserRiskProfilesPage",
-    "UserRiskProfile",
+    "RiskProfilesPage",
+    "RiskProfile",
 ]
 
 
 __locals = locals()
 for __name in __all__:
     if not __name.startswith("__"):
         setattr(__locals[__name], "__module__", "incydr.models")  # noqa
```

### Comparing `incydr-1.2.0/incydr/enums/file_events.py` & `incydr-2.0.0/incydr/enums/file_events.py`

 * *Files identical despite different names*

### Comparing `incydr-1.2.0/LICENSE.txt` & `incydr-2.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `incydr-1.2.0/README.md` & `incydr-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `incydr-1.2.0/pyproject.toml` & `incydr-2.0.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 classifiers = [
   "Development Status :: 4 - Beta",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
+  "Programming Language :: Python :: 3.11",
+  "Programming Language :: Python :: 3.12",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
   "boltons",
   "requests",
   "requests-toolbelt",
```

### Comparing `incydr-1.2.0/PKG-INFO` & `incydr-2.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.3
 Name: incydr
-Version: 1.2.0
+Version: 2.0.0
 Summary: Code42's Incydr Python SDK
 Project-URL: Documentation, https://github.com/code42/incydr_python#readme
 Project-URL: Issues, https://github.com/code42/incydr_python/issues
 Project-URL: Source, https://github.com/code42/incydr_python/incydr
 Author-email: Code42 <integrations@code42.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
 Requires-Dist: boltons
 Requires-Dist: isodate
 Requires-Dist: pydantic[dotenv]==1.*
 Requires-Dist: python-dateutil
```

