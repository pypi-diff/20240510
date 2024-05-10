# Comparing `tmp/anvil-app-server-1.8.0.tar.gz` & `tmp/anvil-app-server-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anvil-app-server-1.8.0.tar", last modified: Fri Apr 28 14:19:42 2023, max compression
+gzip compressed data, was "anvil-app-server-1.9.0.tar", last modified: Fri Aug  4 07:58:38 2023, max compression
```

## Comparing `anvil-app-server-1.8.0.tar` & `anvil-app-server-1.9.0.tar`

### file list

```diff
@@ -1,87 +1,90 @@
-drwxrwxr-x   0 meredydd  (1001) meredydd  (1001)        0 2023-04-28 14:19:42.580594 anvil-app-server-1.8.0/
--rw-rw-r--   0 meredydd  (1001) meredydd  (1001)     1121 2023-04-28 14:19:42.580594 anvil-app-server-1.8.0/PKG-INFO
-drwxrwxr-x   0 meredydd  (1001) meredydd  (1001)        0 2023-04-28 14:19:42.576594 anvil-app-server-1.8.0/anvil_app_server/
--rw-rw-r--   0 meredydd  (1001) meredydd  (1001)    10039 2023-04-28 14:16:54.000000 anvil-app-server-1.8.0/anvil_app_server/Blank.zip
--rw-rw-r--   0 meredydd  (1001) meredydd  (1001)    10262 2023-04-28 14:16:54.000000 anvil-app-server-1.8.0/anvil_app_server/Default.zip
--rw-rw-r--   0 meredydd  (1001) meredydd  (1001)    12594 2023-04-28 14:16:54.000000 anvil-app-server-1.8.0/anvil_app_server/TodoList.zip
--rw-rw-r--   0 meredydd  (1001) meredydd  (1001)     7226 2023-04-28 14:16:54.000000 anvil-app-server-1.8.0/anvil_app_server/__init__.py
--rw-rw-r--   0 meredydd  (1001) meredydd  (1001)      742 2021-09-09 17:34:46.000000 anvil-app-server-1.8.0/anvil_app_server/shell.py
-drwxrwxr-x   0 meredydd  (1001) meredydd  (1001)        0 2023-04-28 14:19:42.576594 anvil-app-server-1.8.0/anvil_app_server.egg-info/
--rw-rw-r--   0 meredydd  (1001) meredydd  (1001)     1121 2023-04-28 14:19:42.000000 anvil-app-server-1.8.0/anvil_app_server.egg-info/PKG-INFO
--rw-rw-r--   0 meredydd  (1001) meredydd  (1001)     2847 2023-04-28 14:19:42.000000 anvil-app-server-1.8.0/anvil_app_server.egg-info/SOURCES.txt
--rw-rw-r--   0 meredydd  (1001) meredydd  (1001)        1 2023-04-28 14:19:42.000000 anvil-app-server-1.8.0/anvil_app_server.egg-info/dependency_links.txt
--rw-rw-r--   0 meredydd  (1001) meredydd  (1001)      155 2023-04-28 14:19:42.000000 anvil-app-server-1.8.0/anvil_app_server.egg-info/entry_points.txt
--rw-rw-r--   0 meredydd  (1001) meredydd  (1001)       55 2023-04-28 14:19:42.000000 anvil-app-server-1.8.0/anvil_app_server.egg-info/requires.txt
--rw-rw-r--   0 meredydd  (1001) meredydd  (1001)       79 2023-04-28 14:19:42.000000 anvil-app-server-1.8.0/anvil_app_server.egg-info/top_level.txt
-drwxrwxr-x   0 meredydd  (1001) meredydd  (1001)        0 2023-04-28 14:19:42.576594 anvil-app-server-1.8.0/anvil_downlink_host/
--rw-rw-r--   0 meredydd  (1001) meredydd  (1001)    20028 2023-03-20 13:27:34.000000 anvil-app-server-1.8.0/anvil_downlink_host/__init__.py
--rw-rw-r--   0 meredydd  (1001) meredydd  (1001)    17467 2023-03-20 13:27:34.000000 anvil-app-server-1.8.0/anvil_downlink_host/full_python.py
--rw-rw-r--   0 meredydd  (1001) meredydd  (1001)    15364 2022-06-08 12:52:10.000000 anvil-app-server-1.8.0/anvil_downlink_host/pdf_renderer.py
--rw-rw-r--   0 meredydd  (1001) meredydd  (1001)      100 2021-09-09 17:34:46.000000 anvil-app-server-1.8.0/anvil_downlink_host/run.py
-drwxrwxr-x   0 meredydd  (1001) meredydd  (1001)        0 2023-04-28 14:19:42.576594 anvil-app-server-1.8.0/anvil_downlink_util/
--rw-rw-r--   0 meredydd  (1001) meredydd  (1001)        0 2021-10-08 13:19:20.000000 anvil-app-server-1.8.0/anvil_downlink_util/__init__.py
--rw-rw-r--   0 meredydd  (1001) meredydd  (1001)     1501 2021-10-08 13:19:20.000000 anvil-app-server-1.8.0/anvil_downlink_util/pipes.py
-drwxrwxr-x   0 meredydd  (1001) meredydd  (1001)        0 2023-04-28 14:19:42.576594 anvil-app-server-1.8.0/anvil_downlink_worker/
--rw-rw-r--   0 meredydd  (1001) meredydd  (1001)     8804 2023-03-20 13:27:34.000000 anvil-app-server-1.8.0/anvil_downlink_worker/__init__.py
-drwxrwxr-x   0 meredydd  (1001) meredydd  (1001)        0 2023-04-28 14:19:42.576594 anvil-app-server-1.8.0/anvil_downlink_worker/anvil/
--rw-rw-r--   0 meredydd  (1001) meredydd  (1001)     4684 2022-05-19 09:15:03.000000 anvil-app-server-1.8.0/anvil_downlink_worker/anvil/__init__.py
--rw-rw-r--   0 meredydd  (1001) meredydd  (1001)     2951 2023-04-26 21:52:21.000000 anvil-app-server-1.8.0/anvil_downlink_worker/anvil/_components.py
--rw-rw-r--   0 meredydd  (1001) meredydd  (1001)     4143 2021-09-09 17:34:46.000000 anvil-app-server-1.8.0/anvil_downlink_worker/anvil/_form_templating.py
--rw-rw-r--   0 meredydd  (1001) meredydd  (1001)     4111 2022-04-20 22:17:12.000000 anvil-app-server-1.8.0/anvil_downlink_worker/anvil/_serialise.py
--rw-rw-r--   0 meredydd  (1001) meredydd  (1001)    56083 2023-03-20 13:27:34.000000 anvil-app-server-1.8.0/anvil_downlink_worker/anvil/_server.py
--rw-rw-r--   0 meredydd  (1001) meredydd  (1001)    16093 2023-03-20 13:27:34.000000 anvil-app-server-1.8.0/anvil_downlink_worker/anvil/_threaded_server.py
--rw-rw-r--   0 meredydd  (1001) meredydd  (1001)    10975 2022-05-24 19:01:05.000000 anvil-app-server-1.8.0/anvil_downlink_worker/anvil/email.py
-drwxrwxr-x   0 meredydd  (1001) meredydd  (1001)        0 2023-04-28 14:19:42.576594 anvil-app-server-1.8.0/anvil_downlink_worker/anvil/facebook/
--rw-rw-r--   0 meredydd  (1001) meredydd  (1001)        0 2021-09-09 17:34:46.000000 anvil-app-server-1.8.0/anvil_downlink_worker/anvil/facebook/__init__.py
--rw-rw-r--   0 meredydd  (1001) meredydd  (1001)      421 2021-09-09 17:34:46.000000 anvil-app-server-1.8.0/anvil_downlink_worker/anvil/facebook/auth.py
-drwxrwxr-x   0 meredydd  (1001) meredydd  (1001)        0 2023-04-28 14:19:42.576594 anvil-app-server-1.8.0/anvil_downlink_worker/anvil/files/
--rw-rw-r--   0 meredydd  (1001) meredydd  (1001)    12369 2023-01-03 13:49:28.000000 anvil-app-server-1.8.0/anvil_downlink_worker/anvil/files/__init__.py
-drwxrwxr-x   0 meredydd  (1001) meredydd  (1001)        0 2023-04-28 14:19:42.576594 anvil-app-server-1.8.0/anvil_downlink_worker/anvil/google/
--rw-rw-r--   0 meredydd  (1001) meredydd  (1001)      181 2021-09-09 17:34:46.000000 anvil-app-server-1.8.0/anvil_downlink_worker/anvil/google/__init__.py
--rw-rw-r--   0 meredydd  (1001) meredydd  (1001)      621 2021-09-09 17:34:46.000000 anvil-app-server-1.8.0/anvil_downlink_worker/anvil/google/auth.py
--rw-rw-r--   0 meredydd  (1001) meredydd  (1001)    21821 2023-01-03 13:49:28.000000 anvil-app-server-1.8.0/anvil_downlink_worker/anvil/google/drive.py
--rw-rw-r--   0 meredydd  (1001) meredydd  (1001)     1435 2021-09-09 17:34:46.000000 anvil-app-server-1.8.0/anvil_downlink_worker/anvil/google/mail.py
--rw-rw-r--   0 meredydd  (1001) meredydd  (1001)    13576 2022-12-19 17:36:19.000000 anvil-app-server-1.8.0/anvil_downlink_worker/anvil/google/sheets.py
--rw-rw-r--   0 meredydd  (1001) meredydd  (1001)     4137 2023-04-20 21:39:12.000000 anvil-app-server-1.8.0/anvil_downlink_worker/anvil/http.py
--rw-rw-r--   0 meredydd  (1001) meredydd  (1001)      339 2021-09-09 17:34:46.000000 anvil-app-server-1.8.0/anvil_downlink_worker/anvil/js.py
--rw-rw-r--   0 meredydd  (1001) meredydd  (1001)     1638 2022-12-19 17:36:19.000000 anvil-app-server-1.8.0/anvil_downlink_worker/anvil/media.py
-drwxrwxr-x   0 meredydd  (1001) meredydd  (1001)        0 2023-04-28 14:19:42.576594 anvil-app-server-1.8.0/anvil_downlink_worker/anvil/microsoft/
--rw-rw-r--   0 meredydd  (1001) meredydd  (1001)        0 2021-09-09 17:34:46.000000 anvil-app-server-1.8.0/anvil_downlink_worker/anvil/microsoft/__init__.py
--rw-rw-r--   0 meredydd  (1001) meredydd  (1001)      688 2021-09-09 17:34:46.000000 anvil-app-server-1.8.0/anvil_downlink_worker/anvil/microsoft/auth.py
--rw-rw-r--   0 meredydd  (1001) meredydd  (1001)      693 2023-03-03 12:04:38.000000 anvil-app-server-1.8.0/anvil_downlink_worker/anvil/mpl_util.py
--rw-rw-r--   0 meredydd  (1001) meredydd  (1001)     3512 2023-01-03 13:49:28.000000 anvil-app-server-1.8.0/anvil_downlink_worker/anvil/pdf.py
--rw-rw-r--   0 meredydd  (1001) meredydd  (1001)       86 2021-09-09 17:34:46.000000 anvil-app-server-1.8.0/anvil_downlink_worker/anvil/regex.py
--rw-rw-r--   0 meredydd  (1001) meredydd  (1001)      944 2021-09-09 17:34:46.000000 anvil-app-server-1.8.0/anvil_downlink_worker/anvil/secrets.py
--rw-rw-r--   0 meredydd  (1001) meredydd  (1001)    10549 2023-02-06 10:21:14.000000 anvil-app-server-1.8.0/anvil_downlink_worker/anvil/server.py
--rw-rw-r--   0 meredydd  (1001) meredydd  (1001)     2075 2021-09-09 17:34:46.000000 anvil-app-server-1.8.0/anvil_downlink_worker/anvil/stripe.py
-drwxrwxr-x   0 meredydd  (1001) meredydd  (1001)        0 2023-04-28 14:19:42.580594 anvil-app-server-1.8.0/anvil_downlink_worker/anvil/tables/
--rw-rw-r--   0 meredydd  (1001) meredydd  (1001)     9866 2023-04-12 13:59:51.000000 anvil-app-server-1.8.0/anvil_downlink_worker/anvil/tables/__init__.py
--rw-rw-r--   0 meredydd  (1001) meredydd  (1001)      898 2022-05-19 09:15:03.000000 anvil-app-server-1.8.0/anvil_downlink_worker/anvil/tables/_base_classes.py
--rw-rw-r--   0 meredydd  (1001) meredydd  (1001)      308 2022-12-21 14:53:30.000000 anvil-app-server-1.8.0/anvil_downlink_worker/anvil/tables/_config.py
--rw-rw-r--   0 meredydd  (1001) meredydd  (1001)     1039 2022-12-19 17:40:31.000000 anvil-app-server-1.8.0/anvil_downlink_worker/anvil/tables/_errors.py
--rw-rw-r--   0 meredydd  (1001) meredydd  (1001)      428 2022-04-20 22:17:12.000000 anvil-app-server-1.8.0/anvil_downlink_worker/anvil/tables/_helpers.py
--rw-rw-r--   0 meredydd  (1001) meredydd  (1001)     5160 2022-06-19 19:43:30.000000 anvil-app-server-1.8.0/anvil_downlink_worker/anvil/tables/query.py
-drwxrwxr-x   0 meredydd  (1001) meredydd  (1001)        0 2023-04-28 14:19:42.580594 anvil-app-server-1.8.0/anvil_downlink_worker/anvil/tables/v2/
--rw-rw-r--   0 meredydd  (1001) meredydd  (1001)      231 2022-05-19 09:15:03.000000 anvil-app-server-1.8.0/anvil_downlink_worker/anvil/tables/v2/__init__.py
--rw-rw-r--   0 meredydd  (1001) meredydd  (1001)     1183 2022-04-20 22:17:12.000000 anvil-app-server-1.8.0/anvil_downlink_worker/anvil/tables/v2/_app_tables.py
--rw-rw-r--   0 meredydd  (1001) meredydd  (1001)     2105 2022-12-21 14:53:30.000000 anvil-app-server-1.8.0/anvil_downlink_worker/anvil/tables/v2/_batcher.py
--rw-rw-r--   0 meredydd  (1001) meredydd  (1001)      845 2022-04-20 22:17:12.000000 anvil-app-server-1.8.0/anvil_downlink_worker/anvil/tables/v2/_constants.py
--rw-rw-r--   0 meredydd  (1001) meredydd  (1001)      284 2022-05-19 09:15:03.000000 anvil-app-server-1.8.0/anvil_downlink_worker/anvil/tables/v2/_load_hacks.py
--rw-rw-r--   0 meredydd  (1001) meredydd  (1001)     1211 2022-04-20 22:17:12.000000 anvil-app-server-1.8.0/anvil_downlink_worker/anvil/tables/v2/_refs.py
--rw-rw-r--   0 meredydd  (1001) meredydd  (1001)    20172 2023-03-20 13:27:34.000000 anvil-app-server-1.8.0/anvil_downlink_worker/anvil/tables/v2/_row.py
--rw-rw-r--   0 meredydd  (1001) meredydd  (1001)     9520 2023-04-12 13:59:51.000000 anvil-app-server-1.8.0/anvil_downlink_worker/anvil/tables/v2/_search.py
--rw-rw-r--   0 meredydd  (1001) meredydd  (1001)     4398 2023-04-12 13:59:51.000000 anvil-app-server-1.8.0/anvil_downlink_worker/anvil/tables/v2/_table.py
--rw-rw-r--   0 meredydd  (1001) meredydd  (1001)     4668 2022-12-21 14:53:30.000000 anvil-app-server-1.8.0/anvil_downlink_worker/anvil/tables/v2/_utils.py
--rw-rw-r--   0 meredydd  (1001) meredydd  (1001)     1964 2022-12-21 14:53:30.000000 anvil-app-server-1.8.0/anvil_downlink_worker/anvil/tz.py
-drwxrwxr-x   0 meredydd  (1001) meredydd  (1001)        0 2023-04-28 14:19:42.580594 anvil-app-server-1.8.0/anvil_downlink_worker/anvil/users/
--rw-rw-r--   0 meredydd  (1001) meredydd  (1001)    39409 2022-12-21 14:53:30.000000 anvil-app-server-1.8.0/anvil_downlink_worker/anvil/users/__init__.py
--rw-rw-r--   0 meredydd  (1001) meredydd  (1001)      205 2021-09-09 17:34:46.000000 anvil-app-server-1.8.0/anvil_downlink_worker/anvil/users/config.py
--rw-rw-r--   0 meredydd  (1001) meredydd  (1001)      979 2022-04-20 22:17:12.000000 anvil-app-server-1.8.0/anvil_downlink_worker/anvil/users/exceptions.py
-drwxrwxr-x   0 meredydd  (1001) meredydd  (1001)        0 2023-04-28 14:19:42.580594 anvil-app-server-1.8.0/anvil_downlink_worker/anvil/users/mfa/
--rw-rw-r--   0 meredydd  (1001) meredydd  (1001)    18907 2022-12-21 14:53:30.000000 anvil-app-server-1.8.0/anvil_downlink_worker/anvil/users/mfa/__init__.py
--rw-rw-r--   0 meredydd  (1001) meredydd  (1001)     2525 2021-09-09 17:34:46.000000 anvil-app-server-1.8.0/anvil_downlink_worker/anvil/util.py
--rw-rw-r--   0 meredydd  (1001) meredydd  (1001)       49 2021-09-09 17:34:46.000000 anvil-app-server-1.8.0/anvil_downlink_worker/exec2.py
--rw-rw-r--   0 meredydd  (1001) meredydd  (1001)       15 2021-09-09 17:34:46.000000 anvil-app-server-1.8.0/anvil_downlink_worker/exec3.py
--rw-rw-r--   0 meredydd  (1001) meredydd  (1001)     3464 2023-03-20 13:27:34.000000 anvil-app-server-1.8.0/anvil_downlink_worker/full_python_worker.py
--rw-rw-r--   0 meredydd  (1001) meredydd  (1001)       38 2023-04-28 14:19:42.580594 anvil-app-server-1.8.0/setup.cfg
--rw-rw-r--   0 meredydd  (1001) meredydd  (1001)     1812 2023-04-28 14:16:54.000000 anvil-app-server-1.8.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-04 07:58:38.082934 anvil-app-server-1.9.0/
+-rw-rw-rw-   0        0        0     1056 2023-08-04 07:58:38.082434 anvil-app-server-1.9.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-04 07:58:38.022934 anvil-app-server-1.9.0/anvil_app_server/
+-rw-rw-rw-   0        0        0    11288 2023-08-04 07:57:31.000000 anvil-app-server-1.9.0/anvil_app_server/Blank.zip
+-rw-rw-rw-   0        0        0    11511 2023-08-04 07:57:31.000000 anvil-app-server-1.9.0/anvil_app_server/Default.zip
+-rw-rw-rw-   0        0        0    14110 2023-08-04 07:57:31.000000 anvil-app-server-1.9.0/anvil_app_server/TodoList.zip
+-rw-rw-rw-   0        0        0     7226 2023-08-04 07:57:32.000000 anvil-app-server-1.9.0/anvil_app_server/__init__.py
+-rw-rw-rw-   0        0        0      742 2021-09-11 17:26:20.000000 anvil-app-server-1.9.0/anvil_app_server/shell.py
+drwxrwxrwx   0        0        0        0 2023-08-04 07:58:38.028433 anvil-app-server-1.9.0/anvil_app_server.egg-info/
+-rw-rw-rw-   0        0        0     1056 2023-08-04 07:58:37.000000 anvil-app-server-1.9.0/anvil_app_server.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2945 2023-08-04 07:58:37.000000 anvil-app-server-1.9.0/anvil_app_server.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-04 07:58:37.000000 anvil-app-server-1.9.0/anvil_app_server.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      155 2023-08-04 07:58:37.000000 anvil-app-server-1.9.0/anvil_app_server.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       55 2023-08-04 07:58:37.000000 anvil-app-server-1.9.0/anvil_app_server.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       79 2023-08-04 07:58:37.000000 anvil-app-server-1.9.0/anvil_app_server.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-04 07:58:38.031933 anvil-app-server-1.9.0/anvil_downlink_host/
+-rw-rw-rw-   0        0        0    20573 2023-03-13 10:17:14.000000 anvil-app-server-1.9.0/anvil_downlink_host/__init__.py
+-rw-rw-rw-   0        0        0    17853 2023-03-13 10:17:14.000000 anvil-app-server-1.9.0/anvil_downlink_host/full_python.py
+-rw-rw-rw-   0        0        0    15364 2022-06-04 12:27:29.000000 anvil-app-server-1.9.0/anvil_downlink_host/pdf_renderer.py
+-rw-rw-rw-   0        0        0      100 2021-09-11 17:26:20.000000 anvil-app-server-1.9.0/anvil_downlink_host/run.py
+drwxrwxrwx   0        0        0        0 2023-08-04 07:58:38.033934 anvil-app-server-1.9.0/anvil_downlink_util/
+-rw-rw-rw-   0        0        0        0 2021-10-06 18:58:46.000000 anvil-app-server-1.9.0/anvil_downlink_util/__init__.py
+-rw-rw-rw-   0        0        0     1501 2021-10-06 18:58:46.000000 anvil-app-server-1.9.0/anvil_downlink_util/pipes.py
+drwxrwxrwx   0        0        0        0 2023-08-04 07:58:38.037435 anvil-app-server-1.9.0/anvil_downlink_worker/
+-rw-rw-rw-   0        0        0     9057 2023-03-13 10:17:14.000000 anvil-app-server-1.9.0/anvil_downlink_worker/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-04 07:58:38.053433 anvil-app-server-1.9.0/anvil_downlink_worker/anvil/
+-rw-rw-rw-   0        0        0     4684 2023-07-10 08:37:03.000000 anvil-app-server-1.9.0/anvil_downlink_worker/anvil/__init__.py
+-rw-rw-rw-   0        0        0     2951 2023-08-02 10:34:24.000000 anvil-app-server-1.9.0/anvil_downlink_worker/anvil/_components.py
+-rw-rw-rw-   0        0        0     4143 2021-09-11 17:26:20.000000 anvil-app-server-1.9.0/anvil_downlink_worker/anvil/_form_templating.py
+-rw-rw-rw-   0        0        0     4111 2022-04-02 09:11:16.000000 anvil-app-server-1.9.0/anvil_downlink_worker/anvil/_serialise.py
+-rw-rw-rw-   0        0        0    57693 2023-05-10 18:01:10.000000 anvil-app-server-1.9.0/anvil_downlink_worker/anvil/_server.py
+-rw-rw-rw-   0        0        0    16530 2023-03-13 10:17:14.000000 anvil-app-server-1.9.0/anvil_downlink_worker/anvil/_threaded_server.py
+-rw-rw-rw-   0        0        0    10975 2022-05-29 12:40:51.000000 anvil-app-server-1.9.0/anvil_downlink_worker/anvil/email.py
+drwxrwxrwx   0        0        0        0 2023-08-04 07:58:38.054933 anvil-app-server-1.9.0/anvil_downlink_worker/anvil/ext_tables/
+-rw-rw-rw-   0        0        0       50 2023-07-31 21:23:38.000000 anvil-app-server-1.9.0/anvil_downlink_worker/anvil/ext_tables/__init__.py
+-rw-rw-rw-   0        0        0     5829 2023-07-31 21:23:38.000000 anvil-app-server-1.9.0/anvil_downlink_worker/anvil/ext_tables/impl.py
+drwxrwxrwx   0        0        0        0 2023-08-04 07:58:38.056933 anvil-app-server-1.9.0/anvil_downlink_worker/anvil/facebook/
+-rw-rw-rw-   0        0        0        0 2021-09-11 17:26:20.000000 anvil-app-server-1.9.0/anvil_downlink_worker/anvil/facebook/__init__.py
+-rw-rw-rw-   0        0        0      421 2021-09-11 17:26:20.000000 anvil-app-server-1.9.0/anvil_downlink_worker/anvil/facebook/auth.py
+drwxrwxrwx   0        0        0        0 2023-08-04 07:58:38.057433 anvil-app-server-1.9.0/anvil_downlink_worker/anvil/files/
+-rw-rw-rw-   0        0        0    12369 2022-12-12 10:47:47.000000 anvil-app-server-1.9.0/anvil_downlink_worker/anvil/files/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-04 07:58:38.061933 anvil-app-server-1.9.0/anvil_downlink_worker/anvil/google/
+-rw-rw-rw-   0        0        0      181 2021-09-11 17:26:20.000000 anvil-app-server-1.9.0/anvil_downlink_worker/anvil/google/__init__.py
+-rw-rw-rw-   0        0        0      621 2021-09-11 17:26:20.000000 anvil-app-server-1.9.0/anvil_downlink_worker/anvil/google/auth.py
+-rw-rw-rw-   0        0        0    21821 2022-12-12 10:47:47.000000 anvil-app-server-1.9.0/anvil_downlink_worker/anvil/google/drive.py
+-rw-rw-rw-   0        0        0     1435 2021-09-11 17:26:20.000000 anvil-app-server-1.9.0/anvil_downlink_worker/anvil/google/mail.py
+-rw-rw-rw-   0        0        0    13576 2022-11-11 17:50:27.000000 anvil-app-server-1.9.0/anvil_downlink_worker/anvil/google/sheets.py
+-rw-rw-rw-   0        0        0     4237 2023-07-31 21:23:38.000000 anvil-app-server-1.9.0/anvil_downlink_worker/anvil/http.py
+-rw-rw-rw-   0        0        0      339 2021-09-11 17:26:20.000000 anvil-app-server-1.9.0/anvil_downlink_worker/anvil/js.py
+-rw-rw-rw-   0        0        0     1638 2022-08-25 20:59:10.000000 anvil-app-server-1.9.0/anvil_downlink_worker/anvil/media.py
+drwxrwxrwx   0        0        0        0 2023-08-04 07:58:38.063434 anvil-app-server-1.9.0/anvil_downlink_worker/anvil/microsoft/
+-rw-rw-rw-   0        0        0        0 2021-09-11 17:26:20.000000 anvil-app-server-1.9.0/anvil_downlink_worker/anvil/microsoft/__init__.py
+-rw-rw-rw-   0        0        0      688 2021-09-11 17:26:20.000000 anvil-app-server-1.9.0/anvil_downlink_worker/anvil/microsoft/auth.py
+-rw-rw-rw-   0        0        0      704 2023-05-10 18:01:10.000000 anvil-app-server-1.9.0/anvil_downlink_worker/anvil/mpl_util.py
+-rw-rw-rw-   0        0        0     3512 2022-12-12 10:47:47.000000 anvil-app-server-1.9.0/anvil_downlink_worker/anvil/pdf.py
+-rw-rw-rw-   0        0        0       86 2021-09-11 17:26:20.000000 anvil-app-server-1.9.0/anvil_downlink_worker/anvil/regex.py
+-rw-rw-rw-   0        0        0      944 2021-09-11 17:26:20.000000 anvil-app-server-1.9.0/anvil_downlink_worker/anvil/secrets.py
+-rw-rw-rw-   0        0        0    10549 2023-02-12 18:45:17.000000 anvil-app-server-1.9.0/anvil_downlink_worker/anvil/server.py
+-rw-rw-rw-   0        0        0     2075 2021-09-11 17:26:20.000000 anvil-app-server-1.9.0/anvil_downlink_worker/anvil/stripe.py
+drwxrwxrwx   0        0        0        0 2023-08-04 07:58:38.068934 anvil-app-server-1.9.0/anvil_downlink_worker/anvil/tables/
+-rw-rw-rw-   0        0        0    10676 2023-07-31 21:23:38.000000 anvil-app-server-1.9.0/anvil_downlink_worker/anvil/tables/__init__.py
+-rw-rw-rw-   0        0        0      898 2022-05-29 12:40:51.000000 anvil-app-server-1.9.0/anvil_downlink_worker/anvil/tables/_base_classes.py
+-rw-rw-rw-   0        0        0      308 2022-11-30 15:07:00.000000 anvil-app-server-1.9.0/anvil_downlink_worker/anvil/tables/_config.py
+-rw-rw-rw-   0        0        0     1039 2022-05-29 12:40:51.000000 anvil-app-server-1.9.0/anvil_downlink_worker/anvil/tables/_errors.py
+-rw-rw-rw-   0        0        0      428 2022-04-02 09:11:16.000000 anvil-app-server-1.9.0/anvil_downlink_worker/anvil/tables/_helpers.py
+-rw-rw-rw-   0        0        0     5160 2022-06-18 09:41:33.000000 anvil-app-server-1.9.0/anvil_downlink_worker/anvil/tables/query.py
+drwxrwxrwx   0        0        0        0 2023-08-04 07:58:38.077934 anvil-app-server-1.9.0/anvil_downlink_worker/anvil/tables/v2/
+-rw-rw-rw-   0        0        0      231 2022-05-29 12:40:51.000000 anvil-app-server-1.9.0/anvil_downlink_worker/anvil/tables/v2/__init__.py
+-rw-rw-rw-   0        0        0     1593 2023-07-31 21:23:38.000000 anvil-app-server-1.9.0/anvil_downlink_worker/anvil/tables/v2/_app_tables.py
+-rw-rw-rw-   0        0        0     2105 2022-11-30 15:07:00.000000 anvil-app-server-1.9.0/anvil_downlink_worker/anvil/tables/v2/_batcher.py
+-rw-rw-rw-   0        0        0      845 2022-04-02 09:11:16.000000 anvil-app-server-1.9.0/anvil_downlink_worker/anvil/tables/v2/_constants.py
+-rw-rw-rw-   0        0        0      284 2022-05-29 12:40:51.000000 anvil-app-server-1.9.0/anvil_downlink_worker/anvil/tables/v2/_load_hacks.py
+-rw-rw-rw-   0        0        0     1211 2022-04-02 09:11:16.000000 anvil-app-server-1.9.0/anvil_downlink_worker/anvil/tables/v2/_refs.py
+-rw-rw-rw-   0        0        0    20690 2023-05-10 18:01:11.000000 anvil-app-server-1.9.0/anvil_downlink_worker/anvil/tables/v2/_row.py
+-rw-rw-rw-   0        0        0     9779 2023-05-10 18:01:11.000000 anvil-app-server-1.9.0/anvil_downlink_worker/anvil/tables/v2/_search.py
+-rw-rw-rw-   0        0        0     4518 2023-05-10 18:01:11.000000 anvil-app-server-1.9.0/anvil_downlink_worker/anvil/tables/v2/_table.py
+-rw-rw-rw-   0        0        0     4809 2023-07-31 21:23:38.000000 anvil-app-server-1.9.0/anvil_downlink_worker/anvil/tables/v2/_utils.py
+-rw-rw-rw-   0        0        0     1964 2022-11-11 17:50:27.000000 anvil-app-server-1.9.0/anvil_downlink_worker/anvil/tz.py
+drwxrwxrwx   0        0        0        0 2023-08-04 07:58:38.080434 anvil-app-server-1.9.0/anvil_downlink_worker/anvil/users/
+-rw-rw-rw-   0        0        0    39409 2022-11-30 15:07:00.000000 anvil-app-server-1.9.0/anvil_downlink_worker/anvil/users/__init__.py
+-rw-rw-rw-   0        0        0      205 2021-09-11 17:26:20.000000 anvil-app-server-1.9.0/anvil_downlink_worker/anvil/users/config.py
+-rw-rw-rw-   0        0        0      979 2022-04-02 09:09:48.000000 anvil-app-server-1.9.0/anvil_downlink_worker/anvil/users/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-08-04 07:58:38.081434 anvil-app-server-1.9.0/anvil_downlink_worker/anvil/users/mfa/
+-rw-rw-rw-   0        0        0    18907 2022-12-12 10:47:47.000000 anvil-app-server-1.9.0/anvil_downlink_worker/anvil/users/mfa/__init__.py
+-rw-rw-rw-   0        0        0     2525 2021-09-11 17:26:19.000000 anvil-app-server-1.9.0/anvil_downlink_worker/anvil/util.py
+-rw-rw-rw-   0        0        0       49 2021-09-11 17:26:20.000000 anvil-app-server-1.9.0/anvil_downlink_worker/exec2.py
+-rw-rw-rw-   0        0        0       15 2021-09-11 17:26:20.000000 anvil-app-server-1.9.0/anvil_downlink_worker/exec3.py
+-rw-rw-rw-   0        0        0     3556 2023-03-13 10:17:14.000000 anvil-app-server-1.9.0/anvil_downlink_worker/full_python_worker.py
+-rw-rw-rw-   0        0        0       42 2023-08-04 07:58:38.082934 anvil-app-server-1.9.0/setup.cfg
+-rw-rw-rw-   0        0        0     1812 2023-08-04 07:57:31.000000 anvil-app-server-1.9.0/setup.py
```

### Comparing `anvil-app-server-1.8.0/PKG-INFO` & `anvil-app-server-1.9.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,47 @@
-Metadata-Version: 2.1
-Name: anvil-app-server
-Version: 1.8.0
-Summary: A standalone server for Anvil full-stack Python web apps
-Home-page: https://anvil.works
-Author: Anvil
-Author-email: contact@anvil.works
-License: GNU Affero General Public License v3
-Project-URL: Source Code, https://github.com/anvil-works/anvil-runtime
-Description: 
-        ## A standalone server for Anvil full-stack Python web apps.
-        
-        This package includes several assets, some not in Python:
-         - The "anvil-standalone-runtime" script for launching the runtime
-         - The "downlink" Python code for the server-side parts of apps
-         - The core Anvil server (requires Java to launch)
-         - The client-side Anvil runtime (Javascript, using the Skulpt Python-to-JS compiler)
-        
-        Head over to [the Github Repository](https://github.com/anvil-works/anvil-runtime) for usage instructions, and to learn more.
-            
-Keywords: anvil web apps standalone browser Python
-Platform: UNKNOWN
-Classifier: License :: OSI Approved :: GNU Affero General Public License v3
-Description-Content-Type: text/markdown
+from setuptools import setup,find_packages
+setup(
+    name="anvil-app-server",
+    version="1.9.0",
+    packages=find_packages(),
+    install_requires=["pychrome", "anvil-uplink==0.4.2", "progressbar2", "wheel", "psutil"],
+
+    # Include the App Server JAR directly in this debug build of the package. That way the release version won't be downloaded on first run.
+    package_data={
+        "anvil_app_server": [
+            "TodoList.zip",
+            "Default.zip",
+            "Blank.zip"
+        ] 
+    },
+
+    author="Anvil",
+    author_email="contact@anvil.works",
+    description="A standalone server for Anvil full-stack Python web apps",
+    long_description="""
+## A standalone server for Anvil full-stack Python web apps.
+
+This package includes several assets, some not in Python:
+ - The "anvil-standalone-runtime" script for launching the runtime
+ - The "downlink" Python code for the server-side parts of apps
+ - The core Anvil server (requires Java to launch)
+ - The client-side Anvil runtime (Javascript, using the Skulpt Python-to-JS compiler)
+
+Head over to [the Github Repository](https://github.com/anvil-works/anvil-runtime) for usage instructions, and to learn more.
+    """,
+    long_description_content_type="text/markdown",
+    keywords="anvil web apps standalone browser Python",
+    url="https://anvil.works",
+    license="GNU Affero General Public License v3",
+    project_urls={
+        "Source Code": "https://github.com/anvil-works/anvil-runtime"
+    },
+    classifiers=[
+        "License :: OSI Approved :: GNU Affero General Public License v3"
+    ],
+    entry_points = {
+        "console_scripts": [
+        "anvil-app-server=anvil_app_server:launch",
+        "psql-anvil-app-server=anvil_app_server:psql",
+        "create-anvil-app=anvil_app_server:create_app"
+        ]
+    })
```

### Comparing `anvil-app-server-1.8.0/anvil_app_server/__init__.py` & `anvil-app-server-1.9.0/anvil_app_server/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,15 +140,15 @@
         print("psql 'host=localhost port={} user=postgres dbname=postgres options=--search-path=app_tables'".format(port))
         os.system("psql 'host=localhost port={} user=postgres dbname=postgres options=--search-path=app_tables'".format(port))
 
 
 def find_or_download_app_server(): # Work out whether we already have the server JAR file. It could be in the package itself, or in ~/.anvil
     package_dir = os.path.dirname(__file__)
     home_dir = os.path.expanduser("~")
-    server_jar_name = "anvil-app-server.20230428-151654.jar"
+    server_jar_name = "anvil-app-server.20230804-085732.jar"
 
     package_dir_path = os.path.join(package_dir, server_jar_name)
     home_dir_path = os.path.join(home_dir, ".anvil", server_jar_name)
 
     if os.path.isfile(package_dir_path):
         print("Found Anvil App Server JAR in package directory")
         return package_dir_path
```

### Comparing `anvil-app-server-1.8.0/anvil_app_server/shell.py` & `anvil-app-server-1.9.0/anvil_app_server/shell.py`

 * *Files identical despite different names*

### Comparing `anvil-app-server-1.8.0/anvil_app_server.egg-info/PKG-INFO` & `anvil-app-server-1.9.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,26 @@
-Metadata-Version: 2.1
-Name: anvil-app-server
-Version: 1.8.0
-Summary: A standalone server for Anvil full-stack Python web apps
-Home-page: https://anvil.works
-Author: Anvil
-Author-email: contact@anvil.works
-License: GNU Affero General Public License v3
-Project-URL: Source Code, https://github.com/anvil-works/anvil-runtime
-Description: 
-        ## A standalone server for Anvil full-stack Python web apps.
-        
-        This package includes several assets, some not in Python:
-         - The "anvil-standalone-runtime" script for launching the runtime
-         - The "downlink" Python code for the server-side parts of apps
-         - The core Anvil server (requires Java to launch)
-         - The client-side Anvil runtime (Javascript, using the Skulpt Python-to-JS compiler)
-        
-        Head over to [the Github Repository](https://github.com/anvil-works/anvil-runtime) for usage instructions, and to learn more.
-            
-Keywords: anvil web apps standalone browser Python
-Platform: UNKNOWN
-Classifier: License :: OSI Approved :: GNU Affero General Public License v3
-Description-Content-Type: text/markdown
+Metadata-Version: 2.1
+Name: anvil-app-server
+Version: 1.9.0
+Summary: A standalone server for Anvil full-stack Python web apps
+Home-page: https://anvil.works
+Author: Anvil
+Author-email: contact@anvil.works
+License: GNU Affero General Public License v3
+Project-URL: Source Code, https://github.com/anvil-works/anvil-runtime
+Keywords: anvil web apps standalone browser Python
+Platform: UNKNOWN
+Classifier: License :: OSI Approved :: GNU Affero General Public License v3
+Description-Content-Type: text/markdown
+
+
+## A standalone server for Anvil full-stack Python web apps.
+
+This package includes several assets, some not in Python:
+ - The "anvil-standalone-runtime" script for launching the runtime
+ - The "downlink" Python code for the server-side parts of apps
+ - The core Anvil server (requires Java to launch)
+ - The client-side Anvil runtime (Javascript, using the Skulpt Python-to-JS compiler)
+
+Head over to [the Github Repository](https://github.com/anvil-works/anvil-runtime) for usage instructions, and to learn more.
+    
+
```

### Comparing `anvil-app-server-1.8.0/anvil_app_server.egg-info/SOURCES.txt` & `anvil-app-server-1.9.0/anvil_app_server.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,16 @@
 anvil_downlink_worker/anvil/pdf.py
 anvil_downlink_worker/anvil/regex.py
 anvil_downlink_worker/anvil/secrets.py
 anvil_downlink_worker/anvil/server.py
 anvil_downlink_worker/anvil/stripe.py
 anvil_downlink_worker/anvil/tz.py
 anvil_downlink_worker/anvil/util.py
+anvil_downlink_worker/anvil/ext_tables/__init__.py
+anvil_downlink_worker/anvil/ext_tables/impl.py
 anvil_downlink_worker/anvil/facebook/__init__.py
 anvil_downlink_worker/anvil/facebook/auth.py
 anvil_downlink_worker/anvil/files/__init__.py
 anvil_downlink_worker/anvil/google/__init__.py
 anvil_downlink_worker/anvil/google/auth.py
 anvil_downlink_worker/anvil/google/drive.py
 anvil_downlink_worker/anvil/google/mail.py
```

### Comparing `anvil-app-server-1.8.0/anvil_downlink_host/__init__.py` & `anvil-app-server-1.9.0/anvil_downlink_host/__init__.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,545 +1,545 @@
-import collections, json, os, psutil, random, signal, subprocess, sys, threading, time, traceback, platform
-from ws4py.client.threadedclient import WebSocketClient
-
-
-# Configuration
-
-TIMEOUT = int(os.environ.get("DOWNLINK_WORKER_TIMEOUT", "30"))
-KEEPALIVE_TIMEOUT = int(os.environ.get("DOWNLINK_KEEPALIVE_TIMEOUT", "30"))
-DROP_PRIVILEGES = os.environ.get("DROP_PRIVILEGES")
-RUNTIME_ID = os.environ.get("RUNTIME_ID", None) or ('python2-full' if sys.version_info[0] < 3 else 'python3-full')
-USER_ID = os.environ.get("DOWNLINK_USER_ID", None)
-ORG_ID = os.environ.get("DOWNLINK_ORG_ID", None)
-ENV_ID = os.environ.get("DOWNLINK_ENV_ID", None)
-SPEC_HASH = os.environ.get("DOWNLINK_SPEC_HASH", None)
-APP_CACHE_SIZE = int(os.environ.get("APP_CACHE_SIZE", "16"))
-ENABLE_PDF_RENDER = os.environ.get("ENABLE_PDF_RENDER")
-PER_WORKER_SOFT_MEMORY_LIMIT = int(os.environ["PER_WORKER_SOFT_MEMORY_LIMIT_MB"])*1024*1024 \
-                                    if "PER_WORKER_SOFT_MEMORY_LIMIT_MB" in os.environ else None
-IDLE_TIMEOUT_SECONDS = int(os.environ.get("IDLE_TIMEOUT_SECONDS","0"))
-
-IS_WINDOWS = "Windows" in platform.system() or "CYGWIN" in platform.system()
-
-for V in ["DOWNLINK_WORKER_TIMEOUT", "DROP_PRIVILEGES", "RUNTIME_ID", "DOWNLINK_USER_ID", "DOWNLINK_ORG_ID", "APP_CACHE_SIZE", "ENABLE_PDF_RENDER"]:
-    if V in os.environ:
-        del os.environ[V]
-
-# Worker modules register themselves here
-workers_by_id = {}
-
-# Cache app content
-app_cache = collections.OrderedDict()
-
-
-def send_with_header(json_data, blob=None):
-    """"Send data to the API router"""
-    connection.send_with_header(json_data, blob)
-
-# Host state
-
-launch_worker = None
-launch_pdf_worker = None
-
-connection = None
-
-rnd = random.SystemRandom()
-MY_SESSION_ID = "".join((rnd.choice("abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789") for _ in range(20)))
-
-draining_start_time = None
-
-
-def is_idle():
-    return len(workers_by_id) == 0
-
-
-def maybe_quit_if_draining_and_done():
-    if draining_start_time is not None and is_idle():
-        if time.time() < draining_start_time + 10:
-            print("Giving API 10 seconds' grace for drain...")
-            def f():
-                time.sleep(draining_start_time + 10 - time.time())
-                maybe_quit_if_draining_and_done()
-            threading.Thread(target=f).start()
-        else:
-            print("Drain complete. Exiting.")
-            os._exit(0)
-
-
-# Utility functions
-
-def get_demote_fn(app_id):
-    if os.name == "nt":
-        return None
-
-    # TODO: Use app_id here to seed UID generation. It might be an actual app ID, or None
-    uid = 20000
-    def do_demotion():
-        if DROP_PRIVILEGES and os.getuid() == 0:
-            os.setgroups([])
-            os.setgid(uid)
-            os.setegid(uid)
-            os.setuid(uid)
-            os.seteuid(uid)
-
-        # Give ourselves an isolated process group so we can take child processes with us when we go
-        os.setpgid(0, 0)
-
-    return do_demotion
-
-
-class PopenWithGroupKill(subprocess.Popen):
-    def terminate(self):
-        try:
-            os.killpg(self.pid, 9)
-        except:
-            pass
-        super(PopenWithGroupKill, self).terminate()
-
-
-# Handle communication with API router
-class Connection(WebSocketClient):
-    def __init__(self, url, key):
-        print("Connecting to " + url)
-        WebSocketClient.__init__(self, url)
-
-        self._sending_lock = threading.RLock()
-        self._send_next_bin = None
-        self._key = key
-        self._last_keepalive_reply = time.time()
-        self._last_activity = time.time()
-        self._idle_timeout_timer = None
-
-        threading.Timer(30, self.check_keepalives).start()
-
-    def record_activity(self):
-        self._last_activity = time.time()
-
-    def reset_idle_timer(self):
-        if self._idle_timeout_timer:
-            self._idle_timeout_timer.cancel()
-        if IDLE_TIMEOUT_SECONDS:
-            self._idle_timeout_timer = threading.Timer(IDLE_TIMEOUT_SECONDS, self.idle_timeout).start()
-
-    def idle_timeout(self):
-        if is_idle() and self._last_activity < time.time() - IDLE_TIMEOUT_SECONDS:
-            print("Idle timeout")
-            signal_drain()
-        else:
-            self.reset_idle_timer()
-
-    def check_keepalives(self):
-        if time.time() - self._last_keepalive_reply > KEEPALIVE_TIMEOUT:
-            print("No keepalive reply in %s seconds. Exiting." % KEEPALIVE_TIMEOUT)
-            os._exit(1)
-        else:
-            threading.Timer(30, self.check_keepalives).start()
-
-    def opened(self):
-        print("Anvil websocket open")
-        self.record_activity()
-        spec = {
-            'runtime': RUNTIME_ID,
-            'session_id': MY_SESSION_ID,
-        }
-
-        if USER_ID is not None:
-            spec['user_id'] = USER_ID
-        elif ORG_ID is not None:
-            spec['org_id'] = ORG_ID
-        elif ENV_ID is not None:
-            spec['env_id'] = ENV_ID
-            spec['spec_hash'] = SPEC_HASH
-
-        id = os.environ.get("DOWNLINK_ID", None)
-        if id:
-            spec['id'] = id
-        self.send(json.dumps({
-            'key': self._key,
-            'v': 2,
-            'spec': spec,
-        }))
-
-    def closed(self, code, reason=None):
-        print("Anvil websocket closed (code %s, reason=%s)" % (code, reason))
-        # The world has ended. Let whatever is in charge of restarting us sort it out.
-        os._exit(1)
-
-    def received_message(self, message):
-        try:
-            self._received_message(message)
-        except Exception as e:
-            print("Error in received_message():")
-            traceback.print_exc()
-            raise
-
-    def _received_message(self, message):
-
-        if message.is_binary:
-            self._send_next_bin(message.data)
-
-        else:
-            data = json.loads(message.data.decode())
-
-            type = data["type"] if 'type' in data else None
-            id = data["id"] if 'id' in data else None
-            is_keepalive = id and id.startswith("downlink-keepalive")
-
-            if not is_keepalive:
-                self.record_activity()
-
-            if 'auth' in data:
-                print("Downlink authenticated OK")
-                self.reset_idle_timer()
-
-            elif 'output' in data:
-                # Output from something this worker has called.
-                calling_worker = workers_by_id.get(data.get('id'))
-                originating_call = calling_worker.outbound_ids.get(id) if calling_worker is not None else None
-
-                if originating_call is not None:
-                    data['id'] = originating_call
-                    self.send_with_header(data)
-                else:
-                    print("Bogus output, probably for an old request (worker: %s): %s" %
-                          ("FOUND" if calling_worker else "MISSING", repr(data)[:100]))
-
-            elif type in ["CALL_WITH_APP", "LAUNCH_BACKGROUND_WITH_APP", "CALL", "LAUNCH_BACKGROUND", "LAUNCH_REPL"]:
-
-                if "app" not in data:
-                    cached_app = app_cache.get((data["app-id"], data["app-version"]))
-                    if cached_app is not None:
-                        #print("Filling out app from cache for %s" % ((data["app-id"], data["app-version"]),))
-                        data["type"] += "_WITH_APP"
-                        data["app"] = cached_app
-
-                #print "Launching new worker for ID " + id
-                if draining_start_time:
-                    self.send_with_header({"id": id, "error": {"type": "anvil.server.DownlinkDrainingError", "message": "New call routed to draining downlink"}})
-                else:
-                    if data.get("command", None) == "anvil.private.pdf.do_print":
-                        if launch_pdf_worker:
-                            launch_pdf_worker(data)
-                        else:
-                            self.send_with_header({"id": id, "error": {"type": "anvil.server.RuntimeUnavailableError", "message": "PDF Rendering unavailable"}})
-                    else:
-                        launch_worker(data)
-
-                #print "Launched"
-
-            elif type in ["REPL_COMMAND", "REPL_KEEPALIVE", "TERMINATE_REPL"]:
-                worker = workers_by_id.get(data['repl'])
-
-                # TODO allow REPL commands to be run on us too
-
-                if worker is not None:
-                    worker.handle_inbound_message(data)
-                else:
-                    print("Couldn't find repl %s; current workers: %s" % (data['repl'], workers_by_id.keys()))
-                    connection.send_with_header(
-                        {'error': {'type': 'anvil.server.NotRunningTask', 'message': 'No such REPL running'},
-                         'id': data['id']}
-                    )
-
-            elif type == "KILL_TASK":
-
-                worker = workers_by_id.get(data['task'])
-                if worker is not None:
-                    worker.kill_background_task()
-
-            elif type == "GET_TASK_STATE":
-
-                worker = workers_by_id.get(data['task'])
-                if worker is not None:
-                    worker.get_task_state(data)
-                else:
-                    connection.send_with_header(
-                        {'error': {'type': 'anvil.server.NotRunningTask', 'message': 'No such task running'},
-                         'id': data['id']})
-
-            elif type == "SET_IDLE_TIMEOUT":
-                global IDLE_TIMEOUT_SECONDS
-                IDLE_TIMEOUT_SECONDS = data['timeout']
-                self.reset_idle_timer()
-                print("Resetting idle timeout to", data['timeout'])
-
-            elif type == "CHUNK_HEADER":
-                if data['requestId'] in workers_by_id:
-                    worker = workers_by_id[data['requestId']]
-
-                    def send_next_bin(bin_data):
-                        worker.handle_inbound_message(data, bin_data)
-                        self._send_next_bin = None
-
-                    self._send_next_bin = send_next_bin
-                else:
-                    print("Ignoring media for unknown request %s" % data['requestId'])
-                    self._send_next_bin = lambda x: 0
-
-            elif (type is None or type == "PROVIDE_APP") and "id" in data:
-                if type == "PROVIDE_APP":
-                    #print("PROVIDE_APP: Cache fill for %s" % ((data["app-id"], data["app-version"]),))
-                    app_cache[(data["app-id"], data["app-version"])] = data["app"]
-                    if len(app_cache) > APP_CACHE_SIZE:
-                        app_cache.popitem(False)
-
-                if id in workers_by_id:
-                    workers_by_id[id].handle_inbound_message(data)
-                elif is_keepalive:
-                    self._last_keepalive_reply = time.time()
-                else:
-                    print("Bogus reply for " + id + ": " + repr(data)[:120])
-
-            elif type is None and "error" in data:
-                print("Fatal error from Anvil server: " + str(data["error"]))
-                os._exit(1)
-            else:
-                print("Anvil websocket got unrecognised message: "+repr(data))
-
-    def send(self, payload, binary=False):
-        with self._sending_lock:
-            return WebSocketClient.send(self, payload, binary)
-
-    def send_with_header(self, json_data, blob=None):
-        if (not json_data.get("id","").startswith("downlink-keepalive")) and json_data.get("type") != "STATS":
-            self.record_activity()
-        with self._sending_lock:
-            WebSocketClient.send(self, json.dumps(json_data), False)
-            if blob is not None:
-                WebSocketClient.send(self, blob, True)
-
-
-# Defined in two places, so it can be used by BaseWorker and the full-python worker. Yeuch.
-def report_worker_stats(self):
-    p = self.proc_info
-    if p is None:
-        return {}
-    try:
-        cpu = p.cpu_times()
-        mem = p.memory_full_info()
-        return {
-            "info": self.task_info,
-            "age":  time.time() - p.create_time(),
-            "cpu": {
-                "user": cpu.user + cpu.children_user,
-                "system": cpu.system + cpu.children_system,
-                "total": cpu.user + cpu.system + cpu.children_user + cpu.children_system
-            },
-            "mem": {"vms": mem.vms, "uss": mem.uss},
-        }
-    except psutil.Error:
-        return {}
-
-
-# Shared tools for managing worker processes.
-# Nomenclature: "Inbound" calls come from the API server. "Outbound" calls come from the server.
-class BaseWorker(object):
-    def __init__(self, initial_msg, task_info):
-        self.req_ids = set()
-        self.outbound_ids = {} # Outbound ID -> inbound ID it came from
-        self._media_tracking = {} # reqID -> (set([mediaId, mediaId, ]), finishedCallback)
-        self.lock = threading.RLock() # TODO do we need this?
-        self.start_times = {}
-        self.proc_info = None
-        self.task_info = task_info
-
-        self.initial_req_id = initial_msg['id']
-
-    # Handle bookkeeping for which requests we're handling and waiting for
-
-    def record_outbound_call_started(self, outbound_msg):
-        outbound_id = outbound_msg['id']
-        if outbound_id in workers_by_id:
-            raise Exception("Duplicate ID: %s" % outbound_id)
-        self.outbound_ids[outbound_msg['id']] = outbound_msg.get('originating-call', self.initial_req_id)
-        workers_by_id[outbound_id] = self
-
-    def record_outbound_call_complete(self, outbound_id):
-        self.outbound_ids.pop(outbound_id, None)
-        workers_by_id.pop(outbound_id, None)
-
-    def record_inbound_call_started(self, inbound_msg):
-        inbound_id = inbound_msg['id']
-        self.req_ids.add(inbound_id)
-        self.start_times[inbound_id] = time.time()
-        workers_by_id[inbound_id] = self
-
-    def record_inbound_call_complete(self, inbound_id):
-        self.req_ids.discard(inbound_id)
-        self.start_times.pop(inbound_id, None)
-        workers_by_id.pop(inbound_id, None)
-
-        if len(self.req_ids) == 0:
-            self.on_all_inbound_calls_complete()
-
-        maybe_quit_if_draining_and_done()
-
-    def clean_up_all_outstanding_records(self):
-        for id in self.req_ids:
-            self._media_tracking.pop(id, None)
-            workers_by_id.pop(id, None)
-        for id in self.outbound_ids:
-            self._media_tracking.pop(id, None)
-            workers_by_id.pop(id, None)
-
-    def ensure_id_is_mine(self, req_id):
-        if not (req_id in self.req_ids or req_id in self.outbound_ids):
-            raise Exception("Worker attempted to send an ID that doesn't belong to it")
-
-    # Events to be overridden by children
-
-    def handle_inbound_message(self, msg, bindata=None):
-        raise Exception("handle_inbound_message() not implemented")
-
-    def on_all_inbound_calls_complete(self):
-        raise Exception("on_all_inbound_calls_complete() not implemented")
-
-    def repl_keepalive(self):
-        raise Exception("repl_keepalive() not implemented")
-
-    # A common task is to track when the worker has finished sending media for a particular request,
-    # so we can safely kill it.
-
-    def on_media_complete(self, msg, callback):
-        """Register a callback to execute when the worker has finished sending all the media in the given message."""
-        media_ids = set()
-        for o in msg.get("objects", []):
-            if "DataMedia" in o.get("type", []):
-                media_ids.add(o["id"])
-        if len(media_ids) == 0:
-            callback()
-        else:
-            # print("Waiting for media for request '%s': %s" % (msg['id'], repr(list(media_ids))))
-            self._media_tracking[msg['id']] = (media_ids, callback)
-
-    def transmitted_media(self, request_id, media_id):
-        """The worker has finished sending the specified media object; call any necessary callbacks"""
-
-        # print("Media complete: '%s', '%s'" % (request_id, media_id))
-        if request_id in self._media_tracking:
-            media_ids, callback = self._media_tracking[request_id]
-            media_ids.discard(media_id)
-            if len(media_ids) == 0:
-                callback()
-                del self._media_tracking[request_id]
-
-    # Slightly awkward shimming of profiling information into a response message
-    def fill_out_profiling(self, response_msg, description="Downlink dispatch"):
-        """Add profiling information to a response message"""
-
-        p = response_msg.get("profile", None)
-        response_msg["profile"] = {
-            "origin": "Server (Python)",
-            "description": description,
-            "start-time": float(self.start_times.get(response_msg['id'], 0)*1000),
-            "end-time": float(time.time()*1000)
-        }
-        if p is not None:
-            response_msg["profile"]["children"] = [p]
-
-            for o in response_msg.get("objects", []):
-                if o["path"][0] == "profile":
-                    o["path"].insert(1,"children")
-                    o["path"].insert(2, 0)
-
-    report_stats = report_worker_stats
-
-
-# Import the actual worker modules
-
-def init_pdf_worker():
-    global launch_pdf_worker
-
-    if sys.version_info < (3,7,0):
-        print("Warning: PDF Rendering requires Python 3.7. Renderer not initialised")
-    elif IS_WINDOWS:
-        print("Warning: PDF Rendering not supported on Windows. Renderer not initialised")
-    else:
-        from . import pdf_renderer
-        launch_pdf_worker = pdf_renderer.launch
-
-
-if RUNTIME_ID == "pdf-renderer":
-    init_pdf_worker()
-elif RUNTIME_ID.endswith('-sandbox') and not os.getenv("FAKE_SANDBOX"):
-    from . import pypy_sandbox
-    launch_worker = pypy_sandbox.launch
-else:
-    from . import full_python
-    launch_worker = full_python.launch
-
-    if ENABLE_PDF_RENDER:
-        init_pdf_worker()
-
-
-def signal_drain(_signum=None, _frame=None):
-    global draining_start_time
-    if draining_start_time:
-        print("Downlink has already been draining for %s seconds. %s call(s) remaining:" % (int(time.time() - draining_start_time), len(workers_by_id)))
-        print(list(workers_by_id.keys()))
-    else:
-        connection.send_with_header({
-            "type": "DRAIN"
-        })
-        print("Draining downlink. %s call(s) remaining:" % len(workers_by_id))
-        print(list(workers_by_id.keys()))
-        draining_start_time = time.time()
-        maybe_quit_if_draining_and_done()
-
-
-def report_stats():
-    workers = set(workers_by_id.values())
-    worker_stats = []
-    for worker in workers:
-        stats = worker.report_stats()
-        mem_usage = stats.get("mem", {}).get("uss", 0)
-        if PER_WORKER_SOFT_MEMORY_LIMIT is not None and mem_usage > PER_WORKER_SOFT_MEMORY_LIMIT:
-            print("Worker is using %.0fMB: %s " % (mem_usage/(1024*1024.0), stats.get('info')))
-            worker.drain()
-        worker_stats.append(stats)
-    connection.send_with_header({
-        "type": "STATS",
-        "data": worker_stats
-    })
-
-
-
-def run_downlink_host():
-    global connection
-
-    url = os.environ.get("DOWNLINK_SERVER", "ws://localhost:3000/downlink")
-    key = os.environ.get("DOWNLINK_KEY", "ZeXiedeaceimahm1ePhaguvu5Ush9E")
-    os.environ['TZ'] = 'UTC'
-
-    for v in ["DOWNLINK_SERVER", "DOWNLINK_KEY"]:
-        if v in os.environ:
-            del os.environ[v]
-
-    connection = Connection(url, key)
-
-    connection.connect()
-
-    if not IS_WINDOWS:
-        try:
-            signal.signal(signal.SIGUSR2, signal_drain)
-        except Exception as e:
-            print("Failed to add signal handler: %s" % e)
-
-    n = 0
-    while True:
-        try:
-            for _ in range(2):
-                time.sleep(5)
-                report_stats()
-
-            connection.send_with_header({
-                "type": "CALL",
-                "id": "downlink-keepalive-%d" % n,
-                "command": "anvil.private.echo",
-                "args": ["keep-alive"],
-                "kwargs": {},
-            })
-            n += 1
-        except Exception as e:
-            print("Keepalive failed. The downlink has probably disconnected.")
-            print(e)
-            os._exit(1)
+import collections, json, os, psutil, random, signal, subprocess, sys, threading, time, traceback, platform
+from ws4py.client.threadedclient import WebSocketClient
+
+
+# Configuration
+
+TIMEOUT = int(os.environ.get("DOWNLINK_WORKER_TIMEOUT", "30"))
+KEEPALIVE_TIMEOUT = int(os.environ.get("DOWNLINK_KEEPALIVE_TIMEOUT", "30"))
+DROP_PRIVILEGES = os.environ.get("DROP_PRIVILEGES")
+RUNTIME_ID = os.environ.get("RUNTIME_ID", None) or ('python2-full' if sys.version_info[0] < 3 else 'python3-full')
+USER_ID = os.environ.get("DOWNLINK_USER_ID", None)
+ORG_ID = os.environ.get("DOWNLINK_ORG_ID", None)
+ENV_ID = os.environ.get("DOWNLINK_ENV_ID", None)
+SPEC_HASH = os.environ.get("DOWNLINK_SPEC_HASH", None)
+APP_CACHE_SIZE = int(os.environ.get("APP_CACHE_SIZE", "16"))
+ENABLE_PDF_RENDER = os.environ.get("ENABLE_PDF_RENDER")
+PER_WORKER_SOFT_MEMORY_LIMIT = int(os.environ["PER_WORKER_SOFT_MEMORY_LIMIT_MB"])*1024*1024 \
+                                    if "PER_WORKER_SOFT_MEMORY_LIMIT_MB" in os.environ else None
+IDLE_TIMEOUT_SECONDS = int(os.environ.get("IDLE_TIMEOUT_SECONDS","0"))
+
+IS_WINDOWS = "Windows" in platform.system() or "CYGWIN" in platform.system()
+
+for V in ["DOWNLINK_WORKER_TIMEOUT", "DROP_PRIVILEGES", "RUNTIME_ID", "DOWNLINK_USER_ID", "DOWNLINK_ORG_ID", "APP_CACHE_SIZE", "ENABLE_PDF_RENDER"]:
+    if V in os.environ:
+        del os.environ[V]
+
+# Worker modules register themselves here
+workers_by_id = {}
+
+# Cache app content
+app_cache = collections.OrderedDict()
+
+
+def send_with_header(json_data, blob=None):
+    """"Send data to the API router"""
+    connection.send_with_header(json_data, blob)
+
+# Host state
+
+launch_worker = None
+launch_pdf_worker = None
+
+connection = None
+
+rnd = random.SystemRandom()
+MY_SESSION_ID = "".join((rnd.choice("abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789") for _ in range(20)))
+
+draining_start_time = None
+
+
+def is_idle():
+    return len(workers_by_id) == 0
+
+
+def maybe_quit_if_draining_and_done():
+    if draining_start_time is not None and is_idle():
+        if time.time() < draining_start_time + 10:
+            print("Giving API 10 seconds' grace for drain...")
+            def f():
+                time.sleep(draining_start_time + 10 - time.time())
+                maybe_quit_if_draining_and_done()
+            threading.Thread(target=f).start()
+        else:
+            print("Drain complete. Exiting.")
+            os._exit(0)
+
+
+# Utility functions
+
+def get_demote_fn(app_id):
+    if os.name == "nt":
+        return None
+
+    # TODO: Use app_id here to seed UID generation. It might be an actual app ID, or None
+    uid = 20000
+    def do_demotion():
+        if DROP_PRIVILEGES and os.getuid() == 0:
+            os.setgroups([])
+            os.setgid(uid)
+            os.setegid(uid)
+            os.setuid(uid)
+            os.seteuid(uid)
+
+        # Give ourselves an isolated process group so we can take child processes with us when we go
+        os.setpgid(0, 0)
+
+    return do_demotion
+
+
+class PopenWithGroupKill(subprocess.Popen):
+    def terminate(self):
+        try:
+            os.killpg(self.pid, 9)
+        except:
+            pass
+        super(PopenWithGroupKill, self).terminate()
+
+
+# Handle communication with API router
+class Connection(WebSocketClient):
+    def __init__(self, url, key):
+        print("Connecting to " + url)
+        WebSocketClient.__init__(self, url)
+
+        self._sending_lock = threading.RLock()
+        self._send_next_bin = None
+        self._key = key
+        self._last_keepalive_reply = time.time()
+        self._last_activity = time.time()
+        self._idle_timeout_timer = None
+
+        threading.Timer(30, self.check_keepalives).start()
+
+    def record_activity(self):
+        self._last_activity = time.time()
+
+    def reset_idle_timer(self):
+        if self._idle_timeout_timer:
+            self._idle_timeout_timer.cancel()
+        if IDLE_TIMEOUT_SECONDS:
+            self._idle_timeout_timer = threading.Timer(IDLE_TIMEOUT_SECONDS, self.idle_timeout).start()
+
+    def idle_timeout(self):
+        if is_idle() and self._last_activity < time.time() - IDLE_TIMEOUT_SECONDS:
+            print("Idle timeout")
+            signal_drain()
+        else:
+            self.reset_idle_timer()
+
+    def check_keepalives(self):
+        if time.time() - self._last_keepalive_reply > KEEPALIVE_TIMEOUT:
+            print("No keepalive reply in %s seconds. Exiting." % KEEPALIVE_TIMEOUT)
+            os._exit(1)
+        else:
+            threading.Timer(30, self.check_keepalives).start()
+
+    def opened(self):
+        print("Anvil websocket open")
+        self.record_activity()
+        spec = {
+            'runtime': RUNTIME_ID,
+            'session_id': MY_SESSION_ID,
+        }
+
+        if USER_ID is not None:
+            spec['user_id'] = USER_ID
+        elif ORG_ID is not None:
+            spec['org_id'] = ORG_ID
+        elif ENV_ID is not None:
+            spec['env_id'] = ENV_ID
+            spec['spec_hash'] = SPEC_HASH
+
+        id = os.environ.get("DOWNLINK_ID", None)
+        if id:
+            spec['id'] = id
+        self.send(json.dumps({
+            'key': self._key,
+            'v': 2,
+            'spec': spec,
+        }))
+
+    def closed(self, code, reason=None):
+        print("Anvil websocket closed (code %s, reason=%s)" % (code, reason))
+        # The world has ended. Let whatever is in charge of restarting us sort it out.
+        os._exit(1)
+
+    def received_message(self, message):
+        try:
+            self._received_message(message)
+        except Exception as e:
+            print("Error in received_message():")
+            traceback.print_exc()
+            raise
+
+    def _received_message(self, message):
+
+        if message.is_binary:
+            self._send_next_bin(message.data)
+
+        else:
+            data = json.loads(message.data.decode())
+
+            type = data["type"] if 'type' in data else None
+            id = data["id"] if 'id' in data else None
+            is_keepalive = id and id.startswith("downlink-keepalive")
+
+            if not is_keepalive:
+                self.record_activity()
+
+            if 'auth' in data:
+                print("Downlink authenticated OK")
+                self.reset_idle_timer()
+
+            elif 'output' in data:
+                # Output from something this worker has called.
+                calling_worker = workers_by_id.get(data.get('id'))
+                originating_call = calling_worker.outbound_ids.get(id) if calling_worker is not None else None
+
+                if originating_call is not None:
+                    data['id'] = originating_call
+                    self.send_with_header(data)
+                else:
+                    print("Bogus output, probably for an old request (worker: %s): %s" %
+                          ("FOUND" if calling_worker else "MISSING", repr(data)[:100]))
+
+            elif type in ["CALL_WITH_APP", "LAUNCH_BACKGROUND_WITH_APP", "CALL", "LAUNCH_BACKGROUND", "LAUNCH_REPL"]:
+
+                if "app" not in data:
+                    cached_app = app_cache.get((data["app-id"], data["app-version"]))
+                    if cached_app is not None:
+                        #print("Filling out app from cache for %s" % ((data["app-id"], data["app-version"]),))
+                        data["type"] += "_WITH_APP"
+                        data["app"] = cached_app
+
+                #print "Launching new worker for ID " + id
+                if draining_start_time:
+                    self.send_with_header({"id": id, "error": {"type": "anvil.server.DownlinkDrainingError", "message": "New call routed to draining downlink"}})
+                else:
+                    if data.get("command", None) == "anvil.private.pdf.do_print":
+                        if launch_pdf_worker:
+                            launch_pdf_worker(data)
+                        else:
+                            self.send_with_header({"id": id, "error": {"type": "anvil.server.RuntimeUnavailableError", "message": "PDF Rendering unavailable"}})
+                    else:
+                        launch_worker(data)
+
+                #print "Launched"
+
+            elif type in ["REPL_COMMAND", "REPL_KEEPALIVE", "TERMINATE_REPL"]:
+                worker = workers_by_id.get(data['repl'])
+
+                # TODO allow REPL commands to be run on us too
+
+                if worker is not None:
+                    worker.handle_inbound_message(data)
+                else:
+                    print("Couldn't find repl %s; current workers: %s" % (data['repl'], workers_by_id.keys()))
+                    connection.send_with_header(
+                        {'error': {'type': 'anvil.server.NotRunningTask', 'message': 'No such REPL running'},
+                         'id': data['id']}
+                    )
+
+            elif type == "KILL_TASK":
+
+                worker = workers_by_id.get(data['task'])
+                if worker is not None:
+                    worker.kill_background_task()
+
+            elif type == "GET_TASK_STATE":
+
+                worker = workers_by_id.get(data['task'])
+                if worker is not None:
+                    worker.get_task_state(data)
+                else:
+                    connection.send_with_header(
+                        {'error': {'type': 'anvil.server.NotRunningTask', 'message': 'No such task running'},
+                         'id': data['id']})
+
+            elif type == "SET_IDLE_TIMEOUT":
+                global IDLE_TIMEOUT_SECONDS
+                IDLE_TIMEOUT_SECONDS = data['timeout']
+                self.reset_idle_timer()
+                print("Resetting idle timeout to", data['timeout'])
+
+            elif type == "CHUNK_HEADER":
+                if data['requestId'] in workers_by_id:
+                    worker = workers_by_id[data['requestId']]
+
+                    def send_next_bin(bin_data):
+                        worker.handle_inbound_message(data, bin_data)
+                        self._send_next_bin = None
+
+                    self._send_next_bin = send_next_bin
+                else:
+                    print("Ignoring media for unknown request %s" % data['requestId'])
+                    self._send_next_bin = lambda x: 0
+
+            elif (type is None or type == "PROVIDE_APP") and "id" in data:
+                if type == "PROVIDE_APP":
+                    #print("PROVIDE_APP: Cache fill for %s" % ((data["app-id"], data["app-version"]),))
+                    app_cache[(data["app-id"], data["app-version"])] = data["app"]
+                    if len(app_cache) > APP_CACHE_SIZE:
+                        app_cache.popitem(False)
+
+                if id in workers_by_id:
+                    workers_by_id[id].handle_inbound_message(data)
+                elif is_keepalive:
+                    self._last_keepalive_reply = time.time()
+                else:
+                    print("Bogus reply for " + id + ": " + repr(data)[:120])
+
+            elif type is None and "error" in data:
+                print("Fatal error from Anvil server: " + str(data["error"]))
+                os._exit(1)
+            else:
+                print("Anvil websocket got unrecognised message: "+repr(data))
+
+    def send(self, payload, binary=False):
+        with self._sending_lock:
+            return WebSocketClient.send(self, payload, binary)
+
+    def send_with_header(self, json_data, blob=None):
+        if (not json_data.get("id","").startswith("downlink-keepalive")) and json_data.get("type") != "STATS":
+            self.record_activity()
+        with self._sending_lock:
+            WebSocketClient.send(self, json.dumps(json_data), False)
+            if blob is not None:
+                WebSocketClient.send(self, blob, True)
+
+
+# Defined in two places, so it can be used by BaseWorker and the full-python worker. Yeuch.
+def report_worker_stats(self):
+    p = self.proc_info
+    if p is None:
+        return {}
+    try:
+        cpu = p.cpu_times()
+        mem = p.memory_full_info()
+        return {
+            "info": self.task_info,
+            "age":  time.time() - p.create_time(),
+            "cpu": {
+                "user": cpu.user + cpu.children_user,
+                "system": cpu.system + cpu.children_system,
+                "total": cpu.user + cpu.system + cpu.children_user + cpu.children_system
+            },
+            "mem": {"vms": mem.vms, "uss": mem.uss},
+        }
+    except psutil.Error:
+        return {}
+
+
+# Shared tools for managing worker processes.
+# Nomenclature: "Inbound" calls come from the API server. "Outbound" calls come from the server.
+class BaseWorker(object):
+    def __init__(self, initial_msg, task_info):
+        self.req_ids = set()
+        self.outbound_ids = {} # Outbound ID -> inbound ID it came from
+        self._media_tracking = {} # reqID -> (set([mediaId, mediaId, ]), finishedCallback)
+        self.lock = threading.RLock() # TODO do we need this?
+        self.start_times = {}
+        self.proc_info = None
+        self.task_info = task_info
+
+        self.initial_req_id = initial_msg['id']
+
+    # Handle bookkeeping for which requests we're handling and waiting for
+
+    def record_outbound_call_started(self, outbound_msg):
+        outbound_id = outbound_msg['id']
+        if outbound_id in workers_by_id:
+            raise Exception("Duplicate ID: %s" % outbound_id)
+        self.outbound_ids[outbound_msg['id']] = outbound_msg.get('originating-call', self.initial_req_id)
+        workers_by_id[outbound_id] = self
+
+    def record_outbound_call_complete(self, outbound_id):
+        self.outbound_ids.pop(outbound_id, None)
+        workers_by_id.pop(outbound_id, None)
+
+    def record_inbound_call_started(self, inbound_msg):
+        inbound_id = inbound_msg['id']
+        self.req_ids.add(inbound_id)
+        self.start_times[inbound_id] = time.time()
+        workers_by_id[inbound_id] = self
+
+    def record_inbound_call_complete(self, inbound_id):
+        self.req_ids.discard(inbound_id)
+        self.start_times.pop(inbound_id, None)
+        workers_by_id.pop(inbound_id, None)
+
+        if len(self.req_ids) == 0:
+            self.on_all_inbound_calls_complete()
+
+        maybe_quit_if_draining_and_done()
+
+    def clean_up_all_outstanding_records(self):
+        for id in self.req_ids:
+            self._media_tracking.pop(id, None)
+            workers_by_id.pop(id, None)
+        for id in self.outbound_ids:
+            self._media_tracking.pop(id, None)
+            workers_by_id.pop(id, None)
+
+    def ensure_id_is_mine(self, req_id):
+        if not (req_id in self.req_ids or req_id in self.outbound_ids):
+            raise Exception("Worker attempted to send an ID that doesn't belong to it")
+
+    # Events to be overridden by children
+
+    def handle_inbound_message(self, msg, bindata=None):
+        raise Exception("handle_inbound_message() not implemented")
+
+    def on_all_inbound_calls_complete(self):
+        raise Exception("on_all_inbound_calls_complete() not implemented")
+
+    def repl_keepalive(self):
+        raise Exception("repl_keepalive() not implemented")
+
+    # A common task is to track when the worker has finished sending media for a particular request,
+    # so we can safely kill it.
+
+    def on_media_complete(self, msg, callback):
+        """Register a callback to execute when the worker has finished sending all the media in the given message."""
+        media_ids = set()
+        for o in msg.get("objects", []):
+            if "DataMedia" in o.get("type", []):
+                media_ids.add(o["id"])
+        if len(media_ids) == 0:
+            callback()
+        else:
+            # print("Waiting for media for request '%s': %s" % (msg['id'], repr(list(media_ids))))
+            self._media_tracking[msg['id']] = (media_ids, callback)
+
+    def transmitted_media(self, request_id, media_id):
+        """The worker has finished sending the specified media object; call any necessary callbacks"""
+
+        # print("Media complete: '%s', '%s'" % (request_id, media_id))
+        if request_id in self._media_tracking:
+            media_ids, callback = self._media_tracking[request_id]
+            media_ids.discard(media_id)
+            if len(media_ids) == 0:
+                callback()
+                del self._media_tracking[request_id]
+
+    # Slightly awkward shimming of profiling information into a response message
+    def fill_out_profiling(self, response_msg, description="Downlink dispatch"):
+        """Add profiling information to a response message"""
+
+        p = response_msg.get("profile", None)
+        response_msg["profile"] = {
+            "origin": "Server (Python)",
+            "description": description,
+            "start-time": float(self.start_times.get(response_msg['id'], 0)*1000),
+            "end-time": float(time.time()*1000)
+        }
+        if p is not None:
+            response_msg["profile"]["children"] = [p]
+
+            for o in response_msg.get("objects", []):
+                if o["path"][0] == "profile":
+                    o["path"].insert(1,"children")
+                    o["path"].insert(2, 0)
+
+    report_stats = report_worker_stats
+
+
+# Import the actual worker modules
+
+def init_pdf_worker():
+    global launch_pdf_worker
+
+    if sys.version_info < (3,7,0):
+        print("Warning: PDF Rendering requires Python 3.7. Renderer not initialised")
+    elif IS_WINDOWS:
+        print("Warning: PDF Rendering not supported on Windows. Renderer not initialised")
+    else:
+        from . import pdf_renderer
+        launch_pdf_worker = pdf_renderer.launch
+
+
+if RUNTIME_ID == "pdf-renderer":
+    init_pdf_worker()
+elif RUNTIME_ID.endswith('-sandbox') and not os.getenv("FAKE_SANDBOX"):
+    from . import pypy_sandbox
+    launch_worker = pypy_sandbox.launch
+else:
+    from . import full_python
+    launch_worker = full_python.launch
+
+    if ENABLE_PDF_RENDER:
+        init_pdf_worker()
+
+
+def signal_drain(_signum=None, _frame=None):
+    global draining_start_time
+    if draining_start_time:
+        print("Downlink has already been draining for %s seconds. %s call(s) remaining:" % (int(time.time() - draining_start_time), len(workers_by_id)))
+        print(list(workers_by_id.keys()))
+    else:
+        connection.send_with_header({
+            "type": "DRAIN"
+        })
+        print("Draining downlink. %s call(s) remaining:" % len(workers_by_id))
+        print(list(workers_by_id.keys()))
+        draining_start_time = time.time()
+        maybe_quit_if_draining_and_done()
+
+
+def report_stats():
+    workers = set(workers_by_id.values())
+    worker_stats = []
+    for worker in workers:
+        stats = worker.report_stats()
+        mem_usage = stats.get("mem", {}).get("uss", 0)
+        if PER_WORKER_SOFT_MEMORY_LIMIT is not None and mem_usage > PER_WORKER_SOFT_MEMORY_LIMIT:
+            print("Worker is using %.0fMB: %s " % (mem_usage/(1024*1024.0), stats.get('info')))
+            worker.drain()
+        worker_stats.append(stats)
+    connection.send_with_header({
+        "type": "STATS",
+        "data": worker_stats
+    })
+
+
+
+def run_downlink_host():
+    global connection
+
+    url = os.environ.get("DOWNLINK_SERVER", "ws://localhost:3000/downlink")
+    key = os.environ.get("DOWNLINK_KEY", "ZeXiedeaceimahm1ePhaguvu5Ush9E")
+    os.environ['TZ'] = 'UTC'
+
+    for v in ["DOWNLINK_SERVER", "DOWNLINK_KEY"]:
+        if v in os.environ:
+            del os.environ[v]
+
+    connection = Connection(url, key)
+
+    connection.connect()
+
+    if not IS_WINDOWS:
+        try:
+            signal.signal(signal.SIGUSR2, signal_drain)
+        except Exception as e:
+            print("Failed to add signal handler: %s" % e)
+
+    n = 0
+    while True:
+        try:
+            for _ in range(2):
+                time.sleep(5)
+                report_stats()
+
+            connection.send_with_header({
+                "type": "CALL",
+                "id": "downlink-keepalive-%d" % n,
+                "command": "anvil.private.echo",
+                "args": ["keep-alive"],
+                "kwargs": {},
+            })
+            n += 1
+        except Exception as e:
+            print("Keepalive failed. The downlink has probably disconnected.")
+            print(e)
+            os._exit(1)
```

### Comparing `anvil-app-server-1.8.0/anvil_downlink_host/full_python.py` & `anvil-app-server-1.9.0/anvil_downlink_host/full_python.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,386 +1,386 @@
-import  os, psutil, random, sys, threading, time
-from subprocess import PIPE
-from anvil_downlink_util.pipes import MessagePipe
-
-# State representing which workers are running here
-from anvil_downlink_host import workers_by_id, send_with_header, maybe_quit_if_draining_and_done, \
-                                    PopenWithGroupKill, get_demote_fn, TIMEOUT, \
-                                    report_worker_stats
-
-CAN_PERSIST = (os.environ.get("DOWNLINK_CAN_PERSIST", "false").lower() in {"true", "1"})
-
-cached_workers = {}
-CACHE_LOCK = threading.Lock()
-
-class Worker:
-    def __init__(self, first_req_id, enable_profiling=False, app_id=None, app_version=None, cache_key=None, set_timeout=True, task_info=None):
-        self.initial_req_id = first_req_id
-        self.req_ids = {first_req_id}
-        self.outbound_ids = {} # Outbound ID -> inbound ID it came from
-        self.lock = threading.RLock()
-        self.media_tracking = {} # reqID -> (set([mediaId, mediaId, ]), finishedCallback)
-
-        self.proc = PopenWithGroupKill([sys.executable, "-um", "anvil_downlink_worker.full_python_worker"],
-                                       bufsize=0, stdin=PIPE, stdout=PIPE, preexec_fn=get_demote_fn(app_id))
-        self.proc_info = psutil.Process(self.proc.pid)
-        self.task_info = task_info
-        self.from_worker = MessagePipe(self.proc.stdout)
-        self.to_worker = MessagePipe(self.proc.stdin)
-
-        workers_by_id[first_req_id] = self
-        self.cache_key = cache_key
-        if cache_key is not None:
-            #print("Saving to cache for %s [version %s]" % (cache_key, app_version))
-            with CACHE_LOCK:
-                old_version, displaced_worker = cached_workers.get(cache_key, (None, None))
-                cached_workers[cache_key] = (app_version, self)
-            if displaced_worker is not None:
-                print("Displacing persistent worker for %s:\nVersion %s -> %s" % (cache_key, old_version, app_version))
-                displaced_worker.drain()
-            else:
-                print("New persistent worker for %s (version %s)" % (cache_key, app_version))
-
-        self.timed_out = False
-        self.timeouts = {}
-        self.app_version = app_version
-        if cache_key is None and set_timeout:
-            self.set_timeout(first_req_id)
-
-        self.start_time = {first_req_id: time.time()}
-        self.enable_profiling = {first_req_id: enable_profiling}
-        self.killing_task = False
-        self.global_error = None
-
-        threading.Thread(target=self.read_loop).start()
-
-    def on_media_complete(self, msg, callback):
-        media_ids = set()
-        for o in msg.get("objects", []):
-            if "DataMedia" in o.get("type", []):
-                media_ids.add(o["id"])
-        if len(media_ids) == 0:
-            callback()
-        else:
-            #print("Waiting for media for request '%s': %s" % (msg['id'], repr(list(media_ids))))
-            self.media_tracking[msg['id']] = (media_ids, callback)
-
-    def transmitted_media(self, request_id, media_id):
-        #print("Media complete: '%s', '%s'" % (request_id, media_id))
-        if request_id in self.media_tracking:
-            media_ids, callback = self.media_tracking[request_id]
-            media_ids.discard(media_id)
-            if len(media_ids) == 0:
-                callback()
-                del self.media_tracking[request_id]
-
-    def set_timeout(self, timeout_key):
-        #print("Set timeout for %s" % timeout_key)
-        if timeout_key in self.timeouts:
-            return
-        timeout_timer = threading.Timer(TIMEOUT, lambda: self.soft_timeout(timeout_key))
-        self.timeouts[timeout_key] = timeout_timer
-        timeout_timer.start()
-
-    def clear_timeout(self, timeout_key):
-        timeout_timer = self.timeouts.pop(timeout_key, None)
-        if timeout_timer is not None:
-            timeout_timer.cancel()
-
-    def soft_timeout(self, timeout_key):
-        # Something has timed out. If we are cached, drain ourselves nicely before terminating
-        print("TIMEOUT for %s" % timeout_key)
-        self.timed_out = True
-        if self.cache_key is None:
-            self.hard_timeout()
-        else:
-            print("Cached worker %s timed out; draining" % self.cache_key)
-            with CACHE_LOCK:
-                if self.cache_key in cached_workers and cached_workers[self.cache_key][1] is self:
-                    cached_workers.pop(self.cache_key, None)
-            self.timeout_timer = threading.Timer(TIMEOUT, self.hard_timeout)
-            self.timeout_timer.start()
-
-    def hard_timeout(self):
-        print("TIMEOUT TERMINATE FOR %s" % self.req_ids)
-        self.timed_out = True
-        self.proc.terminate()
-
-    def kill_with_error(self, err):
-        self.global_error = err
-        self.proc.terminate()
-
-    def drain(self):
-        # Finish up our execution and time out.
-        if self.cache_key is None:
-            print("Worker for %s is not cached, ignoring drain request" % self.req_ids)
-        elif len(self.req_ids) == 0:
-            print("Worker for %s drained, terminating instantly (version %s)" % (self.cache_key, self.app_version))
-            try:
-                self.proc.terminate()
-            except:
-                pass
-        else:
-            print("Worker for %s draining, setting timeout (version %s)" % (self.cache_key, self.app_version))
-            self.set_timeout("DRAINED")
-
-    def responded(self, req_id):
-        self.clear_timeout(req_id)
-        self.req_ids.discard(req_id)
-        workers_by_id.pop(req_id, None)
-        self.start_time.pop(req_id, None)
-        self.enable_profiling.pop(req_id, None)
-        if (self.cache_key is None or cached_workers.get(self.cache_key, (None,None))[1] is not self) and len(self.req_ids) == 0:
-            # Drain complete; goodbye!
-            if self.cache_key is not None:
-                print("Cache worker for %s drained (version %s)" % (self.cache_key, self.app_version))
-            self.proc.terminate()
-
-        maybe_quit_if_draining_and_done()
-        #print("Done @%s -> %s" % (self.cache_key, cached_workers.get(self.cache_key)))
-
-    def kill_background_task(self):
-        if self.killing_task:
-            return
-        self.killing_task = True
-        print("SOFT KILL BACKGROUND TASK %s" % self.initial_req_id)
-
-        # Request state. If it returns with in 5 seconds, we will die with state, else we hard-kill
-        self.timeout_timer = threading.Timer(5, self._hard_kill_background_task)
-        self.send({'type': 'GET_TASK_STATE', 'id': 'pre-kill-task-state'})
-        self.timeout_timer.start()
-
-    def _hard_kill_background_task(self):
-        print("HARD KILL BACKGROUND TASK %s" % self.initial_req_id)
-        try:
-            self.req_ids.discard('pre-kill-task-state')
-            send_with_header({'type': 'NOTIFY_TASK_KILLED', 'id': self.initial_req_id})
-        finally:
-            self.hard_timeout()
-
-    # Output gets forwarded straight upstream
-    def read_loop(self):
-        try:
-            while True:
-                try:
-                    msg, bindata = self.from_worker.receive()
-                except EOFError:
-                    break
-                type = msg.get("type")
-                id = msg.get("id") or msg.get("requestId")
-
-                if type == "CALL" or type == "GET_APP":
-                    self.outbound_ids[msg["id"]] = msg.get('originating-call')
-                    workers_by_id[msg["id"]] = self
-                else:
-                    if id is None:
-                        if "output" in msg:
-                            # Output from unknown thread? Broadcast it.
-                            print("Broadcasting output from unknown thread: %s" % msg)
-                            for i in self.req_ids:
-                                msg["id"] = i
-                                send_with_header(msg)
-                        else:
-                            print("Discarding invalid message with no ID: %s" % repr(msg))
-                        continue
-                    if id not in self.req_ids and id not in self.outbound_ids:
-                        print("Discarding invalid message with bogus ID: %s" % repr(msg))
-                        if type == "CHUNK_HEADER":
-                            print("Discarding binary data chunk")
-                        continue
-
-                try:
-                    if type == "CHUNK_HEADER":
-                        send_with_header(msg, bindata)
-                        if msg.get("lastChunk"):
-                            self.transmitted_media(msg['requestId'], msg['mediaId'])
-                    else:
-
-                        if "response" in msg and self.enable_profiling.get(id):
-                            p = msg.get("profile", None)
-                            msg["profile"] = {
-                                "origin": "Server (Python)",
-                                "description": "Downlink dispatch",
-                                "start-time": float(self.start_time.get(id, 0)*1000),
-                                "end-time": float(time.time()*1000)
-                            }
-                            if p is not None:
-                                msg["profile"]["children"] = [p]
-
-                                for o in msg.get("objects", []):
-                                    if o["path"][0] == "profile":
-                                        o["path"].insert(1,"children")
-                                        o["path"].insert(2, 0)
-
-                        if "response" in msg and msg['id'] == 'pre-kill-task-state':
-                            # Special case handling for a "clean" kill (where we manage to recover the state)
-
-                            objects = msg.get('objects', [])
-                            for o in objects:
-                                if 'path' in o and o['path'][0] == 'response':
-                                    o['path'][0] = 'taskState'
-                                if 'DataMedia' in o['type']:
-                                    msg['objects'] = []
-                                    msg['response'] = None
-                                    break
-
-                            self.req_ids.discard('pre-kill-task-state')
-
-                            send_with_header({'type': 'NOTIFY_TASK_KILLED', 'id': self.initial_req_id,
-                                                         'taskState': msg['response'], 'objects': objects})
-
-                            if self.timeout_timer:
-                                self.timeout_timer.cancel()
-
-                            self.proc.terminate()
-                        else:
-                            send_with_header(msg)
-
-                    if "response" in msg or "error" in msg:
-                        #if statsd and (id in self.start_time):
-                        #    statsd.timing('Downlink.WorkerLifetime', (time.time()*1000) - self.start_time.get(id, 0)*1000)
-                        self.on_media_complete(msg, lambda: self.responded(id))
-                        if "error" in msg and msg.get("moduleLoadFailed"):
-                            self.kill_with_error(msg["error"])
-
-
-                except UnicodeError:
-                    send_with_header({"id": id, "error": {"type": "UnicodeError", "message": "This function returned a binary string (not text). If you want to return binary data, use a BlobMedia object instead."}})
-                    self.responded(id)
-
-        except EOFError:
-            print("EOFError while reading worker stdout. This should not have happened.")
-            pass
-
-        finally:
-            for i in self.req_ids:
-                workers_by_id.pop(i, None)
-            for i in self.outbound_ids.keys():
-                workers_by_id.pop(i, None)
-            rt = self.proc.poll()
-            if rt is None:
-                self.proc.terminate()
-            for _,t in self.timeouts.items():
-                t.cancel()
-            if self.cache_key is not None and cached_workers.get(self.cache_key, (None,None))[1] is self:
-                cached_workers.pop(self.cache_key, None)
-
-            error_id = "".join([random.choice('0123456789abcdef') for x in range(10)])
-            for i in self.req_ids:
-                if self.global_error is not None:
-                    err = self.global_error
-                elif self.timed_out:
-                    err = {
-                        'message': "Server code took too long",
-                        'type': "anvil.server.TimeoutError"
-                    }
-                elif rt == -9:
-                    err = {
-                        'message': "Server code execution process was killed. It may have run out of memory: %s" % (error_id),
-                        'type': "anvil.server.ExecutionTerminatedError"
-                    }
-                    sys.stderr.write(err['message'] + " (IDs %s)\n" % i)
-                    sys.stderr.flush()
-                else:
-                    err = {
-                        'message': "Server code exited unexpectedly: %s" % (error_id),
-                        'type': "anvil.server.ExecutionTerminatedError"
-                    }
-                    sys.stderr.write(err['message'] + " (IDs %s)\n" % i)
-                    sys.stderr.flush()
-                send_with_header({'id': i, 'error': err})
-            print ("Worker terminated for IDs %s (return code %s)" % (self.req_ids, rt))
-            maybe_quit_if_draining_and_done()
-
-    def send(self, msg, bindata=None):
-        id = msg.get("id")
-        if msg.get("type") in ["CALL", "CALL_WITH_APP", "GET_TASK_STATE", "LAUNCH_REPL", "REPL_COMMAND", "TERMINATE_REPL"]:
-            # It's a new request! Start the timeout
-            #print ("Setting timeout and routing for new request ID %s" % id)
-            workers_by_id[id] = self
-            if msg.get("enable-profiling"):
-                self.enable_profiling[id] = True
-                self.start_time[id] = time.time()
-            self.req_ids.add(id)
-            if msg["type"] != "REPL_COMMAND":
-                self.set_timeout(id)
-
-        elif msg.get("type") == "REPL_KEEPALIVE":
-            self.clear_timeout(msg["repl"])
-            self.set_timeout(msg["repl"])
-            send_with_header({"id": id, "response": None})
-            return
-
-        try:
-            self.to_worker.send(msg, bindata)
-        except (BrokenPipeError, EOFError) as e:
-            print("Host got {}: {} sending to worker, terminating.".format(type(e).__name__, e))
-            self.proc.terminate()
-
-        def outbound_done():
-            self.outbound_ids.pop(id, None)
-            workers_by_id.pop(id, None)
-            maybe_quit_if_draining_and_done()
-
-        if "response" in msg or "error" in msg:
-            self.on_media_complete(msg, outbound_done)
-
-    def get_task_state(self, msg):
-        self.send(msg)
-
-    def handle_inbound_message(self, msg, bindata=None):
-        self.send(msg, bindata)
-        if bin is not None and msg.get("last_chunk"):
-            self.transmitted_media(msg.get("requestId"), msg.get("mediaId"))
-
-    report_stats = report_worker_stats
-
-
-def launch(data):
-    type = data.get("type")
-    id = data.get("id")
-
-    persist_key = data.get("persist-key")
-
-    start_time = time.time()
-
-    is_background_task = (type in ["LAUNCH_BACKGROUND", "LAUNCH_BACKGROUND_WITH_APP"])
-    is_repl_launch = type == "LAUNCH_REPL"
-    cache_key = None
-    worker = None
-    version = None
-    supplied_version = data.get("app-version")
-
-    print ("%s '%s' for app '%s' (ID %s)" % ("Launching REPL" if is_repl_launch else "Launching BG task" if is_background_task else "Calling function",
-                                             data.get("command", "<no func>"), data.get("app-id", "<unknown>"), id))
-
-    if CAN_PERSIST and not is_background_task and persist_key is not None and "app-id" in data and supplied_version is not None:
-        cache_key = repr((data["app-id"], persist_key))
-        #print("Attempt persistence: %s" % cache_key)
-        version, worker = cached_workers.get(cache_key, (None,None))
-        #print("Version %s:\n%s\nvs\n%s" % (("MATCH" if version==supplied_version else "MISMATCH"), version, supplied_version))
-
-    if data.get('command') == "anvil.private.pdf.get_component" and not is_background_task:
-        wid = data['args'][0][0]
-        worker = workers_by_id.get(wid)
-        if worker is None:
-            send_with_header({'id': id, 'error': {'message': "No component worker found for print call '%s'" % wid}})
-            return
-
-    elif worker is None or version != supplied_version:
-        worker = Worker(id, data.get("enable-profiling", False), data.get("app-id", "<unknown>"),
-                        cache_key=cache_key, app_version=supplied_version, set_timeout=not is_background_task and not is_repl_launch,
-                        task_info={
-                            "app_id": data["app-id"],
-                            "type": "repl" if is_repl_launch else "background_task" if is_background_task else "persistent_worker" if cache_key else "server_call",
-                            "task": data.get("command"),
-                            "persist": {"key": persist_key, "version": supplied_version} if cache_key else None,
-                        })
-
-    worker.send(data)
-
-    # if statsd:
-    #     if is_background_task:
-    #         statsd.incr('Downlink.LaunchBackgroundTask')
-    #     else:
-    #         statsd.incr('Downlink.Call')
-
+import  os, psutil, random, sys, threading, time
+from subprocess import PIPE
+from anvil_downlink_util.pipes import MessagePipe
+
+# State representing which workers are running here
+from anvil_downlink_host import workers_by_id, send_with_header, maybe_quit_if_draining_and_done, \
+                                    PopenWithGroupKill, get_demote_fn, TIMEOUT, \
+                                    report_worker_stats
+
+CAN_PERSIST = (os.environ.get("DOWNLINK_CAN_PERSIST", "false").lower() in {"true", "1"})
+
+cached_workers = {}
+CACHE_LOCK = threading.Lock()
+
+class Worker:
+    def __init__(self, first_req_id, enable_profiling=False, app_id=None, app_version=None, cache_key=None, set_timeout=True, task_info=None):
+        self.initial_req_id = first_req_id
+        self.req_ids = {first_req_id}
+        self.outbound_ids = {} # Outbound ID -> inbound ID it came from
+        self.lock = threading.RLock()
+        self.media_tracking = {} # reqID -> (set([mediaId, mediaId, ]), finishedCallback)
+
+        self.proc = PopenWithGroupKill([sys.executable, "-um", "anvil_downlink_worker.full_python_worker"],
+                                       bufsize=0, stdin=PIPE, stdout=PIPE, preexec_fn=get_demote_fn(app_id))
+        self.proc_info = psutil.Process(self.proc.pid)
+        self.task_info = task_info
+        self.from_worker = MessagePipe(self.proc.stdout)
+        self.to_worker = MessagePipe(self.proc.stdin)
+
+        workers_by_id[first_req_id] = self
+        self.cache_key = cache_key
+        if cache_key is not None:
+            #print("Saving to cache for %s [version %s]" % (cache_key, app_version))
+            with CACHE_LOCK:
+                old_version, displaced_worker = cached_workers.get(cache_key, (None, None))
+                cached_workers[cache_key] = (app_version, self)
+            if displaced_worker is not None:
+                print("Displacing persistent worker for %s:\nVersion %s -> %s" % (cache_key, old_version, app_version))
+                displaced_worker.drain()
+            else:
+                print("New persistent worker for %s (version %s)" % (cache_key, app_version))
+
+        self.timed_out = False
+        self.timeouts = {}
+        self.app_version = app_version
+        if cache_key is None and set_timeout:
+            self.set_timeout(first_req_id)
+
+        self.start_time = {first_req_id: time.time()}
+        self.enable_profiling = {first_req_id: enable_profiling}
+        self.killing_task = False
+        self.global_error = None
+
+        threading.Thread(target=self.read_loop).start()
+
+    def on_media_complete(self, msg, callback):
+        media_ids = set()
+        for o in msg.get("objects", []):
+            if "DataMedia" in o.get("type", []):
+                media_ids.add(o["id"])
+        if len(media_ids) == 0:
+            callback()
+        else:
+            #print("Waiting for media for request '%s': %s" % (msg['id'], repr(list(media_ids))))
+            self.media_tracking[msg['id']] = (media_ids, callback)
+
+    def transmitted_media(self, request_id, media_id):
+        #print("Media complete: '%s', '%s'" % (request_id, media_id))
+        if request_id in self.media_tracking:
+            media_ids, callback = self.media_tracking[request_id]
+            media_ids.discard(media_id)
+            if len(media_ids) == 0:
+                callback()
+                del self.media_tracking[request_id]
+
+    def set_timeout(self, timeout_key):
+        #print("Set timeout for %s" % timeout_key)
+        if timeout_key in self.timeouts:
+            return
+        timeout_timer = threading.Timer(TIMEOUT, lambda: self.soft_timeout(timeout_key))
+        self.timeouts[timeout_key] = timeout_timer
+        timeout_timer.start()
+
+    def clear_timeout(self, timeout_key):
+        timeout_timer = self.timeouts.pop(timeout_key, None)
+        if timeout_timer is not None:
+            timeout_timer.cancel()
+
+    def soft_timeout(self, timeout_key):
+        # Something has timed out. If we are cached, drain ourselves nicely before terminating
+        print("TIMEOUT for %s" % timeout_key)
+        self.timed_out = True
+        if self.cache_key is None:
+            self.hard_timeout()
+        else:
+            print("Cached worker %s timed out; draining" % self.cache_key)
+            with CACHE_LOCK:
+                if self.cache_key in cached_workers and cached_workers[self.cache_key][1] is self:
+                    cached_workers.pop(self.cache_key, None)
+            self.timeout_timer = threading.Timer(TIMEOUT, self.hard_timeout)
+            self.timeout_timer.start()
+
+    def hard_timeout(self):
+        print("TIMEOUT TERMINATE FOR %s" % self.req_ids)
+        self.timed_out = True
+        self.proc.terminate()
+
+    def kill_with_error(self, err):
+        self.global_error = err
+        self.proc.terminate()
+
+    def drain(self):
+        # Finish up our execution and time out.
+        if self.cache_key is None:
+            print("Worker for %s is not cached, ignoring drain request" % self.req_ids)
+        elif len(self.req_ids) == 0:
+            print("Worker for %s drained, terminating instantly (version %s)" % (self.cache_key, self.app_version))
+            try:
+                self.proc.terminate()
+            except:
+                pass
+        else:
+            print("Worker for %s draining, setting timeout (version %s)" % (self.cache_key, self.app_version))
+            self.set_timeout("DRAINED")
+
+    def responded(self, req_id):
+        self.clear_timeout(req_id)
+        self.req_ids.discard(req_id)
+        workers_by_id.pop(req_id, None)
+        self.start_time.pop(req_id, None)
+        self.enable_profiling.pop(req_id, None)
+        if (self.cache_key is None or cached_workers.get(self.cache_key, (None,None))[1] is not self) and len(self.req_ids) == 0:
+            # Drain complete; goodbye!
+            if self.cache_key is not None:
+                print("Cache worker for %s drained (version %s)" % (self.cache_key, self.app_version))
+            self.proc.terminate()
+
+        maybe_quit_if_draining_and_done()
+        #print("Done @%s -> %s" % (self.cache_key, cached_workers.get(self.cache_key)))
+
+    def kill_background_task(self):
+        if self.killing_task:
+            return
+        self.killing_task = True
+        print("SOFT KILL BACKGROUND TASK %s" % self.initial_req_id)
+
+        # Request state. If it returns with in 5 seconds, we will die with state, else we hard-kill
+        self.timeout_timer = threading.Timer(5, self._hard_kill_background_task)
+        self.send({'type': 'GET_TASK_STATE', 'id': 'pre-kill-task-state'})
+        self.timeout_timer.start()
+
+    def _hard_kill_background_task(self):
+        print("HARD KILL BACKGROUND TASK %s" % self.initial_req_id)
+        try:
+            self.req_ids.discard('pre-kill-task-state')
+            send_with_header({'type': 'NOTIFY_TASK_KILLED', 'id': self.initial_req_id})
+        finally:
+            self.hard_timeout()
+
+    # Output gets forwarded straight upstream
+    def read_loop(self):
+        try:
+            while True:
+                try:
+                    msg, bindata = self.from_worker.receive()
+                except EOFError:
+                    break
+                type = msg.get("type")
+                id = msg.get("id") or msg.get("requestId")
+
+                if type == "CALL" or type == "GET_APP":
+                    self.outbound_ids[msg["id"]] = msg.get('originating-call')
+                    workers_by_id[msg["id"]] = self
+                else:
+                    if id is None:
+                        if "output" in msg:
+                            # Output from unknown thread? Broadcast it.
+                            print("Broadcasting output from unknown thread: %s" % msg)
+                            for i in self.req_ids:
+                                msg["id"] = i
+                                send_with_header(msg)
+                        else:
+                            print("Discarding invalid message with no ID: %s" % repr(msg))
+                        continue
+                    if id not in self.req_ids and id not in self.outbound_ids:
+                        print("Discarding invalid message with bogus ID: %s" % repr(msg))
+                        if type == "CHUNK_HEADER":
+                            print("Discarding binary data chunk")
+                        continue
+
+                try:
+                    if type == "CHUNK_HEADER":
+                        send_with_header(msg, bindata)
+                        if msg.get("lastChunk"):
+                            self.transmitted_media(msg['requestId'], msg['mediaId'])
+                    else:
+
+                        if "response" in msg and self.enable_profiling.get(id):
+                            p = msg.get("profile", None)
+                            msg["profile"] = {
+                                "origin": "Server (Python)",
+                                "description": "Downlink dispatch",
+                                "start-time": float(self.start_time.get(id, 0)*1000),
+                                "end-time": float(time.time()*1000)
+                            }
+                            if p is not None:
+                                msg["profile"]["children"] = [p]
+
+                                for o in msg.get("objects", []):
+                                    if o["path"][0] == "profile":
+                                        o["path"].insert(1,"children")
+                                        o["path"].insert(2, 0)
+
+                        if "response" in msg and msg['id'] == 'pre-kill-task-state':
+                            # Special case handling for a "clean" kill (where we manage to recover the state)
+
+                            objects = msg.get('objects', [])
+                            for o in objects:
+                                if 'path' in o and o['path'][0] == 'response':
+                                    o['path'][0] = 'taskState'
+                                if 'DataMedia' in o['type']:
+                                    msg['objects'] = []
+                                    msg['response'] = None
+                                    break
+
+                            self.req_ids.discard('pre-kill-task-state')
+
+                            send_with_header({'type': 'NOTIFY_TASK_KILLED', 'id': self.initial_req_id,
+                                                         'taskState': msg['response'], 'objects': objects})
+
+                            if self.timeout_timer:
+                                self.timeout_timer.cancel()
+
+                            self.proc.terminate()
+                        else:
+                            send_with_header(msg)
+
+                    if "response" in msg or "error" in msg:
+                        #if statsd and (id in self.start_time):
+                        #    statsd.timing('Downlink.WorkerLifetime', (time.time()*1000) - self.start_time.get(id, 0)*1000)
+                        self.on_media_complete(msg, lambda: self.responded(id))
+                        if "error" in msg and msg.get("moduleLoadFailed"):
+                            self.kill_with_error(msg["error"])
+
+
+                except UnicodeError:
+                    send_with_header({"id": id, "error": {"type": "UnicodeError", "message": "This function returned a binary string (not text). If you want to return binary data, use a BlobMedia object instead."}})
+                    self.responded(id)
+
+        except EOFError:
+            print("EOFError while reading worker stdout. This should not have happened.")
+            pass
+
+        finally:
+            for i in self.req_ids:
+                workers_by_id.pop(i, None)
+            for i in self.outbound_ids.keys():
+                workers_by_id.pop(i, None)
+            rt = self.proc.poll()
+            if rt is None:
+                self.proc.terminate()
+            for _,t in self.timeouts.items():
+                t.cancel()
+            if self.cache_key is not None and cached_workers.get(self.cache_key, (None,None))[1] is self:
+                cached_workers.pop(self.cache_key, None)
+
+            error_id = "".join([random.choice('0123456789abcdef') for x in range(10)])
+            for i in self.req_ids:
+                if self.global_error is not None:
+                    err = self.global_error
+                elif self.timed_out:
+                    err = {
+                        'message': "Server code took too long",
+                        'type': "anvil.server.TimeoutError"
+                    }
+                elif rt == -9:
+                    err = {
+                        'message': "Server code execution process was killed. It may have run out of memory: %s" % (error_id),
+                        'type': "anvil.server.ExecutionTerminatedError"
+                    }
+                    sys.stderr.write(err['message'] + " (IDs %s)\n" % i)
+                    sys.stderr.flush()
+                else:
+                    err = {
+                        'message': "Server code exited unexpectedly: %s" % (error_id),
+                        'type': "anvil.server.ExecutionTerminatedError"
+                    }
+                    sys.stderr.write(err['message'] + " (IDs %s)\n" % i)
+                    sys.stderr.flush()
+                send_with_header({'id': i, 'error': err})
+            print ("Worker terminated for IDs %s (return code %s)" % (self.req_ids, rt))
+            maybe_quit_if_draining_and_done()
+
+    def send(self, msg, bindata=None):
+        id = msg.get("id")
+        if msg.get("type") in ["CALL", "CALL_WITH_APP", "GET_TASK_STATE", "LAUNCH_REPL", "REPL_COMMAND", "TERMINATE_REPL"]:
+            # It's a new request! Start the timeout
+            #print ("Setting timeout and routing for new request ID %s" % id)
+            workers_by_id[id] = self
+            if msg.get("enable-profiling"):
+                self.enable_profiling[id] = True
+                self.start_time[id] = time.time()
+            self.req_ids.add(id)
+            if msg["type"] != "REPL_COMMAND":
+                self.set_timeout(id)
+
+        elif msg.get("type") == "REPL_KEEPALIVE":
+            self.clear_timeout(msg["repl"])
+            self.set_timeout(msg["repl"])
+            send_with_header({"id": id, "response": None})
+            return
+
+        try:
+            self.to_worker.send(msg, bindata)
+        except (BrokenPipeError, EOFError) as e:
+            print("Host got {}: {} sending to worker, terminating.".format(type(e).__name__, e))
+            self.proc.terminate()
+
+        def outbound_done():
+            self.outbound_ids.pop(id, None)
+            workers_by_id.pop(id, None)
+            maybe_quit_if_draining_and_done()
+
+        if "response" in msg or "error" in msg:
+            self.on_media_complete(msg, outbound_done)
+
+    def get_task_state(self, msg):
+        self.send(msg)
+
+    def handle_inbound_message(self, msg, bindata=None):
+        self.send(msg, bindata)
+        if bin is not None and msg.get("last_chunk"):
+            self.transmitted_media(msg.get("requestId"), msg.get("mediaId"))
+
+    report_stats = report_worker_stats
+
+
+def launch(data):
+    type = data.get("type")
+    id = data.get("id")
+
+    persist_key = data.get("persist-key")
+
+    start_time = time.time()
+
+    is_background_task = (type in ["LAUNCH_BACKGROUND", "LAUNCH_BACKGROUND_WITH_APP"])
+    is_repl_launch = type == "LAUNCH_REPL"
+    cache_key = None
+    worker = None
+    version = None
+    supplied_version = data.get("app-version")
+
+    print ("%s '%s' for app '%s' (ID %s)" % ("Launching REPL" if is_repl_launch else "Launching BG task" if is_background_task else "Calling function",
+                                             data.get("command", "<no func>"), data.get("app-id", "<unknown>"), id))
+
+    if CAN_PERSIST and not is_background_task and persist_key is not None and "app-id" in data and supplied_version is not None:
+        cache_key = repr((data["app-id"], persist_key))
+        #print("Attempt persistence: %s" % cache_key)
+        version, worker = cached_workers.get(cache_key, (None,None))
+        #print("Version %s:\n%s\nvs\n%s" % (("MATCH" if version==supplied_version else "MISMATCH"), version, supplied_version))
+
+    if data.get('command') == "anvil.private.pdf.get_component" and not is_background_task:
+        wid = data['args'][0][0]
+        worker = workers_by_id.get(wid)
+        if worker is None:
+            send_with_header({'id': id, 'error': {'message': "No component worker found for print call '%s'" % wid}})
+            return
+
+    elif worker is None or version != supplied_version:
+        worker = Worker(id, data.get("enable-profiling", False), data.get("app-id", "<unknown>"),
+                        cache_key=cache_key, app_version=supplied_version, set_timeout=not is_background_task and not is_repl_launch,
+                        task_info={
+                            "app_id": data["app-id"],
+                            "type": "repl" if is_repl_launch else "background_task" if is_background_task else "persistent_worker" if cache_key else "server_call",
+                            "task": data.get("command"),
+                            "persist": {"key": persist_key, "version": supplied_version} if cache_key else None,
+                        })
+
+    worker.send(data)
+
+    # if statsd:
+    #     if is_background_task:
+    #         statsd.incr('Downlink.LaunchBackgroundTask')
+    #     else:
+    #         statsd.incr('Downlink.Call')
+
```

### Comparing `anvil-app-server-1.8.0/anvil_downlink_host/pdf_renderer.py` & `anvil-app-server-1.9.0/anvil_downlink_host/pdf_renderer.py`

 * *Files identical despite different names*

### Comparing `anvil-app-server-1.8.0/anvil_downlink_util/pipes.py` & `anvil-app-server-1.9.0/anvil_downlink_util/pipes.py`

 * *Files identical despite different names*

### Comparing `anvil-app-server-1.8.0/anvil_downlink_worker/__init__.py` & `anvil-app-server-1.9.0/anvil_downlink_worker/__init__.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,253 +1,253 @@
-from __future__ import absolute_import
-import ast, sys, imp, importlib
-
-# The downlink may need to coexist with the Uplink (for example in the standalone App Server).
-# In these deployments, the downlink's version of the 'anvil' module is shipped as
-# anvil_downlink_worker.anvil, and so we do some path gymnastics to load it from there:
-old_path = sys.path
-sys.path = __path__ + sys.path
-import anvil
-sys.path = old_path
-
-import anvil.server
-from anvil import _server, _serialise, _threaded_server, _form_templating
-
-if sys.version_info[0] < 3:
-    from .exec2 import do_exec
-else:
-    from .exec3 import do_exec
-
-_server._do_call = _threaded_server.do_call
-_serialise.holding_reqresps = True # Don't do anything until we've loaded apps
-
-
-def find(lst, f):
-    for item in lst:
-        if f(item):
-            return item
-
-
-def find_in_app(app, mod_name):
-    return find(app.get('server_modules', []), lambda m: m['name'] == mod_name) or \
-           find(app.get('modules', []), lambda m: m['name'] == mod_name)
-
-
-class ErrorLoadingUserCode(Exception):
-    def __init__(self, exc):
-        self.exc = exc
-        Exception.__init__(self, "Error loading user code: " + str(exc))
-
-
-# Our jobs:
-#
-# 1. Assemble a virtual filesystem corresponding to an app's source code
-# 2. (for Python 3 back-compatibility:) Intercept requests to import top-level modules in the main app,
-#    and instead load the module in its main-app package, then alias it into sys.modules
-#
-class SimpleLoader(object):
-    def __init__(self, module, real_name=None):
-        self._module = module
-        self._real_name = real_name
-
-    def load_module(self, name):
-        #print("Loading: " + name)
-        if name in sys.modules:
-            return sys.modules[name]
-
-        real_name = self._real_name or name
-
-        mod = self._module.get("module_object") or imp.new_module(real_name)
-        sys.modules[real_name] = mod
-        # Grungy horrid double-loading hack for Python 3
-        if name != real_name:
-            sys.modules[name] = mod
-
-        if self._module.get('is_package'):
-            mod.__path__ = []
-
-        if 'code' in self._module:
-            try:
-                do_exec(compile(self._module['code'], real_name.replace(".", "/") + '.py', 'exec'), mod.__dict__)
-            except ErrorLoadingUserCode as e:
-                raise
-            except Exception as e:
-                raise ErrorLoadingUserCode(e)
-
-        # Belt and braces? (honestly not sure about this -M)
-        sys.modules[name] = mod
-
-        return mod
-
-
-class AppModuleFinder(object):
-
-    def __init__(self):
-        self._app = None
-        self._modules = {}
-        self._main_package = ''
-
-    def _load_mods(self, app_spec, prefix=''):
-        for module in app_spec.get('modules', []) + app_spec.get('server_modules', []):
-            self._modules[prefix + module['name']] = module
-
-        for form in app_spec.get('forms', []):
-            self._modules[prefix + form['class_name']] = form
-
-            runtime_version = app_spec.get('runtime_options', {}).get('version', 0)
-            if runtime_version < 2:
-                template_mod = sys.modules['anvil']
-            else:
-                modname = prefix + form['class_name']
-                if not form.get('is_package'):
-                    modname = ".".join(modname.split(".")[:-1])
-                modname += "._anvil_designer"
-                if modname in self._modules:
-                    template_mod = self._modules[modname]['module_object']
-                else:
-                    template_mod = imp.new_module(modname)
-                    self._modules[modname] = {'module_object': template_mod}
-
-            leaf_name = form['class_name'].split(".")[-1]
-            if runtime_version < 3:
-                # TODO: Decide whether we want this in runtime V3. Right now it explodes on forms without containers.
-                setattr(template_mod, leaf_name+"Template", _form_templating.mk_template_class(form))
-
-
-    def set_app(self, app_spec):
-        self._app = app_spec
-        self._main_package = app_spec.get('package_name', 'main_app_package')
-        _form_templating.packages_by_app_id[''] = self._main_package
-
-        deps = self._app.get('dependency_code', {})
-        for dep_id in deps:
-            dep = deps[dep_id]
-            if 'package_name' in dep:
-                _form_templating.packages_by_app_id[dep_id] = dep['package_name']
-                self._modules[dep['package_name']] = {'is_package': True}
-                self._load_mods(dep, dep['package_name']+".")
-
-        self._modules[self._main_package] = {'is_package': True}
-        self._load_mods(self._app, self._main_package+".")
-
-    def get_main_package(self):
-        return self._main_package
-
-    def find_module(self, name, path=None):
-        #print("Finding: " + name)
-        #print(list(self._modules))
-        mod = self._modules.get(name)
-        if mod is not None:
-            return SimpleLoader(mod)
-
-        # Hack: Intercept top-level import requests
-
-        #print("Initial miss on %s, trying %s" % (name, self._main_package+"."+name))
-        mod = self._modules.get(self._main_package+"."+name)
-        if mod is not None:
-            return SimpleLoader(mod, self._main_package+"."+name)
-
-    def app_is_loaded(self):
-        return self._app is not None
-
-
-module_finder = AppModuleFinder()
-sys.meta_path.append(module_finder)
-
-modules_to_import = []
-
-def load_app(app):
-    global modules_to_import
-
-    module_finder.set_app(app)
-
-    app_package = module_finder.get_main_package()
-    modules_to_import = [app_package + "." + m['name'] for m in app.get("server_modules", [])]
-
-    deps = app.get('dependency_code', {})
-    for dep_app in deps.values():
-        if "package_name" in dep_app:
-            modules_to_import += [dep_app["package_name"] + "." + m['name'] for m in dep_app.get("server_modules", [])]
-
-    # We have our app now. Anyone who's waiting should go ahead and execute.
-    _serialise.release_reqresps()
-
-
-_initial_import_done = False
-
-
-def load_app_modules():
-    """Call from _threaded_server when the environment is ready to import all server modules in this app"""
-    global _initial_import_done
-    if _initial_import_done: return
-    try:
-        for n in modules_to_import:
-            importlib.import_module(n)
-    except ErrorLoadingUserCode as e:
-        raise e.exc
-    _initial_import_done = True
-
-
-repl_scopes = {}
-
-def run_repl(code, scope):
-    module_ast = ast.parse(code, "<input>", "exec")
-    node_list = module_ast.body
-
-    if not node_list:
-        return
-
-    if isinstance(node_list[-1], ast.Expr):
-        to_run_exec, to_run_interactive = node_list[:-1], node_list[-1:]
-    else:
-        to_run_exec, to_run_interactive = node_list, []
-
-    if to_run_exec:
-        cobj = compile(ast.Module(to_run_exec, type_ignores=[]), "<input>", "exec")
-        do_exec(cobj, scope)
-    if to_run_interactive:
-        cobj = compile(ast.Interactive(to_run_interactive), "<input>", "single")
-        do_exec(cobj, scope)
-
-
-def handle_incoming_call(msg, send_to_host):
-    if msg['type'].startswith("LAUNCH_BACKGROUND"):
-        anvil.server.task_state = {}
-
-    if not module_finder.app_is_loaded():
-        if msg.get('app'):
-            load_app(msg['app'])
-        else:
-            send_to_host({"type": "GET_APP", "id": _threaded_server.gen_id(), "originating-call": msg['id'],
-                          "app-id": msg["app-id"], "app-version": msg["app-version"]})
-
-    # This part happens out here because uplinks can't do REPLs:
-    run_fn = None
-    if msg['type'] == "LAUNCH_REPL":
-        def run_fn():
-            send_to_host({'output': "Application loaded\n", 'id': msg['id']})
-            raise _threaded_server.SendNoResponse
-
-    elif msg["type"] == "REPL_COMMAND":
-        # adding __package__ allows relative imports to work in the repl
-        # we add the repl scope now if it doesn't exist
-        # since we don't have the package name when we launch the repl
-        # for convenience we include anvil (which also adds anvil.server)
-        scope = repl_scopes.setdefault(
-            msg["repl"], {"anvil": anvil, "__package__": module_finder.get_main_package() or None}
-        )
-
-        def run_fn():
-            run_repl(msg['command'], scope)
-
-    elif msg['type'] == "TERMINATE_REPL":
-        repl_scopes.pop(msg['repl'], None)
-        send_to_host({"id": msg['repl'], "response": None})
-        send_to_host({"id": msg['id'], "response": None})
-        return
-
-    try:
-        _threaded_server.IncomingRequest(msg, load_app_modules,
-                                         run_fn=run_fn,
-                                         dump_task_state=(msg['type'].startswith("LAUNCH_BACKGROUND")))
-    except:
-        send_to_host(_server._report_exception(msg['id']))
+from __future__ import absolute_import
+import ast, sys, imp, importlib
+
+# The downlink may need to coexist with the Uplink (for example in the standalone App Server).
+# In these deployments, the downlink's version of the 'anvil' module is shipped as
+# anvil_downlink_worker.anvil, and so we do some path gymnastics to load it from there:
+old_path = sys.path
+sys.path = __path__ + sys.path
+import anvil
+sys.path = old_path
+
+import anvil.server
+from anvil import _server, _serialise, _threaded_server, _form_templating
+
+if sys.version_info[0] < 3:
+    from .exec2 import do_exec
+else:
+    from .exec3 import do_exec
+
+_server._do_call = _threaded_server.do_call
+_serialise.holding_reqresps = True # Don't do anything until we've loaded apps
+
+
+def find(lst, f):
+    for item in lst:
+        if f(item):
+            return item
+
+
+def find_in_app(app, mod_name):
+    return find(app.get('server_modules', []), lambda m: m['name'] == mod_name) or \
+           find(app.get('modules', []), lambda m: m['name'] == mod_name)
+
+
+class ErrorLoadingUserCode(Exception):
+    def __init__(self, exc):
+        self.exc = exc
+        Exception.__init__(self, "Error loading user code: " + str(exc))
+
+
+# Our jobs:
+#
+# 1. Assemble a virtual filesystem corresponding to an app's source code
+# 2. (for Python 3 back-compatibility:) Intercept requests to import top-level modules in the main app,
+#    and instead load the module in its main-app package, then alias it into sys.modules
+#
+class SimpleLoader(object):
+    def __init__(self, module, real_name=None):
+        self._module = module
+        self._real_name = real_name
+
+    def load_module(self, name):
+        #print("Loading: " + name)
+        if name in sys.modules:
+            return sys.modules[name]
+
+        real_name = self._real_name or name
+
+        mod = self._module.get("module_object") or imp.new_module(real_name)
+        sys.modules[real_name] = mod
+        # Grungy horrid double-loading hack for Python 3
+        if name != real_name:
+            sys.modules[name] = mod
+
+        if self._module.get('is_package'):
+            mod.__path__ = []
+
+        if 'code' in self._module:
+            try:
+                do_exec(compile(self._module['code'], real_name.replace(".", "/") + '.py', 'exec'), mod.__dict__)
+            except ErrorLoadingUserCode as e:
+                raise
+            except Exception as e:
+                raise ErrorLoadingUserCode(e)
+
+        # Belt and braces? (honestly not sure about this -M)
+        sys.modules[name] = mod
+
+        return mod
+
+
+class AppModuleFinder(object):
+
+    def __init__(self):
+        self._app = None
+        self._modules = {}
+        self._main_package = ''
+
+    def _load_mods(self, app_spec, prefix=''):
+        for module in app_spec.get('modules', []) + app_spec.get('server_modules', []):
+            self._modules[prefix + module['name']] = module
+
+        for form in app_spec.get('forms', []):
+            self._modules[prefix + form['class_name']] = form
+
+            runtime_version = app_spec.get('runtime_options', {}).get('version', 0)
+            if runtime_version < 2:
+                template_mod = sys.modules['anvil']
+            else:
+                modname = prefix + form['class_name']
+                if not form.get('is_package'):
+                    modname = ".".join(modname.split(".")[:-1])
+                modname += "._anvil_designer"
+                if modname in self._modules:
+                    template_mod = self._modules[modname]['module_object']
+                else:
+                    template_mod = imp.new_module(modname)
+                    self._modules[modname] = {'module_object': template_mod}
+
+            leaf_name = form['class_name'].split(".")[-1]
+            if runtime_version < 3:
+                # TODO: Decide whether we want this in runtime V3. Right now it explodes on forms without containers.
+                setattr(template_mod, leaf_name+"Template", _form_templating.mk_template_class(form))
+
+
+    def set_app(self, app_spec):
+        self._app = app_spec
+        self._main_package = app_spec.get('package_name', 'main_app_package')
+        _form_templating.packages_by_app_id[''] = self._main_package
+
+        deps = self._app.get('dependency_code', {})
+        for dep_id in deps:
+            dep = deps[dep_id]
+            if 'package_name' in dep:
+                _form_templating.packages_by_app_id[dep_id] = dep['package_name']
+                self._modules[dep['package_name']] = {'is_package': True}
+                self._load_mods(dep, dep['package_name']+".")
+
+        self._modules[self._main_package] = {'is_package': True}
+        self._load_mods(self._app, self._main_package+".")
+
+    def get_main_package(self):
+        return self._main_package
+
+    def find_module(self, name, path=None):
+        #print("Finding: " + name)
+        #print(list(self._modules))
+        mod = self._modules.get(name)
+        if mod is not None:
+            return SimpleLoader(mod)
+
+        # Hack: Intercept top-level import requests
+
+        #print("Initial miss on %s, trying %s" % (name, self._main_package+"."+name))
+        mod = self._modules.get(self._main_package+"."+name)
+        if mod is not None:
+            return SimpleLoader(mod, self._main_package+"."+name)
+
+    def app_is_loaded(self):
+        return self._app is not None
+
+
+module_finder = AppModuleFinder()
+sys.meta_path.append(module_finder)
+
+modules_to_import = []
+
+def load_app(app):
+    global modules_to_import
+
+    module_finder.set_app(app)
+
+    app_package = module_finder.get_main_package()
+    modules_to_import = [app_package + "." + m['name'] for m in app.get("server_modules", [])]
+
+    deps = app.get('dependency_code', {})
+    for dep_app in deps.values():
+        if "package_name" in dep_app:
+            modules_to_import += [dep_app["package_name"] + "." + m['name'] for m in dep_app.get("server_modules", [])]
+
+    # We have our app now. Anyone who's waiting should go ahead and execute.
+    _serialise.release_reqresps()
+
+
+_initial_import_done = False
+
+
+def load_app_modules():
+    """Call from _threaded_server when the environment is ready to import all server modules in this app"""
+    global _initial_import_done
+    if _initial_import_done: return
+    try:
+        for n in modules_to_import:
+            importlib.import_module(n)
+    except ErrorLoadingUserCode as e:
+        raise e.exc
+    _initial_import_done = True
+
+
+repl_scopes = {}
+
+def run_repl(code, scope):
+    module_ast = ast.parse(code, "<input>", "exec")
+    node_list = module_ast.body
+
+    if not node_list:
+        return
+
+    if isinstance(node_list[-1], ast.Expr):
+        to_run_exec, to_run_interactive = node_list[:-1], node_list[-1:]
+    else:
+        to_run_exec, to_run_interactive = node_list, []
+
+    if to_run_exec:
+        cobj = compile(ast.Module(to_run_exec, type_ignores=[]), "<input>", "exec")
+        do_exec(cobj, scope)
+    if to_run_interactive:
+        cobj = compile(ast.Interactive(to_run_interactive), "<input>", "single")
+        do_exec(cobj, scope)
+
+
+def handle_incoming_call(msg, send_to_host):
+    if msg['type'].startswith("LAUNCH_BACKGROUND"):
+        anvil.server.task_state = {}
+
+    if not module_finder.app_is_loaded():
+        if msg.get('app'):
+            load_app(msg['app'])
+        else:
+            send_to_host({"type": "GET_APP", "id": _threaded_server.gen_id(), "originating-call": msg['id'],
+                          "app-id": msg["app-id"], "app-version": msg["app-version"]})
+
+    # This part happens out here because uplinks can't do REPLs:
+    run_fn = None
+    if msg['type'] == "LAUNCH_REPL":
+        def run_fn():
+            send_to_host({'output': "Application loaded\n", 'id': msg['id']})
+            raise _threaded_server.SendNoResponse
+
+    elif msg["type"] == "REPL_COMMAND":
+        # adding __package__ allows relative imports to work in the repl
+        # we add the repl scope now if it doesn't exist
+        # since we don't have the package name when we launch the repl
+        # for convenience we include anvil (which also adds anvil.server)
+        scope = repl_scopes.setdefault(
+            msg["repl"], {"anvil": anvil, "__package__": module_finder.get_main_package() or None}
+        )
+
+        def run_fn():
+            run_repl(msg['command'], scope)
+
+    elif msg['type'] == "TERMINATE_REPL":
+        repl_scopes.pop(msg['repl'], None)
+        send_to_host({"id": msg['repl'], "response": None})
+        send_to_host({"id": msg['id'], "response": None})
+        return
+
+    try:
+        _threaded_server.IncomingRequest(msg, load_app_modules,
+                                         run_fn=run_fn,
+                                         dump_task_state=(msg['type'].startswith("LAUNCH_BACKGROUND")))
+    except:
+        send_to_host(_server._report_exception(msg['id']))
```

### Comparing `anvil-app-server-1.8.0/anvil_downlink_worker/anvil/__init__.py` & `anvil-app-server-1.9.0/anvil_downlink_worker/anvil/__init__.py`

 * *Files identical despite different names*

### Comparing `anvil-app-server-1.8.0/anvil_downlink_worker/anvil/_components.py` & `anvil-app-server-1.9.0/anvil_downlink_worker/anvil/_components.py`

 * *Files identical despite different names*

### Comparing `anvil-app-server-1.8.0/anvil_downlink_worker/anvil/_form_templating.py` & `anvil-app-server-1.9.0/anvil_downlink_worker/anvil/_form_templating.py`

 * *Files identical despite different names*

### Comparing `anvil-app-server-1.8.0/anvil_downlink_worker/anvil/_serialise.py` & `anvil-app-server-1.9.0/anvil_downlink_worker/anvil/_serialise.py`

 * *Files identical despite different names*

### Comparing `anvil-app-server-1.8.0/anvil_downlink_worker/anvil/_server.py` & `anvil-app-server-1.9.0/anvil_downlink_worker/anvil/_server.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,1610 +1,1610 @@
-# Helpers for implementing anvil.server.
-# Used in uplink, downlink and pypy-sandbox.
-import importlib
-
-import anvil
-import traceback
-import numbers
-import sys
-import re
-import json
-import math
-import anvil.tz
-import functools
-
-_do_call = None
-
-string_type = str if sys.version_info >= (3,) else basestring
-long_type = int if sys.version_info >= (3,) else long
-
-POS_INFINITY = float("inf")
-NEG_INFINITY = float("-inf")
-
-_value_types = {}
-_serialization_helpers = {} # {module_name: helper_fn}
-
-class LiveObjectProxy(anvil.LiveObject):
-
-    def __init__(self,spec,known_methods=None):
-        for k in ["itemCache", "iterItems"]:
-            if spec.get(k, {}) is None:
-                del spec[k]
-
-        if known_methods is not None:
-            if spec.get("methods") is None:
-                spec["methods"] = known_methods[spec["backend"]]
-            else:
-                known_methods[spec["backend"]] = spec["methods"]
-        anvil.LiveObject.__init__(self, spec)
-
-    def __getattr__(self, item):
-        if item in self._spec["methods"]:
-            def item_fn(*args, **kwargs):
-                return _do_call(args, kwargs, fn_name=item, live_object=self)
-
-            return item_fn
-        else:
-            raise AttributeError(item)
-
-    def __getitem__(self, item):
-
-        if "__anvil_iter_page__" in self._spec["methods"]:
-            if isinstance(item, (int,long_type)):
-                if item < 0:
-                    raise IndexError("list index cannot be negative")
-
-                iter = LiveObjectProxy.Iter(self, item)
-                try:
-                    return iter.next()
-                except StopIteration:
-                    raise IndexError("list index out of range")
-            elif isinstance(item, slice):
-                if (item.start and item.start < 0) or (item.stop and item.stop < 0) or (item.step and item.step < 0):
-                    raise Exception("list slice indices and step cannot be negative")
-                return LiveObjectProxy.Iter(self, item.start, item.stop, item.step)
-
-
-        if item in self._spec.get("itemCache", {}):
-            return self._spec["itemCache"][item]
-
-        getitem = self.__getattr__("__getitem__")
-
-        try:
-            return getitem(item)
-        except AnvilWrappedError as e:
-            raise _deserialise_exception(e.error_obj)
-
-    def __setitem__(self, key, value):
-        if key in self._spec.get("itemCache", {}):
-            del self._spec["itemCache"][key]
-
-        setitem = self.__getattr__("__setitem__")
-        try:
-            r = setitem(key, value)
-        except AnvilWrappedError as e:
-            raise _deserialise_exception(e.error_obj)
-
-        if "itemCache" in self._spec and (isinstance(value, string_type) or isinstance(value, numbers.Number) or isinstance(value, bool) or value is None):
-            self._spec["itemCache"][key] = value
-
-        return r
-
-    class Iter:
-        def __init__(self, live_object, start=None, stop=None, step=None):
-            self._live_object = live_object
-
-            i = live_object._spec.get("iterItems", {})
-            self._idx = start if start is not None else 0
-            self._items = i.get("items", None)
-            self._next_page = i.get("nextPage", None)
-            self._stop = stop
-            self._step = step if step is not None else 1
-
-        def _fetch_state(self):
-            r = _do_call([self._next_page], {}, fn_name="__anvil_iter_page__", live_object=self._live_object)
-            self._items = r["items"]
-            self._next_page = r.get("nextPage", None)
-
-        def __iter__(self):
-            return self
-
-        def next(self):
-            if self._items is None:
-                try:
-                    self._fetch_state()
-                except AnvilWrappedError as e:
-                    raise _deserialise_exception(e.error_obj)
-
-            if self._idx < len(self._items) and (self._stop is None or self._idx < self._stop):
-                r = self._items[self._idx]
-                self._idx += self._step
-                return r
-
-            if self._next_page is None or (self._stop is not None and self._idx >= self._stop):
-                raise StopIteration
-
-            self._idx -= len(self._items) if self._items is not None else self._idx
-            if self._stop is not None:
-                self._stop -= len(self._items) if self._items is not None else 0
-            self._items = None
-            return self.next()
-
-        def __next__(self):
-            return self.next()
-
-    def __iter__(self):
-        if "__anvil_iter_page__" in self._spec["methods"]:
-            return LiveObjectProxy.Iter(self)
-        else:
-            raise Exception("Not iterable: <LiveObject: %s>" % self._spec.get("backend", "INVALID"))
-
-    def __bool__(self):
-        if "__nonzero__" in self._spec["methods"]:
-            return self.__getattr__("__nonzero__")()
-        else:
-            return True
-
-    __nonzero__ = __bool__
-
-    def __len__(self):
-        if "__len__" in self._spec["methods"]:
-            return int(self.__getattr__("__len__")())
-        else:
-            l = 0
-            for _ in self.__iter__():
-                l += 1
-            return l
-
-
-# Wildcard for unwrap_capability
-class _CapAny(object):
-    def __repr__(self):
-        return "ANY"
-
-def _check_valid_scope(scope, name="scope"):
-    if type(scope) is not list:
-            raise TypeError("The {} of a Capabilty must be a list".format(name))
-    try:
-        return json.loads(json.dumps(scope))
-    except TypeError as e:
-        raise TypeError("The {} provided is not valid JSON data. {}".format(name, e))
-
-
-class Capability(object):
-    def __init__(self, scope, mac=None, narrow=None):
-        scope = _check_valid_scope(scope)
-        self._scope = scope
-        self._mac = mac
-        if mac is not None:
-            pass
-        elif not len(scope):
-            raise ValueError("Cannot construct a capability with an empty scope")
-        elif scope[0] == "_":
-            raise ValueError("To construct a Capability from scratch, its scope cannot start with ['_']")
-
-        self._narrow = narrow or []
-        self._do_apply_update = None
-        self._do_get_update = None
-        self._queued_update = {}
-        self._hash = None
-
-    @property
-    def scope(self):
-        return self._scope + self._narrow
-
-    def narrow(self, narrowing_suffix):
-        narrowing_suffix = _check_valid_scope(narrowing_suffix, "narrow argument")
-        return Capability(self._scope, self._mac, self._narrow + narrowing_suffix)
-
-    def __repr__(self):
-        return "<anvil.server.Capability:{}>".format(self.scope)
-
-    def __eq__(self, other):
-        if type(other) is not Capability:
-            return NotImplemented
-        return self.scope == other.scope
-
-    def __hash__(self):
-        if self._hash is None:
-            self._hash = hash(json.dumps(self.scope))
-        return self._hash
-
-    def set_update_handler(self, apply_update, get_update=None):
-        self._do_apply_update = apply_update
-        self._do_get_update = get_update
-
-    # RPC machinery:
-    # An update has arrived from a server call. Default behaviour: Merge if it's a dict, overwrite if it isn't
-    def _apply_update(self, update):
-        if self._do_apply_update is not None:
-            self._do_apply_update(update)
-
-        if self._do_get_update is None:
-            # Default update propagation rules
-            if isinstance(update, dict):
-                self._queued_update.update(**update)
-            else:
-                self._queued_update = update
-
-    send_update = _apply_update
-
-    # RPC machinery:
-    # We're about to return from a server call which passed this capability in; do we have an update for them?
-    # None -> nothing to send
-    def _get_update(self):
-        if self._do_get_update is not None:
-            return self._do_get_update()
-        else:
-            return None if self._queued_update == {} else self._queued_update
-
-    # Sentinel value for unwrap_capability
-    ANY = _CapAny()
-
-#!defFunction(anvil.server,list,capability,scope_pattern)!2: "Checks that its first argument is a valid Capability, and that its scope matches the supplied pattern.\n\nTo match, the scope must:\n - Be at least as broad as the pattern (ie the same length or shorter)\n- Contain the same values in the same position as the pattern - unless that position in the pattern is Capability.ANY, which matches any value\n\nReturns a list of matched scope elements, of the same length as the pattern. (If the scope was broader than required, missing elements are set to None.)" ["unwrap_capability"]
-def unwrap_capability(cap, scope_pattern):
-    if type(cap) is not Capability:
-        raise TypeError("Not a valid Capability: found {}".format(type(cap).__name__))
-    if type(scope_pattern) is not list:
-        raise TypeError("scope_pattern should be a list, not {}".format(type(scope_pattern).__name__))
-
-    scope = cap.scope
-    ret = [None] * len(scope_pattern)
-
-    if len(scope) > len(scope_pattern):
-        raise ValueError("Capability is too narrow: required %s; got %s" % (scope_pattern, scope))
-
-    for i in range(len(scope)):
-        if scope_pattern[i] is Capability.ANY or scope[i] == scope_pattern[i]:
-            ret[i] = scope[i]
-        else:
-            raise ValueError("Incorrect Capability: required %s; got %s" % (scope_pattern, cap.scope))
-
-    return ret
-
-# DEPRECATED: replaced by unwrap_capability - included here for Backwards compatibility
-Capability.require = staticmethod(unwrap_capability)
-
-
-class SerializationInfo(object):
-    def __init__(self, fromdata=None, remote_is_trusted=False):
-        self._txdata = {}
-        self._localdata = {}
-        self._defaultkey = None
-        self._trusted = remote_is_trusted
-        self._enable_txdata = True
-        if fromdata is None:
-            pass
-        elif type(fromdata) is dict:
-            self._txdata[":GLOBAL"] = fromdata
-        else:
-            it = iter(fromdata)
-            for k, v in zip(it, it):
-                self._txdata[k] = v
-
-    def __bool__(self):
-        return bool(self._enable_txdata)
-
-    __nonzero__ = __bool__
-
-    def _to_json(self):
-        if len(self._txdata) == 1 and ":GLOBAL" in self._txdata:
-            return self._txdata[":GLOBAL"]
-        else:
-            r = []
-            for k, v in self._txdata.items():
-                r.append(k)
-                r.append(v)
-            return r
-
-    def _resolve_key(self, key):
-        if key is None:
-            return self._defaultkey
-        elif isinstance(key, type):
-            try:
-                return key.SERIALIZATION_INFO[0]
-            except AttributeError:
-                return key.__module__ + "." + key.__name__
-        else:
-            return ":" + str(key)
-
-    def _set_default_key(self, key):
-        self._defaultkey = key
-
-    def _set_txdata_available(self, enable):
-        self._enable_txdata = enable
-    
-    def _set_data_factory(self, _data, resolved_key, factory):
-        data = _data.get(resolved_key)
-        if data is None:
-            data = _data[resolved_key] = factory()
-        return data
-
-    def shared_data(self, key=None, transmitted_data_factory=dict, local_data_factory=dict):
-        key = self._resolve_key(key)
-        localdata = self._set_data_factory(self._localdata, key, local_data_factory)
-        if not self._enable_txdata:
-            return None, localdata
-        txdata = self._set_data_factory(self._txdata, key, transmitted_data_factory)
-        return txdata, localdata
-
-    @property
-    def remote_is_trusted(self):
-        return self._trusted
-
-    @property
-    def local_is_trusted(self):
-        return anvil.is_server_side()
-
-    def __repr__(self):
-        # TODO adjust for public api
-        return "SerializationInfo<" + repr(self._txdata) + ", " + repr(self._localdata) + ">"
-
-
-# Backwards compatibility: If you use SerializationInfo like a dict, it man works like  if you use it like a dict
-def _wrap_global_dict(attr_name):
-    def f(self, *args, **kws):
-        transmitted_data = self.shared_data("GLOBAL")[0]
-        if transmitted_data is None:
-            # using the old API so better to throw here
-            raise RuntimeError("This object is part of shared_data; you cannot access shared_data from its __serialize__ method.")
-        return getattr(transmitted_data, attr_name)(*args, **kws)
-    return f
-
-
-for method in ["__getitem__", "__setitem__", "__delitem__", "__iter__", "__len__", "__contains__", "keys", "items",
-               "values", "get", "pop", "popitem", "clear", "update", "setdefault"]:
-    setattr(SerializationInfo, method, _wrap_global_dict(method))
-
-
-# DEPRECATED: there is no longer any reason to inherit from this
-class Serializable(object):
-    SERIALIZATION_INFO = None
-
-    def __serialize__(self, info):
-        return self.__dict__
-
-    # You only need one of __deserialize__ (called instead of __init__)
-    # or __new_deserialized__ (called instead of __new__+__init__).
-    # (Of the two, you almost always want __deserialize__.)
-    def __deserialize__(self, from_data, info):
-        self.__dict__.update(from_data)
-
-    @classmethod
-    def __new_deserialized__(cls, from_data, info):
-        obj = cls.__new__(cls)
-        obj.__dict__.update(from_data)
-        return obj
-
-
-# Add-in for maintaining object identity across serialization
-class SerializeWithIdentity(object):
-    @classmethod
-    def __new_deserialized__(cls, from_data, global_data):
-        clsname, _ = cls.SERIALIZATION_INFO
-        cache = global_data.get(clsname)
-        if cache is None:
-            cache = global_data[clsname] = {}
-        my_id = from_data[0]
-        # We use global_data to cache instances we're constructing
-        # (non-JSONable keys certainly won't conflict with other global_data users)
-        obj = cache.get(my_id)
-        if obj is None:
-            obj = cache[my_id] = cls.__new__(cls)
-
-        if len(from_data) > 1:
-            obj.__deserialize__(from_data[1], global_data)
-
-        return obj
-
-    def __serialize__(self, global_data):
-        my_id, gd = self._serialization_key if hasattr(self, "_serialization_key") else (None, None)
-        if gd is global_data:
-            return [my_id]
-
-        clsname, _ = self.SERIALIZATION_INFO
-        my_id = global_data.get(clsname+"_max", 0)
-        global_data[clsname+"_max"] = my_id + 1
-
-        self._serialization_key = (my_id, global_data)
-
-        data = self.__serialize_once__(global_data)
-        if isinstance(data, dict):
-            data = dict(data)
-            data.pop("_serialization_key", None)
-
-        return [my_id, data]
-
-
-def portable_class(cls, name=None):
-    def register(cls, name):
-        if not hasattr(cls, "__new__"):
-            raise TypeError("Portable classes must be new-style classes (inherit from object). %s is not a new-style class." % repr(cls))
-        if name is None:
-            name = cls.__module__ + "." + cls.__name__
-        elif not isinstance(name, str):
-            raise TypeError("The second argument to portable_class must be a str")
-        _value_types[name] = cls
-        cls.SERIALIZATION_INFO = (name, cls)
-        return cls
-
-    if name is None and isinstance(cls, str):
-        name = cls
-        return lambda cls: register(cls, name)
-    else:
-        return register(cls, name)
-
-
-# Old name, for apps written before portable classes were released
-serializable_type = portable_class
-
-
-class LazyMedia(anvil.Media):
-    def __init__(self, spec):
-        if isinstance(spec,LazyMedia):
-            spec = spec._spec
-        self._spec = spec
-        self._details = None
-        self._fetched = None
-
-    def _fetch(self):
-        if self._details is None:
-            import anvil.server
-            self._fetched = anvil.server.call("anvil.private.fetch_lazy_media", self._spec)
-        return self._fetched
-
-    def _get(self, key, attr=None):
-        if attr is None:
-            attr = key
-        return self._spec[key] if key in self._spec else getattr(self._fetch(), attr)
-
-    def get_name(self):
-        try:
-            return self._get("name")
-        except AnvilWrappedError as e:
-            raise _deserialise_exception(e.error_obj)
-
-    def get_url(self, download=True):
-        return anvil.server.call("anvil.private.get_lazy_media_url", self, download)
-
-    def get_content_type(self):
-        try:
-            return self._get("mime-type", "content_type")
-        except AnvilWrappedError as e:
-            raise _deserialise_exception(e.error_obj)
-
-    def get_length(self):
-        try:
-            return self._get("length")
-        except AnvilWrappedError as e:
-            raise _deserialise_exception(e.error_obj)
-
-    def get_bytes(self):
-        try:
-            return self._fetch().get_bytes()
-        except AnvilWrappedError as e:
-            raise _deserialise_exception(e.error_obj)
-
-
-class AnvilWrappedError(Exception):
-    registered_type_name = None
-
-    def __init__(self, message=""):
-        if isinstance(message, dict):
-            self.manually_created = False
-            self.error_obj = message
-        else:
-            self.manually_created = True
-            self.error_obj = {"message": str(message), "trace": []}
-            t = type(self).registered_type_name
-            if t is not None:
-                self.error_obj["type"] = t
-        self.message = self.error_obj.get("message", "")
-        Exception.__init__(self, self.message)
-
-    def __repr__(self):
-        r = Exception.__repr__(self)
-        if type(self) is not AnvilWrappedError:
-            return r
-        eo_type = self.error_obj.get("type")
-        if eo_type is None:
-            return r
-
-        return "AnvilWrappedError" + "(" + eo_type + r[len("AnvilWrappedError"):] + ")"
-
-
-def augment_exception(exc_class):
-    def f(error_obj):
-        e = exc_class(error_obj['message'])
-        e._anvil_error_obj = error_obj
-        return e
-    return f
-
-_named_exceptions = {
-    "KeyError": augment_exception(KeyError)
-}
-
-
-def _register_exception_type(name, cls):
-    _named_exceptions[name] = cls
-    cls.registered_type_name = name
-
-
-def _deserialise_exception(error_obj):
-    return _named_exceptions.get(error_obj.get("type"), AnvilWrappedError)(error_obj)
-
-
-def get_liveobject_cache_filter_spec(input_data):
-    """Returns a specification of a filter for LiveObject cache updates, which passes only LiveObjects present in input_data"""
-    spec = {}
-
-    def f(data):
-        if isinstance(data, list):
-            for i in data: f(i)
-        elif isinstance(data, dict):
-            for k,v in data.items(): f(v)
-        elif isinstance(data, LiveObjectProxy):
-            b = spec.get(data._spec["backend"])
-            if b is None:
-                b = spec[data._spec["backend"]] = set()
-            b.add(data._spec["id"])
-
-    f(input_data)
-    return spec
-
-
-def combine_cache_updates(updates, new_updates, filter_spec):
-    if updates is None:
-        updates = {}
-
-    for k in new_updates:
-        permitted_ids = filter_spec.get(k)
-        if permitted_ids is None:
-            continue
-        caches = updates.get(k)
-        if caches is None:
-            caches = updates[k] = dict()
-        for id in new_updates[k]:
-            if id not in permitted_ids:
-                continue
-            caches[id] = new_updates[k][id]
-
-
-def apply_cache_updates(cache_updates, objects_to_walk):
-    """Recursively walk an object tree, applying cache updates wherever necessary"""
-
-    def f(data):
-        if isinstance(data, list):
-            for i in data: f(i)
-        elif isinstance(data, dict):
-            for k,v in data.items(): f(v)
-        elif isinstance(data, LiveObjectProxy):
-            update = cache_updates.get(data._spec["backend"], {})
-            if data._spec["id"] in update:
-                data._spec["itemCache"] = update[data._spec["id"]]
-
-    f(objects_to_walk)
-
-
-class MaybeWrappedError(Exception):
-    def __init__(self, message=""):
-        if isinstance(message, dict):
-            Exception.__init__(self, message["message"])
-        else:
-            Exception.__init__(self, message)
-
-
-class SerializationError(MaybeWrappedError):
-    pass
-
-
-class InternalError(MaybeWrappedError):
-    pass
-
-
-class InvalidResponseError(MaybeWrappedError):
-    pass
-
-
-class RuntimeUnavailableError(MaybeWrappedError):
-    pass
-
-
-class UplinkDisconnectedError(MaybeWrappedError):
-    pass
-
-
-class ExecutionTerminatedError(MaybeWrappedError):
-    pass
-
-
-class TimeoutError(MaybeWrappedError):
-    pass
-
-
-class QuotaExceededError(MaybeWrappedError):
-    pass
-
-
-class NoServerFunctionError(AnvilWrappedError):
-    pass
-
-
-class CookieError(AnvilWrappedError):
-    pass
-
-
-class _FailError(MaybeWrappedError):
-    pass
-
-
-class BackgroundTaskError(MaybeWrappedError):
-    pass
-
-
-class BackgroundTaskNotFound(MaybeWrappedError):
-    pass
-
-
-class BackgroundTaskKilled(MaybeWrappedError):
-    pass
-
-
-class PermissionDenied(MaybeWrappedError):
-    pass
-
-
-class ServiceNotAdded(MaybeWrappedError):
-    pass
-
-
-
-_register_exception_type("anvil.server.SerializationError", SerializationError)
-_register_exception_type("anvil.server.InternalError", InternalError)
-_register_exception_type("anvil.server.InvalidResponseError", InvalidResponseError)
-_register_exception_type("anvil.server.RuntimeUnavailableError", RuntimeUnavailableError)
-_register_exception_type("anvil.server.UplinkDisconnectedError", UplinkDisconnectedError)
-_register_exception_type("anvil.server.ExecutionTerminatedError", ExecutionTerminatedError)
-_register_exception_type("anvil.server.TimeoutError", TimeoutError)
-_register_exception_type("anvil.server.QuotaExceededError", QuotaExceededError)
-_register_exception_type("anvil.server.NoServerFunctionError", NoServerFunctionError)
-_register_exception_type("anvil.server.CookieError", CookieError)
-_register_exception_type("anvil.server._FailError", _FailError)
-_register_exception_type("anvil.server.BackgroundTaskError", BackgroundTaskError)
-_register_exception_type("anvil.server.BackgroundTaskNotFound", BackgroundTaskNotFound)
-_register_exception_type("anvil.server.PermissionDenied", PermissionDenied)
-_register_exception_type("anvil.server.ServiceNotAdded", ServiceNotAdded)
-
-
-
-def _report_exception(request_id=None):
-    exc_type, exc_value, exc_traceback = sys.exc_info()
-    tb = traceback.extract_tb(exc_traceback)
-
-    trace = [(filename.replace("\\","/"), lineno) for (filename, lineno, _, _) in tb]
-    trace.reverse()
-
-    # Last element of trace is where we called into user code. Remove it.
-    trace.pop()
-
-    if isinstance(exc_value, AnvilWrappedError):
-        if not exc_value.manually_created:
-            # First element of trace is where we re-raised the exception. Remove it.
-            trace = trace[1:]
-        exc_value.error_obj["trace"] = exc_value.error_obj.get("trace", []) + trace
-        r = {
-            "error": exc_value.error_obj,
-            "id": request_id
-        }
-        return r
-    elif isinstance(exc_value, SyntaxError):
-        # Remove whole internal trace and replace it with line where error occurred.
-        trace=[(exc_value.filename, exc_value.lineno)]
-        return {
-            "error": {
-                "type": "SyntaxError",
-                "trace": trace,
-                "message": str(exc_value)
-            },
-            "id": request_id
-        }
-    elif isinstance(exc_value, MaybeWrappedError):
-        return {
-            "error": {
-                "type": "anvil.server.%s" % exc_type.__name__,
-                "trace": trace,
-                "message": str(exc_value),
-            },
-            "id": request_id
-        }
-    elif hasattr(exc_value, "_anvil_error_obj"):
-        error_obj = dict(exc_value._anvil_error_obj)
-        error_obj['trace'] = exc_value._anvil_error_obj.get("trace", []) + trace[1:]
-
-        return {
-            "error": error_obj,
-            "id": request_id
-        }
-    else:
-        return {
-            "error": {
-                "type": str(exc_type.__name__),
-                "trace": trace,
-                "message": str(exc_value),
-            },
-            "id": request_id
-        }
-
-def reconstruct_val(v, known_liveobject_methods, reconstruct_data_media=None):
-
-    for t in v["type"]:
-        if t == "DataMedia":
-            if reconstruct_data_media is None:
-                raise Exception("No data media deserialiser provided. Cannot reconstruct.")
-            return reconstruct_data_media(v)
-        elif t == "LazyMedia":
-            return LazyMedia(v)
-        elif t == "LiveObject":
-            return reconstruct_live_object(v, known_liveobject_methods)
-        elif t == "Capability":
-            return Capability(v["scope"], v["mac"])
-        elif t == "Date":
-            return parsedate(v["value"]) if v["value"] else None
-        elif t == "DateTime":
-            return parsedatetime(v["value"]) if v["value"] else None
-        elif t == "Long":
-            return long_type(v["value"])
-        elif t == "Float":
-            return float(v["value"])
-        elif t == "Primitive":
-            return v["value"]
-        elif t == "ValueType":
-            return v["typeName"]
-        elif t == "ClassType":
-            return v["typeName"]
-
-    raise Exception("Server module cannot accept an object of type '%s'" % v["type"][0])
-
-
-
-def reconstruct_live_object(d, known_methods):
-
-    # Need to fill out known_methods before we can reconstruct members:
-    if d.get('methods') is not None:
-        known_methods[d["backend"]] = d["methods"]
-
-    reconstructed_item_cache = {}
-    for k,v in d.get("itemCache", {}).items():
-        reconstructed_item_cache[k] = reconstruct_val(v, known_methods)
-    d["itemCache"] = reconstructed_item_cache
-
-    if d.get("iterItems"):
-        reconstructed_iteritems = []
-        for i in d["iterItems"]["items"]:
-            reconstructed_iteritems.append(reconstruct_val(i, known_methods))
-        d["iterItems"]["items"] = reconstructed_iteritems
-
-    return LiveObjectProxy(d, known_methods)
-
-
-def serialise_val(v, known_liveobject_methods):
-    import datetime
-    if isinstance(v, long_type) and not isinstance(v, bool):
-        return {
-            "type": ["Long"],
-            "value": str(v)
-        }
-    elif isinstance(v, float) and (v == POS_INFINITY or v == NEG_INFINITY or math.isnan(v)):
-        return {
-            "type": ["Float"],
-            "value": "Infinity" if v == POS_INFINITY else \
-                        "-Infinity" if v == NEG_INFINITY else \
-                        "NaN"
-        }
-    elif isinstance(v, (numbers.Number, bool, string_type)) or v is None:
-        return {
-            "type": ["Primitive"],
-            "value": v
-        }
-    elif isinstance(v, anvil.LiveObject):
-        return serialise_live_object(v, known_liveobject_methods)
-    elif isinstance(v, datetime.datetime):
-        s = "%04d-%02d-%02d %02d:%02d:%02d.%06d" % (v.year, v.month, v.day, v.hour, v.minute, v.second, v.microsecond)
-
-        if v.tzinfo is not None:
-            offset = v.tzinfo.utcoffset(v).total_seconds()
-        else:
-            offset = anvil.tz.tzlocal().utcoffset(v).total_seconds()
-
-        sign = "+" if offset >= 0 else "-"
-        z = "%s%02d%02d" % (sign, abs(int(offset/3600)), int((offset % 3600)/60))
-
-        return {
-            "type": ["DateTime"],
-            "value": s + z
-        }
-    elif isinstance(v, datetime.date):
-        s = "%04d-%02d-%02d" % (v.year, v.month, v.day)
-        return {
-            "type": ["Date"],
-            "value": s
-        }
-    elif isinstance(v, LazyMedia):
-        return dict(v._spec)
-    else:
-        for [n, cls] in _value_types.items():
-            if isinstance(v, cls):
-                type_name = n
-                break
-        else:
-            raise Exception("Cannot serialise object of type %s" % type(v).__name__)
-
-        return {
-            "type": ["ValueType"],
-            "typeName": type_name
-        }
-
-
-def serialise_live_object(obj, known_methods):
-    obj = obj._spec.copy()
-    obj["type"] = ["LiveObject"]
-
-    km = known_methods.get(obj["backend"])
-    if obj["methods"] == km:
-        del obj["methods"]
-    else:
-        known_methods[obj["backend"]] = obj["methods"]
-
-    serialised_item_cache = {}
-    for k,v in sorted(obj.get("itemCache", {}).items(), key=lambda x: x[0]):
-        # Dictionaries aren't ordered, so we can't allow this element
-        # to write into known_methods. We give it a copy instead.
-        serialised_item_cache[k] = serialise_val(v, known_methods.copy())
-    obj["itemCache"] = serialised_item_cache
-
-    if obj.get("iterItems"):
-        serialised_iteritems = []
-        for i in obj["iterItems"]["items"]:
-            serialised_iteritems.append(serialise_val(i, known_methods))
-        obj["iterItems"]["items"] = serialised_iteritems
-
-    return obj
-
-
-def _repr_path(p):
-    return "".join(("[%s]" % repr(k) for k in p))
-
-def _module_prefixes(module):
-    module_parts = module.split(".")
-    return [".".join(module_parts[:i]) for i in range(1, len(module_parts)+1)]
-
-_called_serialization_helpers = set()
-
-def _check_and_call_serialization_helper(cls_fullname):
-    "checks if a class has a registered helper, calls the helper if it exists (once)"
-    if cls_fullname in _called_serialization_helpers:
-        return False
-
-    for prefix in _module_prefixes(cls_fullname):
-        if prefix in _serialization_helpers:
-            _serialization_helpers[prefix](cls_fullname)
-            _called_serialization_helpers.add(cls_fullname)
-            return True
-
-    return False
-
-
-def fill_out_media(json, handle_media_fn, collect_capabilities=None, remote_is_trusted=False):
-    obj_descr = []
-    path = []
-    known_liveobject_methods = {}
-    serialization_info = SerializationInfo(remote_is_trusted=remote_is_trusted)
-    import datetime
-
-    def do_fom(_json):
-
-        t_json = type(_json)
-
-        if hasattr(_json, "SERIALIZATION_INFO"):
-            type_name, tp = _json.SERIALIZATION_INFO
-            valid_type_name = type_name in _value_types
-
-            if valid_type_name and tp is _json:
-                _json = None
-                obj_descr.append({
-                    "type": ["ClassType"],
-                    "path": list(path),
-                    "typeName": type_name
-                })
-
-            elif not valid_type_name or t_json is not tp:
-                raise SerializationError("Cannot serialize %s (must be registered with @anvil.server.portable_class) at msg%s" % (t_json, _repr_path(path)))
-            else:
-                serialization_info._set_default_key(type_name)
-
-                try:
-                    serialize = _json.__serialize__
-                except AttributeError:
-                    def serialize(_):
-                        return _json.__dict__
-
-                content = serialize(serialization_info)
-
-                _json = do_fom(content)
-
-                # Append this afterwards, so we deserialise our content first
-                obj_descr.append({
-                    "type": ["ValueType"],
-                    "path": list(path),
-                    "typeName": type_name
-                })
-
-        elif isinstance(_json, dict):
-            _json = dict(_json)
-            for k,v in sorted(_json.items(),key=lambda x: x[0]):
-                if not isinstance(k, string_type):
-                    raise SerializationError("Cannot serialize dictionaries with keys that aren't strings at msg%s" % _repr_path(path + [k]))
-                path.append(k)
-                _json[k] = do_fom(v)
-                path.pop()
-        elif isinstance(_json, list) or isinstance(_json, tuple):
-            _json = list(_json)
-            for i in range(len(_json)):
-                path.append(i)
-                _json[i] = do_fom(_json[i])
-                path.pop()
-        elif isinstance(_json, LazyMedia):
-            d = dict(_json._spec)
-            d["path"] = list(path)
-            obj_descr.append(d)
-            _json = None
-        elif isinstance(_json, anvil.Media):
-            extra = handle_media_fn(_json)
-            d = {"type": ["DataMedia"], "path": list(path), "mime-type": _json.content_type, "name": _json.name}
-            if extra is not None:
-                d.update(extra)
-            obj_descr.append(d)
-            _json = None
-        elif isinstance(_json, Capability):
-            if collect_capabilities is not None:
-                collect_capabilities.append(_json)
-            d = {
-                "type": ["Capability"],
-                "path": list(path),
-                "scope": _json._scope,
-                "mac": _json._mac
-            }
-            if _json._narrow:
-                d["narrow"] = _json._narrow
-            obj_descr.append(d)
-            _json = None
-        elif isinstance(_json, anvil.LiveObject):
-            #print "Serialising LiveObject: " + repr(_json._spec) + " at " + repr(path)
-            serialised_liveobject = serialise_live_object(_json, known_liveobject_methods)
-            serialised_liveobject["path"] = list(path)
-            obj_descr.append(serialised_liveobject)
-            _json = None
-        elif isinstance(_json, (datetime.date, datetime.datetime)) or \
-                (isinstance(_json, long_type) and (_json > 2147483647 or _json < -2147483647)) or \
-                (isinstance(_json, float) and (_json == POS_INFINITY or _json == NEG_INFINITY or math.isnan(_json))):
-            serialised_val = serialise_val(_json, known_liveobject_methods)
-            serialised_val["path"] = list(path)
-            obj_descr.append(serialised_val)
-            _json = None
-        elif _check_and_call_serialization_helper(t_json.__module__ + "." + t_json.__name__):
-            _json = do_fom(_json)
-        elif 'numpy' in sys.modules and hasattr(sys.modules['numpy'], 'generic') and isinstance(_json, sys.modules['numpy'].generic):
-
-            _json = _json.item() # convert
-
-        elif not (isinstance(_json, string_type) or _json is None or _json is True or _json is False or isinstance(_json, (int, long_type)) or isinstance(_json, float)):
-
-            # Rescue: Convert numpy types to nearest equivalent
-            if 'numpy' in sys.modules:
-                import numpy
-                if isinstance(_json, numpy.ndarray):
-                    _json = do_fom(_json.tolist())
-                else:
-                    raise SerializationError("Cannot serialize %s object at msg%s" % (t_json, _repr_path(path)))
-            else:
-                raise SerializationError("Cannot serialize %s object at msg%s" % (t_json, _repr_path(path)))
-
-        return _json
-
-    json = do_fom(json)
-
-    vt_global = serialization_info._to_json()
-    if len(vt_global) != 0:
-        path.append("vt_global")
-        serialization_info._set_txdata_available(False)
-        od = obj_descr
-        obj_descr = []
-        json["vt_global"] = do_fom(vt_global)
-        obj_descr += od
-        path.pop()
-
-    json["objects"] = obj_descr
-
-    return json
-
-
-def fill_out_cap_updates(resp, caps_passed_in):
-    """We're about to return from a call; ask all the capabilities that got passed in whether they want to send
-       any updates to our caller."""
-
-    for cap in caps_passed_in:
-        update = cap._get_update()
-        if update is not None:
-            cu = resp.get('capUpdates')
-            if cu is None:
-                cu = resp['capUpdates'] = {}
-            cu[json.dumps(cap.scope)] = update
-
-
-def apply_cap_updates(resp, caps_passed_out):
-    """We have just made a server call that has returned. Apply any necessary updates to the capabilities we
-       passed into this call"""
-
-    updates = resp.get('capUpdates', {})
-
-    # Normalise updates to how _this_ `json` impl does things (ugh)
-    updates = {json.dumps(json.loads(k)): v for k,v in updates.items()}
-
-    for cap in caps_passed_out:
-        scope_json = json.dumps(cap.scope)
-        update = updates.get(scope_json)
-        if update is not None:
-            cap._apply_update(update)
-
-
-def simple_strpdate(s):
-    import datetime
-    return datetime.date(int(s[0:4]), int(s[5:7]), int(s[8:10]))
-
-
-def simple_strpdatetime(s):
-    import datetime
-    return datetime.datetime(int(s[0:4]), int(s[5:7]), int(s[8:10]), int(s[11:13]), int(s[14:16]), int(s[17:19]), int(s[20:26])) # datetime.datetime.strptime(s, "%Y-%m-%d %H:%M:%S.%f")
-
-def parsedate(s):
-    return simple_strpdate(s)
-
-
-def parsedatetime(s):
-
-    has_tz = len(s) > 5 and \
-             (s[-5] == "-" or s[-5] == "+") and \
-             48 <= ord(s[-4]) <= 57 and \
-             48 <= ord(s[-3]) <= 57 and \
-             48 <= ord(s[-2]) <= 57 and \
-             48 <= ord(s[-1]) <= 57
-
-    if not has_tz:
-        # Parse a naive datetime
-        return simple_strpdatetime(s)
-
-    # Timezone present. First parse without it
-    d = simple_strpdatetime(s[:-5])
-
-    # Now construct a tzoffset
-    hours = int(s[-5:-2])
-    minutes = int(s[-5] + s[-2:])
-    total_minutes = hours*60+minutes
-
-    return d.replace(tzinfo=anvil.tz.tzoffset(minutes=total_minutes))
-
-def _retrieve_portable_class(type_name, d):
-    value_type = _value_types.get(type_name)
-    if value_type is not None:
-        return value_type
-    # Try importing the relevant module
-    i = type_name.rfind('.')
-    if i != -1:
-        # TODO do we filter what we can specify as import? I don't *think* this is dangerous...
-        if not _check_and_call_serialization_helper(type_name):
-            module_name = type_name[:i]
-            importlib.import_module(module_name)
-        value_type = _value_types.get(type_name)
-
-    if value_type is None:
-        raise SerializationError("No such serializable type: %s at msg%s" % (type_name, _repr_path(d["path"])))
-
-    return value_type
-
-
-def _reconstruct_objects(json, reconstruct_data_media, hold_back_value_types=False, collect_capabilities=None, remote_is_trusted=False):
-    known_liveobject_methods = {}
-    serialization_info = SerializationInfo(json.get("vt_global"), remote_is_trusted=remote_is_trusted) if not hold_back_value_types else None
-
-    if "objects" in json:
-        held_back_objects = []
-        for d in json["objects"]:
-            if hold_back_value_types and ("ValueType" in d["type"] or "ClassType" in d["type"]):
-                held_back_objects.append(d)
-                continue
-
-            reconstructed = reconstruct_val(d, known_liveobject_methods, reconstruct_data_media)
-            if collect_capabilities is not None and type(reconstructed) is Capability:
-                collect_capabilities.append(reconstructed)
-
-            obj = json
-            last_obj = None
-            key = None
-            for k in d["path"]:
-                last_obj = obj
-                key = k
-                obj = obj[k]
-
-            if last_obj is not None:
-
-                if "ValueType" in d["type"]:
-                    # Hack: The "reconstructed value" here is actually just the type name
-                    type_name = reconstructed
-                    value_type = _retrieve_portable_class(type_name, d)
-                    try:
-                        reconstruct = value_type.__new_deserialized__
-                    except AttributeError:
-                        def reconstruct(data, info):
-                            obj = value_type.__new__(value_type)
-                            try:
-                                deserialize = obj.__deserialize__
-                            except AttributeError:
-                                def deserialize(data, info):
-                                    obj.__dict__.update(data)
-                            deserialize(data, info)
-                            return obj
-
-                    serialization_info._set_txdata_available(d["path"][0] != 'vt_global')
-                    serialization_info._set_default_key(type_name)
-                    last_obj[key] = reconstruct(last_obj[key], serialization_info)
-                elif "ClassType" in d["type"]:
-                    last_obj[key] = _retrieve_portable_class(reconstructed, d)
-                else:
-                    last_obj[key] = reconstructed
-
-        if hold_back_value_types:
-            json["objects"] = held_back_objects
-        else:
-            del json["objects"]
-
-    return json
-
-on_register = None # optional
-registrations = {}
-
-class HttpRequest(object):
-
-    def __init__(self):
-        self._prevent_access = True
-
-    def __getattribute__(self, name):
-        if object.__getattribute__(self, "_prevent_access"):
-            raise Exception("anvil.server.request is only available in http_endpoint calls.")
-
-        return object.__getattribute__(self, name)
-
-    @property
-    def body_json(self):
-        if hasattr(self, "_body_json"):
-            return self._body_json
-        elif self.body is not None and self.headers.get("content-type", None) == "application/json":
-            self._body_json = json.loads(self.body.get_bytes())
-        else:
-            self._body_json = None
-        return self._body_json
-
-
-
-
-api_request = HttpRequest()
-
-def _lower_str(s):
-    if not isinstance(s, str):
-        return s
-    return s.lower()
-
-class HttpHeaders(object):
-
-    def __init__(self, headers=None):
-        headers = headers or {}
-        assert isinstance(headers, dict), "headers should be a dict"
-        headers = {_lower_str(h): v for (h, v) in headers.items()}
-        self._headers = list(headers.items())
-
-    def __setitem__(self, name, val):
-        name = _lower_str(name)
-        self._headers = [(h,v) for (h,v) in self._headers if h != name]
-
-        self.add(name, val)
-
-    def __delitem__(self, name):
-        name = _lower_str(name)
-        self._headers = [(h,v) for (h,v) in self._headers if h != name]
-
-    def add(self, name, val):
-        self._headers.append((name, val))
-
-    def clear(self):
-        self._headers = []
-
-    def copy(self):
-        new_self = HttpHeaders()
-        new_self._headers = self._headers.copy()
-        return new_self
-
-    def __repr__(self):
-        return "HttpHeaders(" + repr(self._headers) + ")"
-
-
-class HttpResponse(object):
-    def __init__(self, status=200, body="", headers=None):
-        self.status = status
-        self.body = body
-        self.headers = headers
-
-    @property
-    def headers(self):
-        return self._headers
-
-    @headers.setter
-    def headers(self, value):
-        if value is None or isinstance(value, dict):
-            self._headers = HttpHeaders(value)
-        elif isinstance(value, HttpHeaders):
-            self._headers = value.copy()
-        else:
-            raise TypeError("headers should be set to a dictionary")
-
-
-class CallContext(object):
-    class ClientInfo(object):
-        def __repr__(self):
-            return "<ClientInfo:%s>" % repr(self.__dict__)
-
-    class Location(object):
-        def __init__(self, location):
-            self.city = location.get('city')
-
-            self.subdivision = location.get('subdivision', {}).get('name')
-
-            l = location.get('location', {})
-            self.latitude = l.get('lat')
-            self.longitude = l.get('lng')
-
-            c = location.get('country', {})
-            self.country_code = c.get('code')
-            self.country = c.get('name')
-
-        def __repr__(self):
-            return "<Location:%s>" % repr(self.__dict__)
-
-    class StackFrame(object):
-        def __init__(self, sf):
-            self.type = sf.get("type")
-            self.is_trusted = self.type in {'server_module', 'uplink', 'background_task'}
-
-        def __repr__(self):
-            return "<StackFrame:%s>" % repr(self.__dict__)
-
-    _DEFAULT_TYPE = "server_module"
-
-    def _setup(self, client, call_stack):
-        self.type = CallContext._DEFAULT_TYPE
-        if client is not None:
-            self.client = CallContext.ClientInfo()
-            self.client.type = client.get('type')
-            self.client.ip = client.get('ip')
-            self.background_task_id = client.get('background-task-id')
-            l = client.get('location')
-            self.client.location = CallContext.Location(l) if l else None
-            self.remote_caller = CallContext.StackFrame(call_stack[0] if call_stack else client)
-        else:
-            self.client = None
-            self.remote_caller = None
-            self.background_task_id = None
-
-    __init__ = _setup
-
-    def __repr__(self):
-        return "<CallContext:%s>" % repr(self.__dict__)
-
-
-# can be used as a decorator too
-# N.B. There is a full implementation of the 'require=' kwarg here, but we've chosen not to expose it yet. If we expose it, will need to pass through from callable, like require_user.
-def register(fn, name=None, name_prefix=None, require_user=None):
-    require=None
-
-    if isinstance(fn, string_type):
-        # Someone's using the old syntax. Our bad.
-        (fn, name) = (name, fn)
-
-    if name is None:
-        name = fn.__name__
-
-    original_name = name
-    if name_prefix is not None:
-        name = "%s:%s" % (name_prefix, name)
-
-    # 'require_user' is either True (check that user is logged in), False (equivalent to None), or 
-    # a function that takes the currently logged in user and returns whether to let them in.
-
-    if require_user == True:
-        def simple_require_user():
-            import anvil.users
-            if anvil.users.get_user() is None:
-                raise anvil.users.AuthenticationFailed("You must be logged in to call this server function")
-            return True
-        require = simple_require_user
-    elif require_user == False:
-        require = None
-    elif require_user is not None:
-        # Must be a function.
-        def complex_require_user():
-            import anvil.users
-            user = anvil.users.get_user()
-            if user is None:
-                raise anvil.users.AuthenticationFailed("You must be logged in to call server function '%s'" % original_name)
-            elif not require_user(user):
-                raise PermissionDenied("You do not have permission to call server function '%s'" % original_name)
-            else:
-                return True
-        require = complex_require_user
-
-    # 'require' is an optional function that returns something truthy if the user should be let in. Otherwise, it can raise 
-    # an Exception (which will be passed on) or return something falsey (in which case a PermissionDenied exception will be raised.)
-
-    if require is not None:
-        def require_wrap(f):
-            def with_req(*args, **kwargs):
-                if require():
-                    return f(*args, **kwargs)
-                else:
-                    raise PermissionDenied("You do not have permission to call server function '%s'" % original_name)
-            return with_req
-    else:
-        def require_wrap(f):
-            return fn
-
-    registrations[name] = require_wrap(fn)
-
-    if on_register is not None:
-        on_register(name, False)
-
-    def reregister(new_f):
-        registrations[name] = require_wrap(new_f)
-        new_f._anvil_reregister = reregister
-
-    fn._anvil_reregister = reregister
-
-    return fn
-
-#!defFunction(anvil.server,%,[name], [require_user])!2: {anvil$args: {fn_or_name: "The name by which you want to call your function from the client.", require_user: "Allows you to verify whether a user is logged in. Can be a boolean or a function."}, anvil$helpLink: "server#calling-server-functions-from-client-code", $doc: "When applied to a function as a decorator, the function becomes available from the client side."} ["callable"]
-def callable(fn_or_name=None, require_user=None):
-    if fn_or_name is None or isinstance(fn_or_name, string_type):
-        return lambda f: register(f, fn_or_name, require_user=require_user)
-    else:
-        return register(fn_or_name)
-
-
-def background_task(fn_or_name=None):
-    if fn_or_name is None or isinstance(fn_or_name, string_type):
-        return lambda f: register(f, fn_or_name, name_prefix="task")
-    else:
-        return register(fn_or_name, name_prefix="task")
-
-
-# A parameterised decorator
-def callable_as(name):
-    print("@callable_as is deprecated. Please use @callable directly.")
-    return lambda f: register(f, name)
-
-
-
-def http_endpoint(path, require_credentials=False, authenticate_users=False, authenticate_user=False,
-                  methods=["GET","POST"], enable_cors=False, cross_site_session=False, _task_prefix="http"):
-    def decorator(fn):
-        path_parts = []
-        def register_path_part(s):
-            path_parts.append(s.group(1))
-            return "([^/]*)"
-
-        path_regex = re.sub(":([^/]*)", register_path_part, path)
-
-        def wrapped_fn(method, path, query_params, form_params, origin, headers, remote_address, body, username, password, same_app_alternate_origin=None, **more_kwargs):
-
-            api_request._prevent_access = False
-
-            if cross_site_session:
-                import anvil.server
-                anvil.server._switch_session()
-
-            api_request.user = None
-            if authenticate_users or authenticate_user:
-                import anvil.users
-                try:
-                    api_request.user = anvil.users.get_user() or \
-                                        anvil.users.login_with_email(username, password)
-                except Exception as e:
-                    return {"status": 401,
-                            "body": "Unauthorized",
-                            "headers": {"WWW-Authenticate": "Basic realm=\"Anvil App API\""}}
-            elif require_credentials:
-                if username is None or password is None:
-                    return {"status": 401,
-                            "body": "Unauthorized",
-                            "headers": {"WWW-Authenticate": "Basic realm=\"Anvil App API\""}}
-
-            def add_cross_origin_to_header_dict(d):
-                if enable_cors:
-                    d["Access-Control-Allow-Origin"] = enable_cors if isinstance(enable_cors, str) else "*"
-                elif same_app_alternate_origin:
-                    d["Access-Control-Allow-Origin"] = same_app_alternate_origin
-                if enable_cors or same_app_alternate_origin and \
-                        "access-control-allow-headers" not in [h.lower() for h in d.keys()]:
-                    allow_headers = ["content-type"]
-                    for k in headers.keys():
-                        if k.lower() == "access-control-request-headers":
-                            hs = [h.strip().lower() for h in headers[k].split(",")]
-                            allow_headers += [h for h in hs if h not in allow_headers]
-
-                    d["Access-Control-Allow-Headers"] = ", ".join(allow_headers)
-
-                return d
-
-            if method not in methods:
-                if method == "OPTIONS" and (enable_cors or same_app_alternate_origin):
-                    return {"status": 200,
-                            "body": "",
-                            "headers": add_cross_origin_to_header_dict({})}
-                else:
-                    return {"status": 405,
-                            "body": "Method not supported",
-                            "headers": {"Allow": ", ".join(methods)}}
-
-            api_request.path = path
-            api_request.method = method
-            api_request.query_params = query_params
-            api_request.form_params = form_params
-            api_request.origin = origin
-            api_request.headers = headers
-            api_request.remote_address = remote_address
-            api_request.body = body
-            api_request.username = username
-            api_request.password = password
-
-
-            # Path takes precedence over query params. Query params take precedence over form params.
-            kwargs = dict(form_params)
-            kwargs.update(query_params)
-            match = re.match(path_regex, path)
-            for i,m in enumerate(match.groups()):
-                kwargs[path_parts[i]] = m
-
-            response = fn(**kwargs)
-
-            api_request._prevent_access = True
-
-            if isinstance(response, HttpResponse):
-                return {"status":  response.status,
-                        "body":    response.body,
-                        "headers": add_cross_origin_to_header_dict(response.headers)._headers}
-            else:
-                return {"status":  200,
-                        "body":    response,
-                        "headers": add_cross_origin_to_header_dict({})}
-
-        register(wrapped_fn, path_regex, _task_prefix)
-
-        return fn
-    return decorator
-
-
-wellknown_endpoint = functools.partial(http_endpoint, _task_prefix = "http-wellknown")
-
-
-class AnvilCookie(object):
-
-    def __init__(self, type):
-        self._type = type
-
-    def __getitem__(self, name):
-        return _do_call([self._type, name], None, fn_name="anvil.private.get_cookie")
-
-    def __setitem__(self, name, value):
-        kw = {}
-        kw[name] = value
-        self.set(30, **kw)
-
-    def __delitem__(self, name):
-        _do_call([self._type, name], None, fn_name="anvil.private.del_cookie")
-
-    def get(self, key, default=None):
-        try:
-            return _do_call([self._type, key], None, fn_name="anvil.private.get_cookie")
-        except KeyError:
-            return default
-
-    def set(self, timeout_days=30, **values):
-        _do_call([self._type, timeout_days], values, fn_name="anvil.private.set_cookie")
-
-    def clear(self):
-        _do_call([self._type], None, fn_name="anvil.private.clear_cookie")
-
-
-class CookieContainer(object):
-
-    def __init__(self):
-        self.local = AnvilCookie("local")
-        self.shared = AnvilCookie("shared")
-
-
-cookies = CookieContainer()
-
-
-class NotABackgroundTaskState(object):
-    def __setitem__(self, key, value):
-        raise Exception("Cannot access anvil.server.task_state outside a background task")
-
-    def __getitem__(self, item):
-        raise Exception("Cannot access anvil.server.task_state outside a background task")
-
-
-# Raise event on all sessions in the current environment, on a specific session, on multiple sessions, or on a named channel
-def raise_event(name, payload=None, session_id=None, session_ids=None, channel=None):
-    anvil.server.call("anvil.private.raise_event", name, payload, session_id=session_id, session_ids=session_ids, channel=channel)
-
-
-# List all sessions in the current environment, or only those where the specified user is logged in.
-def list_client_sessions(user=None):
-    return anvil.server.call("anvil.private.list_sessions", user=user)
-
-
-# Get the value of anvil.server.session for a particular session in the current environment
-def get_client_session(session_id):
-    return anvil.server.call("anvil.private.get_session_data", session_id)
-
-
-# Get the ID of the current session
-#!defFunction(anvil.server,%)!2: "Returns the current session's ID." ["get_session_id"]
-def get_session_id():
-    return anvil.server.call("anvil.private.get_session_id")
-
-
-# Subscribe this session to receive events from the named channel
-def subscribe(channel):
-    return anvil.server.call("anvil.private.subscribe", channel)
-
-
-# Unsubscribe this session from receiving events from the named channel
-def unsubscribe(channel):
-    return anvil.server.call("anvil.private.unsubscribe", channel)
-
-
-def get_subscriptions():
-    return anvil.server.call("anvil.private.get_subscriptions")
-
-
-def plotly_serialization_helper(class_fullname):
-    name_parts = class_fullname.split(".")
-    module_name = ".".join(name_parts[:-1])
-    class_name = name_parts[-1]
-
-    module = importlib.import_module(module_name)
-    cls = getattr(module, class_name)
-
-    if not hasattr(cls, '__serialize__'):
-        # print(f"Registering {cls}")
-        def serialize(self, global_data):
-            # print("Serialising %s on downlink" % type(self))
-            return self.to_plotly_json()
-
-        @staticmethod
-        def new_deserialized(data, global_data):
-            # print("Deserialising %s on downlink" % cls)
-            return cls(data)
-
-        cls.__serialize__ = serialize
-        cls.__new_deserialized__ = new_deserialized
-        portable_class(cls, class_fullname)
-
-
-_serialization_helpers["plotly.graph_objs"] = plotly_serialization_helper
+# Helpers for implementing anvil.server.
+# Used in uplink, downlink and pypy-sandbox.
+import importlib
+
+import anvil
+import traceback
+import numbers
+import sys
+import re
+import json
+import math
+import anvil.tz
+import functools
+
+_do_call = None
+
+string_type = str if sys.version_info >= (3,) else basestring
+long_type = int if sys.version_info >= (3,) else long
+
+POS_INFINITY = float("inf")
+NEG_INFINITY = float("-inf")
+
+_value_types = {}
+_serialization_helpers = {} # {module_name: helper_fn}
+
+class LiveObjectProxy(anvil.LiveObject):
+
+    def __init__(self,spec,known_methods=None):
+        for k in ["itemCache", "iterItems"]:
+            if spec.get(k, {}) is None:
+                del spec[k]
+
+        if known_methods is not None:
+            if spec.get("methods") is None:
+                spec["methods"] = known_methods[spec["backend"]]
+            else:
+                known_methods[spec["backend"]] = spec["methods"]
+        anvil.LiveObject.__init__(self, spec)
+
+    def __getattr__(self, item):
+        if item in self._spec["methods"]:
+            def item_fn(*args, **kwargs):
+                return _do_call(args, kwargs, fn_name=item, live_object=self)
+
+            return item_fn
+        else:
+            raise AttributeError(item)
+
+    def __getitem__(self, item):
+
+        if "__anvil_iter_page__" in self._spec["methods"]:
+            if isinstance(item, (int,long_type)):
+                if item < 0:
+                    raise IndexError("list index cannot be negative")
+
+                iter = LiveObjectProxy.Iter(self, item)
+                try:
+                    return iter.next()
+                except StopIteration:
+                    raise IndexError("list index out of range")
+            elif isinstance(item, slice):
+                if (item.start and item.start < 0) or (item.stop and item.stop < 0) or (item.step and item.step < 0):
+                    raise Exception("list slice indices and step cannot be negative")
+                return LiveObjectProxy.Iter(self, item.start, item.stop, item.step)
+
+
+        if item in self._spec.get("itemCache", {}):
+            return self._spec["itemCache"][item]
+
+        getitem = self.__getattr__("__getitem__")
+
+        try:
+            return getitem(item)
+        except AnvilWrappedError as e:
+            raise _deserialise_exception(e.error_obj)
+
+    def __setitem__(self, key, value):
+        if key in self._spec.get("itemCache", {}):
+            del self._spec["itemCache"][key]
+
+        setitem = self.__getattr__("__setitem__")
+        try:
+            r = setitem(key, value)
+        except AnvilWrappedError as e:
+            raise _deserialise_exception(e.error_obj)
+
+        if "itemCache" in self._spec and (isinstance(value, string_type) or isinstance(value, numbers.Number) or isinstance(value, bool) or value is None):
+            self._spec["itemCache"][key] = value
+
+        return r
+
+    class Iter:
+        def __init__(self, live_object, start=None, stop=None, step=None):
+            self._live_object = live_object
+
+            i = live_object._spec.get("iterItems", {})
+            self._idx = start if start is not None else 0
+            self._items = i.get("items", None)
+            self._next_page = i.get("nextPage", None)
+            self._stop = stop
+            self._step = step if step is not None else 1
+
+        def _fetch_state(self):
+            r = _do_call([self._next_page], {}, fn_name="__anvil_iter_page__", live_object=self._live_object)
+            self._items = r["items"]
+            self._next_page = r.get("nextPage", None)
+
+        def __iter__(self):
+            return self
+
+        def next(self):
+            if self._items is None:
+                try:
+                    self._fetch_state()
+                except AnvilWrappedError as e:
+                    raise _deserialise_exception(e.error_obj)
+
+            if self._idx < len(self._items) and (self._stop is None or self._idx < self._stop):
+                r = self._items[self._idx]
+                self._idx += self._step
+                return r
+
+            if self._next_page is None or (self._stop is not None and self._idx >= self._stop):
+                raise StopIteration
+
+            self._idx -= len(self._items) if self._items is not None else self._idx
+            if self._stop is not None:
+                self._stop -= len(self._items) if self._items is not None else 0
+            self._items = None
+            return self.next()
+
+        def __next__(self):
+            return self.next()
+
+    def __iter__(self):
+        if "__anvil_iter_page__" in self._spec["methods"]:
+            return LiveObjectProxy.Iter(self)
+        else:
+            raise Exception("Not iterable: <LiveObject: %s>" % self._spec.get("backend", "INVALID"))
+
+    def __bool__(self):
+        if "__nonzero__" in self._spec["methods"]:
+            return self.__getattr__("__nonzero__")()
+        else:
+            return True
+
+    __nonzero__ = __bool__
+
+    def __len__(self):
+        if "__len__" in self._spec["methods"]:
+            return int(self.__getattr__("__len__")())
+        else:
+            l = 0
+            for _ in self.__iter__():
+                l += 1
+            return l
+
+
+# Wildcard for unwrap_capability
+class _CapAny(object):
+    def __repr__(self):
+        return "ANY"
+
+def _check_valid_scope(scope, name="scope"):
+    if type(scope) is not list:
+            raise TypeError("The {} of a Capabilty must be a list".format(name))
+    try:
+        return json.loads(json.dumps(scope))
+    except TypeError as e:
+        raise TypeError("The {} provided is not valid JSON data. {}".format(name, e))
+
+
+class Capability(object):
+    def __init__(self, scope, mac=None, narrow=None):
+        scope = _check_valid_scope(scope)
+        self._scope = scope
+        self._mac = mac
+        if mac is not None:
+            pass
+        elif not len(scope):
+            raise ValueError("Cannot construct a capability with an empty scope")
+        elif scope[0] == "_":
+            raise ValueError("To construct a Capability from scratch, its scope cannot start with ['_']")
+
+        self._narrow = narrow or []
+        self._do_apply_update = None
+        self._do_get_update = None
+        self._queued_update = {}
+        self._hash = None
+
+    @property
+    def scope(self):
+        return self._scope + self._narrow
+
+    def narrow(self, narrowing_suffix):
+        narrowing_suffix = _check_valid_scope(narrowing_suffix, "narrow argument")
+        return Capability(self._scope, self._mac, self._narrow + narrowing_suffix)
+
+    def __repr__(self):
+        return "<anvil.server.Capability:{}>".format(self.scope)
+
+    def __eq__(self, other):
+        if type(other) is not Capability:
+            return NotImplemented
+        return self.scope == other.scope
+
+    def __hash__(self):
+        if self._hash is None:
+            self._hash = hash(json.dumps(self.scope))
+        return self._hash
+
+    def set_update_handler(self, apply_update, get_update=None):
+        self._do_apply_update = apply_update
+        self._do_get_update = get_update
+
+    # RPC machinery:
+    # An update has arrived from a server call. Default behaviour: Merge if it's a dict, overwrite if it isn't
+    def _apply_update(self, update):
+        if self._do_apply_update is not None:
+            self._do_apply_update(update)
+
+        if self._do_get_update is None:
+            # Default update propagation rules
+            if isinstance(update, dict):
+                self._queued_update.update(**update)
+            else:
+                self._queued_update = update
+
+    send_update = _apply_update
+
+    # RPC machinery:
+    # We're about to return from a server call which passed this capability in; do we have an update for them?
+    # None -> nothing to send
+    def _get_update(self):
+        if self._do_get_update is not None:
+            return self._do_get_update()
+        else:
+            return None if self._queued_update == {} else self._queued_update
+
+    # Sentinel value for unwrap_capability
+    ANY = _CapAny()
+
+#!defFunction(anvil.server,list,capability,scope_pattern)!2: "Checks that its first argument is a valid Capability, and that its scope matches the supplied pattern.\n\nTo match, the scope must:\n - Be at least as broad as the pattern (ie the same length or shorter)\n- Contain the same values in the same position as the pattern - unless that position in the pattern is Capability.ANY, which matches any value\n\nReturns a list of matched scope elements, of the same length as the pattern. (If the scope was broader than required, missing elements are set to None.)" ["unwrap_capability"]
+def unwrap_capability(cap, scope_pattern):
+    if type(cap) is not Capability:
+        raise TypeError("Not a valid Capability: found {}".format(type(cap).__name__))
+    if type(scope_pattern) is not list:
+        raise TypeError("scope_pattern should be a list, not {}".format(type(scope_pattern).__name__))
+
+    scope = cap.scope
+    ret = [None] * len(scope_pattern)
+
+    if len(scope) > len(scope_pattern):
+        raise ValueError("Capability is too narrow: required %s; got %s" % (scope_pattern, scope))
+
+    for i in range(len(scope)):
+        if scope_pattern[i] is Capability.ANY or scope[i] == scope_pattern[i]:
+            ret[i] = scope[i]
+        else:
+            raise ValueError("Incorrect Capability: required %s; got %s" % (scope_pattern, cap.scope))
+
+    return ret
+
+# DEPRECATED: replaced by unwrap_capability - included here for Backwards compatibility
+Capability.require = staticmethod(unwrap_capability)
+
+
+class SerializationInfo(object):
+    def __init__(self, fromdata=None, remote_is_trusted=False):
+        self._txdata = {}
+        self._localdata = {}
+        self._defaultkey = None
+        self._trusted = remote_is_trusted
+        self._enable_txdata = True
+        if fromdata is None:
+            pass
+        elif type(fromdata) is dict:
+            self._txdata[":GLOBAL"] = fromdata
+        else:
+            it = iter(fromdata)
+            for k, v in zip(it, it):
+                self._txdata[k] = v
+
+    def __bool__(self):
+        return bool(self._enable_txdata)
+
+    __nonzero__ = __bool__
+
+    def _to_json(self):
+        if len(self._txdata) == 1 and ":GLOBAL" in self._txdata:
+            return self._txdata[":GLOBAL"]
+        else:
+            r = []
+            for k, v in self._txdata.items():
+                r.append(k)
+                r.append(v)
+            return r
+
+    def _resolve_key(self, key):
+        if key is None:
+            return self._defaultkey
+        elif isinstance(key, type):
+            try:
+                return key.SERIALIZATION_INFO[0]
+            except AttributeError:
+                return key.__module__ + "." + key.__name__
+        else:
+            return ":" + str(key)
+
+    def _set_default_key(self, key):
+        self._defaultkey = key
+
+    def _set_txdata_available(self, enable):
+        self._enable_txdata = enable
+    
+    def _set_data_factory(self, _data, resolved_key, factory):
+        data = _data.get(resolved_key)
+        if data is None:
+            data = _data[resolved_key] = factory()
+        return data
+
+    def shared_data(self, key=None, transmitted_data_factory=dict, local_data_factory=dict):
+        key = self._resolve_key(key)
+        localdata = self._set_data_factory(self._localdata, key, local_data_factory)
+        if not self._enable_txdata:
+            return None, localdata
+        txdata = self._set_data_factory(self._txdata, key, transmitted_data_factory)
+        return txdata, localdata
+
+    @property
+    def remote_is_trusted(self):
+        return self._trusted
+
+    @property
+    def local_is_trusted(self):
+        return anvil.is_server_side()
+
+    def __repr__(self):
+        # TODO adjust for public api
+        return "SerializationInfo<" + repr(self._txdata) + ", " + repr(self._localdata) + ">"
+
+
+# Backwards compatibility: If you use SerializationInfo like a dict, it man works like  if you use it like a dict
+def _wrap_global_dict(attr_name):
+    def f(self, *args, **kws):
+        transmitted_data = self.shared_data("GLOBAL")[0]
+        if transmitted_data is None:
+            # using the old API so better to throw here
+            raise RuntimeError("This object is part of shared_data; you cannot access shared_data from its __serialize__ method.")
+        return getattr(transmitted_data, attr_name)(*args, **kws)
+    return f
+
+
+for method in ["__getitem__", "__setitem__", "__delitem__", "__iter__", "__len__", "__contains__", "keys", "items",
+               "values", "get", "pop", "popitem", "clear", "update", "setdefault"]:
+    setattr(SerializationInfo, method, _wrap_global_dict(method))
+
+
+# DEPRECATED: there is no longer any reason to inherit from this
+class Serializable(object):
+    SERIALIZATION_INFO = None
+
+    def __serialize__(self, info):
+        return self.__dict__
+
+    # You only need one of __deserialize__ (called instead of __init__)
+    # or __new_deserialized__ (called instead of __new__+__init__).
+    # (Of the two, you almost always want __deserialize__.)
+    def __deserialize__(self, from_data, info):
+        self.__dict__.update(from_data)
+
+    @classmethod
+    def __new_deserialized__(cls, from_data, info):
+        obj = cls.__new__(cls)
+        obj.__dict__.update(from_data)
+        return obj
+
+
+# Add-in for maintaining object identity across serialization
+class SerializeWithIdentity(object):
+    @classmethod
+    def __new_deserialized__(cls, from_data, global_data):
+        clsname, _ = cls.SERIALIZATION_INFO
+        cache = global_data.get(clsname)
+        if cache is None:
+            cache = global_data[clsname] = {}
+        my_id = from_data[0]
+        # We use global_data to cache instances we're constructing
+        # (non-JSONable keys certainly won't conflict with other global_data users)
+        obj = cache.get(my_id)
+        if obj is None:
+            obj = cache[my_id] = cls.__new__(cls)
+
+        if len(from_data) > 1:
+            obj.__deserialize__(from_data[1], global_data)
+
+        return obj
+
+    def __serialize__(self, global_data):
+        my_id, gd = self._serialization_key if hasattr(self, "_serialization_key") else (None, None)
+        if gd is global_data:
+            return [my_id]
+
+        clsname, _ = self.SERIALIZATION_INFO
+        my_id = global_data.get(clsname+"_max", 0)
+        global_data[clsname+"_max"] = my_id + 1
+
+        self._serialization_key = (my_id, global_data)
+
+        data = self.__serialize_once__(global_data)
+        if isinstance(data, dict):
+            data = dict(data)
+            data.pop("_serialization_key", None)
+
+        return [my_id, data]
+
+
+def portable_class(cls, name=None):
+    def register(cls, name):
+        if not hasattr(cls, "__new__"):
+            raise TypeError("Portable classes must be new-style classes (inherit from object). %s is not a new-style class." % repr(cls))
+        if name is None:
+            name = cls.__module__ + "." + cls.__name__
+        elif not isinstance(name, str):
+            raise TypeError("The second argument to portable_class must be a str")
+        _value_types[name] = cls
+        cls.SERIALIZATION_INFO = (name, cls)
+        return cls
+
+    if name is None and isinstance(cls, str):
+        name = cls
+        return lambda cls: register(cls, name)
+    else:
+        return register(cls, name)
+
+
+# Old name, for apps written before portable classes were released
+serializable_type = portable_class
+
+
+class LazyMedia(anvil.Media):
+    def __init__(self, spec):
+        if isinstance(spec,LazyMedia):
+            spec = spec._spec
+        self._spec = spec
+        self._details = None
+        self._fetched = None
+
+    def _fetch(self):
+        if self._details is None:
+            import anvil.server
+            self._fetched = anvil.server.call("anvil.private.fetch_lazy_media", self._spec)
+        return self._fetched
+
+    def _get(self, key, attr=None):
+        if attr is None:
+            attr = key
+        return self._spec[key] if key in self._spec else getattr(self._fetch(), attr)
+
+    def get_name(self):
+        try:
+            return self._get("name")
+        except AnvilWrappedError as e:
+            raise _deserialise_exception(e.error_obj)
+
+    def get_url(self, download=True):
+        return anvil.server.call("anvil.private.get_lazy_media_url", self, download)
+
+    def get_content_type(self):
+        try:
+            return self._get("mime-type", "content_type")
+        except AnvilWrappedError as e:
+            raise _deserialise_exception(e.error_obj)
+
+    def get_length(self):
+        try:
+            return self._get("length")
+        except AnvilWrappedError as e:
+            raise _deserialise_exception(e.error_obj)
+
+    def get_bytes(self):
+        try:
+            return self._fetch().get_bytes()
+        except AnvilWrappedError as e:
+            raise _deserialise_exception(e.error_obj)
+
+
+class AnvilWrappedError(Exception):
+    registered_type_name = None
+
+    def __init__(self, message=""):
+        if isinstance(message, dict):
+            self.manually_created = False
+            self.error_obj = message
+        else:
+            self.manually_created = True
+            self.error_obj = {"message": str(message), "trace": []}
+            t = type(self).registered_type_name
+            if t is not None:
+                self.error_obj["type"] = t
+        self.message = self.error_obj.get("message", "")
+        Exception.__init__(self, self.message)
+
+    def __repr__(self):
+        r = Exception.__repr__(self)
+        if type(self) is not AnvilWrappedError:
+            return r
+        eo_type = self.error_obj.get("type")
+        if eo_type is None:
+            return r
+
+        return "AnvilWrappedError" + "(" + eo_type + r[len("AnvilWrappedError"):] + ")"
+
+
+def augment_exception(exc_class):
+    def f(error_obj):
+        e = exc_class(error_obj['message'])
+        e._anvil_error_obj = error_obj
+        return e
+    return f
+
+_named_exceptions = {
+    "KeyError": augment_exception(KeyError)
+}
+
+
+def _register_exception_type(name, cls):
+    _named_exceptions[name] = cls
+    cls.registered_type_name = name
+
+
+def _deserialise_exception(error_obj):
+    return _named_exceptions.get(error_obj.get("type"), AnvilWrappedError)(error_obj)
+
+
+def get_liveobject_cache_filter_spec(input_data):
+    """Returns a specification of a filter for LiveObject cache updates, which passes only LiveObjects present in input_data"""
+    spec = {}
+
+    def f(data):
+        if isinstance(data, list):
+            for i in data: f(i)
+        elif isinstance(data, dict):
+            for k,v in data.items(): f(v)
+        elif isinstance(data, LiveObjectProxy):
+            b = spec.get(data._spec["backend"])
+            if b is None:
+                b = spec[data._spec["backend"]] = set()
+            b.add(data._spec["id"])
+
+    f(input_data)
+    return spec
+
+
+def combine_cache_updates(updates, new_updates, filter_spec):
+    if updates is None:
+        updates = {}
+
+    for k in new_updates:
+        permitted_ids = filter_spec.get(k)
+        if permitted_ids is None:
+            continue
+        caches = updates.get(k)
+        if caches is None:
+            caches = updates[k] = dict()
+        for id in new_updates[k]:
+            if id not in permitted_ids:
+                continue
+            caches[id] = new_updates[k][id]
+
+
+def apply_cache_updates(cache_updates, objects_to_walk):
+    """Recursively walk an object tree, applying cache updates wherever necessary"""
+
+    def f(data):
+        if isinstance(data, list):
+            for i in data: f(i)
+        elif isinstance(data, dict):
+            for k,v in data.items(): f(v)
+        elif isinstance(data, LiveObjectProxy):
+            update = cache_updates.get(data._spec["backend"], {})
+            if data._spec["id"] in update:
+                data._spec["itemCache"] = update[data._spec["id"]]
+
+    f(objects_to_walk)
+
+
+class MaybeWrappedError(Exception):
+    def __init__(self, message=""):
+        if isinstance(message, dict):
+            Exception.__init__(self, message["message"])
+        else:
+            Exception.__init__(self, message)
+
+
+class SerializationError(MaybeWrappedError):
+    pass
+
+
+class InternalError(MaybeWrappedError):
+    pass
+
+
+class InvalidResponseError(MaybeWrappedError):
+    pass
+
+
+class RuntimeUnavailableError(MaybeWrappedError):
+    pass
+
+
+class UplinkDisconnectedError(MaybeWrappedError):
+    pass
+
+
+class ExecutionTerminatedError(MaybeWrappedError):
+    pass
+
+
+class TimeoutError(MaybeWrappedError):
+    pass
+
+
+class QuotaExceededError(MaybeWrappedError):
+    pass
+
+
+class NoServerFunctionError(AnvilWrappedError):
+    pass
+
+
+class CookieError(AnvilWrappedError):
+    pass
+
+
+class _FailError(MaybeWrappedError):
+    pass
+
+
+class BackgroundTaskError(MaybeWrappedError):
+    pass
+
+
+class BackgroundTaskNotFound(MaybeWrappedError):
+    pass
+
+
+class BackgroundTaskKilled(MaybeWrappedError):
+    pass
+
+
+class PermissionDenied(MaybeWrappedError):
+    pass
+
+
+class ServiceNotAdded(MaybeWrappedError):
+    pass
+
+
+
+_register_exception_type("anvil.server.SerializationError", SerializationError)
+_register_exception_type("anvil.server.InternalError", InternalError)
+_register_exception_type("anvil.server.InvalidResponseError", InvalidResponseError)
+_register_exception_type("anvil.server.RuntimeUnavailableError", RuntimeUnavailableError)
+_register_exception_type("anvil.server.UplinkDisconnectedError", UplinkDisconnectedError)
+_register_exception_type("anvil.server.ExecutionTerminatedError", ExecutionTerminatedError)
+_register_exception_type("anvil.server.TimeoutError", TimeoutError)
+_register_exception_type("anvil.server.QuotaExceededError", QuotaExceededError)
+_register_exception_type("anvil.server.NoServerFunctionError", NoServerFunctionError)
+_register_exception_type("anvil.server.CookieError", CookieError)
+_register_exception_type("anvil.server._FailError", _FailError)
+_register_exception_type("anvil.server.BackgroundTaskError", BackgroundTaskError)
+_register_exception_type("anvil.server.BackgroundTaskNotFound", BackgroundTaskNotFound)
+_register_exception_type("anvil.server.PermissionDenied", PermissionDenied)
+_register_exception_type("anvil.server.ServiceNotAdded", ServiceNotAdded)
+
+
+
+def _report_exception(request_id=None):
+    exc_type, exc_value, exc_traceback = sys.exc_info()
+    tb = traceback.extract_tb(exc_traceback)
+
+    trace = [(filename.replace("\\","/"), lineno) for (filename, lineno, _, _) in tb]
+    trace.reverse()
+
+    # Last element of trace is where we called into user code. Remove it.
+    trace.pop()
+
+    if isinstance(exc_value, AnvilWrappedError):
+        if not exc_value.manually_created:
+            # First element of trace is where we re-raised the exception. Remove it.
+            trace = trace[1:]
+        exc_value.error_obj["trace"] = exc_value.error_obj.get("trace", []) + trace
+        r = {
+            "error": exc_value.error_obj,
+            "id": request_id
+        }
+        return r
+    elif isinstance(exc_value, SyntaxError):
+        # Remove whole internal trace and replace it with line where error occurred.
+        trace=[(exc_value.filename, exc_value.lineno)]
+        return {
+            "error": {
+                "type": "SyntaxError",
+                "trace": trace,
+                "message": str(exc_value)
+            },
+            "id": request_id
+        }
+    elif isinstance(exc_value, MaybeWrappedError):
+        return {
+            "error": {
+                "type": "anvil.server.%s" % exc_type.__name__,
+                "trace": trace,
+                "message": str(exc_value),
+            },
+            "id": request_id
+        }
+    elif hasattr(exc_value, "_anvil_error_obj"):
+        error_obj = dict(exc_value._anvil_error_obj)
+        error_obj['trace'] = exc_value._anvil_error_obj.get("trace", []) + trace[1:]
+
+        return {
+            "error": error_obj,
+            "id": request_id
+        }
+    else:
+        return {
+            "error": {
+                "type": str(exc_type.__name__),
+                "trace": trace,
+                "message": str(exc_value),
+            },
+            "id": request_id
+        }
+
+def reconstruct_val(v, known_liveobject_methods, reconstruct_data_media=None):
+
+    for t in v["type"]:
+        if t == "DataMedia":
+            if reconstruct_data_media is None:
+                raise Exception("No data media deserialiser provided. Cannot reconstruct.")
+            return reconstruct_data_media(v)
+        elif t == "LazyMedia":
+            return LazyMedia(v)
+        elif t == "LiveObject":
+            return reconstruct_live_object(v, known_liveobject_methods)
+        elif t == "Capability":
+            return Capability(v["scope"], v["mac"])
+        elif t == "Date":
+            return parsedate(v["value"]) if v["value"] else None
+        elif t == "DateTime":
+            return parsedatetime(v["value"]) if v["value"] else None
+        elif t == "Long":
+            return long_type(v["value"])
+        elif t == "Float":
+            return float(v["value"])
+        elif t == "Primitive":
+            return v["value"]
+        elif t == "ValueType":
+            return v["typeName"]
+        elif t == "ClassType":
+            return v["typeName"]
+
+    raise Exception("Server module cannot accept an object of type '%s'" % v["type"][0])
+
+
+
+def reconstruct_live_object(d, known_methods):
+
+    # Need to fill out known_methods before we can reconstruct members:
+    if d.get('methods') is not None:
+        known_methods[d["backend"]] = d["methods"]
+
+    reconstructed_item_cache = {}
+    for k,v in d.get("itemCache", {}).items():
+        reconstructed_item_cache[k] = reconstruct_val(v, known_methods)
+    d["itemCache"] = reconstructed_item_cache
+
+    if d.get("iterItems"):
+        reconstructed_iteritems = []
+        for i in d["iterItems"]["items"]:
+            reconstructed_iteritems.append(reconstruct_val(i, known_methods))
+        d["iterItems"]["items"] = reconstructed_iteritems
+
+    return LiveObjectProxy(d, known_methods)
+
+
+def serialise_val(v, known_liveobject_methods):
+    import datetime
+    if isinstance(v, long_type) and not isinstance(v, bool):
+        return {
+            "type": ["Long"],
+            "value": str(v)
+        }
+    elif isinstance(v, float) and (v == POS_INFINITY or v == NEG_INFINITY or math.isnan(v)):
+        return {
+            "type": ["Float"],
+            "value": "Infinity" if v == POS_INFINITY else \
+                        "-Infinity" if v == NEG_INFINITY else \
+                        "NaN"
+        }
+    elif isinstance(v, (numbers.Number, bool, string_type)) or v is None:
+        return {
+            "type": ["Primitive"],
+            "value": v
+        }
+    elif isinstance(v, anvil.LiveObject):
+        return serialise_live_object(v, known_liveobject_methods)
+    elif isinstance(v, datetime.datetime):
+        s = "%04d-%02d-%02d %02d:%02d:%02d.%06d" % (v.year, v.month, v.day, v.hour, v.minute, v.second, v.microsecond)
+
+        if v.tzinfo is not None:
+            offset = v.tzinfo.utcoffset(v).total_seconds()
+        else:
+            offset = anvil.tz.tzlocal().utcoffset(v).total_seconds()
+
+        sign = "+" if offset >= 0 else "-"
+        z = "%s%02d%02d" % (sign, abs(int(offset/3600)), int((offset % 3600)/60))
+
+        return {
+            "type": ["DateTime"],
+            "value": s + z
+        }
+    elif isinstance(v, datetime.date):
+        s = "%04d-%02d-%02d" % (v.year, v.month, v.day)
+        return {
+            "type": ["Date"],
+            "value": s
+        }
+    elif isinstance(v, LazyMedia):
+        return dict(v._spec)
+    else:
+        for [n, cls] in _value_types.items():
+            if isinstance(v, cls):
+                type_name = n
+                break
+        else:
+            raise Exception("Cannot serialise object of type %s" % type(v).__name__)
+
+        return {
+            "type": ["ValueType"],
+            "typeName": type_name
+        }
+
+
+def serialise_live_object(obj, known_methods):
+    obj = obj._spec.copy()
+    obj["type"] = ["LiveObject"]
+
+    km = known_methods.get(obj["backend"])
+    if obj["methods"] == km:
+        del obj["methods"]
+    else:
+        known_methods[obj["backend"]] = obj["methods"]
+
+    serialised_item_cache = {}
+    for k,v in sorted(obj.get("itemCache", {}).items(), key=lambda x: x[0]):
+        # Dictionaries aren't ordered, so we can't allow this element
+        # to write into known_methods. We give it a copy instead.
+        serialised_item_cache[k] = serialise_val(v, known_methods.copy())
+    obj["itemCache"] = serialised_item_cache
+
+    if obj.get("iterItems"):
+        serialised_iteritems = []
+        for i in obj["iterItems"]["items"]:
+            serialised_iteritems.append(serialise_val(i, known_methods))
+        obj["iterItems"]["items"] = serialised_iteritems
+
+    return obj
+
+
+def _repr_path(p):
+    return "".join(("[%s]" % repr(k) for k in p))
+
+def _module_prefixes(module):
+    module_parts = module.split(".")
+    return [".".join(module_parts[:i]) for i in range(1, len(module_parts)+1)]
+
+_called_serialization_helpers = set()
+
+def _check_and_call_serialization_helper(cls_fullname):
+    "checks if a class has a registered helper, calls the helper if it exists (once)"
+    if cls_fullname in _called_serialization_helpers:
+        return False
+
+    for prefix in _module_prefixes(cls_fullname):
+        if prefix in _serialization_helpers:
+            _serialization_helpers[prefix](cls_fullname)
+            _called_serialization_helpers.add(cls_fullname)
+            return True
+
+    return False
+
+
+def fill_out_media(json, handle_media_fn, collect_capabilities=None, remote_is_trusted=False):
+    obj_descr = []
+    path = []
+    known_liveobject_methods = {}
+    serialization_info = SerializationInfo(remote_is_trusted=remote_is_trusted)
+    import datetime
+
+    def do_fom(_json):
+
+        t_json = type(_json)
+
+        if hasattr(_json, "SERIALIZATION_INFO"):
+            type_name, tp = _json.SERIALIZATION_INFO
+            valid_type_name = type_name in _value_types
+
+            if valid_type_name and tp is _json:
+                _json = None
+                obj_descr.append({
+                    "type": ["ClassType"],
+                    "path": list(path),
+                    "typeName": type_name
+                })
+
+            elif not valid_type_name or t_json is not tp:
+                raise SerializationError("Cannot serialize %s (must be registered with @anvil.server.portable_class) at msg%s" % (t_json, _repr_path(path)))
+            else:
+                serialization_info._set_default_key(type_name)
+
+                try:
+                    serialize = _json.__serialize__
+                except AttributeError:
+                    def serialize(_):
+                        return _json.__dict__
+
+                content = serialize(serialization_info)
+
+                _json = do_fom(content)
+
+                # Append this afterwards, so we deserialise our content first
+                obj_descr.append({
+                    "type": ["ValueType"],
+                    "path": list(path),
+                    "typeName": type_name
+                })
+
+        elif isinstance(_json, dict):
+            _json = dict(_json)
+            for k,v in sorted(_json.items(),key=lambda x: x[0]):
+                if not isinstance(k, string_type):
+                    raise SerializationError("Cannot serialize dictionaries with keys that aren't strings at msg%s" % _repr_path(path + [k]))
+                path.append(k)
+                _json[k] = do_fom(v)
+                path.pop()
+        elif isinstance(_json, list) or isinstance(_json, tuple):
+            _json = list(_json)
+            for i in range(len(_json)):
+                path.append(i)
+                _json[i] = do_fom(_json[i])
+                path.pop()
+        elif isinstance(_json, LazyMedia):
+            d = dict(_json._spec)
+            d["path"] = list(path)
+            obj_descr.append(d)
+            _json = None
+        elif isinstance(_json, anvil.Media):
+            extra = handle_media_fn(_json)
+            d = {"type": ["DataMedia"], "path": list(path), "mime-type": _json.content_type, "name": _json.name}
+            if extra is not None:
+                d.update(extra)
+            obj_descr.append(d)
+            _json = None
+        elif isinstance(_json, Capability):
+            if collect_capabilities is not None:
+                collect_capabilities.append(_json)
+            d = {
+                "type": ["Capability"],
+                "path": list(path),
+                "scope": _json._scope,
+                "mac": _json._mac
+            }
+            if _json._narrow:
+                d["narrow"] = _json._narrow
+            obj_descr.append(d)
+            _json = None
+        elif isinstance(_json, anvil.LiveObject):
+            #print "Serialising LiveObject: " + repr(_json._spec) + " at " + repr(path)
+            serialised_liveobject = serialise_live_object(_json, known_liveobject_methods)
+            serialised_liveobject["path"] = list(path)
+            obj_descr.append(serialised_liveobject)
+            _json = None
+        elif isinstance(_json, (datetime.date, datetime.datetime)) or \
+                (isinstance(_json, long_type) and (_json > 2147483647 or _json < -2147483647)) or \
+                (isinstance(_json, float) and (_json == POS_INFINITY or _json == NEG_INFINITY or math.isnan(_json))):
+            serialised_val = serialise_val(_json, known_liveobject_methods)
+            serialised_val["path"] = list(path)
+            obj_descr.append(serialised_val)
+            _json = None
+        elif _check_and_call_serialization_helper(t_json.__module__ + "." + t_json.__name__):
+            _json = do_fom(_json)
+        elif 'numpy' in sys.modules and hasattr(sys.modules['numpy'], 'generic') and isinstance(_json, sys.modules['numpy'].generic):
+
+            _json = _json.item() # convert
+
+        elif not (isinstance(_json, string_type) or _json is None or _json is True or _json is False or isinstance(_json, (int, long_type)) or isinstance(_json, float)):
+
+            # Rescue: Convert numpy types to nearest equivalent
+            if 'numpy' in sys.modules:
+                import numpy
+                if isinstance(_json, numpy.ndarray):
+                    _json = do_fom(_json.tolist())
+                else:
+                    raise SerializationError("Cannot serialize %s object at msg%s" % (t_json, _repr_path(path)))
+            else:
+                raise SerializationError("Cannot serialize %s object at msg%s" % (t_json, _repr_path(path)))
+
+        return _json
+
+    json = do_fom(json)
+
+    vt_global = serialization_info._to_json()
+    if len(vt_global) != 0:
+        path.append("vt_global")
+        serialization_info._set_txdata_available(False)
+        od = obj_descr
+        obj_descr = []
+        json["vt_global"] = do_fom(vt_global)
+        obj_descr += od
+        path.pop()
+
+    json["objects"] = obj_descr
+
+    return json
+
+
+def fill_out_cap_updates(resp, caps_passed_in):
+    """We're about to return from a call; ask all the capabilities that got passed in whether they want to send
+       any updates to our caller."""
+
+    for cap in caps_passed_in:
+        update = cap._get_update()
+        if update is not None:
+            cu = resp.get('capUpdates')
+            if cu is None:
+                cu = resp['capUpdates'] = {}
+            cu[json.dumps(cap.scope)] = update
+
+
+def apply_cap_updates(resp, caps_passed_out):
+    """We have just made a server call that has returned. Apply any necessary updates to the capabilities we
+       passed into this call"""
+
+    updates = resp.get('capUpdates', {})
+
+    # Normalise updates to how _this_ `json` impl does things (ugh)
+    updates = {json.dumps(json.loads(k)): v for k,v in updates.items()}
+
+    for cap in caps_passed_out:
+        scope_json = json.dumps(cap.scope)
+        update = updates.get(scope_json)
+        if update is not None:
+            cap._apply_update(update)
+
+
+def simple_strpdate(s):
+    import datetime
+    return datetime.date(int(s[0:4]), int(s[5:7]), int(s[8:10]))
+
+
+def simple_strpdatetime(s):
+    import datetime
+    return datetime.datetime(int(s[0:4]), int(s[5:7]), int(s[8:10]), int(s[11:13]), int(s[14:16]), int(s[17:19]), int(s[20:26])) # datetime.datetime.strptime(s, "%Y-%m-%d %H:%M:%S.%f")
+
+def parsedate(s):
+    return simple_strpdate(s)
+
+
+def parsedatetime(s):
+
+    has_tz = len(s) > 5 and \
+             (s[-5] == "-" or s[-5] == "+") and \
+             48 <= ord(s[-4]) <= 57 and \
+             48 <= ord(s[-3]) <= 57 and \
+             48 <= ord(s[-2]) <= 57 and \
+             48 <= ord(s[-1]) <= 57
+
+    if not has_tz:
+        # Parse a naive datetime
+        return simple_strpdatetime(s)
+
+    # Timezone present. First parse without it
+    d = simple_strpdatetime(s[:-5])
+
+    # Now construct a tzoffset
+    hours = int(s[-5:-2])
+    minutes = int(s[-5] + s[-2:])
+    total_minutes = hours*60+minutes
+
+    return d.replace(tzinfo=anvil.tz.tzoffset(minutes=total_minutes))
+
+def _retrieve_portable_class(type_name, d):
+    value_type = _value_types.get(type_name)
+    if value_type is not None:
+        return value_type
+    # Try importing the relevant module
+    i = type_name.rfind('.')
+    if i != -1:
+        # TODO do we filter what we can specify as import? I don't *think* this is dangerous...
+        if not _check_and_call_serialization_helper(type_name):
+            module_name = type_name[:i]
+            importlib.import_module(module_name)
+        value_type = _value_types.get(type_name)
+
+    if value_type is None:
+        raise SerializationError("No such serializable type: %s at msg%s" % (type_name, _repr_path(d["path"])))
+
+    return value_type
+
+
+def _reconstruct_objects(json, reconstruct_data_media, hold_back_value_types=False, collect_capabilities=None, remote_is_trusted=False):
+    known_liveobject_methods = {}
+    serialization_info = SerializationInfo(json.get("vt_global"), remote_is_trusted=remote_is_trusted) if not hold_back_value_types else None
+
+    if "objects" in json:
+        held_back_objects = []
+        for d in json["objects"]:
+            if hold_back_value_types and ("ValueType" in d["type"] or "ClassType" in d["type"]):
+                held_back_objects.append(d)
+                continue
+
+            reconstructed = reconstruct_val(d, known_liveobject_methods, reconstruct_data_media)
+            if collect_capabilities is not None and type(reconstructed) is Capability:
+                collect_capabilities.append(reconstructed)
+
+            obj = json
+            last_obj = None
+            key = None
+            for k in d["path"]:
+                last_obj = obj
+                key = k
+                obj = obj[k]
+
+            if last_obj is not None:
+
+                if "ValueType" in d["type"]:
+                    # Hack: The "reconstructed value" here is actually just the type name
+                    type_name = reconstructed
+                    value_type = _retrieve_portable_class(type_name, d)
+                    try:
+                        reconstruct = value_type.__new_deserialized__
+                    except AttributeError:
+                        def reconstruct(data, info):
+                            obj = value_type.__new__(value_type)
+                            try:
+                                deserialize = obj.__deserialize__
+                            except AttributeError:
+                                def deserialize(data, info):
+                                    obj.__dict__.update(data)
+                            deserialize(data, info)
+                            return obj
+
+                    serialization_info._set_txdata_available(d["path"][0] != 'vt_global')
+                    serialization_info._set_default_key(type_name)
+                    last_obj[key] = reconstruct(last_obj[key], serialization_info)
+                elif "ClassType" in d["type"]:
+                    last_obj[key] = _retrieve_portable_class(reconstructed, d)
+                else:
+                    last_obj[key] = reconstructed
+
+        if hold_back_value_types:
+            json["objects"] = held_back_objects
+        else:
+            del json["objects"]
+
+    return json
+
+on_register = None # optional
+registrations = {}
+
+class HttpRequest(object):
+
+    def __init__(self):
+        self._prevent_access = True
+
+    def __getattribute__(self, name):
+        if object.__getattribute__(self, "_prevent_access"):
+            raise Exception("anvil.server.request is only available in http_endpoint calls.")
+
+        return object.__getattribute__(self, name)
+
+    @property
+    def body_json(self):
+        if hasattr(self, "_body_json"):
+            return self._body_json
+        elif self.body is not None and self.headers.get("content-type", None) == "application/json":
+            self._body_json = json.loads(self.body.get_bytes())
+        else:
+            self._body_json = None
+        return self._body_json
+
+
+
+
+api_request = HttpRequest()
+
+def _lower_str(s):
+    if not isinstance(s, str):
+        return s
+    return s.lower()
+
+class HttpHeaders(object):
+
+    def __init__(self, headers=None):
+        headers = headers or {}
+        assert isinstance(headers, dict), "headers should be a dict"
+        headers = {_lower_str(h): v for (h, v) in headers.items()}
+        self._headers = list(headers.items())
+
+    def __setitem__(self, name, val):
+        name = _lower_str(name)
+        self._headers = [(h,v) for (h,v) in self._headers if h != name]
+
+        self.add(name, val)
+
+    def __delitem__(self, name):
+        name = _lower_str(name)
+        self._headers = [(h,v) for (h,v) in self._headers if h != name]
+
+    def add(self, name, val):
+        self._headers.append((name, val))
+
+    def clear(self):
+        self._headers = []
+
+    def copy(self):
+        new_self = HttpHeaders()
+        new_self._headers = self._headers.copy()
+        return new_self
+
+    def __repr__(self):
+        return "HttpHeaders(" + repr(self._headers) + ")"
+
+
+class HttpResponse(object):
+    def __init__(self, status=200, body="", headers=None):
+        self.status = status
+        self.body = body
+        self.headers = headers
+
+    @property
+    def headers(self):
+        return self._headers
+
+    @headers.setter
+    def headers(self, value):
+        if value is None or isinstance(value, dict):
+            self._headers = HttpHeaders(value)
+        elif isinstance(value, HttpHeaders):
+            self._headers = value.copy()
+        else:
+            raise TypeError("headers should be set to a dictionary")
+
+
+class CallContext(object):
+    class ClientInfo(object):
+        def __repr__(self):
+            return "<ClientInfo:%s>" % repr(self.__dict__)
+
+    class Location(object):
+        def __init__(self, location):
+            self.city = location.get('city')
+
+            self.subdivision = location.get('subdivision', {}).get('name')
+
+            l = location.get('location', {})
+            self.latitude = l.get('lat')
+            self.longitude = l.get('lng')
+
+            c = location.get('country', {})
+            self.country_code = c.get('code')
+            self.country = c.get('name')
+
+        def __repr__(self):
+            return "<Location:%s>" % repr(self.__dict__)
+
+    class StackFrame(object):
+        def __init__(self, sf):
+            self.type = sf.get("type")
+            self.is_trusted = self.type in {'server_module', 'uplink', 'background_task'}
+
+        def __repr__(self):
+            return "<StackFrame:%s>" % repr(self.__dict__)
+
+    _DEFAULT_TYPE = "server_module"
+
+    def _setup(self, client, call_stack):
+        self.type = CallContext._DEFAULT_TYPE
+        if client is not None:
+            self.client = CallContext.ClientInfo()
+            self.client.type = client.get('type')
+            self.client.ip = client.get('ip')
+            self.background_task_id = client.get('background-task-id')
+            l = client.get('location')
+            self.client.location = CallContext.Location(l) if l else None
+            self.remote_caller = CallContext.StackFrame(call_stack[0] if call_stack else client)
+        else:
+            self.client = None
+            self.remote_caller = None
+            self.background_task_id = None
+
+    __init__ = _setup
+
+    def __repr__(self):
+        return "<CallContext:%s>" % repr(self.__dict__)
+
+
+# can be used as a decorator too
+# N.B. There is a full implementation of the 'require=' kwarg here, but we've chosen not to expose it yet. If we expose it, will need to pass through from callable, like require_user.
+def register(fn, name=None, name_prefix=None, require_user=None):
+    require=None
+
+    if isinstance(fn, string_type):
+        # Someone's using the old syntax. Our bad.
+        (fn, name) = (name, fn)
+
+    if name is None:
+        name = fn.__name__
+
+    original_name = name
+    if name_prefix is not None:
+        name = "%s:%s" % (name_prefix, name)
+
+    # 'require_user' is either True (check that user is logged in), False (equivalent to None), or 
+    # a function that takes the currently logged in user and returns whether to let them in.
+
+    if require_user == True:
+        def simple_require_user():
+            import anvil.users
+            if anvil.users.get_user() is None:
+                raise anvil.users.AuthenticationFailed("You must be logged in to call this server function")
+            return True
+        require = simple_require_user
+    elif require_user == False:
+        require = None
+    elif require_user is not None:
+        # Must be a function.
+        def complex_require_user():
+            import anvil.users
+            user = anvil.users.get_user()
+            if user is None:
+                raise anvil.users.AuthenticationFailed("You must be logged in to call server function '%s'" % original_name)
+            elif not require_user(user):
+                raise PermissionDenied("You do not have permission to call server function '%s'" % original_name)
+            else:
+                return True
+        require = complex_require_user
+
+    # 'require' is an optional function that returns something truthy if the user should be let in. Otherwise, it can raise 
+    # an Exception (which will be passed on) or return something falsey (in which case a PermissionDenied exception will be raised.)
+
+    if require is not None:
+        def require_wrap(f):
+            def with_req(*args, **kwargs):
+                if require():
+                    return f(*args, **kwargs)
+                else:
+                    raise PermissionDenied("You do not have permission to call server function '%s'" % original_name)
+            return with_req
+    else:
+        def require_wrap(f):
+            return fn
+
+    registrations[name] = require_wrap(fn)
+
+    if on_register is not None:
+        on_register(name, False)
+
+    def reregister(new_f):
+        registrations[name] = require_wrap(new_f)
+        new_f._anvil_reregister = reregister
+
+    fn._anvil_reregister = reregister
+
+    return fn
+
+#!defFunction(anvil.server,%,[name], [require_user])!2: {anvil$args: {fn_or_name: "The name by which you want to call your function from the client.", require_user: "Allows you to verify whether a user is logged in. Can be a boolean or a function."}, anvil$helpLink: "server#calling-server-functions-from-client-code", $doc: "When applied to a function as a decorator, the function becomes available from the client side."} ["callable"]
+def callable(fn_or_name=None, require_user=None):
+    if fn_or_name is None or isinstance(fn_or_name, string_type):
+        return lambda f: register(f, fn_or_name, require_user=require_user)
+    else:
+        return register(fn_or_name)
+
+
+def background_task(fn_or_name=None):
+    if fn_or_name is None or isinstance(fn_or_name, string_type):
+        return lambda f: register(f, fn_or_name, name_prefix="task")
+    else:
+        return register(fn_or_name, name_prefix="task")
+
+
+# A parameterised decorator
+def callable_as(name):
+    print("@callable_as is deprecated. Please use @callable directly.")
+    return lambda f: register(f, name)
+
+
+
+def http_endpoint(path, require_credentials=False, authenticate_users=False, authenticate_user=False,
+                  methods=["GET","POST"], enable_cors=False, cross_site_session=False, _task_prefix="http"):
+    def decorator(fn):
+        path_parts = []
+        def register_path_part(s):
+            path_parts.append(s.group(1))
+            return "([^/]*)"
+
+        path_regex = re.sub(":([^/]*)", register_path_part, path)
+
+        def wrapped_fn(method, path, query_params, form_params, origin, headers, remote_address, body, username, password, same_app_alternate_origin=None, **more_kwargs):
+
+            api_request._prevent_access = False
+
+            if cross_site_session:
+                import anvil.server
+                anvil.server._switch_session()
+
+            api_request.user = None
+            if authenticate_users or authenticate_user:
+                import anvil.users
+                try:
+                    api_request.user = anvil.users.get_user() or \
+                                        anvil.users.login_with_email(username, password)
+                except Exception as e:
+                    return {"status": 401,
+                            "body": "Unauthorized",
+                            "headers": {"WWW-Authenticate": "Basic realm=\"Anvil App API\""}}
+            elif require_credentials:
+                if username is None or password is None:
+                    return {"status": 401,
+                            "body": "Unauthorized",
+                            "headers": {"WWW-Authenticate": "Basic realm=\"Anvil App API\""}}
+
+            def add_cross_origin_to_header_dict(d):
+                if enable_cors:
+                    d["Access-Control-Allow-Origin"] = enable_cors if isinstance(enable_cors, str) else "*"
+                elif same_app_alternate_origin:
+                    d["Access-Control-Allow-Origin"] = same_app_alternate_origin
+                if enable_cors or same_app_alternate_origin and \
+                        "access-control-allow-headers" not in [h.lower() for h in d.keys()]:
+                    allow_headers = ["content-type"]
+                    for k in headers.keys():
+                        if k.lower() == "access-control-request-headers":
+                            hs = [h.strip().lower() for h in headers[k].split(",")]
+                            allow_headers += [h for h in hs if h not in allow_headers]
+
+                    d["Access-Control-Allow-Headers"] = ", ".join(allow_headers)
+
+                return d
+
+            if method not in methods:
+                if method == "OPTIONS" and (enable_cors or same_app_alternate_origin):
+                    return {"status": 200,
+                            "body": "",
+                            "headers": add_cross_origin_to_header_dict({})}
+                else:
+                    return {"status": 405,
+                            "body": "Method not supported",
+                            "headers": {"Allow": ", ".join(methods)}}
+
+            api_request.path = path
+            api_request.method = method
+            api_request.query_params = query_params
+            api_request.form_params = form_params
+            api_request.origin = origin
+            api_request.headers = headers
+            api_request.remote_address = remote_address
+            api_request.body = body
+            api_request.username = username
+            api_request.password = password
+
+
+            # Path takes precedence over query params. Query params take precedence over form params.
+            kwargs = dict(form_params)
+            kwargs.update(query_params)
+            match = re.match(path_regex, path)
+            for i,m in enumerate(match.groups()):
+                kwargs[path_parts[i]] = m
+
+            response = fn(**kwargs)
+
+            api_request._prevent_access = True
+
+            if isinstance(response, HttpResponse):
+                return {"status":  response.status,
+                        "body":    response.body,
+                        "headers": add_cross_origin_to_header_dict(response.headers)._headers}
+            else:
+                return {"status":  200,
+                        "body":    response,
+                        "headers": add_cross_origin_to_header_dict({})}
+
+        register(wrapped_fn, path_regex, _task_prefix)
+
+        return fn
+    return decorator
+
+
+wellknown_endpoint = functools.partial(http_endpoint, _task_prefix = "http-wellknown")
+
+
+class AnvilCookie(object):
+
+    def __init__(self, type):
+        self._type = type
+
+    def __getitem__(self, name):
+        return _do_call([self._type, name], None, fn_name="anvil.private.get_cookie")
+
+    def __setitem__(self, name, value):
+        kw = {}
+        kw[name] = value
+        self.set(30, **kw)
+
+    def __delitem__(self, name):
+        _do_call([self._type, name], None, fn_name="anvil.private.del_cookie")
+
+    def get(self, key, default=None):
+        try:
+            return _do_call([self._type, key], None, fn_name="anvil.private.get_cookie")
+        except KeyError:
+            return default
+
+    def set(self, timeout_days=30, **values):
+        _do_call([self._type, timeout_days], values, fn_name="anvil.private.set_cookie")
+
+    def clear(self):
+        _do_call([self._type], None, fn_name="anvil.private.clear_cookie")
+
+
+class CookieContainer(object):
+
+    def __init__(self):
+        self.local = AnvilCookie("local")
+        self.shared = AnvilCookie("shared")
+
+
+cookies = CookieContainer()
+
+
+class NotABackgroundTaskState(object):
+    def __setitem__(self, key, value):
+        raise Exception("Cannot access anvil.server.task_state outside a background task")
+
+    def __getitem__(self, item):
+        raise Exception("Cannot access anvil.server.task_state outside a background task")
+
+
+# Raise event on all sessions in the current environment, on a specific session, on multiple sessions, or on a named channel
+def raise_event(name, payload=None, session_id=None, session_ids=None, channel=None):
+    anvil.server.call("anvil.private.raise_event", name, payload, session_id=session_id, session_ids=session_ids, channel=channel)
+
+
+# List all sessions in the current environment, or only those where the specified user is logged in.
+def list_client_sessions(user=None):
+    return anvil.server.call("anvil.private.list_sessions", user=user)
+
+
+# Get the value of anvil.server.session for a particular session in the current environment
+def get_client_session(session_id):
+    return anvil.server.call("anvil.private.get_session_data", session_id)
+
+
+# Get the ID of the current session
+#!defFunction(anvil.server,%)!2: "Returns the current session's ID." ["get_session_id"]
+def get_session_id():
+    return anvil.server.call("anvil.private.get_session_id")
+
+
+# Subscribe this session to receive events from the named channel
+def subscribe(channel):
+    return anvil.server.call("anvil.private.subscribe", channel)
+
+
+# Unsubscribe this session from receiving events from the named channel
+def unsubscribe(channel):
+    return anvil.server.call("anvil.private.unsubscribe", channel)
+
+
+def get_subscriptions():
+    return anvil.server.call("anvil.private.get_subscriptions")
+
+
+def plotly_serialization_helper(class_fullname):
+    name_parts = class_fullname.split(".")
+    module_name = ".".join(name_parts[:-1])
+    class_name = name_parts[-1]
+
+    module = importlib.import_module(module_name)
+    cls = getattr(module, class_name)
+
+    if not hasattr(cls, '__serialize__'):
+        # print(f"Registering {cls}")
+        def serialize(self, global_data):
+            # print("Serialising %s on downlink" % type(self))
+            return self.to_plotly_json()
+
+        @staticmethod
+        def new_deserialized(data, global_data):
+            # print("Deserialising %s on downlink" % cls)
+            return cls(data)
+
+        cls.__serialize__ = serialize
+        cls.__new_deserialized__ = new_deserialized
+        portable_class(cls, class_fullname)
+
+
+_serialization_helpers["plotly.graph_objs"] = plotly_serialization_helper
```

### Comparing `anvil-app-server-1.8.0/anvil_downlink_worker/anvil/_threaded_server.py` & `anvil-app-server-1.9.0/anvil_downlink_worker/anvil/_threaded_server.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,437 +1,437 @@
-# Helpers for implementing anvil.server on an (optionally threaded) Real Python process.
-# Used in uplink and downlink, and now even in the PyPy sandbox.
-
-import random, string, json, re, sys, time, importlib, anvil
-
-
-# For single-threaded implementations, re-entrant calls occupy the same thread,
-# so we fake "switching a thread" by pushing all the thread-locals onto a stack
-# while we're handling an inner call
-class StackableLocal(object):
-    def _push_stack(self):
-        _nested = dict(self.__dict__)
-        self.__dict__.clear()
-        self.__dict__['_nested'] = _nested
-        self.__init__()
-
-    def _pop_stack(self):
-        nested = self._nested
-        self.__dict__.clear()
-        self.__dict__.update(nested)
-
-    def __new__(cls, *args, **kwargs):
-        v = object.__new__(cls)
-        cls.__init__(v, *args, **kwargs)
-        _stackables.append(v)
-        return v
-
-
-_stackables = []
-
-try:
-    import threading
-    ThreadLocal = threading.local
-    MULTITHREADED = True
-except:
-    MULTITHREADED = False
-    ThreadLocal = StackableLocal
-
-
-from . import  _serialise, _server
-from ._server import LazyMedia, registrations
-
-string_type = str if sys.version_info >= (3,) else basestring
-
-console_output = sys.stdout
-
-class HttpRequest(ThreadLocal):
-
-    def __init__(self):
-        self._prevent_access = True
-
-    def __getattribute__(self, name):
-        if name not in ['_push_stack', '_pop_stack', '_nested', '__dict__', '__init__'] and \
-                ThreadLocal.__getattribute__(self, "_prevent_access"):
-            raise Exception("anvil.server.request is only available in http_endpoint calls.")
-
-        return ThreadLocal.__getattribute__(self, name)
-
-    @property
-    def body_json(self):
-        if hasattr(self, "_body_json"):
-            return self._body_json
-        elif self.body is not None and self.headers.get("content-type", None) == "application/json":
-            self._body_json = json.loads(self.body.get_bytes())
-        else:
-            self._body_json = None
-        return self._body_json
-
-
-_server.api_request = HttpRequest()
-
-
-def gen_id():
-    sr = random.SystemRandom()
-    chars = string.ascii_letters + string.digits
-    return ''.join(sr.choice(chars) for _ in range(10))
-
-
-# Overwrite with functions from context
-send_reqresp = None
-
-
-class LocalCallInfo(ThreadLocal):
-    def __init__(self):
-        self.call_id = None
-        self.stack_id = None
-        self.session = None
-        self.cache_filter = {}
-        self.cache_update = {}
-        self.dump_task_state = False
-        self.enable_profiling = False
-
-    def __getitem__(self, item):
-        return self.session.__getitem__(item)
-
-    def __setitem__(self, key, value):
-        return self.session.__setitem__(key, value)
-
-    def __delitem__(self, key):
-        del self.session[key]
-
-    def get(self, key, default=None):
-        return self.session.get(key, default)
-
-    def __iter__(self):
-        return self.session.__iter__()
-
-    def __repr__(self):
-        return "<Session:%s>" % repr(self.session)
-
-
-class LocalCallContext(_server.CallContext, ThreadLocal):
-    def __init__(self):
-        self._setup(None, [])
-
-
-call_info = LocalCallInfo()
-call_context = LocalCallContext()
-call_responses = {}
-waiting_for_calls = threading.Condition() if MULTITHREADED else None
-
-
-# If MULTITHREADED is False, better overwrite this
-def poll_for_call_responses(*args):
-    raise AssertionError("We're in single-threaded mode, but poll_for_call_responses() is not set")
-
-
-backends = {}
-
-
-def _switch_session():
-    import anvil.server
-    sjson = anvil.server.call('anvil.private.switch_session!') or {"session": {}, "objects": []}
-    call_info.session = _server._reconstruct_objects(sjson, None, remote_is_trusted=True)["session"]
-
-
-default_app = anvil.app
-
-
-class LocalAppInfo(ThreadLocal):
-    def __getattr__(self, attr):
-        return getattr(default_app, attr)
-
-    def __setattr__(self, key, value):
-        raise AttributeError("This object is read-only")
-
-    def _setup(self, environment={}, **kwargs):
-        self.__dict__.update(kwargs, environment=anvil._AppInfo._Environment(**environment))
-
-
-anvil.app = LocalAppInfo()
-
-
-class SendNoResponse(Exception):
-    pass
-
-
-class IncomingRequest(_serialise.IncomingReqResp):
-    def __init__(self, json, import_modules=None, run_fn=None, dump_task_state=False, setup_task_state=None):
-        self.import_modules = import_modules
-        self.run_fn = run_fn
-        self.dump_task_state = dump_task_state
-        self.setup_task_state = setup_task_state
-        remote_is_trusted = _server.CallContext.StackFrame(json.get('call-stack', [{}])[0]).is_trusted
-        _serialise.IncomingReqResp.__init__(self, json, remote_is_trusted=remote_is_trusted)
-
-    def execute(self):
-        def make_call():
-            call_info.call_id = self.json.get('id')
-            call_info.stack_id = self.json.get('call-stack-id', None)
-            call_info.session_id = self.json.get('session-id')
-            sjson = self.json.get('sessionData', {'session': None, 'objects': []})
-            call_info.session = None
-            call_info.enable_profiling = self.json.get('enable-profiling', False)
-            if call_info.enable_profiling:
-                call_info.profile = {
-                    "origin": "Server (Python)",
-                    "description": "Python _threaded_server execution",
-                    "start-time": time.time()*1000,
-                }
-            call_info.cache_filter = _server.get_liveobject_cache_filter_spec([self.json.get('args'), self.json.get('kwargs')])
-            call_info.cache_update = {}
-            call_info.dump_task_state = self.dump_task_state
-            call_context._setup(self.json.get('client', {}), self.json.get('call-stack'))
-            anvil.app._setup(**self.json.get('app-info', {}))
-            if self.setup_task_state:
-                self.setup_task_state(call_info.call_id, True)
-            import_complete = False
-            try:
-                if self.import_modules:
-                    self.import_modules()
-                import_complete = True
-
-                # Now we've imported enough to deserialise custom types
-                self.reconstruct_remaining_data()
-                call_info.session = _server._reconstruct_objects(sjson, None, remote_is_trusted=self.remote_is_trusted).get("session", {})
-
-                if self.run_fn is not None:
-                    response = self.run_fn()
-                elif 'liveObjectCall' in self.json:
-                    loc = self.json['liveObjectCall']
-                    spec = dict(loc)
-
-                    if call_context.remote_caller is None:
-                        spec["source"] = "UNKNOWN"
-                    elif call_context.remote_caller.is_trusted:
-                        spec["source"] = "server"
-                    else:
-                        spec["source"] = "client"
-
-                    del spec["method"]
-                    backend = loc['backend']
-                    if backend not in backends:
-                        raise Exception("No such LiveObject backend: " + repr(backend))
-                    inst = backends[backend](spec)
-                    method = getattr(inst, loc['method'])
-
-                    call_info.cache_filter.setdefault(backend, set()).add(spec['id'])
-
-                    response = method(*self.json['args'], **self.json['kwargs'])
-                else:
-                    command = self.json['command']
-                    for reg in registrations:
-                        m = re.match(reg, command)
-                        if m and len(m.group(0)) == len(command):
-                            response = registrations[reg](*self.json["args"], **self.json["kwargs"])
-                            break
-                    else:
-                        if self.json.get('stale-uplink?'):
-                            raise _server.UplinkDisconnectedError({'type': 'anvil.server.UplinkDisconnectedError',
-                                                                   'message':'The uplink server for "%s" has been disconnected' % command})
-
-                        else:
-                            raise _server.NoServerFunctionError({'type': 'anvil.server.NoServerFunctionError',
-                                                                 'message': 'No server function matching "%s" has been registered' % command})
-
-                def err(*args):
-                    raise Exception("Cannot save DataMedia objects in anvil.server.session")
-
-                try:
-                    sjson = _server.fill_out_media({'session': call_info.session}, err, remote_is_trusted=True)
-                    json.dumps(sjson)
-                except TypeError as e:
-                    raise _server.SerializationError("Tried to store illegal value in a anvil.server.session. " + e.args[0])
-                except _server.SerializationError as e:
-                    raise _server.SerializationError("Tried to store illegal value in a anvil.server.session. " + e.args[0])
-
-                resp = {"id": self.json["id"], "response": response, "sessionData": sjson, "cacheUpdates": call_info.cache_update}
-
-                if call_info.enable_profiling:
-                    call_info.profile["end-time"] = time.time()*1000
-                    resp["profile"] = call_info.profile
-
-                _server.fill_out_cap_updates(resp, self.capabilities)
-
-                if self.dump_task_state:
-                    try:
-                        task_state = dict(anvil.server.task_state)
-                        tjson = _server.fill_out_media({'taskState': task_state}, err, remote_is_trusted=True)
-                        json.dumps(tjson)
-                        resp['taskState'] = task_state
-                    except (TypeError, _server.SerializationError):
-                        pass
-
-                try:
-                    send_reqresp(resp, remote_is_trusted=call_context.remote_caller.is_trusted)
-                except _server.SerializationError as e:
-                    raise _server.SerializationError("Cannot serialize return value from function. " + str(e))
-            except SendNoResponse:
-                pass
-            except:
-
-                e = _server._report_exception(self.json["id"])
-
-                if self.dump_task_state:
-                    def err(*args):
-                        raise Exception("Cannot save DataMedia objects in anvil.server.session")
-
-                    try:
-                        task_state = dict(anvil.server.task_state)
-                        tjson = _server.fill_out_media({'taskState': task_state}, err, remote_is_trusted=True)
-                        json.dumps(tjson)
-                    except (TypeError, _server.SerializationError):
-                        pass
-                    else:
-                        e['taskState'] = task_state
-
-                if not import_complete:
-                    e['moduleLoadFailed'] = True
-
-                try:
-                    send_reqresp(e)
-                except:
-                    trace = "\ncalled from ".join(["%s:%s" % (t[0], t[1]) for t in e["error"]["trace"]])
-                    console_output.write(("Failed to report exception: %s: %s\nat %s\n" % (e["error"]["type"], e["error"]["message"], trace)).encode("utf-8"))
-                    console_output.flush()
-            finally:
-                if self.setup_task_state:
-                    self.setup_task_state(call_info.call_id, False)
-                self.complete()
-
-        if MULTITHREADED:
-            threading.Thread(target=make_call).start()
-        else:
-            make_call()
-
-    def complete(self):
-        pass
-
-
-class IncomingResponse(_serialise.IncomingReqResp):
-    def __init__(self, json):
-        # Responses from the server are trusted by definition
-        _serialise.IncomingReqResp.__init__(self, json, remote_is_trusted=True)
-
-    def execute(self):
-        id = self.json['id']
-        if id in call_responses:
-            call_responses[id] = (self, self.json)
-            if MULTITHREADED:
-                with waiting_for_calls:
-                    waiting_for_calls.notifyAll()
-        else:
-            print("Got a response for an unknown ID: " + repr(self.json))
-
-
-def kill_outstanding_requests(msg):
-    for k in call_responses.keys():
-        if call_responses[k] is None:
-            call_responses[k] = (None, {'error': {'message': msg}})
-
-    if not MULTITHREADED:
-        raise Exception("_threaded_server.kill_outstanding_requests() does not work in single-threaded mode")
-
-    with waiting_for_calls:
-        waiting_for_calls.notifyAll()
-
-
-def register_live_object_backend(cls):
-
-    name = "uplink." + cls.__name__
-    backends[name] = cls
-
-    if _server.on_register is not None:
-        _server.on_register(name, True)
-
-    return cls
-
-
-live_object_backend = register_live_object_backend
-
-
-def do_call(args, kwargs, fn_name=None, live_object=None): # Yes, I do mean args and kwargs without *s
-    id = gen_id()
-
-    call_responses[id] = None
-
-    capabilities_for_update = []
-
-    if call_info.enable_profiling:
-        profile = {
-            "origin": "Server (Python)",
-            "description": "Outgoing call from Python _threaded_server",
-            "start-time": time.time()*1000
-        }
-
-    def send_call():
-        # print("Call stack ID = " + repr(_call_info.stack_id))
-        if call_info.stack_id is None:
-            call_info.stack_id = "outbound-" + gen_id()
-        req = {'type': 'CALL', 'id': id, 'args': args, 'kwargs': kwargs,
-               'call-stack-id': call_info.stack_id, 'originating-call': call_info.call_id}
-
-        if live_object:
-            req["liveObjectCall"] = { k: live_object._spec[k] for k in ["id", "backend", "mac", "permissions"] }
-            req["liveObjectCall"]["method"] = fn_name
-        elif fn_name:
-            req["command"] = fn_name
-        else:
-            raise Exception("Expected one of fn_name or live_object")
-        try:
-            # We're calling a server function and those are always trusted
-            send_reqresp(req, collect_capabilities=capabilities_for_update, remote_is_trusted=True)
-        except _server.SerializationError as e:
-            raise _server.SerializationError("Cannot serialize arguments to function. " + str(e))
-
-    if MULTITHREADED:
-        with waiting_for_calls:
-            send_call()
-            while call_responses[id] is None:
-                waiting_for_calls.wait()
-    else:
-        send_call()
-        dump_task_state = call_info.dump_task_state
-        # Fake a thread switch
-        for s in _stackables:
-            s._push_stack()
-        while call_responses[id] is None:
-            poll_for_call_responses(dump_task_state)
-            dump_task_state = False # only do it first time
-        for s in _stackables:
-            s._pop_stack()
-
-    if call_info.enable_profiling:
-        profile["end-time"] = time.time()*1000
-
-    reqresp, r = call_responses.pop(id)
-
-    # Now we're in the right thread, we can do any custom deserialisation
-    if reqresp:
-        reqresp.reconstruct_remaining_data()
-
-    if "cacheUpdates" in r:
-        # Apply updates to any of our own objects that were passed in
-        _server.apply_cache_updates(r['cacheUpdates'], [args, kwargs, live_object])
-        # Queue up whichever updates *we* should be returning
-        _server.combine_cache_updates(call_info.cache_update, r['cacheUpdates'], call_info.cache_filter)
-
-    _server.apply_cap_updates(r, capabilities_for_update)
-
-    if call_info.enable_profiling:
-        if "profile" in r:
-            profile["children"] = [r["profile"]]
-
-        if hasattr(call_info, "profile"):
-            if "children" not in call_info.profile:
-                call_info.profile["children"] = []
-
-            call_info.profile["children"].append(profile)
-
-    if 'response' in r:
-        return r['response']
-    if 'error' in r:
-        error_from_server = _server._deserialise_exception(r["error"])
-        raise error_from_server
-    else:
-        raise Exception("Bogus response from server: " + repr(r))
+# Helpers for implementing anvil.server on an (optionally threaded) Real Python process.
+# Used in uplink and downlink, and now even in the PyPy sandbox.
+
+import random, string, json, re, sys, time, importlib, anvil
+
+
+# For single-threaded implementations, re-entrant calls occupy the same thread,
+# so we fake "switching a thread" by pushing all the thread-locals onto a stack
+# while we're handling an inner call
+class StackableLocal(object):
+    def _push_stack(self):
+        _nested = dict(self.__dict__)
+        self.__dict__.clear()
+        self.__dict__['_nested'] = _nested
+        self.__init__()
+
+    def _pop_stack(self):
+        nested = self._nested
+        self.__dict__.clear()
+        self.__dict__.update(nested)
+
+    def __new__(cls, *args, **kwargs):
+        v = object.__new__(cls)
+        cls.__init__(v, *args, **kwargs)
+        _stackables.append(v)
+        return v
+
+
+_stackables = []
+
+try:
+    import threading
+    ThreadLocal = threading.local
+    MULTITHREADED = True
+except:
+    MULTITHREADED = False
+    ThreadLocal = StackableLocal
+
+
+from . import  _serialise, _server
+from ._server import LazyMedia, registrations
+
+string_type = str if sys.version_info >= (3,) else basestring
+
+console_output = sys.stdout
+
+class HttpRequest(ThreadLocal):
+
+    def __init__(self):
+        self._prevent_access = True
+
+    def __getattribute__(self, name):
+        if name not in ['_push_stack', '_pop_stack', '_nested', '__dict__', '__init__'] and \
+                ThreadLocal.__getattribute__(self, "_prevent_access"):
+            raise Exception("anvil.server.request is only available in http_endpoint calls.")
+
+        return ThreadLocal.__getattribute__(self, name)
+
+    @property
+    def body_json(self):
+        if hasattr(self, "_body_json"):
+            return self._body_json
+        elif self.body is not None and self.headers.get("content-type", None) == "application/json":
+            self._body_json = json.loads(self.body.get_bytes())
+        else:
+            self._body_json = None
+        return self._body_json
+
+
+_server.api_request = HttpRequest()
+
+
+def gen_id():
+    sr = random.SystemRandom()
+    chars = string.ascii_letters + string.digits
+    return ''.join(sr.choice(chars) for _ in range(10))
+
+
+# Overwrite with functions from context
+send_reqresp = None
+
+
+class LocalCallInfo(ThreadLocal):
+    def __init__(self):
+        self.call_id = None
+        self.stack_id = None
+        self.session = None
+        self.cache_filter = {}
+        self.cache_update = {}
+        self.dump_task_state = False
+        self.enable_profiling = False
+
+    def __getitem__(self, item):
+        return self.session.__getitem__(item)
+
+    def __setitem__(self, key, value):
+        return self.session.__setitem__(key, value)
+
+    def __delitem__(self, key):
+        del self.session[key]
+
+    def get(self, key, default=None):
+        return self.session.get(key, default)
+
+    def __iter__(self):
+        return self.session.__iter__()
+
+    def __repr__(self):
+        return "<Session:%s>" % repr(self.session)
+
+
+class LocalCallContext(_server.CallContext, ThreadLocal):
+    def __init__(self):
+        self._setup(None, [])
+
+
+call_info = LocalCallInfo()
+call_context = LocalCallContext()
+call_responses = {}
+waiting_for_calls = threading.Condition() if MULTITHREADED else None
+
+
+# If MULTITHREADED is False, better overwrite this
+def poll_for_call_responses(*args):
+    raise AssertionError("We're in single-threaded mode, but poll_for_call_responses() is not set")
+
+
+backends = {}
+
+
+def _switch_session():
+    import anvil.server
+    sjson = anvil.server.call('anvil.private.switch_session!') or {"session": {}, "objects": []}
+    call_info.session = _server._reconstruct_objects(sjson, None, remote_is_trusted=True)["session"]
+
+
+default_app = anvil.app
+
+
+class LocalAppInfo(ThreadLocal):
+    def __getattr__(self, attr):
+        return getattr(default_app, attr)
+
+    def __setattr__(self, key, value):
+        raise AttributeError("This object is read-only")
+
+    def _setup(self, environment={}, **kwargs):
+        self.__dict__.update(kwargs, environment=anvil._AppInfo._Environment(**environment))
+
+
+anvil.app = LocalAppInfo()
+
+
+class SendNoResponse(Exception):
+    pass
+
+
+class IncomingRequest(_serialise.IncomingReqResp):
+    def __init__(self, json, import_modules=None, run_fn=None, dump_task_state=False, setup_task_state=None):
+        self.import_modules = import_modules
+        self.run_fn = run_fn
+        self.dump_task_state = dump_task_state
+        self.setup_task_state = setup_task_state
+        remote_is_trusted = _server.CallContext.StackFrame(json.get('call-stack', [{}])[0]).is_trusted
+        _serialise.IncomingReqResp.__init__(self, json, remote_is_trusted=remote_is_trusted)
+
+    def execute(self):
+        def make_call():
+            call_info.call_id = self.json.get('id')
+            call_info.stack_id = self.json.get('call-stack-id', None)
+            call_info.session_id = self.json.get('session-id')
+            sjson = self.json.get('sessionData', {'session': None, 'objects': []})
+            call_info.session = None
+            call_info.enable_profiling = self.json.get('enable-profiling', False)
+            if call_info.enable_profiling:
+                call_info.profile = {
+                    "origin": "Server (Python)",
+                    "description": "Python _threaded_server execution",
+                    "start-time": time.time()*1000,
+                }
+            call_info.cache_filter = _server.get_liveobject_cache_filter_spec([self.json.get('args'), self.json.get('kwargs')])
+            call_info.cache_update = {}
+            call_info.dump_task_state = self.dump_task_state
+            call_context._setup(self.json.get('client', {}), self.json.get('call-stack'))
+            anvil.app._setup(**self.json.get('app-info', {}))
+            if self.setup_task_state:
+                self.setup_task_state(call_info.call_id, True)
+            import_complete = False
+            try:
+                if self.import_modules:
+                    self.import_modules()
+                import_complete = True
+
+                # Now we've imported enough to deserialise custom types
+                self.reconstruct_remaining_data()
+                call_info.session = _server._reconstruct_objects(sjson, None, remote_is_trusted=self.remote_is_trusted).get("session", {})
+
+                if self.run_fn is not None:
+                    response = self.run_fn()
+                elif 'liveObjectCall' in self.json:
+                    loc = self.json['liveObjectCall']
+                    spec = dict(loc)
+
+                    if call_context.remote_caller is None:
+                        spec["source"] = "UNKNOWN"
+                    elif call_context.remote_caller.is_trusted:
+                        spec["source"] = "server"
+                    else:
+                        spec["source"] = "client"
+
+                    del spec["method"]
+                    backend = loc['backend']
+                    if backend not in backends:
+                        raise Exception("No such LiveObject backend: " + repr(backend))
+                    inst = backends[backend](spec)
+                    method = getattr(inst, loc['method'])
+
+                    call_info.cache_filter.setdefault(backend, set()).add(spec['id'])
+
+                    response = method(*self.json['args'], **self.json['kwargs'])
+                else:
+                    command = self.json['command']
+                    for reg in registrations:
+                        m = re.match(reg, command)
+                        if m and len(m.group(0)) == len(command):
+                            response = registrations[reg](*self.json["args"], **self.json["kwargs"])
+                            break
+                    else:
+                        if self.json.get('stale-uplink?'):
+                            raise _server.UplinkDisconnectedError({'type': 'anvil.server.UplinkDisconnectedError',
+                                                                   'message':'The uplink server for "%s" has been disconnected' % command})
+
+                        else:
+                            raise _server.NoServerFunctionError({'type': 'anvil.server.NoServerFunctionError',
+                                                                 'message': 'No server function matching "%s" has been registered' % command})
+
+                def err(*args):
+                    raise Exception("Cannot save DataMedia objects in anvil.server.session")
+
+                try:
+                    sjson = _server.fill_out_media({'session': call_info.session}, err, remote_is_trusted=True)
+                    json.dumps(sjson)
+                except TypeError as e:
+                    raise _server.SerializationError("Tried to store illegal value in a anvil.server.session. " + e.args[0])
+                except _server.SerializationError as e:
+                    raise _server.SerializationError("Tried to store illegal value in a anvil.server.session. " + e.args[0])
+
+                resp = {"id": self.json["id"], "response": response, "sessionData": sjson, "cacheUpdates": call_info.cache_update}
+
+                if call_info.enable_profiling:
+                    call_info.profile["end-time"] = time.time()*1000
+                    resp["profile"] = call_info.profile
+
+                _server.fill_out_cap_updates(resp, self.capabilities)
+
+                if self.dump_task_state:
+                    try:
+                        task_state = dict(anvil.server.task_state)
+                        tjson = _server.fill_out_media({'taskState': task_state}, err, remote_is_trusted=True)
+                        json.dumps(tjson)
+                        resp['taskState'] = task_state
+                    except (TypeError, _server.SerializationError):
+                        pass
+
+                try:
+                    send_reqresp(resp, remote_is_trusted=call_context.remote_caller.is_trusted)
+                except _server.SerializationError as e:
+                    raise _server.SerializationError("Cannot serialize return value from function. " + str(e))
+            except SendNoResponse:
+                pass
+            except:
+
+                e = _server._report_exception(self.json["id"])
+
+                if self.dump_task_state:
+                    def err(*args):
+                        raise Exception("Cannot save DataMedia objects in anvil.server.session")
+
+                    try:
+                        task_state = dict(anvil.server.task_state)
+                        tjson = _server.fill_out_media({'taskState': task_state}, err, remote_is_trusted=True)
+                        json.dumps(tjson)
+                    except (TypeError, _server.SerializationError):
+                        pass
+                    else:
+                        e['taskState'] = task_state
+
+                if not import_complete:
+                    e['moduleLoadFailed'] = True
+
+                try:
+                    send_reqresp(e)
+                except:
+                    trace = "\ncalled from ".join(["%s:%s" % (t[0], t[1]) for t in e["error"]["trace"]])
+                    console_output.write(("Failed to report exception: %s: %s\nat %s\n" % (e["error"]["type"], e["error"]["message"], trace)).encode("utf-8"))
+                    console_output.flush()
+            finally:
+                if self.setup_task_state:
+                    self.setup_task_state(call_info.call_id, False)
+                self.complete()
+
+        if MULTITHREADED:
+            threading.Thread(target=make_call).start()
+        else:
+            make_call()
+
+    def complete(self):
+        pass
+
+
+class IncomingResponse(_serialise.IncomingReqResp):
+    def __init__(self, json):
+        # Responses from the server are trusted by definition
+        _serialise.IncomingReqResp.__init__(self, json, remote_is_trusted=True)
+
+    def execute(self):
+        id = self.json['id']
+        if id in call_responses:
+            call_responses[id] = (self, self.json)
+            if MULTITHREADED:
+                with waiting_for_calls:
+                    waiting_for_calls.notifyAll()
+        else:
+            print("Got a response for an unknown ID: " + repr(self.json))
+
+
+def kill_outstanding_requests(msg):
+    for k in call_responses.keys():
+        if call_responses[k] is None:
+            call_responses[k] = (None, {'error': {'message': msg}})
+
+    if not MULTITHREADED:
+        raise Exception("_threaded_server.kill_outstanding_requests() does not work in single-threaded mode")
+
+    with waiting_for_calls:
+        waiting_for_calls.notifyAll()
+
+
+def register_live_object_backend(cls):
+
+    name = "uplink." + cls.__name__
+    backends[name] = cls
+
+    if _server.on_register is not None:
+        _server.on_register(name, True)
+
+    return cls
+
+
+live_object_backend = register_live_object_backend
+
+
+def do_call(args, kwargs, fn_name=None, live_object=None): # Yes, I do mean args and kwargs without *s
+    id = gen_id()
+
+    call_responses[id] = None
+
+    capabilities_for_update = []
+
+    if call_info.enable_profiling:
+        profile = {
+            "origin": "Server (Python)",
+            "description": "Outgoing call from Python _threaded_server",
+            "start-time": time.time()*1000
+        }
+
+    def send_call():
+        # print("Call stack ID = " + repr(_call_info.stack_id))
+        if call_info.stack_id is None:
+            call_info.stack_id = "outbound-" + gen_id()
+        req = {'type': 'CALL', 'id': id, 'args': args, 'kwargs': kwargs,
+               'call-stack-id': call_info.stack_id, 'originating-call': call_info.call_id}
+
+        if live_object:
+            req["liveObjectCall"] = { k: live_object._spec[k] for k in ["id", "backend", "mac", "permissions"] }
+            req["liveObjectCall"]["method"] = fn_name
+        elif fn_name:
+            req["command"] = fn_name
+        else:
+            raise Exception("Expected one of fn_name or live_object")
+        try:
+            # We're calling a server function and those are always trusted
+            send_reqresp(req, collect_capabilities=capabilities_for_update, remote_is_trusted=True)
+        except _server.SerializationError as e:
+            raise _server.SerializationError("Cannot serialize arguments to function. " + str(e))
+
+    if MULTITHREADED:
+        with waiting_for_calls:
+            send_call()
+            while call_responses[id] is None:
+                waiting_for_calls.wait()
+    else:
+        send_call()
+        dump_task_state = call_info.dump_task_state
+        # Fake a thread switch
+        for s in _stackables:
+            s._push_stack()
+        while call_responses[id] is None:
+            poll_for_call_responses(dump_task_state)
+            dump_task_state = False # only do it first time
+        for s in _stackables:
+            s._pop_stack()
+
+    if call_info.enable_profiling:
+        profile["end-time"] = time.time()*1000
+
+    reqresp, r = call_responses.pop(id)
+
+    # Now we're in the right thread, we can do any custom deserialisation
+    if reqresp:
+        reqresp.reconstruct_remaining_data()
+
+    if "cacheUpdates" in r:
+        # Apply updates to any of our own objects that were passed in
+        _server.apply_cache_updates(r['cacheUpdates'], [args, kwargs, live_object])
+        # Queue up whichever updates *we* should be returning
+        _server.combine_cache_updates(call_info.cache_update, r['cacheUpdates'], call_info.cache_filter)
+
+    _server.apply_cap_updates(r, capabilities_for_update)
+
+    if call_info.enable_profiling:
+        if "profile" in r:
+            profile["children"] = [r["profile"]]
+
+        if hasattr(call_info, "profile"):
+            if "children" not in call_info.profile:
+                call_info.profile["children"] = []
+
+            call_info.profile["children"].append(profile)
+
+    if 'response' in r:
+        return r['response']
+    if 'error' in r:
+        error_from_server = _server._deserialise_exception(r["error"])
+        raise error_from_server
+    else:
+        raise Exception("Bogus response from server: " + repr(r))
```

### Comparing `anvil-app-server-1.8.0/anvil_downlink_worker/anvil/email.py` & `anvil-app-server-1.9.0/anvil_downlink_worker/anvil/email.py`

 * *Files identical despite different names*

### Comparing `anvil-app-server-1.8.0/anvil_downlink_worker/anvil/files/__init__.py` & `anvil-app-server-1.9.0/anvil_downlink_worker/anvil/files/__init__.py`

 * *Files identical despite different names*

### Comparing `anvil-app-server-1.8.0/anvil_downlink_worker/anvil/google/auth.py` & `anvil-app-server-1.9.0/anvil_downlink_worker/anvil/google/auth.py`

 * *Files identical despite different names*

### Comparing `anvil-app-server-1.8.0/anvil_downlink_worker/anvil/google/drive.py` & `anvil-app-server-1.9.0/anvil_downlink_worker/anvil/google/drive.py`

 * *Files identical despite different names*

### Comparing `anvil-app-server-1.8.0/anvil_downlink_worker/anvil/google/mail.py` & `anvil-app-server-1.9.0/anvil_downlink_worker/anvil/google/mail.py`

 * *Files identical despite different names*

### Comparing `anvil-app-server-1.8.0/anvil_downlink_worker/anvil/google/sheets.py` & `anvil-app-server-1.9.0/anvil_downlink_worker/anvil/google/sheets.py`

 * *Files identical despite different names*

### Comparing `anvil-app-server-1.8.0/anvil_downlink_worker/anvil/http.py` & `anvil-app-server-1.9.0/anvil_downlink_worker/anvil/http.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,104 +1,104 @@
-import anvil.server
-
-import json as json_mod
-
-class HttpErrorStatus(Exception):
-    "Represents an HTTP error response (eg 404 Not Found)"
-    def __init__(self, status, content, message=None):
-        self.status = status
-        self.content = content
-        if message is None:
-            message = "HTTP error %s" % status
-        Exception.__init__(self, message)
-#!defAttr()!1: {name: "status", type: "number", description: "The numeric HTTP status error (eg 404 for \"not found\").\n\nStatus will be 0 for errors that prevent the request completing at all (eg cross-origin policy in the browser)."}
-#!defAttr()!1: {name: "content", pyType: "anvil.Media instance", description: "The content returned by the request (eg the body of a 404 response)"}
-#!defClass(anvil.http,HttpError)!0:
-
-
-# Backward compatibility
-HttpError = HttpErrorStatus
-
-
-class HttpRequestFailed(anvil.server.AnvilWrappedError):
-    "Represents an HTTP request that failed to complete entirely"
-    pass
-
-
-anvil.server._register_exception_type("anvil.http.HttpRequestFailed", HttpRequestFailed)
-
-def _has_content(method):
-    return method != "GET" and method != "HEAD"
-
-#!defFunction(anvil.http,_,url,[method="GET"],[data=None],[json=False],[headers=None],[username=None],[password=None],[timeout=None])!2: 
-# {
-#   $doc: "Make an HTTP request to the specified URL.",
-#   anvil$helpLink: "/docs/http-apis/making-http-requests",
-#   anvil$args: {
-#     url: "The request will be made to this URL.",
-#     method: "The HTTP method. Defaults to 'GET'.",
-#     data: "The data to send in the request body",
-#     json: "If set to True, the response is parsed into Python objects (dicts/lists/etc), and ‘data’ is JSON-encoded before sending. If False, the response will be a Media object.",
-#     headers: "A dict of strings to set HTTP headers",
-#     username: "If specified, used to perform HTTP Basic authentication",
-#     password: "If specified, used to perform HTTP Basic authentication",
-#     timeout: "An int or float representing the amount of time, in seconds, to wait for a response. Default is 60 seconds.",
-#   } 
-# }["request"]
-def request(url, method='GET', data=None, headers=None, username=None, password=None, json=False, timeout=None):
-    method = str(method).upper()
-
-    if headers is None:
-        headers = {}
-    if json and data is not None and _has_content(method):
-        data = json_mod.dumps(data)
-        headers["content-type"] = "application/json"
-    if timeout is not None:
-        if not isinstance(timeout, (int, float)):
-            raise TypeError("timeout must be a number")
-        timeout = timeout * 1000
-
-    resp = anvil.server.call(
-        "anvil.private.http.request",
-        url=url,
-        method=method,
-        data=data,
-        headers=headers,
-        username=username,
-        password=password,
-        timeout=timeout,
-    )
-    # Parse JSON if we have it
-
-    if json:
-        try:
-            b = resp["content"].get_bytes()
-            # Ew. microjson barfs if we give it a "unicode" object.
-            # We only use microjson in the old 2.7 sandbox, so
-            # this can go away soon.
-            if not isinstance(b, str):
-                b = b.decode()
-            resp["content"] = json_mod.loads(b)
-        except:
-            raise HttpError(resp["status"], resp["content"], "Invalid JSON in response")
-
-    if resp["status"] < 200 or resp["status"] > 299:
-        raise HttpError(resp["status"], resp["content"])
-
-    return resp["content"]
-
-
-#!defFunction(anvil.http,_,string_to_encode)!2: "URL-encode a string" ["url_encode"]
-def url_encode(string_to_encode):
-    return anvil.server.call("anvil.private.http.url_encode", string_to_encode)
-
-#!defFunction(anvil.http,_,string_to_encode)!2: "URL-decode a string. Raises UrlEncodingError on failure." ["url_decode"]
-def url_decode(string_to_decode):
-    return anvil.server.call("anvil.private.http.url_decode", string_to_decode)
-
-
-#!defClass(anvil.http,UrlEncodingError)!0:
-class UrlEncodingError(anvil.server.AnvilWrappedError):
-    pass
-
-
-anvil.server._register_exception_type("anvil.http.UrlEncodingError", UrlEncodingError)
+import anvil.server
+
+import json as json_mod
+
+class HttpErrorStatus(Exception):
+    "Represents an HTTP error response (eg 404 Not Found)"
+    def __init__(self, status, content, message=None):
+        self.status = status
+        self.content = content
+        if message is None:
+            message = "HTTP error %s" % status
+        Exception.__init__(self, message)
+#!defAttr()!1: {name: "status", type: "number", description: "The numeric HTTP status error (eg 404 for \"not found\").\n\nStatus will be 0 for errors that prevent the request completing at all (eg cross-origin policy in the browser)."}
+#!defAttr()!1: {name: "content", pyType: "anvil.Media instance", description: "The content returned by the request (eg the body of a 404 response)"}
+#!defClass(anvil.http,HttpError)!0:
+
+
+# Backward compatibility
+HttpError = HttpErrorStatus
+
+
+class HttpRequestFailed(anvil.server.AnvilWrappedError):
+    "Represents an HTTP request that failed to complete entirely"
+    pass
+
+
+anvil.server._register_exception_type("anvil.http.HttpRequestFailed", HttpRequestFailed)
+
+def _has_content(method):
+    return method != "GET" and method != "HEAD"
+
+#!defFunction(anvil.http,_,url,[method="GET"],[data=None],[json=False],[headers=None],[username=None],[password=None],[timeout=None])!2: 
+# {
+#   $doc: "Make an HTTP request to the specified URL.",
+#   anvil$helpLink: "/docs/http-apis/making-http-requests",
+#   anvil$args: {
+#     url: "The request will be made to this URL.",
+#     method: "The HTTP method. Defaults to 'GET'.",
+#     data: "The data to send in the request body",
+#     json: "If set to True, the response is parsed into Python objects (dicts/lists/etc), and 'data' is JSON-encoded before sending. If False, the response will be a Media object.",
+#     headers: "A dict of strings to set HTTP headers",
+#     username: "If specified, used to perform HTTP Basic authentication",
+#     password: "If specified, used to perform HTTP Basic authentication",
+#     timeout: "An int or float representing the amount of time, in seconds, to wait for a response. Default is 60 seconds.",
+#   } 
+# }["request"]
+def request(url, method='GET', data=None, headers=None, username=None, password=None, json=False, timeout=None):
+    method = str(method).upper()
+
+    if headers is None:
+        headers = {}
+    if json and data is not None and _has_content(method):
+        data = json_mod.dumps(data)
+        headers["content-type"] = "application/json"
+    if timeout is not None:
+        if not isinstance(timeout, (int, float)):
+            raise TypeError("timeout must be a number")
+        timeout = timeout * 1000
+
+    resp = anvil.server.call(
+        "anvil.private.http.request",
+        url=url,
+        method=method,
+        data=data,
+        headers=headers,
+        username=username,
+        password=password,
+        timeout=timeout,
+    )
+    # Parse JSON if we have it
+
+    if json:
+        try:
+            b = resp["content"].get_bytes()
+            # Ew. microjson barfs if we give it a "unicode" object.
+            # We only use microjson in the old 2.7 sandbox, so
+            # this can go away soon.
+            if not isinstance(b, str):
+                b = b.decode()
+            resp["content"] = json_mod.loads(b)
+        except:
+            raise HttpError(resp["status"], resp["content"], "Invalid JSON in response")
+
+    if resp["status"] < 200 or resp["status"] > 299:
+        raise HttpError(resp["status"], resp["content"])
+
+    return resp["content"]
+
+
+#!defFunction(anvil.http,_,string_to_encode)!2: "URL-encode a string" ["url_encode"]
+def url_encode(string_to_encode):
+    return anvil.server.call("anvil.private.http.url_encode", string_to_encode)
+
+#!defFunction(anvil.http,_,string_to_encode)!2: "URL-decode a string. Raises UrlEncodingError on failure." ["url_decode"]
+def url_decode(string_to_decode):
+    return anvil.server.call("anvil.private.http.url_decode", string_to_decode)
+
+
+#!defClass(anvil.http,UrlEncodingError)!0:
+class UrlEncodingError(anvil.server.AnvilWrappedError):
+    pass
+
+
+anvil.server._register_exception_type("anvil.http.UrlEncodingError", UrlEncodingError)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `anvil-app-server-1.8.0/anvil_downlink_worker/anvil/media.py` & `anvil-app-server-1.9.0/anvil_downlink_worker/anvil/media.py`

 * *Files identical despite different names*

### Comparing `anvil-app-server-1.8.0/anvil_downlink_worker/anvil/microsoft/auth.py` & `anvil-app-server-1.9.0/anvil_downlink_worker/anvil/microsoft/auth.py`

 * *Files identical despite different names*

### Comparing `anvil-app-server-1.8.0/anvil_downlink_worker/anvil/mpl_util.py` & `anvil-app-server-1.9.0/anvil_downlink_worker/anvil/mpl_util.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-import matplotlib.pyplot as plt
-import anvil
-import io
-
-
-#!defFunction(anvil.mpl_util,anvil.Media instance,[dpi=],[facecolor=],[edgecolor=],[format=],[transparent=],[frameon=],[bbox_inches=],[pad_inches=],[filename=])!2: "Return the current Matplotlib figure as an PNG image. Returns an Anvil Media object that can be displayed in Image components.\n\nOptional arguments have the same meaning as for 'savefig()'" ["plot_image"]
-def plot_image(format='png', transparent=True, filename="plot.png", **kwargs):
-  with io.BytesIO() as buf:
-    plt.savefig(buf, format=format, transparent=transparent, **kwargs)
-    buf.seek(0)    
-    return anvil.BlobMedia('image/png', buf.read(), name=filename)
+import matplotlib.pyplot as plt
+import anvil
+import io
+
+
+#!defFunction(anvil.mpl_util,anvil.Media instance,[dpi=],[facecolor=],[edgecolor=],[format=],[transparent=],[frameon=],[bbox_inches=],[pad_inches=],[filename=])!2: "Return the current Matplotlib figure as an PNG image. Returns an Anvil Media object that can be displayed in Image components.\n\nOptional arguments have the same meaning as for 'savefig()'" ["plot_image"]
+def plot_image(format='png', transparent=True, filename="plot.png", **kwargs):
+  with io.BytesIO() as buf:
+    plt.savefig(buf, format=format, transparent=transparent, **kwargs)
+    buf.seek(0)    
+    return anvil.BlobMedia('image/png', buf.read(), name=filename)
```

### Comparing `anvil-app-server-1.8.0/anvil_downlink_worker/anvil/pdf.py` & `anvil-app-server-1.9.0/anvil_downlink_worker/anvil/pdf.py`

 * *Files identical despite different names*

### Comparing `anvil-app-server-1.8.0/anvil_downlink_worker/anvil/secrets.py` & `anvil-app-server-1.9.0/anvil_downlink_worker/anvil/secrets.py`

 * *Files identical despite different names*

### Comparing `anvil-app-server-1.8.0/anvil_downlink_worker/anvil/server.py` & `anvil-app-server-1.9.0/anvil_downlink_worker/anvil/server.py`

 * *Files identical despite different names*

### Comparing `anvil-app-server-1.8.0/anvil_downlink_worker/anvil/stripe.py` & `anvil-app-server-1.9.0/anvil_downlink_worker/anvil/stripe.py`

 * *Files identical despite different names*

### Comparing `anvil-app-server-1.8.0/anvil_downlink_worker/anvil/tables/__init__.py` & `anvil-app-server-1.9.0/anvil_downlink_worker/anvil/tables/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,232 +1,255 @@
-import time
-
-import anvil.server
-
-from ._base_classes import Row, SearchIterator, Table
-from . import _config
-from ._errors import NoSuchColumnError, QuotaExceededError, RowDeleted, TableError, TransactionConflict
-from ._helpers import _hash_wrapper
-
-# Hack: Force ourselves into the top-level package, even
-# if we were loaded into a runtime-v1 per-app Anvil package
-__package__ = "anvil.tables"
-__name__ = "anvil.tables"
-
-
-# Use old app tables by default
-class AppTables(object):
-    cache = None
-
-    def __getattr__(self, name):
-        if AppTables.cache is None:
-            AppTables.cache = anvil.server.call("anvil.private.tables.get_app_tables")
-
-        tbl = AppTables.cache.get(name)
-        if tbl is not None:
-            return tbl
-
-        raise AttributeError("No such app table: '%s'" % name)
-
-    def __setattr__(self, name, val):
-        raise Exception("app_tables is read-only")
-
-_set_class = object.__dict__["__class__"].__set__
-
-def _lazy_replace_class(self):
-    if _config.get_client_config().get("enable_v2"):
-        from . import v2
-        v2._app_tables._clear_cache()
-        _set_class(self, type(v2.app_tables))
-    else:
-        AppTables.cache = None
-        _set_class(self, AppTables)
-
-
-
-def _wrap_dunder(method):
-    def wrapped(self, *args, **kws):
-        _lazy_replace_class(self)
-        return getattr(self, method)(*args, **kws)
-
-    return wrapped
-
-
-class _LazyAppTables(object):
-    def __getattribute__(self, name):
-        _lazy_replace_class(self)
-        return getattr(self, name)
-
-    __setattr__ = _wrap_dunder("__setattr__")
-    __getitem__ = _wrap_dunder("__getitem__")
-    __dir__ = _wrap_dunder("__dir__")
-
-
-class _LazyContext(object):
-    def __enter__(self):
-        global batch_update, batch_delete
-        if not _config.get_client_config().get("enable_v2"):
-            batch_update.__class__ = batch_delete.__class__ = type(None)
-            return self.__enter__()
-
-        from .v2 import _batcher as _b
-
-        for obj, orig in zip((batch_update, batch_delete), ("batch_update", "batch_delete")):
-            obj.__class__ = type(getattr(_b, orig))
-            obj.__init__()
-            setattr(_b, orig, obj)
-        return self.__enter__()
-
-    def __exit__(self, *args):
-        assert not isinstance(self, _LazyContext)
-        return self.__exit__(*args)
-
-
-def _clear_cache():
-    _config.reset_config()
-    _set_class(app_tables, _LazyAppTables)
-
-
-#!defModuleAttr(anvil.tables)!1:
-# {
-# 	name: "app_tables",
-# 	type: "any",
-# 	anvil$helpLink: "/docs/data-tables/data-tables-in-code",
-# 	$doc: "Access Table objects from the datatables services. You can access a Table object with dot notation e.g. `app_tables.my_table`. To access a table with strings use `getattr(app_tables, 'my_table')`. If no table is present an AttributeError will be thrown."
-# }
-#
-app_tables = _LazyAppTables()
-batch_update = _LazyContext()
-batch_delete = _LazyContext()
-# Not very nice but these references exist in uplink code
-# before we have a chance to know if we're using the v1/v2 config option
-# we can't call anvil.server until the uplink has made a connetion
-
-
-def get_table_by_id(table_id):
-    if _config.get_client_config().get("enable_v2"):
-        from .v2 import get_table_by_id
-
-        return get_table_by_id(table_id)
-    raise TableError("get_table_by_id is only available in Accelerated Tables beta")
-
-
-#!defModuleAttr(anvil.tables)!1:
-# {
-# 	name: "app_tables",
-# 	type: "any",
-# 	anvil$helpLink: "/docs/data-tables/data-tables-in-code",
-# 	$doc: "Access Table objects from the datatables services. You can access a Table object with dot notation e.g. `app_tables.my_table`. To access a table with strings use `getattr(app_tables, 'my_table')`. If no table is present an AttributeError will be thrown."
-# }
-#
-
-
-class Transaction:
-    def __init__(self, relaxed=False):
-        self._aborting = False
-        self._isolation = "relaxed" if relaxed else None
-
-    #!defMethod(anvil.tables.Transaction instance)!2: "Begin the transaction" ["__enter__"]
-    def __enter__(self):
-        anvil.server.call("anvil.private.tables.open_transaction", isolation=self._isolation)
-        return self
-
-    #!defMethod(_)!2: "End the transaction" ["__exit__"]
-    def __exit__(self, e_type, e_val, tb):
-        anvil.server.call("anvil.private.tables.close_transaction", self._aborting or e_val is not None)
-
-    #!defMethod(_)!2: "Abort this transaction. When it ends, all write operations performed during it will be cancelled" ["abort"]
-    def abort(self):
-        self._aborting = True
-
-
-#!defClass(anvil.tables,%Transaction)!:
-
-
-#!defFunction(anvil.tables,%,function,server_function)!2:
-# {
-# 	$doc: "When applied to a function (as a decorator), the whole function will run in a data tables transaction. If it conflicts with another transaction, it will retry up to five times.",
-# anvil$helpLink: "/docs/data-tables/transactions"
-#  } ["in_transaction"]
-def in_transaction(maybe_f=None, relaxed=None):
-    def wrap(f):
-        def new_f(*args, **kwargs):
-            n = 0
-            while True:
-                try:
-                    with Transaction(relaxed=relaxed):
-                        return f(*args, **kwargs)
-                except TransactionConflict:
-                    # lazy load random incase we make random.js a slow path on the client
-                    import random
-
-                    n += 1
-                    if n == 18:
-                        raise
-                    # print(f"RETRYING TXN {n}")
-                    # Max total sleep time is a little under 150 seconds (avg 75), so server calls will timeout before this finishes usually.
-                    sleep_amt = random.random() * (1.5**n) * 0.05
-                    try:
-                        time.sleep(sleep_amt)
-                    except:
-                        anvil.server.call("anvil.private._sleep", sleep_amt)
-
-        try:
-            reregister = f._anvil_reregister
-        except AttributeError:
-            pass
-        else:
-            reregister(new_f)
-
-        new_f.__name__ = f.__name__
-
-        return new_f
-
-    if maybe_f is None:
-        return wrap
-    else:
-        return wrap(maybe_f)
-
-
-#!defFunction(anvil.tables,_,column_name,ascending=)!2: "Sort the results of this table search by a particular column. Default to ascending order." ["order_by"]
-@anvil.server.portable_class
-class order_by(object):
-    def __init__(self, column_name, ascending=True):
-        self.column_name = column_name
-        self.ascending = ascending
-
-    __hash__, __eq__ = _hash_wrapper("column_name", "ascending")
-
-
-# backward compatability
-from .query import fetch_only
-from .query import page_size as _page_size
-
-
-#!defFunction(anvil.tables,%,[via_host=],[via_port=])!2: "Get a Postgres connection string for accessing this app's Data Tables via SQL.\n\nThe returned string includes temporary login credentials and sets the search path to a schema representing this app's Data Table environment.\n\nYou can override the host and port for the database connection to connect via a secure tunnel.\n\n(Available on the Dedicated Plan only.)" ["get_connection_string"]
-def get_connection_string(via_host=None, via_port=None):
-    return anvil.server.call(
-        "anvil.private.get_direct_postgres_connection_string", via_host=via_host, via_port=via_port
-    )
-
-
-#!defMethod(table row, **column_values)!2: "Add a row to the data table. Use keyword arguments to specify column values." ["add_row"]
-#!defMethod(client readable view)!2: "Return a view on the table that can be read by client code. Use keyword arguments to specify view restrictions" ["client_readable"]
-#!defMethod(client writable view)!2: "Return a view on the table that can be written by client code. Use keyword arguments to specify view restrictions. This does not give the client write access to other tables referred to by the table." ["client_writable"]
-#!defMethod(client writable view)!2: "Return a view on this table that can be written by client code. Use keyword arguments to specify view restrictions." ["client_writable_cascade"]
-#!defMethod(_)!2: "Delete all the rows from the data table" ["delete_all_rows"]
-#!defMethod(_)!2: "Get a single matching row from the data table whose columns match the keyword arguments. Returns None if no matching row exists, and raises an exception if more than one row matches.\n\nEg: app_tables.table_1.get(name='John Smith')" ["get"]
-#!defMethod(row,id)!2: "Get the matching row from this data table, by its unique ID" ["get_by_id"]
-#!defMethod(bool,row)!2: "Returns true if the table (or view) contains the provided row." ["has_row"]
-#!defMethod(list of dicts)!2: "Get the spec for the table as a list of dicts. Each dict contains the name and type of a column." ["list_columns"]
-#!defMethod(Row or None)!2: "Get rows from a data table. If you specify keyword arguments, you will retrieve only rows whose columns match those values.\n\nEg: app_tables.table_1.search(name='John Smith')" ["search"]
-#!defMethod(Media object, [escape_for_excel=False])!2: "Get the table in CSV format, optionally escaped for use in Excel. Returns a downloadable Media object; use its url property." ["to_csv"]
-#!defClassNoConstructor(anvil.tables,#Table)!1: "A table returned from app_tables"
-
-#!defMethod(Media object, [escape_for_excel=False])!2: "Get the results of the SearchIterator in CSV format, optionally escaped for use in Excel. Returns a downloadable Media object; use its url property." ["to_csv"]
-#!defClassNoConstructor(anvil.tables,#SearchIterator)!1: "An iterator of table rows returned from a search()";
-
-
-#!defMethod(_)!2: "Delete the row from its data table" ["delete"]
-#!defMethod(id)!2: "Get the unique ID of the table row" ["get_id"]
-#!defMethod(_,**column_values)!2: "update the data for multiple columns" ["update"]
-#!defClassNoConstructor(anvil.tables,#Row)!1: "A table row";
+import time
+
+import anvil.server
+
+from ._base_classes import Row, SearchIterator, Table
+from . import _config
+from ._errors import NoSuchColumnError, QuotaExceededError, RowDeleted, TableError, TransactionConflict
+from ._helpers import _hash_wrapper
+
+# Hack: Force ourselves into the top-level package, even
+# if we were loaded into a runtime-v1 per-app Anvil package
+__package__ = "anvil.tables"
+__name__ = "anvil.tables"
+
+
+# Use old app tables by default
+class AppTables(object):
+    cache = None
+
+    def __getattr__(self, name):
+        if AppTables.cache is None:
+            AppTables.cache = anvil.server.call("anvil.private.tables.get_app_tables")
+
+        tbl = AppTables.cache.get(name)
+        if tbl is not None:
+            return tbl
+
+        raise AttributeError("No such app table: '%s'" % name)
+
+    def __setattr__(self, name, val):
+        raise Exception("app_tables is read-only")
+    
+    def __iter__(self):
+        return AppTableIterator()
+    
+
+class AppTableIterator:
+    def __init__(self):
+        self._it = None
+
+    def __iter__(self):
+        return self
+    
+    def __next__(self):
+        # because __iter__ can't suspend
+        if AppTables.cache is None:
+            AppTables.cache = anvil.server.call("anvil.private.tables.get_app_tables")
+        if self._it is None:
+            self._it = AppTables.cache.keys().__iter__()
+        return next(self._it)
+    
+    next = __next__
+
+
+_set_class = object.__dict__["__class__"].__set__
+
+def _lazy_replace_class(self):
+    if _config.get_client_config().get("enable_v2"):
+        from . import v2
+        v2._app_tables._clear_cache()
+        _set_class(self, type(v2.app_tables))
+    else:
+        AppTables.cache = None
+        _set_class(self, AppTables)
+
+
+
+def _wrap_dunder(method):
+    def wrapped(self, *args, **kws):
+        _lazy_replace_class(self)
+        return getattr(self, method)(*args, **kws)
+
+    return wrapped
+
+
+class _LazyAppTables(object):
+    def __getattribute__(self, name):
+        _lazy_replace_class(self)
+        return getattr(self, name)
+
+    __setattr__ = _wrap_dunder("__setattr__")
+    __getitem__ = _wrap_dunder("__getitem__")
+    __dir__ = _wrap_dunder("__dir__")
+    __iter__ = AppTables.__iter__
+
+
+class _LazyContext(object):
+    def __enter__(self):
+        global batch_update, batch_delete
+        if not _config.get_client_config().get("enable_v2"):
+            batch_update.__class__ = batch_delete.__class__ = type(None)
+            return self.__enter__()
+
+        from .v2 import _batcher as _b
+
+        for obj, orig in zip((batch_update, batch_delete), ("batch_update", "batch_delete")):
+            obj.__class__ = type(getattr(_b, orig))
+            obj.__init__()
+            setattr(_b, orig, obj)
+        return self.__enter__()
+
+    def __exit__(self, *args):
+        assert not isinstance(self, _LazyContext)
+        return self.__exit__(*args)
+
+
+def _clear_cache():
+    _config.reset_config()
+    _set_class(app_tables, _LazyAppTables)
+
+
+#!defModuleAttr(anvil.tables)!1:
+# {
+# 	name: "app_tables",
+# 	type: "any",
+# 	anvil$helpLink: "/docs/data-tables/data-tables-in-code",
+# 	$doc: "Access Table objects from the datatables services. You can access a Table object with dot notation e.g. `app_tables.my_table`. To access a table with strings use `getattr(app_tables, 'my_table')`. If no table is present an AttributeError will be thrown."
+# }
+#
+app_tables = _LazyAppTables()
+batch_update = _LazyContext()
+batch_delete = _LazyContext()
+# Not very nice but these references exist in uplink code
+# before we have a chance to know if we're using the v1/v2 config option
+# we can't call anvil.server until the uplink has made a connetion
+
+
+def get_table_by_id(table_id):
+    if _config.get_client_config().get("enable_v2"):
+        from .v2 import get_table_by_id
+
+        return get_table_by_id(table_id)
+    raise TableError("get_table_by_id is only available in Accelerated Tables beta")
+
+
+#!defModuleAttr(anvil.tables)!1:
+# {
+# 	name: "app_tables",
+# 	type: "any",
+# 	anvil$helpLink: "/docs/data-tables/data-tables-in-code",
+# 	$doc: "Access Table objects from the datatables services. You can access a Table object with dot notation e.g. `app_tables.my_table`. To access a table with strings use `getattr(app_tables, 'my_table')`. If no table is present an AttributeError will be thrown."
+# }
+#
+
+
+class Transaction:
+    def __init__(self, relaxed=False):
+        self._aborting = False
+        self._isolation = "relaxed" if relaxed else None
+
+    #!defMethod(anvil.tables.Transaction instance)!2: "Begin the transaction" ["__enter__"]
+    def __enter__(self):
+        anvil.server.call("anvil.private.tables.open_transaction", isolation=self._isolation)
+        return self
+
+    #!defMethod(_)!2: "End the transaction" ["__exit__"]
+    def __exit__(self, e_type, e_val, tb):
+        anvil.server.call("anvil.private.tables.close_transaction", self._aborting or e_val is not None)
+
+    #!defMethod(_)!2: "Abort this transaction. When it ends, all write operations performed during it will be cancelled" ["abort"]
+    def abort(self):
+        self._aborting = True
+
+
+#!defClass(anvil.tables,%Transaction)!:
+
+
+#!defFunction(anvil.tables,%,function,server_function)!2:
+# {
+# 	$doc: "When applied to a function (as a decorator), the whole function will run in a data tables transaction. If it conflicts with another transaction, it will retry up to five times.",
+# anvil$helpLink: "/docs/data-tables/transactions"
+#  } ["in_transaction"]
+def in_transaction(maybe_f=None, relaxed=None):
+    def wrap(f):
+        def new_f(*args, **kwargs):
+            n = 0
+            while True:
+                try:
+                    with Transaction(relaxed=relaxed):
+                        return f(*args, **kwargs)
+                except TransactionConflict:
+                    # lazy load random incase we make random.js a slow path on the client
+                    import random
+
+                    n += 1
+                    if n == 18:
+                        raise
+                    # print(f"RETRYING TXN {n}")
+                    # Max total sleep time is a little under 150 seconds (avg 75), so server calls will timeout before this finishes usually.
+                    sleep_amt = random.random() * (1.5**n) * 0.05
+                    try:
+                        time.sleep(sleep_amt)
+                    except:
+                        anvil.server.call("anvil.private._sleep", sleep_amt)
+
+        try:
+            reregister = f._anvil_reregister
+        except AttributeError:
+            pass
+        else:
+            reregister(new_f)
+
+        new_f.__name__ = f.__name__
+
+        return new_f
+
+    if maybe_f is None:
+        return wrap
+    else:
+        return wrap(maybe_f)
+
+
+#!defFunction(anvil.tables,_,column_name,ascending=)!2: "Sort the results of this table search by a particular column. Default to ascending order." ["order_by"]
+@anvil.server.portable_class
+class order_by(object):
+    def __init__(self, column_name, ascending=True):
+        self.column_name = column_name
+        self.ascending = ascending
+
+    __hash__, __eq__ = _hash_wrapper("column_name", "ascending")
+
+
+# backward compatability
+from .query import fetch_only
+from .query import page_size as _page_size
+
+
+#!defFunction(anvil.tables,%,[via_host=],[via_port=])!2: "Get a Postgres connection string for accessing this app's Data Tables via SQL.\n\nThe returned string includes temporary login credentials and sets the search path to a schema representing this app's Data Table environment.\n\nYou can override the host and port for the database connection to connect via a secure tunnel.\n\n(Available on the Dedicated Plan only.)" ["get_connection_string"]
+def get_connection_string(via_host=None, via_port=None):
+    return anvil.server.call(
+        "anvil.private.get_direct_postgres_connection_string", via_host=via_host, via_port=via_port
+    )
+
+
+#!defMethod(table row, **column_values)!2: "Add a row to the data table. Use keyword arguments to specify column values." ["add_row"]
+#!defMethod(client readable view)!2: "Return a view on the table that can be read by client code. Use keyword arguments to specify view restrictions" ["client_readable"]
+#!defMethod(client writable view)!2: "Return a view on the table that can be written by client code. Use keyword arguments to specify view restrictions. This does not give the client write access to other tables referred to by the table." ["client_writable"]
+#!defMethod(client writable view)!2: "Return a view on this table that can be written by client code. Use keyword arguments to specify view restrictions." ["client_writable_cascade"]
+#!defMethod(_)!2: "Delete all the rows from the data table" ["delete_all_rows"]
+#!defMethod(_)!2: "Get a single matching row from the data table whose columns match the keyword arguments. Returns None if no matching row exists, and raises an exception if more than one row matches.\n\nEg: app_tables.table_1.get(name='John Smith')" ["get"]
+#!defMethod(row,id)!2: "Get the matching row from this data table, by its unique ID" ["get_by_id"]
+#!defMethod(bool,row)!2: "Returns true if the table (or view) contains the provided row." ["has_row"]
+#!defMethod(list of dicts)!2: "Get the spec for the table as a list of dicts. Each dict contains the name and type of a column." ["list_columns"]
+#!defMethod(Row or None)!2: "Get rows from a data table. If you specify keyword arguments, you will retrieve only rows whose columns match those values.\n\nEg: app_tables.table_1.search(name='John Smith')" ["search"]
+#!defMethod(Media object, [escape_for_excel=False])!2: "Get the table in CSV format, optionally escaped for use in Excel. Returns a downloadable Media object; use its url property." ["to_csv"]
+#!defClassNoConstructor(anvil.tables,#Table)!1: "A table returned from app_tables"
+
+#!defMethod(Media object, [escape_for_excel=False])!2: "Get the results of the SearchIterator in CSV format, optionally escaped for use in Excel. Returns a downloadable Media object; use its url property." ["to_csv"]
+#!defClassNoConstructor(anvil.tables,#SearchIterator)!1: "An iterator of table rows returned from a search()";
+
+
+#!defMethod(_)!2: "Delete the row from its data table" ["delete"]
+#!defMethod(id)!2: "Get the unique ID of the table row" ["get_id"]
+#!defMethod(_,**column_values)!2: "update the data for multiple columns" ["update"]
+#!defClassNoConstructor(anvil.tables,#Row)!1: "A table row";
```

### Comparing `anvil-app-server-1.8.0/anvil_downlink_worker/anvil/tables/_base_classes.py` & `anvil-app-server-1.9.0/anvil_downlink_worker/anvil/tables/_base_classes.py`

 * *Files identical despite different names*

### Comparing `anvil-app-server-1.8.0/anvil_downlink_worker/anvil/tables/_errors.py` & `anvil-app-server-1.9.0/anvil_downlink_worker/anvil/tables/_errors.py`

 * *Files identical despite different names*

### Comparing `anvil-app-server-1.8.0/anvil_downlink_worker/anvil/tables/query.py` & `anvil-app-server-1.9.0/anvil_downlink_worker/anvil/tables/query.py`

 * *Files identical despite different names*

### Comparing `anvil-app-server-1.8.0/anvil_downlink_worker/anvil/tables/v2/_batcher.py` & `anvil-app-server-1.9.0/anvil_downlink_worker/anvil/tables/v2/_batcher.py`

 * *Files identical despite different names*

### Comparing `anvil-app-server-1.8.0/anvil_downlink_worker/anvil/tables/v2/_constants.py` & `anvil-app-server-1.9.0/anvil_downlink_worker/anvil/tables/v2/_constants.py`

 * *Files identical despite different names*

### Comparing `anvil-app-server-1.8.0/anvil_downlink_worker/anvil/tables/v2/_refs.py` & `anvil-app-server-1.9.0/anvil_downlink_worker/anvil/tables/v2/_refs.py`

 * *Files identical despite different names*

### Comparing `anvil-app-server-1.8.0/anvil_downlink_worker/anvil/tables/v2/_row.py` & `anvil-app-server-1.9.0/anvil_downlink_worker/anvil/tables/v2/_row.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,518 +1,518 @@
-import anvil.server
-from anvil.server import Capability
-
-from .._base_classes import Row as BaseRow
-from .._errors import NoSuchColumnError, RowDeleted, TableError
-from . import _batcher
-from ._constants import CAP_KEY, DATETIME, MEDIA, MULTIPLE, NOT_FOUND, SERVER_PREFIX, SHARED_DATA_KEY, SINGLE, UNCACHED
-from ._utils import check_serialized, clean_local_datetime, init_spec_rows, init_view_data, merge_row_data, validate_cap
-
-PREFIX = SERVER_PREFIX + "row."
-_make_refs = None  # for circular imports
-_auto_create_is_enabled = None
-
-
-def _copy(so):
-    if type(so) is list:
-        return [_copy(o) for o in so]
-    if type(so) is dict:
-        return {k: _copy(v) for k, v in so.items()}
-    return so
-
-
-@anvil.server.portable_class
-class Row(BaseRow):
-    @classmethod
-    def _create(cls, view_key, table_id, row_id, spec=None, cap=None):
-        row = object.__new__(cls)
-        row._view_key = view_key
-        row._table_id = table_id
-        row._id = row_id
-        row._cap = cap
-        row._cache = {}
-        row._spec = spec  # None when we are deserialized without access to table_data
-        row._cache_spec = spec["cache"] if spec is not None else []
-        row._has_uncached = True
-        row._exists = True
-        row._dirty_spec = False  # used for serialization
-        if cap is not None:
-            cap.set_update_handler(row._cap_update_handler)
-        return row
-
-    @classmethod
-    def _create_from_untrusted(cls, view_key, table_id, row_id, cap, local_data):
-        # check that we can trust the data that was sent!
-        row = local_data.get(cap)
-        if row is None:
-            row = local_data[cap] = cls._create(view_key, table_id, row_id, None, cap)
-        return row
-
-    @classmethod
-    def _create_from_trusted(cls, view_key, table_id, row_id, table_data):
-        table_id, row_id = str(table_id), str(row_id)
-        view_data = table_data[view_key]
-        rows = view_data["rows"]
-        row_data = rows[row_id]
-        if isinstance(row_data, Row):
-            # prevent circular and use the created row from view_data
-            return row_data
-        spec = view_data["spec"]
-        row = rows[row_id] = cls._create(view_key, table_id, row_id, spec)
-        # Replace the compact row_data with ourself
-        # This prevents circular references and has the benefit that
-        # we create the same rows and linked rows when creating Row objects from the same data
-        row._unpack(table_data, row_data)
-        if view_data.get("dirty_spec"):
-            # a serialized row marked its spec as dirty after an update
-            row._clear_cache()
-        return row
-
-    @classmethod
-    def _create_from_local_values(cls, view_key, table_id, row_id, spec, cap, local_items):
-        # the basic idea here is that we need to clean datetime objects and UNCACHE any linked rows
-        # where the view_key doesn't match what we expect from the col_spec
-        table_id, row_id = str(table_id), str(row_id)
-        row = cls._create(view_key, table_id, row_id, spec, cap)
-        clean_items = row._walk_local_items(local_items, missing=None)
-        row._cache.update(clean_items)
-        row._check_has_cached()
-        return row
-
-    # DESERIALIZE
-    @classmethod
-    def __new_deserialized__(cls, data, info):
-        table_data, local_data = info.shared_data(SHARED_DATA_KEY)
-        view_key, table_id, row_id, cap = data
-        if not info.remote_is_trusted:
-            validate_cap(cap, view_key, table_id, row_id)
-            table_data = None  # just incase
-        if not table_data:
-            # table_data None is not enough because we may be sending rows back and forward
-            # i.e. passing from client to server to client goes untrusted -> trusted -> client
-            return cls._create_from_untrusted(view_key, table_id, row_id, cap, local_data)
-        return cls._create_from_trusted(view_key, table_id, row_id, table_data)
-
-    def _unpack(self, table_data, row_data):
-        assert type(row_data) in (list, dict), "Unable to create Row object, bad row_data"
-        spec = table_data[self._view_key]["spec"]
-        if self._spec is None:
-            self._spec = spec
-        cols = spec["cols"] if spec is not None else []
-        initial_load = not bool(self._cache)
-        row_data_type = type(row_data)
-        # if the spec is None we must have a dict data type with a single cap key
-        # this potentially happens in (and is enforced by) serialization
-        if row_data_type is list:
-            unpacked_cache, cap = self._unpack_compact(table_data, spec, cols, row_data, initial_load)
-        elif row_data_type is dict:
-            unpacked_cache, cap = self._unpack_dict(table_data, cols, row_data, initial_load)
-        else:
-            raise TableError("the row data is invalid")
-
-        assert type(cap) is Capability, "invalid row_data"
-        if self._cap is None:
-            self._cap = cap
-            cap.set_update_handler(self._cap_update_handler)
-        self._cache.update(unpacked_cache)
-        self._check_has_cached()
-
-    def _unpack_compact(self, table_data, spec, cols, row_data, initial_load):
-        # spec["cache"] 1s matches the len(row_data) (+cap)
-        iter_row_data = iter(row_data)
-        unpacked_cache = {}
-        for col, is_cached in zip(cols, spec["cache"]):
-            if is_cached:
-                val = self._unpack_linked(next(iter_row_data), col, table_data)
-            elif initial_load:
-                val = UNCACHED  # there's nothing there yet so fill it
-            else:
-                continue
-            unpacked_cache[col["name"]] = val
-        return unpacked_cache, next(iter_row_data)
-
-    def _unpack_dict(self, table_data, cols, row_data, initial_load):
-        unpacked_cache = {}
-        for i, col in enumerate(cols):
-            val = row_data.pop(str(i), UNCACHED)
-            if val is UNCACHED and not initial_load:
-                # does this ever happen?
-                continue
-            unpacked_cache[col["name"]] = self._unpack_linked(val, col, table_data)
-        cap = row_data.pop(CAP_KEY, None)
-        assert len(row_data) == 0, "Invalid row data"
-        return unpacked_cache, cap
-
-    def _unpack_linked(self, val, col, table_data):
-        table_id = col.get("table_id")
-        if table_id is None or val is UNCACHED or val is None:
-            # not a linked row, or UNCACHED linked row (serialize cache dispute), or linked row is None
-            return val
-        col_type, view_key = col["type"], col["view_key"]
-        if col_type == SINGLE:
-            row_id = val
-            return Row._create_from_trusted(view_key, table_id, row_id, table_data)
-        elif col_type == MULTIPLE:
-            row_ids = val
-            return [Row._create_from_trusted(view_key, table_id, row_id, table_data) for row_id in row_ids]
-
-        raise AssertionError("bad col type with table_id")
-
-    # SERIALIZATION
-    def __serialize__(self, info):
-        table_data, local_data = info.shared_data(SHARED_DATA_KEY)
-        if table_data is not None and info.local_is_trusted:
-            self._merge_and_reduce(table_data, local_data)
-        return [self._view_key, self._table_id, self._id, self._cap]
-
-    def _merge_linked(self, val, col, g_table_data, local_data):
-        type = col["type"]
-        if val is UNCACHED or val is None:
-            # maybe we were serialized and converted linked row(s) to UNCACHED
-            # or actually the linked row is None
-            pass
-        elif type == SINGLE:
-            row = val
-            val = row._merge_and_reduce(g_table_data, local_data)
-        elif type == MULTIPLE:
-            val = [row._merge_and_reduce(g_table_data, local_data) for row in val]
-        return val
-
-    def _make_row_data(self, g_table_data, local_data, cache_spec):
-        table_spec = self._spec
-        table_cols = table_spec["cols"] if table_spec is not None else []
-        cache = self._cache
-        # we can't rely on the order of cache in python 2
-        cached_data = []
-        for i, (col, is_cached) in enumerate(zip(table_cols, cache_spec)):
-            if not is_cached:
-                continue
-            name = col["name"]
-            val = self._merge_linked(cache[name], col, g_table_data, local_data)
-            cached_data.append((i, val))
-        cached_data.append((CAP_KEY, self._cap))
-        return cached_data
-
-    def _merge_and_reduce(self, g_table_data, local_data):
-        if check_serialized(self, local_data):
-            return int(self._id)
-        g_view_data = init_view_data(self._view_key, g_table_data)
-        table_spec, row_id, cache_spec = self._spec, self._id, self._cache_spec
-
-        # We assert that there is no way for rows from the same view_key to have different col_specs
-        # This includes the order
-        # the only thing they may differ on is cache_specs
-        g_table_spec, g_table_rows = init_spec_rows(g_view_data, table_spec, cache_spec)
-        g_cache_spec = g_table_spec["cache"] if g_table_spec is not None else None
-
-        if table_spec is not None and g_cache_spec is not None:
-            is_dirty = self._dirty_spec or len(cache_spec) != len(g_cache_spec)
-        else:
-            is_dirty = self._dirty_spec
-
-        if is_dirty:
-            g_view_data["dirty_spec"] = True
-            cache_spec = []
-
-        cached_data = self._make_row_data(g_table_data, local_data, cache_spec)
-        existing = g_table_rows.get(row_id, [])
-
-        if not is_dirty and cache_spec == g_cache_spec and type(existing) is list:
-            row_data = [val for _, val in cached_data]
-        else:
-            row_data = {str(key): val for key, val in cached_data}
-
-        merge_row_data(row_id, row_data, g_table_rows, g_table_spec, cache_spec)
-        return int(row_id)
-
-    # PRIVATE METHODS
-    def _cap_update_handler(self, updates):
-        if updates is False:
-            # We've been deleted clear_cache so that
-            # server calls are required for data access
-            self._clear_cache()
-            self._exists = False
-            return
-        elif self._spec is None:
-            return
-        clean_items = self._walk_local_items(updates)
-        self._cache.update(clean_items)
-        self._check_has_cached()
-
-    def _check_has_cached(self):
-        if self._spec is None:
-            return
-        self._cache_spec = [int(self._cache[col["name"]] is not UNCACHED) for col in self._spec["cols"]]
-        self._has_uncached = any(val is UNCACHED for val in self._cache.values())
-
-    def _clear_cache(self):
-        # clearing the cache also clears the spec - this forces a call to the server to update a spec
-        self._spec = None
-        self._cache.clear()
-        self._cache_spec = []
-        self._has_uncached = True
-
-    def _fill_cache(self, fetch=None):
-        if fetch is not None:
-            uncached_keys = None if fetch is True else fetch
-        elif self._spec is None:
-            uncached_keys = None
-        elif self._has_uncached:
-            uncached_keys = [key for key, val in self._cache.items() if val is UNCACHED]
-        else:
-            return  # no uncached values
-
-        table_data = anvil.server.call(PREFIX + "fetch", self._cap, uncached_keys)
-        rows = table_data[self._view_key]["rows"]
-        row_data = rows[self._id]
-        # Replace the compact row data with this Row instance
-        # so circular references don't clobber the data while we're unpacking.
-        rows[self._id] = self
-        self._unpack(table_data, row_data)
-
-    def _walk_local_items(self, items, missing=NOT_FOUND):
-        # We are about to put local items in the cache
-        # so check linked rows have valid view keys datetimes have tz.offset applied
-        items = items.copy()
-        rv = {}
-        cols = self._spec["cols"]
-        for col in cols:
-            name, type = col["name"], col["type"]
-            val = items.pop(name, missing)
-            if val is NOT_FOUND:
-                continue
-            else:
-                rv[name] = _copy(val)
-            if val is UNCACHED or val is None:
-                continue
-            elif type == DATETIME:
-                rv[name] = clean_local_datetime(val)
-                continue
-            elif type == MEDIA:
-                rv[name] = UNCACHED  # we need to fetch a lazy media with a valid url
-                continue
-            elif type == SINGLE:
-                val = [val]
-            elif type != MULTIPLE:
-                continue
-            rows = val
-            expected_view_key = col["view_key"]
-            if any(row._view_key != expected_view_key for row in rows):
-                rv[name] = UNCACHED
-        if len(items):
-            # more items than we should have - our col spec is no good anymore
-            self._dirty_spec = True
-            rv.update(items)
-        return rv
-
-    def _check_exists(self):
-        # only call this if we're not doing a server call
-        if not self._exists:
-            raise RowDeleted("This row has been deleted")
-
-    # DUNDER METHODS
-    def __iter__(self):
-        # call to __iter__ can't suspend
-        # so only do suspension stuff in __next__
-        # note that this will not get called for dict(row)
-        # keys() and __getitem__ wins for a call to dict
-        return RowIterator(self)
-
-    def __contains__(self, key):
-        return key in self.keys()
-
-    def __getitem__(self, key):
-        if not isinstance(key, str):
-            raise TypeError("Row columns are always strings, not {}".format(type(key).__name__))
-        if _batcher.batch_update.active:
-            rv = _batcher.batch_update.read(self._cap, key)
-            if key is not NOT_FOUND:
-                return _copy(rv)
-        if self._spec is None:
-            self._fill_cache()
-        hit = self._cache.get(key, NOT_FOUND)
-        if hit is UNCACHED:
-            # we have a spec now so we'll fetch the remaining columns
-            self._fill_cache()
-        elif hit is NOT_FOUND:
-            global _auto_create_is_enabled
-            if _auto_create_is_enabled is None:
-                _auto_create_is_enabled = anvil.server.call(PREFIX + "can_auto_create")
-            if _auto_create_is_enabled:
-                # try to force fetch this key - incase we have a bad spec - i.e auto-columns
-                self._fill_cache([key])
-        else:
-            return _copy(hit)
-        try:
-            return _copy(self._cache[key])
-        except KeyError:
-            raise NoSuchColumnError("No such column '" + key + "'")
-
-    def __setitem__(self, key, value):
-        return self.update(**{key: value})
-
-    def __eq__(self, other):
-        if not isinstance(other, Row):
-            return NotImplemented
-        return other._id == self._id and other._table_id == self._table_id
-
-    def __hash__(self):
-        self._check_exists()
-        return hash((self._table_id, self._id))
-
-    def __repr__(self):
-        if self._spec is None:
-            return "<anvil.tables.Row object>"
-
-        # custom reprs depending on type
-        trunc_str = lambda s: repr(s) if len(s) < 20 else repr(s[:17] + "...")
-        dt_repr = lambda d: "datetime(" + str(d) + ")"
-        d_repr = lambda d: "date(" + str(d) + ")"
-        printable_types = {"string": trunc_str, "bool": repr, "date": d_repr, "datetime": dt_repr, "number": repr}
-
-        # Find cols that are both cached and easily printed
-        cache, cols = self._cache, self._spec["cols"]
-        cached_printable_cols = [
-            (c["name"], printable_types[c["type"]], cache[c["name"]])
-            for c in cols
-            if c["type"] in printable_types and cache[c["name"]] is not UNCACHED
-        ]
-        # Only keep the first 5
-        cached_printable_cols = cached_printable_cols[:5]
-        # Find all the remaining columns
-        num_remaning = len(cols) - len(cached_printable_cols)
-
-        vals = ", ".join(
-            "{}={}".format(name, None if val is None else meth(val)) for name, meth, val in cached_printable_cols
-        )
-
-        if not num_remaning:
-            and_more = ""
-        elif cached_printable_cols:
-            and_more = ", plus {} more column{}".format(num_remaning, "s" if num_remaning != 1 else "")
-        else:
-            and_more = "{} column{}".format(num_remaning, "s" if num_remaning != 1 else "")
-
-        return "<anvil.tables.Row: {}{}>".format(vals, and_more)
-
-    # PUBLIC API
-    # deprecated
-    def get_id(self):
-        # For compatibility with LiveObjects
-        self._check_exists()
-        return "[{},{}]".format(self._table_id, self._id)
-
-    # TODO reinclude this api
-    # @property
-    # def id(self):
-    #     return self._id
-
-    # TODO reinclude this api
-    # @property
-    # def table_id(self):
-    #     return self._table_id
-
-    def get(self, key, default=None):
-        try:
-            return self[key]
-        except NoSuchColumnError:
-            return default
-
-
-    def keys(self):
-        if self._spec is None:
-            # if we don't have a _spec we don't have any keys
-            # but we don't need to blindly call _fill_uncached: UNCACHED values are fine
-            self._fill_cache()
-        return self._cache.keys()
-
-    def _get_view(self):
-        self._fill_cache()
-        view = _copy(self._cache)
-        if _batcher.batch_update.active:
-            batched = _batcher.batch_update.get_updates(self._cap)
-            view.update(_copy(batched))
-        return view
-
-    def items(self):
-        return self._get_view().items()
-
-    def values(self):
-        return self._get_view().values()
-
-    def update(*args, **new_items):
-        # avoid name conflicts with columns, could use (self, other, /, **kws)
-        # but positioin only args not available in py2/Skulpt
-        if not args:
-            raise TypeError("method 'update' of 'Row' object needs an argument")
-        elif len(args) > 2:
-            raise TypeError("expected at most 1 argument, got %d" % (len(args) - 1))
-        elif len(args) == 2:
-            new_items = dict(args[1], **new_items)
-        self = args[0]
-        if not new_items:
-            # backwards compatability hack
-            self._clear_cache()
-            return
-
-        # circular reference
-        if _batcher.batch_update.active:
-            return _batcher.batch_update.push(self._cap, new_items)
-
-        global _make_refs
-        if _make_refs is None:
-            from ._refs import make_refs  # circular import
-
-            _make_refs = make_refs
-
-        anvil.server.call(PREFIX + "update", self._cap, _make_refs(new_items))
-        self._cap.send_update(new_items)
-
-    def delete(self):
-        if _batcher.batch_delete.active:
-            return _batcher.batch_delete.push(self._cap)
-
-        anvil.server.call(PREFIX + "delete", self._cap)
-        self._cap.send_update(False)
-
-    def refresh(self, fetch=None):
-        if fetch is not None:
-            from ..query import fetch_only
-
-            if not isinstance(fetch, fetch_only):
-                raise TypeError("the second argument to refresh should be a q.fetch_only() object")
-            fetch = fetch.spec
-        self._clear_cache()
-        self._fill_cache(fetch)
-
-
-class RowIterator:
-    def __init__(self, row):
-        self._row = row
-        self._fill_required = row._spec is None
-        self._iter = iter(row._cache.items())
-
-    def __iter__(self):
-        return self
-
-    def __next__(self):
-        if self._fill_required:
-            self._row._fill_cache()
-            self.__init__(self._row)
-
-        key, value = next(self._iter)
-        if value is UNCACHED:
-            # fill the rest of the cache
-            # since we probably want all the items!
-            # we rely here on the _cache keys not changing during iteration
-            # which works since we've filled it with UNCACHED values that match our expected keys
-            self._row._fill_cache()
-            value = self._row._cache[key]
-
-        if _batcher.batch_update.active:
-            batched = _batcher.batch_update.read(self._row._cap, key)
-            if batched is not NOT_FOUND:
-                value = batched
-
-        return (key, _copy(value))
-
-    next = __next__
+import anvil.server
+from anvil.server import Capability
+
+from .._base_classes import Row as BaseRow
+from .._errors import NoSuchColumnError, RowDeleted, TableError
+from . import _batcher
+from ._constants import CAP_KEY, DATETIME, MEDIA, MULTIPLE, NOT_FOUND, SERVER_PREFIX, SHARED_DATA_KEY, SINGLE, UNCACHED
+from ._utils import check_serialized, clean_local_datetime, init_spec_rows, init_view_data, merge_row_data, validate_cap
+
+PREFIX = SERVER_PREFIX + "row."
+_make_refs = None  # for circular imports
+_auto_create_is_enabled = None
+
+
+def _copy(so):
+    if type(so) is list:
+        return [_copy(o) for o in so]
+    if type(so) is dict:
+        return {k: _copy(v) for k, v in so.items()}
+    return so
+
+
+@anvil.server.portable_class
+class Row(BaseRow):
+    @classmethod
+    def _create(cls, view_key, table_id, row_id, spec=None, cap=None):
+        row = object.__new__(cls)
+        row._view_key = view_key
+        row._table_id = table_id
+        row._id = row_id
+        row._cap = cap
+        row._cache = {}
+        row._spec = spec  # None when we are deserialized without access to table_data
+        row._cache_spec = spec["cache"] if spec is not None else []
+        row._has_uncached = True
+        row._exists = True
+        row._dirty_spec = False  # used for serialization
+        if cap is not None:
+            cap.set_update_handler(row._cap_update_handler)
+        return row
+
+    @classmethod
+    def _create_from_untrusted(cls, view_key, table_id, row_id, cap, local_data):
+        # check that we can trust the data that was sent!
+        row = local_data.get(cap)
+        if row is None:
+            row = local_data[cap] = cls._create(view_key, table_id, row_id, None, cap)
+        return row
+
+    @classmethod
+    def _create_from_trusted(cls, view_key, table_id, row_id, table_data):
+        table_id, row_id = str(table_id), str(row_id)
+        view_data = table_data[view_key]
+        rows = view_data["rows"]
+        row_data = rows[row_id]
+        if isinstance(row_data, Row):
+            # prevent circular and use the created row from view_data
+            return row_data
+        spec = view_data["spec"]
+        row = rows[row_id] = cls._create(view_key, table_id, row_id, spec)
+        # Replace the compact row_data with ourself
+        # This prevents circular references and has the benefit that
+        # we create the same rows and linked rows when creating Row objects from the same data
+        row._unpack(table_data, row_data)
+        if view_data.get("dirty_spec"):
+            # a serialized row marked its spec as dirty after an update
+            row._clear_cache()
+        return row
+
+    @classmethod
+    def _create_from_local_values(cls, view_key, table_id, row_id, spec, cap, local_items):
+        # the basic idea here is that we need to clean datetime objects and UNCACHE any linked rows
+        # where the view_key doesn't match what we expect from the col_spec
+        table_id, row_id = str(table_id), str(row_id)
+        row = cls._create(view_key, table_id, row_id, spec, cap)
+        clean_items = row._walk_local_items(local_items, missing=None)
+        row._cache.update(clean_items)
+        row._check_has_cached()
+        return row
+
+    # DESERIALIZE
+    @classmethod
+    def __new_deserialized__(cls, data, info):
+        table_data, local_data = info.shared_data(SHARED_DATA_KEY)
+        view_key, table_id, row_id, cap = data
+        if not info.remote_is_trusted:
+            validate_cap(cap, view_key, table_id, row_id)
+            table_data = None  # just incase
+        if not table_data:
+            # table_data None is not enough because we may be sending rows back and forward
+            # i.e. passing from client to server to client goes untrusted -> trusted -> client
+            return cls._create_from_untrusted(view_key, table_id, row_id, cap, local_data)
+        return cls._create_from_trusted(view_key, table_id, row_id, table_data)
+
+    def _unpack(self, table_data, row_data):
+        assert type(row_data) in (list, dict), "Unable to create Row object, bad row_data"
+        spec = table_data[self._view_key]["spec"]
+        if self._spec is None:
+            self._spec = spec
+        cols = spec["cols"] if spec is not None else []
+        initial_load = not bool(self._cache)
+        row_data_type = type(row_data)
+        # if the spec is None we must have a dict data type with a single cap key
+        # this potentially happens in (and is enforced by) serialization
+        if row_data_type is list:
+            unpacked_cache, cap = self._unpack_compact(table_data, spec, cols, row_data, initial_load)
+        elif row_data_type is dict:
+            unpacked_cache, cap = self._unpack_dict(table_data, cols, row_data, initial_load)
+        else:
+            raise TableError("the row data is invalid")
+
+        assert type(cap) is Capability, "invalid row_data"
+        if self._cap is None:
+            self._cap = cap
+            cap.set_update_handler(self._cap_update_handler)
+        self._cache.update(unpacked_cache)
+        self._check_has_cached()
+
+    def _unpack_compact(self, table_data, spec, cols, row_data, initial_load):
+        # spec["cache"] 1s matches the len(row_data) (+cap)
+        iter_row_data = iter(row_data)
+        unpacked_cache = {}
+        for col, is_cached in zip(cols, spec["cache"]):
+            if is_cached:
+                val = self._unpack_linked(next(iter_row_data), col, table_data)
+            elif initial_load:
+                val = UNCACHED  # there's nothing there yet so fill it
+            else:
+                continue
+            unpacked_cache[col["name"]] = val
+        return unpacked_cache, next(iter_row_data)
+
+    def _unpack_dict(self, table_data, cols, row_data, initial_load):
+        unpacked_cache = {}
+        for i, col in enumerate(cols):
+            val = row_data.pop(str(i), UNCACHED)
+            if val is UNCACHED and not initial_load:
+                # does this ever happen?
+                continue
+            unpacked_cache[col["name"]] = self._unpack_linked(val, col, table_data)
+        cap = row_data.pop(CAP_KEY, None)
+        assert len(row_data) == 0, "Invalid row data"
+        return unpacked_cache, cap
+
+    def _unpack_linked(self, val, col, table_data):
+        table_id = col.get("table_id")
+        if table_id is None or val is UNCACHED or val is None:
+            # not a linked row, or UNCACHED linked row (serialize cache dispute), or linked row is None
+            return val
+        col_type, view_key = col["type"], col["view_key"]
+        if col_type == SINGLE:
+            row_id = val
+            return Row._create_from_trusted(view_key, table_id, row_id, table_data)
+        elif col_type == MULTIPLE:
+            row_ids = val
+            return [Row._create_from_trusted(view_key, table_id, row_id, table_data) for row_id in row_ids]
+
+        raise AssertionError("bad col type with table_id")
+
+    # SERIALIZATION
+    def __serialize__(self, info):
+        table_data, local_data = info.shared_data(SHARED_DATA_KEY)
+        if table_data is not None and info.local_is_trusted:
+            self._merge_and_reduce(table_data, local_data)
+        return [self._view_key, self._table_id, self._id, self._cap]
+
+    def _merge_linked(self, val, col, g_table_data, local_data):
+        type = col["type"]
+        if val is UNCACHED or val is None:
+            # maybe we were serialized and converted linked row(s) to UNCACHED
+            # or actually the linked row is None
+            pass
+        elif type == SINGLE:
+            row = val
+            val = row._merge_and_reduce(g_table_data, local_data)
+        elif type == MULTIPLE:
+            val = [row._merge_and_reduce(g_table_data, local_data) for row in val]
+        return val
+
+    def _make_row_data(self, g_table_data, local_data, cache_spec):
+        table_spec = self._spec
+        table_cols = table_spec["cols"] if table_spec is not None else []
+        cache = self._cache
+        # we can't rely on the order of cache in python 2
+        cached_data = []
+        for i, (col, is_cached) in enumerate(zip(table_cols, cache_spec)):
+            if not is_cached:
+                continue
+            name = col["name"]
+            val = self._merge_linked(cache[name], col, g_table_data, local_data)
+            cached_data.append((i, val))
+        cached_data.append((CAP_KEY, self._cap))
+        return cached_data
+
+    def _merge_and_reduce(self, g_table_data, local_data):
+        if check_serialized(self, local_data):
+            return int(self._id)
+        g_view_data = init_view_data(self._view_key, g_table_data)
+        table_spec, row_id, cache_spec = self._spec, self._id, self._cache_spec
+
+        # We assert that there is no way for rows from the same view_key to have different col_specs
+        # This includes the order
+        # the only thing they may differ on is cache_specs
+        g_table_spec, g_table_rows = init_spec_rows(g_view_data, table_spec, cache_spec)
+        g_cache_spec = g_table_spec["cache"] if g_table_spec is not None else None
+
+        if table_spec is not None and g_cache_spec is not None:
+            is_dirty = self._dirty_spec or len(cache_spec) != len(g_cache_spec)
+        else:
+            is_dirty = self._dirty_spec
+
+        if is_dirty:
+            g_view_data["dirty_spec"] = True
+            cache_spec = []
+
+        cached_data = self._make_row_data(g_table_data, local_data, cache_spec)
+        existing = g_table_rows.get(row_id, [])
+
+        if not is_dirty and cache_spec == g_cache_spec and type(existing) is list:
+            row_data = [val for _, val in cached_data]
+        else:
+            row_data = {str(key): val for key, val in cached_data}
+
+        merge_row_data(row_id, row_data, g_table_rows, g_table_spec, cache_spec)
+        return int(row_id)
+
+    # PRIVATE METHODS
+    def _cap_update_handler(self, updates):
+        if updates is False:
+            # We've been deleted clear_cache so that
+            # server calls are required for data access
+            self._clear_cache()
+            self._exists = False
+            return
+        elif self._spec is None:
+            return
+        clean_items = self._walk_local_items(updates)
+        self._cache.update(clean_items)
+        self._check_has_cached()
+
+    def _check_has_cached(self):
+        if self._spec is None:
+            return
+        self._cache_spec = [int(self._cache[col["name"]] is not UNCACHED) for col in self._spec["cols"]]
+        self._has_uncached = any(val is UNCACHED for val in self._cache.values())
+
+    def _clear_cache(self):
+        # clearing the cache also clears the spec - this forces a call to the server to update a spec
+        self._spec = None
+        self._cache.clear()
+        self._cache_spec = []
+        self._has_uncached = True
+
+    def _fill_cache(self, fetch=None):
+        if fetch is not None:
+            uncached_keys = None if fetch is True else fetch
+        elif self._spec is None:
+            uncached_keys = None
+        elif self._has_uncached:
+            uncached_keys = [key for key, val in self._cache.items() if val is UNCACHED]
+        else:
+            return  # no uncached values
+
+        table_data = anvil.server.call(PREFIX + "fetch", self._cap, uncached_keys)
+        rows = table_data[self._view_key]["rows"]
+        row_data = rows[self._id]
+        # Replace the compact row data with this Row instance
+        # so circular references don't clobber the data while we're unpacking.
+        rows[self._id] = self
+        self._unpack(table_data, row_data)
+
+    def _walk_local_items(self, items, missing=NOT_FOUND):
+        # We are about to put local items in the cache
+        # so check linked rows have valid view keys datetimes have tz.offset applied
+        items = items.copy()
+        rv = {}
+        cols = self._spec["cols"]
+        for col in cols:
+            name, type = col["name"], col["type"]
+            val = items.pop(name, missing)
+            if val is NOT_FOUND:
+                continue
+            else:
+                rv[name] = _copy(val)
+            if val is UNCACHED or val is None:
+                continue
+            elif type == DATETIME:
+                rv[name] = clean_local_datetime(val)
+                continue
+            elif type == MEDIA:
+                rv[name] = UNCACHED  # we need to fetch a lazy media with a valid url
+                continue
+            elif type == SINGLE:
+                val = [val]
+            elif type != MULTIPLE:
+                continue
+            rows = val
+            expected_view_key = col["view_key"]
+            if any(row._view_key != expected_view_key for row in rows):
+                rv[name] = UNCACHED
+        if len(items):
+            # more items than we should have - our col spec is no good anymore
+            self._dirty_spec = True
+            rv.update(items)
+        return rv
+
+    def _check_exists(self):
+        # only call this if we're not doing a server call
+        if not self._exists:
+            raise RowDeleted("This row has been deleted")
+
+    # DUNDER METHODS
+    def __iter__(self):
+        # call to __iter__ can't suspend
+        # so only do suspension stuff in __next__
+        # note that this will not get called for dict(row)
+        # keys() and __getitem__ wins for a call to dict
+        return RowIterator(self)
+
+    def __contains__(self, key):
+        return key in self.keys()
+
+    def __getitem__(self, key):
+        if not isinstance(key, str):
+            raise TypeError("Row columns are always strings, not {}".format(type(key).__name__))
+        if _batcher.batch_update.active:
+            rv = _batcher.batch_update.read(self._cap, key)
+            if key is not NOT_FOUND:
+                return _copy(rv)
+        if self._spec is None:
+            self._fill_cache()
+        hit = self._cache.get(key, NOT_FOUND)
+        if hit is UNCACHED:
+            # we have a spec now so we'll fetch the remaining columns
+            self._fill_cache()
+        elif hit is NOT_FOUND:
+            global _auto_create_is_enabled
+            if _auto_create_is_enabled is None:
+                _auto_create_is_enabled = anvil.server.call(PREFIX + "can_auto_create")
+            if _auto_create_is_enabled:
+                # try to force fetch this key - incase we have a bad spec - i.e auto-columns
+                self._fill_cache([key])
+        else:
+            return _copy(hit)
+        try:
+            return _copy(self._cache[key])
+        except KeyError:
+            raise NoSuchColumnError("No such column '" + key + "'")
+
+    def __setitem__(self, key, value):
+        return self.update(**{key: value})
+
+    def __eq__(self, other):
+        if not isinstance(other, Row):
+            return NotImplemented
+        return other._id == self._id and other._table_id == self._table_id
+
+    def __hash__(self):
+        self._check_exists()
+        return hash((self._table_id, self._id))
+
+    def __repr__(self):
+        if self._spec is None:
+            return "<anvil.tables.Row object>"
+
+        # custom reprs depending on type
+        trunc_str = lambda s: repr(s) if len(s) < 20 else repr(s[:17] + "...")
+        dt_repr = lambda d: "datetime(" + str(d) + ")"
+        d_repr = lambda d: "date(" + str(d) + ")"
+        printable_types = {"string": trunc_str, "bool": repr, "date": d_repr, "datetime": dt_repr, "number": repr}
+
+        # Find cols that are both cached and easily printed
+        cache, cols = self._cache, self._spec["cols"]
+        cached_printable_cols = [
+            (c["name"], printable_types[c["type"]], cache[c["name"]])
+            for c in cols
+            if c["type"] in printable_types and cache[c["name"]] is not UNCACHED
+        ]
+        # Only keep the first 5
+        cached_printable_cols = cached_printable_cols[:5]
+        # Find all the remaining columns
+        num_remaning = len(cols) - len(cached_printable_cols)
+
+        vals = ", ".join(
+            "{}={}".format(name, None if val is None else meth(val)) for name, meth, val in cached_printable_cols
+        )
+
+        if not num_remaning:
+            and_more = ""
+        elif cached_printable_cols:
+            and_more = ", plus {} more column{}".format(num_remaning, "s" if num_remaning != 1 else "")
+        else:
+            and_more = "{} column{}".format(num_remaning, "s" if num_remaning != 1 else "")
+
+        return "<anvil.tables.Row: {}{}>".format(vals, and_more)
+
+    # PUBLIC API
+    # deprecated
+    def get_id(self):
+        # For compatibility with LiveObjects
+        self._check_exists()
+        return "[{},{}]".format(self._table_id, self._id)
+
+    # TODO reinclude this api
+    # @property
+    # def id(self):
+    #     return self._id
+
+    # TODO reinclude this api
+    # @property
+    # def table_id(self):
+    #     return self._table_id
+
+    def get(self, key, default=None):
+        try:
+            return self[key]
+        except NoSuchColumnError:
+            return default
+
+
+    def keys(self):
+        if self._spec is None:
+            # if we don't have a _spec we don't have any keys
+            # but we don't need to blindly call _fill_uncached: UNCACHED values are fine
+            self._fill_cache()
+        return self._cache.keys()
+
+    def _get_view(self):
+        self._fill_cache()
+        view = _copy(self._cache)
+        if _batcher.batch_update.active:
+            batched = _batcher.batch_update.get_updates(self._cap)
+            view.update(_copy(batched))
+        return view
+
+    def items(self):
+        return self._get_view().items()
+
+    def values(self):
+        return self._get_view().values()
+
+    def update(*args, **new_items):
+        # avoid name conflicts with columns, could use (self, other, /, **kws)
+        # but positioin only args not available in py2/Skulpt
+        if not args:
+            raise TypeError("method 'update' of 'Row' object needs an argument")
+        elif len(args) > 2:
+            raise TypeError("expected at most 1 argument, got %d" % (len(args) - 1))
+        elif len(args) == 2:
+            new_items = dict(args[1], **new_items)
+        self = args[0]
+        if not new_items:
+            # backwards compatability hack
+            self._clear_cache()
+            return
+
+        # circular reference
+        if _batcher.batch_update.active:
+            return _batcher.batch_update.push(self._cap, new_items)
+
+        global _make_refs
+        if _make_refs is None:
+            from ._refs import make_refs  # circular import
+
+            _make_refs = make_refs
+
+        anvil.server.call(PREFIX + "update", self._cap, _make_refs(new_items))
+        self._cap.send_update(new_items)
+
+    def delete(self):
+        if _batcher.batch_delete.active:
+            return _batcher.batch_delete.push(self._cap)
+
+        anvil.server.call(PREFIX + "delete", self._cap)
+        self._cap.send_update(False)
+
+    def refresh(self, fetch=None):
+        if fetch is not None:
+            from ..query import fetch_only
+
+            if not isinstance(fetch, fetch_only):
+                raise TypeError("the second argument to refresh should be a q.fetch_only() object")
+            fetch = fetch.spec
+        self._clear_cache()
+        self._fill_cache(fetch)
+
+
+class RowIterator:
+    def __init__(self, row):
+        self._row = row
+        self._fill_required = row._spec is None
+        self._iter = iter(row._cache.items())
+
+    def __iter__(self):
+        return self
+
+    def __next__(self):
+        if self._fill_required:
+            self._row._fill_cache()
+            self.__init__(self._row)
+
+        key, value = next(self._iter)
+        if value is UNCACHED:
+            # fill the rest of the cache
+            # since we probably want all the items!
+            # we rely here on the _cache keys not changing during iteration
+            # which works since we've filled it with UNCACHED values that match our expected keys
+            self._row._fill_cache()
+            value = self._row._cache[key]
+
+        if _batcher.batch_update.active:
+            batched = _batcher.batch_update.read(self._row._cap, key)
+            if batched is not NOT_FOUND:
+                value = batched
+
+        return (key, _copy(value))
+
+    next = __next__
```

### Comparing `anvil-app-server-1.8.0/anvil_downlink_worker/anvil/tables/v2/_table.py` & `anvil-app-server-1.9.0/anvil_downlink_worker/anvil/tables/v2/_table.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,120 +1,120 @@
-import anvil.server
-from anvil.server import Capability
-
-from .._base_classes import Table as BaseTable
-from ._constants import CASCADE, KNOWN_PERMS, READ, SERVER_PREFIX, WRITE
-from ._refs import make_refs
-from ._row import Row
-from ._search import SearchIterator
-from ._utils import validate_cap
-
-PREFIX = SERVER_PREFIX + "table."
-
-
-@anvil.server.portable_class
-class Table(BaseTable):
-    @classmethod
-    def _create(cls, cap, view_key, table_id):
-        assert cap is None or type(cap) is Capability, "expected a table capability"
-        self = object.__new__(cls)
-        self._cap = cap
-        self._view_key = view_key
-        self._id = str(table_id)
-        return self
-
-    @classmethod
-    def __new_deserialized__(cls, data, info):
-        if not info.remote_is_trusted:
-            validate_cap(*data)
-        return cls._create(*data)
-
-    def __serialize__(self, _info):
-        return [self._cap, self._view_key, self._id]
-
-    def __iter__(self):
-        raise TypeError("You can't iterate on a table. Call search() on this table to get an iterator of rows instead.")
-
-    def __eq__(self, other):
-        if not isinstance(other, Table):
-            return NotImplemented
-        return other._id == self._id
-
-    def __hash__(self):
-        return hash(self._id)
-
-    def __contains__(self, row):
-        return self.has_row(row)
-
-    def _get_view(self, perm, args, kws):
-        assert perm in KNOWN_PERMS, "bad permission"
-        new_cap, view_key = anvil.server.call(
-            PREFIX + "get_view", self._cap, perm, None, make_refs(args), make_refs(kws)
-        )
-        return Table._create(new_cap, view_key, self._id)
-
-    # PUBLIC API
-    def restrict_columns(self, col_spec):
-        new_cap, view_key = anvil.server.call("get_restricted_columns", self._cap, col_spec)
-        return Table._create(new_cap, view_key, self._id)
-
-    def client_readable(self, *args, **kws):
-        return self._get_view(READ, args, kws)
-
-    def client_writable(self, *args, **kws):
-        return self._get_view(WRITE, args, kws)
-
-    def client_writable_cascade(self, *args, **kws):
-        return self._get_view(CASCADE, args, kws)
-
-    def delete_all_rows(self):
-        return anvil.server.call(PREFIX + "delete_all_rows", self._cap)
-
-    def add_rows(self, rows):
-        # rows can be an iterable of dicts
-        row_dicts = []
-        refs = []
-        for row in rows:
-            row = dict(row)
-            refs.append(make_refs(row))
-            row_dicts.append(row)
-        row_id_caps, spec = anvil.server.call(PREFIX + "add_rows", self._cap, refs)
-        return [
-            Row._create_from_local_values(self._view_key, self._id, row_id, spec, cap, row_items)
-            for (row_id, cap), row_items in zip(row_id_caps, row_dicts)
-        ]
-
-    def add_row(self, **data):
-        row_id, cap, spec = anvil.server.call(PREFIX + "add_row", self._cap, make_refs(data))
-        return Row._create_from_local_values(self._view_key, self._id, row_id, spec, cap, data)
-
-    def get(self, *args, **kws):
-        row_id_table_data = anvil.server.call(PREFIX + "get_row", self._cap, make_refs(args), make_refs(kws))
-        return row_id_table_data and Row._create_from_trusted(self._view_key, self._id, *row_id_table_data)
-
-    def get_by_id(self, row_id, fetch=None):
-        row_id_table_data = anvil.server.call(PREFIX + "get_row_by_id", self._cap, row_id, fetch=fetch)
-        return row_id_table_data and Row._create_from_trusted(self._view_key, self._id, *row_id_table_data)
-
-    def has_row(self, row):
-        if not isinstance(row, Row):
-            # backwards compatability return False
-            return False
-        elif row._table_id != self._id:
-            return False
-        return anvil.server.call(PREFIX + "has_row", self._cap, row._id)
-
-    def list_columns(self):
-        return anvil.server.call(PREFIX + "list_columns", self._cap)
-
-    def search(self, *args, **kws):
-        kws = make_refs(kws)
-        row_ids, cap, cap_next, table_data = anvil.server.call(PREFIX + "search", self._cap, args, kws)
-        return SearchIterator._create(self._view_key, self._id, row_ids, cap, cap_next, table_data)
-
-    def to_csv(self, escape_for_excel=False):
-        return anvil.server.call(PREFIX + "to_csv", self._cap, escape_for_excel=escape_for_excel)
-
-    # TODO reinclude this API
-    # @property
-    # def id(self):
-    #     return self._id
+import anvil.server
+from anvil.server import Capability
+
+from .._base_classes import Table as BaseTable
+from ._constants import CASCADE, KNOWN_PERMS, READ, SERVER_PREFIX, WRITE
+from ._refs import make_refs
+from ._row import Row
+from ._search import SearchIterator
+from ._utils import validate_cap
+
+PREFIX = SERVER_PREFIX + "table."
+
+
+@anvil.server.portable_class
+class Table(BaseTable):
+    @classmethod
+    def _create(cls, cap, view_key, table_id):
+        assert cap is None or type(cap) is Capability, "expected a table capability"
+        self = object.__new__(cls)
+        self._cap = cap
+        self._view_key = view_key
+        self._id = str(table_id)
+        return self
+
+    @classmethod
+    def __new_deserialized__(cls, data, info):
+        if not info.remote_is_trusted:
+            validate_cap(*data)
+        return cls._create(*data)
+
+    def __serialize__(self, _info):
+        return [self._cap, self._view_key, self._id]
+
+    def __iter__(self):
+        raise TypeError("You can't iterate on a table. Call search() on this table to get an iterator of rows instead.")
+
+    def __eq__(self, other):
+        if not isinstance(other, Table):
+            return NotImplemented
+        return other._id == self._id
+
+    def __hash__(self):
+        return hash(self._id)
+
+    def __contains__(self, row):
+        return self.has_row(row)
+
+    def _get_view(self, perm, args, kws):
+        assert perm in KNOWN_PERMS, "bad permission"
+        new_cap, view_key = anvil.server.call(
+            PREFIX + "get_view", self._cap, perm, None, make_refs(args), make_refs(kws)
+        )
+        return Table._create(new_cap, view_key, self._id)
+
+    # PUBLIC API
+    def restrict_columns(self, col_spec):
+        new_cap, view_key = anvil.server.call("get_restricted_columns", self._cap, col_spec)
+        return Table._create(new_cap, view_key, self._id)
+
+    def client_readable(self, *args, **kws):
+        return self._get_view(READ, args, kws)
+
+    def client_writable(self, *args, **kws):
+        return self._get_view(WRITE, args, kws)
+
+    def client_writable_cascade(self, *args, **kws):
+        return self._get_view(CASCADE, args, kws)
+
+    def delete_all_rows(self):
+        return anvil.server.call(PREFIX + "delete_all_rows", self._cap)
+
+    def add_rows(self, rows):
+        # rows can be an iterable of dicts
+        row_dicts = []
+        refs = []
+        for row in rows:
+            row = dict(row)
+            refs.append(make_refs(row))
+            row_dicts.append(row)
+        row_id_caps, spec = anvil.server.call(PREFIX + "add_rows", self._cap, refs)
+        return [
+            Row._create_from_local_values(self._view_key, self._id, row_id, spec, cap, row_items)
+            for (row_id, cap), row_items in zip(row_id_caps, row_dicts)
+        ]
+
+    def add_row(self, **data):
+        row_id, cap, spec = anvil.server.call(PREFIX + "add_row", self._cap, make_refs(data))
+        return Row._create_from_local_values(self._view_key, self._id, row_id, spec, cap, data)
+
+    def get(self, *args, **kws):
+        row_id_table_data = anvil.server.call(PREFIX + "get_row", self._cap, make_refs(args), make_refs(kws))
+        return row_id_table_data and Row._create_from_trusted(self._view_key, self._id, *row_id_table_data)
+
+    def get_by_id(self, row_id, fetch=None):
+        row_id_table_data = anvil.server.call(PREFIX + "get_row_by_id", self._cap, row_id, fetch=fetch)
+        return row_id_table_data and Row._create_from_trusted(self._view_key, self._id, *row_id_table_data)
+
+    def has_row(self, row):
+        if not isinstance(row, Row):
+            # backwards compatability return False
+            return False
+        elif row._table_id != self._id:
+            return False
+        return anvil.server.call(PREFIX + "has_row", self._cap, row._id)
+
+    def list_columns(self):
+        return anvil.server.call(PREFIX + "list_columns", self._cap)
+
+    def search(self, *args, **kws):
+        kws = make_refs(kws)
+        row_ids, cap, cap_next, table_data = anvil.server.call(PREFIX + "search", self._cap, args, kws)
+        return SearchIterator._create(self._view_key, self._id, row_ids, cap, cap_next, table_data)
+
+    def to_csv(self, escape_for_excel=False):
+        return anvil.server.call(PREFIX + "to_csv", self._cap, escape_for_excel=escape_for_excel)
+
+    # TODO reinclude this API
+    # @property
+    # def id(self):
+    #     return self._id
```

### Comparing `anvil-app-server-1.8.0/anvil_downlink_worker/anvil/tables/v2/_utils.py` & `anvil-app-server-1.9.0/anvil_downlink_worker/anvil/tables/v2/_utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,135 +1,135 @@
-import anvil.tz
-from anvil.server import Capability, unwrap_capability
-
-from ._constants import CAP_KEY, NOT_FOUND, UNCACHED
-
-
-def validate_cap(cap, view_key, table_id, row_id=NOT_FOUND):
-    import json  # we don't need this on the client
-
-    _, _, view_dict, narrowed, _ = unwrap_capability(cap, ["_", "t", Capability.ANY, Capability.ANY, Capability.ANY])
-    assert view_dict == json.loads(view_key)
-    assert table_id == str(view_dict["id"])
-    if row_id is not NOT_FOUND:
-        assert row_id == str(narrowed["r"])
-
-
-def clean_local_datetime(d):
-    if d.tzinfo is not None:
-        offset = d.utcoffset().total_seconds()
-    else:
-        offset = anvil.tz.tzlocal().utcoffset(d).total_seconds()
-    return d.replace(tzinfo=anvil.tz.tzoffset(seconds=offset))
-
-
-# Serialization helpers
-def check_serialized(self, local_data):
-    self_id = id(self)
-    serialized = local_data.get(self_id, False)
-    local_data[self_id] = True
-    return serialized
-
-
-def init_view_data(view_key, g_table_data):
-    return g_table_data.setdefault(view_key, {})
-
-
-def init_spec_rows(g_view_data, table_spec, cache_spec=None):
-    g_table_spec = g_view_data.get("spec")
-    if g_table_spec is not None:
-        pass
-    elif table_spec is None or cache_spec is None:
-        g_table_spec = g_view_data["spec"] = table_spec
-    else:
-        g_table_spec = g_view_data["spec"] = {"cols": table_spec["cols"], "cache": cache_spec}
-    g_table_rows = g_view_data.setdefault("rows", {})
-    return g_table_spec, g_table_rows
-
-
-def merge_row_data(row_id, row_data, g_table_rows, g_table_spec, row_cache_spec):
-    # we've already cleaned the row_data
-    #  - it will only be a compact list if the caches match
-    #  - and g_row_data is either None or also a compact list
-    # otherwise row_data will be a dict
-    g_row_data = g_table_rows.get(row_id)
-
-    # FAST - common case - nothing in row_data
-    if g_row_data is None:
-        g_table_rows[row_id] = row_data
-        return
-
-    g_row_type = type(g_row_data)
-    row_type = type(row_data)
-
-    # handle all UNCACHED - i.e. the partially cached writer wins
-    if g_row_type is list and len(g_row_data) == 1:
-        # the row serialized before us has an all 0 cache_spec and is compact
-        # we are either a dict or a list of the same length
-        g_table_rows[row_id] = row_data
-        return
-    if not any(row_cache_spec):
-        # the row to merge has an all 0 cache_spec
-        return
-
-    # SLOW PATH - uncommon cases
-    # Another reference to this row (not the exact same row) was already serialized before us
-    if row_type is list:
-        # g_row_data must also be a compact list if row_data is a list
-        # they must have the same length at this stage since we know the cache specs match
-        if g_row_type is list:
-            # fail safe sanity check
-            merge_compact(row_data, g_row_data)
-        
-    elif g_row_type is dict:
-        # then the previously serialized reference to this row
-        # didn't match the g_cache_spec
-        # so just take the itersect of the dictionaries
-        g_table_rows[row_id] = merge_dicts(row_data, g_row_data)
-        return
-    else:
-        # finally the g_row_type is a compact list and we are a dict - make it a dict
-        g_cache_spec = g_table_spec["cache"]
-        merge_dict_with_compact(row_data, g_row_data, row_cache_spec, g_cache_spec)
-        g_table_rows[row_id] = row_data
-
-
-def merge_compact(row_data, g_row_data):
-    # any conflicts just replace with UNCACHED sentinel
-    # use len - 1 so we skip the Capability
-    for i in range(len(row_data) - 1):
-        gbl, loc = g_row_data[i], row_data[i]
-        if gbl != loc:
-            g_row_data[i] = UNCACHED
-
-
-def merge_dicts(row_data, g_row_data):
-    # walk the smallest
-    merged = {}
-    a, b = (row_data, g_row_data) if len(row_data) < len(g_row_data) else (g_row_data, row_data)
-    cap = a.pop(CAP_KEY)
-    for key, a_val in a.items():
-        b_val = b.get(key, NOT_FOUND)
-        if a_val == b_val:
-            merged[key] = a_val
-    merged[CAP_KEY] = a[CAP_KEY] = cap
-    return a
-
-
-def merge_dict_with_compact(row_data, g_row_data, row_cache_spec, g_cache_spec):
-    iter_g_row_data = iter(g_row_data)
-    for i, (is_cached, g_is_cached) in enumerate(zip(row_cache_spec, g_cache_spec)):
-        i = str(i)
-        if not g_is_cached:
-            # we could use the incoming caller wins here
-            if is_cached:
-                row_data.pop(i)
-            continue
-
-        g_val = next(iter_g_row_data)
-        if not is_cached:
-            continue
-
-        if i in row_data and row_data[i] != g_val:
-            row_data.pop(i)
-
-    return row_data
+import anvil.tz
+from anvil.server import Capability, unwrap_capability
+
+from ._constants import CAP_KEY, NOT_FOUND, UNCACHED
+
+
+def validate_cap(cap, view_key, table_id, row_id=NOT_FOUND):
+    import json  # we don't need this on the client
+
+    _, _, view_dict, narrowed, _ = unwrap_capability(cap, ["_", "t", Capability.ANY, Capability.ANY, Capability.ANY])
+    assert view_dict == json.loads(view_key)
+    assert table_id == str(view_dict["id"])
+    if row_id is not NOT_FOUND:
+        assert row_id == str(narrowed["r"])
+
+
+def clean_local_datetime(d):
+    if d.tzinfo is not None:
+        offset = d.utcoffset().total_seconds()
+    else:
+        offset = anvil.tz.tzlocal().utcoffset(d).total_seconds()
+    return d.replace(tzinfo=anvil.tz.tzoffset(seconds=offset))
+
+
+# Serialization helpers
+def check_serialized(self, local_data):
+    self_id = id(self)
+    serialized = local_data.get(self_id, False)
+    local_data[self_id] = True
+    return serialized
+
+
+def init_view_data(view_key, g_table_data):
+    return g_table_data.setdefault(view_key, {})
+
+
+def init_spec_rows(g_view_data, table_spec, cache_spec=None):
+    g_table_spec = g_view_data.get("spec")
+    if g_table_spec is not None:
+        pass
+    elif table_spec is None or cache_spec is None:
+        g_table_spec = g_view_data["spec"] = table_spec
+    else:
+        g_table_spec = g_view_data["spec"] = {"cols": table_spec["cols"], "cache": cache_spec}
+    g_table_rows = g_view_data.setdefault("rows", {})
+    return g_table_spec, g_table_rows
+
+
+def merge_row_data(row_id, row_data, g_table_rows, g_table_spec, row_cache_spec):
+    # we've already cleaned the row_data
+    #  - it will only be a compact list if the caches match
+    #  - and g_row_data is either None or also a compact list
+    # otherwise row_data will be a dict
+    g_row_data = g_table_rows.get(row_id)
+
+    # FAST - common case - nothing in row_data
+    if g_row_data is None:
+        g_table_rows[row_id] = row_data
+        return
+
+    g_row_type = type(g_row_data)
+    row_type = type(row_data)
+
+    # handle all UNCACHED - i.e. the partially cached writer wins
+    if g_row_type is list and len(g_row_data) == 1:
+        # the row serialized before us has an all 0 cache_spec and is compact
+        # we are either a dict or a list of the same length
+        g_table_rows[row_id] = row_data
+        return
+    if not any(row_cache_spec):
+        # the row to merge has an all 0 cache_spec
+        return
+
+    # SLOW PATH - uncommon cases
+    # Another reference to this row (not the exact same row) was already serialized before us
+    if row_type is list:
+        # g_row_data must also be a compact list if row_data is a list
+        # they must have the same length at this stage since we know the cache specs match
+        if g_row_type is list:
+            # fail safe sanity check
+            merge_compact(row_data, g_row_data)
+        
+    elif g_row_type is dict:
+        # then the previously serialized reference to this row
+        # didn't match the g_cache_spec
+        # so just take the itersect of the dictionaries
+        g_table_rows[row_id] = merge_dicts(row_data, g_row_data)
+        return
+    else:
+        # finally the g_row_type is a compact list and we are a dict - make it a dict
+        g_cache_spec = g_table_spec["cache"]
+        merge_dict_with_compact(row_data, g_row_data, row_cache_spec, g_cache_spec)
+        g_table_rows[row_id] = row_data
+
+
+def merge_compact(row_data, g_row_data):
+    # any conflicts just replace with UNCACHED sentinel
+    # use len - 1 so we skip the Capability
+    for i in range(len(row_data) - 1):
+        gbl, loc = g_row_data[i], row_data[i]
+        if gbl != loc:
+            g_row_data[i] = UNCACHED
+
+
+def merge_dicts(row_data, g_row_data):
+    # walk the smallest
+    merged = {}
+    a, b = (row_data, g_row_data) if len(row_data) < len(g_row_data) else (g_row_data, row_data)
+    cap = a.pop(CAP_KEY)
+    for key, a_val in a.items():
+        b_val = b.get(key, NOT_FOUND)
+        if a_val == b_val:
+            merged[key] = a_val
+    merged[CAP_KEY] = a[CAP_KEY] = cap
+    return a
+
+
+def merge_dict_with_compact(row_data, g_row_data, row_cache_spec, g_cache_spec):
+    iter_g_row_data = iter(g_row_data)
+    for i, (is_cached, g_is_cached) in enumerate(zip(row_cache_spec, g_cache_spec)):
+        i = str(i)
+        if not g_is_cached:
+            # we could use the incoming caller wins here
+            if is_cached:
+                row_data.pop(i, None)
+            continue
+
+        g_val = next(iter_g_row_data)
+        if not is_cached:
+            continue
+
+        if i in row_data and row_data[i] != g_val:
+            row_data.pop(i)
+
+    return row_data
```

### Comparing `anvil-app-server-1.8.0/anvil_downlink_worker/anvil/tz.py` & `anvil-app-server-1.9.0/anvil_downlink_worker/anvil/tz.py`

 * *Files identical despite different names*

### Comparing `anvil-app-server-1.8.0/anvil_downlink_worker/anvil/users/__init__.py` & `anvil-app-server-1.9.0/anvil_downlink_worker/anvil/users/__init__.py`

 * *Files identical despite different names*

### Comparing `anvil-app-server-1.8.0/anvil_downlink_worker/anvil/users/exceptions.py` & `anvil-app-server-1.9.0/anvil_downlink_worker/anvil/users/exceptions.py`

 * *Files identical despite different names*

### Comparing `anvil-app-server-1.8.0/anvil_downlink_worker/anvil/users/mfa/__init__.py` & `anvil-app-server-1.9.0/anvil_downlink_worker/anvil/users/mfa/__init__.py`

 * *Files identical despite different names*

### Comparing `anvil-app-server-1.8.0/anvil_downlink_worker/anvil/util.py` & `anvil-app-server-1.9.0/anvil_downlink_worker/anvil/util.py`

 * *Files identical despite different names*

### Comparing `anvil-app-server-1.8.0/anvil_downlink_worker/full_python_worker.py` & `anvil-app-server-1.9.0/anvil_downlink_worker/full_python_worker.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,92 +1,92 @@
-# Run this file, using a serialised version of the RPC protocol on stdin + stdout
-from __future__ import absolute_import
-import os, sys, threading, json, importlib
-from anvil_downlink_worker import handle_incoming_call, load_app
-from anvil_downlink_util.pipes import MessagePipe
-from anvil import _serialise, _server, _threaded_server
-import anvil.server
-import anvil.pdf
-
-PIPE_IN = MessagePipe(os.fdopen(os.dup(0), 'rb'))
-PIPE_OUT = MessagePipe(os.fdopen(os.dup(1), 'wb'))
-OLD_STDERR = os.fdopen(os.dup(2), 'wb')
-
-_threaded_server.console_output = OLD_STDERR
-
-# We use stdin and stdout to talk Anvil-RPC to our manager process.
-# We overwrite sys.stdout and sys.stderr with shims that produce 'output' updates across
-# that interface, and to make sure no direct use of FDs 0/1/2 get in its way
-# To make sure no clever use Overwrite actual stdin and stdout with a thread that forwards them
-new_stdout = os.open(os.devnull, os.O_RDWR)
-os.dup2(new_stdout, 0)
-os.dup2(new_stdout, 1)
-#os.dup2(new_stdout, 2)
-
-
-def write_pipe(data, bin=None):
-    try:
-        PIPE_OUT.send(data, bin)
-    except ValueError:
-        raise _server.SerializationError("You can only pass strings, numbers, arrays, lists, LiveObjects and Media to or from server functions")
-
-
-class DummyStdout:
-    def write(self, s):
-        write_pipe({'output': s, 'id': _threaded_server.call_info.call_id})
-    def flush(self):
-        pass
-
-
-sys.stdout = DummyStdout()
-#sys.stderr = sys.stdout
-
-def dbg(s):
-    sys.stderr.write(s+"\n")
-    sys.stderr.flush()
-
-
-def send_reqresp(r, collect_capabilities=None, remote_is_trusted=False):
-    _serialise.serialise(r, write_pipe, collect_capabilities=collect_capabilities, remote_is_trusted=remote_is_trusted)
-
-_threaded_server.send_reqresp = send_reqresp
-
-
-def run():
-    while True:
-        msg, bindata = PIPE_IN.receive()
-        type = msg.get("type", None)
-        if type in ["CALL_WITH_APP", "LAUNCH_BACKGROUND_WITH_APP", "CALL", "LAUNCH_BACKGROUND",
-                    "LAUNCH_REPL", "REPL_COMMAND", "TERMINATE_REPL"]:
-            handle_incoming_call(msg, write_pipe)
-
-        elif type == "PROVIDE_APP":
-            load_app(msg["app"])
-
-        elif type == "GET_TASK_STATE":
-            def err(*args):
-                raise _server.SerializationError("Cannot use BlobMedia objects in task state.")
-
-            try:
-                sjson = _server.fill_out_media({'id': msg['id'], 'response': anvil.server.task_state}, err,
-                                               remote_is_trusted=False)
-                json.dumps(sjson)
-            except (TypeError, _server.SerializationError) as e:
-                write_pipe({'id': msg['id'], 'error': {'type': 'anvil.server.SerializationError', 'message': "Illegal value in a anvil.server.task_state. " + e.args[0]}})
-            except Exception as e:
-                write_pipe({'id': msg['id'], 'error': {'type': 'anvil.server.InternalError', 'message': "Could not get task state: " + e.args[0]}})
-            else:
-                write_pipe(sjson)
-
-        elif type == "CHUNK_HEADER":
-            _serialise.process_blob_header(msg)
-            _serialise.process_blob(bindata)
-        elif type is None and ("response" in msg or "error" in msg):
-            _threaded_server.IncomingResponse(msg)
-        else:
-            print("Downlink worker socket got unrecognised message: "+repr(msg))
-            sys.stdout.flush()
-            os._exit(1)
-
-
-if __name__ == "__main__":
-    run()
+# Run this file, using a serialised version of the RPC protocol on stdin + stdout
+from __future__ import absolute_import
+import os, sys, threading, json, importlib
+from anvil_downlink_worker import handle_incoming_call, load_app
+from anvil_downlink_util.pipes import MessagePipe
+from anvil import _serialise, _server, _threaded_server
+import anvil.server
+import anvil.pdf
+
+PIPE_IN = MessagePipe(os.fdopen(os.dup(0), 'rb'))
+PIPE_OUT = MessagePipe(os.fdopen(os.dup(1), 'wb'))
+OLD_STDERR = os.fdopen(os.dup(2), 'wb')
+
+_threaded_server.console_output = OLD_STDERR
+
+# We use stdin and stdout to talk Anvil-RPC to our manager process.
+# We overwrite sys.stdout and sys.stderr with shims that produce 'output' updates across
+# that interface, and to make sure no direct use of FDs 0/1/2 get in its way
+# To make sure no clever use Overwrite actual stdin and stdout with a thread that forwards them
+new_stdout = os.open(os.devnull, os.O_RDWR)
+os.dup2(new_stdout, 0)
+os.dup2(new_stdout, 1)
+#os.dup2(new_stdout, 2)
+
+
+def write_pipe(data, bin=None):
+    try:
+        PIPE_OUT.send(data, bin)
+    except ValueError:
+        raise _server.SerializationError("You can only pass strings, numbers, arrays, lists, LiveObjects and Media to or from server functions")
+
+
+class DummyStdout:
+    def write(self, s):
+        write_pipe({'output': s, 'id': _threaded_server.call_info.call_id})
+    def flush(self):
+        pass
+
+
+sys.stdout = DummyStdout()
+#sys.stderr = sys.stdout
+
+def dbg(s):
+    sys.stderr.write(s+"\n")
+    sys.stderr.flush()
+
+
+def send_reqresp(r, collect_capabilities=None, remote_is_trusted=False):
+    _serialise.serialise(r, write_pipe, collect_capabilities=collect_capabilities, remote_is_trusted=remote_is_trusted)
+
+_threaded_server.send_reqresp = send_reqresp
+
+
+def run():
+    while True:
+        msg, bindata = PIPE_IN.receive()
+        type = msg.get("type", None)
+        if type in ["CALL_WITH_APP", "LAUNCH_BACKGROUND_WITH_APP", "CALL", "LAUNCH_BACKGROUND",
+                    "LAUNCH_REPL", "REPL_COMMAND", "TERMINATE_REPL"]:
+            handle_incoming_call(msg, write_pipe)
+
+        elif type == "PROVIDE_APP":
+            load_app(msg["app"])
+
+        elif type == "GET_TASK_STATE":
+            def err(*args):
+                raise _server.SerializationError("Cannot use BlobMedia objects in task state.")
+
+            try:
+                sjson = _server.fill_out_media({'id': msg['id'], 'response': anvil.server.task_state}, err,
+                                               remote_is_trusted=False)
+                json.dumps(sjson)
+            except (TypeError, _server.SerializationError) as e:
+                write_pipe({'id': msg['id'], 'error': {'type': 'anvil.server.SerializationError', 'message': "Illegal value in a anvil.server.task_state. " + e.args[0]}})
+            except Exception as e:
+                write_pipe({'id': msg['id'], 'error': {'type': 'anvil.server.InternalError', 'message': "Could not get task state: " + e.args[0]}})
+            else:
+                write_pipe(sjson)
+
+        elif type == "CHUNK_HEADER":
+            _serialise.process_blob_header(msg)
+            _serialise.process_blob(bindata)
+        elif type is None and ("response" in msg or "error" in msg):
+            _threaded_server.IncomingResponse(msg)
+        else:
+            print("Downlink worker socket got unrecognised message: "+repr(msg))
+            sys.stdout.flush()
+            os._exit(1)
+
+
+if __name__ == "__main__":
+    run()
```

