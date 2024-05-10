# Comparing `tmp/owega-5.6.3.tar.gz` & `tmp/owega-5.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "owega-5.6.3.tar", last modified: Wed May  8 02:37:45 2024, max compression
+gzip compressed data, was "owega-5.6.4.tar", last modified: Fri May 10 10:32:35 2024, max compression
```

## Comparing `owega-5.6.3.tar` & `owega-5.6.4.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-08 02:37:45.573945 owega-5.6.3/
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      496 2024-04-17 02:21:38.000000 owega-5.6.3/LICENSE
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    15847 2024-05-08 02:37:45.572944 owega-5.6.3/PKG-INFO
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     5023 2024-04-17 02:21:38.000000 owega-5.6.3/README.md
-drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-08 02:37:45.570945 owega-5.6.3/owega/
-drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-08 02:37:45.571945 owega-5.6.3/owega/OweHandlers/
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      156 2024-04-27 12:05:16.000000 owega-5.6.3/owega/OweHandlers/__init__.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      980 2024-05-08 01:58:10.000000 owega-5.6.3/owega/OweHandlers/handle_add_sysmem.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1590 2024-05-08 01:58:10.000000 owega-5.6.3/owega/OweHandlers/handle_commands.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1185 2024-05-08 01:58:10.000000 owega-5.6.3/owega/OweHandlers/handle_context.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1601 2024-05-08 01:58:10.000000 owega-5.6.3/owega/OweHandlers/handle_del_sysmem.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1816 2024-05-08 01:58:10.000000 owega-5.6.3/owega/OweHandlers/handle_dinput.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     3457 2024-05-08 01:58:10.000000 owega-5.6.3/owega/OweHandlers/handle_edit.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1339 2024-05-08 01:58:10.000000 owega-5.6.3/owega/OweHandlers/handle_estimation.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     5059 2024-05-08 01:58:10.000000 owega-5.6.3/owega/OweHandlers/handle_finput.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1816 2024-05-08 01:58:10.000000 owega-5.6.3/owega/OweHandlers/handle_frequency.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      521 2024-05-08 01:58:10.000000 owega-5.6.3/owega/OweHandlers/handle_genconf.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      523 2024-05-08 01:58:10.000000 owega-5.6.3/owega/OweHandlers/handle_history.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     3310 2024-05-08 01:58:10.000000 owega-5.6.3/owega/OweHandlers/handle_image.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1118 2024-05-08 01:58:10.000000 owega-5.6.3/owega/OweHandlers/handle_load.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1698 2024-05-08 01:58:10.000000 owega-5.6.3/owega/OweHandlers/handle_model.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1791 2024-05-08 01:58:10.000000 owega-5.6.3/owega/OweHandlers/handle_presence.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      637 2024-05-08 01:58:10.000000 owega-5.6.3/owega/OweHandlers/handle_quit.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1090 2024-05-08 01:58:10.000000 owega-5.6.3/owega/OweHandlers/handle_save.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      945 2024-05-08 01:58:10.000000 owega-5.6.3/owega/OweHandlers/handle_system.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1739 2024-05-08 01:58:10.000000 owega-5.6.3/owega/OweHandlers/handle_temperature.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1404 2024-05-08 01:58:10.000000 owega-5.6.3/owega/OweHandlers/handle_tokens.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1556 2024-05-08 01:58:10.000000 owega-5.6.3/owega/OweHandlers/handle_top_p.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1245 2024-05-08 01:58:10.000000 owega-5.6.3/owega/OweHandlers/handle_tts.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     2407 2024-04-27 12:05:16.000000 owega-5.6.3/owega/OweHandlers/handlers.py
-drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-08 02:37:45.571945 owega-5.6.3/owega/OwegaFun/
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      873 2024-04-27 12:05:16.000000 owega-5.6.3/owega/OwegaFun/__init__.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     3867 2024-04-17 02:21:38.000000 owega-5.6.3/owega/OwegaFun/functions.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     4342 2024-04-27 12:05:16.000000 owega-5.6.3/owega/OwegaFun/longTermSouvenirs.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     5816 2024-04-27 12:05:16.000000 owega-5.6.3/owega/OwegaFun/utility.py
-drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-08 02:37:45.572944 owega-5.6.3/owega/OwegaSession/
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      100 2024-04-17 02:21:38.000000 owega-5.6.3/owega/OwegaSession/__init__.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     2763 2024-04-27 12:05:16.000000 owega-5.6.3/owega/OwegaSession/main_bottom_toolbar.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     5592 2024-04-27 12:05:16.000000 owega-5.6.3/owega/OwegaSession/promptsession.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      175 2024-05-08 01:58:10.000000 owega-5.6.3/owega/__init__.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       94 2024-04-17 02:21:38.000000 owega-5.6.3/owega/__main__.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     9227 2024-05-08 02:31:24.000000 owega-5.6.3/owega/ask.py
-drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-08 02:37:45.572944 owega-5.6.3/owega/changelog/
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       80 2024-04-27 12:05:16.000000 owega-5.6.3/owega/changelog/__init__.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    23840 2024-05-08 02:33:11.000000 owega-5.6.3/owega/changelog/changelog.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1534 2024-04-27 12:05:16.000000 owega-5.6.3/owega/changelog/changelogEntry.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     3315 2024-04-17 02:21:38.000000 owega-5.6.3/owega/changelog/version.py
-drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-08 02:37:45.572944 owega-5.6.3/owega/config/
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       86 2024-04-17 02:21:38.000000 owega-5.6.3/owega/config/__init__.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1810 2024-04-27 12:05:16.000000 owega-5.6.3/owega/config/baseConf.py
-drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-08 02:37:45.572944 owega-5.6.3/owega/conversation/
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       83 2024-04-17 02:21:38.000000 owega-5.6.3/owega/conversation/__init__.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    10105 2024-04-27 12:05:16.000000 owega-5.6.3/owega/conversation/conversation.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1417 2024-04-18 20:54:01.000000 owega-5.6.3/owega/getLogger.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       64 2024-04-17 02:21:38.000000 owega-5.6.3/owega/handlerBase.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      549 2024-04-17 02:21:38.000000 owega-5.6.3/owega/license.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    12103 2024-04-27 12:05:16.000000 owega-5.6.3/owega/owega.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     6111 2024-04-27 12:05:16.000000 owega-5.6.3/owega/utils.py
-drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-08 02:37:45.572944 owega-5.6.3/owega.egg-info/
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    15847 2024-05-08 02:37:45.000000 owega-5.6.3/owega.egg-info/PKG-INFO
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1656 2024-05-08 02:37:45.000000 owega-5.6.3/owega.egg-info/SOURCES.txt
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)        1 2024-05-08 02:37:45.000000 owega-5.6.3/owega.egg-info/dependency_links.txt
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       43 2024-05-08 02:37:45.000000 owega-5.6.3/owega.egg-info/entry_points.txt
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      156 2024-05-08 02:37:45.000000 owega-5.6.3/owega.egg-info/requires.txt
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)        6 2024-05-08 02:37:45.000000 owega-5.6.3/owega.egg-info/top_level.txt
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       90 2024-04-17 02:21:38.000000 owega-5.6.3/pyproject.toml
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       38 2024-05-08 02:37:45.573945 owega-5.6.3/setup.cfg
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     2082 2024-04-27 12:05:16.000000 owega-5.6.3/setup.py
+drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-10 10:32:35.541177 owega-5.6.4/
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      496 2024-04-17 02:21:38.000000 owega-5.6.4/LICENSE
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    15910 2024-05-10 10:32:35.541177 owega-5.6.4/PKG-INFO
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     5023 2024-04-17 02:21:38.000000 owega-5.6.4/README.md
+drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-10 10:32:35.539177 owega-5.6.4/owega/
+drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-10 10:32:35.540177 owega-5.6.4/owega/OweHandlers/
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      156 2024-04-27 12:05:16.000000 owega-5.6.4/owega/OweHandlers/__init__.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      980 2024-05-08 02:39:07.000000 owega-5.6.4/owega/OweHandlers/handle_add_sysmem.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1590 2024-05-08 02:39:07.000000 owega-5.6.4/owega/OweHandlers/handle_commands.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1185 2024-05-08 02:39:07.000000 owega-5.6.4/owega/OweHandlers/handle_context.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1601 2024-05-08 02:39:07.000000 owega-5.6.4/owega/OweHandlers/handle_del_sysmem.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1816 2024-05-08 02:39:07.000000 owega-5.6.4/owega/OweHandlers/handle_dinput.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     3457 2024-05-08 02:39:07.000000 owega-5.6.4/owega/OweHandlers/handle_edit.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1339 2024-05-08 02:39:07.000000 owega-5.6.4/owega/OweHandlers/handle_estimation.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     5059 2024-05-08 02:39:07.000000 owega-5.6.4/owega/OweHandlers/handle_finput.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1816 2024-05-08 02:39:07.000000 owega-5.6.4/owega/OweHandlers/handle_frequency.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      521 2024-05-08 02:39:07.000000 owega-5.6.4/owega/OweHandlers/handle_genconf.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      523 2024-05-08 02:39:07.000000 owega-5.6.4/owega/OweHandlers/handle_history.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     3310 2024-05-08 02:39:08.000000 owega-5.6.4/owega/OweHandlers/handle_image.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1118 2024-05-08 02:39:08.000000 owega-5.6.4/owega/OweHandlers/handle_load.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1698 2024-05-08 02:39:08.000000 owega-5.6.4/owega/OweHandlers/handle_model.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1791 2024-05-08 02:39:08.000000 owega-5.6.4/owega/OweHandlers/handle_presence.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      637 2024-05-08 02:39:08.000000 owega-5.6.4/owega/OweHandlers/handle_quit.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1090 2024-05-08 02:39:08.000000 owega-5.6.4/owega/OweHandlers/handle_save.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      945 2024-05-08 02:39:08.000000 owega-5.6.4/owega/OweHandlers/handle_system.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1739 2024-05-08 02:39:08.000000 owega-5.6.4/owega/OweHandlers/handle_temperature.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1404 2024-05-08 02:39:08.000000 owega-5.6.4/owega/OweHandlers/handle_tokens.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1556 2024-05-08 02:39:08.000000 owega-5.6.4/owega/OweHandlers/handle_top_p.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1245 2024-05-08 02:39:08.000000 owega-5.6.4/owega/OweHandlers/handle_tts.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     2407 2024-04-27 12:05:16.000000 owega-5.6.4/owega/OweHandlers/handlers.py
+drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-10 10:32:35.540177 owega-5.6.4/owega/OwegaFun/
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      873 2024-04-27 12:05:16.000000 owega-5.6.4/owega/OwegaFun/__init__.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     3867 2024-04-17 02:21:38.000000 owega-5.6.4/owega/OwegaFun/functions.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     4342 2024-04-27 12:05:16.000000 owega-5.6.4/owega/OwegaFun/longTermSouvenirs.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     5816 2024-04-27 12:05:16.000000 owega-5.6.4/owega/OwegaFun/utility.py
+drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-10 10:32:35.540177 owega-5.6.4/owega/OwegaSession/
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      100 2024-04-17 02:21:38.000000 owega-5.6.4/owega/OwegaSession/__init__.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     2763 2024-04-27 12:05:16.000000 owega-5.6.4/owega/OwegaSession/main_bottom_toolbar.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     5592 2024-04-27 12:05:16.000000 owega-5.6.4/owega/OwegaSession/promptsession.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      175 2024-05-08 02:39:08.000000 owega-5.6.4/owega/__init__.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       94 2024-04-17 02:21:38.000000 owega-5.6.4/owega/__main__.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     9363 2024-05-10 10:30:26.000000 owega-5.6.4/owega/ask.py
+drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-10 10:32:35.541177 owega-5.6.4/owega/changelog/
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       80 2024-04-27 12:05:16.000000 owega-5.6.4/owega/changelog/__init__.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    23992 2024-05-10 10:32:17.000000 owega-5.6.4/owega/changelog/changelog.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1534 2024-04-27 12:05:16.000000 owega-5.6.4/owega/changelog/changelogEntry.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     3315 2024-04-17 02:21:38.000000 owega-5.6.4/owega/changelog/version.py
+drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-10 10:32:35.541177 owega-5.6.4/owega/config/
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       86 2024-04-17 02:21:38.000000 owega-5.6.4/owega/config/__init__.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1810 2024-04-27 12:05:16.000000 owega-5.6.4/owega/config/baseConf.py
+drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-10 10:32:35.541177 owega-5.6.4/owega/conversation/
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       83 2024-04-17 02:21:38.000000 owega-5.6.4/owega/conversation/__init__.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    10105 2024-04-27 12:05:16.000000 owega-5.6.4/owega/conversation/conversation.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1418 2024-05-10 10:21:38.000000 owega-5.6.4/owega/getLogger.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       64 2024-04-17 02:21:38.000000 owega-5.6.4/owega/handlerBase.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      549 2024-04-17 02:21:38.000000 owega-5.6.4/owega/license.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    12103 2024-04-27 12:05:16.000000 owega-5.6.4/owega/owega.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     6111 2024-04-27 12:05:16.000000 owega-5.6.4/owega/utils.py
+drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-10 10:32:35.541177 owega-5.6.4/owega.egg-info/
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    15910 2024-05-10 10:32:35.000000 owega-5.6.4/owega.egg-info/PKG-INFO
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1656 2024-05-10 10:32:35.000000 owega-5.6.4/owega.egg-info/SOURCES.txt
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)        1 2024-05-10 10:32:35.000000 owega-5.6.4/owega.egg-info/dependency_links.txt
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       43 2024-05-10 10:32:35.000000 owega-5.6.4/owega.egg-info/entry_points.txt
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      156 2024-05-10 10:32:35.000000 owega-5.6.4/owega.egg-info/requires.txt
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)        6 2024-05-10 10:32:35.000000 owega-5.6.4/owega.egg-info/top_level.txt
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       90 2024-04-17 02:21:38.000000 owega-5.6.4/pyproject.toml
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       38 2024-05-10 10:32:35.541177 owega-5.6.4/setup.cfg
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     2082 2024-04-27 12:05:16.000000 owega-5.6.4/setup.py
```

### Comparing `owega-5.6.3/PKG-INFO` & `owega-5.6.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: owega
-Version: 5.6.3
+Version: 5.6.4
 Summary: A command-line interface for conversing with GPT models (from OpenAI)
 Home-page: https://git.pyrokinesis.fr/darkgeem/owega
 Author: darkgeem
 Author-email: darkgeem@pyrokinesis.fr
 License: WTFPL
 Project-URL: Source, https://git.pyrokinesis.fr/darkgeem/owega
 Project-URL: Support, https://discord.gg/KdRmyRrA48
