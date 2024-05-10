# Comparing `tmp/anvil-uplink-0.4.1.tar.gz` & `tmp/anvil-uplink-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\anvil-uplink-0.4.1.tar", last modified: Wed Oct 26 16:05:35 2022, max compression
+gzip compressed data, was "dist\anvil-uplink-0.4.2.tar", last modified: Tue Feb  7 10:41:19 2023, max compression
```

## Comparing `anvil-uplink-0.4.1.tar` & `anvil-uplink-0.4.2.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxrwxrwx   0        0        0        0 2022-10-26 16:05:35.006003 anvil-uplink-0.4.1/
--rw-rw-rw-   0        0        0      236 2022-07-08 11:06:57.000000 anvil-uplink-0.4.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1332 2022-10-26 16:05:35.006003 anvil-uplink-0.4.1/PKG-INFO
--rw-rw-rw-   0        0        0      191 2022-07-08 11:06:57.000000 anvil-uplink-0.4.1/README.rst
-drwxrwxrwx   0        0        0        0 2022-10-26 16:05:34.947002 anvil-uplink-0.4.1/anvil/
--rw-rw-rw-   0        0        0     4684 2022-07-26 14:31:31.000000 anvil-uplink-0.4.1/anvil/__init__.py
--rw-rw-rw-   0        0        0     2951 2022-10-26 10:52:14.000000 anvil-uplink-0.4.1/anvil/_components.py
--rw-rw-rw-   0        0        0     4111 2022-07-08 11:06:57.000000 anvil-uplink-0.4.1/anvil/_serialise.py
--rw-rw-rw-   0        0        0    54276 2022-10-05 10:00:39.000000 anvil-uplink-0.4.1/anvil/_server.py
--rw-rw-rw-   0        0        0    16093 2022-07-08 11:06:57.000000 anvil-uplink-0.4.1/anvil/_threaded_server.py
--rw-rw-rw-   0        0        0     3024 2022-07-08 11:06:57.000000 anvil-uplink-0.4.1/anvil/alchemy.py
--rw-rw-rw-   0        0        0     3100 2022-07-26 14:31:31.000000 anvil-uplink-0.4.1/anvil/app_creator.py
--rw-rw-rw-   0        0        0    10975 2022-07-26 14:31:31.000000 anvil-uplink-0.4.1/anvil/email.py
-drwxrwxrwx   0        0        0        0 2022-10-26 16:05:34.949003 anvil-uplink-0.4.1/anvil/facebook/
--rw-rw-rw-   0        0        0        0 2022-07-08 11:06:57.000000 anvil-uplink-0.4.1/anvil/facebook/__init__.py
--rw-rw-rw-   0        0        0      421 2022-07-08 11:06:57.000000 anvil-uplink-0.4.1/anvil/facebook/auth.py
-drwxrwxrwx   0        0        0        0 2022-10-26 16:05:34.951004 anvil-uplink-0.4.1/anvil/files/
--rw-rw-rw-   0        0        0    10538 2022-07-26 14:31:31.000000 anvil-uplink-0.4.1/anvil/files/__init__.py
-drwxrwxrwx   0        0        0        0 2022-10-26 16:05:34.958002 anvil-uplink-0.4.1/anvil/google/
--rw-rw-rw-   0        0        0      181 2022-07-08 11:06:57.000000 anvil-uplink-0.4.1/anvil/google/__init__.py
--rw-rw-rw-   0        0        0      621 2022-07-08 11:06:57.000000 anvil-uplink-0.4.1/anvil/google/auth.py
--rw-rw-rw-   0        0        0    19166 2022-07-08 11:06:57.000000 anvil-uplink-0.4.1/anvil/google/drive.py
--rw-rw-rw-   0        0        0     1435 2022-07-08 11:06:57.000000 anvil-uplink-0.4.1/anvil/google/mail.py
--rw-rw-rw-   0        0        0    13576 2022-10-11 07:55:59.000000 anvil-uplink-0.4.1/anvil/google/sheets.py
--rw-rw-rw-   0        0        0      339 2022-07-08 11:06:57.000000 anvil-uplink-0.4.1/anvil/js.py
--rw-rw-rw-   0        0        0     1638 2022-09-13 10:19:52.000000 anvil-uplink-0.4.1/anvil/media.py
-drwxrwxrwx   0        0        0        0 2022-10-26 16:05:34.960002 anvil-uplink-0.4.1/anvil/microsoft/
--rw-rw-rw-   0        0        0        0 2022-07-08 11:06:57.000000 anvil-uplink-0.4.1/anvil/microsoft/__init__.py
--rw-rw-rw-   0        0        0      688 2022-07-08 11:06:57.000000 anvil-uplink-0.4.1/anvil/microsoft/auth.py
--rw-rw-rw-   0        0        0      698 2022-07-08 11:06:57.000000 anvil-uplink-0.4.1/anvil/mpl_util.py
--rw-rw-rw-   0        0        0      405 2022-07-08 11:06:57.000000 anvil-uplink-0.4.1/anvil/pdf.py
--rw-rw-rw-   0        0        0       86 2022-07-08 11:06:57.000000 anvil-uplink-0.4.1/anvil/regex.py
--rw-rw-rw-   0        0        0     2009 2022-07-08 11:06:57.000000 anvil-uplink-0.4.1/anvil/run_app_via_uplink.py
--rw-rw-rw-   0        0        0      944 2022-07-08 11:06:57.000000 anvil-uplink-0.4.1/anvil/secrets.py
--rw-rw-rw-   0        0        0    15293 2022-09-13 10:19:52.000000 anvil-uplink-0.4.1/anvil/server.py
--rw-rw-rw-   0        0        0     2075 2022-07-08 11:06:57.000000 anvil-uplink-0.4.1/anvil/stripe.py
-drwxrwxrwx   0        0        0        0 2022-10-26 16:05:34.969005 anvil-uplink-0.4.1/anvil/tables/
--rw-rw-rw-   0        0        0     9570 2022-07-26 14:31:31.000000 anvil-uplink-0.4.1/anvil/tables/__init__.py
--rw-rw-rw-   0        0        0      898 2022-07-26 14:31:31.000000 anvil-uplink-0.4.1/anvil/tables/_base_classes.py
--rw-rw-rw-   0        0        0      250 2022-07-26 14:31:31.000000 anvil-uplink-0.4.1/anvil/tables/_config.py
--rw-rw-rw-   0        0        0     1039 2022-07-26 14:31:31.000000 anvil-uplink-0.4.1/anvil/tables/_errors.py
--rw-rw-rw-   0        0        0      428 2022-07-08 11:06:57.000000 anvil-uplink-0.4.1/anvil/tables/_helpers.py
--rw-rw-rw-   0        0        0     5160 2022-07-26 14:31:31.000000 anvil-uplink-0.4.1/anvil/tables/query.py
-drwxrwxrwx   0        0        0        0 2022-10-26 16:05:34.982003 anvil-uplink-0.4.1/anvil/tables/v2/
--rw-rw-rw-   0        0        0      231 2022-07-26 14:31:31.000000 anvil-uplink-0.4.1/anvil/tables/v2/__init__.py
--rw-rw-rw-   0        0        0     1183 2022-07-08 11:06:57.000000 anvil-uplink-0.4.1/anvil/tables/v2/_app_tables.py
--rw-rw-rw-   0        0        0     1730 2022-07-08 11:06:57.000000 anvil-uplink-0.4.1/anvil/tables/v2/_batcher.py
--rw-rw-rw-   0        0        0      845 2022-07-08 11:06:57.000000 anvil-uplink-0.4.1/anvil/tables/v2/_constants.py
--rw-rw-rw-   0        0        0      284 2022-07-26 14:31:31.000000 anvil-uplink-0.4.1/anvil/tables/v2/_load_hacks.py
--rw-rw-rw-   0        0        0     1211 2022-07-08 11:06:57.000000 anvil-uplink-0.4.1/anvil/tables/v2/_refs.py
--rw-rw-rw-   0        0        0    19668 2022-10-03 10:16:06.000000 anvil-uplink-0.4.1/anvil/tables/v2/_row.py
--rw-rw-rw-   0        0        0     9461 2022-07-26 14:31:31.000000 anvil-uplink-0.4.1/anvil/tables/v2/_search.py
--rw-rw-rw-   0        0        0     4339 2022-07-26 14:31:31.000000 anvil-uplink-0.4.1/anvil/tables/v2/_table.py
--rw-rw-rw-   0        0        0     4587 2022-10-18 11:00:12.000000 anvil-uplink-0.4.1/anvil/tables/v2/_utils.py
--rw-rw-rw-   0        0        0     1884 2022-07-08 11:06:57.000000 anvil-uplink-0.4.1/anvil/tz.py
-drwxrwxrwx   0        0        0        0 2022-10-26 16:05:34.986003 anvil-uplink-0.4.1/anvil/users/
--rw-rw-rw-   0        0        0    39389 2022-07-26 14:31:31.000000 anvil-uplink-0.4.1/anvil/users/__init__.py
--rw-rw-rw-   0        0        0      205 2022-07-08 11:06:57.000000 anvil-uplink-0.4.1/anvil/users/config.py
--rw-rw-rw-   0        0        0      979 2022-07-08 11:06:57.000000 anvil-uplink-0.4.1/anvil/users/exceptions.py
-drwxrwxrwx   0        0        0        0 2022-10-26 16:05:34.987002 anvil-uplink-0.4.1/anvil/users/mfa/
--rw-rw-rw-   0        0        0    18862 2022-07-08 11:06:57.000000 anvil-uplink-0.4.1/anvil/users/mfa/__init__.py
--rw-rw-rw-   0        0        0     2525 2022-07-08 11:06:55.000000 anvil-uplink-0.4.1/anvil/util.py
-drwxrwxrwx   0        0        0        0 2022-10-26 16:05:34.995003 anvil-uplink-0.4.1/anvil_uplink.egg-info/
--rw-rw-rw-   0        0        0     1332 2022-10-26 16:05:34.000000 anvil-uplink-0.4.1/anvil_uplink.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1454 2022-10-26 16:05:34.000000 anvil-uplink-0.4.1/anvil_uplink.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-10-26 16:05:34.000000 anvil-uplink-0.4.1/anvil_uplink.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2022-10-26 16:05:34.000000 anvil-uplink-0.4.1/anvil_uplink.egg-info/requires.txt
--rw-rw-rw-   0        0        0       29 2022-10-26 16:05:34.000000 anvil-uplink-0.4.1/anvil_uplink.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2022-10-26 16:05:34.997003 anvil-uplink-0.4.1/facebook/
--rw-rw-rw-   0        0        0        0 2022-07-08 11:06:57.000000 anvil-uplink-0.4.1/facebook/__init__.py
--rw-rw-rw-   0        0        0       34 2022-07-08 11:06:57.000000 anvil-uplink-0.4.1/facebook/auth.py
-drwxrwxrwx   0        0        0        0 2022-10-26 16:05:35.003013 anvil-uplink-0.4.1/google/
--rw-rw-rw-   0        0        0       27 2022-07-08 11:06:57.000000 anvil-uplink-0.4.1/google/__init__.py
--rw-rw-rw-   0        0        0       32 2022-07-08 11:06:57.000000 anvil-uplink-0.4.1/google/auth.py
--rw-rw-rw-   0        0        0       33 2022-07-08 11:06:57.000000 anvil-uplink-0.4.1/google/drive.py
--rw-rw-rw-   0        0        0       32 2022-07-08 11:06:57.000000 anvil-uplink-0.4.1/google/mail.py
--rw-rw-rw-   0        0        0       33 2022-07-08 11:06:57.000000 anvil-uplink-0.4.1/google/sheets.py
--rw-rw-rw-   0        0        0       74 2022-10-26 16:05:35.007003 anvil-uplink-0.4.1/setup.cfg
--rw-rw-rw-   0        0        0     4187 2022-10-26 16:04:58.000000 anvil-uplink-0.4.1/setup.py
-drwxrwxrwx   0        0        0        0 2022-10-26 16:05:35.004002 anvil-uplink-0.4.1/tables/
--rw-rw-rw-   0        0        0       63 2022-07-08 11:06:57.000000 anvil-uplink-0.4.1/tables/__init__.py
+drwxrwxrwx   0        0        0        0 2023-02-07 10:41:19.398012 anvil-uplink-0.4.2/
+-rw-rw-rw-   0        0        0      236 2022-07-08 11:06:57.000000 anvil-uplink-0.4.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     1332 2023-02-07 10:41:19.398012 anvil-uplink-0.4.2/PKG-INFO
+-rw-rw-rw-   0        0        0      191 2022-07-08 11:06:57.000000 anvil-uplink-0.4.2/README.rst
+drwxrwxrwx   0        0        0        0 2023-02-07 10:41:19.326660 anvil-uplink-0.4.2/anvil/
+-rw-rw-rw-   0        0        0     4684 2022-07-26 14:31:31.000000 anvil-uplink-0.4.2/anvil/__init__.py
+-rw-rw-rw-   0        0        0     2951 2023-02-07 10:38:36.000000 anvil-uplink-0.4.2/anvil/_components.py
+-rw-rw-rw-   0        0        0     4111 2022-07-08 11:06:57.000000 anvil-uplink-0.4.2/anvil/_serialise.py
+-rw-rw-rw-   0        0        0    56000 2023-01-26 14:34:47.000000 anvil-uplink-0.4.2/anvil/_server.py
+-rw-rw-rw-   0        0        0    16093 2022-07-08 11:06:57.000000 anvil-uplink-0.4.2/anvil/_threaded_server.py
+-rw-rw-rw-   0        0        0     3024 2022-07-08 11:06:57.000000 anvil-uplink-0.4.2/anvil/alchemy.py
+-rw-rw-rw-   0        0        0     3100 2022-07-26 14:31:31.000000 anvil-uplink-0.4.2/anvil/app_creator.py
+-rw-rw-rw-   0        0        0    10975 2022-07-26 14:31:31.000000 anvil-uplink-0.4.2/anvil/email.py
+drwxrwxrwx   0        0        0        0 2023-02-07 10:41:19.329662 anvil-uplink-0.4.2/anvil/facebook/
+-rw-rw-rw-   0        0        0        0 2022-07-08 11:06:57.000000 anvil-uplink-0.4.2/anvil/facebook/__init__.py
+-rw-rw-rw-   0        0        0      421 2022-07-08 11:06:57.000000 anvil-uplink-0.4.2/anvil/facebook/auth.py
+drwxrwxrwx   0        0        0        0 2023-02-07 10:41:19.331660 anvil-uplink-0.4.2/anvil/files/
+-rw-rw-rw-   0        0        0    12369 2023-01-26 14:34:47.000000 anvil-uplink-0.4.2/anvil/files/__init__.py
+drwxrwxrwx   0        0        0        0 2023-02-07 10:41:19.340659 anvil-uplink-0.4.2/anvil/google/
+-rw-rw-rw-   0        0        0      181 2022-07-08 11:06:57.000000 anvil-uplink-0.4.2/anvil/google/__init__.py
+-rw-rw-rw-   0        0        0      621 2022-07-08 11:06:57.000000 anvil-uplink-0.4.2/anvil/google/auth.py
+-rw-rw-rw-   0        0        0    21821 2023-01-26 14:34:47.000000 anvil-uplink-0.4.2/anvil/google/drive.py
+-rw-rw-rw-   0        0        0     1435 2022-07-08 11:06:57.000000 anvil-uplink-0.4.2/anvil/google/mail.py
+-rw-rw-rw-   0        0        0    13576 2023-01-26 14:34:47.000000 anvil-uplink-0.4.2/anvil/google/sheets.py
+-rw-rw-rw-   0        0        0      339 2022-07-08 11:06:57.000000 anvil-uplink-0.4.2/anvil/js.py
+-rw-rw-rw-   0        0        0     1638 2023-01-26 14:34:47.000000 anvil-uplink-0.4.2/anvil/media.py
+drwxrwxrwx   0        0        0        0 2023-02-07 10:41:19.343661 anvil-uplink-0.4.2/anvil/microsoft/
+-rw-rw-rw-   0        0        0        0 2022-07-08 11:06:57.000000 anvil-uplink-0.4.2/anvil/microsoft/__init__.py
+-rw-rw-rw-   0        0        0      688 2022-07-08 11:06:57.000000 anvil-uplink-0.4.2/anvil/microsoft/auth.py
+-rw-rw-rw-   0        0        0      698 2022-07-08 11:06:57.000000 anvil-uplink-0.4.2/anvil/mpl_util.py
+-rw-rw-rw-   0        0        0      405 2022-07-08 11:06:57.000000 anvil-uplink-0.4.2/anvil/pdf.py
+-rw-rw-rw-   0        0        0       86 2022-07-08 11:06:57.000000 anvil-uplink-0.4.2/anvil/regex.py
+-rw-rw-rw-   0        0        0     2009 2022-07-08 11:06:57.000000 anvil-uplink-0.4.2/anvil/run_app_via_uplink.py
+-rw-rw-rw-   0        0        0      944 2022-07-08 11:06:57.000000 anvil-uplink-0.4.2/anvil/secrets.py
+-rw-rw-rw-   0        0        0    15407 2023-01-26 14:34:47.000000 anvil-uplink-0.4.2/anvil/server.py
+-rw-rw-rw-   0        0        0     2075 2022-07-08 11:06:57.000000 anvil-uplink-0.4.2/anvil/stripe.py
+drwxrwxrwx   0        0        0        0 2023-02-07 10:41:19.353032 anvil-uplink-0.4.2/anvil/tables/
+-rw-rw-rw-   0        0        0     9740 2023-01-26 14:34:47.000000 anvil-uplink-0.4.2/anvil/tables/__init__.py
+-rw-rw-rw-   0        0        0      898 2022-07-26 14:31:31.000000 anvil-uplink-0.4.2/anvil/tables/_base_classes.py
+-rw-rw-rw-   0        0        0      308 2023-01-26 14:34:47.000000 anvil-uplink-0.4.2/anvil/tables/_config.py
+-rw-rw-rw-   0        0        0     1039 2022-07-26 14:31:31.000000 anvil-uplink-0.4.2/anvil/tables/_errors.py
+-rw-rw-rw-   0        0        0      428 2022-07-08 11:06:57.000000 anvil-uplink-0.4.2/anvil/tables/_helpers.py
+-rw-rw-rw-   0        0        0     5160 2022-07-26 14:31:31.000000 anvil-uplink-0.4.2/anvil/tables/query.py
+drwxrwxrwx   0        0        0        0 2023-02-07 10:41:19.370042 anvil-uplink-0.4.2/anvil/tables/v2/
+-rw-rw-rw-   0        0        0      231 2022-07-26 14:31:31.000000 anvil-uplink-0.4.2/anvil/tables/v2/__init__.py
+-rw-rw-rw-   0        0        0     1183 2022-07-08 11:06:57.000000 anvil-uplink-0.4.2/anvil/tables/v2/_app_tables.py
+-rw-rw-rw-   0        0        0     2105 2023-01-26 14:34:47.000000 anvil-uplink-0.4.2/anvil/tables/v2/_batcher.py
+-rw-rw-rw-   0        0        0      845 2022-07-08 11:06:57.000000 anvil-uplink-0.4.2/anvil/tables/v2/_constants.py
+-rw-rw-rw-   0        0        0      284 2022-07-26 14:31:31.000000 anvil-uplink-0.4.2/anvil/tables/v2/_load_hacks.py
+-rw-rw-rw-   0        0        0     1211 2022-07-08 11:06:57.000000 anvil-uplink-0.4.2/anvil/tables/v2/_refs.py
+-rw-rw-rw-   0        0        0    20029 2023-01-26 14:34:47.000000 anvil-uplink-0.4.2/anvil/tables/v2/_row.py
+-rw-rw-rw-   0        0        0     9461 2022-07-26 14:31:31.000000 anvil-uplink-0.4.2/anvil/tables/v2/_search.py
+-rw-rw-rw-   0        0        0     4339 2022-07-26 14:31:31.000000 anvil-uplink-0.4.2/anvil/tables/v2/_table.py
+-rw-rw-rw-   0        0        0     4668 2023-01-26 14:34:47.000000 anvil-uplink-0.4.2/anvil/tables/v2/_utils.py
+-rw-rw-rw-   0        0        0     1964 2023-01-26 14:34:47.000000 anvil-uplink-0.4.2/anvil/tz.py
+drwxrwxrwx   0        0        0        0 2023-02-07 10:41:19.375005 anvil-uplink-0.4.2/anvil/users/
+-rw-rw-rw-   0        0        0    39409 2023-01-26 14:34:47.000000 anvil-uplink-0.4.2/anvil/users/__init__.py
+-rw-rw-rw-   0        0        0      205 2022-07-08 11:06:57.000000 anvil-uplink-0.4.2/anvil/users/config.py
+-rw-rw-rw-   0        0        0      979 2022-07-08 11:06:57.000000 anvil-uplink-0.4.2/anvil/users/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-02-07 10:41:19.376011 anvil-uplink-0.4.2/anvil/users/mfa/
+-rw-rw-rw-   0        0        0    18907 2023-01-26 14:34:47.000000 anvil-uplink-0.4.2/anvil/users/mfa/__init__.py
+-rw-rw-rw-   0        0        0     2525 2022-07-08 11:06:55.000000 anvil-uplink-0.4.2/anvil/util.py
+drwxrwxrwx   0        0        0        0 2023-02-07 10:41:19.385012 anvil-uplink-0.4.2/anvil_uplink.egg-info/
+-rw-rw-rw-   0        0        0     1332 2023-02-07 10:41:18.000000 anvil-uplink-0.4.2/anvil_uplink.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1454 2023-02-07 10:41:19.000000 anvil-uplink-0.4.2/anvil_uplink.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-02-07 10:41:18.000000 anvil-uplink-0.4.2/anvil_uplink.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-02-07 10:41:18.000000 anvil-uplink-0.4.2/anvil_uplink.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       29 2023-02-07 10:41:18.000000 anvil-uplink-0.4.2/anvil_uplink.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-02-07 10:41:19.387012 anvil-uplink-0.4.2/facebook/
+-rw-rw-rw-   0        0        0        0 2022-07-08 11:06:57.000000 anvil-uplink-0.4.2/facebook/__init__.py
+-rw-rw-rw-   0        0        0       34 2022-07-08 11:06:57.000000 anvil-uplink-0.4.2/facebook/auth.py
+drwxrwxrwx   0        0        0        0 2023-02-07 10:41:19.394012 anvil-uplink-0.4.2/google/
+-rw-rw-rw-   0        0        0       27 2022-07-08 11:06:57.000000 anvil-uplink-0.4.2/google/__init__.py
+-rw-rw-rw-   0        0        0       32 2022-07-08 11:06:57.000000 anvil-uplink-0.4.2/google/auth.py
+-rw-rw-rw-   0        0        0       33 2022-07-08 11:06:57.000000 anvil-uplink-0.4.2/google/drive.py
+-rw-rw-rw-   0        0        0       32 2022-07-08 11:06:57.000000 anvil-uplink-0.4.2/google/mail.py
+-rw-rw-rw-   0        0        0       33 2022-07-08 11:06:57.000000 anvil-uplink-0.4.2/google/sheets.py
+-rw-rw-rw-   0        0        0       74 2023-02-07 10:41:19.399013 anvil-uplink-0.4.2/setup.cfg
+-rw-rw-rw-   0        0        0     4187 2023-02-07 10:40:45.000000 anvil-uplink-0.4.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-02-07 10:41:19.396015 anvil-uplink-0.4.2/tables/
+-rw-rw-rw-   0        0        0       63 2022-07-08 11:06:57.000000 anvil-uplink-0.4.2/tables/__init__.py
```

### Comparing `anvil-uplink-0.4.1/PKG-INFO` & `anvil-uplink-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: anvil-uplink
-Version: 0.4.1
+Version: 0.4.2
 Summary: The Anvil server uplink library
 Home-page: https://anvil.works
 Author: Meredydd Luff
 Author-email: meredydd@anvil.works
 License: MIT
 Description: Anvil Server Uplink Library
