# Comparing `tmp/owega-5.6.4.tar.gz` & `tmp/owega-5.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "owega-5.6.4.tar", last modified: Fri May 10 10:32:35 2024, max compression
+gzip compressed data, was "owega-5.7.0.tar", last modified: Fri May 10 13:38:29 2024, max compression
```

## Comparing `owega-5.6.4.tar` & `owega-5.7.0.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-10 10:32:35.541177 owega-5.6.4/
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      496 2024-04-17 02:21:38.000000 owega-5.6.4/LICENSE
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    15910 2024-05-10 10:32:35.541177 owega-5.6.4/PKG-INFO
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     5023 2024-04-17 02:21:38.000000 owega-5.6.4/README.md
-drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-10 10:32:35.539177 owega-5.6.4/owega/
-drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-10 10:32:35.540177 owega-5.6.4/owega/OweHandlers/
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      156 2024-04-27 12:05:16.000000 owega-5.6.4/owega/OweHandlers/__init__.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      980 2024-05-08 02:39:07.000000 owega-5.6.4/owega/OweHandlers/handle_add_sysmem.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1590 2024-05-08 02:39:07.000000 owega-5.6.4/owega/OweHandlers/handle_commands.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1185 2024-05-08 02:39:07.000000 owega-5.6.4/owega/OweHandlers/handle_context.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1601 2024-05-08 02:39:07.000000 owega-5.6.4/owega/OweHandlers/handle_del_sysmem.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1816 2024-05-08 02:39:07.000000 owega-5.6.4/owega/OweHandlers/handle_dinput.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     3457 2024-05-08 02:39:07.000000 owega-5.6.4/owega/OweHandlers/handle_edit.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1339 2024-05-08 02:39:07.000000 owega-5.6.4/owega/OweHandlers/handle_estimation.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     5059 2024-05-08 02:39:07.000000 owega-5.6.4/owega/OweHandlers/handle_finput.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1816 2024-05-08 02:39:07.000000 owega-5.6.4/owega/OweHandlers/handle_frequency.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      521 2024-05-08 02:39:07.000000 owega-5.6.4/owega/OweHandlers/handle_genconf.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      523 2024-05-08 02:39:07.000000 owega-5.6.4/owega/OweHandlers/handle_history.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     3310 2024-05-08 02:39:08.000000 owega-5.6.4/owega/OweHandlers/handle_image.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1118 2024-05-08 02:39:08.000000 owega-5.6.4/owega/OweHandlers/handle_load.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1698 2024-05-08 02:39:08.000000 owega-5.6.4/owega/OweHandlers/handle_model.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1791 2024-05-08 02:39:08.000000 owega-5.6.4/owega/OweHandlers/handle_presence.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      637 2024-05-08 02:39:08.000000 owega-5.6.4/owega/OweHandlers/handle_quit.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1090 2024-05-08 02:39:08.000000 owega-5.6.4/owega/OweHandlers/handle_save.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      945 2024-05-08 02:39:08.000000 owega-5.6.4/owega/OweHandlers/handle_system.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1739 2024-05-08 02:39:08.000000 owega-5.6.4/owega/OweHandlers/handle_temperature.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1404 2024-05-08 02:39:08.000000 owega-5.6.4/owega/OweHandlers/handle_tokens.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1556 2024-05-08 02:39:08.000000 owega-5.6.4/owega/OweHandlers/handle_top_p.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1245 2024-05-08 02:39:08.000000 owega-5.6.4/owega/OweHandlers/handle_tts.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     2407 2024-04-27 12:05:16.000000 owega-5.6.4/owega/OweHandlers/handlers.py
-drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-10 10:32:35.540177 owega-5.6.4/owega/OwegaFun/
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      873 2024-04-27 12:05:16.000000 owega-5.6.4/owega/OwegaFun/__init__.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     3867 2024-04-17 02:21:38.000000 owega-5.6.4/owega/OwegaFun/functions.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     4342 2024-04-27 12:05:16.000000 owega-5.6.4/owega/OwegaFun/longTermSouvenirs.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     5816 2024-04-27 12:05:16.000000 owega-5.6.4/owega/OwegaFun/utility.py
-drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-10 10:32:35.540177 owega-5.6.4/owega/OwegaSession/
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      100 2024-04-17 02:21:38.000000 owega-5.6.4/owega/OwegaSession/__init__.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     2763 2024-04-27 12:05:16.000000 owega-5.6.4/owega/OwegaSession/main_bottom_toolbar.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     5592 2024-04-27 12:05:16.000000 owega-5.6.4/owega/OwegaSession/promptsession.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      175 2024-05-08 02:39:08.000000 owega-5.6.4/owega/__init__.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       94 2024-04-17 02:21:38.000000 owega-5.6.4/owega/__main__.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     9363 2024-05-10 10:30:26.000000 owega-5.6.4/owega/ask.py
-drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-10 10:32:35.541177 owega-5.6.4/owega/changelog/
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       80 2024-04-27 12:05:16.000000 owega-5.6.4/owega/changelog/__init__.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    23992 2024-05-10 10:32:17.000000 owega-5.6.4/owega/changelog/changelog.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1534 2024-04-27 12:05:16.000000 owega-5.6.4/owega/changelog/changelogEntry.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     3315 2024-04-17 02:21:38.000000 owega-5.6.4/owega/changelog/version.py
-drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-10 10:32:35.541177 owega-5.6.4/owega/config/
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       86 2024-04-17 02:21:38.000000 owega-5.6.4/owega/config/__init__.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1810 2024-04-27 12:05:16.000000 owega-5.6.4/owega/config/baseConf.py
-drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-10 10:32:35.541177 owega-5.6.4/owega/conversation/
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       83 2024-04-17 02:21:38.000000 owega-5.6.4/owega/conversation/__init__.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    10105 2024-04-27 12:05:16.000000 owega-5.6.4/owega/conversation/conversation.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1418 2024-05-10 10:21:38.000000 owega-5.6.4/owega/getLogger.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       64 2024-04-17 02:21:38.000000 owega-5.6.4/owega/handlerBase.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      549 2024-04-17 02:21:38.000000 owega-5.6.4/owega/license.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    12103 2024-04-27 12:05:16.000000 owega-5.6.4/owega/owega.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     6111 2024-04-27 12:05:16.000000 owega-5.6.4/owega/utils.py
-drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-10 10:32:35.541177 owega-5.6.4/owega.egg-info/
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    15910 2024-05-10 10:32:35.000000 owega-5.6.4/owega.egg-info/PKG-INFO
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1656 2024-05-10 10:32:35.000000 owega-5.6.4/owega.egg-info/SOURCES.txt
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)        1 2024-05-10 10:32:35.000000 owega-5.6.4/owega.egg-info/dependency_links.txt
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       43 2024-05-10 10:32:35.000000 owega-5.6.4/owega.egg-info/entry_points.txt
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      156 2024-05-10 10:32:35.000000 owega-5.6.4/owega.egg-info/requires.txt
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)        6 2024-05-10 10:32:35.000000 owega-5.6.4/owega.egg-info/top_level.txt
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       90 2024-04-17 02:21:38.000000 owega-5.6.4/pyproject.toml
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       38 2024-05-10 10:32:35.541177 owega-5.6.4/setup.cfg
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     2082 2024-04-27 12:05:16.000000 owega-5.6.4/setup.py
+drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-10 13:38:29.766134 owega-5.7.0/
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     6078 2024-05-10 13:30:40.000000 owega-5.7.0/LICENSE
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    15977 2024-05-10 13:38:29.766134 owega-5.7.0/PKG-INFO
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     5023 2024-04-17 02:21:38.000000 owega-5.7.0/README.md
+drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-10 13:38:29.764134 owega-5.7.0/owega/
+drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-10 13:38:29.765134 owega-5.7.0/owega/OweHandlers/
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      156 2024-04-27 12:05:16.000000 owega-5.7.0/owega/OweHandlers/__init__.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      980 2024-05-08 02:39:07.000000 owega-5.7.0/owega/OweHandlers/handle_add_sysmem.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1590 2024-05-08 02:39:07.000000 owega-5.7.0/owega/OweHandlers/handle_commands.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1185 2024-05-08 02:39:07.000000 owega-5.7.0/owega/OweHandlers/handle_context.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1601 2024-05-08 02:39:07.000000 owega-5.7.0/owega/OweHandlers/handle_del_sysmem.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1816 2024-05-08 02:39:07.000000 owega-5.7.0/owega/OweHandlers/handle_dinput.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     3457 2024-05-08 02:39:07.000000 owega-5.7.0/owega/OweHandlers/handle_edit.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1339 2024-05-08 02:39:07.000000 owega-5.7.0/owega/OweHandlers/handle_estimation.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     5059 2024-05-08 02:39:07.000000 owega-5.7.0/owega/OweHandlers/handle_finput.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1816 2024-05-08 02:39:07.000000 owega-5.7.0/owega/OweHandlers/handle_frequency.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      521 2024-05-08 02:39:07.000000 owega-5.7.0/owega/OweHandlers/handle_genconf.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      523 2024-05-08 02:39:07.000000 owega-5.7.0/owega/OweHandlers/handle_history.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     3310 2024-05-08 02:39:08.000000 owega-5.7.0/owega/OweHandlers/handle_image.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1118 2024-05-08 02:39:08.000000 owega-5.7.0/owega/OweHandlers/handle_load.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1698 2024-05-08 02:39:08.000000 owega-5.7.0/owega/OweHandlers/handle_model.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1791 2024-05-08 02:39:08.000000 owega-5.7.0/owega/OweHandlers/handle_presence.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      637 2024-05-08 02:39:08.000000 owega-5.7.0/owega/OweHandlers/handle_quit.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1090 2024-05-08 02:39:08.000000 owega-5.7.0/owega/OweHandlers/handle_save.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      945 2024-05-08 02:39:08.000000 owega-5.7.0/owega/OweHandlers/handle_system.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1739 2024-05-08 02:39:08.000000 owega-5.7.0/owega/OweHandlers/handle_temperature.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1404 2024-05-08 02:39:08.000000 owega-5.7.0/owega/OweHandlers/handle_tokens.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1556 2024-05-08 02:39:08.000000 owega-5.7.0/owega/OweHandlers/handle_top_p.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1245 2024-05-08 02:39:08.000000 owega-5.7.0/owega/OweHandlers/handle_tts.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     2407 2024-04-27 12:05:16.000000 owega-5.7.0/owega/OweHandlers/handlers.py
+drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-10 13:38:29.765134 owega-5.7.0/owega/OwegaFun/
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      873 2024-04-27 12:05:16.000000 owega-5.7.0/owega/OwegaFun/__init__.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     3867 2024-04-17 02:21:38.000000 owega-5.7.0/owega/OwegaFun/functions.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     4342 2024-04-27 12:05:16.000000 owega-5.7.0/owega/OwegaFun/longTermSouvenirs.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     5816 2024-04-27 12:05:16.000000 owega-5.7.0/owega/OwegaFun/utility.py
+drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-10 13:38:29.765134 owega-5.7.0/owega/OwegaSession/
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      100 2024-04-17 02:21:38.000000 owega-5.7.0/owega/OwegaSession/__init__.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     2763 2024-04-27 12:05:16.000000 owega-5.7.0/owega/OwegaSession/main_bottom_toolbar.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     5592 2024-04-27 12:05:16.000000 owega-5.7.0/owega/OwegaSession/promptsession.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      175 2024-05-08 02:39:08.000000 owega-5.7.0/owega/__init__.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       94 2024-04-17 02:21:38.000000 owega-5.7.0/owega/__main__.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     9363 2024-05-10 10:34:51.000000 owega-5.7.0/owega/ask.py
+drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-10 13:38:29.765134 owega-5.7.0/owega/changelog/
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       80 2024-04-27 12:05:16.000000 owega-5.7.0/owega/changelog/__init__.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    24145 2024-05-10 12:58:21.000000 owega-5.7.0/owega/changelog/changelog.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1534 2024-04-27 12:05:16.000000 owega-5.7.0/owega/changelog/changelogEntry.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     3315 2024-04-17 02:21:38.000000 owega-5.7.0/owega/changelog/version.py
+drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-10 13:38:29.765134 owega-5.7.0/owega/config/
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       86 2024-04-17 02:21:38.000000 owega-5.7.0/owega/config/__init__.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1810 2024-04-27 12:05:16.000000 owega-5.7.0/owega/config/baseConf.py
+drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-10 13:38:29.765134 owega-5.7.0/owega/conversation/
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       83 2024-04-17 02:21:38.000000 owega-5.7.0/owega/conversation/__init__.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    10105 2024-04-27 12:05:16.000000 owega-5.7.0/owega/conversation/conversation.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1418 2024-05-10 10:34:51.000000 owega-5.7.0/owega/getLogger.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       64 2024-04-17 02:21:38.000000 owega-5.7.0/owega/handlerBase.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     6143 2024-05-10 13:31:27.000000 owega-5.7.0/owega/license.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    12103 2024-04-27 12:05:16.000000 owega-5.7.0/owega/owega.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     6111 2024-04-27 12:05:16.000000 owega-5.7.0/owega/utils.py
+drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-10 13:38:29.765134 owega-5.7.0/owega.egg-info/
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    15977 2024-05-10 13:38:29.000000 owega-5.7.0/owega.egg-info/PKG-INFO
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1656 2024-05-10 13:38:29.000000 owega-5.7.0/owega.egg-info/SOURCES.txt
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)        1 2024-05-10 13:38:29.000000 owega-5.7.0/owega.egg-info/dependency_links.txt
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       43 2024-05-10 13:38:29.000000 owega-5.7.0/owega.egg-info/entry_points.txt
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      156 2024-05-10 13:38:29.000000 owega-5.7.0/owega.egg-info/requires.txt
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)        6 2024-05-10 13:38:29.000000 owega-5.7.0/owega.egg-info/top_level.txt
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       90 2024-04-17 02:21:38.000000 owega-5.7.0/pyproject.toml
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       38 2024-05-10 13:38:29.766134 owega-5.7.0/setup.cfg
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     2085 2024-05-10 12:54:49.000000 owega-5.7.0/setup.py
```

### Comparing `owega-5.6.4/PKG-INFO` & `owega-5.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: owega
-Version: 5.6.4
+Version: 5.7.0
 Summary: A command-line interface for conversing with GPT models (from OpenAI)
 Home-page: https://git.pyrokinesis.fr/darkgeem/owega
 Author: darkgeem
 Author-email: darkgeem@pyrokinesis.fr
