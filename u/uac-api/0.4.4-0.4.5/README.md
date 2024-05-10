# Comparing `tmp/uac-api-0.4.4.tar.gz` & `tmp/uac-api-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uac-api-0.4.4.tar", last modified: Wed May  8 05:35:20 2024, max compression
+gzip compressed data, was "uac-api-0.4.5.tar", last modified: Fri May 10 17:12:35 2024, max compression
```

## Comparing `uac-api-0.4.4.tar` & `uac-api-0.4.5.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-05-08 05:35:20.082136 uac-api-0.4.4/
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)    18579 2024-05-08 05:35:20.081874 uac-api-0.4.4/PKG-INFO
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)    18142 2024-05-04 05:41:22.000000 uac-api-0.4.4/README.md
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-04-26 03:33:40.000000 uac-api-0.4.4/pyproject.toml
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)       38 2024-05-08 05:35:20.082189 uac-api-0.4.4/setup.cfg
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      985 2024-05-04 04:48:08.000000 uac-api-0.4.4/setup.py
-drwxr-xr-x   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-05-08 05:35:20.079264 uac-api-0.4.4/uac_api/
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     8893 2024-05-08 05:22:05.000000 uac-api-0.4.4/uac_api/__init__.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     9357 2024-04-29 16:35:47.000000 uac-api-0.4.4/uac_api/agents.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     1192 2024-04-26 03:33:40.000000 uac-api-0.4.4/uac_api/audits.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)    10489 2024-04-29 13:49:08.000000 uac-api-0.4.4/uac_api/bundles.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2107 2024-04-29 17:20:04.000000 uac-api-0.4.4/uac_api/business_services.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     4997 2024-04-26 03:33:40.000000 uac-api-0.4.4/uac_api/calendars.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      402 2024-04-26 03:33:40.000000 uac-api-0.4.4/uac_api/cluster_nodes.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     9129 2024-04-29 13:50:56.000000 uac-api-0.4.4/uac_api/connections.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     3014 2024-04-29 18:48:08.000000 uac-api-0.4.4/uac_api/credentials.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     3442 2024-04-30 02:41:31.000000 uac-api-0.4.4/uac_api/custom_days.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     1895 2024-04-29 13:46:36.000000 uac-api-0.4.4/uac_api/email_templates.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      558 2024-04-29 13:47:11.000000 uac-api-0.4.4/uac_api/ldap.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      278 2024-05-08 03:14:21.000000 uac-api-0.4.4/uac_api/metrics.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2103 2024-04-29 13:47:38.000000 uac-api-0.4.4/uac_api/oauth_clients.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     1935 2024-04-29 13:48:02.000000 uac-api-0.4.4/uac_api/oms_servers.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)    14604 2024-05-06 19:19:54.000000 uac-api-0.4.4/uac_api/payload.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     1107 2024-05-01 04:54:15.000000 uac-api-0.4.4/uac_api/properties.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     1375 2024-05-01 05:59:17.000000 uac-api-0.4.4/uac_api/reports.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     1790 2024-04-29 13:50:06.000000 uac-api-0.4.4/uac_api/scripts.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     1440 2024-05-08 03:58:02.000000 uac-api-0.4.4/uac_api/server_operations.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2615 2024-04-29 13:50:28.000000 uac-api-0.4.4/uac_api/simulations.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      305 2024-04-26 03:33:40.000000 uac-api-0.4.4/uac_api/system.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)    45039 2024-05-03 19:21:36.000000 uac-api-0.4.4/uac_api/task_instances.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)    10686 2024-05-06 19:27:09.000000 uac-api-0.4.4/uac_api/tasks.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     6774 2024-05-01 07:18:22.000000 uac-api-0.4.4/uac_api/triggers.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2493 2024-04-29 13:52:45.000000 uac-api-0.4.4/uac_api/universal_event_templates.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2233 2024-04-26 03:33:40.000000 uac-api-0.4.4/uac_api/universal_events.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     5719 2024-05-08 05:31:59.000000 uac-api-0.4.4/uac_api/universal_templates.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     1804 2024-04-29 13:53:42.000000 uac-api-0.4.4/uac_api/user_groups.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     4312 2024-05-01 04:31:22.000000 uac-api-0.4.4/uac_api/users.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     7831 2024-05-05 22:44:01.000000 uac-api-0.4.4/uac_api/utils.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     3831 2024-04-29 13:54:30.000000 uac-api-0.4.4/uac_api/variables.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     3378 2024-05-01 06:36:43.000000 uac-api-0.4.4/uac_api/virtual_resources.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     4287 2024-04-29 13:55:16.000000 uac-api-0.4.4/uac_api/webhooks.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)    10350 2024-05-04 05:17:55.000000 uac-api-0.4.4/uac_api/workflows.py
-drwxr-xr-x   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-05-08 05:35:20.081524 uac-api-0.4.4/uac_api.egg-info/
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)    18579 2024-05-08 05:35:20.000000 uac-api-0.4.4/uac_api.egg-info/PKG-INFO
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      972 2024-05-08 05:35:20.000000 uac-api-0.4.4/uac_api.egg-info/SOURCES.txt
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        1 2024-05-08 05:35:20.000000 uac-api-0.4.4/uac_api.egg-info/dependency_links.txt
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)       18 2024-05-08 05:35:20.000000 uac-api-0.4.4/uac_api.egg-info/requires.txt
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        8 2024-05-08 05:35:20.000000 uac-api-0.4.4/uac_api.egg-info/top_level.txt
+drwxr-xr-x   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-05-10 17:12:35.163651 uac-api-0.4.5/
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)    18579 2024-05-10 17:12:35.163415 uac-api-0.4.5/PKG-INFO
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)    18142 2024-05-04 05:41:22.000000 uac-api-0.4.5/README.md
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-04-26 03:33:40.000000 uac-api-0.4.5/pyproject.toml
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)       38 2024-05-10 17:12:35.163699 uac-api-0.4.5/setup.cfg
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      985 2024-05-04 04:48:08.000000 uac-api-0.4.5/setup.py
+drwxr-xr-x   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-05-10 17:12:35.160784 uac-api-0.4.5/uac_api/
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     8893 2024-05-10 17:11:39.000000 uac-api-0.4.5/uac_api/__init__.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     9357 2024-04-29 16:35:47.000000 uac-api-0.4.5/uac_api/agents.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     1192 2024-04-26 03:33:40.000000 uac-api-0.4.5/uac_api/audits.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)    10489 2024-04-29 13:49:08.000000 uac-api-0.4.5/uac_api/bundles.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2107 2024-04-29 17:20:04.000000 uac-api-0.4.5/uac_api/business_services.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     4997 2024-04-26 03:33:40.000000 uac-api-0.4.5/uac_api/calendars.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      402 2024-04-26 03:33:40.000000 uac-api-0.4.5/uac_api/cluster_nodes.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     9129 2024-04-29 13:50:56.000000 uac-api-0.4.5/uac_api/connections.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     3014 2024-04-29 18:48:08.000000 uac-api-0.4.5/uac_api/credentials.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     3442 2024-04-30 02:41:31.000000 uac-api-0.4.5/uac_api/custom_days.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     1895 2024-04-29 13:46:36.000000 uac-api-0.4.5/uac_api/email_templates.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      558 2024-04-29 13:47:11.000000 uac-api-0.4.5/uac_api/ldap.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      278 2024-05-08 03:14:21.000000 uac-api-0.4.5/uac_api/metrics.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2103 2024-04-29 13:47:38.000000 uac-api-0.4.5/uac_api/oauth_clients.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     1935 2024-04-29 13:48:02.000000 uac-api-0.4.5/uac_api/oms_servers.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)    14604 2024-05-06 19:19:54.000000 uac-api-0.4.5/uac_api/payload.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     1107 2024-05-01 04:54:15.000000 uac-api-0.4.5/uac_api/properties.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     1375 2024-05-01 05:59:17.000000 uac-api-0.4.5/uac_api/reports.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     1790 2024-04-29 13:50:06.000000 uac-api-0.4.5/uac_api/scripts.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     1440 2024-05-08 03:58:02.000000 uac-api-0.4.5/uac_api/server_operations.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2615 2024-04-29 13:50:28.000000 uac-api-0.4.5/uac_api/simulations.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      305 2024-04-26 03:33:40.000000 uac-api-0.4.5/uac_api/system.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)    45039 2024-05-03 19:21:36.000000 uac-api-0.4.5/uac_api/task_instances.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)    10686 2024-05-06 19:27:09.000000 uac-api-0.4.5/uac_api/tasks.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     6774 2024-05-01 07:18:22.000000 uac-api-0.4.5/uac_api/triggers.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2493 2024-04-29 13:52:45.000000 uac-api-0.4.5/uac_api/universal_event_templates.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2233 2024-04-26 03:33:40.000000 uac-api-0.4.5/uac_api/universal_events.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     5719 2024-05-08 05:31:59.000000 uac-api-0.4.5/uac_api/universal_templates.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     1804 2024-04-29 13:53:42.000000 uac-api-0.4.5/uac_api/user_groups.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     4312 2024-05-01 04:31:22.000000 uac-api-0.4.5/uac_api/users.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     7831 2024-05-05 22:44:01.000000 uac-api-0.4.5/uac_api/utils.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     3831 2024-04-29 13:54:30.000000 uac-api-0.4.5/uac_api/variables.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     3378 2024-05-01 06:36:43.000000 uac-api-0.4.5/uac_api/virtual_resources.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     4287 2024-04-29 13:55:16.000000 uac-api-0.4.5/uac_api/webhooks.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)    10350 2024-05-04 05:17:55.000000 uac-api-0.4.5/uac_api/workflows.py
+drwxr-xr-x   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-05-10 17:12:35.163038 uac-api-0.4.5/uac_api.egg-info/
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)    18579 2024-05-10 17:12:35.000000 uac-api-0.4.5/uac_api.egg-info/PKG-INFO
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      972 2024-05-10 17:12:35.000000 uac-api-0.4.5/uac_api.egg-info/SOURCES.txt
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        1 2024-05-10 17:12:35.000000 uac-api-0.4.5/uac_api.egg-info/dependency_links.txt
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)       18 2024-05-10 17:12:35.000000 uac-api-0.4.5/uac_api.egg-info/requires.txt
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        8 2024-05-10 17:12:35.000000 uac-api-0.4.5/uac_api.egg-info/top_level.txt
```

### Comparing `uac-api-0.4.4/PKG-INFO` & `uac-api-0.4.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uac-api
-Version: 0.4.4
+Version: 0.4.5
 Summary: A Python wrapper for the Stonebranch UAC API
 Home-page: https://github.com/gomleksiz/uac-api
 Author: Stonebranch
 Author-email: huseyim@gmail.com
 License: CC BY-NC 4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `uac-api-0.4.4/README.md` & `uac-api-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `uac-api-0.4.4/setup.py` & `uac-api-0.4.5/setup.py`

 * *Files identical despite different names*

### Comparing `uac-api-0.4.4/uac_api/__init__.py` & `uac-api-0.4.5/uac_api/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 from .email_templates import EmailTemplates
 from .oauth_clients import OAuthClients
 from .calendars import Calendars
 from .universal_templates import UniversalTemplates
 from .utils import strip_url, filter_secrets
 import logging
 