```

### Comparing `anvil-uplink-0.4.1/anvil/__init__.py` & `anvil-uplink-0.4.2/anvil/__init__.py`

 * *Files identical despite different names*

### Comparing `anvil-uplink-0.4.1/anvil/_components.py` & `anvil-uplink-0.4.2/anvil/_components.py`

 * *Files identical despite different names*

### Comparing `anvil-uplink-0.4.1/anvil/_serialise.py` & `anvil-uplink-0.4.2/anvil/_serialise.py`

 * *Files identical despite different names*

### Comparing `anvil-uplink-0.4.1/anvil/_server.py` & `anvil-uplink-0.4.2/anvil/_server.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,25 +6,26 @@
 import traceback
 import numbers
 import sys
 import re
 import json
 import math
 import anvil.tz
+import functools
 
 _do_call = None
 
 string_type = str if sys.version_info >= (3,) else basestring
 long_type = int if sys.version_info >= (3,) else long
 
 POS_INFINITY = float("inf")
 NEG_INFINITY = float("-inf")
 
 _value_types = {}
-_serialization_helpers = {} # {module_name: helper_fn}, entry removed once helper_fn has been run once.
+_serialization_helpers = {} # {module_name: helper_fn}
 
 class LiveObjectProxy(anvil.LiveObject):
 
     def __init__(self,spec,known_methods=None):
         for k in ["itemCache", "iterItems"]:
             if spec.get(k, {}) is None:
                 del spec[k]