@@ -135,15 +135,15 @@
 See ΦωΦ in action!
 
 [![asciicast](https://asciinema.org/a/613143.png)](https://asciinema.org/a/613143)
 
 
 ## CHANGELOG: 
 ```
-OWEGA v5.6.3 CHANGELOG:
+OWEGA v5.6.4 CHANGELOG:
 
 
 2.0.0: WTFPL license
 2.0.1: added genconf command
 
 2.1.0: added file_input command
 2.1.1: added file_input in help command
@@ -359,8 +359,9 @@
 5.6.0: Added basic support for Chub's API
        (chub mars, mercury, mixtral)
        Also, Mi(s/x)tral support is no more in beta :D
 5.6.1: Added extensive logging for errors.
 5.6.2: Added terminal title status :3
 5.6.3: Fixes config's api_key not being used.
        Better docstrings on handlers.
+5.6.4: Fix for ask.ask() crashing if OPENAI_API_KEY isn't set.
 ```
```

### Comparing `owega-5.6.3/README.md` & `owega-5.6.4/README.md`

 * *Files identical despite different names*

### Comparing `owega-5.6.3/owega/OweHandlers/handle_add_sysmem.py` & `owega-5.6.4/owega/OweHandlers/handle_add_sysmem.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.3/owega/OweHandlers/handle_commands.py` & `owega-5.6.4/owega/OweHandlers/handle_commands.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.3/owega/OweHandlers/handle_context.py` & `owega-5.6.4/owega/OweHandlers/handle_context.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.3/owega/OweHandlers/handle_del_sysmem.py` & `owega-5.6.4/owega/OweHandlers/handle_del_sysmem.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.3/owega/OweHandlers/handle_dinput.py` & `owega-5.6.4/owega/OweHandlers/handle_dinput.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.3/owega/OweHandlers/handle_edit.py` & `owega-5.6.4/owega/OweHandlers/handle_edit.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.3/owega/OweHandlers/handle_estimation.py` & `owega-5.6.4/owega/OweHandlers/handle_estimation.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.3/owega/OweHandlers/handle_finput.py` & `owega-5.6.4/owega/OweHandlers/handle_finput.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.3/owega/OweHandlers/handle_frequency.py` & `owega-5.6.4/owega/OweHandlers/handle_frequency.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.3/owega/OweHandlers/handle_genconf.py` & `owega-5.6.4/owega/OweHandlers/handle_genconf.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.3/owega/OweHandlers/handle_history.py` & `owega-5.6.4/owega/OweHandlers/handle_history.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.3/owega/OweHandlers/handle_image.py` & `owega-5.6.4/owega/OweHandlers/handle_image.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.3/owega/OweHandlers/handle_load.py` & `owega-5.6.4/owega/OweHandlers/handle_load.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.3/owega/OweHandlers/handle_model.py` & `owega-5.6.4/owega/OweHandlers/handle_model.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.3/owega/OweHandlers/handle_presence.py` & `owega-5.6.4/owega/OweHandlers/handle_presence.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.3/owega/OweHandlers/handle_quit.py` & `owega-5.6.4/owega/OweHandlers/handle_quit.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.3/owega/OweHandlers/handle_save.py` & `owega-5.6.4/owega/OweHandlers/handle_save.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.3/owega/OweHandlers/handle_system.py` & `owega-5.6.4/owega/OweHandlers/handle_system.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.3/owega/OweHandlers/handle_temperature.py` & `owega-5.6.4/owega/OweHandlers/handle_temperature.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.3/owega/OweHandlers/handle_tokens.py` & `owega-5.6.4/owega/OweHandlers/handle_tokens.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.3/owega/OweHandlers/handle_top_p.py` & `owega-5.6.4/owega/OweHandlers/handle_top_p.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.3/owega/OweHandlers/handle_tts.py` & `owega-5.6.4/owega/OweHandlers/handle_tts.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.3/owega/OweHandlers/handlers.py` & `owega-5.6.4/owega/OweHandlers/handlers.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.3/owega/OwegaFun/__init__.py` & `owega-5.6.4/owega/OwegaFun/__init__.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.3/owega/OwegaFun/functions.py` & `owega-5.6.4/owega/OwegaFun/functions.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.3/owega/OwegaFun/longTermSouvenirs.py` & `owega-5.6.4/owega/OwegaFun/longTermSouvenirs.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.3/owega/OwegaFun/utility.py` & `owega-5.6.4/owega/OwegaFun/utility.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.3/owega/OwegaSession/main_bottom_toolbar.py` & `owega-5.6.4/owega/OwegaSession/main_bottom_toolbar.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.3/owega/OwegaSession/promptsession.py` & `owega-5.6.4/owega/OwegaSession/promptsession.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.3/owega/ask.py` & `owega-5.6.4/owega/ask.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,15 +69,19 @@
     is_chub = False
     if model.startswith('chub-'):
         model = model[5:]
         is_chub = True
     elif ("mistral" in model) or ("mixtral" in model):
         is_mistral = True
 
-    client = openai.OpenAI()
+    try:
+        client = openai.OpenAI()
+    except openai.OpenAIError:
+        # fix for key not set by $OPENAI_API_KEY
+        client = openai.OpenAI(api_key='')
 
     if (baseConf.get('api_key', '')):
         client.api_key = baseConf.get('api_key', '')
 
     if is_chub:
         logger.info(f"Using Chub's API for model: {model}")
         if model in ["mars", "asha"]:
```

### Comparing `owega-5.6.3/owega/changelog/changelog.py` & `owega-5.6.4/owega/changelog/changelog.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,14 +13,18 @@
         self.version = Version(0, 0, 0)
         self.initLogs()
         self.genLog()
 
     def initLogs(self):
         """Fill the changelog."""
         self.logs.append(
+            ChangelogEntry(5, 6, 4)
+            .addLine("Fix for ask.ask() crashing if OPENAI_API_KEY isn't set.")
+        )
+        self.logs.append(
             ChangelogEntry(5, 6, 3)
             .addLine("Fixes config's api_key not being used.")
             .addLine("Better docstrings on handlers.")
         )
         self.logs.append(
             ChangelogEntry(5, 6, 2)
             .addLine("Added terminal title status :3")
```

### Comparing `owega-5.6.3/owega/changelog/changelogEntry.py` & `owega-5.6.4/owega/changelog/changelogEntry.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.3/owega/changelog/version.py` & `owega-5.6.4/owega/changelog/version.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.3/owega/config/baseConf.py` & `owega-5.6.4/owega/config/baseConf.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.3/owega/conversation/conversation.py` & `owega-5.6.4/owega/conversation/conversation.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.3/owega/getLogger.py` & `owega-5.6.4/owega/getLogger.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,29 +13,29 @@
         'rst': '\x1b[0m'
     }
     logfmtstr = f'[{clr["mag"]}%(asctime)s{clr["rst"]}]'
     logfmtstr += f' [{clr["yel"]}%(filename)s{clr["rst"]}'
     logfmtstr += f':{clr["cyn"]}%(lineno)s{clr["rst"]}]'
     logfmtstr += f' [{clr["red"]}%(name)s{clr["rst"]}]'
     logfmtstr += f' [{clr["blu"]}%(levelname)s{clr["rst"]}]'
-    logfmtstr += f': %(message)s'
+    logfmtstr += ': %(message)s'
     if not color:
         for esc in clr.values():
             logfmtstr = logfmtstr.replace(esc, '')
     return logging.Formatter(logfmtstr)
 
 
 def getLoggerFile():
     user = os.getenv('USER')
     loggerFile = f'/tmp/{user}.owega.log'
     return loggerFile
 
 
 def getLogger(name, debug: bool = False):
-    user = os.getenv('USER')
+    # user = os.getenv('USER')
     loggerFile = getLoggerFile()
     logger = logging.getLogger(name)
 
     consHand = logging.StreamHandler()
     if debug:
         consHand.setLevel(logging.DEBUG)
     else:
```

### Comparing `owega-5.6.3/owega/license.py` & `owega-5.6.4/owega/license.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.3/owega/owega.py` & `owega-5.6.4/owega/owega.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.3/owega/utils.py` & `owega-5.6.4/owega/utils.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.3/owega.egg-info/PKG-INFO` & `owega-5.6.4/owega.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: owega
-Version: 5.6.3
+Version: 5.6.4
 Summary: A command-line interface for conversing with GPT models (from OpenAI)
 Home-page: https://git.pyrokinesis.fr/darkgeem/owega
 Author: darkgeem
 Author-email: darkgeem@pyrokinesis.fr
 License: WTFPL
 Project-URL: Source, https://git.pyrokinesis.fr/darkgeem/owega
 Project-URL: Support, https://discord.gg/KdRmyRrA48
@@ -135,15 +135,15 @@
 See ΦωΦ in action!
 
 [![asciicast](https://asciinema.org/a/613143.png)](https://asciinema.org/a/613143)
 
 
 ## CHANGELOG: 
 ```
-OWEGA v5.6.3 CHANGELOG:
+OWEGA v5.6.4 CHANGELOG:
 
 
 2.0.0: WTFPL license
 2.0.1: added genconf command
 
 2.1.0: added file_input command
 2.1.1: added file_input in help command
@@ -359,8 +359,9 @@
 5.6.0: Added basic support for Chub's API
        (chub mars, mercury, mixtral)
        Also, Mi(s/x)tral support is no more in beta :D
 5.6.1: Added extensive logging for errors.
 5.6.2: Added terminal title status :3
 5.6.3: Fixes config's api_key not being used.
        Better docstrings on handlers.
+5.6.4: Fix for ask.ask() crashing if OPENAI_API_KEY isn't set.
 ```
```

### Comparing `owega-5.6.3/owega.egg-info/SOURCES.txt` & `owega-5.6.4/owega.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `owega-5.6.3/setup.py` & `owega-5.6.4/setup.py`

 * *Files identical despite different names*