-__version__ = "0.4.4"
+__version__ = "0.4.5"
 
 class UniversalController():
     def __init__(self, base_url, credential=None, token=None, ssl_verify=True, logger=None, headers=None) -> None:
         if logger is None:
             logger = logging.getLogger(__name__)
             logger.setLevel(logging.INFO)
             logger.addHandler(logging.StreamHandler())
```

### Comparing `uac-api-0.4.4/uac_api/agents.py` & `uac-api-0.4.5/uac_api/agents.py`

 * *Files identical despite different names*

### Comparing `uac-api-0.4.4/uac_api/audits.py` & `uac-api-0.4.5/uac_api/audits.py`

 * *Files identical despite different names*

### Comparing `uac-api-0.4.4/uac_api/bundles.py` & `uac-api-0.4.5/uac_api/bundles.py`

 * *Files identical despite different names*

### Comparing `uac-api-0.4.4/uac_api/business_services.py` & `uac-api-0.4.5/uac_api/business_services.py`

 * *Files identical despite different names*

### Comparing `uac-api-0.4.4/uac_api/calendars.py` & `uac-api-0.4.5/uac_api/calendars.py`

 * *Files identical despite different names*

### Comparing `uac-api-0.4.4/uac_api/connections.py` & `uac-api-0.4.5/uac_api/connections.py`

 * *Files identical despite different names*

### Comparing `uac-api-0.4.4/uac_api/credentials.py` & `uac-api-0.4.5/uac_api/credentials.py`

 * *Files identical despite different names*

### Comparing `uac-api-0.4.4/uac_api/custom_days.py` & `uac-api-0.4.5/uac_api/custom_days.py`

 * *Files identical despite different names*

### Comparing `uac-api-0.4.4/uac_api/email_templates.py` & `uac-api-0.4.5/uac_api/email_templates.py`

 * *Files identical despite different names*

### Comparing `uac-api-0.4.4/uac_api/ldap.py` & `uac-api-0.4.5/uac_api/ldap.py`

 * *Files identical despite different names*

### Comparing `uac-api-0.4.4/uac_api/oauth_clients.py` & `uac-api-0.4.5/uac_api/oauth_clients.py`

 * *Files identical despite different names*

### Comparing `uac-api-0.4.4/uac_api/oms_servers.py` & `uac-api-0.4.5/uac_api/oms_servers.py`

 * *Files identical despite different names*

### Comparing `uac-api-0.4.4/uac_api/payload.py` & `uac-api-0.4.5/uac_api/payload.py`

 * *Files identical despite different names*

### Comparing `uac-api-0.4.4/uac_api/properties.py` & `uac-api-0.4.5/uac_api/properties.py`

 * *Files identical despite different names*

### Comparing `uac-api-0.4.4/uac_api/reports.py` & `uac-api-0.4.5/uac_api/reports.py`

 * *Files identical despite different names*

### Comparing `uac-api-0.4.4/uac_api/scripts.py` & `uac-api-0.4.5/uac_api/scripts.py`

 * *Files identical despite different names*

### Comparing `uac-api-0.4.4/uac_api/server_operations.py` & `uac-api-0.4.5/uac_api/server_operations.py`

 * *Files identical despite different names*

### Comparing `uac-api-0.4.4/uac_api/simulations.py` & `uac-api-0.4.5/uac_api/simulations.py`

 * *Files identical despite different names*

### Comparing `uac-api-0.4.4/uac_api/task_instances.py` & `uac-api-0.4.5/uac_api/task_instances.py`

 * *Files identical despite different names*

### Comparing `uac-api-0.4.4/uac_api/tasks.py` & `uac-api-0.4.5/uac_api/tasks.py`

 * *Files identical despite different names*

### Comparing `uac-api-0.4.4/uac_api/triggers.py` & `uac-api-0.4.5/uac_api/triggers.py`

 * *Files identical despite different names*

### Comparing `uac-api-0.4.4/uac_api/universal_event_templates.py` & `uac-api-0.4.5/uac_api/universal_event_templates.py`

 * *Files identical despite different names*

### Comparing `uac-api-0.4.4/uac_api/universal_events.py` & `uac-api-0.4.5/uac_api/universal_events.py`

 * *Files identical despite different names*

### Comparing `uac-api-0.4.4/uac_api/universal_templates.py` & `uac-api-0.4.5/uac_api/universal_templates.py`

 * *Files identical despite different names*

### Comparing `uac-api-0.4.4/uac_api/user_groups.py` & `uac-api-0.4.5/uac_api/user_groups.py`

 * *Files identical despite different names*

### Comparing `uac-api-0.4.4/uac_api/users.py` & `uac-api-0.4.5/uac_api/users.py`

 * *Files identical despite different names*

### Comparing `uac-api-0.4.4/uac_api/utils.py` & `uac-api-0.4.5/uac_api/utils.py`

 * *Files identical despite different names*

### Comparing `uac-api-0.4.4/uac_api/variables.py` & `uac-api-0.4.5/uac_api/variables.py`

 * *Files identical despite different names*

### Comparing `uac-api-0.4.4/uac_api/virtual_resources.py` & `uac-api-0.4.5/uac_api/virtual_resources.py`

 * *Files identical despite different names*

### Comparing `uac-api-0.4.4/uac_api/webhooks.py` & `uac-api-0.4.5/uac_api/webhooks.py`

 * *Files identical despite different names*

### Comparing `uac-api-0.4.4/uac_api/workflows.py` & `uac-api-0.4.5/uac_api/workflows.py`

 * *Files identical despite different names*

### Comparing `uac-api-0.4.4/uac_api.egg-info/PKG-INFO` & `uac-api-0.4.5/uac_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uac-api
-Version: 0.4.4
+Version: 0.4.5
 Summary: A Python wrapper for the Stonebranch UAC API
 Home-page: https://github.com/gomleksiz/uac-api
 Author: Stonebranch
 Author-email: huseyim@gmail.com
 License: CC BY-NC 4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `uac-api-0.4.4/uac_api.egg-info/SOURCES.txt` & `uac-api-0.4.5/uac_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