@@ -868,33 +869,41 @@
 def _repr_path(p):
     return "".join(("[%s]" % repr(k) for k in p))
 
 def _module_prefixes(module):
     module_parts = module.split(".")
     return [".".join(module_parts[:i]) for i in range(1, len(module_parts)+1)]
 
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
 
 def fill_out_media(json, handle_media_fn, collect_capabilities=None, remote_is_trusted=False):
     obj_descr = []
     path = []
     known_liveobject_methods = {}
     serialization_info = SerializationInfo(remote_is_trusted=remote_is_trusted)
     import datetime
 
     def do_fom(_json):
 
         t_json = type(_json)
 
-        cls_fullname = t_json.__module__ + "." + t_json.__name__
-        for prefix in _module_prefixes(cls_fullname):
-            if prefix in _serialization_helpers:
-                _serialization_helpers[prefix](cls_fullname)
-                break
-
-
         if hasattr(_json, "SERIALIZATION_INFO"):
             type_name, tp = _json.SERIALIZATION_INFO
             valid_type_name = type_name in _value_types
 
             if valid_type_name and tp is _json:
                 _json = None
                 obj_descr.append({
@@ -973,14 +982,16 @@
         elif isinstance(_json, (datetime.date, datetime.datetime)) or \
                 (isinstance(_json, long_type) and (_json > 2147483647 or _json < -2147483647)) or \
                 (isinstance(_json, float) and (_json == POS_INFINITY or _json == NEG_INFINITY or math.isnan(_json))):
             serialised_val = serialise_val(_json, known_liveobject_methods)
             serialised_val["path"] = list(path)
             obj_descr.append(serialised_val)
             _json = None
+        elif _check_and_call_serialization_helper(t_json.__module__ + "." + t_json.__name__):
+            _json = do_fom(_json)
         elif 'numpy' in sys.modules and hasattr(sys.modules['numpy'], 'generic') and isinstance(_json, sys.modules['numpy'].generic):
 
             _json = _json.item() # convert
 
         elif not (isinstance(_json, string_type) or _json is None or _json is True or _json is False or isinstance(_json, (int, long_type)) or isinstance(_json, float)):
 
             # Rescue: Convert numpy types to nearest equivalent
@@ -1081,19 +1092,15 @@
     value_type = _value_types.get(type_name)
     if value_type is not None:
         return value_type
     # Try importing the relevant module
     i = type_name.rfind('.')
     if i != -1:
         # TODO do we filter what we can specify as import? I don't *think* this is dangerous...
-        for prefix in _module_prefixes(type_name):
-            if prefix in _serialization_helpers:
-                _serialization_helpers[prefix](type_name)
-                break
-        else:
+        if not _check_and_call_serialization_helper(type_name):
             module_name = type_name[:i]
             importlib.import_module(module_name)
         value_type = _value_types.get(type_name)
 
     if value_type is None:
         raise SerializationError("No such serializable type: %s at msg%s" % (type_name, _repr_path(d["path"])))
 
@@ -1362,15 +1369,15 @@
         registrations[name] = require_wrap(new_f)
         new_f._anvil_reregister = reregister
 
     fn._anvil_reregister = reregister
 
     return fn
 
-
+#!defFunction(anvil.server,%,[name], [require_user])!2: {anvil$args: {fn_or_name: "The name by which you want to call your function from the client.", require_user: "Allows you to verify whether a user is logged in. Can be a boolean or a function."}, anvil$helpLink: "server#calling-server-functions-from-client-code", $doc: "When applied to a function as a decorator, the function becomes available from the client side."} ["callable"]
 def callable(fn_or_name=None, require_user=None):
     if fn_or_name is None or isinstance(fn_or_name, string_type):
         return lambda f: register(f, fn_or_name, require_user=require_user)
     else:
         return register(fn_or_name)
 
 
@@ -1382,16 +1389,18 @@
 
 
 # A parameterised decorator
 def callable_as(name):
     print("@callable_as is deprecated. Please use @callable directly.")
     return lambda f: register(f, name)
 
+
+
 def http_endpoint(path, require_credentials=False, authenticate_users=False, authenticate_user=False,
-                  methods=["GET","POST"], enable_cors=False, cross_site_session=False):
+                  methods=["GET","POST"], enable_cors=False, cross_site_session=False, _task_prefix="http"):
     def decorator(fn):
         path_parts = []
         def register_path_part(s):
             path_parts.append(s.group(1))
             return "([^/]*)"
 
         path_regex = re.sub(":([^/]*)", register_path_part, path)
@@ -1475,20 +1484,23 @@
                         "body":    response.body,
                         "headers": add_cross_origin_to_header_dict(response.headers)._headers}
             else:
                 return {"status":  200,
                         "body":    response,
                         "headers": add_cross_origin_to_header_dict({})}
 
