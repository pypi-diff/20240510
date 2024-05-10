# Comparing `tmp/meerschaum-2.1.7.tar.gz` & `tmp/meerschaum-2.2.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meerschaum-2.1.7.tar", last modified: Mon Jan  8 03:49:02 2024, max compression
+gzip compressed data, was "meerschaum-2.2.0.dev1.tar", last modified: Fri May 10 03:58:42 2024, max compression
```

## Comparing `meerschaum-2.1.7.tar` & `meerschaum-2.2.0.dev1.tar`

### file list

```diff
@@ -1,299 +1,299 @@
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-01-08 03:49:02.515344 meerschaum-2.1.7/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    11359 2021-12-27 13:50:47.000000 meerschaum-2.1.7/LICENSE
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      114 2021-12-27 13:50:47.000000 meerschaum-2.1.7/NOTICE
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    23451 2024-01-08 03:49:02.514344 meerschaum-2.1.7/PKG-INFO
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9183 2023-12-01 07:12:21.000000 meerschaum-2.1.7/README.md
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-01-08 03:49:02.445344 meerschaum-2.1.7/meerschaum/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1487 2023-11-26 03:23:44.000000 meerschaum-2.1.7/meerschaum/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2763 2023-12-01 07:12:21.000000 meerschaum-2.1.7/meerschaum/__main__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-01-08 03:49:02.446344 meerschaum-2.1.7/meerschaum/_internal/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      169 2022-04-23 01:15:00.000000 meerschaum-2.1.7/meerschaum/_internal/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-01-08 03:49:02.446344 meerschaum-2.1.7/meerschaum/_internal/arguments/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      519 2022-10-22 06:25:53.000000 meerschaum-2.1.7/meerschaum/_internal/arguments/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    10249 2023-09-25 20:34:26.000000 meerschaum-2.1.7/meerschaum/_internal/arguments/_parse_arguments.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    13597 2023-12-01 07:12:21.000000 meerschaum-2.1.7/meerschaum/_internal/arguments/_parser.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-01-08 03:49:02.447344 meerschaum-2.1.7/meerschaum/_internal/docs/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      126 2021-11-08 16:07:48.000000 meerschaum-2.1.7/meerschaum/_internal/docs/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7076 2023-12-01 07:12:21.000000 meerschaum-2.1.7/meerschaum/_internal/docs/index.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4820 2023-11-26 03:23:44.000000 meerschaum-2.1.7/meerschaum/_internal/entry.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-01-08 03:49:02.447344 meerschaum-2.1.7/meerschaum/_internal/gui/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1313 2023-08-24 14:21:38.000000 meerschaum-2.1.7/meerschaum/_internal/gui/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-01-08 03:49:02.447344 meerschaum-2.1.7/meerschaum/_internal/gui/app/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1565 2022-04-24 10:29:36.000000 meerschaum-2.1.7/meerschaum/_internal/gui/app/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2632 2022-10-18 06:13:35.000000 meerschaum-2.1.7/meerschaum/_internal/gui/app/_windows.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      935 2023-08-24 14:21:38.000000 meerschaum-2.1.7/meerschaum/_internal/gui/app/actions.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1596 2023-08-24 14:21:38.000000 meerschaum-2.1.7/meerschaum/_internal/gui/app/pipes.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-01-08 03:49:02.447344 meerschaum-2.1.7/meerschaum/_internal/shell/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    32826 2024-01-08 03:48:33.000000 meerschaum-2.1.7/meerschaum/_internal/shell/Shell.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3114 2023-11-26 03:23:44.000000 meerschaum-2.1.7/meerschaum/_internal/shell/ShellCompleter.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1280 2022-10-26 04:20:20.000000 meerschaum-2.1.7/meerschaum/_internal/shell/ValidAutoSuggest.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      281 2022-04-24 10:29:36.000000 meerschaum-2.1.7/meerschaum/_internal/shell/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-01-08 03:49:02.448344 meerschaum-2.1.7/meerschaum/_internal/shell/resources/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2022-04-24 10:29:36.000000 meerschaum-2.1.7/meerschaum/_internal/shell/resources/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-01-08 03:49:02.448344 meerschaum-2.1.7/meerschaum/_internal/term/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      520 2023-12-01 07:12:21.000000 meerschaum-2.1.7/meerschaum/_internal/term/TermPageHandler.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1594 2023-11-06 21:03:03.000000 meerschaum-2.1.7/meerschaum/_internal/term/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      716 2023-08-24 14:21:38.000000 meerschaum-2.1.7/meerschaum/_internal/term/tools.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-01-08 03:49:02.451344 meerschaum-2.1.7/meerschaum/actions/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    11360 2023-11-26 03:23:44.000000 meerschaum-2.1.7/meerschaum/actions/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    12756 2024-01-08 03:48:33.000000 meerschaum-2.1.7/meerschaum/actions/api.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    13396 2023-11-13 16:31:14.000000 meerschaum-2.1.7/meerschaum/actions/bootstrap.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4851 2023-09-25 20:34:26.000000 meerschaum-2.1.7/meerschaum/actions/clear.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6213 2023-09-25 20:34:26.000000 meerschaum-2.1.7/meerschaum/actions/copy.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1167 2023-09-25 20:34:26.000000 meerschaum-2.1.7/meerschaum/actions/deduplicate.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    15528 2023-11-13 16:31:14.000000 meerschaum-2.1.7/meerschaum/actions/delete.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2453 2023-09-25 20:34:26.000000 meerschaum-2.1.7/meerschaum/actions/drop.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9487 2023-09-25 20:34:26.000000 meerschaum-2.1.7/meerschaum/actions/edit.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7372 2023-10-04 04:03:08.000000 meerschaum-2.1.7/meerschaum/actions/install.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4206 2023-09-21 17:52:19.000000 meerschaum-2.1.7/meerschaum/actions/login.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2251 2022-08-29 21:54:10.000000 meerschaum-2.1.7/meerschaum/actions/os.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3909 2023-11-13 21:37:33.000000 meerschaum-2.1.7/meerschaum/actions/pause.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2395 2022-02-28 20:55:01.000000 meerschaum-2.1.7/meerschaum/actions/python.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    11326 2023-12-01 07:12:21.000000 meerschaum-2.1.7/meerschaum/actions/register.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      508 2023-11-26 03:23:44.000000 meerschaum-2.1.7/meerschaum/actions/reload.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3205 2023-09-25 20:34:26.000000 meerschaum-2.1.7/meerschaum/actions/setup.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2026 2022-08-29 21:54:10.000000 meerschaum-2.1.7/meerschaum/actions/sh.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    26212 2023-12-01 07:12:21.000000 meerschaum-2.1.7/meerschaum/actions/show.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4311 2023-10-27 06:03:46.000000 meerschaum-2.1.7/meerschaum/actions/sql.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5886 2023-08-28 22:18:25.000000 meerschaum-2.1.7/meerschaum/actions/stack.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    18384 2023-11-06 21:03:03.000000 meerschaum-2.1.7/meerschaum/actions/start.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4311 2023-09-25 20:34:26.000000 meerschaum-2.1.7/meerschaum/actions/stop.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    17266 2023-12-04 02:32:59.000000 meerschaum-2.1.7/meerschaum/actions/sync.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3053 2023-12-01 07:12:21.000000 meerschaum-2.1.7/meerschaum/actions/tag.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6068 2023-09-25 20:34:26.000000 meerschaum-2.1.7/meerschaum/actions/uninstall.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6302 2023-09-25 20:34:26.000000 meerschaum-2.1.7/meerschaum/actions/upgrade.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4885 2023-09-25 20:34:26.000000 meerschaum-2.1.7/meerschaum/actions/verify.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-01-08 03:49:02.452344 meerschaum-2.1.7/meerschaum/api/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7694 2023-12-01 07:12:21.000000 meerschaum-2.1.7/meerschaum/api/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      875 2022-02-28 20:55:01.000000 meerschaum-2.1.7/meerschaum/api/_chain.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1603 2023-08-24 14:21:38.000000 meerschaum-2.1.7/meerschaum/api/_events.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      961 2023-08-24 00:13:16.000000 meerschaum-2.1.7/meerschaum/api/_oauth2.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1609 2023-11-06 21:03:03.000000 meerschaum-2.1.7/meerschaum/api/_websockets.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-01-08 03:49:02.453344 meerschaum-2.1.7/meerschaum/api/dash/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2252 2023-11-06 21:03:03.000000 meerschaum-2.1.7/meerschaum/api/dash/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9418 2023-09-25 20:34:26.000000 meerschaum-2.1.7/meerschaum/api/dash/actions.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-01-08 03:49:02.454344 meerschaum-2.1.7/meerschaum/api/dash/assets/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.1.7/meerschaum/api/dash/assets/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    21923 2021-11-08 16:07:48.000000 meerschaum-2.1.7/meerschaum/api/dash/assets/ansi_up.js
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)   338636 2021-11-08 16:07:48.000000 meerschaum-2.1.7/meerschaum/api/dash/assets/banner_1920x320.png
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9662 2021-11-08 16:07:48.000000 meerschaum-2.1.7/meerschaum/api/dash/assets/favicon.ico
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    10218 2021-11-08 16:07:48.000000 meerschaum-2.1.7/meerschaum/api/dash/assets/logo_48x48.png
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    67702 2021-11-08 16:07:48.000000 meerschaum-2.1.7/meerschaum/api/dash/assets/logo_500x500.png
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-01-08 03:49:02.455344 meerschaum-2.1.7/meerschaum/api/dash/callbacks/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      325 2023-09-25 20:34:26.000000 meerschaum-2.1.7/meerschaum/api/dash/callbacks/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    30454 2023-12-01 07:12:21.000000 meerschaum-2.1.7/meerschaum/api/dash/callbacks/dashboard.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6233 2023-09-26 04:28:45.000000 meerschaum-2.1.7/meerschaum/api/dash/callbacks/jobs.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2613 2023-08-24 14:21:38.000000 meerschaum-2.1.7/meerschaum/api/dash/callbacks/login.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2777 2022-07-26 06:45:25.000000 meerschaum-2.1.7/meerschaum/api/dash/callbacks/plugins.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3600 2023-08-24 14:21:38.000000 meerschaum-2.1.7/meerschaum/api/dash/callbacks/register.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6364 2023-11-06 21:03:03.000000 meerschaum-2.1.7/meerschaum/api/dash/components.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      843 2021-11-08 16:07:48.000000 meerschaum-2.1.7/meerschaum/api/dash/connectors.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2046 2023-08-24 14:21:38.000000 meerschaum-2.1.7/meerschaum/api/dash/graphs.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6672 2023-11-06 21:03:03.000000 meerschaum-2.1.7/meerschaum/api/dash/jobs.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    12591 2023-11-26 03:23:44.000000 meerschaum-2.1.7/meerschaum/api/dash/keys.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-01-08 03:49:02.456344 meerschaum-2.1.7/meerschaum/api/dash/pages/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      273 2023-07-21 01:07:38.000000 meerschaum-2.1.7/meerschaum/api/dash/pages/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3930 2023-11-26 03:23:44.000000 meerschaum-2.1.7/meerschaum/api/dash/pages/dashboard.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      595 2023-08-24 14:21:38.000000 meerschaum-2.1.7/meerschaum/api/dash/pages/error.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4600 2023-10-04 04:03:08.000000 meerschaum-2.1.7/meerschaum/api/dash/pages/login.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1549 2023-08-24 14:21:38.000000 meerschaum-2.1.7/meerschaum/api/dash/pages/plugins.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2364 2023-08-24 14:21:38.000000 meerschaum-2.1.7/meerschaum/api/dash/pages/register.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    14866 2023-11-06 21:03:03.000000 meerschaum-2.1.7/meerschaum/api/dash/pipes.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3115 2023-08-24 14:21:38.000000 meerschaum-2.1.7/meerschaum/api/dash/plugins.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      504 2022-07-26 06:45:25.000000 meerschaum-2.1.7/meerschaum/api/dash/sync.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2362 2023-11-06 21:03:03.000000 meerschaum-2.1.7/meerschaum/api/dash/users.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      924 2022-10-31 13:18:31.000000 meerschaum-2.1.7/meerschaum/api/dash/websockets.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3298 2023-11-06 21:03:03.000000 meerschaum-2.1.7/meerschaum/api/dash/webterm.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-01-08 03:49:02.456344 meerschaum-2.1.7/meerschaum/api/models/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      276 2021-11-08 16:07:48.000000 meerschaum-2.1.7/meerschaum/api/models/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      263 2021-11-08 16:07:48.000000 meerschaum-2.1.7/meerschaum/api/models/_interfaces.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      304 2021-11-08 16:07:48.000000 meerschaum-2.1.7/meerschaum/api/models/_locations.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      295 2021-11-08 16:07:48.000000 meerschaum-2.1.7/meerschaum/api/models/_metrics.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      463 2021-11-20 21:54:59.000000 meerschaum-2.1.7/meerschaum/api/models/_pipes.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-01-08 03:49:02.456344 meerschaum-2.1.7/meerschaum/api/resources/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      115 2021-11-08 16:07:48.000000 meerschaum-2.1.7/meerschaum/api/resources/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-01-08 03:49:02.456344 meerschaum-2.1.7/meerschaum/api/resources/static/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.1.7/meerschaum/api/resources/static/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-01-08 03:49:02.457344 meerschaum-2.1.7/meerschaum/api/resources/static/css/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.1.7/meerschaum/api/resources/static/css/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)   180286 2021-11-08 16:07:48.000000 meerschaum-2.1.7/meerschaum/api/resources/static/css/bootstrap.min.css
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1714 2023-09-25 20:34:26.000000 meerschaum-2.1.7/meerschaum/api/resources/static/css/dash.css
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6087 2021-11-08 16:07:48.000000 meerschaum-2.1.7/meerschaum/api/resources/static/css/dbc_dark.css
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)       81 2021-11-08 16:07:48.000000 meerschaum-2.1.7/meerschaum/api/resources/static/css/styles.css
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5383 2023-11-06 21:03:03.000000 meerschaum-2.1.7/meerschaum/api/resources/static/css/xterm.css
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-01-08 03:49:02.457344 meerschaum-2.1.7/meerschaum/api/resources/static/ico/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.1.7/meerschaum/api/resources/static/ico/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9662 2021-11-08 16:07:48.000000 meerschaum-2.1.7/meerschaum/api/resources/static/ico/logo.ico
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-01-08 03:49:02.458344 meerschaum-2.1.7/meerschaum/api/resources/static/js/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.1.7/meerschaum/api/resources/static/js/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      540 2021-11-08 16:07:48.000000 meerschaum-2.1.7/meerschaum/api/resources/static/js/action_button.js
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.1.7/meerschaum/api/resources/static/js/main.js
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1729 2023-11-06 21:03:03.000000 meerschaum-2.1.7/meerschaum/api/resources/static/js/terminado.js
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)   282870 2023-11-06 21:03:03.000000 meerschaum-2.1.7/meerschaum/api/resources/static/js/xterm.js
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-01-08 03:49:02.458344 meerschaum-2.1.7/meerschaum/api/resources/static/png/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.1.7/meerschaum/api/resources/static/png/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-01-08 03:49:02.459344 meerschaum-2.1.7/meerschaum/api/resources/templates/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.1.7/meerschaum/api/resources/templates/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1019 2021-11-08 16:07:48.000000 meerschaum-2.1.7/meerschaum/api/resources/templates/index.html
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1711 2021-11-08 16:07:48.000000 meerschaum-2.1.7/meerschaum/api/resources/templates/old_index.html
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      141 2021-11-08 16:07:48.000000 meerschaum-2.1.7/meerschaum/api/resources/templates/secret.html
--rwxr-xr-x   0 bmeares   (1000) bmeares   (1000)     4443 2023-11-26 03:23:44.000000 meerschaum-2.1.7/meerschaum/api/resources/templates/termpage.html
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-01-08 03:49:02.460344 meerschaum-2.1.7/meerschaum/api/routes/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      564 2023-08-24 14:21:38.000000 meerschaum-2.1.7/meerschaum/api/routes/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2240 2022-06-27 01:07:31.000000 meerschaum-2.1.7/meerschaum/api/routes/_actions.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1849 2023-10-04 04:03:08.000000 meerschaum-2.1.7/meerschaum/api/routes/_connectors.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      578 2022-02-28 20:55:01.000000 meerschaum-2.1.7/meerschaum/api/routes/_index.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1935 2023-12-01 07:12:21.000000 meerschaum-2.1.7/meerschaum/api/routes/_login.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2469 2023-08-24 14:21:38.000000 meerschaum-2.1.7/meerschaum/api/routes/_misc.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    21677 2023-11-13 16:31:14.000000 meerschaum-2.1.7/meerschaum/api/routes/_pipes.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6151 2023-08-24 14:21:38.000000 meerschaum-2.1.7/meerschaum/api/routes/_plugins.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7204 2023-08-24 00:13:16.000000 meerschaum-2.1.7/meerschaum/api/routes/_users.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      825 2022-06-27 01:07:31.000000 meerschaum-2.1.7/meerschaum/api/routes/_version.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3909 2023-11-06 21:03:03.000000 meerschaum-2.1.7/meerschaum/api/routes/_webterm.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-01-08 03:49:02.460344 meerschaum-2.1.7/meerschaum/api/tables/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      482 2023-10-26 06:22:59.000000 meerschaum-2.1.7/meerschaum/api/tables/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-01-08 03:49:02.462344 meerschaum-2.1.7/meerschaum/config/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    11517 2023-11-13 16:31:14.000000 meerschaum-2.1.7/meerschaum/config/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5184 2023-11-13 16:31:14.000000 meerschaum-2.1.7/meerschaum/config/_default.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     8218 2023-11-26 03:23:44.000000 meerschaum-2.1.7/meerschaum/config/_edit.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4419 2023-11-06 21:03:03.000000 meerschaum-2.1.7/meerschaum/config/_environment.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6635 2023-12-01 07:12:21.000000 meerschaum-2.1.7/meerschaum/config/_formatting.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1073 2023-09-25 20:34:26.000000 meerschaum-2.1.7/meerschaum/config/_jobs.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1526 2023-11-06 21:03:03.000000 meerschaum-2.1.7/meerschaum/config/_patch.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7983 2023-11-06 21:03:03.000000 meerschaum-2.1.7/meerschaum/config/_paths.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1220 2022-02-28 20:55:01.000000 meerschaum-2.1.7/meerschaum/config/_preprocess.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    14720 2023-09-25 20:34:26.000000 meerschaum-2.1.7/meerschaum/config/_read_config.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3551 2024-01-08 03:48:33.000000 meerschaum-2.1.7/meerschaum/config/_shell.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4120 2023-08-28 22:18:25.000000 meerschaum-2.1.7/meerschaum/config/_sync.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)       71 2024-01-08 03:48:33.000000 meerschaum-2.1.7/meerschaum/config/_version.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-01-08 03:49:02.462344 meerschaum-2.1.7/meerschaum/config/resources/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.1.7/meerschaum/config/resources/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-01-08 03:49:02.462344 meerschaum-2.1.7/meerschaum/config/stack/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9034 2023-08-28 22:18:25.000000 meerschaum-2.1.7/meerschaum/config/stack/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-01-08 03:49:02.462344 meerschaum-2.1.7/meerschaum/config/stack/grafana/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2010 2022-11-01 03:52:40.000000 meerschaum-2.1.7/meerschaum/config/stack/grafana/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-01-08 03:49:02.462344 meerschaum-2.1.7/meerschaum/config/stack/mosquitto/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      186 2021-11-08 16:07:48.000000 meerschaum-2.1.7/meerschaum/config/stack/mosquitto/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-01-08 03:49:02.462344 meerschaum-2.1.7/meerschaum/config/stack/mosquitto/resources/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.1.7/meerschaum/config/stack/mosquitto/resources/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-01-08 03:49:02.463344 meerschaum-2.1.7/meerschaum/config/stack/resources/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.1.7/meerschaum/config/stack/resources/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-01-08 03:49:02.463344 meerschaum-2.1.7/meerschaum/config/static/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4361 2023-11-26 03:23:44.000000 meerschaum-2.1.7/meerschaum/config/static/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-01-08 03:49:02.463344 meerschaum-2.1.7/meerschaum/connectors/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6381 2023-04-25 23:57:31.000000 meerschaum-2.1.7/meerschaum/connectors/Connector.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    12023 2023-10-04 04:03:08.000000 meerschaum-2.1.7/meerschaum/connectors/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-01-08 03:49:02.465344 meerschaum-2.1.7/meerschaum/connectors/api/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4355 2023-12-01 07:12:21.000000 meerschaum-2.1.7/meerschaum/connectors/api/APIConnector.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      205 2021-11-08 16:07:48.000000 meerschaum-2.1.7/meerschaum/connectors/api/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2755 2023-08-28 22:18:25.000000 meerschaum-2.1.7/meerschaum/connectors/api/_actions.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2072 2023-09-25 20:34:26.000000 meerschaum-2.1.7/meerschaum/connectors/api/_fetch.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2050 2023-08-28 22:18:25.000000 meerschaum-2.1.7/meerschaum/connectors/api/_login.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1093 2023-08-28 22:18:25.000000 meerschaum-2.1.7/meerschaum/connectors/api/_misc.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    20962 2023-11-10 05:44:22.000000 meerschaum-2.1.7/meerschaum/connectors/api/_pipes.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5163 2023-08-28 22:18:25.000000 meerschaum-2.1.7/meerschaum/connectors/api/_plugins.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6922 2023-10-04 04:03:08.000000 meerschaum-2.1.7/meerschaum/connectors/api/_request.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1489 2022-07-25 06:37:48.000000 meerschaum-2.1.7/meerschaum/connectors/api/_uri.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5275 2023-08-28 22:18:25.000000 meerschaum-2.1.7/meerschaum/connectors/api/_users.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4044 2023-08-28 22:18:25.000000 meerschaum-2.1.7/meerschaum/connectors/parse.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-01-08 03:49:02.465344 meerschaum-2.1.7/meerschaum/connectors/plugin/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2084 2022-10-25 06:38:00.000000 meerschaum-2.1.7/meerschaum/connectors/plugin/PluginConnector.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      198 2021-11-08 16:07:48.000000 meerschaum-2.1.7/meerschaum/connectors/plugin/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7363 2023-08-24 14:21:38.000000 meerschaum-2.1.7/meerschaum/connectors/poll.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-01-08 03:49:02.467344 meerschaum-2.1.7/meerschaum/connectors/sql/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    11522 2023-11-13 16:31:14.000000 meerschaum-2.1.7/meerschaum/connectors/sql/SQLConnector.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      175 2021-11-08 16:07:48.000000 meerschaum-2.1.7/meerschaum/connectors/sql/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4123 2023-11-13 16:31:14.000000 meerschaum-2.1.7/meerschaum/connectors/sql/_cli.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    10382 2023-11-22 21:34:51.000000 meerschaum-2.1.7/meerschaum/connectors/sql/_create_engine.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    13086 2024-01-08 03:48:33.000000 meerschaum-2.1.7/meerschaum/connectors/sql/_fetch.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6447 2023-11-13 16:31:14.000000 meerschaum-2.1.7/meerschaum/connectors/sql/_instance.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)   100925 2024-01-08 03:48:33.000000 meerschaum-2.1.7/meerschaum/connectors/sql/_pipes.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     8323 2023-09-25 20:34:26.000000 meerschaum-2.1.7/meerschaum/connectors/sql/_plugins.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    34262 2023-11-13 16:31:14.000000 meerschaum-2.1.7/meerschaum/connectors/sql/_sql.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3460 2023-10-26 06:22:59.000000 meerschaum-2.1.7/meerschaum/connectors/sql/_uri.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    10100 2023-11-13 16:31:14.000000 meerschaum-2.1.7/meerschaum/connectors/sql/_users.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-01-08 03:49:02.468344 meerschaum-2.1.7/meerschaum/connectors/sql/tables/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9001 2023-12-04 02:32:59.000000 meerschaum-2.1.7/meerschaum/connectors/sql/tables/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1573 2022-02-28 20:55:01.000000 meerschaum-2.1.7/meerschaum/connectors/sql/tables/types.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      187 2022-04-24 10:29:36.000000 meerschaum-2.1.7/meerschaum/connectors/sql/tools.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-01-08 03:49:02.468344 meerschaum-2.1.7/meerschaum/core/
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-01-08 03:49:02.470344 meerschaum-2.1.7/meerschaum/core/Pipe/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    16230 2023-12-01 07:12:21.000000 meerschaum-2.1.7/meerschaum/core/Pipe/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    13202 2023-04-26 08:12:59.000000 meerschaum-2.1.7/meerschaum/core/Pipe/_attributes.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7613 2023-04-25 23:57:31.000000 meerschaum-2.1.7/meerschaum/core/Pipe/_bootstrap.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2261 2023-09-25 20:34:26.000000 meerschaum-2.1.7/meerschaum/core/Pipe/_clear.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    20880 2023-12-04 02:32:59.000000 meerschaum-2.1.7/meerschaum/core/Pipe/_data.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    10267 2023-11-13 06:20:00.000000 meerschaum-2.1.7/meerschaum/core/Pipe/_deduplicate.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2118 2023-11-13 16:31:14.000000 meerschaum-2.1.7/meerschaum/core/Pipe/_delete.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1052 2023-09-25 20:34:26.000000 meerschaum-2.1.7/meerschaum/core/Pipe/_drop.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3694 2024-01-08 03:48:33.000000 meerschaum-2.1.7/meerschaum/core/Pipe/_dtypes.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     8471 2022-12-05 04:26:42.000000 meerschaum-2.1.7/meerschaum/core/Pipe/_edit.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5234 2023-11-26 03:23:44.000000 meerschaum-2.1.7/meerschaum/core/Pipe/_fetch.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2240 2023-01-16 21:21:28.000000 meerschaum-2.1.7/meerschaum/core/Pipe/_register.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1352 2023-04-25 23:57:31.000000 meerschaum-2.1.7/meerschaum/core/Pipe/_show.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    28038 2024-01-08 03:48:33.000000 meerschaum-2.1.7/meerschaum/core/Pipe/_sync.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    14262 2023-11-13 16:31:14.000000 meerschaum-2.1.7/meerschaum/core/Pipe/_verify.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-01-08 03:49:02.470344 meerschaum-2.1.7/meerschaum/core/Plugin/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      137 2022-04-24 10:29:36.000000 meerschaum-2.1.7/meerschaum/core/Plugin/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-01-08 03:49:02.470344 meerschaum-2.1.7/meerschaum/core/User/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2448 2023-08-28 22:18:25.000000 meerschaum-2.1.7/meerschaum/core/User/_User.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      161 2022-04-24 10:29:36.000000 meerschaum-2.1.7/meerschaum/core/User/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      251 2022-04-24 10:29:36.000000 meerschaum-2.1.7/meerschaum/core/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-01-08 03:49:02.471344 meerschaum-2.1.7/meerschaum/plugins/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    33706 2023-11-26 03:23:44.000000 meerschaum-2.1.7/meerschaum/plugins/_Plugin.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    20760 2023-11-26 03:23:44.000000 meerschaum-2.1.7/meerschaum/plugins/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-01-08 03:49:02.474344 meerschaum-2.1.7/meerschaum/utils/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      612 2023-12-01 07:12:21.000000 meerschaum-2.1.7/meerschaum/utils/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    11460 2023-12-01 07:12:21.000000 meerschaum-2.1.7/meerschaum/utils/_get_pipes.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-01-08 03:49:02.474344 meerschaum-2.1.7/meerschaum/utils/daemon/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    31961 2023-12-01 07:12:21.000000 meerschaum-2.1.7/meerschaum/utils/daemon/Daemon.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    19362 2023-11-06 21:03:03.000000 meerschaum-2.1.7/meerschaum/utils/daemon/RotatingFile.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     8174 2023-11-26 03:23:44.000000 meerschaum-2.1.7/meerschaum/utils/daemon/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4330 2023-09-26 04:28:45.000000 meerschaum-2.1.7/meerschaum/utils/daemon/_names.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    31955 2024-01-08 03:48:33.000000 meerschaum-2.1.7/meerschaum/utils/dataframe.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3690 2023-01-09 09:23:24.000000 meerschaum-2.1.7/meerschaum/utils/debug.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-01-08 03:49:02.474344 meerschaum-2.1.7/meerschaum/utils/dtypes/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6110 2023-11-06 21:03:03.000000 meerschaum-2.1.7/meerschaum/utils/dtypes/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    14638 2023-11-13 16:31:14.000000 meerschaum-2.1.7/meerschaum/utils/dtypes/sql.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-01-08 03:49:02.475344 meerschaum-2.1.7/meerschaum/utils/formatting/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    13778 2023-11-26 03:23:44.000000 meerschaum-2.1.7/meerschaum/utils/formatting/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3294 2023-09-25 20:34:26.000000 meerschaum-2.1.7/meerschaum/utils/formatting/_jobs.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    19492 2024-01-08 03:48:33.000000 meerschaum-2.1.7/meerschaum/utils/formatting/_pipes.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3096 2023-09-25 20:34:26.000000 meerschaum-2.1.7/meerschaum/utils/formatting/_pprint.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3677 2023-08-24 14:21:38.000000 meerschaum-2.1.7/meerschaum/utils/formatting/_shell.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3196 2023-12-01 07:12:21.000000 meerschaum-2.1.7/meerschaum/utils/interactive.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    43296 2024-01-08 03:48:33.000000 meerschaum-2.1.7/meerschaum/utils/misc.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1006 2022-02-28 20:55:01.000000 meerschaum-2.1.7/meerschaum/utils/networking.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-01-08 03:49:02.476344 meerschaum-2.1.7/meerschaum/utils/packages/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    56534 2024-01-08 03:48:33.000000 meerschaum-2.1.7/meerschaum/utils/packages/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7967 2024-01-08 03:17:41.000000 meerschaum-2.1.7/meerschaum/utils/packages/_packages.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2540 2022-07-25 06:37:48.000000 meerschaum-2.1.7/meerschaum/utils/packages/lazy_loader.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2655 2023-12-01 07:12:21.000000 meerschaum-2.1.7/meerschaum/utils/pool.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7098 2023-10-04 03:17:38.000000 meerschaum-2.1.7/meerschaum/utils/process.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    16490 2023-09-25 20:34:26.000000 meerschaum-2.1.7/meerschaum/utils/prompt.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1951 2023-11-26 03:23:44.000000 meerschaum-2.1.7/meerschaum/utils/schedule.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    46656 2023-12-04 02:32:59.000000 meerschaum-2.1.7/meerschaum/utils/sql.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2472 2023-09-25 20:34:26.000000 meerschaum-2.1.7/meerschaum/utils/threading.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2784 2023-12-04 02:32:59.000000 meerschaum-2.1.7/meerschaum/utils/typing.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-01-08 03:49:02.476344 meerschaum-2.1.7/meerschaum/utils/venv/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3553 2023-08-28 22:18:25.000000 meerschaum-2.1.7/meerschaum/utils/venv/_Venv.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    23183 2023-12-01 07:12:21.000000 meerschaum-2.1.7/meerschaum/utils/venv/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6535 2023-08-24 14:21:38.000000 meerschaum-2.1.7/meerschaum/utils/warnings.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3162 2023-01-09 09:23:24.000000 meerschaum-2.1.7/meerschaum/utils/yaml.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-01-08 03:49:02.477344 meerschaum-2.1.7/meerschaum.egg-info/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    23451 2024-01-08 03:49:02.000000 meerschaum-2.1.7/meerschaum.egg-info/PKG-INFO
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     8405 2024-01-08 03:49:02.000000 meerschaum-2.1.7/meerschaum.egg-info/SOURCES.txt
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        1 2024-01-08 03:49:02.000000 meerschaum-2.1.7/meerschaum.egg-info/dependency_links.txt
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)       88 2024-01-08 03:49:02.000000 meerschaum-2.1.7/meerschaum.egg-info/entry_points.txt
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4713 2024-01-08 03:49:02.000000 meerschaum-2.1.7/meerschaum.egg-info/requires.txt
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)       11 2024-01-08 03:49:02.000000 meerschaum-2.1.7/meerschaum.egg-info/top_level.txt
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        1 2024-01-08 03:49:02.000000 meerschaum-2.1.7/meerschaum.egg-info/zip-safe
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)       38 2024-01-08 03:49:02.515344 meerschaum-2.1.7/setup.cfg
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3106 2023-08-28 22:18:03.000000 meerschaum-2.1.7/setup.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-01-08 03:49:02.477344 meerschaum-2.1.7/tests/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3139 2023-11-13 16:31:14.000000 meerschaum-2.1.7/tests/test_deduplicate.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    15351 2023-11-13 21:37:33.000000 meerschaum-2.1.7/tests/test_pipes_dtypes.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3646 2023-09-25 20:34:26.000000 meerschaum-2.1.7/tests/test_sql.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    21641 2023-12-04 02:32:59.000000 meerschaum-2.1.7/tests/test_sync.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      744 2023-09-25 20:34:26.000000 meerschaum-2.1.7/tests/test_users.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3090 2023-09-25 20:34:26.000000 meerschaum-2.1.7/tests/test_verify.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-10 03:58:42.739412 meerschaum-2.2.0.dev1/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    11359 2021-12-27 13:50:47.000000 meerschaum-2.2.0.dev1/LICENSE
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      114 2021-12-27 13:50:47.000000 meerschaum-2.2.0.dev1/NOTICE
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    23460 2024-05-10 03:58:42.738412 meerschaum-2.2.0.dev1/PKG-INFO
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9183 2023-12-01 07:12:21.000000 meerschaum-2.2.0.dev1/README.md
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-10 03:58:42.689412 meerschaum-2.2.0.dev1/meerschaum/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1487 2023-11-26 03:23:44.000000 meerschaum-2.2.0.dev1/meerschaum/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2763 2023-12-01 07:12:21.000000 meerschaum-2.2.0.dev1/meerschaum/__main__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-10 03:58:42.690412 meerschaum-2.2.0.dev1/meerschaum/_internal/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      169 2022-04-23 01:15:00.000000 meerschaum-2.2.0.dev1/meerschaum/_internal/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-10 03:58:42.690412 meerschaum-2.2.0.dev1/meerschaum/_internal/arguments/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      519 2022-10-22 06:25:53.000000 meerschaum-2.2.0.dev1/meerschaum/_internal/arguments/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    10249 2023-09-25 20:34:26.000000 meerschaum-2.2.0.dev1/meerschaum/_internal/arguments/_parse_arguments.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    13719 2024-05-07 20:25:34.000000 meerschaum-2.2.0.dev1/meerschaum/_internal/arguments/_parser.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-10 03:58:42.691412 meerschaum-2.2.0.dev1/meerschaum/_internal/docs/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      126 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev1/meerschaum/_internal/docs/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7076 2023-12-01 07:12:21.000000 meerschaum-2.2.0.dev1/meerschaum/_internal/docs/index.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4824 2024-03-06 17:41:41.000000 meerschaum-2.2.0.dev1/meerschaum/_internal/entry.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-10 03:58:42.691412 meerschaum-2.2.0.dev1/meerschaum/_internal/gui/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1313 2023-08-24 14:21:38.000000 meerschaum-2.2.0.dev1/meerschaum/_internal/gui/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-10 03:58:42.691412 meerschaum-2.2.0.dev1/meerschaum/_internal/gui/app/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1565 2022-04-24 10:29:36.000000 meerschaum-2.2.0.dev1/meerschaum/_internal/gui/app/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2632 2022-10-18 06:13:35.000000 meerschaum-2.2.0.dev1/meerschaum/_internal/gui/app/_windows.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      935 2023-08-24 14:21:38.000000 meerschaum-2.2.0.dev1/meerschaum/_internal/gui/app/actions.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1596 2023-08-24 14:21:38.000000 meerschaum-2.2.0.dev1/meerschaum/_internal/gui/app/pipes.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-10 03:58:42.691412 meerschaum-2.2.0.dev1/meerschaum/_internal/shell/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    32826 2024-01-08 03:48:33.000000 meerschaum-2.2.0.dev1/meerschaum/_internal/shell/Shell.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3114 2023-11-26 03:23:44.000000 meerschaum-2.2.0.dev1/meerschaum/_internal/shell/ShellCompleter.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1280 2022-10-26 04:20:20.000000 meerschaum-2.2.0.dev1/meerschaum/_internal/shell/ValidAutoSuggest.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      281 2022-04-24 10:29:36.000000 meerschaum-2.2.0.dev1/meerschaum/_internal/shell/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-10 03:58:42.691412 meerschaum-2.2.0.dev1/meerschaum/_internal/shell/resources/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2022-04-24 10:29:36.000000 meerschaum-2.2.0.dev1/meerschaum/_internal/shell/resources/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-10 03:58:42.692412 meerschaum-2.2.0.dev1/meerschaum/_internal/term/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      520 2023-12-01 07:12:21.000000 meerschaum-2.2.0.dev1/meerschaum/_internal/term/TermPageHandler.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1594 2023-11-06 21:03:03.000000 meerschaum-2.2.0.dev1/meerschaum/_internal/term/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      716 2023-08-24 14:21:38.000000 meerschaum-2.2.0.dev1/meerschaum/_internal/term/tools.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-10 03:58:42.695412 meerschaum-2.2.0.dev1/meerschaum/actions/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    11360 2023-11-26 03:23:44.000000 meerschaum-2.2.0.dev1/meerschaum/actions/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    12756 2024-01-08 03:48:33.000000 meerschaum-2.2.0.dev1/meerschaum/actions/api.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    13396 2023-11-13 16:31:14.000000 meerschaum-2.2.0.dev1/meerschaum/actions/bootstrap.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4851 2023-09-25 20:34:26.000000 meerschaum-2.2.0.dev1/meerschaum/actions/clear.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6213 2023-09-25 20:34:26.000000 meerschaum-2.2.0.dev1/meerschaum/actions/copy.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1167 2023-09-25 20:34:26.000000 meerschaum-2.2.0.dev1/meerschaum/actions/deduplicate.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    15528 2023-11-13 16:31:14.000000 meerschaum-2.2.0.dev1/meerschaum/actions/delete.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2453 2023-09-25 20:34:26.000000 meerschaum-2.2.0.dev1/meerschaum/actions/drop.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9487 2023-09-25 20:34:26.000000 meerschaum-2.2.0.dev1/meerschaum/actions/edit.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7431 2024-05-07 20:26:48.000000 meerschaum-2.2.0.dev1/meerschaum/actions/install.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4206 2023-09-21 17:52:19.000000 meerschaum-2.2.0.dev1/meerschaum/actions/login.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2251 2022-08-29 21:54:10.000000 meerschaum-2.2.0.dev1/meerschaum/actions/os.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3909 2023-11-13 21:37:33.000000 meerschaum-2.2.0.dev1/meerschaum/actions/pause.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2395 2022-02-28 20:55:01.000000 meerschaum-2.2.0.dev1/meerschaum/actions/python.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    11326 2023-12-01 07:12:21.000000 meerschaum-2.2.0.dev1/meerschaum/actions/register.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      508 2023-11-26 03:23:44.000000 meerschaum-2.2.0.dev1/meerschaum/actions/reload.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3205 2023-09-25 20:34:26.000000 meerschaum-2.2.0.dev1/meerschaum/actions/setup.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2026 2022-08-29 21:54:10.000000 meerschaum-2.2.0.dev1/meerschaum/actions/sh.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    26212 2023-12-01 07:12:21.000000 meerschaum-2.2.0.dev1/meerschaum/actions/show.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4311 2023-10-27 06:03:46.000000 meerschaum-2.2.0.dev1/meerschaum/actions/sql.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5886 2023-08-28 22:18:25.000000 meerschaum-2.2.0.dev1/meerschaum/actions/stack.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    18384 2023-11-06 21:03:03.000000 meerschaum-2.2.0.dev1/meerschaum/actions/start.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4311 2023-09-25 20:34:26.000000 meerschaum-2.2.0.dev1/meerschaum/actions/stop.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    17518 2024-03-26 19:47:08.000000 meerschaum-2.2.0.dev1/meerschaum/actions/sync.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3053 2023-12-01 07:12:21.000000 meerschaum-2.2.0.dev1/meerschaum/actions/tag.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6068 2023-09-25 20:34:26.000000 meerschaum-2.2.0.dev1/meerschaum/actions/uninstall.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6302 2023-09-25 20:34:26.000000 meerschaum-2.2.0.dev1/meerschaum/actions/upgrade.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4885 2023-09-25 20:34:26.000000 meerschaum-2.2.0.dev1/meerschaum/actions/verify.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-10 03:58:42.695412 meerschaum-2.2.0.dev1/meerschaum/api/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7694 2023-12-01 07:12:21.000000 meerschaum-2.2.0.dev1/meerschaum/api/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      875 2022-02-28 20:55:01.000000 meerschaum-2.2.0.dev1/meerschaum/api/_chain.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1603 2023-08-24 14:21:38.000000 meerschaum-2.2.0.dev1/meerschaum/api/_events.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      961 2023-08-24 00:13:16.000000 meerschaum-2.2.0.dev1/meerschaum/api/_oauth2.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1609 2023-11-06 21:03:03.000000 meerschaum-2.2.0.dev1/meerschaum/api/_websockets.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-10 03:58:42.696412 meerschaum-2.2.0.dev1/meerschaum/api/dash/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2252 2024-03-20 22:38:46.000000 meerschaum-2.2.0.dev1/meerschaum/api/dash/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9418 2023-09-25 20:34:26.000000 meerschaum-2.2.0.dev1/meerschaum/api/dash/actions.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-10 03:58:42.697412 meerschaum-2.2.0.dev1/meerschaum/api/dash/assets/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev1/meerschaum/api/dash/assets/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    21923 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev1/meerschaum/api/dash/assets/ansi_up.js
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)   338636 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev1/meerschaum/api/dash/assets/banner_1920x320.png
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9662 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev1/meerschaum/api/dash/assets/favicon.ico
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    10218 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev1/meerschaum/api/dash/assets/logo_48x48.png
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    67702 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev1/meerschaum/api/dash/assets/logo_500x500.png
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-10 03:58:42.698413 meerschaum-2.2.0.dev1/meerschaum/api/dash/callbacks/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      325 2023-09-25 20:34:26.000000 meerschaum-2.2.0.dev1/meerschaum/api/dash/callbacks/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    32206 2024-05-10 03:51:40.000000 meerschaum-2.2.0.dev1/meerschaum/api/dash/callbacks/dashboard.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7689 2024-05-10 01:45:18.000000 meerschaum-2.2.0.dev1/meerschaum/api/dash/callbacks/jobs.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2613 2023-08-24 14:21:38.000000 meerschaum-2.2.0.dev1/meerschaum/api/dash/callbacks/login.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2777 2022-07-26 06:45:25.000000 meerschaum-2.2.0.dev1/meerschaum/api/dash/callbacks/plugins.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3600 2023-08-24 14:21:38.000000 meerschaum-2.2.0.dev1/meerschaum/api/dash/callbacks/register.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6364 2023-11-06 21:03:03.000000 meerschaum-2.2.0.dev1/meerschaum/api/dash/components.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      843 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev1/meerschaum/api/dash/connectors.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2046 2023-08-24 14:21:38.000000 meerschaum-2.2.0.dev1/meerschaum/api/dash/graphs.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7529 2024-05-10 02:30:25.000000 meerschaum-2.2.0.dev1/meerschaum/api/dash/jobs.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    12591 2023-11-26 03:23:44.000000 meerschaum-2.2.0.dev1/meerschaum/api/dash/keys.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-10 03:58:42.698413 meerschaum-2.2.0.dev1/meerschaum/api/dash/pages/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      273 2023-07-21 01:07:38.000000 meerschaum-2.2.0.dev1/meerschaum/api/dash/pages/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3930 2023-11-26 03:23:44.000000 meerschaum-2.2.0.dev1/meerschaum/api/dash/pages/dashboard.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      595 2023-08-24 14:21:38.000000 meerschaum-2.2.0.dev1/meerschaum/api/dash/pages/error.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4600 2023-10-04 04:03:08.000000 meerschaum-2.2.0.dev1/meerschaum/api/dash/pages/login.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1549 2023-08-24 14:21:38.000000 meerschaum-2.2.0.dev1/meerschaum/api/dash/pages/plugins.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2364 2023-08-24 14:21:38.000000 meerschaum-2.2.0.dev1/meerschaum/api/dash/pages/register.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    17599 2024-05-10 02:32:14.000000 meerschaum-2.2.0.dev1/meerschaum/api/dash/pipes.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3115 2023-08-24 14:21:38.000000 meerschaum-2.2.0.dev1/meerschaum/api/dash/plugins.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      504 2022-07-26 06:45:25.000000 meerschaum-2.2.0.dev1/meerschaum/api/dash/sync.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2362 2023-11-06 21:03:03.000000 meerschaum-2.2.0.dev1/meerschaum/api/dash/users.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      924 2022-10-31 13:18:31.000000 meerschaum-2.2.0.dev1/meerschaum/api/dash/websockets.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3298 2023-11-06 21:03:03.000000 meerschaum-2.2.0.dev1/meerschaum/api/dash/webterm.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-10 03:58:42.699412 meerschaum-2.2.0.dev1/meerschaum/api/models/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      276 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev1/meerschaum/api/models/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      263 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev1/meerschaum/api/models/_interfaces.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      304 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev1/meerschaum/api/models/_locations.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      295 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev1/meerschaum/api/models/_metrics.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      463 2021-11-20 21:54:59.000000 meerschaum-2.2.0.dev1/meerschaum/api/models/_pipes.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-10 03:58:42.699412 meerschaum-2.2.0.dev1/meerschaum/api/resources/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      115 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev1/meerschaum/api/resources/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-10 03:58:42.699412 meerschaum-2.2.0.dev1/meerschaum/api/resources/static/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev1/meerschaum/api/resources/static/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-10 03:58:42.699412 meerschaum-2.2.0.dev1/meerschaum/api/resources/static/css/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev1/meerschaum/api/resources/static/css/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)   180286 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev1/meerschaum/api/resources/static/css/bootstrap.min.css
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1714 2023-09-25 20:34:26.000000 meerschaum-2.2.0.dev1/meerschaum/api/resources/static/css/dash.css
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6087 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev1/meerschaum/api/resources/static/css/dbc_dark.css
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)       81 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev1/meerschaum/api/resources/static/css/styles.css
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5383 2023-11-06 21:03:03.000000 meerschaum-2.2.0.dev1/meerschaum/api/resources/static/css/xterm.css
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-10 03:58:42.700412 meerschaum-2.2.0.dev1/meerschaum/api/resources/static/ico/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev1/meerschaum/api/resources/static/ico/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9662 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev1/meerschaum/api/resources/static/ico/logo.ico
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-10 03:58:42.700412 meerschaum-2.2.0.dev1/meerschaum/api/resources/static/js/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev1/meerschaum/api/resources/static/js/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      540 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev1/meerschaum/api/resources/static/js/action_button.js
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev1/meerschaum/api/resources/static/js/main.js
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1729 2023-11-06 21:03:03.000000 meerschaum-2.2.0.dev1/meerschaum/api/resources/static/js/terminado.js
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)   289441 2024-04-05 14:30:27.000000 meerschaum-2.2.0.dev1/meerschaum/api/resources/static/js/xterm.js
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-10 03:58:42.700412 meerschaum-2.2.0.dev1/meerschaum/api/resources/static/png/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev1/meerschaum/api/resources/static/png/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-10 03:58:42.701412 meerschaum-2.2.0.dev1/meerschaum/api/resources/templates/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev1/meerschaum/api/resources/templates/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1019 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev1/meerschaum/api/resources/templates/index.html
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1711 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev1/meerschaum/api/resources/templates/old_index.html
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      141 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev1/meerschaum/api/resources/templates/secret.html
+-rwxr-xr-x   0 bmeares   (1000) bmeares   (1000)     4443 2023-11-26 03:23:44.000000 meerschaum-2.2.0.dev1/meerschaum/api/resources/templates/termpage.html
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-10 03:58:42.702412 meerschaum-2.2.0.dev1/meerschaum/api/routes/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      564 2023-08-24 14:21:38.000000 meerschaum-2.2.0.dev1/meerschaum/api/routes/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2240 2022-06-27 01:07:31.000000 meerschaum-2.2.0.dev1/meerschaum/api/routes/_actions.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1849 2023-10-04 04:03:08.000000 meerschaum-2.2.0.dev1/meerschaum/api/routes/_connectors.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      578 2022-02-28 20:55:01.000000 meerschaum-2.2.0.dev1/meerschaum/api/routes/_index.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1935 2023-12-01 07:12:21.000000 meerschaum-2.2.0.dev1/meerschaum/api/routes/_login.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2469 2023-08-24 14:21:38.000000 meerschaum-2.2.0.dev1/meerschaum/api/routes/_misc.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    21677 2023-11-13 16:31:14.000000 meerschaum-2.2.0.dev1/meerschaum/api/routes/_pipes.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6151 2023-08-24 14:21:38.000000 meerschaum-2.2.0.dev1/meerschaum/api/routes/_plugins.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7204 2023-08-24 00:13:16.000000 meerschaum-2.2.0.dev1/meerschaum/api/routes/_users.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      825 2022-06-27 01:07:31.000000 meerschaum-2.2.0.dev1/meerschaum/api/routes/_version.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3909 2023-11-06 21:03:03.000000 meerschaum-2.2.0.dev1/meerschaum/api/routes/_webterm.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-10 03:58:42.702412 meerschaum-2.2.0.dev1/meerschaum/api/tables/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      482 2023-10-26 06:22:59.000000 meerschaum-2.2.0.dev1/meerschaum/api/tables/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-10 03:58:42.704412 meerschaum-2.2.0.dev1/meerschaum/config/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    11517 2023-11-13 16:31:14.000000 meerschaum-2.2.0.dev1/meerschaum/config/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5184 2023-11-13 16:31:14.000000 meerschaum-2.2.0.dev1/meerschaum/config/_default.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     8218 2023-11-26 03:23:44.000000 meerschaum-2.2.0.dev1/meerschaum/config/_edit.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4419 2023-11-06 21:03:03.000000 meerschaum-2.2.0.dev1/meerschaum/config/_environment.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6635 2023-12-01 07:12:21.000000 meerschaum-2.2.0.dev1/meerschaum/config/_formatting.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1073 2023-09-25 20:34:26.000000 meerschaum-2.2.0.dev1/meerschaum/config/_jobs.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1526 2023-11-06 21:03:03.000000 meerschaum-2.2.0.dev1/meerschaum/config/_patch.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7983 2023-11-06 21:03:03.000000 meerschaum-2.2.0.dev1/meerschaum/config/_paths.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1220 2022-02-28 20:55:01.000000 meerschaum-2.2.0.dev1/meerschaum/config/_preprocess.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    14720 2023-09-25 20:34:26.000000 meerschaum-2.2.0.dev1/meerschaum/config/_read_config.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3551 2024-01-08 03:48:33.000000 meerschaum-2.2.0.dev1/meerschaum/config/_shell.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4120 2023-08-28 22:18:25.000000 meerschaum-2.2.0.dev1/meerschaum/config/_sync.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)       76 2024-05-10 03:56:14.000000 meerschaum-2.2.0.dev1/meerschaum/config/_version.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-10 03:58:42.704412 meerschaum-2.2.0.dev1/meerschaum/config/resources/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev1/meerschaum/config/resources/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-10 03:58:42.704412 meerschaum-2.2.0.dev1/meerschaum/config/stack/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9034 2023-08-28 22:18:25.000000 meerschaum-2.2.0.dev1/meerschaum/config/stack/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-10 03:58:42.704412 meerschaum-2.2.0.dev1/meerschaum/config/stack/grafana/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2010 2022-11-01 03:52:40.000000 meerschaum-2.2.0.dev1/meerschaum/config/stack/grafana/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-10 03:58:42.704412 meerschaum-2.2.0.dev1/meerschaum/config/stack/mosquitto/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      186 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev1/meerschaum/config/stack/mosquitto/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-10 03:58:42.704412 meerschaum-2.2.0.dev1/meerschaum/config/stack/mosquitto/resources/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev1/meerschaum/config/stack/mosquitto/resources/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-10 03:58:42.704412 meerschaum-2.2.0.dev1/meerschaum/config/stack/resources/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev1/meerschaum/config/stack/resources/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-10 03:58:42.704412 meerschaum-2.2.0.dev1/meerschaum/config/static/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4361 2023-11-26 03:23:44.000000 meerschaum-2.2.0.dev1/meerschaum/config/static/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-10 03:58:42.705412 meerschaum-2.2.0.dev1/meerschaum/connectors/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6381 2023-04-25 23:57:31.000000 meerschaum-2.2.0.dev1/meerschaum/connectors/Connector.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    12023 2023-10-04 04:03:08.000000 meerschaum-2.2.0.dev1/meerschaum/connectors/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-10 03:58:42.706412 meerschaum-2.2.0.dev1/meerschaum/connectors/api/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4355 2023-12-01 07:12:21.000000 meerschaum-2.2.0.dev1/meerschaum/connectors/api/APIConnector.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      205 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev1/meerschaum/connectors/api/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2755 2023-08-28 22:18:25.000000 meerschaum-2.2.0.dev1/meerschaum/connectors/api/_actions.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2072 2023-09-25 20:34:26.000000 meerschaum-2.2.0.dev1/meerschaum/connectors/api/_fetch.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2050 2023-08-28 22:18:25.000000 meerschaum-2.2.0.dev1/meerschaum/connectors/api/_login.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1093 2023-08-28 22:18:25.000000 meerschaum-2.2.0.dev1/meerschaum/connectors/api/_misc.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    20962 2023-11-10 05:44:22.000000 meerschaum-2.2.0.dev1/meerschaum/connectors/api/_pipes.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5217 2024-05-07 20:27:04.000000 meerschaum-2.2.0.dev1/meerschaum/connectors/api/_plugins.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6922 2023-10-04 04:03:08.000000 meerschaum-2.2.0.dev1/meerschaum/connectors/api/_request.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1489 2022-07-25 06:37:48.000000 meerschaum-2.2.0.dev1/meerschaum/connectors/api/_uri.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5275 2023-08-28 22:18:25.000000 meerschaum-2.2.0.dev1/meerschaum/connectors/api/_users.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4044 2023-08-28 22:18:25.000000 meerschaum-2.2.0.dev1/meerschaum/connectors/parse.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-10 03:58:42.706412 meerschaum-2.2.0.dev1/meerschaum/connectors/plugin/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2084 2022-10-25 06:38:00.000000 meerschaum-2.2.0.dev1/meerschaum/connectors/plugin/PluginConnector.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      198 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev1/meerschaum/connectors/plugin/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7363 2023-08-24 14:21:38.000000 meerschaum-2.2.0.dev1/meerschaum/connectors/poll.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-10 03:58:42.707412 meerschaum-2.2.0.dev1/meerschaum/connectors/sql/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    11522 2023-11-13 16:31:14.000000 meerschaum-2.2.0.dev1/meerschaum/connectors/sql/SQLConnector.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      175 2021-11-08 16:07:48.000000 meerschaum-2.2.0.dev1/meerschaum/connectors/sql/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4123 2023-11-13 16:31:14.000000 meerschaum-2.2.0.dev1/meerschaum/connectors/sql/_cli.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    10375 2024-03-26 20:20:31.000000 meerschaum-2.2.0.dev1/meerschaum/connectors/sql/_create_engine.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    13086 2024-01-08 03:48:33.000000 meerschaum-2.2.0.dev1/meerschaum/connectors/sql/_fetch.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6447 2023-11-13 16:31:14.000000 meerschaum-2.2.0.dev1/meerschaum/connectors/sql/_instance.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)   100925 2024-01-08 03:48:33.000000 meerschaum-2.2.0.dev1/meerschaum/connectors/sql/_pipes.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     8323 2023-09-25 20:34:26.000000 meerschaum-2.2.0.dev1/meerschaum/connectors/sql/_plugins.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    34262 2023-11-13 16:31:14.000000 meerschaum-2.2.0.dev1/meerschaum/connectors/sql/_sql.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3460 2023-10-26 06:22:59.000000 meerschaum-2.2.0.dev1/meerschaum/connectors/sql/_uri.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    10100 2023-11-13 16:31:14.000000 meerschaum-2.2.0.dev1/meerschaum/connectors/sql/_users.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-10 03:58:42.708412 meerschaum-2.2.0.dev1/meerschaum/connectors/sql/tables/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9001 2023-12-04 02:32:59.000000 meerschaum-2.2.0.dev1/meerschaum/connectors/sql/tables/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1573 2022-02-28 20:55:01.000000 meerschaum-2.2.0.dev1/meerschaum/connectors/sql/tables/types.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      187 2022-04-24 10:29:36.000000 meerschaum-2.2.0.dev1/meerschaum/connectors/sql/tools.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-10 03:58:42.708412 meerschaum-2.2.0.dev1/meerschaum/core/
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-10 03:58:42.709412 meerschaum-2.2.0.dev1/meerschaum/core/Pipe/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    16230 2023-12-01 07:12:21.000000 meerschaum-2.2.0.dev1/meerschaum/core/Pipe/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    13202 2023-04-26 08:12:59.000000 meerschaum-2.2.0.dev1/meerschaum/core/Pipe/_attributes.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7613 2023-04-25 23:57:31.000000 meerschaum-2.2.0.dev1/meerschaum/core/Pipe/_bootstrap.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2261 2023-09-25 20:34:26.000000 meerschaum-2.2.0.dev1/meerschaum/core/Pipe/_clear.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    20880 2023-12-04 02:32:59.000000 meerschaum-2.2.0.dev1/meerschaum/core/Pipe/_data.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    10267 2023-11-13 06:20:00.000000 meerschaum-2.2.0.dev1/meerschaum/core/Pipe/_deduplicate.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2118 2023-11-13 16:31:14.000000 meerschaum-2.2.0.dev1/meerschaum/core/Pipe/_delete.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1052 2023-09-25 20:34:26.000000 meerschaum-2.2.0.dev1/meerschaum/core/Pipe/_drop.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3694 2024-01-08 03:48:33.000000 meerschaum-2.2.0.dev1/meerschaum/core/Pipe/_dtypes.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     8471 2022-12-05 04:26:42.000000 meerschaum-2.2.0.dev1/meerschaum/core/Pipe/_edit.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5234 2023-11-26 03:23:44.000000 meerschaum-2.2.0.dev1/meerschaum/core/Pipe/_fetch.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2240 2023-01-16 21:21:28.000000 meerschaum-2.2.0.dev1/meerschaum/core/Pipe/_register.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1352 2023-04-25 23:57:31.000000 meerschaum-2.2.0.dev1/meerschaum/core/Pipe/_show.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    28038 2024-01-08 03:48:33.000000 meerschaum-2.2.0.dev1/meerschaum/core/Pipe/_sync.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    14262 2023-11-13 16:31:14.000000 meerschaum-2.2.0.dev1/meerschaum/core/Pipe/_verify.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-10 03:58:42.709412 meerschaum-2.2.0.dev1/meerschaum/core/Plugin/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      137 2022-04-24 10:29:36.000000 meerschaum-2.2.0.dev1/meerschaum/core/Plugin/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-10 03:58:42.710412 meerschaum-2.2.0.dev1/meerschaum/core/User/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2448 2023-08-28 22:18:25.000000 meerschaum-2.2.0.dev1/meerschaum/core/User/_User.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      161 2022-04-24 10:29:36.000000 meerschaum-2.2.0.dev1/meerschaum/core/User/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      251 2022-04-24 10:29:36.000000 meerschaum-2.2.0.dev1/meerschaum/core/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-10 03:58:42.710412 meerschaum-2.2.0.dev1/meerschaum/plugins/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    34013 2024-05-07 20:28:41.000000 meerschaum-2.2.0.dev1/meerschaum/plugins/_Plugin.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    20760 2023-11-26 03:23:44.000000 meerschaum-2.2.0.dev1/meerschaum/plugins/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-10 03:58:42.711412 meerschaum-2.2.0.dev1/meerschaum/utils/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      612 2023-12-01 07:12:21.000000 meerschaum-2.2.0.dev1/meerschaum/utils/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    11460 2023-12-01 07:12:21.000000 meerschaum-2.2.0.dev1/meerschaum/utils/_get_pipes.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-10 03:58:42.712412 meerschaum-2.2.0.dev1/meerschaum/utils/daemon/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    32192 2024-03-26 19:31:51.000000 meerschaum-2.2.0.dev1/meerschaum/utils/daemon/Daemon.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    19362 2023-11-06 21:03:03.000000 meerschaum-2.2.0.dev1/meerschaum/utils/daemon/RotatingFile.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     8174 2023-11-26 03:23:44.000000 meerschaum-2.2.0.dev1/meerschaum/utils/daemon/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4330 2023-09-26 04:28:45.000000 meerschaum-2.2.0.dev1/meerschaum/utils/daemon/_names.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    31955 2024-01-08 03:48:33.000000 meerschaum-2.2.0.dev1/meerschaum/utils/dataframe.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3690 2023-01-09 09:23:24.000000 meerschaum-2.2.0.dev1/meerschaum/utils/debug.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-10 03:58:42.712412 meerschaum-2.2.0.dev1/meerschaum/utils/dtypes/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6261 2024-03-26 20:33:15.000000 meerschaum-2.2.0.dev1/meerschaum/utils/dtypes/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    14638 2023-11-13 16:31:14.000000 meerschaum-2.2.0.dev1/meerschaum/utils/dtypes/sql.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-10 03:58:42.713412 meerschaum-2.2.0.dev1/meerschaum/utils/formatting/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    13778 2023-11-26 03:23:44.000000 meerschaum-2.2.0.dev1/meerschaum/utils/formatting/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3294 2023-09-25 20:34:26.000000 meerschaum-2.2.0.dev1/meerschaum/utils/formatting/_jobs.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    19492 2024-01-08 03:48:33.000000 meerschaum-2.2.0.dev1/meerschaum/utils/formatting/_pipes.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3096 2023-09-25 20:34:26.000000 meerschaum-2.2.0.dev1/meerschaum/utils/formatting/_pprint.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3677 2023-08-24 14:21:38.000000 meerschaum-2.2.0.dev1/meerschaum/utils/formatting/_shell.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3196 2023-12-01 07:12:21.000000 meerschaum-2.2.0.dev1/meerschaum/utils/interactive.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    43296 2024-01-08 03:48:33.000000 meerschaum-2.2.0.dev1/meerschaum/utils/misc.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1006 2022-02-28 20:55:01.000000 meerschaum-2.2.0.dev1/meerschaum/utils/networking.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-10 03:58:42.713412 meerschaum-2.2.0.dev1/meerschaum/utils/packages/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    56534 2024-03-20 22:39:01.000000 meerschaum-2.2.0.dev1/meerschaum/utils/packages/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7968 2024-03-26 20:22:08.000000 meerschaum-2.2.0.dev1/meerschaum/utils/packages/_packages.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2540 2022-07-25 06:37:48.000000 meerschaum-2.2.0.dev1/meerschaum/utils/packages/lazy_loader.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2655 2023-12-01 07:12:21.000000 meerschaum-2.2.0.dev1/meerschaum/utils/pool.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7098 2023-10-04 03:17:38.000000 meerschaum-2.2.0.dev1/meerschaum/utils/process.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    16490 2023-09-25 20:34:26.000000 meerschaum-2.2.0.dev1/meerschaum/utils/prompt.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1951 2023-11-26 03:23:44.000000 meerschaum-2.2.0.dev1/meerschaum/utils/schedule.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    46656 2023-12-04 02:32:59.000000 meerschaum-2.2.0.dev1/meerschaum/utils/sql.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2472 2023-09-25 20:34:26.000000 meerschaum-2.2.0.dev1/meerschaum/utils/threading.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2807 2024-03-20 22:41:20.000000 meerschaum-2.2.0.dev1/meerschaum/utils/typing.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-10 03:58:42.713412 meerschaum-2.2.0.dev1/meerschaum/utils/venv/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3553 2023-08-28 22:18:25.000000 meerschaum-2.2.0.dev1/meerschaum/utils/venv/_Venv.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    23183 2023-12-01 07:12:21.000000 meerschaum-2.2.0.dev1/meerschaum/utils/venv/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6535 2023-08-24 14:21:38.000000 meerschaum-2.2.0.dev1/meerschaum/utils/warnings.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3162 2023-01-09 09:23:24.000000 meerschaum-2.2.0.dev1/meerschaum/utils/yaml.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-10 03:58:42.714412 meerschaum-2.2.0.dev1/meerschaum.egg-info/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    23460 2024-05-10 03:58:42.000000 meerschaum-2.2.0.dev1/meerschaum.egg-info/PKG-INFO
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     8405 2024-05-10 03:58:42.000000 meerschaum-2.2.0.dev1/meerschaum.egg-info/SOURCES.txt
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        1 2024-05-10 03:58:42.000000 meerschaum-2.2.0.dev1/meerschaum.egg-info/dependency_links.txt
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)       88 2024-05-10 03:58:42.000000 meerschaum-2.2.0.dev1/meerschaum.egg-info/entry_points.txt
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4717 2024-05-10 03:58:42.000000 meerschaum-2.2.0.dev1/meerschaum.egg-info/requires.txt
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)       11 2024-05-10 03:58:42.000000 meerschaum-2.2.0.dev1/meerschaum.egg-info/top_level.txt
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        1 2024-05-10 03:58:42.000000 meerschaum-2.2.0.dev1/meerschaum.egg-info/zip-safe
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)       38 2024-05-10 03:58:42.739412 meerschaum-2.2.0.dev1/setup.cfg
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3106 2023-08-28 22:18:03.000000 meerschaum-2.2.0.dev1/setup.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-10 03:58:42.714412 meerschaum-2.2.0.dev1/tests/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3139 2023-11-13 16:31:14.000000 meerschaum-2.2.0.dev1/tests/test_deduplicate.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    15351 2023-11-13 21:37:33.000000 meerschaum-2.2.0.dev1/tests/test_pipes_dtypes.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3646 2023-09-25 20:34:26.000000 meerschaum-2.2.0.dev1/tests/test_sql.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    21641 2023-12-04 02:32:59.000000 meerschaum-2.2.0.dev1/tests/test_sync.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      744 2023-09-25 20:34:26.000000 meerschaum-2.2.0.dev1/tests/test_users.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3090 2023-09-25 20:34:26.000000 meerschaum-2.2.0.dev1/tests/test_verify.py
```

### Comparing `meerschaum-2.1.7/LICENSE` & `meerschaum-2.2.0.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/PKG-INFO` & `meerschaum-2.2.0.dev1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meerschaum
-Version: 2.1.7
+Version: 2.2.0.dev1
 Summary: Sync Time-Series Pipes with Meerschaum
 Home-page: https://meerschaum.io
 Author: Bennett Meares
 Author-email: bennett.meares@gmail.com
 Maintainer-email: bennett.meares@gmail.com
 License: Apache Software License 2.0
 Project-URL: Documentation, https://docs.meerschaum.io
@@ -63,15 +63,15 @@
 Requires-Dist: psutil>=5.8.0; extra == "required"
 Requires-Dist: watchgod>=0.7.0; extra == "required"
 Requires-Dist: dill>=0.3.3; extra == "required"
 Requires-Dist: virtualenv>=20.1.0; extra == "required"
 Requires-Dist: rocketry>=2.5.1; extra == "required"
 Provides-Extra: drivers
 Requires-Dist: cryptography>=38.0.1; extra == "drivers"
-Requires-Dist: psycopg2-binary>=2.8.6; extra == "drivers"
+Requires-Dist: psycopg[binary]>=3.1.18; extra == "drivers"
 Requires-Dist: PyMySQL>=0.9.0; extra == "drivers"
 Requires-Dist: aiomysql>=0.0.21; extra == "drivers"
 Requires-Dist: sqlalchemy-cockroachdb>=2.0.0; extra == "drivers"
 Requires-Dist: duckdb>=0.9.0; extra == "drivers"
 Requires-Dist: duckdb-engine>=0.9.2; extra == "drivers"
 Provides-Extra: drivers
 Requires-Dist: pyodbc>=4.0.30; extra == "drivers"
@@ -124,15 +124,15 @@
 Requires-Dist: pytz; extra == "sql"
 Requires-Dist: joblib>=0.17.0; extra == "sql"
 Requires-Dist: SQLAlchemy>=2.0.5; extra == "sql"
 Requires-Dist: databases>=0.4.0; extra == "sql"
 Requires-Dist: aiosqlite>=0.16.0; extra == "sql"
 Requires-Dist: asyncpg>=0.21.0; extra == "sql"
 Requires-Dist: cryptography>=38.0.1; extra == "sql"
-Requires-Dist: psycopg2-binary>=2.8.6; extra == "sql"
+Requires-Dist: psycopg[binary]>=3.1.18; extra == "sql"
 Requires-Dist: PyMySQL>=0.9.0; extra == "sql"
 Requires-Dist: aiomysql>=0.0.21; extra == "sql"
 Requires-Dist: sqlalchemy-cockroachdb>=2.0.0; extra == "sql"
 Requires-Dist: duckdb>=0.9.0; extra == "sql"
 Requires-Dist: duckdb-engine>=0.9.2; extra == "sql"
 Requires-Dist: wheel>=0.34.2; extra == "sql"
 Requires-Dist: setuptools>=63.3.0; extra == "sql"
@@ -183,15 +183,15 @@
 Requires-Dist: pytz; extra == "api"
 Requires-Dist: joblib>=0.17.0; extra == "api"
 Requires-Dist: SQLAlchemy>=2.0.5; extra == "api"
 Requires-Dist: databases>=0.4.0; extra == "api"
 Requires-Dist: aiosqlite>=0.16.0; extra == "api"
 Requires-Dist: asyncpg>=0.21.0; extra == "api"
 Requires-Dist: cryptography>=38.0.1; extra == "api"
-Requires-Dist: psycopg2-binary>=2.8.6; extra == "api"
+Requires-Dist: psycopg[binary]>=3.1.18; extra == "api"
 Requires-Dist: PyMySQL>=0.9.0; extra == "api"
 Requires-Dist: aiomysql>=0.0.21; extra == "api"
 Requires-Dist: sqlalchemy-cockroachdb>=2.0.0; extra == "api"
 Requires-Dist: duckdb>=0.9.0; extra == "api"
 Requires-Dist: duckdb-engine>=0.9.2; extra == "api"
 Requires-Dist: wheel>=0.34.2; extra == "api"
 Requires-Dist: setuptools>=63.3.0; extra == "api"
@@ -259,15 +259,15 @@
 Requires-Dist: fasteners>=0.18.0; extra == "full"
 Requires-Dist: psutil>=5.8.0; extra == "full"
 Requires-Dist: watchgod>=0.7.0; extra == "full"
 Requires-Dist: dill>=0.3.3; extra == "full"
 Requires-Dist: virtualenv>=20.1.0; extra == "full"
 Requires-Dist: rocketry>=2.5.1; extra == "full"
 Requires-Dist: cryptography>=38.0.1; extra == "full"
-Requires-Dist: psycopg2-binary>=2.8.6; extra == "full"
+Requires-Dist: psycopg[binary]>=3.1.18; extra == "full"
 Requires-Dist: PyMySQL>=0.9.0; extra == "full"
 Requires-Dist: aiomysql>=0.0.21; extra == "full"
 Requires-Dist: sqlalchemy-cockroachdb>=2.0.0; extra == "full"
 Requires-Dist: duckdb>=0.9.0; extra == "full"
 Requires-Dist: duckdb-engine>=0.9.2; extra == "full"
 Requires-Dist: toga>=0.3.0-dev29; extra == "full"
 Requires-Dist: pywebview>=3.6.3; extra == "full"
```

### Comparing `meerschaum-2.1.7/README.md` & `meerschaum-2.2.0.dev1/README.md`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/__init__.py` & `meerschaum-2.2.0.dev1/meerschaum/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/__main__.py` & `meerschaum-2.2.0.dev1/meerschaum/__main__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/_internal/arguments/__init__.py` & `meerschaum-2.2.0.dev1/meerschaum/_internal/arguments/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/_internal/arguments/_parse_arguments.py` & `meerschaum-2.2.0.dev1/meerschaum/_internal/arguments/_parse_arguments.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/_internal/arguments/_parser.py` & `meerschaum-2.2.0.dev1/meerschaum/_internal/arguments/_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -343,14 +343,17 @@
 groups['misc'].add_argument(
     '--patch', action="store_true", help="Patch parameters instead of overwriting."
 )
 groups['misc'].add_argument(
     '--nopretty', action="store_true", help="Print elements without 'pretty' formatting"
 )
 groups['misc'].add_argument(
+    '--skip-deps', action="store_true", help="Skip dependencies when installing plugins.",
+)
+groups['misc'].add_argument(
     '-P', '--params', type=string_to_dict, help=(
         "Parameters dictionary in JSON format or simple format. " +
         "Simple format is for one-depth dictionaries and does not need braces or quotes." +
         "\nJSON Example:\n" +
         "--params '{\"meerschaum\" : { \"connectors\" : " +
         "\"main\" : { \"host\" : \"localhost\" } } }'" +
         "\n\nSimple example:\n" +
```

### Comparing `meerschaum-2.1.7/meerschaum/_internal/docs/index.py` & `meerschaum-2.2.0.dev1/meerschaum/_internal/docs/index.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/_internal/entry.py` & `meerschaum-2.2.0.dev1/meerschaum/_internal/entry.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 #! /usr/bin/env python
 # -*- coding: utf-8 -*-
 # vim:fenc=utf-8
+# type: ignore
 
 """
 The entry point for launching Meerschaum actions.
 """
 
 from __future__ import annotations
 from meerschaum.utils.typing import SuccessTuple, List, Optional, Dict
@@ -57,15 +58,15 @@
         **kw
     ) -> SuccessTuple:
     """Execute a Meerschaum action with keyword arguments.
     Use `_entry()` for parsing sysargs before executing.
     """
     import sys
     from meerschaum.plugins import Plugin
-    from meerschaum.actions import get_shell, get_action, get_main_action_name
+    from meerschaum.actions import get_action, get_main_action_name
     from meerschaum._internal.arguments import remove_leading_action
     from meerschaum.utils.venv import Venv, active_venvs, deactivate_venv
     if kw.get('trace', None):
         from meerschaum.utils.misc import debug_trace
         debug_trace()
     if (
         len(kw.get('action', [])) == 0
```

### Comparing `meerschaum-2.1.7/meerschaum/_internal/gui/__init__.py` & `meerschaum-2.2.0.dev1/meerschaum/_internal/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/_internal/gui/app/__init__.py` & `meerschaum-2.2.0.dev1/meerschaum/_internal/gui/app/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/_internal/gui/app/_windows.py` & `meerschaum-2.2.0.dev1/meerschaum/_internal/gui/app/_windows.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/_internal/gui/app/actions.py` & `meerschaum-2.2.0.dev1/meerschaum/_internal/gui/app/actions.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/_internal/gui/app/pipes.py` & `meerschaum-2.2.0.dev1/meerschaum/_internal/gui/app/pipes.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/_internal/shell/Shell.py` & `meerschaum-2.2.0.dev1/meerschaum/_internal/shell/Shell.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/_internal/shell/ShellCompleter.py` & `meerschaum-2.2.0.dev1/meerschaum/_internal/shell/ShellCompleter.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/_internal/shell/ValidAutoSuggest.py` & `meerschaum-2.2.0.dev1/meerschaum/_internal/shell/ValidAutoSuggest.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/_internal/term/TermPageHandler.py` & `meerschaum-2.2.0.dev1/meerschaum/_internal/term/TermPageHandler.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/_internal/term/__init__.py` & `meerschaum-2.2.0.dev1/meerschaum/_internal/term/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/_internal/term/tools.py` & `meerschaum-2.2.0.dev1/meerschaum/_internal/term/tools.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/actions/__init__.py` & `meerschaum-2.2.0.dev1/meerschaum/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/actions/api.py` & `meerschaum-2.2.0.dev1/meerschaum/actions/api.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/actions/bootstrap.py` & `meerschaum-2.2.0.dev1/meerschaum/actions/bootstrap.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/actions/clear.py` & `meerschaum-2.2.0.dev1/meerschaum/actions/clear.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/actions/copy.py` & `meerschaum-2.2.0.dev1/meerschaum/actions/copy.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/actions/deduplicate.py` & `meerschaum-2.2.0.dev1/meerschaum/actions/deduplicate.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/actions/delete.py` & `meerschaum-2.2.0.dev1/meerschaum/actions/delete.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/actions/drop.py` & `meerschaum-2.2.0.dev1/meerschaum/actions/drop.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/actions/edit.py` & `meerschaum-2.2.0.dev1/meerschaum/actions/edit.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/actions/install.py` & `meerschaum-2.2.0.dev1/meerschaum/actions/install.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,14 +50,15 @@
     from meerschaum._internal.shell import default_action_completer
     return default_action_completer(action=(['install'] + action), **kw)
 
 
 def _install_plugins(
         action: Optional[List[str]] = None,
         repository: Optional[str] = None,
+        skip_deps: bool = False,
         force: bool = False,
         debug: bool = False,
         **kw: Any
     ) -> SuccessTuple:
     """
     Install a plugin.
     
@@ -83,19 +84,22 @@
     from meerschaum.connectors.api import APIConnector
 
     if not action:
         return False, "No plugins to install."
 
     repo_connector = parse_repo_keys(repository)
 
-    successes = {}
     for name in action:
         info(f"Installing plugin '{name}' from Meerschaum repository '{repo_connector}'...")
-        success, msg = repo_connector.install_plugin(name, force=force, debug=debug)
-        successes[name] = (success, msg)
+        success, msg = repo_connector.install_plugin(
+            name,
+            force = force,
+            skip_deps = skip_deps,
+            debug = debug,
+        )
         print_tuple((success, msg))
 
     reload_plugins(debug=debug)
     return True, "Success"
 
 
 def _complete_install_plugins(
```

### Comparing `meerschaum-2.1.7/meerschaum/actions/login.py` & `meerschaum-2.2.0.dev1/meerschaum/actions/login.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/actions/os.py` & `meerschaum-2.2.0.dev1/meerschaum/actions/os.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/actions/pause.py` & `meerschaum-2.2.0.dev1/meerschaum/actions/pause.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/actions/python.py` & `meerschaum-2.2.0.dev1/meerschaum/actions/python.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/actions/register.py` & `meerschaum-2.2.0.dev1/meerschaum/actions/register.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/actions/setup.py` & `meerschaum-2.2.0.dev1/meerschaum/actions/setup.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/actions/sh.py` & `meerschaum-2.2.0.dev1/meerschaum/actions/sh.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/actions/show.py` & `meerschaum-2.2.0.dev1/meerschaum/actions/show.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/actions/sql.py` & `meerschaum-2.2.0.dev1/meerschaum/actions/sql.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/actions/stack.py` & `meerschaum-2.2.0.dev1/meerschaum/actions/stack.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/actions/start.py` & `meerschaum-2.2.0.dev1/meerschaum/actions/start.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/actions/stop.py` & `meerschaum-2.2.0.dev1/meerschaum/actions/stop.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/actions/sync.py` & `meerschaum-2.2.0.dev1/meerschaum/actions/sync.py`

 * *Files 1% similar despite different names*

```diff
@@ -449,24 +449,28 @@
                     f"Failed to execute sync hook '{sync_hook.__name__}' "
                     + f"from plugin '{plugin}':\n{traceback.format_exc()}"
                 )
                 warn(msg, stack=False)
                 return False, msg
         return True, "Success"
 
-    hook_results = []
+    pre_hook_results, post_hook_results = [], []
     def apply_hooks(is_pre_sync: bool):
         _sync_hooks = (_pre_sync_hooks if is_pre_sync else _post_sync_hooks)
+        _hook_results = (pre_hook_results if is_pre_sync else post_hook_results)
         for module_name, sync_hooks in _sync_hooks.items():
             plugin_name = module_name.split('.')[-1] if module_name.startswith('plugins.') else None
             for sync_hook in sync_hooks:
                 hook_result = pool.apply_async(call_sync_hook, (plugin_name, sync_hook))
-                hook_results.append(hook_result)
+                _hook_results.append(hook_result)
 
     apply_hooks(True)
+    for hook_result in pre_hook_results:
+        hook_success, hook_msg = hook_result.get()
+        mrsm.pprint((hook_success, hook_msg))
    
     try:
         with Venv(get_connector_plugin(pipe.connector), debug=debug):
             return_tuple = sync_method(**sync_kwargs)
     except Exception as e:
         import traceback
         traceback.print_exception(type(e), e, e.__traceback__)
@@ -476,15 +480,15 @@
     duration = time.perf_counter() - sync_start
     sync_kwargs.update({
         'success_tuple': return_tuple,
         'sync_duration': duration,
         'sync_complete_timestamp': datetime.now(timezone.utc),
     })
     apply_hooks(False)
-    for hook_result in hook_results:
+    for hook_result in post_hook_results:
         hook_success, hook_msg = hook_result.get()
         mrsm.pprint((hook_success, hook_msg))
 
     return return_tuple
```

### Comparing `meerschaum-2.1.7/meerschaum/actions/tag.py` & `meerschaum-2.2.0.dev1/meerschaum/actions/tag.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/actions/uninstall.py` & `meerschaum-2.2.0.dev1/meerschaum/actions/uninstall.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/actions/upgrade.py` & `meerschaum-2.2.0.dev1/meerschaum/actions/upgrade.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/actions/verify.py` & `meerschaum-2.2.0.dev1/meerschaum/actions/verify.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/api/__init__.py` & `meerschaum-2.2.0.dev1/meerschaum/api/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/api/_chain.py` & `meerschaum-2.2.0.dev1/meerschaum/api/_chain.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/api/_events.py` & `meerschaum-2.2.0.dev1/meerschaum/api/_events.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/api/_oauth2.py` & `meerschaum-2.2.0.dev1/meerschaum/api/_oauth2.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/api/_websockets.py` & `meerschaum-2.2.0.dev1/meerschaum/api/_websockets.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/api/dash/__init__.py` & `meerschaum-2.2.0.dev1/meerschaum/api/dash/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/api/dash/actions.py` & `meerschaum-2.2.0.dev1/meerschaum/api/dash/actions.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/api/dash/assets/ansi_up.js` & `meerschaum-2.2.0.dev1/meerschaum/api/dash/assets/ansi_up.js`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/api/dash/assets/banner_1920x320.png` & `meerschaum-2.2.0.dev1/meerschaum/api/dash/assets/banner_1920x320.png`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/api/dash/assets/favicon.ico` & `meerschaum-2.2.0.dev1/meerschaum/api/dash/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/api/dash/assets/logo_48x48.png` & `meerschaum-2.2.0.dev1/meerschaum/api/dash/assets/logo_48x48.png`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/api/dash/assets/logo_500x500.png` & `meerschaum-2.2.0.dev1/meerschaum/api/dash/assets/logo_500x500.png`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/api/dash/callbacks/dashboard.py` & `meerschaum-2.2.0.dev1/meerschaum/api/dash/callbacks/dashboard.py`

 * *Files 3% similar despite different names*

```diff
@@ -484,19 +484,19 @@
         *keys
     ):
     """
     Update the keys dropdown menus' options.
     """
     ctx = dash.callback_context
     trigger = ctx.triggered[0]['prop_id'].split('.')[0]
+    instance_click = trigger == 'instance-select'
 
     ### Update the instance first.
     update_instance_keys = False
     if not instance_keys:
-        #  instance_keys = get_config('meerschaum', 'web_instance')
         instance_keys = str(get_api_connector())
         update_instance_keys = True
     instance_alerts = []
     try:
         parse_instance_keys(instance_keys)
     except Exception as e:
         instance_alerts += [alert_from_success_tuple((False, str(e)))]
@@ -515,17 +515,17 @@
         num_filter += 1
     if location_keys:
         num_filter += 1
 
     _ck_alone, _mk_alone, _lk_alone = False, False, False
     _ck_filter, _mk_filter, _lk_filter = connector_keys, metric_keys, location_keys
 
-    _ck_alone = connector_keys and num_filter == 1
-    _mk_alone = metric_keys and num_filter == 1
-    _lk_alone = location_keys and num_filter == 1
+    _ck_alone = (connector_keys and num_filter == 1) or instance_click
+    _mk_alone = (metric_keys and num_filter == 1) or instance_click
+    _lk_alone = (location_keys and num_filter == 1) or instance_click
 
     from meerschaum.utils import fetch_pipes_keys
 
     try:
         _all_keys = fetch_pipes_keys('registered', get_web_connector(ctx.states))
         _keys = fetch_pipes_keys(
             'registered', get_web_connector(ctx.states),
@@ -541,23 +541,44 @@
     _seen_keys = {'ck' : set(), 'mk' : set(), 'lk' : set()}
 
     def add_options(options, keys, key_type):
         for ck, mk, lk in keys:
             k = locals()[key_type]
             if k not in _seen_keys[key_type]:
                 _k = 'None' if k in (None, '[None]', 'None', 'null') else k
-                options.append({'label' : _k, 'value' : _k})
+                options.append({'label': _k, 'value': _k})
                 _seen_keys[key_type].add(k)
 
     add_options(_connectors_options, _all_keys if _ck_alone else _keys, 'ck')
     add_options(_metrics_options, _all_keys if _mk_alone else _keys, 'mk')
     add_options(_locations_options, _all_keys if _lk_alone else _keys, 'lk')
-    connector_keys = [ck for ck in connector_keys if ck in [_ck['value'] for _ck in _connectors_options]]
-    metric_keys = [mk for mk in metric_keys if mk in [_mk['value'] for _mk in _metrics_options]]
-    location_keys = [lk for lk in location_keys if lk in [_lk['value'] for _lk in _locations_options]]
+    connector_keys = sorted([
+        ck
+        for ck in connector_keys 
+        if ck in [
+            _ck['value']
+            for _ck in _connectors_options
+        ]
+    ])
+    metric_keys = sorted([
+        mk
+        for mk in metric_keys
+        if mk in [
+            _mk['value']
+            for _mk in _metrics_options
+        ]
+    ])
+    location_keys = sorted([
+        lk
+        for lk in location_keys
+        if lk in [
+            _lk['value']
+            for _lk in _locations_options
+        ]
+    ])
     _connectors_datalist = [html.Option(value=o['value']) for o in _connectors_options]
     _metrics_datalist = [html.Option(value=o['value']) for o in _metrics_options]
     _locations_datalist = [html.Option(value=o['value']) for o in _locations_options]
     return (
         _connectors_options,
         _connectors_datalist,
         connector_keys,
@@ -676,14 +697,17 @@
 )
 
 @dash_app.callback(
     Output("download-dataframe-csv", "data"),
     Input({'type': 'pipe-download-csv-button', 'index': ALL}, 'n_clicks'),
 )
 def download_pipe_csv(n_clicks):
+    """
+    Download the most recent chunk as a CSV file.
+    """
     if not n_clicks:
         raise PreventUpdate
     ctx = dash.callback_context.triggered
     if ctx[0]['value'] is None:
         raise PreventUpdate
     pipe = pipe_from_ctx(ctx, 'n_clicks')
     if pipe is None:
@@ -814,14 +838,59 @@
             import traceback
             traceback.print_exc()
             success, msg = False, f"Encountered exception:\n{e}"
 
     return alert_from_success_tuple((success, msg))
 
 
+dash_app.clientside_callback(
+    """
+    function(n_clicks_arr, url){
+        display_block = {"display": "block"};
+
+        var clicked = false;
+        for (var i = 0; i < n_clicks_arr.length; i++){
+            if (n_clicks_arr[i]){
+                clicked = true;
+                break;
+            }
+        }
+        if (!clicked){ return dash_clientside.no_update; }
+
+        const triggered_id = dash_clientside.callback_context.triggered_id;
+        const action = triggered_id["action"];
+        const pipe_meta = JSON.parse(triggered_id["index"]);
+
+        iframe = document.getElementById('webterm-iframe');
+        if (!iframe){ return dash_clientside.no_update; }
+        var location = pipe_meta.location;
+        if (!pipe_meta.location){
+            location = "None";
+        }
+
+        iframe.contentWindow.postMessage(
+            {
+                action: action,
+                subaction: "pipes",
+                connector_keys: [pipe_meta.connector],
+                metric_keys: [pipe_meta.metric],
+                location_keys: [location],
+                instance: pipe_meta.instance,
+            },
+            url
+        );
+        dash_clientside.set_props("webterm-div", {"style": display_block});
+        return [];
+    }
+    """,
+    Output('content-div-right', 'children'),
+    Input({'type': 'manage-pipe-button', 'index': ALL, 'action': ALL}, 'n_clicks'),
+    State('location', 'href'),
+)
+
 @dash_app.callback(
     Output("navbar-collapse", "is_open"),
     [Input("navbar-toggler", "n_clicks")],
     [State("navbar-collapse", "is_open")],
 )
 def toggle_navbar_collapse(n_clicks: Optional[int], is_open: bool) -> bool:
     """
```

### Comparing `meerschaum-2.1.7/meerschaum/api/dash/callbacks/jobs.py` & `meerschaum-2.2.0.dev1/meerschaum/api/dash/callbacks/jobs.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 """
 
 from __future__ import annotations
 import json
 import functools
 import time
 import traceback
+from datetime import datetime, timezone
 import meerschaum as mrsm
 from meerschaum.utils.typing import Optional, Dict, Any
 from meerschaum.api import get_api_connector, endpoints, CHECK_UPDATE
 from meerschaum.api.dash import dash_app, debug, active_sessions
 from meerschaum.utils.packages import attempt_import, import_dcc, import_html
 dash = attempt_import('dash', lazy=False, check_update=CHECK_UPDATE)
 from dash.exceptions import PreventUpdate
@@ -50,17 +51,22 @@
     ctx = dash.callback_context.triggered
     if ctx[0]['value'] is None:
         raise PreventUpdate
 
     component_dict = json.loads(ctx[0]['prop_id'].split('.' + 'n_clicks')[0])
     daemon_id = component_dict['index']
     daemon = Daemon(daemon_id=daemon_id)
+    now = datetime.now(timezone.utc)
+    filename = (
+        daemon.rotating_log.file_path.name[:(-1 * len('.log'))]
+        + '_' + str(int(now.timestamp())) + '.log'
+    )
     return {
         'content': daemon.log_text,
-        'filename': daemon.rotating_log.file_path.name,
+        'filename': filename,
     }
 
 
 @dash_app.callback(
     Output({'type': 'manage-job-alert-div', 'index': MATCH}, 'children'),
     Output({'type': 'manage-job-buttons-div', 'index': MATCH}, 'children'),
     Output({'type': 'manage-job-status-div', 'index': MATCH}, 'children'),
@@ -70,15 +76,15 @@
     prevent_initial_call = True,
 )
 def manage_job_button_click(
         n_clicks: Optional[int] = None,
         session_data: Optional[Dict[str, Any]] = None,
     ):
     """
-    Start, stop, or pause the given job.
+    Start, stop, pause, or delete the given job.
     """
     if not n_clicks:
         raise PreventUpdate
 
     session_id = session_data.get('session-id', None)
     username = active_sessions.get(session_id, {}).get('username', None)
 
@@ -94,20 +100,26 @@
     ctx = dash.callback_context.triggered
     if ctx[0]['value'] is None:
         raise PreventUpdate
 
     component_dict = json.loads(ctx[0]['prop_id'].split('.' + 'n_clicks')[0])
     daemon_id = component_dict['index']
     manage_job_action = component_dict['action']
-    daemon = Daemon(daemon_id=daemon_id)
+    try:
+        daemon = Daemon(daemon_id=daemon_id)
+    except Exception as e:
+        daemon = None
+    if daemon is None:
+        raise PreventUpdate
 
     manage_functions = {
         'start': functools.partial(daemon.run, allow_dirty_run=True),
         'stop': daemon.quit,
         'pause': daemon.pause,
+        'delete': daemon.cleanup,
     }
     if manage_job_action not in manage_functions:
         return (
             alert_from_success_tuple((False, f"Invalid action '{manage_job_action}'.")),
             dash.no_update,
             dash.no_update,
             dash.no_update,
@@ -131,14 +143,54 @@
     return (
         alert_from_success_tuple((success, msg)),
         build_manage_job_buttons_div_children(daemon),
         build_status_children(daemon),
         build_process_timestamps_children(daemon),
     )
 
+dash_app.clientside_callback(
+    """
+    function(n_clicks_arr, url){
+        display_block = {"display": "block"};
+
+        var clicked = false;
+        for (var i = 0; i < n_clicks_arr.length; i++){
+            if (n_clicks_arr[i]){
+                clicked = true;
+                break;
+            }
+        }
+
+        if (!clicked){
+            return dash_clientside.no_update;
+        }
+
+        const triggered_id = dash_clientside.callback_context.triggered_id;
+        const job_daemon_id = triggered_id["index"];
+
+        iframe = document.getElementById('webterm-iframe');
+        if (!iframe){ return dash_clientside.no_update; }
+
+        iframe.contentWindow.postMessage(
+            {
+               action: "show",
+               subaction: "logs",
+               subaction_text: job_daemon_id,
+            },
+            url
+        );
+        dash_clientside.set_props("webterm-div", {"style": display_block});
+        return [];
+    }
+    """,
+    Output('content-div-right', 'children'),
+    Input({'type': 'follow-logs-button', 'index': ALL}, 'n_clicks'),
+    State('location', 'href'),
+)
+
 
 @dash_app.callback(
     Output({'type': 'manage-job-buttons-div', 'index': ALL}, 'children'),
     Output({'type': 'manage-job-status-div', 'index': ALL}, 'children'),
     Output({'type': 'process-timestamps-div', 'index': ALL}, 'children'),
     Input('refresh-jobs-interval', 'n_intervals'),
     State('session-store', 'data'),
```

### Comparing `meerschaum-2.1.7/meerschaum/api/dash/callbacks/login.py` & `meerschaum-2.2.0.dev1/meerschaum/api/dash/callbacks/login.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/api/dash/callbacks/plugins.py` & `meerschaum-2.2.0.dev1/meerschaum/api/dash/callbacks/plugins.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/api/dash/callbacks/register.py` & `meerschaum-2.2.0.dev1/meerschaum/api/dash/callbacks/register.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/api/dash/components.py` & `meerschaum-2.2.0.dev1/meerschaum/api/dash/components.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/api/dash/connectors.py` & `meerschaum-2.2.0.dev1/meerschaum/api/dash/connectors.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/api/dash/graphs.py` & `meerschaum-2.2.0.dev1/meerschaum/api/dash/graphs.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/api/dash/jobs.py` & `meerschaum-2.2.0.dev1/meerschaum/api/dash/jobs.py`

 * *Files 14% similar despite different names*

```diff
@@ -45,48 +45,61 @@
     cards = []
 
     for d in daemons:
         footer_children = html.Div(
             build_process_timestamps_children(d),
             id = {'type': 'process-timestamps-div', 'index': d.daemon_id},
         )
+        follow_logs_button = dbc.DropdownMenuItem(
+            "Follow logs",
+            id = {'type': 'follow-logs-button', 'index': d.daemon_id},
+        )
+        download_logs_button = dbc.DropdownMenuItem(
+            "Download logs",
+            id = {'type': 'job-download-logs-button', 'index': d.daemon_id},
+        )
+        logs_menu_children = (
+            ([follow_logs_button] if is_authenticated else []) + [download_logs_button]
+        )
         header_children = [
             html.Div(
                 build_status_children(d),
                 id = {'type': 'manage-job-status-div', 'index': d.daemon_id},
                 style = {'float': 'left'},
             ),
             html.Div(
-                dbc.Button(
-                    'Download logs',
-                    size = 'sm',
-                    color = 'link',
-                    id = {'type': 'job-download-logs-button', 'index': d.daemon_id},
+                dbc.DropdownMenu(
+                    logs_menu_children,
+                    label = "Logs",
+                    size = "sm",
+                    align_end = True,
+                    color = "secondary",
+                    menu_variant = 'dark',
                 ),
                 style = {'float': 'right'},
             ),
         ]
 
         body_children = [
             html.H4(html.B(d.daemon_id), className="card-title"),
             html.Div(
                 html.P(
                     d.label,
                     className = "card-text job-card-text", 
                     style = {"word-wrap": "break-word"}
                 ),
-                style={"white-space": "pre-wrap"},
+                style = {"white-space": "pre-wrap"},
             ),
             html.Div(
                 (
                     build_manage_job_buttons_div_children(d)
                     if is_authenticated
                     else []
                 ),
-                id={'type': 'manage-job-buttons-div', 'index': d.daemon_id}
+                id = {'type': 'manage-job-buttons-div', 'index': d.daemon_id},
             ),
             html.Div(id={'type': 'manage-job-alert-div', 'index': d.daemon_id}),
         ]
 
         cards.append(
             dbc.Card([
                 dbc.CardHeader(header_children),
@@ -104,15 +117,15 @@
     """
     buttons = build_manage_job_buttons(daemon)
     if not buttons:
         return []
     return [
         html.Br(),
         dbc.Row([
-            dbc.Col(button, width=4)
+            dbc.Col(button, width=6)
             for button in buttons
         ])
     ]
 
 
 def build_manage_job_buttons(daemon: Daemon):
     """
@@ -149,17 +162,30 @@
         style = {'width': '100%'},
         id = {
             'type': 'manage-job-button',
             'action': 'stop',
             'index': daemon.daemon_id,
         },
     )
+    delete_button = dbc.Button(
+        'Delete',
+        size = 'sm',
+        color = 'danger',
+        style = {'width': '100%'},
+        id = {
+            'type': 'manage-job-button',
+            'action': 'delete',
+            'index': daemon.daemon_id,
+        },
+    )
     buttons = []
     if daemon.status in ('stopped', 'paused'):
         buttons.append(start_button)
+    if daemon.status == 'stopped':
+        buttons.append(delete_button)
     if daemon.status in ('running',):
         buttons.append(pause_button)
     if daemon.status in ('running', 'paused'):
         buttons.append(stop_button)
 
     return buttons
```

### Comparing `meerschaum-2.1.7/meerschaum/api/dash/keys.py` & `meerschaum-2.2.0.dev1/meerschaum/api/dash/keys.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/api/dash/pages/dashboard.py` & `meerschaum-2.2.0.dev1/meerschaum/api/dash/pages/dashboard.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/api/dash/pages/error.py` & `meerschaum-2.2.0.dev1/meerschaum/api/dash/pages/error.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/api/dash/pages/login.py` & `meerschaum-2.2.0.dev1/meerschaum/api/dash/pages/login.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/api/dash/pages/plugins.py` & `meerschaum-2.2.0.dev1/meerschaum/api/dash/pages/plugins.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/api/dash/pages/register.py` & `meerschaum-2.2.0.dev1/meerschaum/api/dash/pages/register.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/api/dash/pipes.py` & `meerschaum-2.2.0.dev1/meerschaum/api/dash/pipes.py`

 * *Files 9% similar despite different names*

```diff
@@ -111,36 +111,92 @@
     authenticated = is_session_authenticated(str(session_id))
 
     _pipes = pipes_from_state(*keys, as_list=True)
     alerts = [alert_from_success_tuple(_pipes)]
     if not isinstance(_pipes, list):
         _pipes = []
     for p in _pipes:
-        footer_children = dbc.Row([
-            dbc.Col(
-                dbc.Button(
-                    'Download recent data',
-                    size = 'sm',
-                    color = 'link',
-                    id = {'type': 'pipe-download-csv-button', 'index': json.dumps(p.meta)},
-                )
-            ),
-        ])
+        meta_str = json.dumps(p.meta)
+        footer_children = dbc.Row(
+            [
+                dbc.Col(
+                    (
+                        dbc.DropdownMenu(
+                            label = "Manage",
+                            children = [
+                                dbc.DropdownMenuItem(
+                                    'Sync',
+                                    id = {
+                                        'type': 'manage-pipe-button',
+                                        'index': meta_str,
+                                        'action': 'sync',
+                                    },
+                                ),
+                                dbc.DropdownMenuItem(
+                                    'Drop',
+                                    id = {
+                                        'type': 'manage-pipe-button',
+                                        'index': meta_str,
+                                        'action': 'drop',
+                                    },
+                                ),
+                                dbc.DropdownMenuItem(
+                                    'Delete',
+                                    id = {
+                                        'type': 'manage-pipe-button',
+                                        'index': meta_str,
+                                        'action': 'delete',
+                                    },
+                                ),
+                            ],
+                            direction = "end",
+                            menu_variant = "dark",
+                            size = 'sm',
+                            color = 'secondary',
+                        )
+                    ) if authenticated else [],
+                    width = 2,
+                ),
+                #  dbc.Col(
+                    #  (
+                        #  dbc.Button(
+                            #  'Sync',
+                            #  size = 'sm',
+                            #  style = {'width': '100%'},
+                            #  id = {'type': 'pipe-sync-button', 'index': meta_str},
+                        #  ) if authenticated else []
+                    #  ),
+                    #  width = 2,
+                #  ),
+                dbc.Col(width=6),
+                dbc.Col(
+                    dbc.Button(
+                        'Download recent data',
+                        size = 'sm',
+                        color = 'link',
+                        style = {'float': 'right'},
+                        id = {'type': 'pipe-download-csv-button', 'index': meta_str},
+                    ),
+                    width = 4,
+                ),
+            ],
+            justify = 'start',
+        )
         card_body_children = [
             html.H5(
                 html.B(str(p)),
                 className = 'card-title',
                 style = {'font-family': ['monospace']}
             ),
             html.Div(
                 dbc.Accordion(
                     accordion_items_from_pipe(p, authenticated=authenticated),
                     flush = True,
                     start_collapsed = True,
-                    id = {'type': 'pipe-accordion', 'index': json.dumps(p.meta)},
+                    id = {'type': 'pipe-accordion', 'index': meta_str},
                 )
             )
 
         ]
         cards.append(
             dbc.Card(children=[
                 dbc.CardBody(children=card_body_children),
@@ -192,14 +248,26 @@
             html.Tr([html.Td("Metric"), html.Td(f"{pipe.metric_key}")]),
             html.Tr([html.Td("Location"), html.Td(f"{pipe.location_key}")]),
             html.Tr([html.Td("Instance"), html.Td(f"{pipe.instance_keys}")]),
             html.Tr([html.Td("Target Table"), html.Td(f"{pipe.target}")]),
         ]
         for col_key, col in pipe.columns.items():
             overview_rows.append(html.Tr([html.Td(f"'{col_key}' Index"), html.Td(col)]))
+        tags = pipe.tags
+        if tags:
+            tags_items = html.Ul([
+                html.Li(tag)
+                for tag in tags
+            ])
+            overview_rows.append(
+                html.Tr([
+                    html.Td("Tags"),
+                    html.Td(tags_items),
+                ])
+            )
 
         items_bodies['overview'] = dbc.Table(
             overview_header + [html.Tbody(overview_rows)],
             bordered=False, hover=True, striped=False,
         )
 
     if 'stats' in active_items:
```

### Comparing `meerschaum-2.1.7/meerschaum/api/dash/plugins.py` & `meerschaum-2.2.0.dev1/meerschaum/api/dash/plugins.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/api/dash/users.py` & `meerschaum-2.2.0.dev1/meerschaum/api/dash/users.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/api/dash/websockets.py` & `meerschaum-2.2.0.dev1/meerschaum/api/dash/websockets.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/api/dash/webterm.py` & `meerschaum-2.2.0.dev1/meerschaum/api/dash/webterm.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/api/resources/static/css/bootstrap.min.css` & `meerschaum-2.2.0.dev1/meerschaum/api/resources/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/api/resources/static/css/dash.css` & `meerschaum-2.2.0.dev1/meerschaum/api/resources/static/css/dash.css`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/api/resources/static/css/dbc_dark.css` & `meerschaum-2.2.0.dev1/meerschaum/api/resources/static/css/dbc_dark.css`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/api/resources/static/css/xterm.css` & `meerschaum-2.2.0.dev1/meerschaum/api/resources/static/css/xterm.css`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/api/resources/static/ico/logo.ico` & `meerschaum-2.2.0.dev1/meerschaum/api/resources/static/ico/logo.ico`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/api/resources/static/js/action_button.js` & `meerschaum-2.2.0.dev1/meerschaum/api/resources/static/js/action_button.js`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/api/resources/static/js/terminado.js` & `meerschaum-2.2.0.dev1/meerschaum/api/resources/static/js/terminado.js`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/api/resources/static/js/xterm.js` & `meerschaum-2.2.0.dev1/meerschaum/api/resources/static/js/xterm.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -25,21 +25,22 @@
                 Object.defineProperty(t, "__esModule", {
                     value: !0
                 }), t.AccessibilityManager = void 0;
                 const n = i(9042),
                     o = i(9924),
                     a = i(844),
                     h = i(4725),
-                    c = i(2585);
-                let l = t.AccessibilityManager = class extends a.Disposable {
+                    c = i(2585),
+                    l = i(3656);
+                let d = t.AccessibilityManager = class extends a.Disposable {
                     constructor(e, t, i, s) {
-                        super(), this._terminal = e, this._coreBrowserService = i, this._renderService = s, this._liveRegionLineCount = 0, this._charsToConsume = [], this._charsToAnnounce = "", this._accessibilityContainer = this._coreBrowserService.mainDocument.createElement("div"), this._accessibilityContainer.classList.add("xterm-accessibility"), this._rowContainer = this._coreBrowserService.mainDocument.createElement("div"), this._rowContainer.setAttribute("role", "list"), this._rowContainer.classList.add("xterm-accessibility-tree"), this._rowElements = [];
+                        super(), this._terminal = e, this._coreBrowserService = i, this._renderService = s, this._rowColumns = new WeakMap, this._liveRegionLineCount = 0, this._charsToConsume = [], this._charsToAnnounce = "", this._accessibilityContainer = this._coreBrowserService.mainDocument.createElement("div"), this._accessibilityContainer.classList.add("xterm-accessibility"), this._rowContainer = this._coreBrowserService.mainDocument.createElement("div"), this._rowContainer.setAttribute("role", "list"), this._rowContainer.classList.add("xterm-accessibility-tree"), this._rowElements = [];
                         for (let e = 0; e < this._terminal.rows; e++) this._rowElements[e] = this._createAccessibilityTreeNode(), this._rowContainer.appendChild(this._rowElements[e]);
                         if (this._topBoundaryFocusListener = e => this._handleBoundaryFocus(e, 0), this._bottomBoundaryFocusListener = e => this._handleBoundaryFocus(e, 1), this._rowElements[0].addEventListener("focus", this._topBoundaryFocusListener), this._rowElements[this._rowElements.length - 1].addEventListener("focus", this._bottomBoundaryFocusListener), this._refreshRowsDimensions(), this._accessibilityContainer.appendChild(this._rowContainer), this._liveRegion = this._coreBrowserService.mainDocument.createElement("div"), this._liveRegion.classList.add("live-region"), this._liveRegion.setAttribute("aria-live", "assertive"), this._accessibilityContainer.appendChild(this._liveRegion), this._liveRegionDebouncer = this.register(new o.TimeBasedDebouncer(this._renderRows.bind(this))), !this._terminal.element) throw new Error("Cannot enable accessibility before Terminal.open");
-                        this._terminal.element.insertAdjacentElement("afterbegin", this._accessibilityContainer), this.register(this._terminal.onResize((e => this._handleResize(e.rows)))), this.register(this._terminal.onRender((e => this._refreshRows(e.start, e.end)))), this.register(this._terminal.onScroll((() => this._refreshRows()))), this.register(this._terminal.onA11yChar((e => this._handleChar(e)))), this.register(this._terminal.onLineFeed((() => this._handleChar("\n")))), this.register(this._terminal.onA11yTab((e => this._handleTab(e)))), this.register(this._terminal.onKey((e => this._handleKey(e.key)))), this.register(this._terminal.onBlur((() => this._clearLiveRegion()))), this.register(this._renderService.onDimensionsChange((() => this._refreshRowsDimensions()))), this.register(this._coreBrowserService.onDprChange((() => this._refreshRowsDimensions()))), this._refreshRows(), this.register((0, a.toDisposable)((() => {
+                        this._terminal.element.insertAdjacentElement("afterbegin", this._accessibilityContainer), this.register(this._terminal.onResize((e => this._handleResize(e.rows)))), this.register(this._terminal.onRender((e => this._refreshRows(e.start, e.end)))), this.register(this._terminal.onScroll((() => this._refreshRows()))), this.register(this._terminal.onA11yChar((e => this._handleChar(e)))), this.register(this._terminal.onLineFeed((() => this._handleChar("\n")))), this.register(this._terminal.onA11yTab((e => this._handleTab(e)))), this.register(this._terminal.onKey((e => this._handleKey(e.key)))), this.register(this._terminal.onBlur((() => this._clearLiveRegion()))), this.register(this._renderService.onDimensionsChange((() => this._refreshRowsDimensions()))), this.register((0, l.addDisposableDomListener)(document, "selectionchange", (() => this._handleSelectionChange()))), this.register(this._coreBrowserService.onDprChange((() => this._refreshRowsDimensions()))), this._refreshRows(), this.register((0, a.toDisposable)((() => {
                             this._accessibilityContainer.remove(), this._rowElements.length = 0
                         })))
                     }
                     _handleTab(e) {
                         for (let t = 0; t < e; t++) this._handleChar(" ")
                     }
                     _handleChar(e) {
@@ -54,18 +55,20 @@
                     _refreshRows(e, t) {
                         this._liveRegionDebouncer.refresh(e, t, this._terminal.rows)
                     }
                     _renderRows(e, t) {
                         const i = this._terminal.buffer,
                             s = i.lines.length.toString();
                         for (let r = e; r <= t; r++) {
-                            const e = i.translateBufferLineToString(i.ydisp + r, !0),
-                                t = (i.ydisp + r + 1).toString(),
-                                n = this._rowElements[r];
-                            n && (0 === e.length ? n.innerText = " " : n.textContent = e, n.setAttribute("aria-posinset", t), n.setAttribute("aria-setsize", s))
+                            const e = i.lines.get(i.ydisp + r),
+                                t = [],
+                                n = e?.translateToString(!0, void 0, void 0, t) || "",
+                                o = (i.ydisp + r + 1).toString(),
+                                a = this._rowElements[r];
+                            a && (0 === n.length ? (a.innerText = " ", this._rowColumns.set(a, [0, 1])) : (a.textContent = n, this._rowColumns.set(a, t)), a.setAttribute("aria-posinset", o), a.setAttribute("aria-setsize", s))
                         }
                         this._announceCharacters()
                     }
                     _announceCharacters() {
                         0 !== this._charsToAnnounce.length && (this._liveRegion.textContent += this._charsToAnnounce, this._charsToAnnounce = "")
                     }
                     _handleBoundaryFocus(e, t) {
@@ -79,14 +82,59 @@
                             this._rowElements.unshift(e), this._rowContainer.insertAdjacentElement("afterbegin", e)
                         } else {
                             const e = this._createAccessibilityTreeNode();
                             this._rowElements.push(e), this._rowContainer.appendChild(e)
                         }
                         this._rowElements[0].addEventListener("focus", this._topBoundaryFocusListener), this._rowElements[this._rowElements.length - 1].addEventListener("focus", this._bottomBoundaryFocusListener), this._terminal.scrollLines(0 === t ? -1 : 1), this._rowElements[0 === t ? 1 : this._rowElements.length - 2].focus(), e.preventDefault(), e.stopImmediatePropagation()
                     }
+                    _handleSelectionChange() {
+                        if (0 === this._rowElements.length) return;
+                        const e = document.getSelection();
+                        if (!e) return;
+                        if (e.isCollapsed) return void(this._rowContainer.contains(e.anchorNode) && this._terminal.clearSelection());
+                        if (!e.anchorNode || !e.focusNode) return void console.error("anchorNode and/or focusNode are null");
+                        let t = {
+                                node: e.anchorNode,
+                                offset: e.anchorOffset
+                            },
+                            i = {
+                                node: e.focusNode,
+                                offset: e.focusOffset
+                            };
+                        if ((t.node.compareDocumentPosition(i.node) & Node.DOCUMENT_POSITION_PRECEDING || t.node === i.node && t.offset > i.offset) && ([t, i] = [i, t]), t.node.compareDocumentPosition(this._rowElements[0]) & (Node.DOCUMENT_POSITION_CONTAINED_BY | Node.DOCUMENT_POSITION_FOLLOWING) && (t = {
+                                node: this._rowElements[0].childNodes[0],
+                                offset: 0
+                            }), !this._rowContainer.contains(t.node)) return;
+                        const s = this._rowElements.slice(-1)[0];
+                        if (i.node.compareDocumentPosition(s) & (Node.DOCUMENT_POSITION_CONTAINED_BY | Node.DOCUMENT_POSITION_PRECEDING) && (i = {
+                                node: s,
+                                offset: s.textContent?.length ?? 0
+                            }), !this._rowContainer.contains(i.node)) return;
+                        const r = ({
+                                node: e,
+                                offset: t
+                            }) => {
+                                const i = e instanceof Text ? e.parentNode : e;
+                                let s = parseInt(i?.getAttribute("aria-posinset"), 10) - 1;
+                                if (isNaN(s)) return console.warn("row is invalid. Race condition?"), null;
+                                const r = this._rowColumns.get(i);
+                                if (!r) return console.warn("columns is null. Race condition?"), null;
+                                let n = t < r.length ? r[t] : r.slice(-1)[0] + 1;
+                                return n >= this._terminal.cols && (++s, n = 0), {
+                                    row: s,
+                                    column: n
+                                }
+                            },
+                            n = r(t),
+                            o = r(i);
+                        if (n && o) {
+                            if (n.row > o.row || n.row === o.row && n.column >= o.column) throw new Error("invalid range");
+                            this._terminal.select(n.column, n.row, (o.row - n.row) * this._terminal.cols - n.column + o.column)
+                        }
+                    }
                     _handleResize(e) {
                         this._rowElements[this._rowElements.length - 1].removeEventListener("focus", this._bottomBoundaryFocusListener);
                         for (let e = this._rowContainer.children.length; e < this._terminal.rows; e++) this._rowElements[e] = this._createAccessibilityTreeNode(), this._rowContainer.appendChild(this._rowElements[e]);
                         for (; this._rowElements.length > e;) this._rowContainer.removeChild(this._rowElements.pop());
                         this._rowElements[this._rowElements.length - 1].addEventListener("focus", this._bottomBoundaryFocusListener), this._refreshRowsDimensions()
                     }
                     _createAccessibilityTreeNode() {
@@ -99,15 +147,15 @@
                             for (let e = 0; e < this._terminal.rows; e++) this._refreshRowDimensions(this._rowElements[e])
                         }
                     }
                     _refreshRowDimensions(e) {
                         e.style.height = `${this._renderService.dimensions.css.cell.height}px`
                     }
                 };
-                t.AccessibilityManager = l = s([r(1, c.IInstantiationService), r(2, h.ICoreBrowserService), r(3, h.IRenderService)], l)
+                t.AccessibilityManager = d = s([r(1, c.IInstantiationService), r(2, h.ICoreBrowserService), r(3, h.IRenderService)], d)
             },
             3614: (e, t) => {
                 function i(e) {
                     return e.replace(/\r?\n/g, "\r")
                 }
 
                 function s(e, t) {
@@ -169,15 +217,15 @@
                     return {
                         dispose: () => {
                             r || (r = !0, e.removeEventListener(t, i, s))
                         }
                     }
                 }
             },
-            6465: function(e, t, i) {
+            3551: function(e, t, i) {
                 var s = this && this.__decorate || function(e, t, i, s) {
                         var r, n = arguments.length,
                             o = n < 3 ? t : null === s ? s = Object.getOwnPropertyDescriptor(t, i) : s;
                         if ("object" == typeof Reflect && "function" == typeof Reflect.decorate) o = Reflect.decorate(e, t, i, s);
                         else
                             for (var a = e.length - 1; a >= 0; a--)(r = e[a]) && (o = (n < 3 ? r(o) : n > 3 ? r(t, i, o) : r(t, i)) || o);
                         return n > 3 && o && Object.defineProperty(t, i, o), o
@@ -185,44 +233,35 @@
                     r = this && this.__param || function(e, t) {
                         return function(i, s) {
                             t(i, s, e)
                         }
                     };
                 Object.defineProperty(t, "__esModule", {
                     value: !0
-                }), t.Linkifier2 = void 0;
+                }), t.Linkifier = void 0;
                 const n = i(3656),
                     o = i(8460),
                     a = i(844),
-                    h = i(2585);
-                let c = t.Linkifier2 = class extends a.Disposable {
+                    h = i(2585),
+                    c = i(4725);
+                let l = t.Linkifier = class extends a.Disposable {
                     get currentLink() {
                         return this._currentLink
                     }
-                    constructor(e) {
-                        super(), this._bufferService = e, this._linkProviders = [], this._linkCacheDisposables = [], this._isMouseOut = !0, this._wasResized = !1, this._activeLine = -1, this._onShowLinkUnderline = this.register(new o.EventEmitter), this.onShowLinkUnderline = this._onShowLinkUnderline.event, this._onHideLinkUnderline = this.register(new o.EventEmitter), this.onHideLinkUnderline = this._onHideLinkUnderline.event, this.register((0, a.getDisposeArrayDisposable)(this._linkCacheDisposables)), this.register((0, a.toDisposable)((() => {
-                            this._lastMouseEvent = void 0
+                    constructor(e, t, i, s, r) {
+                        super(), this._element = e, this._mouseService = t, this._renderService = i, this._bufferService = s, this._linkProviderService = r, this._linkCacheDisposables = [], this._isMouseOut = !0, this._wasResized = !1, this._activeLine = -1, this._onShowLinkUnderline = this.register(new o.EventEmitter), this.onShowLinkUnderline = this._onShowLinkUnderline.event, this._onHideLinkUnderline = this.register(new o.EventEmitter), this.onHideLinkUnderline = this._onHideLinkUnderline.event, this.register((0, a.getDisposeArrayDisposable)(this._linkCacheDisposables)), this.register((0, a.toDisposable)((() => {
+                            this._lastMouseEvent = void 0, this._activeProviderReplies?.clear()
                         }))), this.register(this._bufferService.onResize((() => {
                             this._clearCurrentLink(), this._wasResized = !0
-                        })))
-                    }
-                    registerLinkProvider(e) {
-                        return this._linkProviders.push(e), {
-                            dispose: () => {
-                                const t = this._linkProviders.indexOf(e); - 1 !== t && this._linkProviders.splice(t, 1)
-                            }
-                        }
-                    }
-                    attachToDom(e, t, i) {
-                        this._element = e, this._mouseService = t, this._renderService = i, this.register((0, n.addDisposableDomListener)(this._element, "mouseleave", (() => {
+                        }))), this.register((0, n.addDisposableDomListener)(this._element, "mouseleave", (() => {
                             this._isMouseOut = !0, this._clearCurrentLink()
                         }))), this.register((0, n.addDisposableDomListener)(this._element, "mousemove", this._handleMouseMove.bind(this))), this.register((0, n.addDisposableDomListener)(this._element, "mousedown", this._handleMouseDown.bind(this))), this.register((0, n.addDisposableDomListener)(this._element, "mouseup", this._handleMouseUp.bind(this)))
                     }
                     _handleMouseMove(e) {
-                        if (this._lastMouseEvent = e, !this._element || !this._mouseService) return;
+                        this._lastMouseEvent = e;
                         const t = this._positionFromMouseEvent(e, this._element, this._mouseService);
                         if (!t) return;
                         this._isMouseOut = !1;
                         const i = e.composedPath();
                         for (let e = 0; e < i.length; e++) {
                             const t = i[e];
                             if (t.classList.contains("xterm")) break;
@@ -237,24 +276,24 @@
                     _askForLink(e, t) {
                         this._activeProviderReplies && t || (this._activeProviderReplies?.forEach((e => {
                             e?.forEach((e => {
                                 e.link.dispose && e.link.dispose()
                             }))
                         })), this._activeProviderReplies = new Map, this._activeLine = e.y);
                         let i = !1;
-                        for (const [s, r] of this._linkProviders.entries())
+                        for (const [s, r] of this._linkProviderService.linkProviders.entries())
                             if (t) {
                                 const t = this._activeProviderReplies?.get(s);
                                 t && (i = this._checkLinkProviderResult(s, e, i))
                             } else r.provideLinks(e.y, (t => {
                                 if (this._isMouseOut) return;
                                 const r = t?.map((e => ({
                                     link: e
                                 })));
-                                this._activeProviderReplies?.set(s, r), i = this._checkLinkProviderResult(s, e, i), this._activeProviderReplies?.size === this._linkProviders.length && this._removeIntersectingLinks(e.y, this._activeProviderReplies)
+                                this._activeProviderReplies?.set(s, r), i = this._checkLinkProviderResult(s, e, i), this._activeProviderReplies?.size === this._linkProviderService.linkProviders.length && this._removeIntersectingLinks(e.y, this._activeProviderReplies)
                             }))
                     }
                     _removeIntersectingLinks(e, t) {
                         const i = new Set;
                         for (let s = 0; s < t.size; s++) {
                             const r = t.get(s);
                             if (r)
@@ -277,62 +316,62 @@
                         const s = this._activeProviderReplies.get(e);
                         let r = !1;
                         for (let t = 0; t < e; t++) this._activeProviderReplies.has(t) && !this._activeProviderReplies.get(t) || (r = !0);
                         if (!r && s) {
                             const e = s.find((e => this._linkAtPosition(e.link, t)));
                             e && (i = !0, this._handleNewLink(e))
                         }
-                        if (this._activeProviderReplies.size === this._linkProviders.length && !i)
+                        if (this._activeProviderReplies.size === this._linkProviderService.linkProviders.length && !i)
                             for (let e = 0; e < this._activeProviderReplies.size; e++) {
                                 const s = this._activeProviderReplies.get(e)?.find((e => this._linkAtPosition(e.link, t)));
                                 if (s) {
                                     i = !0, this._handleNewLink(s);
                                     break
                                 }
                             }
                         return i
                     }
                     _handleMouseDown() {
                         this._mouseDownLink = this._currentLink
                     }
                     _handleMouseUp(e) {
-                        if (!this._element || !this._mouseService || !this._currentLink) return;
+                        if (!this._currentLink) return;
                         const t = this._positionFromMouseEvent(e, this._element, this._mouseService);
                         t && this._mouseDownLink === this._currentLink && this._linkAtPosition(this._currentLink.link, t) && this._currentLink.link.activate(e, this._currentLink.link.text)
                     }
                     _clearCurrentLink(e, t) {
-                        this._element && this._currentLink && this._lastMouseEvent && (!e || !t || this._currentLink.link.range.start.y >= e && this._currentLink.link.range.end.y <= t) && (this._linkLeave(this._element, this._currentLink.link, this._lastMouseEvent), this._currentLink = void 0, (0, a.disposeArray)(this._linkCacheDisposables))
+                        this._currentLink && this._lastMouseEvent && (!e || !t || this._currentLink.link.range.start.y >= e && this._currentLink.link.range.end.y <= t) && (this._linkLeave(this._element, this._currentLink.link, this._lastMouseEvent), this._currentLink = void 0, (0, a.disposeArray)(this._linkCacheDisposables))
                     }
                     _handleNewLink(e) {
-                        if (!this._element || !this._lastMouseEvent || !this._mouseService) return;
+                        if (!this._lastMouseEvent) return;
                         const t = this._positionFromMouseEvent(this._lastMouseEvent, this._element, this._mouseService);
                         t && this._linkAtPosition(e.link, t) && (this._currentLink = e, this._currentLink.state = {
                             decorations: {
                                 underline: void 0 === e.link.decorations || e.link.decorations.underline,
                                 pointerCursor: void 0 === e.link.decorations || e.link.decorations.pointerCursor
                             },
                             isHovered: !0
                         }, this._linkHover(this._element, e.link, this._lastMouseEvent), e.link.decorations = {}, Object.defineProperties(e.link.decorations, {
                             pointerCursor: {
                                 get: () => this._currentLink?.state?.decorations.pointerCursor,
                                 set: e => {
-                                    this._currentLink?.state && this._currentLink.state.decorations.pointerCursor !== e && (this._currentLink.state.decorations.pointerCursor = e, this._currentLink.state.isHovered && this._element?.classList.toggle("xterm-cursor-pointer", e))
+                                    this._currentLink?.state && this._currentLink.state.decorations.pointerCursor !== e && (this._currentLink.state.decorations.pointerCursor = e, this._currentLink.state.isHovered && this._element.classList.toggle("xterm-cursor-pointer", e))
                                 }
                             },
                             underline: {
                                 get: () => this._currentLink?.state?.decorations.underline,
                                 set: t => {
                                     this._currentLink?.state && this._currentLink?.state?.decorations.underline !== t && (this._currentLink.state.decorations.underline = t, this._currentLink.state.isHovered && this._fireUnderlineEvent(e.link, t))
                                 }
                             }
-                        }), this._renderService && this._linkCacheDisposables.push(this._renderService.onRenderedViewportChange((e => {
+                        }), this._linkCacheDisposables.push(this._renderService.onRenderedViewportChange((e => {
                             if (!this._currentLink) return;
                             const t = 0 === e.start ? 0 : e.start + 1 + this._bufferService.buffer.ydisp,
                                 i = this._bufferService.buffer.ydisp + 1 + e.end;
-                            if (this._currentLink.link.range.start.y >= t && this._currentLink.link.range.end.y <= i && (this._clearCurrentLink(t, i), this._lastMouseEvent && this._element)) {
+                            if (this._currentLink.link.range.start.y >= t && this._currentLink.link.range.end.y <= i && (this._clearCurrentLink(t, i), this._lastMouseEvent)) {
                                 const e = this._positionFromMouseEvent(this._lastMouseEvent, this._element, this._mouseService);
                                 e && this._askForLink(e, !1)
                             }
                         }))))
                     }
                     _linkHover(e, t, i) {
                         this._currentLink?.state && (this._currentLink.state.isHovered = !0, this._currentLink.state.decorations.underline && this._fireUnderlineEvent(t, !0), this._currentLink.state.decorations.pointerCursor && e.classList.add("xterm-cursor-pointer")), t.hover && t.hover(i, t.text)
@@ -366,15 +405,15 @@
                             x2: i,
                             y2: s,
                             cols: this._bufferService.cols,
                             fg: r
                         }
                     }
                 };
-                t.Linkifier2 = c = s([r(0, h.IBufferService)], c)
+                t.Linkifier = l = s([r(1, c.IMouseService), r(2, c.IRenderService), r(3, h.IBufferService), r(4, c.ILinkProviderService)], l)
             },
             9042: (e, t) => {
                 Object.defineProperty(t, "__esModule", {
                     value: !0
                 }), t.tooMuchOutput = t.promptLabel = void 0, t.promptLabel = "Terminal input", t.tooMuchOutput = "Too much output to announce, navigate to rows manually to read"
             },
             3730: function(e, t, i) {
@@ -467,24 +506,24 @@
                 t.OscLinkProvider = a = s([r(0, o.IBufferService), r(1, o.IOptionsService), r(2, o.IOscLinkService)], a)
             },
             6193: (e, t) => {
                 Object.defineProperty(t, "__esModule", {
                     value: !0
                 }), t.RenderDebouncer = void 0, t.RenderDebouncer = class {
                     constructor(e, t) {
-                        this._parentWindow = e, this._renderCallback = t, this._refreshCallbacks = []
+                        this._renderCallback = e, this._coreBrowserService = t, this._refreshCallbacks = []
                     }
                     dispose() {
-                        this._animationFrame && (this._parentWindow.cancelAnimationFrame(this._animationFrame), this._animationFrame = void 0)
+                        this._animationFrame && (this._coreBrowserService.window.cancelAnimationFrame(this._animationFrame), this._animationFrame = void 0)
                     }
                     addRefreshCallback(e) {
-                        return this._refreshCallbacks.push(e), this._animationFrame || (this._animationFrame = this._parentWindow.requestAnimationFrame((() => this._innerRefresh()))), this._animationFrame
+                        return this._refreshCallbacks.push(e), this._animationFrame || (this._animationFrame = this._coreBrowserService.window.requestAnimationFrame((() => this._innerRefresh()))), this._animationFrame
                     }
                     refresh(e, t, i) {
-                        this._rowCount = i, e = void 0 !== e ? e : 0, t = void 0 !== t ? t : this._rowCount - 1, this._rowStart = void 0 !== this._rowStart ? Math.min(this._rowStart, e) : e, this._rowEnd = void 0 !== this._rowEnd ? Math.max(this._rowEnd, t) : t, this._animationFrame || (this._animationFrame = this._parentWindow.requestAnimationFrame((() => this._innerRefresh())))
+                        this._rowCount = i, e = void 0 !== e ? e : 0, t = void 0 !== t ? t : this._rowCount - 1, this._rowStart = void 0 !== this._rowStart ? Math.min(this._rowStart, e) : e, this._rowEnd = void 0 !== this._rowEnd ? Math.max(this._rowEnd, t) : t, this._animationFrame || (this._animationFrame = this._coreBrowserService.window.requestAnimationFrame((() => this._innerRefresh())))
                     }
                     _innerRefresh() {
                         if (this._animationFrame = void 0, void 0 === this._rowStart || void 0 === this._rowEnd || void 0 === this._rowCount) return void this._runRefreshCallbacks();
                         const e = Math.max(this._rowStart, 0),
                             t = Math.min(this._rowEnd, this._rowCount - 1);
                         this._rowStart = void 0, this._rowEnd = void 0, this._renderCallback(e, t), this._runRefreshCallbacks()
                     }
@@ -496,44 +535,45 @@
             },
             3236: (e, t, i) => {
                 Object.defineProperty(t, "__esModule", {
                     value: !0
                 }), t.Terminal = void 0;
                 const s = i(3614),
                     r = i(3656),
-                    n = i(6465),
+                    n = i(3551),
                     o = i(9042),
                     a = i(3730),
                     h = i(1680),
                     c = i(3107),
                     l = i(5744),
                     d = i(2950),
                     _ = i(1296),
                     u = i(428),
                     f = i(4269),
                     v = i(5114),
-                    g = i(8934),
-                    p = i(3230),
+                    p = i(8934),
+                    g = i(3230),
                     m = i(9312),
                     S = i(4725),
                     C = i(6731),
                     b = i(8055),
-                    y = i(8969),
-                    w = i(8460),
+                    w = i(8969),
+                    y = i(8460),
                     E = i(844),
                     k = i(6114),
                     L = i(8437),
                     D = i(2584),
                     R = i(7399),
                     x = i(5941),
                     A = i(9074),
                     B = i(2585),
                     T = i(5435),
-                    M = i(4567);
-                class O extends y.CoreTerminal {
+                    M = i(4567),
+                    O = i(779);
+                class P extends w.CoreTerminal {
                     get onFocus() {
                         return this._onFocus.event
                     }
                     get onBlur() {
                         return this._onBlur.event
                     }
                     get onA11yChar() {
@@ -542,15 +582,15 @@
                     get onA11yTab() {
                         return this._onA11yTabEmitter.event
                     }
                     get onWillOpen() {
                         return this._onWillOpen.event
                     }
                     constructor(e = {}) {
-                        super(e), this.browser = k, this._keyDownHandled = !1, this._keyDownSeen = !1, this._keyPressHandled = !1, this._unprocessedDeadKey = !1, this._accessibilityManager = this.register(new E.MutableDisposable), this._onCursorMove = this.register(new w.EventEmitter), this.onCursorMove = this._onCursorMove.event, this._onKey = this.register(new w.EventEmitter), this.onKey = this._onKey.event, this._onRender = this.register(new w.EventEmitter), this.onRender = this._onRender.event, this._onSelectionChange = this.register(new w.EventEmitter), this.onSelectionChange = this._onSelectionChange.event, this._onTitleChange = this.register(new w.EventEmitter), this.onTitleChange = this._onTitleChange.event, this._onBell = this.register(new w.EventEmitter), this.onBell = this._onBell.event, this._onFocus = this.register(new w.EventEmitter), this._onBlur = this.register(new w.EventEmitter), this._onA11yCharEmitter = this.register(new w.EventEmitter), this._onA11yTabEmitter = this.register(new w.EventEmitter), this._onWillOpen = this.register(new w.EventEmitter), this._setup(), this.linkifier2 = this.register(this._instantiationService.createInstance(n.Linkifier2)), this.linkifier2.registerLinkProvider(this._instantiationService.createInstance(a.OscLinkProvider)), this._decorationService = this._instantiationService.createInstance(A.DecorationService), this._instantiationService.setService(B.IDecorationService, this._decorationService), this.register(this._inputHandler.onRequestBell((() => this._onBell.fire()))), this.register(this._inputHandler.onRequestRefreshRows(((e, t) => this.refresh(e, t)))), this.register(this._inputHandler.onRequestSendFocus((() => this._reportFocus()))), this.register(this._inputHandler.onRequestReset((() => this.reset()))), this.register(this._inputHandler.onRequestWindowsOptionsReport((e => this._reportWindowsOptions(e)))), this.register(this._inputHandler.onColor((e => this._handleColorEvent(e)))), this.register((0, w.forwardEvent)(this._inputHandler.onCursorMove, this._onCursorMove)), this.register((0, w.forwardEvent)(this._inputHandler.onTitleChange, this._onTitleChange)), this.register((0, w.forwardEvent)(this._inputHandler.onA11yChar, this._onA11yCharEmitter)), this.register((0, w.forwardEvent)(this._inputHandler.onA11yTab, this._onA11yTabEmitter)), this.register(this._bufferService.onResize((e => this._afterResize(e.cols, e.rows)))), this.register((0, E.toDisposable)((() => {
+                        super(e), this.browser = k, this._keyDownHandled = !1, this._keyDownSeen = !1, this._keyPressHandled = !1, this._unprocessedDeadKey = !1, this._accessibilityManager = this.register(new E.MutableDisposable), this._onCursorMove = this.register(new y.EventEmitter), this.onCursorMove = this._onCursorMove.event, this._onKey = this.register(new y.EventEmitter), this.onKey = this._onKey.event, this._onRender = this.register(new y.EventEmitter), this.onRender = this._onRender.event, this._onSelectionChange = this.register(new y.EventEmitter), this.onSelectionChange = this._onSelectionChange.event, this._onTitleChange = this.register(new y.EventEmitter), this.onTitleChange = this._onTitleChange.event, this._onBell = this.register(new y.EventEmitter), this.onBell = this._onBell.event, this._onFocus = this.register(new y.EventEmitter), this._onBlur = this.register(new y.EventEmitter), this._onA11yCharEmitter = this.register(new y.EventEmitter), this._onA11yTabEmitter = this.register(new y.EventEmitter), this._onWillOpen = this.register(new y.EventEmitter), this._setup(), this._decorationService = this._instantiationService.createInstance(A.DecorationService), this._instantiationService.setService(B.IDecorationService, this._decorationService), this._linkProviderService = this._instantiationService.createInstance(O.LinkProviderService), this._instantiationService.setService(S.ILinkProviderService, this._linkProviderService), this._linkProviderService.registerLinkProvider(this._instantiationService.createInstance(a.OscLinkProvider)), this.register(this._inputHandler.onRequestBell((() => this._onBell.fire()))), this.register(this._inputHandler.onRequestRefreshRows(((e, t) => this.refresh(e, t)))), this.register(this._inputHandler.onRequestSendFocus((() => this._reportFocus()))), this.register(this._inputHandler.onRequestReset((() => this.reset()))), this.register(this._inputHandler.onRequestWindowsOptionsReport((e => this._reportWindowsOptions(e)))), this.register(this._inputHandler.onColor((e => this._handleColorEvent(e)))), this.register((0, y.forwardEvent)(this._inputHandler.onCursorMove, this._onCursorMove)), this.register((0, y.forwardEvent)(this._inputHandler.onTitleChange, this._onTitleChange)), this.register((0, y.forwardEvent)(this._inputHandler.onA11yChar, this._onA11yCharEmitter)), this.register((0, y.forwardEvent)(this._inputHandler.onA11yTab, this._onA11yTabEmitter)), this.register(this._bufferService.onResize((e => this._afterResize(e.cols, e.rows)))), this.register((0, E.toDisposable)((() => {
                             this._customKeyEventHandler = void 0, this.element?.parentNode?.removeChild(this.element)
                         })))
                     }
                     _handleColorEvent(e) {
                         if (this._themeService)
                             for (const t of e) {
                                 let e, i = "";
@@ -569,18 +609,18 @@
                                 }
                                 switch (t.type) {
                                     case 0:
                                         const s = b.color.toColorRGB("ansi" === e ? this._themeService.colors.ansi[t.index] : this._themeService.colors[e]);
                                         this.coreService.triggerDataEvent(`${D.C0.ESC}]${i};${(0,x.toRgbString)(s)}${D.C1_ESCAPED.ST}`);
                                         break;
                                     case 1:
-                                        if ("ansi" === e) this._themeService.modifyColors((e => e.ansi[t.index] = b.rgba.toColor(...t.color)));
+                                        if ("ansi" === e) this._themeService.modifyColors((e => e.ansi[t.index] = b.channels.toColor(...t.color)));
                                         else {
                                             const i = e;
-                                            this._themeService.modifyColors((e => e[i] = b.rgba.toColor(...t.color)))
+                                            this._themeService.modifyColors((e => e[i] = b.channels.toColor(...t.color)))
                                         }
                                         break;
                                     case 2:
                                         this._themeService.restoreColor(t.index)
                                 }
                             }
                     }
@@ -595,15 +635,15 @@
                             preventScroll: !0
                         })
                     }
                     _handleScreenReaderModeOptionChange(e) {
                         e ? !this._accessibilityManager.value && this._renderService && (this._accessibilityManager.value = this._instantiationService.createInstance(M.AccessibilityManager, this)) : this._accessibilityManager.clear()
                     }
                     _handleTextAreaFocus(e) {
-                        this.coreService.decPrivateModes.sendFocus && this.coreService.triggerDataEvent(D.C0.ESC + "[I"), this.updateCursorStyle(e), this.element.classList.add("focus"), this._showCursor(), this._onFocus.fire()
+                        this.coreService.decPrivateModes.sendFocus && this.coreService.triggerDataEvent(D.C0.ESC + "[I"), this.element.classList.add("focus"), this._showCursor(), this._onFocus.fire()
                     }
                     blur() {
                         return this.textarea?.blur()
                     }
                     _handleTextAreaBlur() {
                         this.textarea.value = "", this.refresh(this.buffer.y, this.buffer.y), this.coreService.decPrivateModes.sendFocus && this.coreService.triggerDataEvent(D.C0.ESC + "[O"), this.element.classList.remove("focus"), this._onBlur.fire()
                     }
@@ -637,30 +677,30 @@
                         this.register((0, r.addDisposableDomListener)(this.textarea, "keyup", (e => this._keyUp(e)), !0)), this.register((0, r.addDisposableDomListener)(this.textarea, "keydown", (e => this._keyDown(e)), !0)), this.register((0, r.addDisposableDomListener)(this.textarea, "keypress", (e => this._keyPress(e)), !0)), this.register((0, r.addDisposableDomListener)(this.textarea, "compositionstart", (() => this._compositionHelper.compositionstart()))), this.register((0, r.addDisposableDomListener)(this.textarea, "compositionupdate", (e => this._compositionHelper.compositionupdate(e)))), this.register((0, r.addDisposableDomListener)(this.textarea, "compositionend", (() => this._compositionHelper.compositionend()))), this.register((0, r.addDisposableDomListener)(this.textarea, "input", (e => this._inputEvent(e)), !0)), this.register(this.onRender((() => this._compositionHelper.updateCompositionElements())))
                     }
                     open(e) {
                         if (!e) throw new Error("Terminal requires a parent element.");
                         if (e.isConnected || this._logService.debug("Terminal.open was called on an element that was not attached to the DOM"), this.element?.ownerDocument.defaultView && this._coreBrowserService) return void(this.element.ownerDocument.defaultView !== this._coreBrowserService.window && (this._coreBrowserService.window = this.element.ownerDocument.defaultView));
                         this._document = e.ownerDocument, this.options.documentOverride && this.options.documentOverride instanceof Document && (this._document = this.optionsService.rawOptions.documentOverride), this.element = this._document.createElement("div"), this.element.dir = "ltr", this.element.classList.add("terminal"), this.element.classList.add("xterm"), e.appendChild(this.element);
                         const t = this._document.createDocumentFragment();
-                        this._viewportElement = this._document.createElement("div"), this._viewportElement.classList.add("xterm-viewport"), t.appendChild(this._viewportElement), this._viewportScrollArea = this._document.createElement("div"), this._viewportScrollArea.classList.add("xterm-scroll-area"), this._viewportElement.appendChild(this._viewportScrollArea), this.screenElement = this._document.createElement("div"), this.screenElement.classList.add("xterm-screen"), this._helperContainer = this._document.createElement("div"), this._helperContainer.classList.add("xterm-helpers"), this.screenElement.appendChild(this._helperContainer), t.appendChild(this.screenElement), this.textarea = this._document.createElement("textarea"), this.textarea.classList.add("xterm-helper-textarea"), this.textarea.setAttribute("aria-label", o.promptLabel), k.isChromeOS || this.textarea.setAttribute("aria-multiline", "false"), this.textarea.setAttribute("autocorrect", "off"), this.textarea.setAttribute("autocapitalize", "off"), this.textarea.setAttribute("spellcheck", "false"), this.textarea.tabIndex = 0, this._coreBrowserService = this.register(this._instantiationService.createInstance(v.CoreBrowserService, this.textarea, e.ownerDocument.defaultView ?? window, this._document ?? "undefined" != typeof window ? window.document : null)), this._instantiationService.setService(S.ICoreBrowserService, this._coreBrowserService), this.register((0, r.addDisposableDomListener)(this.textarea, "focus", (e => this._handleTextAreaFocus(e)))), this.register((0, r.addDisposableDomListener)(this.textarea, "blur", (() => this._handleTextAreaBlur()))), this._helperContainer.appendChild(this.textarea), this._charSizeService = this._instantiationService.createInstance(u.CharSizeService, this._document, this._helperContainer), this._instantiationService.setService(S.ICharSizeService, this._charSizeService), this._themeService = this._instantiationService.createInstance(C.ThemeService), this._instantiationService.setService(S.IThemeService, this._themeService), this._characterJoinerService = this._instantiationService.createInstance(f.CharacterJoinerService), this._instantiationService.setService(S.ICharacterJoinerService, this._characterJoinerService), this._renderService = this.register(this._instantiationService.createInstance(p.RenderService, this.rows, this.screenElement)), this._instantiationService.setService(S.IRenderService, this._renderService), this.register(this._renderService.onRenderedViewportChange((e => this._onRender.fire(e)))), this.onResize((e => this._renderService.resize(e.cols, e.rows))), this._compositionView = this._document.createElement("div"), this._compositionView.classList.add("composition-view"), this._compositionHelper = this._instantiationService.createInstance(d.CompositionHelper, this.textarea, this._compositionView), this._helperContainer.appendChild(this._compositionView), this.element.appendChild(t);
+                        this._viewportElement = this._document.createElement("div"), this._viewportElement.classList.add("xterm-viewport"), t.appendChild(this._viewportElement), this._viewportScrollArea = this._document.createElement("div"), this._viewportScrollArea.classList.add("xterm-scroll-area"), this._viewportElement.appendChild(this._viewportScrollArea), this.screenElement = this._document.createElement("div"), this.screenElement.classList.add("xterm-screen"), this.register((0, r.addDisposableDomListener)(this.screenElement, "mousemove", (e => this.updateCursorStyle(e)))), this._helperContainer = this._document.createElement("div"), this._helperContainer.classList.add("xterm-helpers"), this.screenElement.appendChild(this._helperContainer), t.appendChild(this.screenElement), this.textarea = this._document.createElement("textarea"), this.textarea.classList.add("xterm-helper-textarea"), this.textarea.setAttribute("aria-label", o.promptLabel), k.isChromeOS || this.textarea.setAttribute("aria-multiline", "false"), this.textarea.setAttribute("autocorrect", "off"), this.textarea.setAttribute("autocapitalize", "off"), this.textarea.setAttribute("spellcheck", "false"), this.textarea.tabIndex = 0, this._coreBrowserService = this.register(this._instantiationService.createInstance(v.CoreBrowserService, this.textarea, e.ownerDocument.defaultView ?? window, this._document ?? "undefined" != typeof window ? window.document : null)), this._instantiationService.setService(S.ICoreBrowserService, this._coreBrowserService), this.register((0, r.addDisposableDomListener)(this.textarea, "focus", (e => this._handleTextAreaFocus(e)))), this.register((0, r.addDisposableDomListener)(this.textarea, "blur", (() => this._handleTextAreaBlur()))), this._helperContainer.appendChild(this.textarea), this._charSizeService = this._instantiationService.createInstance(u.CharSizeService, this._document, this._helperContainer), this._instantiationService.setService(S.ICharSizeService, this._charSizeService), this._themeService = this._instantiationService.createInstance(C.ThemeService), this._instantiationService.setService(S.IThemeService, this._themeService), this._characterJoinerService = this._instantiationService.createInstance(f.CharacterJoinerService), this._instantiationService.setService(S.ICharacterJoinerService, this._characterJoinerService), this._renderService = this.register(this._instantiationService.createInstance(g.RenderService, this.rows, this.screenElement)), this._instantiationService.setService(S.IRenderService, this._renderService), this.register(this._renderService.onRenderedViewportChange((e => this._onRender.fire(e)))), this.onResize((e => this._renderService.resize(e.cols, e.rows))), this._compositionView = this._document.createElement("div"), this._compositionView.classList.add("composition-view"), this._compositionHelper = this._instantiationService.createInstance(d.CompositionHelper, this.textarea, this._compositionView), this._helperContainer.appendChild(this._compositionView), this._mouseService = this._instantiationService.createInstance(p.MouseService), this._instantiationService.setService(S.IMouseService, this._mouseService), this.linkifier = this.register(this._instantiationService.createInstance(n.Linkifier, this.screenElement)), this.element.appendChild(t);
                         try {
                             this._onWillOpen.fire(this.element)
                         } catch {}
-                        this._renderService.hasRenderer() || this._renderService.setRenderer(this._createRenderer()), this._mouseService = this._instantiationService.createInstance(g.MouseService), this._instantiationService.setService(S.IMouseService, this._mouseService), this.viewport = this._instantiationService.createInstance(h.Viewport, this._viewportElement, this._viewportScrollArea), this.viewport.onRequestScrollLines((e => this.scrollLines(e.amount, e.suppressScrollEvent, 1))), this.register(this._inputHandler.onRequestSyncScrollBar((() => this.viewport.syncScrollArea()))), this.register(this.viewport), this.register(this.onCursorMove((() => {
+                        this._renderService.hasRenderer() || this._renderService.setRenderer(this._createRenderer()), this.viewport = this._instantiationService.createInstance(h.Viewport, this._viewportElement, this._viewportScrollArea), this.viewport.onRequestScrollLines((e => this.scrollLines(e.amount, e.suppressScrollEvent, 1))), this.register(this._inputHandler.onRequestSyncScrollBar((() => this.viewport.syncScrollArea()))), this.register(this.viewport), this.register(this.onCursorMove((() => {
                             this._renderService.handleCursorMove(), this._syncTextArea()
-                        }))), this.register(this.onResize((() => this._renderService.handleResize(this.cols, this.rows)))), this.register(this.onBlur((() => this._renderService.handleBlur()))), this.register(this.onFocus((() => this._renderService.handleFocus()))), this.register(this._renderService.onDimensionsChange((() => this.viewport.syncScrollArea()))), this._selectionService = this.register(this._instantiationService.createInstance(m.SelectionService, this.element, this.screenElement, this.linkifier2)), this._instantiationService.setService(S.ISelectionService, this._selectionService), this.register(this._selectionService.onRequestScrollLines((e => this.scrollLines(e.amount, e.suppressScrollEvent)))), this.register(this._selectionService.onSelectionChange((() => this._onSelectionChange.fire()))), this.register(this._selectionService.onRequestRedraw((e => this._renderService.handleSelectionChanged(e.start, e.end, e.columnSelectMode)))), this.register(this._selectionService.onLinuxMouseSelection((e => {
+                        }))), this.register(this.onResize((() => this._renderService.handleResize(this.cols, this.rows)))), this.register(this.onBlur((() => this._renderService.handleBlur()))), this.register(this.onFocus((() => this._renderService.handleFocus()))), this.register(this._renderService.onDimensionsChange((() => this.viewport.syncScrollArea()))), this._selectionService = this.register(this._instantiationService.createInstance(m.SelectionService, this.element, this.screenElement, this.linkifier)), this._instantiationService.setService(S.ISelectionService, this._selectionService), this.register(this._selectionService.onRequestScrollLines((e => this.scrollLines(e.amount, e.suppressScrollEvent)))), this.register(this._selectionService.onSelectionChange((() => this._onSelectionChange.fire()))), this.register(this._selectionService.onRequestRedraw((e => this._renderService.handleSelectionChanged(e.start, e.end, e.columnSelectMode)))), this.register(this._selectionService.onLinuxMouseSelection((e => {
                             this.textarea.value = e, this.textarea.focus(), this.textarea.select()
                         }))), this.register(this._onScroll.event((e => {
                             this.viewport.syncScrollArea(), this._selectionService.refresh()
-                        }))), this.register((0, r.addDisposableDomListener)(this._viewportElement, "scroll", (() => this._selectionService.refresh()))), this.linkifier2.attachToDom(this.screenElement, this._mouseService, this._renderService), this.register(this._instantiationService.createInstance(c.BufferDecorationRenderer, this.screenElement)), this.register((0, r.addDisposableDomListener)(this.element, "mousedown", (e => this._selectionService.handleMouseDown(e)))), this.coreMouseService.areMouseEventsActive ? (this._selectionService.disable(), this.element.classList.add("enable-mouse-events")) : this._selectionService.enable(), this.options.screenReaderMode && (this._accessibilityManager.value = this._instantiationService.createInstance(M.AccessibilityManager, this)), this.register(this.optionsService.onSpecificOptionChange("screenReaderMode", (e => this._handleScreenReaderModeOptionChange(e)))), this.options.overviewRulerWidth && (this._overviewRulerRenderer = this.register(this._instantiationService.createInstance(l.OverviewRulerRenderer, this._viewportElement, this.screenElement))), this.optionsService.onSpecificOptionChange("overviewRulerWidth", (e => {
+                        }))), this.register((0, r.addDisposableDomListener)(this._viewportElement, "scroll", (() => this._selectionService.refresh()))), this.register(this._instantiationService.createInstance(c.BufferDecorationRenderer, this.screenElement)), this.register((0, r.addDisposableDomListener)(this.element, "mousedown", (e => this._selectionService.handleMouseDown(e)))), this.coreMouseService.areMouseEventsActive ? (this._selectionService.disable(), this.element.classList.add("enable-mouse-events")) : this._selectionService.enable(), this.options.screenReaderMode && (this._accessibilityManager.value = this._instantiationService.createInstance(M.AccessibilityManager, this)), this.register(this.optionsService.onSpecificOptionChange("screenReaderMode", (e => this._handleScreenReaderModeOptionChange(e)))), this.options.overviewRulerWidth && (this._overviewRulerRenderer = this.register(this._instantiationService.createInstance(l.OverviewRulerRenderer, this._viewportElement, this.screenElement))), this.optionsService.onSpecificOptionChange("overviewRulerWidth", (e => {
                             !this._overviewRulerRenderer && e && this._viewportElement && this.screenElement && (this._overviewRulerRenderer = this.register(this._instantiationService.createInstance(l.OverviewRulerRenderer, this._viewportElement, this.screenElement)))
                         })), this._charSizeService.measure(), this.refresh(0, this.rows - 1), this._initGlobal(), this.bindMouse()
                     }
                     _createRenderer() {
-                        return this._instantiationService.createInstance(_.DomRenderer, this._document, this.element, this.screenElement, this._viewportElement, this._helperContainer, this.linkifier2)
+                        return this._instantiationService.createInstance(_.DomRenderer, this, this._document, this.element, this.screenElement, this._viewportElement, this._helperContainer, this.linkifier)
                     }
                     bindMouse() {
                         const e = this,
                             t = this.element;
 
                         function i(t) {
                             const i = e._mouseService.getMouseReportCoords(t, e.screenElement);
@@ -673,14 +713,15 @@
                                 case "mouseup":
                                     r = 0, s = t.button < 3 ? t.button : 3;
                                     break;
                                 case "mousedown":
                                     r = 1, s = t.button < 3 ? t.button : 3;
                                     break;
                                 case "wheel":
+                                    if (e._customWheelEventHandler && !1 === e._customWheelEventHandler(t)) return !1;
                                     if (0 === e.viewport.getLinesScrolled(t)) return !1;
                                     r = t.deltaY < 0 ? 0 : 1, s = 4;
                                     break;
                                 default:
                                     return !1
                             }
                             return !(void 0 === r || void 0 === s || s > 4) && e.coreMouseService.triggerMouseEvent({
@@ -715,14 +756,15 @@
                             e ? ("debug" === this.optionsService.rawOptions.logLevel && this._logService.debug("Binding to mouse events:", this.coreMouseService.explainEvents(e)), this.element.classList.add("enable-mouse-events"), this._selectionService.disable()) : (this._logService.debug("Unbinding from mouse events."), this.element.classList.remove("enable-mouse-events"), this._selectionService.enable()), 8 & e ? s.mousemove || (t.addEventListener("mousemove", n.mousemove), s.mousemove = n.mousemove) : (t.removeEventListener("mousemove", s.mousemove), s.mousemove = null), 16 & e ? s.wheel || (t.addEventListener("wheel", n.wheel, {
                                 passive: !1
                             }), s.wheel = n.wheel) : (t.removeEventListener("wheel", s.wheel), s.wheel = null), 2 & e ? s.mouseup || (s.mouseup = n.mouseup) : (this._document.removeEventListener("mouseup", s.mouseup), s.mouseup = null), 4 & e ? s.mousedrag || (s.mousedrag = n.mousedrag) : (this._document.removeEventListener("mousemove", s.mousedrag), s.mousedrag = null)
                         }))), this.coreMouseService.activeProtocol = this.coreMouseService.activeProtocol, this.register((0, r.addDisposableDomListener)(t, "mousedown", (e => {
                             if (e.preventDefault(), this.focus(), this.coreMouseService.areMouseEventsActive && !this._selectionService.shouldForceSelection(e)) return i(e), s.mouseup && this._document.addEventListener("mouseup", s.mouseup), s.mousedrag && this._document.addEventListener("mousemove", s.mousedrag), this.cancel(e)
                         }))), this.register((0, r.addDisposableDomListener)(t, "wheel", (e => {
                             if (!s.wheel) {
+                                if (this._customWheelEventHandler && !1 === this._customWheelEventHandler(e)) return !1;
                                 if (!this.buffer.hasScrollback) {
                                     const t = this.viewport.getLinesScrolled(e);
                                     if (0 === t) return;
                                     const i = D.C0.ESC + (this.coreService.decPrivateModes.applicationCursorKeys ? "O" : "[") + (e.deltaY < 0 ? "A" : "B");
                                     let s = "";
                                     for (let e = 0; e < Math.abs(t); e++) s += i;
                                     return this.coreService.triggerDataEvent(s, !0), this.cancel(e, !0)
@@ -755,16 +797,19 @@
                     }
                     paste(e) {
                         (0, s.paste)(e, this.textarea, this.coreService, this.optionsService)
                     }
                     attachCustomKeyEventHandler(e) {
                         this._customKeyEventHandler = e
                     }
+                    attachCustomWheelEventHandler(e) {
+                        this._customWheelEventHandler = e
+                    }
                     registerLinkProvider(e) {
-                        return this.linkifier2.registerLinkProvider(e)
+                        return this._linkProviderService.registerLinkProvider(e)
                     }
                     registerCharacterJoiner(e) {
                         if (!this._characterJoinerService) throw new Error("Terminal must be opened first");
                         const t = this._characterJoinerService.register(e);
                         return this.refresh(0, this.rows - 1), t
                     }
                     deregisterCharacterJoiner(e) {
@@ -898,15 +943,15 @@
                                 this.coreService.triggerDataEvent(`${D.C0.ESC}[6;${s};${i}t`)
                         }
                     }
                     cancel(e, t) {
                         if (this.options.cancelEvents || t) return e.preventDefault(), e.stopPropagation(), !1
                     }
                 }
-                t.Terminal = O
+                t.Terminal = P
             },
             9924: (e, t) => {
                 Object.defineProperty(t, "__esModule", {
                     value: !0
                 }), t.TimeBasedDebouncer = void 0, t.TimeBasedDebouncer = class {
                     constructor(e, t = 1e3) {
                         this._renderCallback = e, this._debounceThresholdMS = t, this._lastRefreshMs = 0, this._additionalRefreshRequested = !1
@@ -1500,46 +1545,51 @@
                 Object.defineProperty(t, "__esModule", {
                     value: !0
                 }), t.DomRenderer = void 0;
                 const n = i(3787),
                     o = i(2550),
                     a = i(2223),
                     h = i(6171),
-                    c = i(4725),
-                    l = i(8055),
-                    d = i(8460),
-                    _ = i(844),
-                    u = i(2585),
-                    f = "xterm-dom-renderer-owner-",
-                    v = "xterm-rows",
+                    c = i(6052),
+                    l = i(4725),
+                    d = i(8055),
+                    _ = i(8460),
+                    u = i(844),
+                    f = i(2585),
+                    v = "xterm-dom-renderer-owner-",
+                    p = "xterm-rows",
                     g = "xterm-fg-",
-                    p = "xterm-bg-",
-                    m = "xterm-focus",
-                    S = "xterm-selection";
-                let C = 1,
-                    b = t.DomRenderer = class extends _.Disposable {
-                        constructor(e, t, i, s, r, a, c, l, u, g, p, m) {
-                            super(), this._document = e, this._element = t, this._screenElement = i, this._viewportElement = s, this._helperContainer = r, this._linkifier2 = a, this._charSizeService = l, this._optionsService = u, this._bufferService = g, this._coreBrowserService = p, this._themeService = m, this._terminalClass = C++, this._rowElements = [], this.onRequestRedraw = this.register(new d.EventEmitter).event, this._rowContainer = this._document.createElement("div"), this._rowContainer.classList.add(v), this._rowContainer.style.lineHeight = "normal", this._rowContainer.setAttribute("aria-hidden", "true"), this._refreshRowElements(this._bufferService.cols, this._bufferService.rows), this._selectionContainer = this._document.createElement("div"), this._selectionContainer.classList.add(S), this._selectionContainer.setAttribute("aria-hidden", "true"), this.dimensions = (0, h.createRenderDimensions)(), this._updateDimensions(), this.register(this._optionsService.onOptionChange((() => this._handleOptionsChanged()))), this.register(this._themeService.onChangeColors((e => this._injectCss(e)))), this._injectCss(this._themeService.colors), this._rowFactory = c.createInstance(n.DomRendererRowFactory, document), this._element.classList.add(f + this._terminalClass), this._screenElement.appendChild(this._rowContainer), this._screenElement.appendChild(this._selectionContainer), this.register(this._linkifier2.onShowLinkUnderline((e => this._handleLinkHover(e)))), this.register(this._linkifier2.onHideLinkUnderline((e => this._handleLinkLeave(e)))), this.register((0, _.toDisposable)((() => {
-                                this._element.classList.remove(f + this._terminalClass), this._rowContainer.remove(), this._selectionContainer.remove(), this._widthCache.dispose(), this._themeStyleElement.remove(), this._dimensionsStyleElement.remove()
+                    m = "xterm-bg-",
+                    S = "xterm-focus",
+                    C = "xterm-selection";
+                let b = 1,
+                    w = t.DomRenderer = class extends u.Disposable {
+                        constructor(e, t, i, s, r, a, l, d, f, g, m, S, w) {
+                            super(), this._terminal = e, this._document = t, this._element = i, this._screenElement = s, this._viewportElement = r, this._helperContainer = a, this._linkifier2 = l, this._charSizeService = f, this._optionsService = g, this._bufferService = m, this._coreBrowserService = S, this._themeService = w, this._terminalClass = b++, this._rowElements = [], this._selectionRenderModel = (0, c.createSelectionRenderModel)(), this.onRequestRedraw = this.register(new _.EventEmitter).event, this._rowContainer = this._document.createElement("div"), this._rowContainer.classList.add(p), this._rowContainer.style.lineHeight = "normal", this._rowContainer.setAttribute("aria-hidden", "true"), this._refreshRowElements(this._bufferService.cols, this._bufferService.rows), this._selectionContainer = this._document.createElement("div"), this._selectionContainer.classList.add(C), this._selectionContainer.setAttribute("aria-hidden", "true"), this.dimensions = (0, h.createRenderDimensions)(), this._updateDimensions(), this.register(this._optionsService.onOptionChange((() => this._handleOptionsChanged()))), this.register(this._themeService.onChangeColors((e => this._injectCss(e)))), this._injectCss(this._themeService.colors), this._rowFactory = d.createInstance(n.DomRendererRowFactory, document), this._element.classList.add(v + this._terminalClass), this._screenElement.appendChild(this._rowContainer), this._screenElement.appendChild(this._selectionContainer), this.register(this._linkifier2.onShowLinkUnderline((e => this._handleLinkHover(e)))), this.register(this._linkifier2.onHideLinkUnderline((e => this._handleLinkLeave(e)))), this.register((0, u.toDisposable)((() => {
+                                this._element.classList.remove(v + this._terminalClass), this._rowContainer.remove(), this._selectionContainer.remove(), this._widthCache.dispose(), this._themeStyleElement.remove(), this._dimensionsStyleElement.remove()
                             }))), this._widthCache = new o.WidthCache(this._document, this._helperContainer), this._widthCache.setFont(this._optionsService.rawOptions.fontFamily, this._optionsService.rawOptions.fontSize, this._optionsService.rawOptions.fontWeight, this._optionsService.rawOptions.fontWeightBold), this._setDefaultSpacing()
                         }
                         _updateDimensions() {
                             const e = this._coreBrowserService.dpr;
                             this.dimensions.device.char.width = this._charSizeService.width * e, this.dimensions.device.char.height = Math.ceil(this._charSizeService.height * e), this.dimensions.device.cell.width = this.dimensions.device.char.width + Math.round(this._optionsService.rawOptions.letterSpacing), this.dimensions.device.cell.height = Math.floor(this.dimensions.device.char.height * this._optionsService.rawOptions.lineHeight), this.dimensions.device.char.left = 0, this.dimensions.device.char.top = 0, this.dimensions.device.canvas.width = this.dimensions.device.cell.width * this._bufferService.cols, this.dimensions.device.canvas.height = this.dimensions.device.cell.height * this._bufferService.rows, this.dimensions.css.canvas.width = Math.round(this.dimensions.device.canvas.width / e), this.dimensions.css.canvas.height = Math.round(this.dimensions.device.canvas.height / e), this.dimensions.css.cell.width = this.dimensions.css.canvas.width / this._bufferService.cols, this.dimensions.css.cell.height = this.dimensions.css.canvas.height / this._bufferService.rows;
                             for (const e of this._rowElements) e.style.width = `${this.dimensions.css.canvas.width}px`, e.style.height = `${this.dimensions.css.cell.height}px`, e.style.lineHeight = `${this.dimensions.css.cell.height}px`, e.style.overflow = "hidden";
                             this._dimensionsStyleElement || (this._dimensionsStyleElement = this._document.createElement("style"), this._screenElement.appendChild(this._dimensionsStyleElement));
-                            const t = `${this._terminalSelector} .${v} span { display: inline-block; height: 100%; vertical-align: top;}`;
+                            const t = `${this._terminalSelector} .${p} span { display: inline-block; height: 100%; vertical-align: top;}`;
                             this._dimensionsStyleElement.textContent = t, this._selectionContainer.style.height = this._viewportElement.style.height, this._screenElement.style.width = `${this.dimensions.css.canvas.width}px`, this._screenElement.style.height = `${this.dimensions.css.canvas.height}px`
                         }
                         _injectCss(e) {
                             this._themeStyleElement || (this._themeStyleElement = this._document.createElement("style"), this._screenElement.appendChild(this._themeStyleElement));
-                            let t = `${this._terminalSelector} .${v} { color: ${e.foreground.css}; font-family: ${this._optionsService.rawOptions.fontFamily}; font-size: ${this._optionsService.rawOptions.fontSize}px; font-kerning: none; white-space: pre}`;
-                            t += `${this._terminalSelector} .${v} .xterm-dim { color: ${l.color.multiplyOpacity(e.foreground,.5).css};}`, t += `${this._terminalSelector} span:not(.xterm-bold) { font-weight: ${this._optionsService.rawOptions.fontWeight};}${this._terminalSelector} span.xterm-bold { font-weight: ${this._optionsService.rawOptions.fontWeightBold};}${this._terminalSelector} span.xterm-italic { font-style: italic;}`, t += "@keyframes blink_box_shadow_" + this._terminalClass + " { 50% {  border-bottom-style: hidden; }}", t += "@keyframes blink_block_" + this._terminalClass + " { 0% {" + `  background-color: ${e.cursor.css};` + `  color: ${e.cursorAccent.css}; } 50% {  background-color: inherit;` + `  color: ${e.cursor.css}; }}`, t += `${this._terminalSelector} .${v}.${m} .xterm-cursor.xterm-cursor-blink:not(.xterm-cursor-block) { animation: blink_box_shadow_` + this._terminalClass + " 1s step-end infinite;}" + `${this._terminalSelector} .${v}.${m} .xterm-cursor.xterm-cursor-blink.xterm-cursor-block { animation: blink_block_` + this._terminalClass + " 1s step-end infinite;}" + `${this._terminalSelector} .${v} .xterm-cursor.xterm-cursor-block {` + ` background-color: ${e.cursor.css} !important;` + ` color: ${e.cursorAccent.css} !important;}` + `${this._terminalSelector} .${v} .xterm-cursor.xterm-cursor-outline {` + ` outline: 1px solid ${e.cursor.css}; outline-offset: -1px;}` + `${this._terminalSelector} .${v} .xterm-cursor.xterm-cursor-bar {` + ` box-shadow: ${this._optionsService.rawOptions.cursorWidth}px 0 0 ${e.cursor.css} inset;}` + `${this._terminalSelector} .${v} .xterm-cursor.xterm-cursor-underline {` + ` border-bottom: 1px ${e.cursor.css}; border-bottom-style: solid; height: calc(100% - 1px);}`, t += `${this._terminalSelector} .${S} { position: absolute; top: 0; left: 0; z-index: 1; pointer-events: none;}${this._terminalSelector}.focus .${S} div { position: absolute; background-color: ${e.selectionBackgroundOpaque.css};}${this._terminalSelector} .${S} div { position: absolute; background-color: ${e.selectionInactiveBackgroundOpaque.css};}`;
-                            for (const [i, s] of e.ansi.entries()) t += `${this._terminalSelector} .${g}${i} { color: ${s.css}; }${this._terminalSelector} .${g}${i}.xterm-dim { color: ${l.color.multiplyOpacity(s,.5).css}; }${this._terminalSelector} .${p}${i} { background-color: ${s.css}; }`;
-                            t += `${this._terminalSelector} .${g}${a.INVERTED_DEFAULT_COLOR} { color: ${l.color.opaque(e.background).css}; }${this._terminalSelector} .${g}${a.INVERTED_DEFAULT_COLOR}.xterm-dim { color: ${l.color.multiplyOpacity(l.color.opaque(e.background),.5).css}; }${this._terminalSelector} .${p}${a.INVERTED_DEFAULT_COLOR} { background-color: ${e.foreground.css}; }`, this._themeStyleElement.textContent = t
+                            let t = `${this._terminalSelector} .${p} { color: ${e.foreground.css}; font-family: ${this._optionsService.rawOptions.fontFamily}; font-size: ${this._optionsService.rawOptions.fontSize}px; font-kerning: none; white-space: pre}`;
+                            t += `${this._terminalSelector} .${p} .xterm-dim { color: ${d.color.multiplyOpacity(e.foreground,.5).css};}`, t += `${this._terminalSelector} span:not(.xterm-bold) { font-weight: ${this._optionsService.rawOptions.fontWeight};}${this._terminalSelector} span.xterm-bold { font-weight: ${this._optionsService.rawOptions.fontWeightBold};}${this._terminalSelector} span.xterm-italic { font-style: italic;}`;
+                            const i = `blink_underline_${this._terminalClass}`,
+                                s = `blink_bar_${this._terminalClass}`,
+                                r = `blink_block_${this._terminalClass}`;
+                            t += `@keyframes ${i} { 50% {  border-bottom-style: hidden; }}`, t += `@keyframes ${s} { 50% {  box-shadow: none; }}`, t += `@keyframes ${r} { 0% {  background-color: ${e.cursor.css};  color: ${e.cursorAccent.css}; } 50% {  background-color: inherit;  color: ${e.cursor.css}; }}`, t += `${this._terminalSelector} .${p}.${S} .xterm-cursor.xterm-cursor-blink.xterm-cursor-underline { animation: ${i} 1s step-end infinite;}${this._terminalSelector} .${p}.${S} .xterm-cursor.xterm-cursor-blink.xterm-cursor-bar { animation: ${s} 1s step-end infinite;}${this._terminalSelector} .${p}.${S} .xterm-cursor.xterm-cursor-blink.xterm-cursor-block { animation: ${r} 1s step-end infinite;}${this._terminalSelector} .${p} .xterm-cursor.xterm-cursor-block { background-color: ${e.cursor.css}; color: ${e.cursorAccent.css};}${this._terminalSelector} .${p} .xterm-cursor.xterm-cursor-block:not(.xterm-cursor-blink) { background-color: ${e.cursor.css} !important; color: ${e.cursorAccent.css} !important;}${this._terminalSelector} .${p} .xterm-cursor.xterm-cursor-outline { outline: 1px solid ${e.cursor.css}; outline-offset: -1px;}${this._terminalSelector} .${p} .xterm-cursor.xterm-cursor-bar { box-shadow: ${this._optionsService.rawOptions.cursorWidth}px 0 0 ${e.cursor.css} inset;}${this._terminalSelector} .${p} .xterm-cursor.xterm-cursor-underline { border-bottom: 1px ${e.cursor.css}; border-bottom-style: solid; height: calc(100% - 1px);}`, t += `${this._terminalSelector} .${C} { position: absolute; top: 0; left: 0; z-index: 1; pointer-events: none;}${this._terminalSelector}.focus .${C} div { position: absolute; background-color: ${e.selectionBackgroundOpaque.css};}${this._terminalSelector} .${C} div { position: absolute; background-color: ${e.selectionInactiveBackgroundOpaque.css};}`;
+                            for (const [i, s] of e.ansi.entries()) t += `${this._terminalSelector} .${g}${i} { color: ${s.css}; }${this._terminalSelector} .${g}${i}.xterm-dim { color: ${d.color.multiplyOpacity(s,.5).css}; }${this._terminalSelector} .${m}${i} { background-color: ${s.css}; }`;
+                            t += `${this._terminalSelector} .${g}${a.INVERTED_DEFAULT_COLOR} { color: ${d.color.opaque(e.background).css}; }${this._terminalSelector} .${g}${a.INVERTED_DEFAULT_COLOR}.xterm-dim { color: ${d.color.multiplyOpacity(d.color.opaque(e.background),.5).css}; }${this._terminalSelector} .${m}${a.INVERTED_DEFAULT_COLOR} { background-color: ${e.foreground.css}; }`, this._themeStyleElement.textContent = t
                         }
                         _setDefaultSpacing() {
                             const e = this.dimensions.css.cell.width - this._widthCache.get("W", !1, !1);
                             this._rowContainer.style.letterSpacing = `${e}px`, this._rowFactory.defaultSpacing = e
                         }
                         handleDevicePixelRatioChange() {
                             this._updateDimensions(), this._widthCache.clear(), this._setDefaultSpacing()
@@ -1548,31 +1598,32 @@
                             for (let e = this._rowElements.length; e <= t; e++) {
                                 const e = this._document.createElement("div");
                                 this._rowContainer.appendChild(e), this._rowElements.push(e)
                             }
                             for (; this._rowElements.length > t;) this._rowContainer.removeChild(this._rowElements.pop())
                         }
                         handleResize(e, t) {
-                            this._refreshRowElements(e, t), this._updateDimensions()
+                            this._refreshRowElements(e, t), this._updateDimensions(), this.handleSelectionChanged(this._selectionRenderModel.selectionStart, this._selectionRenderModel.selectionEnd, this._selectionRenderModel.columnSelectMode)
                         }
                         handleCharSizeChanged() {
                             this._updateDimensions(), this._widthCache.clear(), this._setDefaultSpacing()
                         }
                         handleBlur() {
-                            this._rowContainer.classList.remove(m), this.renderRows(0, this._bufferService.rows - 1)
+                            this._rowContainer.classList.remove(S), this.renderRows(0, this._bufferService.rows - 1)
                         }
                         handleFocus() {
-                            this._rowContainer.classList.add(m), this.renderRows(this._bufferService.buffer.y, this._bufferService.buffer.y)
+                            this._rowContainer.classList.add(S), this.renderRows(this._bufferService.buffer.y, this._bufferService.buffer.y)
                         }
                         handleSelectionChanged(e, t, i) {
                             if (this._selectionContainer.replaceChildren(), this._rowFactory.handleSelectionChanged(e, t, i), this.renderRows(0, this._bufferService.rows - 1), !e || !t) return;
-                            const s = e[1] - this._bufferService.buffer.ydisp,
-                                r = t[1] - this._bufferService.buffer.ydisp,
-                                n = Math.max(s, 0),
-                                o = Math.min(r, this._bufferService.rows - 1);
+                            this._selectionRenderModel.update(this._terminal, e, t, i);
+                            const s = this._selectionRenderModel.viewportStartRow,
+                                r = this._selectionRenderModel.viewportEndRow,
+                                n = this._selectionRenderModel.viewportCappedStartRow,
+                                o = this._selectionRenderModel.viewportCappedEndRow;
                             if (n >= this._bufferService.rows || o < 0) return;
                             const a = this._document.createDocumentFragment();
                             if (i) {
                                 const i = e[0] > t[0];
                                 a.appendChild(this._createSelectionElement(n, i ? t[0] : e[0], i ? e[0] : t[0], o - n + 1))
                             } else {
                                 const i = s === n ? e[0] : 0,
@@ -1583,16 +1634,18 @@
                                     const e = r === o ? t[0] : this._bufferService.cols;
                                     a.appendChild(this._createSelectionElement(o, 0, e))
                                 }
                             }
                             this._selectionContainer.appendChild(a)
                         }
                         _createSelectionElement(e, t, i, s = 1) {
-                            const r = this._document.createElement("div");
-                            return r.style.height = s * this.dimensions.css.cell.height + "px", r.style.top = e * this.dimensions.css.cell.height + "px", r.style.left = t * this.dimensions.css.cell.width + "px", r.style.width = this.dimensions.css.cell.width * (i - t) + "px", r
+                            const r = this._document.createElement("div"),
+                                n = t * this.dimensions.css.cell.width;
+                            let o = this.dimensions.css.cell.width * (i - t);
+                            return n + o > this.dimensions.css.canvas.width && (o = this.dimensions.css.canvas.width - n), r.style.height = s * this.dimensions.css.cell.height + "px", r.style.top = e * this.dimensions.css.cell.height + "px", r.style.left = `${n}px`, r.style.width = `${o}px`, r
                         }
                         handleCursorMove() {}
                         _handleOptionsChanged() {
                             this._updateDimensions(), this._injectCss(this._themeService.colors), this._widthCache.setFont(this._optionsService.rawOptions.fontFamily, this._optionsService.rawOptions.fontSize, this._optionsService.rawOptions.fontWeight, this._optionsService.rawOptions.fontWeightBold), this._setDefaultSpacing()
                         }
                         clear() {
                             for (const e of this._rowElements) e.replaceChildren()
@@ -1609,15 +1662,15 @@
                                     t = this._rowElements[h],
                                     c = i.lines.get(e);
                                 if (!t || !c) break;
                                 t.replaceChildren(...this._rowFactory.createRow(c, e, e === s, o, a, r, n, this.dimensions.css.cell.width, this._widthCache, -1, -1))
                             }
                         }
                         get _terminalSelector() {
-                            return `.${f}${this._terminalClass}`
+                            return `.${v}${this._terminalClass}`
                         }
                         _handleLinkHover(e) {
                             this._setCellUnderline(e.x1, e.x2, e.y1, e.y2, e.cols, !0)
                         }
                         _handleLinkLeave(e) {
                             this._setCellUnderline(e.x1, e.x2, e.y1, e.y2, e.cols, !1)
                         }
@@ -1636,15 +1689,15 @@
                                     f = this._rowElements[o],
                                     v = a.lines.get(u);
                                 if (!f || !v) break;
                                 f.replaceChildren(...this._rowFactory.createRow(v, u, u === h, d, _, c, l, this.dimensions.css.cell.width, this._widthCache, n ? o === i ? e : 0 : -1, n ? (o === s ? t : r) - 1 : -1))
                             }
                         }
                     };
-                t.DomRenderer = b = s([r(6, u.IInstantiationService), r(7, c.ICharSizeService), r(8, u.IOptionsService), r(9, u.IBufferService), r(10, c.ICoreBrowserService), r(11, c.IThemeService)], b)
+                t.DomRenderer = w = s([r(7, f.IInstantiationService), r(8, l.ICharSizeService), r(9, f.IOptionsService), r(10, f.IBufferService), r(11, l.ICoreBrowserService), r(12, l.IThemeService)], w)
             },
             3787: function(e, t, i) {
                 var s = this && this.__decorate || function(e, t, i, s) {
                         var r, n = arguments.length,
                             o = n < 3 ? t : null === s ? s = Object.getOwnPropertyDescriptor(t, i) : s;
                         if ("object" == typeof Reflect && "function" == typeof Reflect.decorate) o = Reflect.decorate(e, t, i, s);
                         else
@@ -1671,57 +1724,57 @@
                 let f = t.DomRendererRowFactory = class {
                     constructor(e, t, i, s, r, n, o) {
                         this._document = e, this._characterJoinerService = t, this._optionsService = i, this._coreBrowserService = s, this._coreService = r, this._decorationService = n, this._themeService = o, this._workCell = new a.CellData, this._columnSelectMode = !1, this.defaultSpacing = 0
                     }
                     handleSelectionChanged(e, t, i) {
                         this._selectionStart = e, this._selectionEnd = t, this._columnSelectMode = i
                     }
-                    createRow(e, t, i, s, r, a, h, l, _, f, g) {
-                        const p = [],
+                    createRow(e, t, i, s, r, a, h, l, _, f, p) {
+                        const g = [],
                             m = this._characterJoinerService.getJoinedCharacters(t),
                             S = this._themeService.colors;
                         let C, b = e.getNoBgTrimmedLength();
                         i && b < a + 1 && (b = a + 1);
-                        let y = 0,
-                            w = "",
+                        let w = 0,
+                            y = "",
                             E = 0,
                             k = 0,
                             L = 0,
                             D = !1,
                             R = 0,
                             x = !1,
                             A = 0;
                         const B = [],
-                            T = -1 !== f && -1 !== g;
+                            T = -1 !== f && -1 !== p;
                         for (let M = 0; M < b; M++) {
                             e.loadCell(M, this._workCell);
                             let b = this._workCell.getWidth();
                             if (0 === b) continue;
                             let O = !1,
                                 P = M,
                                 I = this._workCell;
                             if (m.length > 0 && M === m[0][0]) {
                                 O = !0;
                                 const t = m.shift();
                                 I = new d.JoinedCellData(this._workCell, e.translateToString(!0, t[0], t[1]), t[1] - t[0]), P = t[1] - 1, b = I.getWidth()
                             }
                             const H = this._isCellInSelection(M, t),
                                 F = i && M === a,
-                                W = T && M >= f && M <= g;
+                                W = T && M >= f && M <= p;
                             let U = !1;
                             this._decorationService.forEachDecorationAtCell(M, t, void 0, (e => {
                                 U = !0
                             }));
                             let N = I.getChars() || o.WHITESPACE_CELL_CHAR;
                             if (" " === N && (I.isUnderline() || I.isOverline()) && (N = " "), A = b * l - _.get(N, I.isBold(), I.isItalic()), C) {
-                                if (y && (H && x || !H && !x && I.bg === E) && (H && x && S.selectionForeground || I.fg === k) && I.extended.ext === L && W === D && A === R && !F && !O && !U) {
-                                    I.isInvisible() ? w += o.WHITESPACE_CELL_CHAR : w += N, y++;
+                                if (w && (H && x || !H && !x && I.bg === E) && (H && x && S.selectionForeground || I.fg === k) && I.extended.ext === L && W === D && A === R && !F && !O && !U) {
+                                    I.isInvisible() ? y += o.WHITESPACE_CELL_CHAR : y += N, w++;
                                     continue
                                 }
-                                y && (C.textContent = w), C = this._document.createElement("span"), y = 0, w = ""
+                                w && (C.textContent = y), C = this._document.createElement("span"), w = 0, y = ""
                             } else C = this._document.createElement("span");
                             if (E = I.bg, k = I.fg, L = I.extended.ext, D = W, R = A, x = H, O && a >= M && a <= P && (a = M), !this._coreService.isCursorHidden && F && this._coreService.isCursorInitialized)
                                 if (B.push("xterm-cursor"), this._coreBrowserService.isFocused) h && B.push("xterm-cursor-blink"), B.push("bar" === s ? "xterm-cursor-bar" : "underline" === s ? "xterm-cursor-underline" : "xterm-cursor-block");
                                 else if (r) switch (r) {
                                 case "outline":
                                     B.push("xterm-cursor-outline");
                                     break;
@@ -1730,20 +1783,20 @@
                                     break;
                                 case "bar":
                                     B.push("xterm-cursor-bar");
                                     break;
                                 case "underline":
                                     B.push("xterm-cursor-underline")
                             }
-                            if (I.isBold() && B.push("xterm-bold"), I.isItalic() && B.push("xterm-italic"), I.isDim() && B.push("xterm-dim"), w = I.isInvisible() ? o.WHITESPACE_CELL_CHAR : I.getChars() || o.WHITESPACE_CELL_CHAR, I.isUnderline() && (B.push(`xterm-underline-${I.extended.underlineStyle}`), " " === w && (w = " "), !I.isUnderlineColorDefault()))
+                            if (I.isBold() && B.push("xterm-bold"), I.isItalic() && B.push("xterm-italic"), I.isDim() && B.push("xterm-dim"), y = I.isInvisible() ? o.WHITESPACE_CELL_CHAR : I.getChars() || o.WHITESPACE_CELL_CHAR, I.isUnderline() && (B.push(`xterm-underline-${I.extended.underlineStyle}`), " " === y && (y = " "), !I.isUnderlineColorDefault()))
                                 if (I.isUnderlineColorRGB()) C.style.textDecorationColor = `rgb(${u.AttributeData.toColorRGB(I.getUnderlineColor()).join(",")})`;
                                 else {
                                     let e = I.getUnderlineColor();
                                     this._optionsService.rawOptions.drawBoldTextInBrightColors && I.isBold() && e < 8 && (e += 8), C.style.textDecorationColor = S.ansi[e].css
-                                } I.isOverline() && (B.push("xterm-overline"), " " === w && (w = " ")), I.isStrikethrough() && B.push("xterm-strikethrough"), W && (C.style.textDecoration = "underline");
+                                } I.isOverline() && (B.push("xterm-overline"), " " === y && (y = " ")), I.isStrikethrough() && B.push("xterm-strikethrough"), W && (C.style.textDecoration = "underline");
                             let $ = I.getFgColor(),
                                 j = I.getFgColorMode(),
                                 z = I.getBgColor(),
                                 K = I.getBgColorMode();
                             const q = !!I.isInverse();
                             if (q) {
                                 const e = $;
@@ -1756,37 +1809,37 @@
                                     "top" !== e.options.layer && J || (e.backgroundColorRGB && (K = 50331648, z = e.backgroundColorRGB.rgba >> 8 & 16777215, V = e.backgroundColorRGB), e.foregroundColorRGB && (j = 50331648, $ = e.foregroundColorRGB.rgba >> 8 & 16777215, G = e.foregroundColorRGB), J = "top" === e.options.layer)
                                 })), !J && H && (V = this._coreBrowserService.isFocused ? S.selectionBackgroundOpaque : S.selectionInactiveBackgroundOpaque, z = V.rgba >> 8 & 16777215, K = 50331648, J = !0, S.selectionForeground && (j = 50331648, $ = S.selectionForeground.rgba >> 8 & 16777215, G = S.selectionForeground)), J && B.push("xterm-decoration-top"), K) {
                                 case 16777216:
                                 case 33554432:
                                     X = S.ansi[z], B.push(`xterm-bg-${z}`);
                                     break;
                                 case 50331648:
-                                    X = c.rgba.toColor(z >> 16, z >> 8 & 255, 255 & z), this._addStyle(C, `background-color:#${v((z>>>0).toString(16),"0",6)}`);
+                                    X = c.channels.toColor(z >> 16, z >> 8 & 255, 255 & z), this._addStyle(C, `background-color:#${v((z>>>0).toString(16),"0",6)}`);
                                     break;
                                 default:
                                     q ? (X = S.foreground, B.push(`xterm-bg-${n.INVERTED_DEFAULT_COLOR}`)) : X = S.background
                             }
                             switch (V || I.isDim() && (V = c.color.multiplyOpacity(X, .5)), j) {
                                 case 16777216:
                                 case 33554432:
                                     I.isBold() && $ < 8 && this._optionsService.rawOptions.drawBoldTextInBrightColors && ($ += 8), this._applyMinimumContrast(C, X, S.ansi[$], I, V, void 0) || B.push(`xterm-fg-${$}`);
                                     break;
                                 case 50331648:
-                                    const e = c.rgba.toColor($ >> 16 & 255, $ >> 8 & 255, 255 & $);
+                                    const e = c.channels.toColor($ >> 16 & 255, $ >> 8 & 255, 255 & $);
                                     this._applyMinimumContrast(C, X, e, I, V, G) || this._addStyle(C, `color:#${v($.toString(16),"0",6)}`);
                                     break;
                                 default:
                                     this._applyMinimumContrast(C, X, S.foreground, I, V, G) || q && B.push(`xterm-fg-${n.INVERTED_DEFAULT_COLOR}`)
                             }
-                            B.length && (C.className = B.join(" "), B.length = 0), F || O || U ? C.textContent = w : y++, A !== this.defaultSpacing && (C.style.letterSpacing = `${A}px`), p.push(C), M = P
+                            B.length && (C.className = B.join(" "), B.length = 0), F || O || U ? C.textContent = y : w++, A !== this.defaultSpacing && (C.style.letterSpacing = `${A}px`), g.push(C), M = P
                         }
-                        return C && y && (C.textContent = w), p
+                        return C && w && (C.textContent = y), g
                     }
                     _applyMinimumContrast(e, t, i, s, r, n) {
-                        if (1 === this._optionsService.rawOptions.minimumContrastRatio || (0, _.excludeFromContrastRatioDemands)(s.getCode())) return !1;
+                        if (1 === this._optionsService.rawOptions.minimumContrastRatio || (0, _.treatGlyphAsBackgroundColor)(s.getCode())) return !1;
                         const o = this._getContrastCache(s);
                         let a;
                         if (r || n || (a = o.getColor(t.rgba, i.rgba)), void 0 === a) {
                             const e = this._optionsService.rawOptions.minimumContrastRatio / (s.isDim() ? 2 : 1);
                             a = c.color.ensureContrastRatio(r || t, n || i, e), o.setColor((r || t).rgba, (n || i).rgba, a ?? null)
                         }
                         return !!a && (this._addStyle(e, `color:${a.css}`), !0)
@@ -1832,21 +1885,25 @@
                         this._flat.fill(-9999), this._holey = new Map
                     }
                     setFont(e, t, i, s) {
                         e === this._font && t === this._fontSize && i === this._weight && s === this._weightBold || (this._font = e, this._fontSize = t, this._weight = i, this._weightBold = s, this._container.style.fontFamily = this._font, this._container.style.fontSize = `${this._fontSize}px`, this._measureElements[0].style.fontWeight = `${i}`, this._measureElements[1].style.fontWeight = `${s}`, this._measureElements[2].style.fontWeight = `${i}`, this._measureElements[3].style.fontWeight = `${s}`, this.clear())
                     }
                     get(e, t, i) {
                         let s = 0;
-                        if (!t && !i && 1 === e.length && (s = e.charCodeAt(0)) < 256) return -9999 !== this._flat[s] ? this._flat[s] : this._flat[s] = this._measure(e, 0);
+                        if (!t && !i && 1 === e.length && (s = e.charCodeAt(0)) < 256) {
+                            if (-9999 !== this._flat[s]) return this._flat[s];
+                            const t = this._measure(e, 0);
+                            return t > 0 && (this._flat[s] = t), t
+                        }
                         let r = e;
                         t && (r += "B"), i && (r += "I");
                         let n = this._holey.get(r);
                         if (void 0 === n) {
                             let s = 0;
-                            t && (s |= 1), i && (s |= 2), n = this._measure(e, s), this._holey.set(r, n)
+                            t && (s |= 1), i && (s |= 2), n = this._measure(e, s), n > 0 && this._holey.set(r, n)
                         }
                         return n
                     }
                     _measure(e, t) {
                         const i = this._measureElements[t];
                         return i.textContent = e.repeat(32), i.offsetWidth / 32
                     }
@@ -1859,22 +1916,30 @@
                 const s = i(6114);
                 t.INVERTED_DEFAULT_COLOR = 257, t.DIM_OPACITY = .5, t.TEXT_BASELINE = s.isFirefox || s.isLegacyEdge ? "bottom" : "ideographic"
             },
             6171: (e, t) => {
                 function i(e) {
                     return 57508 <= e && e <= 57558
                 }
+
+                function s(e) {
+                    return e >= 128512 && e <= 128591 || e >= 127744 && e <= 128511 || e >= 128640 && e <= 128767 || e >= 9728 && e <= 9983 || e >= 9984 && e <= 10175 || e >= 65024 && e <= 65039 || e >= 129280 && e <= 129535 || e >= 127462 && e <= 127487
+                }
                 Object.defineProperty(t, "__esModule", {
                     value: !0
-                }), t.createRenderDimensions = t.excludeFromContrastRatioDemands = t.isRestrictedPowerlineGlyph = t.isPowerlineGlyph = t.throwIfFalsy = void 0, t.throwIfFalsy = function(e) {
+                }), t.computeNextVariantOffset = t.createRenderDimensions = t.treatGlyphAsBackgroundColor = t.allowRescaling = t.isEmoji = t.isRestrictedPowerlineGlyph = t.isPowerlineGlyph = t.throwIfFalsy = void 0, t.throwIfFalsy = function(e) {
                     if (!e) throw new Error("value must not be falsy");
                     return e
                 }, t.isPowerlineGlyph = i, t.isRestrictedPowerlineGlyph = function(e) {
                     return 57520 <= e && e <= 57527
-                }, t.excludeFromContrastRatioDemands = function(e) {
+                }, t.isEmoji = s, t.allowRescaling = function(e, t, r, n) {
+                    return 1 === t && r > Math.ceil(1.5 * n) && void 0 !== e && e > 255 && !s(e) && !i(e) && ! function(e) {
+                        return 57344 <= e && e <= 63743
+                    }(e)
+                }, t.treatGlyphAsBackgroundColor = function(e) {
                     return i(e) || function(e) {
                         return 9472 <= e && e <= 9631
                     }(e)
                 }, t.createRenderDimensions = function() {
                     return {
                         css: {
                             canvas: {
@@ -1899,14 +1964,44 @@
                                 width: 0,
                                 height: 0,
                                 left: 0,
                                 top: 0
                             }
                         }
                     }
+                }, t.computeNextVariantOffset = function(e, t, i = 0) {
+                    return (e - (2 * Math.round(t) - i)) % (2 * Math.round(t))
+                }
+            },
+            6052: (e, t) => {
+                Object.defineProperty(t, "__esModule", {
+                    value: !0
+                }), t.createSelectionRenderModel = void 0;
+                class i {
+                    constructor() {
+                        this.clear()
+                    }
+                    clear() {
+                        this.hasSelection = !1, this.columnSelectMode = !1, this.viewportStartRow = 0, this.viewportEndRow = 0, this.viewportCappedStartRow = 0, this.viewportCappedEndRow = 0, this.startCol = 0, this.endCol = 0, this.selectionStart = void 0, this.selectionEnd = void 0
+                    }
+                    update(e, t, i, s = !1) {
+                        if (this.selectionStart = t, this.selectionEnd = i, !t || !i || t[0] === i[0] && t[1] === i[1]) return void this.clear();
+                        const r = e.buffers.active.ydisp,
+                            n = t[1] - r,
+                            o = i[1] - r,
+                            a = Math.max(n, 0),
+                            h = Math.min(o, e.rows - 1);
+                        a >= e.rows || h < 0 ? this.clear() : (this.hasSelection = !0, this.columnSelectMode = s, this.viewportStartRow = n, this.viewportEndRow = o, this.viewportCappedStartRow = a, this.viewportCappedEndRow = h, this.startCol = t[0], this.endCol = i[0])
+                    }
+                    isCellSelected(e, t, i) {
+                        return !!this.hasSelection && (i -= e.buffer.active.viewportY, this.columnSelectMode ? this.startCol <= this.endCol ? t >= this.startCol && i >= this.viewportCappedStartRow && t < this.endCol && i <= this.viewportCappedEndRow : t < this.startCol && i >= this.viewportCappedStartRow && t >= this.endCol && i <= this.viewportCappedEndRow : i > this.viewportStartRow && i < this.viewportEndRow || this.viewportStartRow === this.viewportEndRow && i === this.viewportStartRow && t >= this.startCol && t < this.endCol || this.viewportStartRow < this.viewportEndRow && i === this.viewportEndRow && t < this.endCol || this.viewportStartRow < this.viewportEndRow && i === this.viewportStartRow && t >= this.startCol)
+                    }
+                }
+                t.createSelectionRenderModel = function() {
+                    return new i
                 }
             },
             456: (e, t) => {
                 Object.defineProperty(t, "__esModule", {
                     value: !0
                 }), t.SelectionModel = void 0, t.SelectionModel = class {
                     constructor(e) {
@@ -1963,36 +2058,57 @@
                     o = i(8460),
                     a = i(844);
                 let h = t.CharSizeService = class extends a.Disposable {
                     get hasValidSize() {
                         return this.width > 0 && this.height > 0
                     }
                     constructor(e, t, i) {
-                        super(), this._optionsService = i, this.width = 0, this.height = 0, this._onCharSizeChange = this.register(new o.EventEmitter), this.onCharSizeChange = this._onCharSizeChange.event, this._measureStrategy = new c(e, t, this._optionsService), this.register(this._optionsService.onMultipleOptionChange(["fontFamily", "fontSize"], (() => this.measure())))
+                        super(), this._optionsService = i, this.width = 0, this.height = 0, this._onCharSizeChange = this.register(new o.EventEmitter), this.onCharSizeChange = this._onCharSizeChange.event;
+                        try {
+                            this._measureStrategy = this.register(new d(this._optionsService))
+                        } catch {
+                            this._measureStrategy = this.register(new l(e, t, this._optionsService))
+                        }
+                        this.register(this._optionsService.onMultipleOptionChange(["fontFamily", "fontSize"], (() => this.measure())))
                     }
                     measure() {
                         const e = this._measureStrategy.measure();
                         e.width === this.width && e.height === this.height || (this.width = e.width, this.height = e.height, this._onCharSizeChange.fire())
                     }
                 };
                 t.CharSizeService = h = s([r(2, n.IOptionsService)], h);
-                class c {
-                    constructor(e, t, i) {
-                        this._document = e, this._parentElement = t, this._optionsService = i, this._result = {
+                class c extends a.Disposable {
+                    constructor() {
+                        super(...arguments), this._result = {
                             width: 0,
                             height: 0
-                        }, this._measureElement = this._document.createElement("span"), this._measureElement.classList.add("xterm-char-measure-element"), this._measureElement.textContent = "W".repeat(32), this._measureElement.setAttribute("aria-hidden", "true"), this._measureElement.style.whiteSpace = "pre", this._measureElement.style.fontKerning = "none", this._parentElement.appendChild(this._measureElement)
+                        }
+                    }
+                    _validateAndSet(e, t) {
+                        void 0 !== e && e > 0 && void 0 !== t && t > 0 && (this._result.width = e, this._result.height = t)
+                    }
+                }
+                class l extends c {
+                    constructor(e, t, i) {
+                        super(), this._document = e, this._parentElement = t, this._optionsService = i, this._measureElement = this._document.createElement("span"), this._measureElement.classList.add("xterm-char-measure-element"), this._measureElement.textContent = "W".repeat(32), this._measureElement.setAttribute("aria-hidden", "true"), this._measureElement.style.whiteSpace = "pre", this._measureElement.style.fontKerning = "none", this._parentElement.appendChild(this._measureElement)
                     }
                     measure() {
-                        this._measureElement.style.fontFamily = this._optionsService.rawOptions.fontFamily, this._measureElement.style.fontSize = `${this._optionsService.rawOptions.fontSize}px`;
-                        const e = {
-                            height: Number(this._measureElement.offsetHeight),
-                            width: Number(this._measureElement.offsetWidth)
-                        };
-                        return 0 !== e.width && 0 !== e.height && (this._result.width = e.width / 32, this._result.height = Math.ceil(e.height)), this._result
+                        return this._measureElement.style.fontFamily = this._optionsService.rawOptions.fontFamily, this._measureElement.style.fontSize = `${this._optionsService.rawOptions.fontSize}px`, this._validateAndSet(Number(this._measureElement.offsetWidth) / 32, Number(this._measureElement.offsetHeight)), this._result
+                    }
+                }
+                class d extends c {
+                    constructor(e) {
+                        super(), this._optionsService = e, this._canvas = new OffscreenCanvas(100, 100), this._ctx = this._canvas.getContext("2d");
+                        const t = this._ctx.measureText("W");
+                        if (!("width" in t && "fontBoundingBoxAscent" in t && "fontBoundingBoxDescent" in t)) throw new Error("Required font metrics not supported")
+                    }
+                    measure() {
+                        this._ctx.font = `${this._optionsService.rawOptions.fontSize}px ${this._optionsService.rawOptions.fontFamily}`;
+                        const e = this._ctx.measureText("W");
+                        return this._validateAndSet(e.width, e.fontBoundingBoxAscent + e.fontBoundingBoxDescent), this._result
                     }
                 }
             },
             4269: function(e, t, i) {
                 var s = this && this.__decorate || function(e, t, i, s) {
                         var r, n = arguments.length,
                             o = n < 3 ? t : null === s ? s = Object.getOwnPropertyDescriptor(t, i) : s;
@@ -2177,14 +2293,33 @@
                         this._outerListener && (this._resolutionMediaMatchList?.removeListener(this._outerListener), this._currentDevicePixelRatio = this._parentWindow.devicePixelRatio, this._resolutionMediaMatchList = this._parentWindow.matchMedia(`screen and (resolution: ${this._parentWindow.devicePixelRatio}dppx)`), this._resolutionMediaMatchList.addListener(this._outerListener))
                     }
                     clearListener() {
                         this._resolutionMediaMatchList && this._outerListener && (this._resolutionMediaMatchList.removeListener(this._outerListener), this._resolutionMediaMatchList = void 0, this._outerListener = void 0)
                     }
                 }
             },
+            779: (e, t, i) => {
+                Object.defineProperty(t, "__esModule", {
+                    value: !0
+                }), t.LinkProviderService = void 0;
+                const s = i(844);
+                class r extends s.Disposable {
+                    constructor() {
+                        super(), this.linkProviders = [], this.register((0, s.toDisposable)((() => this.linkProviders.length = 0)))
+                    }
+                    registerLinkProvider(e) {
+                        return this.linkProviders.push(e), {
+                            dispose: () => {
+                                const t = this.linkProviders.indexOf(e); - 1 !== t && this.linkProviders.splice(t, 1)
+                            }
+                        }
+                    }
+                }
+                t.LinkProviderService = r
+            },
             8934: function(e, t, i) {
                 var s = this && this.__decorate || function(e, t, i, s) {
                         var r, n = arguments.length,
                             o = n < 3 ? t : null === s ? s = Object.getOwnPropertyDescriptor(t, i) : s;
                         if ("object" == typeof Reflect && "function" == typeof Reflect.decorate) o = Reflect.decorate(e, t, i, s);
                         else
                             for (var a = e.length - 1; a >= 0; a--)(r = e[a]) && (o = (n < 3 ? r(o) : n > 3 ? r(t, i, o) : r(t, i)) || o);
@@ -2242,28 +2377,29 @@
                     h = i(844),
                     c = i(7226),
                     l = i(2585);
                 let d = t.RenderService = class extends h.Disposable {
                     get dimensions() {
                         return this._renderer.value.dimensions
                     }
-                    constructor(e, t, i, s, r, o, l, d, _) {
-                        if (super(), this._rowCount = e, this._charSizeService = s, this._renderer = this.register(new h.MutableDisposable), this._pausedResizeTask = new c.DebouncedIdleTask, this._isPaused = !1, this._needsFullRefresh = !1, this._isNextRenderRedrawOnly = !0, this._needsSelectionRefresh = !1, this._canvasWidth = 0, this._canvasHeight = 0, this._selectionState = {
-                                start: void 0,
-                                end: void 0,
-                                columnSelectMode: !1
-                            }, this._onDimensionsChange = this.register(new a.EventEmitter), this.onDimensionsChange = this._onDimensionsChange.event, this._onRenderedViewportChange = this.register(new a.EventEmitter), this.onRenderedViewportChange = this._onRenderedViewportChange.event, this._onRender = this.register(new a.EventEmitter), this.onRender = this._onRender.event, this._onRefreshRequest = this.register(new a.EventEmitter), this.onRefreshRequest = this._onRefreshRequest.event, this._renderDebouncer = new n.RenderDebouncer(l.window, ((e, t) => this._renderRows(e, t))), this.register(this._renderDebouncer), this.register(l.onDprChange((() => this.handleDevicePixelRatioChange()))), this.register(o.onResize((() => this._fullRefresh()))), this.register(o.buffers.onBufferActivate((() => this._renderer.value?.clear()))), this.register(i.onOptionChange((() => this._handleOptionsChanged()))), this.register(this._charSizeService.onCharSizeChange((() => this.handleCharSizeChanged()))), this.register(r.onDecorationRegistered((() => this._fullRefresh()))), this.register(r.onDecorationRemoved((() => this._fullRefresh()))), this.register(i.onMultipleOptionChange(["customGlyphs", "drawBoldTextInBrightColors", "letterSpacing", "lineHeight", "fontFamily", "fontSize", "fontWeight", "fontWeightBold", "minimumContrastRatio"], (() => {
-                                this.clear(), this.handleResize(o.cols, o.rows), this._fullRefresh()
-                            }))), this.register(i.onMultipleOptionChange(["cursorBlink", "cursorStyle"], (() => this.refreshRows(o.buffer.y, o.buffer.y, !0)))), this.register(_.onChangeColors((() => this._fullRefresh()))), "IntersectionObserver" in l.window) {
-                            const e = new l.window.IntersectionObserver((e => this._handleIntersectionChange(e[e.length - 1])), {
+                    constructor(e, t, i, s, r, o, l, d) {
+                        super(), this._rowCount = e, this._charSizeService = s, this._renderer = this.register(new h.MutableDisposable), this._pausedResizeTask = new c.DebouncedIdleTask, this._observerDisposable = this.register(new h.MutableDisposable), this._isPaused = !1, this._needsFullRefresh = !1, this._isNextRenderRedrawOnly = !0, this._needsSelectionRefresh = !1, this._canvasWidth = 0, this._canvasHeight = 0, this._selectionState = {
+                            start: void 0,
+                            end: void 0,
+                            columnSelectMode: !1
+                        }, this._onDimensionsChange = this.register(new a.EventEmitter), this.onDimensionsChange = this._onDimensionsChange.event, this._onRenderedViewportChange = this.register(new a.EventEmitter), this.onRenderedViewportChange = this._onRenderedViewportChange.event, this._onRender = this.register(new a.EventEmitter), this.onRender = this._onRender.event, this._onRefreshRequest = this.register(new a.EventEmitter), this.onRefreshRequest = this._onRefreshRequest.event, this._renderDebouncer = new n.RenderDebouncer(((e, t) => this._renderRows(e, t)), l), this.register(this._renderDebouncer), this.register(l.onDprChange((() => this.handleDevicePixelRatioChange()))), this.register(o.onResize((() => this._fullRefresh()))), this.register(o.buffers.onBufferActivate((() => this._renderer.value?.clear()))), this.register(i.onOptionChange((() => this._handleOptionsChanged()))), this.register(this._charSizeService.onCharSizeChange((() => this.handleCharSizeChanged()))), this.register(r.onDecorationRegistered((() => this._fullRefresh()))), this.register(r.onDecorationRemoved((() => this._fullRefresh()))), this.register(i.onMultipleOptionChange(["customGlyphs", "drawBoldTextInBrightColors", "letterSpacing", "lineHeight", "fontFamily", "fontSize", "fontWeight", "fontWeightBold", "minimumContrastRatio", "rescaleOverlappingGlyphs"], (() => {
+                            this.clear(), this.handleResize(o.cols, o.rows), this._fullRefresh()
+                        }))), this.register(i.onMultipleOptionChange(["cursorBlink", "cursorStyle"], (() => this.refreshRows(o.buffer.y, o.buffer.y, !0)))), this.register(d.onChangeColors((() => this._fullRefresh()))), this._registerIntersectionObserver(l.window, t), this.register(l.onWindowChange((e => this._registerIntersectionObserver(e, t))))
+                    }
+                    _registerIntersectionObserver(e, t) {
+                        if ("IntersectionObserver" in e) {
+                            const i = new e.IntersectionObserver((e => this._handleIntersectionChange(e[e.length - 1])), {
                                 threshold: 0
                             });
-                            e.observe(t), this.register({
-                                dispose: () => e.disconnect()
-                            })
+                            i.observe(t), this._observerDisposable.value = (0, h.toDisposable)((() => i.disconnect()))
                         }
                     }
                     _handleIntersectionChange(e) {
                         this._isPaused = void 0 === e.isIntersecting ? 0 === e.intersectionRatio : !e.isIntersecting, this._isPaused || this._charSizeService.hasValidSize || this._charSizeService.measure(), !this._isPaused && this._needsFullRefresh && (this._pausedResizeTask.flush(), this.refreshRows(0, this._rowCount - 1), this._needsFullRefresh = !1)
                     }
                     refreshRows(e, t, i = !1) {
                         this._isPaused ? this._needsFullRefresh = !0 : (i || (this._isNextRenderRedrawOnly = !1), this._renderDebouncer.refresh(e, t, this._rowCount))
@@ -2301,15 +2437,15 @@
                     clearTextureAtlas() {
                         this._renderer.value && (this._renderer.value.clearTextureAtlas?.(), this._fullRefresh())
                     }
                     handleDevicePixelRatioChange() {
                         this._charSizeService.measure(), this._renderer.value && (this._renderer.value.handleDevicePixelRatioChange(), this.refreshRows(0, this._rowCount - 1))
                     }
                     handleResize(e, t) {
-                        this._renderer.value && (this._isPaused ? this._pausedResizeTask.set((() => this._renderer.value.handleResize(e, t))) : this._renderer.value.handleResize(e, t), this._fullRefresh())
+                        this._renderer.value && (this._isPaused ? this._pausedResizeTask.set((() => this._renderer.value?.handleResize(e, t))) : this._renderer.value.handleResize(e, t), this._fullRefresh())
                     }
                     handleCharSizeChanged() {
                         this._renderer.value?.handleCharSizeChanged()
                     }
                     handleBlur() {
                         this._renderer.value?.handleBlur()
                     }
@@ -2322,15 +2458,15 @@
                     handleCursorMove() {
                         this._renderer.value?.handleCursorMove()
                     }
                     clear() {
                         this._renderer.value?.clear()
                     }
                 };
-                t.RenderService = d = s([r(2, l.IOptionsService), r(3, o.ICharSizeService), r(4, l.IDecorationService), r(5, l.IBufferService), r(6, o.ICoreBrowserService), r(7, l.IInstantiationService), r(8, o.IThemeService)], d)
+                t.RenderService = d = s([r(2, l.IOptionsService), r(3, o.ICharSizeService), r(4, l.IDecorationService), r(5, l.IBufferService), r(6, o.ICoreBrowserService), r(7, o.IThemeService)], d)
             },
             9312: function(e, t, i) {
                 var s = this && this.__decorate || function(e, t, i, s) {
                         var r, n = arguments.length,
                             o = n < 3 ? t : null === s ? s = Object.getOwnPropertyDescriptor(t, i) : s;
                         if ("object" == typeof Reflect && "function" == typeof Reflect.decorate) o = Reflect.decorate(e, t, i, s);
                         else
@@ -2352,16 +2488,16 @@
                     c = i(8460),
                     l = i(844),
                     d = i(6114),
                     _ = i(4841),
                     u = i(511),
                     f = i(2585),
                     v = String.fromCharCode(160),
-                    g = new RegExp(v, "g");
-                let p = t.SelectionService = class extends l.Disposable {
+                    p = new RegExp(v, "g");
+                let g = t.SelectionService = class extends l.Disposable {
                     constructor(e, t, i, s, r, n, o, h, d) {
                         super(), this._element = e, this._screenElement = t, this._linkifier = i, this._bufferService = s, this._coreService = r, this._mouseService = n, this._optionsService = o, this._renderService = h, this._coreBrowserService = d, this._dragScrollAmount = 0, this._enabled = !0, this._workCell = new u.CellData, this._mouseDownTimeStamp = 0, this._oldHasSelection = !1, this._oldSelectionStart = void 0, this._oldSelectionEnd = void 0, this._onLinuxMouseSelection = this.register(new c.EventEmitter), this.onLinuxMouseSelection = this._onLinuxMouseSelection.event, this._onRedrawRequest = this.register(new c.EventEmitter), this.onRequestRedraw = this._onRedrawRequest.event, this._onSelectionChange = this.register(new c.EventEmitter), this.onSelectionChange = this._onSelectionChange.event, this._onRequestScrollLines = this.register(new c.EventEmitter), this.onRequestScrollLines = this._onRequestScrollLines.event, this._mouseMoveListener = e => this._handleMouseMove(e), this._mouseUpListener = e => this._handleMouseUp(e), this._coreService.onUserInput((() => {
                             this.hasSelection && this.clearSelection()
                         })), this._trimListener = this._bufferService.buffer.lines.onTrim((e => this._handleTrim(e))), this.register(this._bufferService.buffers.onBufferActivate((e => this._handleBufferActivate(e)))), this.enable(), this._model = new a.SelectionModel(this._bufferService), this._activeSelectionMode = 0, this.register((0, l.toDisposable)((() => {
                             this._removeMouseDownListeners()
                         })))
                     }
@@ -2409,15 +2545,15 @@
                             }
                             if (e[1] !== t[1]) {
                                 const e = i.lines.get(t[1]),
                                     r = i.translateBufferLineToString(t[1], !0, 0, t[0]);
                                 e && e.isWrapped ? s[s.length - 1] += r : s.push(r)
                             }
                         }
-                        return s.map((e => e.replace(g, " "))).join(d.isWindows ? "\r\n" : "\n")
+                        return s.map((e => e.replace(p, " "))).join(d.isWindows ? "\r\n" : "\n")
                     }
                     clearSelection() {
                         this._model.clearSelection(), this._removeMouseDownListeners(), this.refresh(), this._onSelectionChange.fire()
                     }
                     refresh(e) {
                         this._refreshAnimationFrame || (this._refreshAnimationFrame = this._coreBrowserService.window.requestAnimationFrame((() => this._refresh()))), d.isLinux && e && this.selectionText.length && this._onLinuxMouseSelection.fire(this.selectionText)
                     }
@@ -2653,22 +2789,22 @@
                                     x: this._bufferService.cols - 1,
                                     y: t.last
                                 }
                             };
                         this._model.selectionStart = [0, t.first], this._model.selectionEnd = void 0, this._model.selectionStartLength = (0, _.getRangeLength)(i, this._bufferService.cols)
                     }
                 };
-                t.SelectionService = p = s([r(3, f.IBufferService), r(4, f.ICoreService), r(5, h.IMouseService), r(6, f.IOptionsService), r(7, h.IRenderService), r(8, h.ICoreBrowserService)], p)
+                t.SelectionService = g = s([r(3, f.IBufferService), r(4, f.ICoreService), r(5, h.IMouseService), r(6, f.IOptionsService), r(7, h.IRenderService), r(8, h.ICoreBrowserService)], g)
             },
             4725: (e, t, i) => {
                 Object.defineProperty(t, "__esModule", {
                     value: !0
-                }), t.IThemeService = t.ICharacterJoinerService = t.ISelectionService = t.IRenderService = t.IMouseService = t.ICoreBrowserService = t.ICharSizeService = void 0;
+                }), t.ILinkProviderService = t.IThemeService = t.ICharacterJoinerService = t.ISelectionService = t.IRenderService = t.IMouseService = t.ICoreBrowserService = t.ICharSizeService = void 0;
                 const s = i(8343);
-                t.ICharSizeService = (0, s.createDecorator)("CharSizeService"), t.ICoreBrowserService = (0, s.createDecorator)("CoreBrowserService"), t.IMouseService = (0, s.createDecorator)("MouseService"), t.IRenderService = (0, s.createDecorator)("RenderService"), t.ISelectionService = (0, s.createDecorator)("SelectionService"), t.ICharacterJoinerService = (0, s.createDecorator)("CharacterJoinerService"), t.IThemeService = (0, s.createDecorator)("ThemeService")
+                t.ICharSizeService = (0, s.createDecorator)("CharSizeService"), t.ICoreBrowserService = (0, s.createDecorator)("CoreBrowserService"), t.IMouseService = (0, s.createDecorator)("MouseService"), t.IRenderService = (0, s.createDecorator)("RenderService"), t.ISelectionService = (0, s.createDecorator)("SelectionService"), t.ICharacterJoinerService = (0, s.createDecorator)("CharacterJoinerService"), t.IThemeService = (0, s.createDecorator)("ThemeService"), t.ILinkProviderService = (0, s.createDecorator)("LinkProviderService")
             },
             6731: function(e, t, i) {
                 var s = this && this.__decorate || function(e, t, i, s) {
                         var r, n = arguments.length,
                             o = n < 3 ? t : null === s ? s = Object.getOwnPropertyDescriptor(t, i) : s;
                         if ("object" == typeof Reflect && "function" == typeof Reflect.decorate) o = Reflect.decorate(e, t, i, s);
                         else
@@ -2735,25 +2871,25 @@
                             ansi: t.DEFAULT_ANSI_COLORS.slice(),
                             contrastCache: this._contrastCache,
                             halfContrastCache: this._halfContrastCache
                         }, this._updateRestoreColors(), this._setTheme(this._optionsService.rawOptions.theme), this.register(this._optionsService.onSpecificOptionChange("minimumContrastRatio", (() => this._contrastCache.clear()))), this.register(this._optionsService.onSpecificOptionChange("theme", (() => this._setTheme(this._optionsService.rawOptions.theme))))
                     }
                     _setTheme(e = {}) {
                         const i = this._colors;
-                        if (i.foreground = g(e.foreground, l), i.background = g(e.background, d), i.cursor = g(e.cursor, _), i.cursorAccent = g(e.cursorAccent, u), i.selectionBackgroundTransparent = g(e.selectionBackground, f), i.selectionBackgroundOpaque = o.color.blend(i.background, i.selectionBackgroundTransparent), i.selectionInactiveBackgroundTransparent = g(e.selectionInactiveBackground, i.selectionBackgroundTransparent), i.selectionInactiveBackgroundOpaque = o.color.blend(i.background, i.selectionInactiveBackgroundTransparent), i.selectionForeground = e.selectionForeground ? g(e.selectionForeground, o.NULL_COLOR) : void 0, i.selectionForeground === o.NULL_COLOR && (i.selectionForeground = void 0), o.color.isOpaque(i.selectionBackgroundTransparent)) {
+                        if (i.foreground = p(e.foreground, l), i.background = p(e.background, d), i.cursor = p(e.cursor, _), i.cursorAccent = p(e.cursorAccent, u), i.selectionBackgroundTransparent = p(e.selectionBackground, f), i.selectionBackgroundOpaque = o.color.blend(i.background, i.selectionBackgroundTransparent), i.selectionInactiveBackgroundTransparent = p(e.selectionInactiveBackground, i.selectionBackgroundTransparent), i.selectionInactiveBackgroundOpaque = o.color.blend(i.background, i.selectionInactiveBackgroundTransparent), i.selectionForeground = e.selectionForeground ? p(e.selectionForeground, o.NULL_COLOR) : void 0, i.selectionForeground === o.NULL_COLOR && (i.selectionForeground = void 0), o.color.isOpaque(i.selectionBackgroundTransparent)) {
                             const e = .3;
                             i.selectionBackgroundTransparent = o.color.opacity(i.selectionBackgroundTransparent, e)
                         }
                         if (o.color.isOpaque(i.selectionInactiveBackgroundTransparent)) {
                             const e = .3;
                             i.selectionInactiveBackgroundTransparent = o.color.opacity(i.selectionInactiveBackgroundTransparent, e)
                         }
-                        if (i.ansi = t.DEFAULT_ANSI_COLORS.slice(), i.ansi[0] = g(e.black, t.DEFAULT_ANSI_COLORS[0]), i.ansi[1] = g(e.red, t.DEFAULT_ANSI_COLORS[1]), i.ansi[2] = g(e.green, t.DEFAULT_ANSI_COLORS[2]), i.ansi[3] = g(e.yellow, t.DEFAULT_ANSI_COLORS[3]), i.ansi[4] = g(e.blue, t.DEFAULT_ANSI_COLORS[4]), i.ansi[5] = g(e.magenta, t.DEFAULT_ANSI_COLORS[5]), i.ansi[6] = g(e.cyan, t.DEFAULT_ANSI_COLORS[6]), i.ansi[7] = g(e.white, t.DEFAULT_ANSI_COLORS[7]), i.ansi[8] = g(e.brightBlack, t.DEFAULT_ANSI_COLORS[8]), i.ansi[9] = g(e.brightRed, t.DEFAULT_ANSI_COLORS[9]), i.ansi[10] = g(e.brightGreen, t.DEFAULT_ANSI_COLORS[10]), i.ansi[11] = g(e.brightYellow, t.DEFAULT_ANSI_COLORS[11]), i.ansi[12] = g(e.brightBlue, t.DEFAULT_ANSI_COLORS[12]), i.ansi[13] = g(e.brightMagenta, t.DEFAULT_ANSI_COLORS[13]), i.ansi[14] = g(e.brightCyan, t.DEFAULT_ANSI_COLORS[14]), i.ansi[15] = g(e.brightWhite, t.DEFAULT_ANSI_COLORS[15]), e.extendedAnsi) {
+                        if (i.ansi = t.DEFAULT_ANSI_COLORS.slice(), i.ansi[0] = p(e.black, t.DEFAULT_ANSI_COLORS[0]), i.ansi[1] = p(e.red, t.DEFAULT_ANSI_COLORS[1]), i.ansi[2] = p(e.green, t.DEFAULT_ANSI_COLORS[2]), i.ansi[3] = p(e.yellow, t.DEFAULT_ANSI_COLORS[3]), i.ansi[4] = p(e.blue, t.DEFAULT_ANSI_COLORS[4]), i.ansi[5] = p(e.magenta, t.DEFAULT_ANSI_COLORS[5]), i.ansi[6] = p(e.cyan, t.DEFAULT_ANSI_COLORS[6]), i.ansi[7] = p(e.white, t.DEFAULT_ANSI_COLORS[7]), i.ansi[8] = p(e.brightBlack, t.DEFAULT_ANSI_COLORS[8]), i.ansi[9] = p(e.brightRed, t.DEFAULT_ANSI_COLORS[9]), i.ansi[10] = p(e.brightGreen, t.DEFAULT_ANSI_COLORS[10]), i.ansi[11] = p(e.brightYellow, t.DEFAULT_ANSI_COLORS[11]), i.ansi[12] = p(e.brightBlue, t.DEFAULT_ANSI_COLORS[12]), i.ansi[13] = p(e.brightMagenta, t.DEFAULT_ANSI_COLORS[13]), i.ansi[14] = p(e.brightCyan, t.DEFAULT_ANSI_COLORS[14]), i.ansi[15] = p(e.brightWhite, t.DEFAULT_ANSI_COLORS[15]), e.extendedAnsi) {
                             const s = Math.min(i.ansi.length - 16, e.extendedAnsi.length);
-                            for (let r = 0; r < s; r++) i.ansi[r + 16] = g(e.extendedAnsi[r], t.DEFAULT_ANSI_COLORS[r + 16])
+                            for (let r = 0; r < s; r++) i.ansi[r + 16] = p(e.extendedAnsi[r], t.DEFAULT_ANSI_COLORS[r + 16])
                         }
                         this._contrastCache.clear(), this._halfContrastCache.clear(), this._updateRestoreColors(), this._onChangeColors.fire(this.colors)
                     }
                     restoreColor(e) {
                         this._restoreColor(e), this._onChangeColors.fire(this.colors)
                     }
                     _restoreColor(e) {
@@ -2781,15 +2917,15 @@
                             background: this._colors.background,
                             cursor: this._colors.cursor,
                             ansi: this._colors.ansi.slice()
                         }
                     }
                 };
 
-                function g(e, t) {
+                function p(e, t) {
                     if (void 0 !== e) try {
                         return o.css.toColor(e)
                     } catch {}
                     return t
                 }
                 t.ThemeService = v = s([r(0, c.IOptionsService)], v)
             },
@@ -2885,184 +3021,192 @@
                 }), t.clone = void 0, t.clone = function e(t, i = 5) {
                     if ("object" != typeof t) return t;
                     const s = Array.isArray(t) ? [] : {};
                     for (const r in t) s[r] = i <= 1 ? t[r] : t[r] && e(t[r], i - 1);
                     return s
                 }
             },
-            8055: (e, t, i) => {
+            8055: (e, t) => {
                 Object.defineProperty(t, "__esModule", {
                     value: !0
                 }), t.contrastRatio = t.toPaddedHex = t.rgba = t.rgb = t.css = t.color = t.channels = t.NULL_COLOR = void 0;
-                const s = i(6114);
-                let r = 0,
-                    n = 0,
-                    o = 0,
-                    a = 0;
-                var h, c, l, d, _;
+                let i = 0,
+                    s = 0,
+                    r = 0,
+                    n = 0;
+                var o, a, h, c, l;
 
-                function u(e) {
+                function d(e) {
                     const t = e.toString(16);
                     return t.length < 2 ? "0" + t : t
                 }
 
-                function f(e, t) {
+                function _(e, t) {
                     return e < t ? (t + .05) / (e + .05) : (e + .05) / (t + .05)
                 }
                 t.NULL_COLOR = {
                         css: "#00000000",
                         rgba: 0
                     },
                     function(e) {
                         e.toCss = function(e, t, i, s) {
-                            return void 0 !== s ? `#${u(e)}${u(t)}${u(i)}${u(s)}` : `#${u(e)}${u(t)}${u(i)}`
+                            return void 0 !== s ? `#${d(e)}${d(t)}${d(i)}${d(s)}` : `#${d(e)}${d(t)}${d(i)}`
                         }, e.toRgba = function(e, t, i, s = 255) {
                             return (e << 24 | t << 16 | i << 8 | s) >>> 0
+                        }, e.toColor = function(t, i, s, r) {
+                            return {
+                                css: e.toCss(t, i, s, r),
+                                rgba: e.toRgba(t, i, s, r)
+                            }
                         }
-                    }(h || (t.channels = h = {})),
+                    }(o || (t.channels = o = {})),
                     function(e) {
                         function t(e, t) {
-                            return a = Math.round(255 * t), [r, n, o] = _.toChannels(e.rgba), {
-                                css: h.toCss(r, n, o, a),
-                                rgba: h.toRgba(r, n, o, a)
+                            return n = Math.round(255 * t), [i, s, r] = l.toChannels(e.rgba), {
+                                css: o.toCss(i, s, r, n),
+                                rgba: o.toRgba(i, s, r, n)
                             }
                         }
                         e.blend = function(e, t) {
-                            if (a = (255 & t.rgba) / 255, 1 === a) return {
+                            if (n = (255 & t.rgba) / 255, 1 === n) return {
                                 css: t.css,
                                 rgba: t.rgba
                             };
-                            const i = t.rgba >> 24 & 255,
-                                s = t.rgba >> 16 & 255,
+                            const a = t.rgba >> 24 & 255,
+                                h = t.rgba >> 16 & 255,
                                 c = t.rgba >> 8 & 255,
                                 l = e.rgba >> 24 & 255,
                                 d = e.rgba >> 16 & 255,
                                 _ = e.rgba >> 8 & 255;
-                            return r = l + Math.round((i - l) * a), n = d + Math.round((s - d) * a), o = _ + Math.round((c - _) * a), {
-                                css: h.toCss(r, n, o),
-                                rgba: h.toRgba(r, n, o)
+                            return i = l + Math.round((a - l) * n), s = d + Math.round((h - d) * n), r = _ + Math.round((c - _) * n), {
+                                css: o.toCss(i, s, r),
+                                rgba: o.toRgba(i, s, r)
                             }
                         }, e.isOpaque = function(e) {
                             return 255 == (255 & e.rgba)
                         }, e.ensureContrastRatio = function(e, t, i) {
-                            const s = _.ensureContrastRatio(e.rgba, t.rgba, i);
-                            if (s) return _.toColor(s >> 24 & 255, s >> 16 & 255, s >> 8 & 255)
+                            const s = l.ensureContrastRatio(e.rgba, t.rgba, i);
+                            if (s) return o.toColor(s >> 24 & 255, s >> 16 & 255, s >> 8 & 255)
                         }, e.opaque = function(e) {
                             const t = (255 | e.rgba) >>> 0;
-                            return [r, n, o] = _.toChannels(t), {
-                                css: h.toCss(r, n, o),
+                            return [i, s, r] = l.toChannels(t), {
+                                css: o.toCss(i, s, r),
                                 rgba: t
                             }
                         }, e.opacity = t, e.multiplyOpacity = function(e, i) {
-                            return a = 255 & e.rgba, t(e, a * i / 255)
+                            return n = 255 & e.rgba, t(e, n * i / 255)
                         }, e.toColorRGB = function(e) {
                             return [e.rgba >> 24 & 255, e.rgba >> 16 & 255, e.rgba >> 8 & 255]
                         }
-                    }(c || (t.color = c = {})),
+                    }(a || (t.color = a = {})),
                     function(e) {
-                        let t, i;
-                        if (!s.isNode) {
+                        let t, a;
+                        try {
                             const e = document.createElement("canvas");
                             e.width = 1, e.height = 1;
-                            const s = e.getContext("2d", {
+                            const i = e.getContext("2d", {
                                 willReadFrequently: !0
                             });
-                            s && (t = s, t.globalCompositeOperation = "copy", i = t.createLinearGradient(0, 0, 1, 1))
-                        }
+                            i && (t = i, t.globalCompositeOperation = "copy", a = t.createLinearGradient(0, 0, 1, 1))
+                        } catch {}
                         e.toColor = function(e) {
                             if (e.match(/#[\da-f]{3,8}/i)) switch (e.length) {
                                 case 4:
-                                    return r = parseInt(e.slice(1, 2).repeat(2), 16), n = parseInt(e.slice(2, 3).repeat(2), 16), o = parseInt(e.slice(3, 4).repeat(2), 16), _.toColor(r, n, o);
+                                    return i = parseInt(e.slice(1, 2).repeat(2), 16), s = parseInt(e.slice(2, 3).repeat(2), 16), r = parseInt(e.slice(3, 4).repeat(2), 16), o.toColor(i, s, r);
                                 case 5:
-                                    return r = parseInt(e.slice(1, 2).repeat(2), 16), n = parseInt(e.slice(2, 3).repeat(2), 16), o = parseInt(e.slice(3, 4).repeat(2), 16), a = parseInt(e.slice(4, 5).repeat(2), 16), _.toColor(r, n, o, a);
+                                    return i = parseInt(e.slice(1, 2).repeat(2), 16), s = parseInt(e.slice(2, 3).repeat(2), 16), r = parseInt(e.slice(3, 4).repeat(2), 16), n = parseInt(e.slice(4, 5).repeat(2), 16), o.toColor(i, s, r, n);
                                 case 7:
                                     return {
                                         css: e, rgba: (parseInt(e.slice(1), 16) << 8 | 255) >>> 0
                                     };
                                 case 9:
                                     return {
                                         css: e, rgba: parseInt(e.slice(1), 16) >>> 0
                                     }
                             }
-                            const s = e.match(/rgba?\(\s*(\d{1,3})\s*,\s*(\d{1,3})\s*,\s*(\d{1,3})\s*(,\s*(0|1|\d?\.(\d+))\s*)?\)/);
-                            if (s) return r = parseInt(s[1]), n = parseInt(s[2]), o = parseInt(s[3]), a = Math.round(255 * (void 0 === s[5] ? 1 : parseFloat(s[5]))), _.toColor(r, n, o, a);
-                            if (!t || !i) throw new Error("css.toColor: Unsupported css format");
-                            if (t.fillStyle = i, t.fillStyle = e, "string" != typeof t.fillStyle) throw new Error("css.toColor: Unsupported css format");
-                            if (t.fillRect(0, 0, 1, 1), [r, n, o, a] = t.getImageData(0, 0, 1, 1).data, 255 !== a) throw new Error("css.toColor: Unsupported css format");
+                            const h = e.match(/rgba?\(\s*(\d{1,3})\s*,\s*(\d{1,3})\s*,\s*(\d{1,3})\s*(,\s*(0|1|\d?\.(\d+))\s*)?\)/);
+                            if (h) return i = parseInt(h[1]), s = parseInt(h[2]), r = parseInt(h[3]), n = Math.round(255 * (void 0 === h[5] ? 1 : parseFloat(h[5]))), o.toColor(i, s, r, n);
+                            if (!t || !a) throw new Error("css.toColor: Unsupported css format");
+                            if (t.fillStyle = a, t.fillStyle = e, "string" != typeof t.fillStyle) throw new Error("css.toColor: Unsupported css format");
+                            if (t.fillRect(0, 0, 1, 1), [i, s, r, n] = t.getImageData(0, 0, 1, 1).data, 255 !== n) throw new Error("css.toColor: Unsupported css format");
                             return {
-                                rgba: h.toRgba(r, n, o, a),
+                                rgba: o.toRgba(i, s, r, n),
                                 css: e
                             }
                         }
-                    }(l || (t.css = l = {})),
+                    }(h || (t.css = h = {})),
                     function(e) {
                         function t(e, t, i) {
                             const s = e / 255,
                                 r = t / 255,
                                 n = i / 255;
                             return .2126 * (s <= .03928 ? s / 12.92 : Math.pow((s + .055) / 1.055, 2.4)) + .7152 * (r <= .03928 ? r / 12.92 : Math.pow((r + .055) / 1.055, 2.4)) + .0722 * (n <= .03928 ? n / 12.92 : Math.pow((n + .055) / 1.055, 2.4))
                         }
                         e.relativeLuminance = function(e) {
                             return t(e >> 16 & 255, e >> 8 & 255, 255 & e)
                         }, e.relativeLuminance2 = t
-                    }(d || (t.rgb = d = {})),
+                    }(c || (t.rgb = c = {})),
                     function(e) {
                         function t(e, t, i) {
                             const s = e >> 24 & 255,
                                 r = e >> 16 & 255,
                                 n = e >> 8 & 255;
                             let o = t >> 24 & 255,
                                 a = t >> 16 & 255,
                                 h = t >> 8 & 255,
-                                c = f(d.relativeLuminance2(o, a, h), d.relativeLuminance2(s, r, n));
-                            for (; c < i && (o > 0 || a > 0 || h > 0);) o -= Math.max(0, Math.ceil(.1 * o)), a -= Math.max(0, Math.ceil(.1 * a)), h -= Math.max(0, Math.ceil(.1 * h)), c = f(d.relativeLuminance2(o, a, h), d.relativeLuminance2(s, r, n));
+                                l = _(c.relativeLuminance2(o, a, h), c.relativeLuminance2(s, r, n));
+                            for (; l < i && (o > 0 || a > 0 || h > 0);) o -= Math.max(0, Math.ceil(.1 * o)), a -= Math.max(0, Math.ceil(.1 * a)), h -= Math.max(0, Math.ceil(.1 * h)), l = _(c.relativeLuminance2(o, a, h), c.relativeLuminance2(s, r, n));
                             return (o << 24 | a << 16 | h << 8 | 255) >>> 0
                         }
 
-                        function i(e, t, i) {
+                        function a(e, t, i) {
                             const s = e >> 24 & 255,
                                 r = e >> 16 & 255,
                                 n = e >> 8 & 255;
                             let o = t >> 24 & 255,
                                 a = t >> 16 & 255,
                                 h = t >> 8 & 255,
-                                c = f(d.relativeLuminance2(o, a, h), d.relativeLuminance2(s, r, n));
-                            for (; c < i && (o < 255 || a < 255 || h < 255);) o = Math.min(255, o + Math.ceil(.1 * (255 - o))), a = Math.min(255, a + Math.ceil(.1 * (255 - a))), h = Math.min(255, h + Math.ceil(.1 * (255 - h))), c = f(d.relativeLuminance2(o, a, h), d.relativeLuminance2(s, r, n));
+                                l = _(c.relativeLuminance2(o, a, h), c.relativeLuminance2(s, r, n));
+                            for (; l < i && (o < 255 || a < 255 || h < 255);) o = Math.min(255, o + Math.ceil(.1 * (255 - o))), a = Math.min(255, a + Math.ceil(.1 * (255 - a))), h = Math.min(255, h + Math.ceil(.1 * (255 - h))), l = _(c.relativeLuminance2(o, a, h), c.relativeLuminance2(s, r, n));
                             return (o << 24 | a << 16 | h << 8 | 255) >>> 0
                         }
-                        e.ensureContrastRatio = function(e, s, r) {
-                            const n = d.relativeLuminance(e >> 8),
-                                o = d.relativeLuminance(s >> 8);
-                            if (f(n, o) < r) {
-                                if (o < n) {
-                                    const o = t(e, s, r),
-                                        a = f(n, d.relativeLuminance(o >> 8));
-                                    if (a < r) {
-                                        const t = i(e, s, r);
-                                        return a > f(n, d.relativeLuminance(t >> 8)) ? o : t
+                        e.blend = function(e, t) {
+                            if (n = (255 & t) / 255, 1 === n) return t;
+                            const a = t >> 24 & 255,
+                                h = t >> 16 & 255,
+                                c = t >> 8 & 255,
+                                l = e >> 24 & 255,
+                                d = e >> 16 & 255,
+                                _ = e >> 8 & 255;
+                            return i = l + Math.round((a - l) * n), s = d + Math.round((h - d) * n), r = _ + Math.round((c - _) * n), o.toRgba(i, s, r)
+                        }, e.ensureContrastRatio = function(e, i, s) {
+                            const r = c.relativeLuminance(e >> 8),
+                                n = c.relativeLuminance(i >> 8);
+                            if (_(r, n) < s) {
+                                if (n < r) {
+                                    const n = t(e, i, s),
+                                        o = _(r, c.relativeLuminance(n >> 8));
+                                    if (o < s) {
+                                        const t = a(e, i, s);
+                                        return o > _(r, c.relativeLuminance(t >> 8)) ? n : t
                                     }
-                                    return o
+                                    return n
                                 }
-                                const a = i(e, s, r),
-                                    h = f(n, d.relativeLuminance(a >> 8));
-                                if (h < r) {
-                                    const i = t(e, s, r);
-                                    return h > f(n, d.relativeLuminance(i >> 8)) ? a : i
+                                const o = a(e, i, s),
+                                    h = _(r, c.relativeLuminance(o >> 8));
+                                if (h < s) {
+                                    const n = t(e, i, s);
+                                    return h > _(r, c.relativeLuminance(n >> 8)) ? o : n
                                 }
-                                return a
+                                return o
                             }
-                        }, e.reduceLuminance = t, e.increaseLuminance = i, e.toChannels = function(e) {
+                        }, e.reduceLuminance = t, e.increaseLuminance = a, e.toChannels = function(e) {
                             return [e >> 24 & 255, e >> 16 & 255, e >> 8 & 255, 255 & e]
-                        }, e.toColor = function(e, t, i, s) {
-                            return {
-                                css: h.toCss(e, t, i, s),
-                                rgba: h.toRgba(e, t, i, s)
-                            }
                         }
-                    }(_ || (t.rgba = _ = {})), t.toPaddedHex = u, t.contrastRatio = f
+                    }(l || (t.rgba = l = {})), t.toPaddedHex = d, t.contrastRatio = _
             },
             8969: (e, t, i) => {
                 Object.defineProperty(t, "__esModule", {
                     value: !0
                 }), t.CoreTerminal = void 0;
                 const s = i(844),
                     r = i(2585),
@@ -3073,16 +3217,16 @@
                     c = i(6975),
                     l = i(8460),
                     d = i(1753),
                     _ = i(1480),
                     u = i(7994),
                     f = i(9282),
                     v = i(5435),
-                    g = i(5981),
-                    p = i(2660);
+                    p = i(5981),
+                    g = i(2660);
                 let m = !1;
                 class S extends s.Disposable {
                     get onScroll() {
                         return this._onScrollApi || (this._onScrollApi = this.register(new l.EventEmitter), this._onScroll.event((e => {
                             this._onScrollApi?.fire(e.position)
                         }))), this._onScrollApi.event
                     }
@@ -3098,32 +3242,35 @@
                     get options() {
                         return this.optionsService.options
                     }
                     set options(e) {
                         for (const t in e) this.optionsService.options[t] = e[t]
                     }
                     constructor(e) {
-                        super(), this._windowsWrappingHeuristics = this.register(new s.MutableDisposable), this._onBinary = this.register(new l.EventEmitter), this.onBinary = this._onBinary.event, this._onData = this.register(new l.EventEmitter), this.onData = this._onData.event, this._onLineFeed = this.register(new l.EventEmitter), this.onLineFeed = this._onLineFeed.event, this._onResize = this.register(new l.EventEmitter), this.onResize = this._onResize.event, this._onWriteParsed = this.register(new l.EventEmitter), this.onWriteParsed = this._onWriteParsed.event, this._onScroll = this.register(new l.EventEmitter), this._instantiationService = new n.InstantiationService, this.optionsService = this.register(new h.OptionsService(e)), this._instantiationService.setService(r.IOptionsService, this.optionsService), this._bufferService = this.register(this._instantiationService.createInstance(a.BufferService)), this._instantiationService.setService(r.IBufferService, this._bufferService), this._logService = this.register(this._instantiationService.createInstance(o.LogService)), this._instantiationService.setService(r.ILogService, this._logService), this.coreService = this.register(this._instantiationService.createInstance(c.CoreService)), this._instantiationService.setService(r.ICoreService, this.coreService), this.coreMouseService = this.register(this._instantiationService.createInstance(d.CoreMouseService)), this._instantiationService.setService(r.ICoreMouseService, this.coreMouseService), this.unicodeService = this.register(this._instantiationService.createInstance(_.UnicodeService)), this._instantiationService.setService(r.IUnicodeService, this.unicodeService), this._charsetService = this._instantiationService.createInstance(u.CharsetService), this._instantiationService.setService(r.ICharsetService, this._charsetService), this._oscLinkService = this._instantiationService.createInstance(p.OscLinkService), this._instantiationService.setService(r.IOscLinkService, this._oscLinkService), this._inputHandler = this.register(new v.InputHandler(this._bufferService, this._charsetService, this.coreService, this._logService, this.optionsService, this._oscLinkService, this.coreMouseService, this.unicodeService)), this.register((0, l.forwardEvent)(this._inputHandler.onLineFeed, this._onLineFeed)), this.register(this._inputHandler), this.register((0, l.forwardEvent)(this._bufferService.onResize, this._onResize)), this.register((0, l.forwardEvent)(this.coreService.onData, this._onData)), this.register((0, l.forwardEvent)(this.coreService.onBinary, this._onBinary)), this.register(this.coreService.onRequestScrollToBottom((() => this.scrollToBottom()))), this.register(this.coreService.onUserInput((() => this._writeBuffer.handleUserInput()))), this.register(this.optionsService.onMultipleOptionChange(["windowsMode", "windowsPty"], (() => this._handleWindowsPtyOptionChange()))), this.register(this._bufferService.onScroll((e => {
+                        super(), this._windowsWrappingHeuristics = this.register(new s.MutableDisposable), this._onBinary = this.register(new l.EventEmitter), this.onBinary = this._onBinary.event, this._onData = this.register(new l.EventEmitter), this.onData = this._onData.event, this._onLineFeed = this.register(new l.EventEmitter), this.onLineFeed = this._onLineFeed.event, this._onResize = this.register(new l.EventEmitter), this.onResize = this._onResize.event, this._onWriteParsed = this.register(new l.EventEmitter), this.onWriteParsed = this._onWriteParsed.event, this._onScroll = this.register(new l.EventEmitter), this._instantiationService = new n.InstantiationService, this.optionsService = this.register(new h.OptionsService(e)), this._instantiationService.setService(r.IOptionsService, this.optionsService), this._bufferService = this.register(this._instantiationService.createInstance(a.BufferService)), this._instantiationService.setService(r.IBufferService, this._bufferService), this._logService = this.register(this._instantiationService.createInstance(o.LogService)), this._instantiationService.setService(r.ILogService, this._logService), this.coreService = this.register(this._instantiationService.createInstance(c.CoreService)), this._instantiationService.setService(r.ICoreService, this.coreService), this.coreMouseService = this.register(this._instantiationService.createInstance(d.CoreMouseService)), this._instantiationService.setService(r.ICoreMouseService, this.coreMouseService), this.unicodeService = this.register(this._instantiationService.createInstance(_.UnicodeService)), this._instantiationService.setService(r.IUnicodeService, this.unicodeService), this._charsetService = this._instantiationService.createInstance(u.CharsetService), this._instantiationService.setService(r.ICharsetService, this._charsetService), this._oscLinkService = this._instantiationService.createInstance(g.OscLinkService), this._instantiationService.setService(r.IOscLinkService, this._oscLinkService), this._inputHandler = this.register(new v.InputHandler(this._bufferService, this._charsetService, this.coreService, this._logService, this.optionsService, this._oscLinkService, this.coreMouseService, this.unicodeService)), this.register((0, l.forwardEvent)(this._inputHandler.onLineFeed, this._onLineFeed)), this.register(this._inputHandler), this.register((0, l.forwardEvent)(this._bufferService.onResize, this._onResize)), this.register((0, l.forwardEvent)(this.coreService.onData, this._onData)), this.register((0, l.forwardEvent)(this.coreService.onBinary, this._onBinary)), this.register(this.coreService.onRequestScrollToBottom((() => this.scrollToBottom()))), this.register(this.coreService.onUserInput((() => this._writeBuffer.handleUserInput()))), this.register(this.optionsService.onMultipleOptionChange(["windowsMode", "windowsPty"], (() => this._handleWindowsPtyOptionChange()))), this.register(this._bufferService.onScroll((e => {
                             this._onScroll.fire({
                                 position: this._bufferService.buffer.ydisp,
                                 source: 0
                             }), this._inputHandler.markRangeDirty(this._bufferService.buffer.scrollTop, this._bufferService.buffer.scrollBottom)
                         }))), this.register(this._inputHandler.onScroll((e => {
                             this._onScroll.fire({
                                 position: this._bufferService.buffer.ydisp,
                                 source: 0
                             }), this._inputHandler.markRangeDirty(this._bufferService.buffer.scrollTop, this._bufferService.buffer.scrollBottom)
-                        }))), this._writeBuffer = this.register(new g.WriteBuffer(((e, t) => this._inputHandler.parse(e, t)))), this.register((0, l.forwardEvent)(this._writeBuffer.onWriteParsed, this._onWriteParsed))
+                        }))), this._writeBuffer = this.register(new p.WriteBuffer(((e, t) => this._inputHandler.parse(e, t)))), this.register((0, l.forwardEvent)(this._writeBuffer.onWriteParsed, this._onWriteParsed))
                     }
                     write(e, t) {
                         this._writeBuffer.write(e, t)
                     }
                     writeSync(e, t) {
                         this._logService.logLevel <= r.LogLevelEnum.WARN && !m && (this._logService.warn("writeSync is unreliable and will be removed soon."), m = !0), this._writeBuffer.writeSync(e, t)
                     }
+                    input(e, t = !0) {
+                        this.coreService.triggerDataEvent(e, t)
+                    }
                     resize(e, t) {
                         isNaN(e) || isNaN(t) || (e = Math.max(e, a.MINIMUM_COLS), t = Math.max(t, a.MINIMUM_ROWS), this._bufferService.resize(e, t))
                     }
                     scroll(e, t = !1) {
                         this._bufferService.scroll(e, t)
                     }
                     scrollLines(e, t, i) {
@@ -3235,29 +3382,29 @@
                     c = i(482),
                     l = i(8437),
                     d = i(8460),
                     _ = i(643),
                     u = i(511),
                     f = i(3734),
                     v = i(2585),
-                    g = i(1480),
-                    p = i(6242),
+                    p = i(1480),
+                    g = i(6242),
                     m = i(6351),
                     S = i(5941),
                     C = {
                         "(": 0,
                         ")": 1,
                         "*": 2,
                         "+": 3,
                         "-": 1,
                         ".": 2
                     },
                     b = 131072;
 
-                function y(e, t) {
+                function w(e, t) {
                     if (e > 24) return t.setWinLines || !1;
                     switch (e) {
                         case 1:
                             return !!t.restoreWin;
                         case 2:
                             return !!t.minimizeWin;
                         case 3:
@@ -3299,18 +3446,18 @@
                         case 23:
                             return !!t.popTitle;
                         case 24:
                             return !!t.setWinLines
                     }
                     return !1
                 }
-                var w;
+                var y;
                 ! function(e) {
                     e[e.GET_WIN_SIZE_PIXELS = 0] = "GET_WIN_SIZE_PIXELS", e[e.GET_CELL_SIZE_PIXELS = 1] = "GET_CELL_SIZE_PIXELS"
-                }(w || (t.WindowsOptionsReportType = w = {}));
+                }(y || (t.WindowsOptionsReportType = y = {}));
                 let E = 0;
                 class k extends h.Disposable {
                     getAttrData() {
                         return this._curAttrData
                     }
                     constructor(e, t, i, s, r, h, _, f, v = new a.EscapeSequenceParser) {
                         super(), this._bufferService = e, this._charsetService = t, this._coreService = i, this._logService = s, this._optionsService = r, this._oscLinkService = h, this._coreMouseService = _, this._unicodeService = f, this._parser = v, this._parseBuffer = new Uint32Array(4096), this._stringDecoder = new c.StringToUtf32, this._utf8Decoder = new c.Utf8ToUtf32, this._workCell = new u.CellData, this._windowTitle = "", this._iconName = "", this._windowTitleStack = [], this._iconNameStack = [], this._curAttrData = l.DEFAULT_ATTR_DATA.clone(), this._eraseAttrDataInternal = l.DEFAULT_ATTR_DATA.clone(), this._onRequestBell = this.register(new d.EventEmitter), this.onRequestBell = this._onRequestBell.event, this._onRequestRefreshRows = this.register(new d.EventEmitter), this.onRequestRefreshRows = this._onRequestRefreshRows.event, this._onRequestReset = this.register(new d.EventEmitter), this.onRequestReset = this._onRequestReset.event, this._onRequestSendFocus = this.register(new d.EventEmitter), this.onRequestSendFocus = this._onRequestSendFocus.event, this._onRequestSyncScrollBar = this.register(new d.EventEmitter), this.onRequestSyncScrollBar = this._onRequestSyncScrollBar.event, this._onRequestWindowsOptionsReport = this.register(new d.EventEmitter), this.onRequestWindowsOptionsReport = this._onRequestWindowsOptionsReport.event, this._onA11yChar = this.register(new d.EventEmitter), this.onA11yChar = this._onA11yChar.event, this._onA11yTab = this.register(new d.EventEmitter), this.onA11yTab = this._onA11yTab.event, this._onCursorMove = this.register(new d.EventEmitter), this.onCursorMove = this._onCursorMove.event, this._onLineFeed = this.register(new d.EventEmitter), this.onLineFeed = this._onLineFeed.event, this._onScroll = this.register(new d.EventEmitter), this.onScroll = this._onScroll.event, this._onTitleChange = this.register(new d.EventEmitter), this.onTitleChange = this._onTitleChange.event, this._onColor = this.register(new d.EventEmitter), this.onColor = this._onColor.event, this._parseStack = {
@@ -3456,15 +3603,15 @@
                         }, (e => this.selectProtected(e))), this._parser.registerCsiHandler({
                             intermediates: "$",
                             final: "p"
                         }, (e => this.requestMode(e, !0))), this._parser.registerCsiHandler({
                             prefix: "?",
                             intermediates: "$",
                             final: "p"
-                        }, (e => this.requestMode(e, !1))), this._parser.setExecuteHandler(n.C0.BEL, (() => this.bell())), this._parser.setExecuteHandler(n.C0.LF, (() => this.lineFeed())), this._parser.setExecuteHandler(n.C0.VT, (() => this.lineFeed())), this._parser.setExecuteHandler(n.C0.FF, (() => this.lineFeed())), this._parser.setExecuteHandler(n.C0.CR, (() => this.carriageReturn())), this._parser.setExecuteHandler(n.C0.BS, (() => this.backspace())), this._parser.setExecuteHandler(n.C0.HT, (() => this.tab())), this._parser.setExecuteHandler(n.C0.SO, (() => this.shiftOut())), this._parser.setExecuteHandler(n.C0.SI, (() => this.shiftIn())), this._parser.setExecuteHandler(n.C1.IND, (() => this.index())), this._parser.setExecuteHandler(n.C1.NEL, (() => this.nextLine())), this._parser.setExecuteHandler(n.C1.HTS, (() => this.tabSet())), this._parser.registerOscHandler(0, new p.OscHandler((e => (this.setTitle(e), this.setIconName(e), !0)))), this._parser.registerOscHandler(1, new p.OscHandler((e => this.setIconName(e)))), this._parser.registerOscHandler(2, new p.OscHandler((e => this.setTitle(e)))), this._parser.registerOscHandler(4, new p.OscHandler((e => this.setOrReportIndexedColor(e)))), this._parser.registerOscHandler(8, new p.OscHandler((e => this.setHyperlink(e)))), this._parser.registerOscHandler(10, new p.OscHandler((e => this.setOrReportFgColor(e)))), this._parser.registerOscHandler(11, new p.OscHandler((e => this.setOrReportBgColor(e)))), this._parser.registerOscHandler(12, new p.OscHandler((e => this.setOrReportCursorColor(e)))), this._parser.registerOscHandler(104, new p.OscHandler((e => this.restoreIndexedColor(e)))), this._parser.registerOscHandler(110, new p.OscHandler((e => this.restoreFgColor(e)))), this._parser.registerOscHandler(111, new p.OscHandler((e => this.restoreBgColor(e)))), this._parser.registerOscHandler(112, new p.OscHandler((e => this.restoreCursorColor(e)))), this._parser.registerEscHandler({
+                        }, (e => this.requestMode(e, !1))), this._parser.setExecuteHandler(n.C0.BEL, (() => this.bell())), this._parser.setExecuteHandler(n.C0.LF, (() => this.lineFeed())), this._parser.setExecuteHandler(n.C0.VT, (() => this.lineFeed())), this._parser.setExecuteHandler(n.C0.FF, (() => this.lineFeed())), this._parser.setExecuteHandler(n.C0.CR, (() => this.carriageReturn())), this._parser.setExecuteHandler(n.C0.BS, (() => this.backspace())), this._parser.setExecuteHandler(n.C0.HT, (() => this.tab())), this._parser.setExecuteHandler(n.C0.SO, (() => this.shiftOut())), this._parser.setExecuteHandler(n.C0.SI, (() => this.shiftIn())), this._parser.setExecuteHandler(n.C1.IND, (() => this.index())), this._parser.setExecuteHandler(n.C1.NEL, (() => this.nextLine())), this._parser.setExecuteHandler(n.C1.HTS, (() => this.tabSet())), this._parser.registerOscHandler(0, new g.OscHandler((e => (this.setTitle(e), this.setIconName(e), !0)))), this._parser.registerOscHandler(1, new g.OscHandler((e => this.setIconName(e)))), this._parser.registerOscHandler(2, new g.OscHandler((e => this.setTitle(e)))), this._parser.registerOscHandler(4, new g.OscHandler((e => this.setOrReportIndexedColor(e)))), this._parser.registerOscHandler(8, new g.OscHandler((e => this.setHyperlink(e)))), this._parser.registerOscHandler(10, new g.OscHandler((e => this.setOrReportFgColor(e)))), this._parser.registerOscHandler(11, new g.OscHandler((e => this.setOrReportBgColor(e)))), this._parser.registerOscHandler(12, new g.OscHandler((e => this.setOrReportCursorColor(e)))), this._parser.registerOscHandler(104, new g.OscHandler((e => this.restoreIndexedColor(e)))), this._parser.registerOscHandler(110, new g.OscHandler((e => this.restoreFgColor(e)))), this._parser.registerOscHandler(111, new g.OscHandler((e => this.restoreBgColor(e)))), this._parser.registerOscHandler(112, new g.OscHandler((e => this.restoreCursorColor(e)))), this._parser.registerEscHandler({
                             final: "7"
                         }, (() => this.saveCursor())), this._parser.registerEscHandler({
                             final: "8"
                         }, (() => this.restoreCursor())), this._parser.registerEscHandler({
                             final: "D"
                         }, (() => this.index())), this._parser.registerEscHandler({
                             final: "E"
@@ -3564,51 +3711,51 @@
                         const n = this._charsetService.charset,
                             o = this._optionsService.rawOptions.screenReaderMode,
                             a = this._bufferService.cols,
                             h = this._coreService.decPrivateModes.wraparound,
                             d = this._coreService.modes.insertMode,
                             u = this._curAttrData;
                         let f = this._activeBuffer.lines.get(this._activeBuffer.ybase + this._activeBuffer.y);
-                        this._dirtyRowTracker.markDirty(this._activeBuffer.y), this._activeBuffer.x && i - t > 0 && 2 === f.getWidth(this._activeBuffer.x - 1) && f.setCellFromCodePoint(this._activeBuffer.x - 1, 0, 1, u.fg, u.bg, u.extended);
+                        this._dirtyRowTracker.markDirty(this._activeBuffer.y), this._activeBuffer.x && i - t > 0 && 2 === f.getWidth(this._activeBuffer.x - 1) && f.setCellFromCodepoint(this._activeBuffer.x - 1, 0, 1, u);
                         let v = this._parser.precedingJoinState;
-                        for (let p = t; p < i; ++p) {
-                            if (s = e[p], s < 127 && n) {
+                        for (let g = t; g < i; ++g) {
+                            if (s = e[g], s < 127 && n) {
                                 const e = n[String.fromCharCode(s)];
                                 e && (s = e.charCodeAt(0))
                             }
                             const t = this._unicodeService.charProperties(s, v);
-                            r = g.UnicodeService.extractWidth(t);
-                            const i = g.UnicodeService.extractShouldJoin(t),
-                                m = i ? g.UnicodeService.extractWidth(v) : 0;
+                            r = p.UnicodeService.extractWidth(t);
+                            const i = p.UnicodeService.extractShouldJoin(t),
+                                m = i ? p.UnicodeService.extractWidth(v) : 0;
                             if (v = t, o && this._onA11yChar.fire((0, c.stringFromCodePoint)(s)), this._getCurrentLinkId() && this._oscLinkService.addLineToLink(this._getCurrentLinkId(), this._activeBuffer.ybase + this._activeBuffer.y), this._activeBuffer.x + r - m > a)
                                 if (h) {
                                     const e = f;
                                     let t = this._activeBuffer.x - m;
-                                    for (this._activeBuffer.x = m, this._activeBuffer.y++, this._activeBuffer.y === this._activeBuffer.scrollBottom + 1 ? (this._activeBuffer.y--, this._bufferService.scroll(this._eraseAttrData(), !0)) : (this._activeBuffer.y >= this._bufferService.rows && (this._activeBuffer.y = this._bufferService.rows - 1), this._activeBuffer.lines.get(this._activeBuffer.ybase + this._activeBuffer.y).isWrapped = !0), f = this._activeBuffer.lines.get(this._activeBuffer.ybase + this._activeBuffer.y), m > 0 && f instanceof l.BufferLine && f.copyCellsFrom(e, t, 0, m, !1); t < a;) e.setCellFromCodePoint(t++, 0, 1, u.fg, u.bg, u.extended)
+                                    for (this._activeBuffer.x = m, this._activeBuffer.y++, this._activeBuffer.y === this._activeBuffer.scrollBottom + 1 ? (this._activeBuffer.y--, this._bufferService.scroll(this._eraseAttrData(), !0)) : (this._activeBuffer.y >= this._bufferService.rows && (this._activeBuffer.y = this._bufferService.rows - 1), this._activeBuffer.lines.get(this._activeBuffer.ybase + this._activeBuffer.y).isWrapped = !0), f = this._activeBuffer.lines.get(this._activeBuffer.ybase + this._activeBuffer.y), m > 0 && f instanceof l.BufferLine && f.copyCellsFrom(e, t, 0, m, !1); t < a;) e.setCellFromCodepoint(t++, 0, 1, u)
                                 } else if (this._activeBuffer.x = a - 1, 2 === r) continue;
                             if (i && this._activeBuffer.x) {
                                 const e = f.getWidth(this._activeBuffer.x - 1) ? 1 : 2;
                                 f.addCodepointToCell(this._activeBuffer.x - e, s, r);
-                                for (let e = r - m; --e >= 0;) f.setCellFromCodePoint(this._activeBuffer.x++, 0, 0, u.fg, u.bg, u.extended)
-                            } else if (d && (f.insertCells(this._activeBuffer.x, r - m, this._activeBuffer.getNullCell(u), u), 2 === f.getWidth(a - 1) && f.setCellFromCodePoint(a - 1, _.NULL_CELL_CODE, _.NULL_CELL_WIDTH, u.fg, u.bg, u.extended)), f.setCellFromCodePoint(this._activeBuffer.x++, s, r, u.fg, u.bg, u.extended), r > 0)
-                                for (; --r;) f.setCellFromCodePoint(this._activeBuffer.x++, 0, 0, u.fg, u.bg, u.extended)
+                                for (let e = r - m; --e >= 0;) f.setCellFromCodepoint(this._activeBuffer.x++, 0, 0, u)
+                            } else if (d && (f.insertCells(this._activeBuffer.x, r - m, this._activeBuffer.getNullCell(u)), 2 === f.getWidth(a - 1) && f.setCellFromCodepoint(a - 1, _.NULL_CELL_CODE, _.NULL_CELL_WIDTH, u)), f.setCellFromCodepoint(this._activeBuffer.x++, s, r, u), r > 0)
+                                for (; --r;) f.setCellFromCodepoint(this._activeBuffer.x++, 0, 0, u)
                         }
-                        this._parser.precedingJoinState = v, this._activeBuffer.x < a && i - t > 0 && 0 === f.getWidth(this._activeBuffer.x) && !f.hasContent(this._activeBuffer.x) && f.setCellFromCodePoint(this._activeBuffer.x, 0, 1, u.fg, u.bg, u.extended), this._dirtyRowTracker.markDirty(this._activeBuffer.y)
+                        this._parser.precedingJoinState = v, this._activeBuffer.x < a && i - t > 0 && 0 === f.getWidth(this._activeBuffer.x) && !f.hasContent(this._activeBuffer.x) && f.setCellFromCodepoint(this._activeBuffer.x, 0, 1, u), this._dirtyRowTracker.markDirty(this._activeBuffer.y)
                     }
                     registerCsiHandler(e, t) {
-                        return "t" !== e.final || e.prefix || e.intermediates ? this._parser.registerCsiHandler(e, t) : this._parser.registerCsiHandler(e, (e => !y(e.params[0], this._optionsService.rawOptions.windowOptions) || t(e)))
+                        return "t" !== e.final || e.prefix || e.intermediates ? this._parser.registerCsiHandler(e, t) : this._parser.registerCsiHandler(e, (e => !w(e.params[0], this._optionsService.rawOptions.windowOptions) || t(e)))
                     }
                     registerDcsHandler(e, t) {
                         return this._parser.registerDcsHandler(e, new m.DcsHandler(t))
                     }
                     registerEscHandler(e, t) {
                         return this._parser.registerEscHandler(e, t)
                     }
                     registerOscHandler(e, t) {
-                        return this._parser.registerOscHandler(e, new p.OscHandler(t))
+                        return this._parser.registerOscHandler(e, new g.OscHandler(t))
                     }
                     bell() {
                         return this._onRequestBell.fire(), !0
                     }
                     lineFeed() {
                         return this._dirtyRowTracker.markDirty(this._activeBuffer.y), this._optionsService.rawOptions.convertEol && (this._activeBuffer.x = 0), this._activeBuffer.y++, this._activeBuffer.y === this._activeBuffer.scrollBottom + 1 ? (this._activeBuffer.y--, this._bufferService.scroll(this._eraseAttrData())) : this._activeBuffer.y >= this._bufferService.rows ? this._activeBuffer.y = this._bufferService.rows - 1 : this._activeBuffer.lines.get(this._activeBuffer.ybase + this._activeBuffer.y).isWrapped = !1, this._activeBuffer.x >= this._bufferService.cols && this._activeBuffer.x--, this._dirtyRowTracker.markDirty(this._activeBuffer.y), this._onLineFeed.fire(), !0
                     }
@@ -3704,15 +3851,15 @@
                     }
                     selectProtected(e) {
                         const t = e.params[0];
                         return 1 === t && (this._curAttrData.bg |= 536870912), 2 !== t && 0 !== t || (this._curAttrData.bg &= -536870913), !0
                     }
                     _eraseInBufferLine(e, t, i, s = !1, r = !1) {
                         const n = this._activeBuffer.lines.get(this._activeBuffer.ybase + e);
-                        n.replaceCells(t, i, this._activeBuffer.getNullCell(this._eraseAttrData()), this._eraseAttrData(), r), s && (n.isWrapped = !1)
+                        n.replaceCells(t, i, this._activeBuffer.getNullCell(this._eraseAttrData()), r), s && (n.isWrapped = !1)
                     }
                     _resetBufferLine(e, t = !1) {
                         const i = this._activeBuffer.lines.get(this._activeBuffer.ybase + e);
                         i && (i.fill(this._activeBuffer.getNullCell(this._eraseAttrData()), t), this._bufferService.buffer.clearMarkers(this._activeBuffer.ybase + e), i.isWrapped = !1)
                     }
                     eraseInDisplay(e, t = !1) {
                         let i;
@@ -3766,20 +3913,20 @@
                         let s;
                         for (s = this._bufferService.rows - 1 - this._activeBuffer.scrollBottom, s = this._bufferService.rows - 1 + this._activeBuffer.ybase - s; t--;) this._activeBuffer.lines.splice(i, 1), this._activeBuffer.lines.splice(s, 0, this._activeBuffer.getBlankLine(this._eraseAttrData()));
                         return this._dirtyRowTracker.markRangeDirty(this._activeBuffer.y, this._activeBuffer.scrollBottom), this._activeBuffer.x = 0, !0
                     }
                     insertChars(e) {
                         this._restrictCursor();
                         const t = this._activeBuffer.lines.get(this._activeBuffer.ybase + this._activeBuffer.y);
-                        return t && (t.insertCells(this._activeBuffer.x, e.params[0] || 1, this._activeBuffer.getNullCell(this._eraseAttrData()), this._eraseAttrData()), this._dirtyRowTracker.markDirty(this._activeBuffer.y)), !0
+                        return t && (t.insertCells(this._activeBuffer.x, e.params[0] || 1, this._activeBuffer.getNullCell(this._eraseAttrData())), this._dirtyRowTracker.markDirty(this._activeBuffer.y)), !0
                     }
                     deleteChars(e) {
                         this._restrictCursor();
                         const t = this._activeBuffer.lines.get(this._activeBuffer.ybase + this._activeBuffer.y);
-                        return t && (t.deleteCells(this._activeBuffer.x, e.params[0] || 1, this._activeBuffer.getNullCell(this._eraseAttrData()), this._eraseAttrData()), this._dirtyRowTracker.markDirty(this._activeBuffer.y)), !0
+                        return t && (t.deleteCells(this._activeBuffer.x, e.params[0] || 1, this._activeBuffer.getNullCell(this._eraseAttrData())), this._dirtyRowTracker.markDirty(this._activeBuffer.y)), !0
                     }
                     scrollUp(e) {
                         let t = e.params[0] || 1;
                         for (; t--;) this._activeBuffer.lines.splice(this._activeBuffer.ybase + this._activeBuffer.scrollTop, 1), this._activeBuffer.lines.splice(this._activeBuffer.ybase + this._activeBuffer.scrollBottom, 0, this._activeBuffer.getBlankLine(this._eraseAttrData()));
                         return this._dirtyRowTracker.markRangeDirty(this._activeBuffer.scrollTop, this._activeBuffer.scrollBottom), !0
                     }
                     scrollDown(e) {
@@ -3788,55 +3935,55 @@
                         return this._dirtyRowTracker.markRangeDirty(this._activeBuffer.scrollTop, this._activeBuffer.scrollBottom), !0
                     }
                     scrollLeft(e) {
                         if (this._activeBuffer.y > this._activeBuffer.scrollBottom || this._activeBuffer.y < this._activeBuffer.scrollTop) return !0;
                         const t = e.params[0] || 1;
                         for (let e = this._activeBuffer.scrollTop; e <= this._activeBuffer.scrollBottom; ++e) {
                             const i = this._activeBuffer.lines.get(this._activeBuffer.ybase + e);
-                            i.deleteCells(0, t, this._activeBuffer.getNullCell(this._eraseAttrData()), this._eraseAttrData()), i.isWrapped = !1
+                            i.deleteCells(0, t, this._activeBuffer.getNullCell(this._eraseAttrData())), i.isWrapped = !1
                         }
                         return this._dirtyRowTracker.markRangeDirty(this._activeBuffer.scrollTop, this._activeBuffer.scrollBottom), !0
                     }
                     scrollRight(e) {
                         if (this._activeBuffer.y > this._activeBuffer.scrollBottom || this._activeBuffer.y < this._activeBuffer.scrollTop) return !0;
                         const t = e.params[0] || 1;
                         for (let e = this._activeBuffer.scrollTop; e <= this._activeBuffer.scrollBottom; ++e) {
                             const i = this._activeBuffer.lines.get(this._activeBuffer.ybase + e);
-                            i.insertCells(0, t, this._activeBuffer.getNullCell(this._eraseAttrData()), this._eraseAttrData()), i.isWrapped = !1
+                            i.insertCells(0, t, this._activeBuffer.getNullCell(this._eraseAttrData())), i.isWrapped = !1
                         }
                         return this._dirtyRowTracker.markRangeDirty(this._activeBuffer.scrollTop, this._activeBuffer.scrollBottom), !0
                     }
                     insertColumns(e) {
                         if (this._activeBuffer.y > this._activeBuffer.scrollBottom || this._activeBuffer.y < this._activeBuffer.scrollTop) return !0;
                         const t = e.params[0] || 1;
                         for (let e = this._activeBuffer.scrollTop; e <= this._activeBuffer.scrollBottom; ++e) {
                             const i = this._activeBuffer.lines.get(this._activeBuffer.ybase + e);
-                            i.insertCells(this._activeBuffer.x, t, this._activeBuffer.getNullCell(this._eraseAttrData()), this._eraseAttrData()), i.isWrapped = !1
+                            i.insertCells(this._activeBuffer.x, t, this._activeBuffer.getNullCell(this._eraseAttrData())), i.isWrapped = !1
                         }
                         return this._dirtyRowTracker.markRangeDirty(this._activeBuffer.scrollTop, this._activeBuffer.scrollBottom), !0
                     }
                     deleteColumns(e) {
                         if (this._activeBuffer.y > this._activeBuffer.scrollBottom || this._activeBuffer.y < this._activeBuffer.scrollTop) return !0;
                         const t = e.params[0] || 1;
                         for (let e = this._activeBuffer.scrollTop; e <= this._activeBuffer.scrollBottom; ++e) {
                             const i = this._activeBuffer.lines.get(this._activeBuffer.ybase + e);
-                            i.deleteCells(this._activeBuffer.x, t, this._activeBuffer.getNullCell(this._eraseAttrData()), this._eraseAttrData()), i.isWrapped = !1
+                            i.deleteCells(this._activeBuffer.x, t, this._activeBuffer.getNullCell(this._eraseAttrData())), i.isWrapped = !1
                         }
                         return this._dirtyRowTracker.markRangeDirty(this._activeBuffer.scrollTop, this._activeBuffer.scrollBottom), !0
                     }
                     eraseChars(e) {
                         this._restrictCursor();
                         const t = this._activeBuffer.lines.get(this._activeBuffer.ybase + this._activeBuffer.y);
-                        return t && (t.replaceCells(this._activeBuffer.x, this._activeBuffer.x + (e.params[0] || 1), this._activeBuffer.getNullCell(this._eraseAttrData()), this._eraseAttrData()), this._dirtyRowTracker.markDirty(this._activeBuffer.y)), !0
+                        return t && (t.replaceCells(this._activeBuffer.x, this._activeBuffer.x + (e.params[0] || 1), this._activeBuffer.getNullCell(this._eraseAttrData())), this._dirtyRowTracker.markDirty(this._activeBuffer.y)), !0
                     }
                     repeatPrecedingCharacter(e) {
                         const t = this._parser.precedingJoinState;
                         if (!t) return !0;
                         const i = e.params[0] || 1,
-                            s = g.UnicodeService.extractWidth(t),
+                            s = p.UnicodeService.extractWidth(t),
                             r = this._activeBuffer.x - s,
                             n = this._activeBuffer.lines.get(this._activeBuffer.ybase + this._activeBuffer.y).getString(r),
                             o = new Uint32Array(n.length * i);
                         let a = 0;
                         for (let e = 0; e < n.length;) {
                             const t = n.codePointAt(e) || 0;
                             o[a++] = t, e += t > 65535 ? 2 : 1
@@ -4112,22 +4259,22 @@
                     }
                     setScrollRegion(e) {
                         const t = e.params[0] || 1;
                         let i;
                         return (e.length < 2 || (i = e.params[1]) > this._bufferService.rows || 0 === i) && (i = this._bufferService.rows), i > t && (this._activeBuffer.scrollTop = t - 1, this._activeBuffer.scrollBottom = i - 1, this._setCursor(0, 0)), !0
                     }
                     windowOptions(e) {
-                        if (!y(e.params[0], this._optionsService.rawOptions.windowOptions)) return !0;
+                        if (!w(e.params[0], this._optionsService.rawOptions.windowOptions)) return !0;
                         const t = e.length > 1 ? e.params[1] : 0;
                         switch (e.params[0]) {
                             case 14:
-                                2 !== t && this._onRequestWindowsOptionsReport.fire(w.GET_WIN_SIZE_PIXELS);
+                                2 !== t && this._onRequestWindowsOptionsReport.fire(y.GET_WIN_SIZE_PIXELS);
                                 break;
                             case 16:
-                                this._onRequestWindowsOptionsReport.fire(w.GET_CELL_SIZE_PIXELS);
+                                this._onRequestWindowsOptionsReport.fire(y.GET_CELL_SIZE_PIXELS);
                                 break;
                             case 18:
                                 this._bufferService && this._coreService.triggerDataEvent(`${n.C0.ESC}[8;${this._bufferService.rows};${this._bufferService.cols}t`);
                                 break;
                             case 22:
                                 0 !== t && 2 !== t || (this._windowTitleStack.push(this._windowTitle), this._windowTitleStack.length > 10 && this._windowTitleStack.shift()), 0 !== t && 1 !== t || (this._iconNameStack.push(this._iconName), this._iconNameStack.length > 10 && this._iconNameStack.shift());
                                 break;
@@ -4411,15 +4558,15 @@
                         this._data.clear()
                     }
                 }
             },
             6114: (e, t) => {
                 Object.defineProperty(t, "__esModule", {
                     value: !0
-                }), t.isChromeOS = t.isLinux = t.isWindows = t.isIphone = t.isIpad = t.isMac = t.getSafariVersion = t.isSafari = t.isLegacyEdge = t.isFirefox = t.isNode = void 0, t.isNode = "undefined" != typeof process;
+                }), t.isChromeOS = t.isLinux = t.isWindows = t.isIphone = t.isIpad = t.isMac = t.getSafariVersion = t.isSafari = t.isLegacyEdge = t.isFirefox = t.isNode = void 0, t.isNode = "undefined" != typeof process && "title" in process;
                 const i = t.isNode ? "node" : navigator.userAgent,
                     s = t.isNode ? "node" : navigator.platform;
                 t.isFirefox = i.includes("Firefox"), t.isLegacyEdge = i.includes("Edge"), t.isSafari = /^((?!chrome|android).)*safari/i.test(i), t.getSafariVersion = function() {
                     if (!t.isSafari) return 0;
                     const e = i.match(/Version\/(\d+)/);
                     return null === e || e.length < 2 ? 0 : parseInt(e[1])
                 }, t.isMac = ["Macintosh", "MacIntel", "MacPPC", "Mac68K"].includes(s), t.isIpad = "iPad" === s, t.isIphone = "iPhone" === s, t.isWindows = ["Windows", "Win16", "Win32", "WinCE"].includes(s), t.isLinux = s.indexOf("Linux") >= 0, t.isChromeOS = /\bCrOS\b/.test(i)
@@ -4689,14 +4836,17 @@
                     }
                     isUnderlineColorDefault() {
                         return 268435456 & this.bg && ~this.extended.underlineColor ? 0 == (50331648 & this.extended.underlineColor) : this.isFgDefault()
                     }
                     getUnderlineStyle() {
                         return 268435456 & this.fg ? 268435456 & this.bg ? this.extended.underlineStyle : 1 : 0
                     }
+                    getUnderlineVariantOffset() {
+                        return this.extended.underlineVariantOffset
+                    }
                 }
                 t.AttributeData = i;
                 class s {
                     get ext() {
                         return this._urlId ? -469762049 & this._ext | this.underlineStyle << 26 : this._ext
                     }
                     set ext(e) {
@@ -4716,14 +4866,21 @@
                     }
                     get urlId() {
                         return this._urlId
                     }
                     set urlId(e) {
                         this._urlId = e
                     }
+                    get underlineVariantOffset() {
+                        const e = (3758096384 & this._ext) >> 29;
+                        return e < 0 ? 4294967288 ^ e : e
+                    }
+                    set underlineVariantOffset(e) {
+                        this._ext &= 536870911, this._ext |= e << 29 & 3758096384
+                    }
                     constructor(e = 0, t = 0) {
                         this._ext = 0, this._urlId = 0, this._ext = e, this._urlId = t
                     }
                     clone() {
                         return new s(this._ext, this._urlId)
                     }
                     isEmpty() {
@@ -4851,23 +5008,23 @@
                                 const e = this.getBlankLine(o.DEFAULT_ATTR_DATA, !0);
                                 v.push(e)
                             }
                             v.length > 0 && (s.push({
                                 start: n + c.length + r,
                                 newLines: v
                             }), r += v.length), c.push(...v);
-                            let g = _.length - 1,
-                                p = _[g];
-                            0 === p && (g--, p = _[g]);
+                            let p = _.length - 1,
+                                g = _[p];
+                            0 === g && (p--, g = _[p]);
                             let m = c.length - u - 1,
                                 S = d;
                             for (; m >= 0;) {
-                                const e = Math.min(S, p);
-                                if (void 0 === c[g]) break;
-                                if (c[g].copyCellsFrom(c[m], S - e, p - e, e, !0), p -= e, 0 === p && (g--, p = _[g]), S -= e, 0 === S) {
+                                const e = Math.min(S, g);
+                                if (void 0 === c[p]) break;
+                                if (c[p].copyCellsFrom(c[m], S - e, g - e, e, !0), g -= e, 0 === g && (p--, g = _[p]), S -= e, 0 === S) {
                                     m--;
                                     const e = Math.max(m, 0);
                                     S = (0, a.getWrappedLineTrimmedLength)(c, e, this._cols)
                                 }
                             }
                             for (let t = 0; t < c.length; t++) _[t] < e && c[t].setCell(_[t], i);
                             let C = u - f;
@@ -5004,44 +5161,44 @@
                     }
                     loadCell(e, t) {
                         return a = 3 * e, t.content = this._data[a + 0], t.fg = this._data[a + 1], t.bg = this._data[a + 2], 2097152 & t.content && (t.combinedData = this._combined[e]), 268435456 & t.bg && (t.extended = this._extendedAttrs[e]), t
                     }
                     setCell(e, t) {
                         2097152 & t.content && (this._combined[e] = t.combinedData), 268435456 & t.bg && (this._extendedAttrs[e] = t.extended), this._data[3 * e + 0] = t.content, this._data[3 * e + 1] = t.fg, this._data[3 * e + 2] = t.bg
                     }
-                    setCellFromCodePoint(e, t, i, s, r, n) {
-                        268435456 & r && (this._extendedAttrs[e] = n), this._data[3 * e + 0] = t | i << 22, this._data[3 * e + 1] = s, this._data[3 * e + 2] = r
+                    setCellFromCodepoint(e, t, i, s) {
+                        268435456 & s.bg && (this._extendedAttrs[e] = s.extended), this._data[3 * e + 0] = t | i << 22, this._data[3 * e + 1] = s.fg, this._data[3 * e + 2] = s.bg
                     }
                     addCodepointToCell(e, t, i) {
                         let s = this._data[3 * e + 0];
                         2097152 & s ? this._combined[e] += (0, o.stringFromCodePoint)(t) : 2097151 & s ? (this._combined[e] = (0, o.stringFromCodePoint)(2097151 & s) + (0, o.stringFromCodePoint)(t), s &= -2097152, s |= 2097152) : s = t | 1 << 22, i && (s &= -12582913, s |= i << 22), this._data[3 * e + 0] = s
                     }
-                    insertCells(e, t, i, n) {
-                        if ((e %= this.length) && 2 === this.getWidth(e - 1) && this.setCellFromCodePoint(e - 1, 0, 1, n?.fg || 0, n?.bg || 0, n?.extended || new s.ExtendedAttrs), t < this.length - e) {
+                    insertCells(e, t, i) {
+                        if ((e %= this.length) && 2 === this.getWidth(e - 1) && this.setCellFromCodepoint(e - 1, 0, 1, i), t < this.length - e) {
                             const s = new r.CellData;
                             for (let i = this.length - e - t - 1; i >= 0; --i) this.setCell(e + t + i, this.loadCell(e + i, s));
                             for (let s = 0; s < t; ++s) this.setCell(e + s, i)
                         } else
                             for (let t = e; t < this.length; ++t) this.setCell(t, i);
-                        2 === this.getWidth(this.length - 1) && this.setCellFromCodePoint(this.length - 1, 0, 1, n?.fg || 0, n?.bg || 0, n?.extended || new s.ExtendedAttrs)
+                        2 === this.getWidth(this.length - 1) && this.setCellFromCodepoint(this.length - 1, 0, 1, i)
                     }
-                    deleteCells(e, t, i, n) {
+                    deleteCells(e, t, i) {
                         if (e %= this.length, t < this.length - e) {
                             const s = new r.CellData;
                             for (let i = 0; i < this.length - e - t; ++i) this.setCell(e + i, this.loadCell(e + t + i, s));
                             for (let e = this.length - t; e < this.length; ++e) this.setCell(e, i)
                         } else
                             for (let t = e; t < this.length; ++t) this.setCell(t, i);
-                        e && 2 === this.getWidth(e - 1) && this.setCellFromCodePoint(e - 1, 0, 1, n?.fg || 0, n?.bg || 0, n?.extended || new s.ExtendedAttrs), 0 !== this.getWidth(e) || this.hasContent(e) || this.setCellFromCodePoint(e, 0, 1, n?.fg || 0, n?.bg || 0, n?.extended || new s.ExtendedAttrs)
+                        e && 2 === this.getWidth(e - 1) && this.setCellFromCodepoint(e - 1, 0, 1, i), 0 !== this.getWidth(e) || this.hasContent(e) || this.setCellFromCodepoint(e, 0, 1, i)
                     }
-                    replaceCells(e, t, i, r, n = !1) {
-                        if (n)
-                            for (e && 2 === this.getWidth(e - 1) && !this.isProtected(e - 1) && this.setCellFromCodePoint(e - 1, 0, 1, r?.fg || 0, r?.bg || 0, r?.extended || new s.ExtendedAttrs), t < this.length && 2 === this.getWidth(t - 1) && !this.isProtected(t) && this.setCellFromCodePoint(t, 0, 1, r?.fg || 0, r?.bg || 0, r?.extended || new s.ExtendedAttrs); e < t && e < this.length;) this.isProtected(e) || this.setCell(e, i), e++;
+                    replaceCells(e, t, i, s = !1) {
+                        if (s)
+                            for (e && 2 === this.getWidth(e - 1) && !this.isProtected(e - 1) && this.setCellFromCodepoint(e - 1, 0, 1, i), t < this.length && 2 === this.getWidth(t - 1) && !this.isProtected(t) && this.setCellFromCodepoint(t, 0, 1, i); e < t && e < this.length;) this.isProtected(e) || this.setCell(e, i), e++;
                         else
-                            for (e && 2 === this.getWidth(e - 1) && this.setCellFromCodePoint(e - 1, 0, 1, r?.fg || 0, r?.bg || 0, r?.extended || new s.ExtendedAttrs), t < this.length && 2 === this.getWidth(t - 1) && this.setCellFromCodePoint(t, 0, 1, r?.fg || 0, r?.bg || 0, r?.extended || new s.ExtendedAttrs); e < t && e < this.length;) this.setCell(e++, i)
+                            for (e && 2 === this.getWidth(e - 1) && this.setCellFromCodepoint(e - 1, 0, 1, i), t < this.length && 2 === this.getWidth(t - 1) && this.setCellFromCodepoint(t, 0, 1, i); e < t && e < this.length;) this.setCell(e++, i)
                     }
                     resize(e, t) {
                         if (e === this.length) return 4 * this._data.length * 2 < this._data.buffer.byteLength;
                         const i = 3 * e;
                         if (e > this.length) {
                             if (this._data.buffer.byteLength >= 4 * i) this._data = new Uint32Array(this._data.buffer, 0, i);
                             else {
@@ -5116,23 +5273,26 @@
                                 }
                         const o = Object.keys(e._combined);
                         for (let s = 0; s < o.length; s++) {
                             const r = parseInt(o[s], 10);
                             r >= t && (this._combined[r - t + i] = e._combined[r])
                         }
                     }
-                    translateToString(e = !1, t = 0, i = this.length) {
-                        e && (i = Math.min(i, this.getTrimmedLength()));
-                        let s = "";
+                    translateToString(e, t, i, s) {
+                        t = t ?? 0, i = i ?? this.length, e && (i = Math.min(i, this.getTrimmedLength())), s && (s.length = 0);
+                        let r = "";
                         for (; t < i;) {
                             const e = this._data[3 * t + 0],
-                                i = 2097151 & e;
-                            s += 2097152 & e ? this._combined[t] : i ? (0, o.stringFromCodePoint)(i) : n.WHITESPACE_CELL_CHAR, t += e >> 22 || 1
+                                i = 2097151 & e,
+                                a = 2097152 & e ? this._combined[t] : i ? (0, o.stringFromCodePoint)(i) : n.WHITESPACE_CELL_CHAR;
+                            if (r += a, s)
+                                for (let e = 0; e < a.length; ++e) s.push(t);
+                            t += e >> 22 || 1
                         }
-                        return s
+                        return s && s.push(t), r
                     }
                 }
                 t.BufferLine = h
             },
             4841: (e, t) => {
                 Object.defineProperty(t, "__esModule", {
                     value: !0
@@ -5538,19 +5698,15 @@
                         },
                         a = (e.shiftKey ? 1 : 0) | (e.altKey ? 2 : 0) | (e.ctrlKey ? 4 : 0) | (e.metaKey ? 8 : 0);
                     switch (e.keyCode) {
                         case 0:
                             "UIKeyInputUpArrow" === e.key ? o.key = t ? s.C0.ESC + "OA" : s.C0.ESC + "[A" : "UIKeyInputLeftArrow" === e.key ? o.key = t ? s.C0.ESC + "OD" : s.C0.ESC + "[D" : "UIKeyInputRightArrow" === e.key ? o.key = t ? s.C0.ESC + "OC" : s.C0.ESC + "[C" : "UIKeyInputDownArrow" === e.key && (o.key = t ? s.C0.ESC + "OB" : s.C0.ESC + "[B");
                             break;
                         case 8:
-                            if (e.altKey) {
-                                o.key = s.C0.ESC + s.C0.DEL;
-                                break
-                            }
-                            o.key = s.C0.DEL;
+                            o.key = e.ctrlKey ? "\b" : s.C0.DEL, e.altKey && (o.key = s.C0.ESC + o.key);
                             break;
                         case 9:
                             if (e.shiftKey) {
                                 o.key = s.C0.ESC + "[Z";
                                 break
                             }
                             o.key = s.C0.HT, o.cancel = !0;
@@ -7262,14 +7418,15 @@
                     macOptionClickForcesSelection: !1,
                     minimumContrastRatio: 1,
                     disableStdin: !1,
                     allowProposedApi: !1,
                     allowTransparency: !1,
                     tabStopWidth: 8,
                     theme: {},
+                    rescaleOverlappingGlyphs: !1,
                     rightClickSelectsWord: n.isMac,
                     windowOptions: {},
                     windowsMode: !1,
                     windowsPty: {},
                     wordSeparator: " ()[]{}',\"`",
                     altClickMovesCursor: !0,
                     convertEol: !1,
@@ -7289,15 +7446,17 @@
                                 const s = e[t];
                                 i[t] = this._sanitizeAndValidateOption(t, s)
                             } catch (e) {
                                 console.error(e)
                             }
                         this.rawOptions = i, this.options = {
                             ...i
-                        }, this._setupOptions()
+                        }, this._setupOptions(), this.register((0, r.toDisposable)((() => {
+                            this.rawOptions.linkHandler = null, this.rawOptions.documentOverride = null
+                        })))
                     }
                     onSpecificOptionChange(e, t) {
                         return this.onOptionChange((i => {
                             i === e && t(this.rawOptions[e])
                         }))
                     }
                     onMultipleOptionChange(e, t) {
@@ -7676,23 +7835,29 @@
             }
             blur() {
                 this._core.blur()
             }
             focus() {
                 this._core.focus()
             }
+            input(e, t = !0) {
+                this._core.input(e, t)
+            }
             resize(e, t) {
                 this._verifyIntegers(e, t), this._core.resize(e, t)
             }
             open(e) {
                 this._core.open(e)
             }
             attachCustomKeyEventHandler(e) {
                 this._core.attachCustomKeyEventHandler(e)
             }
+            attachCustomWheelEventHandler(e) {
+                this._core.attachCustomWheelEventHandler(e)
+            }
             registerLinkProvider(e) {
                 return this._core.registerLinkProvider(e)
             }
             registerCharacterJoiner(e) {
                 return this._checkProposedApi(), this._core.registerCharacterJoiner(e)
             }
             deregisterCharacterJoiner(e) {
```

### Comparing `meerschaum-2.1.7/meerschaum/api/resources/templates/index.html` & `meerschaum-2.2.0.dev1/meerschaum/api/resources/templates/index.html`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/api/resources/templates/old_index.html` & `meerschaum-2.2.0.dev1/meerschaum/api/resources/templates/old_index.html`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/api/resources/templates/termpage.html` & `meerschaum-2.2.0.dev1/meerschaum/api/resources/templates/termpage.html`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/api/routes/__init__.py` & `meerschaum-2.2.0.dev1/meerschaum/api/routes/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/api/routes/_actions.py` & `meerschaum-2.2.0.dev1/meerschaum/api/routes/_actions.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/api/routes/_connectors.py` & `meerschaum-2.2.0.dev1/meerschaum/api/routes/_connectors.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/api/routes/_index.py` & `meerschaum-2.2.0.dev1/meerschaum/api/routes/_index.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/api/routes/_login.py` & `meerschaum-2.2.0.dev1/meerschaum/api/routes/_login.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/api/routes/_misc.py` & `meerschaum-2.2.0.dev1/meerschaum/api/routes/_misc.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/api/routes/_pipes.py` & `meerschaum-2.2.0.dev1/meerschaum/api/routes/_pipes.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/api/routes/_plugins.py` & `meerschaum-2.2.0.dev1/meerschaum/api/routes/_plugins.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/api/routes/_users.py` & `meerschaum-2.2.0.dev1/meerschaum/api/routes/_users.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/api/routes/_version.py` & `meerschaum-2.2.0.dev1/meerschaum/api/routes/_version.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/api/routes/_webterm.py` & `meerschaum-2.2.0.dev1/meerschaum/api/routes/_webterm.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/config/__init__.py` & `meerschaum-2.2.0.dev1/meerschaum/config/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/config/_default.py` & `meerschaum-2.2.0.dev1/meerschaum/config/_default.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/config/_edit.py` & `meerschaum-2.2.0.dev1/meerschaum/config/_edit.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/config/_environment.py` & `meerschaum-2.2.0.dev1/meerschaum/config/_environment.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/config/_formatting.py` & `meerschaum-2.2.0.dev1/meerschaum/config/_formatting.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/config/_jobs.py` & `meerschaum-2.2.0.dev1/meerschaum/config/_jobs.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/config/_patch.py` & `meerschaum-2.2.0.dev1/meerschaum/config/_patch.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/config/_paths.py` & `meerschaum-2.2.0.dev1/meerschaum/config/_paths.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/config/_preprocess.py` & `meerschaum-2.2.0.dev1/meerschaum/config/_preprocess.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/config/_read_config.py` & `meerschaum-2.2.0.dev1/meerschaum/config/_read_config.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/config/_shell.py` & `meerschaum-2.2.0.dev1/meerschaum/config/_shell.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/config/_sync.py` & `meerschaum-2.2.0.dev1/meerschaum/config/_sync.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/config/stack/__init__.py` & `meerschaum-2.2.0.dev1/meerschaum/config/stack/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/config/stack/grafana/__init__.py` & `meerschaum-2.2.0.dev1/meerschaum/config/stack/grafana/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/config/static/__init__.py` & `meerschaum-2.2.0.dev1/meerschaum/config/static/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/connectors/Connector.py` & `meerschaum-2.2.0.dev1/meerschaum/connectors/Connector.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/connectors/__init__.py` & `meerschaum-2.2.0.dev1/meerschaum/connectors/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/connectors/api/APIConnector.py` & `meerschaum-2.2.0.dev1/meerschaum/connectors/api/APIConnector.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/connectors/api/_actions.py` & `meerschaum-2.2.0.dev1/meerschaum/connectors/api/_actions.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/connectors/api/_fetch.py` & `meerschaum-2.2.0.dev1/meerschaum/connectors/api/_fetch.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/connectors/api/_login.py` & `meerschaum-2.2.0.dev1/meerschaum/connectors/api/_login.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/connectors/api/_misc.py` & `meerschaum-2.2.0.dev1/meerschaum/connectors/api/_misc.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/connectors/api/_pipes.py` & `meerschaum-2.2.0.dev1/meerschaum/connectors/api/_pipes.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/connectors/api/_plugins.py` & `meerschaum-2.2.0.dev1/meerschaum/connectors/api/_plugins.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,14 +45,15 @@
         return False, response.text
 
     return success, msg
 
 def install_plugin(
         self,
         name: str,
+        skip_deps: bool = False,
         force: bool = False,
         debug: bool = False
     ) -> SuccessTuple:
     """Download and attempt to install a plugin from the API."""
     import os, pathlib, json
     from meerschaum.core import Plugin
     from meerschaum.config._paths import PLUGINS_TEMP_RESOURCES_PATH
@@ -74,15 +75,15 @@
                 success, msg = tuple(j)
             elif isinstance(j, dict) and 'detail' in j:
                 success, msg = False, fail_msg
         except Exception as e:
             success, msg = False, fail_msg
         return success, msg
     plugin = Plugin(name, archive_path=archive_path, repo_connector=self)
-    return plugin.install(force=force, debug=debug)
+    return plugin.install(skip_deps=skip_deps, force=force, debug=debug)
 
 def get_plugins(
         self,
         user_id : Optional[int] = None,
         search_term : Optional[str] = None,
         debug : bool = False
     ) -> Sequence[str]:
```

### Comparing `meerschaum-2.1.7/meerschaum/connectors/api/_request.py` & `meerschaum-2.2.0.dev1/meerschaum/connectors/api/_request.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/connectors/api/_uri.py` & `meerschaum-2.2.0.dev1/meerschaum/connectors/api/_uri.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/connectors/api/_users.py` & `meerschaum-2.2.0.dev1/meerschaum/connectors/api/_users.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/connectors/parse.py` & `meerschaum-2.2.0.dev1/meerschaum/connectors/parse.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/connectors/plugin/PluginConnector.py` & `meerschaum-2.2.0.dev1/meerschaum/connectors/plugin/PluginConnector.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/connectors/poll.py` & `meerschaum-2.2.0.dev1/meerschaum/connectors/poll.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/connectors/sql/SQLConnector.py` & `meerschaum-2.2.0.dev1/meerschaum/connectors/sql/SQLConnector.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/connectors/sql/_cli.py` & `meerschaum-2.2.0.dev1/meerschaum/connectors/sql/_cli.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/connectors/sql/_create_engine.py` & `meerschaum-2.2.0.dev1/meerschaum/connectors/sql/_create_engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -150,26 +150,26 @@
     },
 }
 install_flavor_drivers = {
     'sqlite': ['aiosqlite'],
     'duckdb': ['duckdb', 'duckdb_engine'],
     'mysql': ['pymysql'],
     'mariadb': ['pymysql'],
-    'timescaledb': ['psycopg2'],
-    'postgresql': ['psycopg2'],
-    'citus': ['psycopg2'],
-    'cockroachdb': ['psycopg2', 'sqlalchemy_cockroachdb', 'sqlalchemy_cockroachdb.psycopg2'],
+    'timescaledb': ['psycopg'],
+    'postgresql': ['psycopg'],
+    'citus': ['psycopg'],
+    'cockroachdb': ['psycopg', 'sqlalchemy_cockroachdb', 'sqlalchemy_cockroachdb.psycopg'],
     'mssql': ['pyodbc'],
     'oracle': ['cx_Oracle'],
 }
 require_patching_flavors = {'cockroachdb': [('sqlalchemy-cockroachdb', 'sqlalchemy_cockroachdb')]}
 
 flavor_dialects = {
     'cockroachdb': (
-        'cockroachdb', 'sqlalchemy_cockroachdb.psycopg2', 'CockroachDBDialect_psycopg2'
+        'cockroachdb', 'sqlalchemy_cockroachdb.psycopg', 'CockroachDBDialect_psycopg'
     ),
     'duckdb': ('duckdb', 'duckdb_engine', 'Dialect'),
 }
 
 def create_engine(
         self,
         include_uri: bool = False,
```

### Comparing `meerschaum-2.1.7/meerschaum/connectors/sql/_fetch.py` & `meerschaum-2.2.0.dev1/meerschaum/connectors/sql/_fetch.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/connectors/sql/_instance.py` & `meerschaum-2.2.0.dev1/meerschaum/connectors/sql/_instance.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/connectors/sql/_pipes.py` & `meerschaum-2.2.0.dev1/meerschaum/connectors/sql/_pipes.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/connectors/sql/_plugins.py` & `meerschaum-2.2.0.dev1/meerschaum/connectors/sql/_plugins.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/connectors/sql/_sql.py` & `meerschaum-2.2.0.dev1/meerschaum/connectors/sql/_sql.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/connectors/sql/_uri.py` & `meerschaum-2.2.0.dev1/meerschaum/connectors/sql/_uri.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/connectors/sql/_users.py` & `meerschaum-2.2.0.dev1/meerschaum/connectors/sql/_users.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/connectors/sql/tables/__init__.py` & `meerschaum-2.2.0.dev1/meerschaum/connectors/sql/tables/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/connectors/sql/tables/types.py` & `meerschaum-2.2.0.dev1/meerschaum/connectors/sql/tables/types.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/core/Pipe/__init__.py` & `meerschaum-2.2.0.dev1/meerschaum/core/Pipe/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/core/Pipe/_attributes.py` & `meerschaum-2.2.0.dev1/meerschaum/core/Pipe/_attributes.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/core/Pipe/_bootstrap.py` & `meerschaum-2.2.0.dev1/meerschaum/core/Pipe/_bootstrap.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/core/Pipe/_clear.py` & `meerschaum-2.2.0.dev1/meerschaum/core/Pipe/_clear.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/core/Pipe/_data.py` & `meerschaum-2.2.0.dev1/meerschaum/core/Pipe/_data.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/core/Pipe/_deduplicate.py` & `meerschaum-2.2.0.dev1/meerschaum/core/Pipe/_deduplicate.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/core/Pipe/_delete.py` & `meerschaum-2.2.0.dev1/meerschaum/core/Pipe/_delete.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/core/Pipe/_drop.py` & `meerschaum-2.2.0.dev1/meerschaum/core/Pipe/_drop.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/core/Pipe/_dtypes.py` & `meerschaum-2.2.0.dev1/meerschaum/core/Pipe/_dtypes.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/core/Pipe/_edit.py` & `meerschaum-2.2.0.dev1/meerschaum/core/Pipe/_edit.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/core/Pipe/_fetch.py` & `meerschaum-2.2.0.dev1/meerschaum/core/Pipe/_fetch.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/core/Pipe/_register.py` & `meerschaum-2.2.0.dev1/meerschaum/core/Pipe/_register.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/core/Pipe/_show.py` & `meerschaum-2.2.0.dev1/meerschaum/core/Pipe/_show.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/core/Pipe/_sync.py` & `meerschaum-2.2.0.dev1/meerschaum/core/Pipe/_sync.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/core/Pipe/_verify.py` & `meerschaum-2.2.0.dev1/meerschaum/core/Pipe/_verify.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/core/User/_User.py` & `meerschaum-2.2.0.dev1/meerschaum/core/User/_User.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/plugins/_Plugin.py` & `meerschaum-2.2.0.dev1/meerschaum/plugins/_Plugin.py`

 * *Files 0% similar despite different names*

```diff
@@ -248,25 +248,29 @@
         if debug:
             dprint(f"Created archive '{self.archive_path}'.")
         return self.archive_path
 
 
     def install(
             self,
+            skip_deps: bool = False,
             force: bool = False,
             debug: bool = False,
         ) -> SuccessTuple:
         """
         Extract a plugin's tar archive to the plugins directory.
         
         This function checks if the plugin is already installed and if the version is equal or
         greater than the existing installation.
 
         Parameters
         ----------
+        skip_deps: bool, default False
+            If `True`, do not install dependencies.
+
         force: bool, default False
             If `True`, continue with installation, even if required packages fail to install.
 
         debug: bool, default False
             Verbosity toggle.
 
         Returns
@@ -362,15 +366,19 @@
                 self.name in files_in_plugins_dir
                 or
                 (self.name + '.py') in files_in_plugins_dir
             ):
                 plugin_installation_dir_path = path
                 break
 
-        success_msg = f"Successfully installed plugin '{self}'."
+        success_msg = (
+            f"Successfully installed plugin '{self}'"
+            + ("\n    (skipped dependencies)" if skip_deps else "")
+            + "."
+        )
         success, abort = None, None
 
         if is_same_version and not force:
             success, msg = True, (
                 f"Plugin '{self}' is up-to-date (version {old_version}).\n" +
                 "    Install again with `-f` or `--force` to reinstall."
             )
@@ -419,15 +427,16 @@
 
         ### if we've already failed, return here
         if not success or abort:
             _ongoing_installations.remove(self.full_name)
             return success, msg
 
         ### attempt to install dependencies
-        if not self.install_dependencies(force=force, debug=debug):
+        dependencies_installed = skip_deps or self.install_dependencies(force=force, debug=debug)
+        if not dependencies_installed:
             _ongoing_installations.remove(self.full_name)
             return False, f"Failed to install dependencies for plugin '{self}'."
 
         ### handling success tuple, bool, or other (typically None)
         setup_tuple = self.setup(debug=debug)
         if isinstance(setup_tuple, tuple):
             if not setup_tuple[0]:
```

### Comparing `meerschaum-2.1.7/meerschaum/plugins/__init__.py` & `meerschaum-2.2.0.dev1/meerschaum/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/utils/__init__.py` & `meerschaum-2.2.0.dev1/meerschaum/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/utils/_get_pipes.py` & `meerschaum-2.2.0.dev1/meerschaum/utils/_get_pipes.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/utils/daemon/Daemon.py` & `meerschaum-2.2.0.dev1/meerschaum/utils/daemon/Daemon.py`

 * *Files 0% similar despite different names*

```diff
@@ -861,29 +861,37 @@
             error(_write_properties_success_tuple[1])
 
         _write_pickle_success_tuple = self.write_pickle()
         if not _write_pickle_success_tuple[0]:
             error(_write_pickle_success_tuple[1])
 
 
-    def cleanup(self, keep_logs: bool = False) -> None:
-        """Remove a daemon's directory after execution.
+    def cleanup(self, keep_logs: bool = False) -> SuccessTuple:
+        """
+        Remove a daemon's directory after execution.
 
         Parameters
         ----------
         keep_logs: bool, default False
             If `True`, skip deleting the daemon's log files.
+
+        Returns
+        -------
+        A `SuccessTuple` indicating success.
         """
         if self.path.exists():
             try:
                 shutil.rmtree(self.path)
             except Exception as e:
-                warn(e)
+                msg = f"Failed to clean up '{self.daemon_id}':\n{e}"
+                warn(msg)
+                return False, msg
         if not keep_logs:
             self.rotating_log.delete()
+        return True, "Success"
 
 
     def get_timeout_seconds(self, timeout: Union[int, float, None] = None) -> Union[int, float]:
         """
         Return the timeout value to use. Use `--timeout-seconds` if provided,
         else the configured default (8).
         """
```

### Comparing `meerschaum-2.1.7/meerschaum/utils/daemon/RotatingFile.py` & `meerschaum-2.2.0.dev1/meerschaum/utils/daemon/RotatingFile.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/utils/daemon/__init__.py` & `meerschaum-2.2.0.dev1/meerschaum/utils/daemon/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/utils/daemon/_names.py` & `meerschaum-2.2.0.dev1/meerschaum/utils/daemon/_names.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/utils/dataframe.py` & `meerschaum-2.2.0.dev1/meerschaum/utils/dataframe.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/utils/debug.py` & `meerschaum-2.2.0.dev1/meerschaum/utils/debug.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/utils/dtypes/__init__.py` & `meerschaum-2.2.0.dev1/meerschaum/utils/dtypes/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,16 +2,18 @@
 # -*- coding: utf-8 -*-
 # vim:fenc=utf-8
 
 """
 Utility functions for working with data types.
 """
 
+import traceback
 from decimal import Decimal, Context, InvalidOperation
 from meerschaum.utils.typing import Dict, Union, Any
+from meerschaum.utils.warnings import warn
 
 MRSM_PD_DTYPES: Dict[str, str] = {
     'json': 'object',
     'numeric': 'object',
     'datetime': 'datetime64[ns]',
     'bool': 'bool[pyarrow]',
     'int': 'Int64',
@@ -33,17 +35,15 @@
 
     ### NOTE: Kind of a hack, but if the first word of the given dtype is in all caps,
     ### treat it as a SQL db type.
     if dtype.split(' ')[0].isupper():
         from meerschaum.utils.dtypes.sql import get_pd_type_from_db_type
         return get_pd_type_from_db_type(dtype)
 
-    import traceback
     from meerschaum.utils.packages import attempt_import
-    from meerschaum.utils.warnings import warn
     pandas = attempt_import('pandas', lazy=False)
 
     try:
         return str(pandas.api.types.pandas_dtype(dtype))
     except Exception as e:
         warn(
             f"Invalid dtype '{dtype}', will use 'object' instead:\n"
@@ -84,16 +84,20 @@
                 return False
             ltype = ldtype[lkey]
             rtype = rdtype[rkey]
             if not are_dtypes_equal(ltype, rtype):
                 return False
         return True
 
-    if ldtype == rdtype:
-        return True
+    try:
+        if ldtype == rdtype:
+            return True
+    except Exception as e:
+        warn(f"Exception when comparing dtypes, returning False:\n{traceback.format_exc()}")
+        return False
 
     ### Sometimes pandas dtype objects are passed.
     ldtype = str(ldtype)
     rdtype = str(rdtype)
 
     json_dtypes = ('json', 'object')
     if ldtype in json_dtypes and rdtype in json_dtypes:
@@ -173,15 +177,15 @@
             if not value_is_null(value)
             else Decimal('NaN')
         )
     except Exception as e:
         return value
 
 
-def value_is_null(value: Any) -> Any:
+def value_is_null(value: Any) -> bool:
     """
     Determine if a value is a null-like string.
     """
     return str(value).lower() in ('none', 'nan', 'na', 'nat', '', '<na>')
 
 
 def none_if_null(value: Any) -> Any:
```

### Comparing `meerschaum-2.1.7/meerschaum/utils/dtypes/sql.py` & `meerschaum-2.2.0.dev1/meerschaum/utils/dtypes/sql.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/utils/formatting/__init__.py` & `meerschaum-2.2.0.dev1/meerschaum/utils/formatting/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/utils/formatting/_jobs.py` & `meerschaum-2.2.0.dev1/meerschaum/utils/formatting/_jobs.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/utils/formatting/_pipes.py` & `meerschaum-2.2.0.dev1/meerschaum/utils/formatting/_pipes.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/utils/formatting/_pprint.py` & `meerschaum-2.2.0.dev1/meerschaum/utils/formatting/_pprint.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/utils/formatting/_shell.py` & `meerschaum-2.2.0.dev1/meerschaum/utils/formatting/_shell.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/utils/interactive.py` & `meerschaum-2.2.0.dev1/meerschaum/utils/interactive.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/utils/misc.py` & `meerschaum-2.2.0.dev1/meerschaum/utils/misc.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/utils/networking.py` & `meerschaum-2.2.0.dev1/meerschaum/utils/networking.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/utils/packages/__init__.py` & `meerschaum-2.2.0.dev1/meerschaum/utils/packages/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/utils/packages/_packages.py` & `meerschaum-2.2.0.dev1/meerschaum/utils/packages/_packages.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         'watchgod'                   : 'watchgod>=0.7.0',
         'dill'                       : 'dill>=0.3.3',
         'virtualenv'                 : 'virtualenv>=20.1.0',
         'rocketry'                   : 'rocketry>=2.5.1',
     },
     'drivers': {
         'cryptography'               : 'cryptography>=38.0.1',
-        'psycopg2'                   : 'psycopg2-binary>=2.8.6',
+        'psycopg'                    : 'psycopg[binary]>=3.1.18',
         'pymysql'                    : 'PyMySQL>=0.9.0',
         'aiomysql'                   : 'aiomysql>=0.0.21',
         'sqlalchemy_cockroachdb'     : 'sqlalchemy-cockroachdb>=2.0.0',
         'duckdb'                     : 'duckdb>=0.9.0',
         'duckdb_engine'              : 'duckdb-engine>=0.9.2',
     },
     '_drivers': {
```

### Comparing `meerschaum-2.1.7/meerschaum/utils/packages/lazy_loader.py` & `meerschaum-2.2.0.dev1/meerschaum/utils/packages/lazy_loader.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/utils/pool.py` & `meerschaum-2.2.0.dev1/meerschaum/utils/pool.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/utils/process.py` & `meerschaum-2.2.0.dev1/meerschaum/utils/process.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/utils/prompt.py` & `meerschaum-2.2.0.dev1/meerschaum/utils/prompt.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/utils/schedule.py` & `meerschaum-2.2.0.dev1/meerschaum/utils/schedule.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/utils/sql.py` & `meerschaum-2.2.0.dev1/meerschaum/utils/sql.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/utils/threading.py` & `meerschaum-2.2.0.dev1/meerschaum/utils/threading.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/utils/typing.py` & `meerschaum-2.2.0.dev1/meerschaum/utils/typing.py`

 * *Files 4% similar despite different names*

```diff
@@ -82,15 +82,15 @@
 PipesDict = Dict[
     str, Dict[                           ### connector_keys : metrics
         str, Dict[                       ### metric_key     : locations
             str, 'meerschaum.Pipe'       ### location_key   : Pipe
         ]
     ]
 ]
-WebState = Dict[str, str]
+WebState = Dict[str, Union[str, Dict[str, str]]]
 
 def is_success_tuple(x: Any) -> bool:
     """
     Determine whether an object is a `SuccessTuple`.
     """
     return (
         isinstance(x, tuple)
```

### Comparing `meerschaum-2.1.7/meerschaum/utils/venv/_Venv.py` & `meerschaum-2.2.0.dev1/meerschaum/utils/venv/_Venv.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/utils/venv/__init__.py` & `meerschaum-2.2.0.dev1/meerschaum/utils/venv/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/utils/warnings.py` & `meerschaum-2.2.0.dev1/meerschaum/utils/warnings.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum/utils/yaml.py` & `meerschaum-2.2.0.dev1/meerschaum/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum.egg-info/PKG-INFO` & `meerschaum-2.2.0.dev1/meerschaum.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meerschaum
-Version: 2.1.7
+Version: 2.2.0.dev1
 Summary: Sync Time-Series Pipes with Meerschaum
 Home-page: https://meerschaum.io
 Author: Bennett Meares
 Author-email: bennett.meares@gmail.com
 Maintainer-email: bennett.meares@gmail.com
 License: Apache Software License 2.0
 Project-URL: Documentation, https://docs.meerschaum.io
@@ -63,15 +63,15 @@
 Requires-Dist: psutil>=5.8.0; extra == "required"
 Requires-Dist: watchgod>=0.7.0; extra == "required"
 Requires-Dist: dill>=0.3.3; extra == "required"
 Requires-Dist: virtualenv>=20.1.0; extra == "required"
 Requires-Dist: rocketry>=2.5.1; extra == "required"
 Provides-Extra: drivers
 Requires-Dist: cryptography>=38.0.1; extra == "drivers"
-Requires-Dist: psycopg2-binary>=2.8.6; extra == "drivers"
+Requires-Dist: psycopg[binary]>=3.1.18; extra == "drivers"
 Requires-Dist: PyMySQL>=0.9.0; extra == "drivers"
 Requires-Dist: aiomysql>=0.0.21; extra == "drivers"
 Requires-Dist: sqlalchemy-cockroachdb>=2.0.0; extra == "drivers"
 Requires-Dist: duckdb>=0.9.0; extra == "drivers"
 Requires-Dist: duckdb-engine>=0.9.2; extra == "drivers"
 Provides-Extra: drivers
 Requires-Dist: pyodbc>=4.0.30; extra == "drivers"
@@ -124,15 +124,15 @@
 Requires-Dist: pytz; extra == "sql"
 Requires-Dist: joblib>=0.17.0; extra == "sql"
 Requires-Dist: SQLAlchemy>=2.0.5; extra == "sql"
 Requires-Dist: databases>=0.4.0; extra == "sql"
 Requires-Dist: aiosqlite>=0.16.0; extra == "sql"
 Requires-Dist: asyncpg>=0.21.0; extra == "sql"
 Requires-Dist: cryptography>=38.0.1; extra == "sql"
-Requires-Dist: psycopg2-binary>=2.8.6; extra == "sql"
+Requires-Dist: psycopg[binary]>=3.1.18; extra == "sql"
 Requires-Dist: PyMySQL>=0.9.0; extra == "sql"
 Requires-Dist: aiomysql>=0.0.21; extra == "sql"
 Requires-Dist: sqlalchemy-cockroachdb>=2.0.0; extra == "sql"
 Requires-Dist: duckdb>=0.9.0; extra == "sql"
 Requires-Dist: duckdb-engine>=0.9.2; extra == "sql"
 Requires-Dist: wheel>=0.34.2; extra == "sql"
 Requires-Dist: setuptools>=63.3.0; extra == "sql"
@@ -183,15 +183,15 @@
 Requires-Dist: pytz; extra == "api"
 Requires-Dist: joblib>=0.17.0; extra == "api"
 Requires-Dist: SQLAlchemy>=2.0.5; extra == "api"
 Requires-Dist: databases>=0.4.0; extra == "api"
 Requires-Dist: aiosqlite>=0.16.0; extra == "api"
 Requires-Dist: asyncpg>=0.21.0; extra == "api"
 Requires-Dist: cryptography>=38.0.1; extra == "api"
-Requires-Dist: psycopg2-binary>=2.8.6; extra == "api"
+Requires-Dist: psycopg[binary]>=3.1.18; extra == "api"
 Requires-Dist: PyMySQL>=0.9.0; extra == "api"
 Requires-Dist: aiomysql>=0.0.21; extra == "api"
 Requires-Dist: sqlalchemy-cockroachdb>=2.0.0; extra == "api"
 Requires-Dist: duckdb>=0.9.0; extra == "api"
 Requires-Dist: duckdb-engine>=0.9.2; extra == "api"
 Requires-Dist: wheel>=0.34.2; extra == "api"
 Requires-Dist: setuptools>=63.3.0; extra == "api"
@@ -259,15 +259,15 @@
 Requires-Dist: fasteners>=0.18.0; extra == "full"
 Requires-Dist: psutil>=5.8.0; extra == "full"
 Requires-Dist: watchgod>=0.7.0; extra == "full"
 Requires-Dist: dill>=0.3.3; extra == "full"
 Requires-Dist: virtualenv>=20.1.0; extra == "full"
 Requires-Dist: rocketry>=2.5.1; extra == "full"
 Requires-Dist: cryptography>=38.0.1; extra == "full"
-Requires-Dist: psycopg2-binary>=2.8.6; extra == "full"
+Requires-Dist: psycopg[binary]>=3.1.18; extra == "full"
 Requires-Dist: PyMySQL>=0.9.0; extra == "full"
 Requires-Dist: aiomysql>=0.0.21; extra == "full"
 Requires-Dist: sqlalchemy-cockroachdb>=2.0.0; extra == "full"
 Requires-Dist: duckdb>=0.9.0; extra == "full"
 Requires-Dist: duckdb-engine>=0.9.2; extra == "full"
 Requires-Dist: toga>=0.3.0-dev29; extra == "full"
 Requires-Dist: pywebview>=3.6.3; extra == "full"
```

### Comparing `meerschaum-2.1.7/meerschaum.egg-info/SOURCES.txt` & `meerschaum-2.2.0.dev1/meerschaum.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/meerschaum.egg-info/requires.txt` & `meerschaum-2.2.0.dev1/meerschaum.egg-info/requires.txt`

 * *Files 5% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 pytz
 joblib>=0.17.0
 SQLAlchemy>=2.0.5
 databases>=0.4.0
 aiosqlite>=0.16.0
 asyncpg>=0.21.0
 cryptography>=38.0.1
-psycopg2-binary>=2.8.6
+psycopg[binary]>=3.1.18
 PyMySQL>=0.9.0
 aiomysql>=0.0.21
 sqlalchemy-cockroachdb>=2.0.0
 duckdb>=0.9.0
 duckdb-engine>=0.9.2
 wheel>=0.34.2
 setuptools>=63.3.0
@@ -133,15 +133,15 @@
 mkdocs-section-index>=0.3.3
 mkdocs-linkcheck>=1.0.6
 mkdocs-redirects>=1.0.4
 jinja2==3.0.3
 
 [drivers]
 cryptography>=38.0.1
-psycopg2-binary>=2.8.6
+psycopg[binary]>=3.1.18
 PyMySQL>=0.9.0
 aiomysql>=0.0.21
 sqlalchemy-cockroachdb>=2.0.0
 duckdb>=0.9.0
 duckdb-engine>=0.9.2
 
 [extras]
@@ -189,15 +189,15 @@
 fasteners>=0.18.0
 psutil>=5.8.0
 watchgod>=0.7.0
 dill>=0.3.3
 virtualenv>=20.1.0
 rocketry>=2.5.1
 cryptography>=38.0.1
-psycopg2-binary>=2.8.6
+psycopg[binary]>=3.1.18
 PyMySQL>=0.9.0
 aiomysql>=0.0.21
 sqlalchemy-cockroachdb>=2.0.0
 duckdb>=0.9.0
 duckdb-engine>=0.9.2
 toga>=0.3.0-dev29
 pywebview>=3.6.3
@@ -250,15 +250,15 @@
 pytz
 joblib>=0.17.0
 SQLAlchemy>=2.0.5
 databases>=0.4.0
 aiosqlite>=0.16.0
 asyncpg>=0.21.0
 cryptography>=38.0.1
-psycopg2-binary>=2.8.6
+psycopg[binary]>=3.1.18
 PyMySQL>=0.9.0
 aiomysql>=0.0.21
 sqlalchemy-cockroachdb>=2.0.0
 duckdb>=0.9.0
 duckdb-engine>=0.9.2
 wheel>=0.34.2
 setuptools>=63.3.0
```

### Comparing `meerschaum-2.1.7/setup.py` & `meerschaum-2.2.0.dev1/setup.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/tests/test_deduplicate.py` & `meerschaum-2.2.0.dev1/tests/test_deduplicate.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/tests/test_pipes_dtypes.py` & `meerschaum-2.2.0.dev1/tests/test_pipes_dtypes.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/tests/test_sql.py` & `meerschaum-2.2.0.dev1/tests/test_sql.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/tests/test_sync.py` & `meerschaum-2.2.0.dev1/tests/test_sync.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/tests/test_users.py` & `meerschaum-2.2.0.dev1/tests/test_users.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.1.7/tests/test_verify.py` & `meerschaum-2.2.0.dev1/tests/test_verify.py`

 * *Files identical despite different names*

