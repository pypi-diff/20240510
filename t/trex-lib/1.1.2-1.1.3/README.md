# Comparing `tmp/trex-lib-1.1.2.tar.gz` & `tmp/trex-lib-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trex-lib-1.1.2.tar", last modified: Mon May  6 09:46:33 2024, max compression
+gzip compressed data, was "trex-lib-1.1.3.tar", last modified: Fri May 10 06:11:49 2024, max compression
```

## Comparing `trex-lib-1.1.2.tar` & `trex-lib-1.1.3.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-05-06 09:46:33.736161 trex-lib-1.1.2/
--rw-r--r--   0 jacklok    (501) staff       (20)     1052 2020-09-03 05:31:42.000000 trex-lib-1.1.2/LICENSE
--rw-r--r--   0 jacklok    (501) staff       (20)       58 2020-09-03 00:38:04.000000 trex-lib-1.1.2/MANIFEST.in
--rw-r--r--   0 jacklok    (501) staff       (20)      622 2024-05-06 09:46:33.735987 trex-lib-1.1.2/PKG-INFO
--rw-r--r--   0 jacklok    (501) staff       (20)       34 2020-09-03 04:20:20.000000 trex-lib-1.1.2/README.md
--rw-r--r--   0 jacklok    (501) staff       (20)      172 2021-08-13 04:29:57.000000 trex-lib-1.1.2/pyproject.toml
--rw-r--r--   0 jacklok    (501) staff       (20)       75 2024-05-06 09:46:33.736821 trex-lib-1.1.2/setup.cfg
--rw-r--r--   0 jacklok    (501) staff       (20)     1213 2024-05-06 09:46:32.000000 trex-lib-1.1.2/setup.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-05-06 09:46:33.735306 trex-lib-1.1.2/trex_lib.egg-info/
--rw-r--r--   0 jacklok    (501) staff       (20)      622 2024-05-06 09:46:33.000000 trex-lib-1.1.2/trex_lib.egg-info/PKG-INFO
--rw-r--r--   0 jacklok    (501) staff       (20)     1482 2024-05-06 09:46:33.000000 trex-lib-1.1.2/trex_lib.egg-info/SOURCES.txt
--rw-r--r--   0 jacklok    (501) staff       (20)        1 2024-05-06 09:46:33.000000 trex-lib-1.1.2/trex_lib.egg-info/dependency_links.txt
--rw-r--r--   0 jacklok    (501) staff       (20)       89 2024-05-06 09:46:33.000000 trex-lib-1.1.2/trex_lib.egg-info/requires.txt
--rw-r--r--   0 jacklok    (501) staff       (20)       14 2024-05-06 09:46:33.000000 trex-lib-1.1.2/trex_lib.egg-info/top_level.txt
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-05-06 09:46:33.706659 trex-lib-1.1.2/trexlib/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-09-04 07:13:04.000000 trex-lib-1.1.2/trexlib/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)     5426 2024-04-05 01:57:54.000000 trex-lib-1.1.2/trexlib/conf_to_remove.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-05-06 09:46:33.707869 trex-lib-1.1.2/trexlib/libs/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-01-22 09:26:13.000000 trex-lib-1.1.2/trexlib/libs/__init__.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-05-06 09:46:33.708593 trex-lib-1.1.2/trexlib/libs/controllers/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2023-02-13 02:03:08.000000 trex-lib-1.1.2/trexlib/libs/controllers/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)     9783 2024-04-29 04:45:24.000000 trex-lib-1.1.2/trexlib/libs/controllers/task_base_routes.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-05-06 09:46:33.709757 trex-lib-1.1.2/trexlib/libs/facebook/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2024-04-04 09:51:48.000000 trex-lib-1.1.2/trexlib/libs/facebook/__init__.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-05-06 09:46:33.710878 trex-lib-1.1.2/trexlib/libs/facebook/util/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2024-04-04 09:52:59.000000 trex-lib-1.1.2/trexlib/libs/facebook/util/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)     2727 2024-05-06 09:13:17.000000 trex-lib-1.1.2/trexlib/libs/facebook/util/whatsapp_util.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-05-06 09:46:33.712406 trex-lib-1.1.2/trexlib/libs/firebase/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2022-06-09 04:14:24.000000 trex-lib-1.1.2/trexlib/libs/firebase/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)      378 2022-06-09 06:38:00.000000 trex-lib-1.1.2/trexlib/libs/firebase/firebase_helper.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-05-06 09:46:33.715135 trex-lib-1.1.2/trexlib/libs/flask_wtf/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-01-22 09:26:46.000000 trex-lib-1.1.2/trexlib/libs/flask_wtf/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)      133 2021-01-22 09:30:44.000000 trex-lib-1.1.2/trexlib/libs/flask_wtf/crsf_ext.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1918 2024-05-01 14:52:30.000000 trex-lib-1.1.2/trexlib/libs/flask_wtf/request_wrapper.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-05-06 09:46:33.720386 trex-lib-1.1.2/trexlib/utils/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-09-01 09:38:27.000000 trex-lib-1.1.2/trexlib/utils/__init__.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-05-06 09:46:33.730823 trex-lib-1.1.2/trexlib/utils/common/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-08-31 07:47:30.000000 trex-lib-1.1.2/trexlib/utils/common/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)     4514 2022-09-26 14:54:31.000000 trex-lib-1.1.2/trexlib/utils/common/common_util.py
--rw-r--r--   0 jacklok    (501) staff       (20)      926 2023-08-30 15:08:13.000000 trex-lib-1.1.2/trexlib/utils/common/config_util.py
--rw-r--r--   0 jacklok    (501) staff       (20)      488 2020-09-01 10:21:00.000000 trex-lib-1.1.2/trexlib/utils/common/conftest.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1194 2020-09-04 02:28:26.000000 trex-lib-1.1.2/trexlib/utils/common/crm_util.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1573 2021-04-21 02:37:36.000000 trex-lib-1.1.2/trexlib/utils/common/currency_util.py
--rw-r--r--   0 jacklok    (501) staff       (20)     3707 2024-04-29 04:45:34.000000 trex-lib-1.1.2/trexlib/utils/common/date_util.py
--rw-r--r--   0 jacklok    (501) staff       (20)      290 2020-09-01 10:20:46.000000 trex-lib-1.1.2/trexlib/utils/common/float_util.py
--rw-r--r--   0 jacklok    (501) staff       (20)     4201 2021-03-04 08:12:18.000000 trex-lib-1.1.2/trexlib/utils/common/format_util.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1087 2024-04-29 04:45:42.000000 trex-lib-1.1.2/trexlib/utils/common/pagination_util.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1087 2021-06-24 07:11:43.000000 trex-lib-1.1.2/trexlib/utils/common/phone_util.py
--rw-r--r--   0 jacklok    (501) staff       (20)      825 2021-08-13 09:35:21.000000 trex-lib-1.1.2/trexlib/utils/common/user_util.py
--rw-r--r--   0 jacklok    (501) staff       (20)      934 2024-05-06 09:45:42.000000 trex-lib-1.1.2/trexlib/utils/crypto_util.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-05-06 09:46:33.734138 trex-lib-1.1.2/trexlib/utils/google/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-01-20 04:05:45.000000 trex-lib-1.1.2/trexlib/utils/google/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)    12870 2024-04-29 04:38:39.000000 trex-lib-1.1.2/trexlib/utils/google/bigquery_util.py
--rw-r--r--   0 jacklok    (501) staff       (20)     4132 2024-05-06 09:13:26.000000 trex-lib-1.1.2/trexlib/utils/google/cloud_tasks_util.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1365 2024-04-29 04:44:56.000000 trex-lib-1.1.2/trexlib/utils/google/gcloud_util.py
--rw-r--r--   0 jacklok    (501) staff       (20)      159 2020-09-04 07:30:52.000000 trex-lib-1.1.2/trexlib/utils/log_util.py
--rw-r--r--   0 jacklok    (501) staff       (20)      766 2024-03-21 04:18:42.000000 trex-lib-1.1.2/trexlib/utils/member_card_generator.py
--rw-r--r--   0 jacklok    (501) staff       (20)     3216 2024-04-29 04:46:01.000000 trex-lib-1.1.2/trexlib/utils/security_util.py
--rw-r--r--   0 jacklok    (501) staff       (20)     8213 2024-04-29 04:46:10.000000 trex-lib-1.1.2/trexlib/utils/sms_util.py
--rw-r--r--   0 jacklok    (501) staff       (20)     5170 2024-04-22 11:10:51.000000 trex-lib-1.1.2/trexlib/utils/string_util.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1277 2020-09-04 07:38:09.000000 trex-lib-1.1.2/trexlib/utils/url_util.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-05-10 06:11:49.688165 trex-lib-1.1.3/
+-rw-r--r--   0 jacklok    (501) staff       (20)     1052 2020-09-03 05:31:42.000000 trex-lib-1.1.3/LICENSE
+-rw-r--r--   0 jacklok    (501) staff       (20)       58 2020-09-03 00:38:04.000000 trex-lib-1.1.3/MANIFEST.in
+-rw-r--r--   0 jacklok    (501) staff       (20)      622 2024-05-10 06:11:49.687966 trex-lib-1.1.3/PKG-INFO
+-rw-r--r--   0 jacklok    (501) staff       (20)       34 2020-09-03 04:20:20.000000 trex-lib-1.1.3/README.md
+-rw-r--r--   0 jacklok    (501) staff       (20)      172 2021-08-13 04:29:57.000000 trex-lib-1.1.3/pyproject.toml
+-rw-r--r--   0 jacklok    (501) staff       (20)       75 2024-05-10 06:11:49.688929 trex-lib-1.1.3/setup.cfg
+-rw-r--r--   0 jacklok    (501) staff       (20)     1213 2024-05-10 06:11:42.000000 trex-lib-1.1.3/setup.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-05-10 06:11:49.687385 trex-lib-1.1.3/trex_lib.egg-info/
+-rw-r--r--   0 jacklok    (501) staff       (20)      622 2024-05-10 06:11:49.000000 trex-lib-1.1.3/trex_lib.egg-info/PKG-INFO
+-rw-r--r--   0 jacklok    (501) staff       (20)     1482 2024-05-10 06:11:49.000000 trex-lib-1.1.3/trex_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 jacklok    (501) staff       (20)        1 2024-05-10 06:11:49.000000 trex-lib-1.1.3/trex_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 jacklok    (501) staff       (20)       89 2024-05-10 06:11:49.000000 trex-lib-1.1.3/trex_lib.egg-info/requires.txt
+-rw-r--r--   0 jacklok    (501) staff       (20)       14 2024-05-10 06:11:49.000000 trex-lib-1.1.3/trex_lib.egg-info/top_level.txt
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-05-10 06:11:49.658523 trex-lib-1.1.3/trexlib/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-09-04 07:13:04.000000 trex-lib-1.1.3/trexlib/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     5426 2024-04-05 01:57:54.000000 trex-lib-1.1.3/trexlib/conf_to_remove.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-05-10 06:11:49.659770 trex-lib-1.1.3/trexlib/libs/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-01-22 09:26:13.000000 trex-lib-1.1.3/trexlib/libs/__init__.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-05-10 06:11:49.660635 trex-lib-1.1.3/trexlib/libs/controllers/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2023-02-13 02:03:08.000000 trex-lib-1.1.3/trexlib/libs/controllers/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     9783 2024-04-29 04:45:24.000000 trex-lib-1.1.3/trexlib/libs/controllers/task_base_routes.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-05-10 06:11:49.662149 trex-lib-1.1.3/trexlib/libs/facebook/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2024-04-04 09:51:48.000000 trex-lib-1.1.3/trexlib/libs/facebook/__init__.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-05-10 06:11:49.662914 trex-lib-1.1.3/trexlib/libs/facebook/util/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2024-04-04 09:52:59.000000 trex-lib-1.1.3/trexlib/libs/facebook/util/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     2727 2024-05-06 09:13:17.000000 trex-lib-1.1.3/trexlib/libs/facebook/util/whatsapp_util.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-05-10 06:11:49.664090 trex-lib-1.1.3/trexlib/libs/firebase/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2022-06-09 04:14:24.000000 trex-lib-1.1.3/trexlib/libs/firebase/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      378 2022-06-09 06:38:00.000000 trex-lib-1.1.3/trexlib/libs/firebase/firebase_helper.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-05-10 06:11:49.666011 trex-lib-1.1.3/trexlib/libs/flask_wtf/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-01-22 09:26:46.000000 trex-lib-1.1.3/trexlib/libs/flask_wtf/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      133 2021-01-22 09:30:44.000000 trex-lib-1.1.3/trexlib/libs/flask_wtf/crsf_ext.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     2132 2024-05-09 06:20:59.000000 trex-lib-1.1.3/trexlib/libs/flask_wtf/request_wrapper.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-05-10 06:11:49.673924 trex-lib-1.1.3/trexlib/utils/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-09-01 09:38:27.000000 trex-lib-1.1.3/trexlib/utils/__init__.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-05-10 06:11:49.683954 trex-lib-1.1.3/trexlib/utils/common/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-08-31 07:47:30.000000 trex-lib-1.1.3/trexlib/utils/common/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     4514 2022-09-26 14:54:31.000000 trex-lib-1.1.3/trexlib/utils/common/common_util.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      926 2023-08-30 15:08:13.000000 trex-lib-1.1.3/trexlib/utils/common/config_util.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      488 2020-09-01 10:21:00.000000 trex-lib-1.1.3/trexlib/utils/common/conftest.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1194 2020-09-04 02:28:26.000000 trex-lib-1.1.3/trexlib/utils/common/crm_util.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1573 2021-04-21 02:37:36.000000 trex-lib-1.1.3/trexlib/utils/common/currency_util.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     3707 2024-04-29 04:45:34.000000 trex-lib-1.1.3/trexlib/utils/common/date_util.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      290 2020-09-01 10:20:46.000000 trex-lib-1.1.3/trexlib/utils/common/float_util.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     4201 2021-03-04 08:12:18.000000 trex-lib-1.1.3/trexlib/utils/common/format_util.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1087 2024-04-29 04:45:42.000000 trex-lib-1.1.3/trexlib/utils/common/pagination_util.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1087 2021-06-24 07:11:43.000000 trex-lib-1.1.3/trexlib/utils/common/phone_util.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      825 2021-08-13 09:35:21.000000 trex-lib-1.1.3/trexlib/utils/common/user_util.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      934 2024-05-06 09:45:42.000000 trex-lib-1.1.3/trexlib/utils/crypto_util.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-05-10 06:11:49.686597 trex-lib-1.1.3/trexlib/utils/google/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-01-20 04:05:45.000000 trex-lib-1.1.3/trexlib/utils/google/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    12870 2024-04-29 04:38:39.000000 trex-lib-1.1.3/trexlib/utils/google/bigquery_util.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     4132 2024-05-06 09:13:26.000000 trex-lib-1.1.3/trexlib/utils/google/cloud_tasks_util.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1365 2024-04-29 04:44:56.000000 trex-lib-1.1.3/trexlib/utils/google/gcloud_util.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      159 2020-09-04 07:30:52.000000 trex-lib-1.1.3/trexlib/utils/log_util.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      766 2024-03-21 04:18:42.000000 trex-lib-1.1.3/trexlib/utils/member_card_generator.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     3216 2024-04-29 04:46:01.000000 trex-lib-1.1.3/trexlib/utils/security_util.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     8213 2024-04-29 04:46:10.000000 trex-lib-1.1.3/trexlib/utils/sms_util.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     5170 2024-04-22 11:10:51.000000 trex-lib-1.1.3/trexlib/utils/string_util.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1277 2020-09-04 07:38:09.000000 trex-lib-1.1.3/trexlib/utils/url_util.py
```

### Comparing `trex-lib-1.1.2/LICENSE` & `trex-lib-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `trex-lib-1.1.2/PKG-INFO` & `trex-lib-1.1.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trex-lib
-Version: 1.1.2
+Version: 1.1.3
 Summary: TRex Core library package
 Home-page: https://bitbucket.org/lokjac/trex-lib
 Author: Jack Lok
 Author-email: sglok77@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `trex-lib-1.1.2/setup.py` & `trex-lib-1.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 with open("README.md", "r") as fh:
     long_description = fh.read()
     
 setuptools.setup(
      name='trex-lib',  
-     version='1.1.2',
+     version='1.1.3',
      author="Jack Lok",
      author_email="sglok77@gmail.com",
      description="TRex Core library package",
      long_description=long_description,
      long_description_content_type="text/markdown",
      url="https://bitbucket.org/lokjac/trex-lib",
      packages=setuptools.find_packages(),
```

### Comparing `trex-lib-1.1.2/trex_lib.egg-info/PKG-INFO` & `trex-lib-1.1.3/trex_lib.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trex-lib
-Version: 1.1.2
+Version: 1.1.3
 Summary: TRex Core library package
 Home-page: https://bitbucket.org/lokjac/trex-lib
 Author: Jack Lok
 Author-email: sglok77@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `trex-lib-1.1.2/trex_lib.egg-info/SOURCES.txt` & `trex-lib-1.1.3/trex_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trex-lib-1.1.2/trexlib/conf_to_remove.py` & `trex-lib-1.1.3/trexlib/conf_to_remove.py`

 * *Files identical despite different names*

### Comparing `trex-lib-1.1.2/trexlib/libs/controllers/task_base_routes.py` & `trex-lib-1.1.3/trexlib/libs/controllers/task_base_routes.py`

 * *Files identical despite different names*

### Comparing `trex-lib-1.1.2/trexlib/libs/facebook/util/whatsapp_util.py` & `trex-lib-1.1.3/trexlib/libs/facebook/util/whatsapp_util.py`

 * *Files identical despite different names*

### Comparing `trex-lib-1.1.2/trexlib/libs/flask_wtf/request_wrapper.py` & `trex-lib-1.1.3/trexlib/libs/flask_wtf/request_wrapper.py`

 * *Files 6% similar despite different names*

```diff
@@ -61,14 +61,24 @@
         
         values.update(request_json)
         
         return f(*args, values, **kwargs)
 
     return decorated_function
 
+def request_files(f):
+    
+    @wraps(f)
+    def decorated_function(*args, **kwargs):
+        request_files = request.files
+        
+        return f(*args, request_files, **kwargs)
+
+    return decorated_function
+
 def request_form(f):
     
     @wraps(f)
     def decorated_function(*args, **kwargs):
         
         return f(*args, request.form, **kwargs)
```

### Comparing `trex-lib-1.1.2/trexlib/utils/common/common_util.py` & `trex-lib-1.1.3/trexlib/utils/common/common_util.py`

 * *Files identical despite different names*

### Comparing `trex-lib-1.1.2/trexlib/utils/common/config_util.py` & `trex-lib-1.1.3/trexlib/utils/common/config_util.py`

 * *Files identical despite different names*

### Comparing `trex-lib-1.1.2/trexlib/utils/common/crm_util.py` & `trex-lib-1.1.3/trexlib/utils/common/crm_util.py`

 * *Files identical despite different names*

### Comparing `trex-lib-1.1.2/trexlib/utils/common/currency_util.py` & `trex-lib-1.1.3/trexlib/utils/common/currency_util.py`

 * *Files identical despite different names*

### Comparing `trex-lib-1.1.2/trexlib/utils/common/date_util.py` & `trex-lib-1.1.3/trexlib/utils/common/date_util.py`

 * *Files identical despite different names*

### Comparing `trex-lib-1.1.2/trexlib/utils/common/format_util.py` & `trex-lib-1.1.3/trexlib/utils/common/format_util.py`

 * *Files identical despite different names*

### Comparing `trex-lib-1.1.2/trexlib/utils/common/pagination_util.py` & `trex-lib-1.1.3/trexlib/utils/common/pagination_util.py`

 * *Files identical despite different names*

### Comparing `trex-lib-1.1.2/trexlib/utils/common/phone_util.py` & `trex-lib-1.1.3/trexlib/utils/common/phone_util.py`

 * *Files identical despite different names*

### Comparing `trex-lib-1.1.2/trexlib/utils/common/user_util.py` & `trex-lib-1.1.3/trexlib/utils/common/user_util.py`

 * *Files identical despite different names*

### Comparing `trex-lib-1.1.2/trexlib/utils/crypto_util.py` & `trex-lib-1.1.3/trexlib/utils/crypto_util.py`

 * *Files identical despite different names*

### Comparing `trex-lib-1.1.2/trexlib/utils/google/bigquery_util.py` & `trex-lib-1.1.3/trexlib/utils/google/bigquery_util.py`

 * *Files identical despite different names*

### Comparing `trex-lib-1.1.2/trexlib/utils/google/cloud_tasks_util.py` & `trex-lib-1.1.3/trexlib/utils/google/cloud_tasks_util.py`

 * *Files identical despite different names*

### Comparing `trex-lib-1.1.2/trexlib/utils/google/gcloud_util.py` & `trex-lib-1.1.3/trexlib/utils/google/gcloud_util.py`

 * *Files identical despite different names*

### Comparing `trex-lib-1.1.2/trexlib/utils/member_card_generator.py` & `trex-lib-1.1.3/trexlib/utils/member_card_generator.py`

 * *Files identical despite different names*

### Comparing `trex-lib-1.1.2/trexlib/utils/security_util.py` & `trex-lib-1.1.3/trexlib/utils/security_util.py`

 * *Files identical despite different names*

### Comparing `trex-lib-1.1.2/trexlib/utils/sms_util.py` & `trex-lib-1.1.3/trexlib/utils/sms_util.py`

 * *Files identical despite different names*

### Comparing `trex-lib-1.1.2/trexlib/utils/string_util.py` & `trex-lib-1.1.3/trexlib/utils/string_util.py`

 * *Files identical despite different names*

### Comparing `trex-lib-1.1.2/trexlib/utils/url_util.py` & `trex-lib-1.1.3/trexlib/utils/url_util.py`

 * *Files identical despite different names*