-        register(wrapped_fn, path_regex, "http")
+        register(wrapped_fn, path_regex, _task_prefix)
 
         return fn
     return decorator
 
 
+wellknown_endpoint = functools.partial(http_endpoint, _task_prefix = "http-wellknown")
+
+
 class AnvilCookie(object):
 
     def __init__(self, type):
         self._type = type
 
     def __getitem__(self, name):
         return _do_call([self._type, name], None, fn_name="anvil.private.get_cookie")
@@ -1544,14 +1556,15 @@
 
 # Get the value of anvil.server.session for a particular session in the current environment
 def get_client_session(session_id):
     return anvil.server.call("anvil.private.get_session_data", session_id)
 
 
 # Get the ID of the current session
+#!defFunction(anvil.server,%)!2: "Returns the current session's ID." ["get_session_id"]
 def get_session_id():
     return anvil.server.call("anvil.private.get_session_id")
 
 
 # Subscribe this session to receive events from the named channel
 def subscribe(channel):
     return anvil.server.call("anvil.private.subscribe", channel)
@@ -1559,8 +1572,35 @@
 
 # Unsubscribe this session from receiving events from the named channel
 def unsubscribe(channel):
     return anvil.server.call("anvil.private.unsubscribe", channel)
 
 
 def get_subscriptions():
-    return anvil.server.call("anvil.private.get_subscriptions")
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

### Comparing `anvil-uplink-0.4.1/anvil/_threaded_server.py` & `anvil-uplink-0.4.2/anvil/_threaded_server.py`

 * *Files identical despite different names*

### Comparing `anvil-uplink-0.4.1/anvil/alchemy.py` & `anvil-uplink-0.4.2/anvil/alchemy.py`

 * *Files identical despite different names*

### Comparing `anvil-uplink-0.4.1/anvil/app_creator.py` & `anvil-uplink-0.4.2/anvil/app_creator.py`

 * *Files identical despite different names*

### Comparing `anvil-uplink-0.4.1/anvil/email.py` & `anvil-uplink-0.4.2/anvil/email.py`

 * *Files identical despite different names*

### Comparing `anvil-uplink-0.4.1/anvil/files/__init__.py` & `anvil-uplink-0.4.2/anvil/files/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -27,15 +27,18 @@
 
 def enable_debug_logging():
     logger.setLevel(logging.DEBUG)
 
 
 MAX_REMOTE_METADATA_AGE = 5
 DOWNLOAD_TIMEOUT = 5
-FILES_TABLE = getattr(app_tables, "files") # TODO: Get table name from server config
+try:
+    FILES_TABLE = getattr(app_tables, "files") # TODO: Get table name from server config
+except AttributeError:
+    raise Exception("Files table not found. Please add one through the Data Files page of the Anvil Editor.")
 
 class Files(object):
 
     def __init__(self):
         self._table_id = FILES_TABLE._id # TODO: Switch to .id when it works
         self._temp_dir = os.path.join(gettempdir(), "anvil-data-files")
         try:
@@ -105,15 +108,15 @@
         file_row['file_version'] = new_file_version
         logger.debug("Uploaded %s" % path)
         db.execute("UPDATE remote_files SET file_version=? WHERE table_id=? AND path=?", [new_file_version, self._table_id, path])
         db.commit()
         db.execute("UPDATE local_files SET status='PRESENT', last_touched=?, local_file_version=?, remote_file_version=? WHERE table_id=? AND path=?", [time(), new_file_version, new_file_version, self._table_id, path])
         db.commit()
 