-License: WTFPL
+License: DGPL-1.0
 Project-URL: Source, https://git.pyrokinesis.fr/darkgeem/owega
 Project-URL: Support, https://discord.gg/KdRmyRrA48
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Information Technology
@@ -135,15 +135,15 @@
 See ΦωΦ in action!
 
 [![asciicast](https://asciinema.org/a/613143.png)](https://asciinema.org/a/613143)
 
 
 ## CHANGELOG: 
 ```
-OWEGA v5.6.4 CHANGELOG:
+OWEGA v5.7.0 CHANGELOG:
 
 
 2.0.0: WTFPL license
 2.0.1: added genconf command
 
 2.1.0: added file_input command
 2.1.1: added file_input in help command
@@ -360,8 +360,10 @@
        (chub mars, mercury, mixtral)
        Also, Mi(s/x)tral support is no more in beta :D
 5.6.1: Added extensive logging for errors.
 5.6.2: Added terminal title status :3
 5.6.3: Fixes config's api_key not being used.
        Better docstrings on handlers.
 5.6.4: Fix for ask.ask() crashing if OPENAI_API_KEY isn't set.
+
+5.7.0: Changed the license to the DarkGeem Public License v1.0
 ```
```

### Comparing `owega-5.6.4/README.md` & `owega-5.7.0/README.md`

 * *Files identical despite different names*

### Comparing `owega-5.6.4/owega/OweHandlers/handle_add_sysmem.py` & `owega-5.7.0/owega/OweHandlers/handle_add_sysmem.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.4/owega/OweHandlers/handle_commands.py` & `owega-5.7.0/owega/OweHandlers/handle_commands.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.4/owega/OweHandlers/handle_context.py` & `owega-5.7.0/owega/OweHandlers/handle_context.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.4/owega/OweHandlers/handle_del_sysmem.py` & `owega-5.7.0/owega/OweHandlers/handle_del_sysmem.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.4/owega/OweHandlers/handle_dinput.py` & `owega-5.7.0/owega/OweHandlers/handle_dinput.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.4/owega/OweHandlers/handle_edit.py` & `owega-5.7.0/owega/OweHandlers/handle_edit.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.4/owega/OweHandlers/handle_estimation.py` & `owega-5.7.0/owega/OweHandlers/handle_estimation.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.4/owega/OweHandlers/handle_finput.py` & `owega-5.7.0/owega/OweHandlers/handle_finput.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.4/owega/OweHandlers/handle_frequency.py` & `owega-5.7.0/owega/OweHandlers/handle_frequency.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.4/owega/OweHandlers/handle_genconf.py` & `owega-5.7.0/owega/OweHandlers/handle_genconf.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.4/owega/OweHandlers/handle_history.py` & `owega-5.7.0/owega/OweHandlers/handle_history.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.4/owega/OweHandlers/handle_image.py` & `owega-5.7.0/owega/OweHandlers/handle_image.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.4/owega/OweHandlers/handle_load.py` & `owega-5.7.0/owega/OweHandlers/handle_load.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.4/owega/OweHandlers/handle_model.py` & `owega-5.7.0/owega/OweHandlers/handle_model.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.4/owega/OweHandlers/handle_presence.py` & `owega-5.7.0/owega/OweHandlers/handle_presence.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.4/owega/OweHandlers/handle_quit.py` & `owega-5.7.0/owega/OweHandlers/handle_quit.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.4/owega/OweHandlers/handle_save.py` & `owega-5.7.0/owega/OweHandlers/handle_save.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.4/owega/OweHandlers/handle_system.py` & `owega-5.7.0/owega/OweHandlers/handle_system.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.4/owega/OweHandlers/handle_temperature.py` & `owega-5.7.0/owega/OweHandlers/handle_temperature.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.4/owega/OweHandlers/handle_tokens.py` & `owega-5.7.0/owega/OweHandlers/handle_tokens.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.4/owega/OweHandlers/handle_top_p.py` & `owega-5.7.0/owega/OweHandlers/handle_top_p.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.4/owega/OweHandlers/handle_tts.py` & `owega-5.7.0/owega/OweHandlers/handle_tts.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.4/owega/OweHandlers/handlers.py` & `owega-5.7.0/owega/OweHandlers/handlers.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.4/owega/OwegaFun/__init__.py` & `owega-5.7.0/owega/OwegaFun/__init__.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.4/owega/OwegaFun/functions.py` & `owega-5.7.0/owega/OwegaFun/functions.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.4/owega/OwegaFun/longTermSouvenirs.py` & `owega-5.7.0/owega/OwegaFun/longTermSouvenirs.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.4/owega/OwegaFun/utility.py` & `owega-5.7.0/owega/OwegaFun/utility.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.4/owega/OwegaSession/main_bottom_toolbar.py` & `owega-5.7.0/owega/OwegaSession/main_bottom_toolbar.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.4/owega/OwegaSession/promptsession.py` & `owega-5.7.0/owega/OwegaSession/promptsession.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.4/owega/ask.py` & `owega-5.7.0/owega/ask.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.4/owega/changelog/changelog.py` & `owega-5.7.0/owega/changelog/changelog.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,14 +13,19 @@
         self.version = Version(0, 0, 0)
         self.initLogs()
         self.genLog()
 
     def initLogs(self):
         """Fill the changelog."""
         self.logs.append(
+            ChangelogEntry(5, 7, 0)
+            .addLine("Changed the license to the DarkGeem Public License v1.0")
+        )
+
+        self.logs.append(
             ChangelogEntry(5, 6, 4)
             .addLine("Fix for ask.ask() crashing if OPENAI_API_KEY isn't set.")
         )
         self.logs.append(
             ChangelogEntry(5, 6, 3)
             .addLine("Fixes config's api_key not being used.")
             .addLine("Better docstrings on handlers.")
```

### Comparing `owega-5.6.4/owega/changelog/changelogEntry.py` & `owega-5.7.0/owega/changelog/changelogEntry.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.4/owega/changelog/version.py` & `owega-5.7.0/owega/changelog/version.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.4/owega/config/baseConf.py` & `owega-5.7.0/owega/config/baseConf.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.4/owega/conversation/conversation.py` & `owega-5.7.0/owega/conversation/conversation.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.4/owega/getLogger.py` & `owega-5.7.0/owega/getLogger.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.4/owega/owega.py` & `owega-5.7.0/owega/owega.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.4/owega/utils.py` & `owega-5.7.0/owega/utils.py`

 * *Files identical despite different names*

### Comparing `owega-5.6.4/owega.egg-info/PKG-INFO` & `owega-5.7.0/owega.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: owega
-Version: 5.6.4
+Version: 5.7.0
 Summary: A command-line interface for conversing with GPT models (from OpenAI)
 Home-page: https://git.pyrokinesis.fr/darkgeem/owega
 Author: darkgeem
 Author-email: darkgeem@pyrokinesis.fr
-License: WTFPL
+License: DGPL-1.0
 Project-URL: Source, https://git.pyrokinesis.fr/darkgeem/owega
 Project-URL: Support, https://discord.gg/KdRmyRrA48
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Information Technology
@@ -135,15 +135,15 @@
 See ΦωΦ in action!
 
 [![asciicast](https://asciinema.org/a/613143.png)](https://asciinema.org/a/613143)
 
 
 ## CHANGELOG: 
 ```
-OWEGA v5.6.4 CHANGELOG:
+OWEGA v5.7.0 CHANGELOG:
 
 
 2.0.0: WTFPL license
 2.0.1: added genconf command
 
 2.1.0: added file_input command
 2.1.1: added file_input in help command
@@ -360,8 +360,10 @@
        (chub mars, mercury, mixtral)
        Also, Mi(s/x)tral support is no more in beta :D
 5.6.1: Added extensive logging for errors.
 5.6.2: Added terminal title status :3
 5.6.3: Fixes config's api_key not being used.
        Better docstrings on handlers.
 5.6.4: Fix for ask.ask() crashing if OPENAI_API_KEY isn't set.
+
+5.7.0: Changed the license to the DarkGeem Public License v1.0
 ```
```

### Comparing `owega-5.6.4/owega.egg-info/SOURCES.txt` & `owega-5.7.0/owega.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `owega-5.6.4/setup.py` & `owega-5.7.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -62,14 +62,14 @@
     ],
     entry_points={
         'console_scripts': [
             'owega = owega.owega:main',
         ]
     },
     install_requires=requirements,
-    license="WTFPL",
+    license="DGPL-1.0",
     license_files=["LICEN[CS]E*"],
     project_urls={
         'Source': 'https://git.pyrokinesis.fr/darkgeem/owega',
         'Support': 'https://discord.gg/KdRmyRrA48',
     },
 )
```