-
+    #!defMethod(string)!2: "Return the path of a file" ["__getitem__"]
     def __getitem__(self, path):
         db = self._get_db()
         cur = db.cursor()
         local_path = os.path.join(self._cache_dir, path)
 
         # Fetch and possibly upsert remote table metadata into local DB.
         cur.execute("SELECT * FROM tables WHERE table_id = ?", [self._table_id])
@@ -206,15 +209,16 @@
             logger.debug("LOCAL FILES")
             cur.execute("SELECT * FROM local_files")
             for r in cur.fetchall():
                 logger.debug(dict(r))
             logger.debug("")
 
             return local_path
-
+    
+    #!defMethod(anvil.files.EditingContextManager instance, path)!2: "Edit a file. To ensure the proper acquisition and release of the file, use the `editing`` function in a `with` statement e.g. `with data_files.editing('test.txt') as file:`" ["editing"]
     def editing(self, path):
         local_path = self[path]
         db = self._get_db()
         table_id = self._table_id
         upload = self.upload
 
         class Editing():
@@ -222,16 +226,28 @@
                 return local_path
 
             def __exit__(self, exc_type, exc_val, exc_tb):
                 upload(db, path)
 
         return Editing()
 
+    #!defMethod(anvil.files.OpenContextManager instance, path, [mode="r"])!2: "The open() function opens the file (if possible) and returns the corresponding file object." ["open"]
     @contextmanager
     def open(self, path, mode='r'):
         with open(data_files[path], mode) as f:
             yield f
         if "w" in mode or "a" in mode or "+" in mode or "x" in mode:
             self.upload(self._get_db(), path)
 
+#!defClass(anvil.files,%Files)!:
+
+#!defMethod(string)!2: "Begin editing the file." ["__enter__"]
+#!defMethod(_)!2: "End editing the file, uploading its new contents." ["__exit__"]
+#!defClassNoConstructor(anvil.files,#%EditingContextManager)!1: "<a href='https://docs.python.org/3/library/contextlib.html#contextlib.contextmanager' target='_blank'>Context manager</a> for editing data files."
+
+#!defMethod(File object)!2: "Open the file." ["__enter__"]
+#!defMethod(_)!2: "Close the file, uploading its contents if it was opened for writing or appending." ["__exit__"]
+#!defClassNoConstructor(anvil.files,#%OpenContextManager)!1: "<a href='https://docs.python.org/3/library/contextlib.html#contextlib.contextmanager' target='_blank'>Context manager</a> for opening data files."
+
+#!defModuleAttr(anvil.files)!1: {name: "data_files", pyType: "anvil.files.Files instance", description: "Access Data Files from the <a href='https://docs.python.org/3/library/contextlib.html#contextlib.contextmanager' target='_blank'>Data Files Service</a>. To access a file stored in the Data Files Service use square brackets containing the path of the desired file - `data_files['<file_path>']`."}
 data_files = Files()
```

### Comparing `anvil-uplink-0.4.1/anvil/google/auth.py` & `anvil-uplink-0.4.2/anvil/google/auth.py`

 * *Files identical despite different names*

### Comparing `anvil-uplink-0.4.1/anvil/google/drive.py` & `anvil-uplink-0.4.2/anvil/google/drive.py`

 * *Files 11% similar despite different names*

```diff
@@ -110,25 +110,31 @@
 
 class DriveItem(ApiItem):
 
     def __setitem__(self, item_name, value):
         if item_name in ["title"]: # List of valid fields to set
             update_metadata(self, {item_name: value}, self.creds)
         else:
-            object.__setitem__(self, item_name, value)
+            raise KeyError(item_name)
 
+    #!defMethod(,dest_folder)!2: "Move the DriveItem from one folder to another" ["move"]
     def move(self, dest_folder):
         return update_metadata(self, { 'parents': [{ 'id': dest_folder.id, 'old_id': self['parents'][0]['id'] }]}, self.creds)
-
+    
+    #!defMethod(_)!2: "Move the DriveItem to the trash folder" ["trash"]
     def trash(self):
         ctor = type(self)
         return ctor(rpc.call("anvil.private.google.drive.trash", self.id, self.creds), self.creds)
 
+    #!defMethod(_)!2: "Delete the DriveItem (this cannot be undone)" ["delete"]
     def delete(self):
         rpc.call("anvil.private.google.drive.delete", self.id, self.creds)
+#!defAttr()!1: {name: "id", type: "string", description: "ID of the DriveItem"}
+#!defClass(anvil.google.drive,#DriveItem)!:
+
 
 
 class File(DriveItem,rpc.LazyMedia):
 
     def __init__(self,d,creds):
       rpc.LazyMedia.__init__(self,d["anvil_LazyMedia"])
       ApiItem.__init__(self,d,creds)
@@ -153,15 +159,15 @@
         # Was "elif attr_name == "_obj" or attr_name == "creds":"
         # but that broke at least _spec, and possibly something else
         else:
             object.__setattr__(self, attr_name, value)
         #else:
         #    raise Exception("Cannot set attribute '" + attr_name + "' of a Google Drive file")
 
-
+    #!defMethod(_)!2: "Get the contents of an object representing a Google Drive file. Native Google files such as Docs, Slides and Sheets must first be exported to an appropriate file type. All other file types support get_bytes()." ["get_bytes"]
     def get_bytes(self, revision=None):
 
         if revision:
             url = revision["downloadUrl"]
         else:
             url = self._obj["downloadUrl"]
 
@@ -173,29 +179,31 @@
         return self["mimeType"]
 
     def get_name(self):
         return self["title"]
 
     def get_length(self):
         return int(self["fileSize"])
-
+    
+    #!defMethod(,content)!2: "Set the contents of an object representing a Google Drive file." ["set_bytes"]
     def set_bytes(self, content):
 
         # Use simple upload to replace content. Don't need to touch metadata.
 
         content_type = "text/plain"
 
         if not isinstance(content, str):
             raise Exception("The 'bytes' of a file must be a Python string. To upload a Media object, use set_media().")
 
         r = rpc.call("anvil.private.google.drive.set_content", self.id, content, self.creds)
 
         self._obj["mimeType"] = content_type
         return File(r, self.creds)
 
+    #!defMethod(,media)!2: "Upload new contents to an existing File. Media must be a Media object." ["set_media"]
     def set_media(self, media):
         if not isinstance(media, anvil.Media):
             raise Exception("set_media() must be called with a Media object.")
 
         r = rpc.call("anvil.private.google.drive.set_content", self.id, media, self.creds)
 
         self._obj["mimeType"] = media.content_type
@@ -205,16 +213,18 @@
     def list_revisions(self):
 
         def request_page_fn(page_token):
             return rpc.call("anvil.private.google.drive.list_file_revisions", self.id, self.creds, page_token)
 
         return wrap_gen(_list_gen(request_page_fn), self.creds, FileRevision);
 
+
     def __str__(self):
         return "<Google Drive File: %s>" % self["title"]
+#!defClass(anvil.google.drive,#File, anvil.google.drive.DriveItem, anvil.Media)!:
 
 
 class FileRevision(ApiItem):
 
     def __getattr__(self, attr_name):
         if attr_name == "date":
             return self["modifiedDate"]
@@ -231,61 +241,70 @@
             return list(self.list_folders())
         else:
             return DriveItem.__getattr__(self, attr_name)
 
     # Bear in mind that these query strings must correspond exactly to the server
     # proxy whitelist, or the request will be refused for app files.
 
+    #!defMethod(generator[anvil.google.drive.File instance])!2: "List the files (not folders) in the Folder." ["list_files"]
     def list_files(self):
-
         def request_page_fn(page_token):
             return rpc.call("anvil.private.google.drive.list_files", 
                             self.id, 
                             self.creds, 
                             page_token=page_token,
                             trashed=False,
                             mime_type='!application/vnd.google-apps.folder')
-
         return wrap_gen(_list_gen(request_page_fn), self.creds);
 
+    #!defMethod(generator[anvil.google.drive.Folder instance])!2: "List the folders (not files) in the Folder." ["list_folders"]
     def list_folders(self):
 
         def request_page_fn(page_token):
             return rpc.call("anvil.private.google.drive.list_files", 
                             self.id, 
                             self.creds, 
                             page_token=page_token,
                             trashed=False,
                             mime_type='application/vnd.google-apps.folder')
 
         return wrap_gen(_list_gen(request_page_fn), self.creds);
 
+    #!defMethod(anvil.google.drive.File instance,title)!2: "Get the File item by title. The title argument should be a string." ["get"]
     def get(self, title):
         return wrap_item(_query_single(self.id, self.creds, title=title, trashed=False), self.creds)
 
+    #!defMethod(anvil.google.drive.File instance,id)!2: "Get the File item by ID. The ID argument should be a string." ["get_by_id"]
     def get_by_id(self, id):
         if not isinstance(id, basestring):
             raise Exception("ID must be a string")
 
         if id == "":
             raise Exception("The empty string is not a valid ID")
 
         return wrap_item(rpc.call("anvil.private.google.drive.get_file_by_id", self.id, id, self.creds), self.creds)
 
+    #!defMethod(,title)!2: "Create a new folder within the Folder." ["create_folder"]
     def create_folder(self, title):
         return create_item_simple(title, self, "application/vnd.google-apps.folder", self.creds)
 
+    #!defMethod(,title, [content_bytes=None], [content_type='text/plain'])!2: "Create a new file within the Folder." ["create_file"]
     def create_file(self, title, content_bytes = None, content_type = "text/plain"):
         if content_bytes:
             return create_item_multipart(title, self, content_bytes, self.creds, content_type=content_type)
         else:
             return create_item_simple(title, self, content_type, self.creds)
 
     def __str__(self):
         return "<Google Drive Folder: %s>" % self["title"]
+#!defAttr()!1: {name: "folders", type: "list(anvil.google.drive.Folder instance)", description: "List of Folder items in the Folder"}
+#!defAttr()!1: {name: "files", type: "list(anvil.google.drive.File instance)", description: "List of File items in the Folder"}
+#!defMethod(_)!2: {anvil$helpLink: "/docs/integrations/google/google-drive#folders"} ["__init__"]
+#!defClass(anvil.google.drive,#Folder, anvil.google.drive.DriveItem)!:
+
 
 #####
 # Documentation
 #####
 """
 id: google_drive
 docs_url: /docs/integrations/google/google-drive
@@ -555,18 +574,27 @@
 
 """
 
 
 #####
 # API methods
 #####
-
+#!defFunction(anvil.google.drive,_,[extra_scopes=])!2: 
+# {
+#   $doc: "Prompt the user to log in to their Google account and ask permission to access their Google Drive files.",
+#   anvil$helpLink: "/docs/integrations/google/google-drive#user-files"
+# } ["login"]
 def login(extra_scopes=[]):
     return anvil.google.auth.login(google_api_scopes + extra_scopes)
 
+#!defFunction(anvil.google.drive, anvil.google.drive.Folder instance)!2: 
+# {
+#   $doc: "Return the top-level folder containing all the files in the Users drive. anvil.google.drive.login() must be called first.",
+#   anvil$helpLink: "/docs/integrations/google/google-drive#user-files"
+# } ["get_user_files"]
 def get_user_files():
     return Folder(rpc.call("anvil.private.google.drive.get_user_files"), "google-user")
 
 class AppFilesCollection:
 
     def __getattr__(self, python_name):
         id = None
```

### Comparing `anvil-uplink-0.4.1/anvil/google/mail.py` & `anvil-uplink-0.4.2/anvil/google/mail.py`

 * *Files identical despite different names*

### Comparing `anvil-uplink-0.4.1/anvil/google/sheets.py` & `anvil-uplink-0.4.2/anvil/google/sheets.py`

 * *Files identical despite different names*

### Comparing `anvil-uplink-0.4.1/anvil/media.py` & `anvil-uplink-0.4.2/anvil/media.py`

 * *Files identical despite different names*

### Comparing `anvil-uplink-0.4.1/anvil/microsoft/auth.py` & `anvil-uplink-0.4.2/anvil/microsoft/auth.py`

 * *Files identical despite different names*

### Comparing `anvil-uplink-0.4.1/anvil/mpl_util.py` & `anvil-uplink-0.4.2/anvil/mpl_util.py`

 * *Files identical despite different names*

### Comparing `anvil-uplink-0.4.1/anvil/run_app_via_uplink.py` & `anvil-uplink-0.4.2/anvil/run_app_via_uplink.py`

 * *Files identical despite different names*

### Comparing `anvil-uplink-0.4.1/anvil/secrets.py` & `anvil-uplink-0.4.2/anvil/secrets.py`

 * *Files identical despite different names*

### Comparing `anvil-uplink-0.4.1/anvil/server.py` & `anvil-uplink-0.4.2/anvil/server.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,14 +34,15 @@
                       ServiceNotAdded,
                       CookieError, 
                       _FailError, 
                       BackgroundTaskError,
                       BackgroundTaskNotFound,
                       BackgroundTaskKilled,
                       http_endpoint, 
+                      wellknown_endpoint,
                       api_request as request, 
                       HttpResponse, 
                       Capability,
                       unwrap_capability,
                       cookies,
                       CallContext,
                       raise_event,
@@ -362,14 +363,16 @@
     global _key, _url, _connection
     _key = _url = None
     with _connection_lock:
         c = _connection
         _connection = None
     if c:
         try:
+            import anvil.tables
+            anvil.tables._clear_cache()
             c.close()
         except:
             pass
 
 
 
 def run_forever():
```

### Comparing `anvil-uplink-0.4.1/anvil/stripe.py` & `anvil-uplink-0.4.2/anvil/stripe.py`

 * *Files identical despite different names*

### Comparing `anvil-uplink-0.4.1/anvil/tables/__init__.py` & `anvil-uplink-0.4.2/anvil/tables/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import time
 
 import anvil.server
 
 from ._base_classes import Row, SearchIterator, Table
-from ._config import get_client_config as _get_config
+from . import _config
 from ._errors import NoSuchColumnError, QuotaExceededError, RowDeleted, TableError, TransactionConflict
 from ._helpers import _hash_wrapper
 
 # Hack: Force ourselves into the top-level package, even
 # if we were loaded into a runtime-v1 per-app Anvil package
 __package__ = "anvil.tables"
 __name__ = "anvil.tables"
@@ -26,23 +26,25 @@
             return tbl
 
         raise AttributeError("No such app table: '%s'" % name)
 
     def __setattr__(self, name, val):
         raise Exception("app_tables is read-only")
 
+_set_class = object.__dict__["__class__"].__set__
 
 def _lazy_replace_class(self):
-    set_class = object.__dict__["__class__"].__set__
-    if _get_config().get("enable_v2"):
+    if _config.get_client_config().get("enable_v2"):
         from . import v2
-
-        set_class(self, type(v2.app_tables))
+        v2._app_tables._clear_cache()
+        _set_class(self, type(v2.app_tables))
     else:
-        set_class(self, AppTables)
+        AppTables.cache = None
+        _set_class(self, AppTables)
+
 
 
 def _wrap_dunder(method):
     def wrapped(self, *args, **kws):
         _lazy_replace_class(self)
         return getattr(self, method)(*args, **kws)
 
@@ -58,15 +60,15 @@
     __getitem__ = _wrap_dunder("__getitem__")
     __dir__ = _wrap_dunder("__dir__")
 
 
 class _LazyContext(object):
     def __enter__(self):
         global batch_update, batch_delete
-        if not _get_config().get("enable_v2"):
+        if not _config.get_client_config().get("enable_v2"):
             batch_update.__class__ = batch_delete.__class__ = type(None)
             return self.__enter__()
 
         from .v2 import _batcher as _b
 
         for obj, orig in zip((batch_update, batch_delete), ("batch_update", "batch_delete")):
             obj.__class__ = type(getattr(_b, orig))
@@ -75,14 +77,19 @@
         return self.__enter__()
 
     def __exit__(self, *args):
         assert not isinstance(self, _LazyContext)
         return self.__exit__(*args)
 
 
+def _clear_cache():
+    _config.reset_config()
+    _set_class(app_tables, _LazyAppTables)
+
+
 #!defModuleAttr(anvil.tables)!1:
 # {
 # 	name: "app_tables",
 # 	type: "any",
 # 	anvil$helpLink: "/docs/data-tables/data-tables-in-code",
 # 	$doc: "Access Table objects from the datatables services. You can access a Table object with dot notation e.g. `app_tables.my_table`. To access a table with strings use `getattr(app_tables, 'my_table')`. If no table is present an AttributeError will be thrown."
 # }
@@ -92,15 +99,15 @@
 batch_delete = _LazyContext()
 # Not very nice but these references exist in uplink code
 # before we have a chance to know if we're using the v1/v2 config option
 # we can't call anvil.server until the uplink has made a connetion
 
 
 def get_table_by_id(table_id):
-    if _get_config().get("enable_v2"):
+    if _config.get_client_config().get("enable_v2"):
         from .v2 import get_table_by_id
 
         return get_table_by_id(table_id)
     raise TableError("get_table_by_id is only available in Accelerated Tables beta")
 
 
 #!defModuleAttr(anvil.tables)!1:
```

### Comparing `anvil-uplink-0.4.1/anvil/tables/_base_classes.py` & `anvil-uplink-0.4.2/anvil/tables/_base_classes.py`

 * *Files identical despite different names*

### Comparing `anvil-uplink-0.4.1/anvil/tables/_errors.py` & `anvil-uplink-0.4.2/anvil/tables/_errors.py`

 * *Files identical despite different names*

### Comparing `anvil-uplink-0.4.1/anvil/tables/query.py` & `anvil-uplink-0.4.2/anvil/tables/query.py`

 * *Files identical despite different names*

### Comparing `anvil-uplink-0.4.1/anvil/tables/v2/_app_tables.py` & `anvil-uplink-0.4.2/anvil/tables/v2/_app_tables.py`

 * *Files identical despite different names*

### Comparing `anvil-uplink-0.4.1/anvil/tables/v2/_batcher.py` & `anvil-uplink-0.4.2/anvil/tables/v2/_batcher.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import anvil.server
 
-from ._constants import SERVER_PREFIX
+from ._constants import SERVER_PREFIX, NOT_FOUND
 
 PREFIX = SERVER_PREFIX + "row."
 _make_refs = None  # Circular import
 
 
 class _Batcher:
     _name = ""
@@ -13,51 +13,62 @@
     def __new__(cls):
         if cls._instance is None:
             cls._instance = object.__new__(cls)
         return cls._instance
 
     def __init__(self):
         self._active = False
-        self._updates = ()
+        self._updates = []
+        self._buffer = {}
         self._func = PREFIX + self._name
 
     @property
     def active(self):
         return self._active
 
     def push(self, cap, update=False):
-        self._updates += ((cap, update),)
+        self._updates.append((cap, update))
 
     def reset(self):
         self._active = False
-        self._updates = ()
+        self._updates.clear()
+        self._buffer.clear()
 
     def __enter__(self):
         if self._active:
             raise RuntimeError("nested batching is not suppported")
         self._active = True
 
     def get_args(self, updates):
         raise NotImplementedError
 
     def __exit__(self, exc_type, exc_value, traceback):
         updates = self._updates
-        self.reset()
-        if exc_value is not None:
-            return
-        if not updates:
-            return
-        anvil.server.call(self._func, self.get_args(updates))
-        for cap, update in updates:
-            cap.send_update(update)
+        try:
+            if exc_value is None and updates:
+                anvil.server.call(self._func, self.get_args(updates))
+                for cap, update in updates:
+                    cap.send_update(update)
+        finally:
+            self.reset()
 
 
 class BatchUpdate(_Batcher):
     _name = "batch_update"
 
+    def push(self, cap, update):
+        self._updates.append((cap, update))
+        self._buffer.setdefault(cap, {}).update(update)
+
+    def get_updates(self, cap):
+        return self._buffer.get(cap, {})
+
+    def read(self, cap, key):
+        return self.get_updates(cap).get(key, NOT_FOUND)
+
     def get_args(self, updates):
         global _make_refs
         if _make_refs is None:
             from ._refs import make_refs  # circular import
 
             _make_refs = make_refs
```

### Comparing `anvil-uplink-0.4.1/anvil/tables/v2/_constants.py` & `anvil-uplink-0.4.2/anvil/tables/v2/_constants.py`

 * *Files identical despite different names*

### Comparing `anvil-uplink-0.4.1/anvil/tables/v2/_refs.py` & `anvil-uplink-0.4.2/anvil/tables/v2/_refs.py`

 * *Files identical despite different names*

### Comparing `anvil-uplink-0.4.1/anvil/tables/v2/_row.py` & `anvil-uplink-0.4.2/anvil/tables/v2/_row.py`

 * *Files 3% similar despite different names*

```diff
@@ -173,65 +173,57 @@
         elif type == SINGLE:
             row = val
             val = row._merge_and_reduce(g_table_data, local_data)
         elif type == MULTIPLE:
             val = [row._merge_and_reduce(g_table_data, local_data) for row in val]
         return val
 
-    def _make_row_data(self, g_table_data, local_data, cache_spec, adder):
+    def _make_row_data(self, g_table_data, local_data, cache_spec):
         table_spec = self._spec
         table_cols = table_spec["cols"] if table_spec is not None else []
         cache = self._cache
         # we can't rely on the order of cache in python 2
+        cached_data = []
         for i, (col, is_cached) in enumerate(zip(table_cols, cache_spec)):
             if not is_cached:
                 continue
             name = col["name"]
             val = self._merge_linked(cache[name], col, g_table_data, local_data)
-            adder(i, val)
-        adder(CAP_KEY, self._cap)
+            cached_data.append((i, val))
+        cached_data.append((CAP_KEY, self._cap))
+        return cached_data
 
     def _merge_and_reduce(self, g_table_data, local_data):
         if check_serialized(self, local_data):
             return int(self._id)
         g_view_data = init_view_data(self._view_key, g_table_data)
         table_spec, row_id, cache_spec = self._spec, self._id, self._cache_spec
 
         # We assert that there is no way for rows from the same view_key to have different col_specs
         # This includes the order
-        # the only thing they may differ on is cached_specs
+        # the only thing they may differ on is cache_specs
         g_table_spec, g_table_rows = init_spec_rows(g_view_data, table_spec, cache_spec)
-        g_row_data = g_table_rows.get(row_id, [])
         g_cache_spec = g_table_spec["cache"] if g_table_spec is not None else None
-        # the local cache spec is always a list
-        # so if the g_gable_spec is None then is_compact will always be False
+
         if table_spec is not None and g_cache_spec is not None:
             is_dirty = self._dirty_spec or len(cache_spec) != len(g_cache_spec)
-            is_compact = not is_dirty and cache_spec == g_cache_spec and type(g_row_data) is list
         else:
             is_dirty = self._dirty_spec
-            is_compact = False
-
-        if is_compact:
-            row_data = []
-
-            def adder(_, val):
-                row_data.append(val)
-
-        else:
-            row_data = {}
-
-            def adder(index, val):
-                row_data[str(index)] = val
 
         if is_dirty:
             g_view_data["dirty_spec"] = True
             cache_spec = []
 
-        self._make_row_data(g_table_data, local_data, cache_spec, adder)
+        cached_data = self._make_row_data(g_table_data, local_data, cache_spec)
+        existing = g_table_rows.get(row_id, [])
+
+        if not is_dirty and cache_spec == g_cache_spec and type(existing) is list:
+            row_data = [val for _, val in cached_data]
+        else:
+            row_data = {str(key): val for key, val in cached_data}
 
         merge_row_data(row_id, row_data, g_table_rows, g_table_spec, cache_spec)
         return int(row_id)
 
     # PRIVATE METHODS
     def _cap_update_handler(self, updates):
         if updates is False:
@@ -327,14 +319,18 @@
 
     def __contains__(self, key):
         return key in self.keys()
 
     def __getitem__(self, key):
         if not isinstance(key, str):
             raise TypeError("Row columns are always strings, not {}".format(type(key).__name__))
+        if _batcher.batch_update.active:
+            rv = _batcher.batch_update.read(self._cap, key)
+            if key is not NOT_FOUND:
+                return _copy(rv)
         if self._spec is None:
             self._fill_cache()
         hit = self._cache.get(key, NOT_FOUND)
         if hit is UNCACHED:
             # we have a spec now so we'll fetch the remaining columns
             self._fill_cache()
         elif hit is NOT_FOUND:
@@ -418,21 +414,27 @@
     def keys(self):
         if self._spec is None:
             # if we don't have a _spec we don't have any keys
             # but we don't need to blindly call _fill_uncached: UNCACHED values are fine
             self._fill_cache()
         return self._cache.keys()
 
-    def items(self):
+    def _get_view(self):
         self._fill_cache()
-        return _copy(self._cache).items()
+        view = _copy(self._cache)
+        if _batcher.batch_update.active:
+            batched = _batcher.batch_update.get_updates(self._cap)
+            view.update(_copy(batched))
+        return view
+
+    def items(self):
+        return self._get_view().items()
 
     def values(self):
-        self._fill_cache()
-        return _copy(self._cache).values()
+        return self._get_view().values()
 
     def update(*args, **new_items):
         # avoid name conflicts with columns, could use (self, other, /, **kws)
         # but positioin only args not available in py2/Skulpt
         if not args:
             raise TypeError("method 'update' of 'Row' object needs an argument")
         elif len(args) > 2:
@@ -485,19 +487,25 @@
     def __iter__(self):
         return self
 
     def __next__(self):
         if self._fill_required:
             self._row._fill_cache()
             self.__init__(self._row)
-        item = next(self._iter)
-        if item[1] is not UNCACHED:
-            return item
-        self._row._fill_cache()
-        # fill the rest of the cache
-        # since we probably want all the items!
-        key = item[0]
-        # we rely here on the _cache keys not changing during iteration
-        # which works since we've filled it with UNCACHED values that match our expected keys
-        return (key, _copy(self._row._cache[key]))
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
 
     next = __next__
```

### Comparing `anvil-uplink-0.4.1/anvil/tables/v2/_search.py` & `anvil-uplink-0.4.2/anvil/tables/v2/_search.py`

 * *Files identical despite different names*

### Comparing `anvil-uplink-0.4.1/anvil/tables/v2/_table.py` & `anvil-uplink-0.4.2/anvil/tables/v2/_table.py`

 * *Files identical despite different names*

### Comparing `anvil-uplink-0.4.1/anvil/tables/v2/_utils.py` & `anvil-uplink-0.4.2/anvil/tables/v2/_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,15 +72,18 @@
         return
 
     # SLOW PATH - uncommon cases
     # Another reference to this row (not the exact same row) was already serialized before us
     if row_type is list:
         # g_row_data must also be a compact list if row_data is a list
         # they must have the same length at this stage since we know the cache specs match
-        merge_compact(row_data, g_row_data)
+        if g_row_type is list:
+            # fail safe sanity check
+            merge_compact(row_data, g_row_data)
+        
     elif g_row_type is dict:
         # then the previously serialized reference to this row
         # didn't match the g_cache_spec
         # so just take the itersect of the dictionaries
         g_table_rows[row_id] = merge_dicts(row_data, g_row_data)
         return
     else:
```

### Comparing `anvil-uplink-0.4.1/anvil/tz.py` & `anvil-uplink-0.4.2/anvil/tz.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,58 +1,66 @@
 import datetime
 import time
 
 
 class tzoffset(datetime.tzinfo):
 
-	#!defMethod(_,[seconds], [minutes], [hours])!2: "Create a timezone with a specific offset. Use an offset in seconds, minutes or hours" ["__init__"]
+    #!defMethod(_,[seconds], [minutes], [hours])!2: "Create a timezone with a specific offset. Use an offset in seconds, minutes or hours" ["__init__"]
     def __init__(self, **kwargs):
         # Must initialise with seconds OR minutes OR hours, or with no arguments to get an offset of zero.
-        if len(kwargs) > 1 or (len(kwargs) == 1 and not 'seconds' in kwargs and not 'hours' in kwargs and not 'minutes' in kwargs):
-            raise Exception("tzoffset must be initialised with precisely one of 'seconds', 'minutes' or 'hours' keyword arguments")
+        if len(kwargs) > 1 or (
+            len(kwargs) == 1 and "seconds" not in kwargs and "hours" not in kwargs and "minutes" not in kwargs
+        ):
+            raise TypeError(
+                "tzoffset must be initialised with precisely one of 'seconds', 'minutes' or 'hours' keyword arguments"
+            )
 
         self._offset = datetime.timedelta(**kwargs)
 
-
     def utcoffset(self, dt):
         return self._offset
 
     def dst(self, dt):
         return datetime.timedelta()
 
     def tzname(self, dt):
         return None
 
     def __repr__(self):
-        return "tzoffset(%s hours)" % (self._offset.total_seconds() / 3600)
+        mod = self.__module__
+        name = type(self).__name__
+        offset = self._offset.total_seconds() / 3600
+        return "<{}.{} ({} hour offset)>".format(mod, name, offset)
+
+
 #!defClass(anvil.tz, tzoffset)!:
 
 
 # People should probably never use this, but we provide it for completeness.
 class tzlocal(tzoffset):
 
-	#!defMethod(_)!2: "Use the local timezone of the browser" ["__init__"]
+    #!defMethod(_)!2: "Use the local timezone of the browser" ["__init__"]
     def __init__(self):
         if time.localtime().tm_isdst and time.daylight:
             s = -time.altzone
         else:
             s = -time.timezone
         tzoffset.__init__(self, seconds=s)
 
 
-    def __repr__(self):
-        return "tzlocal(%s hour offset)" % (self._offset.total_seconds() / 3600)
 #!defClass(anvil.tz, tzlocal, anvil.tz.tzoffset)!:
 
 
 class tzutc(tzoffset):
 
-	#!defMethod(_)!2: "Create a timezone set to utc" ["__init__"]
+    #!defMethod(_)!2: "Create a timezone set to utc" ["__init__"]
     def __init__(self):
         tzoffset.__init__(self, minutes=0)
 
     def __repr__(self):
-        return "tzutc"
+        return "<anvil.tz.tzutc>"
+
+
 #!defClass(anvil.tz, tzutc, anvil.tz.tzoffset)!:
 
 #!defModuleAttr(anvil.tz)!1: {name: 'UTC', type: 'any', description: 'An object representing the UTC timezone'}
 UTC = tzutc()
```

### Comparing `anvil-uplink-0.4.1/anvil/users/__init__.py` & `anvil-uplink-0.4.2/anvil/users/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 def _to_user_row(user):
     if type(user) is list:
         from anvil.tables.v2._row import Row
         user = Row._create_from_trusted(*user)
     return user
 
 def _to_row_ref(user):
-    from anvil.tables import _get_config
-    if _get_config().get("enable_v2"):
+    from anvil.tables._config import get_client_config
+    if get_client_config().get("enable_v2"):
         from anvil.tables.v2._refs import to_ref
         user = to_ref(user)
     return user
 
 #!suggestAttr(anvil.users,login_with_form)!0:
 
 #!defFunction(anvil.users,_)!2: "Forget the current logged-in user" ["logout"]
```

### Comparing `anvil-uplink-0.4.1/anvil/users/exceptions.py` & `anvil-uplink-0.4.2/anvil/users/exceptions.py`

 * *Files identical despite different names*

### Comparing `anvil-uplink-0.4.1/anvil/users/mfa/__init__.py` & `anvil-uplink-0.4.2/anvil/users/mfa/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -202,22 +202,23 @@
                 mfa_error = None
                 mfa_methods['totp'] = None
                 selected_mfa_type = 'totp'
             elif m == 'select-twilio':
                 mfa_error = None
                 mfa_methods['twilio-verify'] = None
                 selected_mfa_type = 'twilio-verify'
+            elif m == 'fido':
+                # fido is a single step process - we're done
+                return mfa_methods['fido'], password_box.text
 
             elif selected_mfa_type == 'totp':
                 if validate_totp_code(mfa_methods['totp'], totp_box.text):
                     return mfa_methods['totp'], password_box.text
                 else:
                     mfa_error = "Incorrect code entered. Please try again."
-            elif selected_mfa_type == 'fido':
-                return mfa_methods['fido'], password_box.text
             elif selected_mfa_type == 'twilio-verify':
                 mfa_error = None
                 if m == 'resend-sms':
                     channel = "sms"
                     mfa_methods['twilio-verify'] = None
                     mfa_error = "Text message resent"
                 elif m == 'call':
```

### Comparing `anvil-uplink-0.4.1/anvil/util.py` & `anvil-uplink-0.4.2/anvil/util.py`

 * *Files identical despite different names*

### Comparing `anvil-uplink-0.4.1/anvil_uplink.egg-info/PKG-INFO` & `anvil-uplink-0.4.2/anvil_uplink.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: anvil-uplink
-Version: 0.4.1
+Version: 0.4.2
 Summary: The Anvil server uplink library
 Home-page: https://anvil.works
 Author: Meredydd Luff
 Author-email: meredydd@anvil.works
 License: MIT
 Description: Anvil Server Uplink Library
```

### Comparing `anvil-uplink-0.4.1/anvil_uplink.egg-info/SOURCES.txt` & `anvil-uplink-0.4.2/anvil_uplink.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `anvil-uplink-0.4.1/setup.py` & `anvil-uplink-0.4.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 setup(
     name='anvil-uplink',
 
     # Versions should comply with PEP440.  For a discussion on single-sourcing
     # the version across setup.py and the project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
 
-    version='0.4.1',
+    version='0.4.2',
 
     description='The Anvil server uplink library',
     long_description=long_description,
 
     # The project's main homepage.
     url='https://anvil.works',
```

