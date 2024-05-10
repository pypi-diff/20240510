# Comparing `tmp/auto-test-common-2.0.4.tar.gz` & `tmp/auto-test-common-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto-test-common-2.0.4.tar", last modified: Mon May  6 02:08:03 2024, max compression
+gzip compressed data, was "auto-test-common-2.0.5.tar", last modified: Fri May 10 01:39:43 2024, max compression
```

## Comparing `auto-test-common-2.0.4.tar` & `auto-test-common-2.0.5.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-05-06 02:08:03.041325 auto-test-common-2.0.4/
--rw-r--r--   0 edz        (502) staff       (20)      628 2024-05-06 02:08:03.041437 auto-test-common-2.0.4/PKG-INFO
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-05-06 02:08:02.996030 auto-test-common-2.0.4/auto_test_common.egg-info/
--rw-r--r--   0 edz        (502) staff       (20)      628 2024-05-06 02:08:02.000000 auto-test-common-2.0.4/auto_test_common.egg-info/PKG-INFO
--rw-r--r--   0 edz        (502) staff       (20)     1821 2024-05-06 02:08:02.000000 auto-test-common-2.0.4/auto_test_common.egg-info/SOURCES.txt
--rw-r--r--   0 edz        (502) staff       (20)        1 2024-05-06 02:08:02.000000 auto-test-common-2.0.4/auto_test_common.egg-info/dependency_links.txt
--rw-r--r--   0 edz        (502) staff       (20)       57 2024-05-06 02:08:02.000000 auto-test-common-2.0.4/auto_test_common.egg-info/entry_points.txt
--rw-r--r--   0 edz        (502) staff       (20)      727 2024-05-06 02:08:02.000000 auto-test-common-2.0.4/auto_test_common.egg-info/requires.txt
--rw-r--r--   0 edz        (502) staff       (20)        7 2024-05-06 02:08:02.000000 auto-test-common-2.0.4/auto_test_common.egg-info/top_level.txt
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-05-06 02:08:02.996335 auto-test-common-2.0.4/common/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:32:00.000000 auto-test-common-2.0.4/common/__init__.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-05-06 02:08:02.999034 auto-test-common-2.0.4/common/autotest/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:59:00.000000 auto-test-common-2.0.4/common/autotest/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     5450 2024-04-24 07:01:06.000000 auto-test-common-2.0.4/common/autotest/assert_function.py
--rw-r--r--   0 edz        (502) staff       (20)    12818 2024-04-30 05:25:45.000000 auto-test-common-2.0.4/common/autotest/base_requests.py
--rw-r--r--   0 edz        (502) staff       (20)     8211 2024-04-24 05:16:27.000000 auto-test-common-2.0.4/common/autotest/handle_allure.py
--rw-r--r--   0 edz        (502) staff       (20)    14203 2024-04-24 05:16:27.000000 auto-test-common-2.0.4/common/autotest/handle_assert.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-05-06 02:08:03.001244 auto-test-common-2.0.4/common/common/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 03:00:00.000000 auto-test-common-2.0.4/common/common/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     7645 2024-04-24 05:16:27.000000 auto-test-common-2.0.4/common/common/api_driver.py
--rw-r--r--   0 edz        (502) staff       (20)     3808 2023-12-19 05:35:52.000000 auto-test-common-2.0.4/common/common/constant.py
--rw-r--r--   0 edz        (502) staff       (20)     1763 2023-04-14 00:29:00.000000 auto-test-common-2.0.4/common/common/test.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-05-06 02:08:03.002014 auto-test-common-2.0.4/common/config/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 auto-test-common-2.0.4/common/config/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     2808 2023-08-29 05:34:25.000000 auto-test-common-2.0.4/common/config/config.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-05-06 02:08:03.006135 auto-test-common-2.0.4/common/data/
--rw-r--r--   0 edz        (502) staff       (20)       28 2022-03-29 12:15:00.000000 auto-test-common-2.0.4/common/data/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)    25961 2024-04-24 05:16:27.000000 auto-test-common-2.0.4/common/data/data_process.py
--rw-r--r--   0 edz        (502) staff       (20)      426 2024-04-24 00:46:49.000000 auto-test-common-2.0.4/common/data/eval_data_handle.py
--rw-r--r--   0 edz        (502) staff       (20)     7933 2024-04-24 05:16:27.000000 auto-test-common-2.0.4/common/data/faker_handle.py
--rw-r--r--   0 edz        (502) staff       (20)    12614 2024-04-24 05:16:27.000000 auto-test-common-2.0.4/common/data/handle_common.py
--rw-r--r--   0 edz        (502) staff       (20)     3037 2023-06-12 02:50:37.000000 auto-test-common-2.0.4/common/data/template_data.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-05-06 02:08:03.010331 auto-test-common-2.0.4/common/db/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 auto-test-common-2.0.4/common/db/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     3592 2023-05-15 07:43:20.000000 auto-test-common-2.0.4/common/db/handle_db.py
--rw-r--r--   0 edz        (502) staff       (20)     1345 2022-12-13 01:35:00.000000 auto-test-common-2.0.4/common/db/handle_db_batch.py
--rw-r--r--   0 edz        (502) staff       (20)     1991 2024-04-24 00:46:49.000000 auto-test-common-2.0.4/common/db/handle_mongo.py
--rw-r--r--   0 edz        (502) staff       (20)     1223 2023-04-14 00:29:00.000000 auto-test-common-2.0.4/common/db/handle_mysqldb.py
--rw-r--r--   0 edz        (502) staff       (20)     1533 2023-04-14 00:29:00.000000 auto-test-common-2.0.4/common/db/handle_oracle.py
--rw-r--r--   0 edz        (502) staff       (20)     1665 2023-04-14 00:29:00.000000 auto-test-common-2.0.4/common/db/handle_sqlserver.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-05-06 02:08:03.012659 auto-test-common-2.0.4/common/driver/
--rw-r--r--   0 edz        (502) staff       (20)        0 2023-06-05 07:58:39.000000 auto-test-common-2.0.4/common/driver/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)      127 2023-06-05 08:02:38.000000 auto-test-common-2.0.4/common/driver/api_page.py
--rw-r--r--   0 edz        (502) staff       (20)     3037 2023-06-05 08:02:38.000000 auto-test-common-2.0.4/common/driver/ui_page.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-05-06 02:08:03.020578 auto-test-common-2.0.4/common/file/
--rw-r--r--   0 edz        (502) staff       (20)     5030 2024-04-24 05:16:27.000000 auto-test-common-2.0.4/common/file/ReadFile.py
--rw-r--r--   0 edz        (502) staff       (20)       41 2022-03-29 11:09:00.000000 auto-test-common-2.0.4/common/file/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)    10873 2024-04-24 00:46:49.000000 auto-test-common-2.0.4/common/file/handle_excel.py
--rw-r--r--   0 edz        (502) staff       (20)     2265 2023-05-25 07:52:43.000000 auto-test-common-2.0.4/common/file/handle_file.py
--rw-r--r--   0 edz        (502) staff       (20)     1364 2023-04-14 00:29:00.000000 auto-test-common-2.0.4/common/file/handle_reques.py
--rw-r--r--   0 edz        (502) staff       (20)     2360 2024-04-24 00:46:49.000000 auto-test-common-2.0.4/common/file/handle_system.py
--rw-r--r--   0 edz        (502) staff       (20)      955 2023-06-01 02:02:40.000000 auto-test-common-2.0.4/common/file/handle_yaml.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-05-06 02:08:03.021640 auto-test-common-2.0.4/common/mq/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 auto-test-common-2.0.4/common/mq/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     2059 2023-04-14 00:29:00.000000 auto-test-common-2.0.4/common/mq/handle_rabbit.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-05-06 02:08:03.032348 auto-test-common-2.0.4/common/plat/
--rw-r--r--   0 edz        (502) staff       (20)     3385 2024-01-10 05:46:42.000000 auto-test-common-2.0.4/common/plat/ATF_platform.py
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-04-16 11:02:00.000000 auto-test-common-2.0.4/common/plat/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     1384 2022-04-27 12:06:00.000000 auto-test-common-2.0.4/common/plat/jenkin_platform.py
--rw-r--r--   0 edz        (502) staff       (20)     7734 2023-11-29 00:51:05.000000 auto-test-common-2.0.4/common/plat/jira_platform.py
--rw-r--r--   0 edz        (502) staff       (20)     7268 2023-11-30 01:02:07.000000 auto-test-common-2.0.4/common/plat/mysql_platform.py
--rw-r--r--   0 edz        (502) staff       (20)    17680 2024-04-24 00:46:49.000000 auto-test-common-2.0.4/common/plat/service_platform.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-05-06 02:08:03.040718 auto-test-common-2.0.4/common/plugin/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-31 18:00:00.000000 auto-test-common-2.0.4/common/plugin/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     1527 2024-04-24 00:46:49.000000 auto-test-common-2.0.4/common/plugin/allure_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)     5156 2024-04-24 00:46:49.000000 auto-test-common-2.0.4/common/plugin/assert_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)    10554 2024-04-24 00:46:49.000000 auto-test-common-2.0.4/common/plugin/atf_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)     7770 2024-04-24 00:46:49.000000 auto-test-common-2.0.4/common/plugin/data_bus.py
--rw-r--r--   0 edz        (502) staff       (20)     5415 2024-04-24 00:46:49.000000 auto-test-common-2.0.4/common/plugin/data_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)    13056 2024-04-24 05:10:23.000000 auto-test-common-2.0.4/common/plugin/file_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)      904 2022-03-31 14:08:00.000000 auto-test-common-2.0.4/common/plugin/hooks_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)       30 2023-06-08 05:24:28.000000 auto-test-common-2.0.4/common/plugin/my_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)    13130 2023-05-31 08:41:08.000000 auto-test-common-2.0.4/common/plugin/pytest_playwright.py
--rw-r--r--   0 edz        (502) staff       (20)    23509 2024-05-06 01:03:53.000000 auto-test-common-2.0.4/common/plugin/pytest_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)     1421 2023-08-23 05:46:04.000000 auto-test-common-2.0.4/common/plugin/template_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)     2090 2024-04-24 00:46:49.000000 auto-test-common-2.0.4/common/plugin/yaml_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)      443 2024-05-06 02:08:03.042035 auto-test-common-2.0.4/setup.cfg
--rw-r--r--   0 edz        (502) staff       (20)     2101 2024-04-30 05:32:18.000000 auto-test-common-2.0.4/setup.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-05-10 01:39:43.135099 auto-test-common-2.0.5/
+-rw-r--r--   0 edz        (502) staff       (20)      628 2024-05-10 01:39:43.135267 auto-test-common-2.0.5/PKG-INFO
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-05-10 01:39:43.073640 auto-test-common-2.0.5/auto_test_common.egg-info/
+-rw-r--r--   0 edz        (502) staff       (20)      628 2024-05-10 01:39:42.000000 auto-test-common-2.0.5/auto_test_common.egg-info/PKG-INFO
+-rw-r--r--   0 edz        (502) staff       (20)     1821 2024-05-10 01:39:42.000000 auto-test-common-2.0.5/auto_test_common.egg-info/SOURCES.txt
+-rw-r--r--   0 edz        (502) staff       (20)        1 2024-05-10 01:39:42.000000 auto-test-common-2.0.5/auto_test_common.egg-info/dependency_links.txt
+-rw-r--r--   0 edz        (502) staff       (20)       57 2024-05-10 01:39:42.000000 auto-test-common-2.0.5/auto_test_common.egg-info/entry_points.txt
+-rw-r--r--   0 edz        (502) staff       (20)      727 2024-05-10 01:39:42.000000 auto-test-common-2.0.5/auto_test_common.egg-info/requires.txt
+-rw-r--r--   0 edz        (502) staff       (20)        7 2024-05-10 01:39:42.000000 auto-test-common-2.0.5/auto_test_common.egg-info/top_level.txt
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-05-10 01:39:43.074413 auto-test-common-2.0.5/common/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:32:00.000000 auto-test-common-2.0.5/common/__init__.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-05-10 01:39:43.077442 auto-test-common-2.0.5/common/autotest/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:59:00.000000 auto-test-common-2.0.5/common/autotest/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     5450 2024-04-24 07:01:06.000000 auto-test-common-2.0.5/common/autotest/assert_function.py
+-rw-r--r--   0 edz        (502) staff       (20)    12818 2024-04-30 05:25:45.000000 auto-test-common-2.0.5/common/autotest/base_requests.py
+-rw-r--r--   0 edz        (502) staff       (20)     8348 2024-05-10 01:35:28.000000 auto-test-common-2.0.5/common/autotest/handle_allure.py
+-rw-r--r--   0 edz        (502) staff       (20)    14203 2024-04-24 05:16:27.000000 auto-test-common-2.0.5/common/autotest/handle_assert.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-05-10 01:39:43.080884 auto-test-common-2.0.5/common/common/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 03:00:00.000000 auto-test-common-2.0.5/common/common/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     8052 2024-05-10 01:20:06.000000 auto-test-common-2.0.5/common/common/api_driver.py
+-rw-r--r--   0 edz        (502) staff       (20)     3808 2023-12-19 05:35:52.000000 auto-test-common-2.0.5/common/common/constant.py
+-rw-r--r--   0 edz        (502) staff       (20)     1763 2023-04-14 00:29:00.000000 auto-test-common-2.0.5/common/common/test.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-05-10 01:39:43.085472 auto-test-common-2.0.5/common/config/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 auto-test-common-2.0.5/common/config/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     2808 2023-08-29 05:34:25.000000 auto-test-common-2.0.5/common/config/config.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-05-10 01:39:43.092268 auto-test-common-2.0.5/common/data/
+-rw-r--r--   0 edz        (502) staff       (20)       28 2022-03-29 12:15:00.000000 auto-test-common-2.0.5/common/data/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)    25961 2024-04-24 05:16:27.000000 auto-test-common-2.0.5/common/data/data_process.py
+-rw-r--r--   0 edz        (502) staff       (20)      426 2024-04-24 00:46:49.000000 auto-test-common-2.0.5/common/data/eval_data_handle.py
+-rw-r--r--   0 edz        (502) staff       (20)     7933 2024-04-24 05:16:27.000000 auto-test-common-2.0.5/common/data/faker_handle.py
+-rw-r--r--   0 edz        (502) staff       (20)    12614 2024-04-24 05:16:27.000000 auto-test-common-2.0.5/common/data/handle_common.py
+-rw-r--r--   0 edz        (502) staff       (20)     3037 2023-06-12 02:50:37.000000 auto-test-common-2.0.5/common/data/template_data.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-05-10 01:39:43.097081 auto-test-common-2.0.5/common/db/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 auto-test-common-2.0.5/common/db/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     3592 2023-05-15 07:43:20.000000 auto-test-common-2.0.5/common/db/handle_db.py
+-rw-r--r--   0 edz        (502) staff       (20)     1345 2022-12-13 01:35:00.000000 auto-test-common-2.0.5/common/db/handle_db_batch.py
+-rw-r--r--   0 edz        (502) staff       (20)     1991 2024-04-24 00:46:49.000000 auto-test-common-2.0.5/common/db/handle_mongo.py
+-rw-r--r--   0 edz        (502) staff       (20)     1223 2023-04-14 00:29:00.000000 auto-test-common-2.0.5/common/db/handle_mysqldb.py
+-rw-r--r--   0 edz        (502) staff       (20)     1533 2023-04-14 00:29:00.000000 auto-test-common-2.0.5/common/db/handle_oracle.py
+-rw-r--r--   0 edz        (502) staff       (20)     1665 2023-04-14 00:29:00.000000 auto-test-common-2.0.5/common/db/handle_sqlserver.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-05-10 01:39:43.098774 auto-test-common-2.0.5/common/driver/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2023-06-05 07:58:39.000000 auto-test-common-2.0.5/common/driver/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)      127 2023-06-05 08:02:38.000000 auto-test-common-2.0.5/common/driver/api_page.py
+-rw-r--r--   0 edz        (502) staff       (20)     3037 2023-06-05 08:02:38.000000 auto-test-common-2.0.5/common/driver/ui_page.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-05-10 01:39:43.105893 auto-test-common-2.0.5/common/file/
+-rw-r--r--   0 edz        (502) staff       (20)     5030 2024-04-24 05:16:27.000000 auto-test-common-2.0.5/common/file/ReadFile.py
+-rw-r--r--   0 edz        (502) staff       (20)       41 2022-03-29 11:09:00.000000 auto-test-common-2.0.5/common/file/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)    10873 2024-04-24 00:46:49.000000 auto-test-common-2.0.5/common/file/handle_excel.py
+-rw-r--r--   0 edz        (502) staff       (20)     2265 2023-05-25 07:52:43.000000 auto-test-common-2.0.5/common/file/handle_file.py
+-rw-r--r--   0 edz        (502) staff       (20)     1364 2023-04-14 00:29:00.000000 auto-test-common-2.0.5/common/file/handle_reques.py
+-rw-r--r--   0 edz        (502) staff       (20)     2360 2024-04-24 00:46:49.000000 auto-test-common-2.0.5/common/file/handle_system.py
+-rw-r--r--   0 edz        (502) staff       (20)      955 2023-06-01 02:02:40.000000 auto-test-common-2.0.5/common/file/handle_yaml.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-05-10 01:39:43.107092 auto-test-common-2.0.5/common/mq/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 auto-test-common-2.0.5/common/mq/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     2059 2023-04-14 00:29:00.000000 auto-test-common-2.0.5/common/mq/handle_rabbit.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-05-10 01:39:43.113519 auto-test-common-2.0.5/common/plat/
+-rw-r--r--   0 edz        (502) staff       (20)     3385 2024-01-10 05:46:42.000000 auto-test-common-2.0.5/common/plat/ATF_platform.py
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-04-16 11:02:00.000000 auto-test-common-2.0.5/common/plat/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     1384 2022-04-27 12:06:00.000000 auto-test-common-2.0.5/common/plat/jenkin_platform.py
+-rw-r--r--   0 edz        (502) staff       (20)     7734 2023-11-29 00:51:05.000000 auto-test-common-2.0.5/common/plat/jira_platform.py
+-rw-r--r--   0 edz        (502) staff       (20)     7268 2023-11-30 01:02:07.000000 auto-test-common-2.0.5/common/plat/mysql_platform.py
+-rw-r--r--   0 edz        (502) staff       (20)    17680 2024-04-24 00:46:49.000000 auto-test-common-2.0.5/common/plat/service_platform.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-05-10 01:39:43.133474 auto-test-common-2.0.5/common/plugin/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-31 18:00:00.000000 auto-test-common-2.0.5/common/plugin/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     1527 2024-04-24 00:46:49.000000 auto-test-common-2.0.5/common/plugin/allure_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)     5156 2024-04-24 00:46:49.000000 auto-test-common-2.0.5/common/plugin/assert_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)    10554 2024-04-24 00:46:49.000000 auto-test-common-2.0.5/common/plugin/atf_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)     7770 2024-04-24 00:46:49.000000 auto-test-common-2.0.5/common/plugin/data_bus.py
+-rw-r--r--   0 edz        (502) staff       (20)     5415 2024-04-24 00:46:49.000000 auto-test-common-2.0.5/common/plugin/data_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)    13056 2024-04-24 05:10:23.000000 auto-test-common-2.0.5/common/plugin/file_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)      904 2022-03-31 14:08:00.000000 auto-test-common-2.0.5/common/plugin/hooks_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)       30 2023-06-08 05:24:28.000000 auto-test-common-2.0.5/common/plugin/my_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)    13130 2023-05-31 08:41:08.000000 auto-test-common-2.0.5/common/plugin/pytest_playwright.py
+-rw-r--r--   0 edz        (502) staff       (20)    23509 2024-05-06 01:03:53.000000 auto-test-common-2.0.5/common/plugin/pytest_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)     1421 2023-08-23 05:46:04.000000 auto-test-common-2.0.5/common/plugin/template_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)     2090 2024-04-24 00:46:49.000000 auto-test-common-2.0.5/common/plugin/yaml_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)      443 2024-05-10 01:39:43.137821 auto-test-common-2.0.5/setup.cfg
+-rw-r--r--   0 edz        (502) staff       (20)     2101 2024-04-30 05:32:18.000000 auto-test-common-2.0.5/setup.py
```

### Comparing `auto-test-common-2.0.4/PKG-INFO` & `auto-test-common-2.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-test-common
-Version: 2.0.4
+Version: 2.0.5
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: shiqiang.ou
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `auto-test-common-2.0.4/auto_test_common.egg-info/PKG-INFO` & `auto-test-common-2.0.5/auto_test_common.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-test-common
-Version: 2.0.4
+Version: 2.0.5
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: shiqiang.ou
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `auto-test-common-2.0.4/auto_test_common.egg-info/SOURCES.txt` & `auto-test-common-2.0.5/auto_test_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.4/auto_test_common.egg-info/requires.txt` & `auto-test-common-2.0.5/auto_test_common.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.4/common/autotest/assert_function.py` & `auto-test-common-2.0.5/common/autotest/assert_function.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.4/common/autotest/base_requests.py` & `auto-test-common-2.0.5/common/autotest/base_requests.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.4/common/autotest/handle_allure.py` & `auto-test-common-2.0.5/common/autotest/handle_allure.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,16 +61,19 @@
     :param content: 附件内容
     """
     logger.info(f'{step}:{content}')
     try:
         with allure.step(step):
             allure.attach(json.dumps(content, ensure_ascii=False, indent=4), step, allure.attachment_type.TEXT)
     except Exception as e:
-        with allure.step(step):
-            allure.attach(content, step, allure.attachment_type.TEXT)
+        try:
+            with allure.step(step):
+                allure.attach(content, step, allure.attachment_type.TEXT)
+        except Exception as e:
+            logger.warning(f'{step}:{content} 无法推送到allure中测试步骤')
 
 def screenshot(page:Page, desc:str)->None:
     """
     截图
     """
     page.screenshot(timeout=5000, path=TEST_TARGET_RESULTS_PATH)
     #把截图放入到allure
```

### Comparing `auto-test-common-2.0.4/common/autotest/handle_assert.py` & `auto-test-common-2.0.5/common/autotest/handle_assert.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.4/common/common/api_driver.py` & `auto-test-common-2.0.5/common/common/api_driver.py`

 * *Files 7% similar despite different names*

```diff
@@ -43,49 +43,49 @@
             header,header_desc = cls.getCommontHeader(header)
             res = session.request(method=method, url=url, params=data, headers=header, cookies=cookie,
                                   auth=_auth,verify=False)
             allure_api_step(desc, url, method, header_desc, data, '', res)
 
         elif parametric_key == 'data':
             header,header_desc = cls.getCommontHeader(header)
-            res = session.request(method=method, url=url, data=data, files=file, headers=header, cookies=cookie,
+            res = session.request(method=method, url=url, data=cls.dataEncode(data), files=file, headers=header, cookies=cookie,
                                   auth=_auth,verify=False)
             allure_api_step(desc, url, method, header_desc, data, file, res)
 
         elif parametric_key == 'text':
             header,header_desc = cls.getCommontHeader(header)
             header['Content-Type'] = 'text/plain'
-            res = session.request(method=method, url=url, data=data, files=file, headers=header, cookies=cookie,
+            res = session.request(method=method, url=url, data=cls.dataEncode(data), files=file, headers=header, cookies=cookie,
                                   auth=_auth, verify=False)
             allure_api_step(desc, url, method, header_desc, data, file, res)
 
         elif parametric_key == 'json':
             header,header_desc = cls.getCommontHeader(header)
             header['Content-Type'] = 'application/json'
             res = session.request(method=method, url=url, json=data, files=file, headers=header, cookies=cookie,
                                   auth=_auth,verify=False)
             allure_api_step(desc, url, method, header_desc, data, file, res)
 
         elif parametric_key == 'xml':
             header,header_desc = cls.getCommontHeader(header)
             header['Content-Type'] = 'application/xml'
-            res = session.request(method=method, url=url, data=data, files=file, headers=header, cookies=cookie,
+            res = session.request(method=method, url=url, data=cls.dataEncode(data), files=file, headers=header, cookies=cookie,
                                   auth=_auth, verify=False)
             allure_api_step(desc, url, method, header_desc, data, file, res)
 
         elif parametric_key == 'form':
             header,header_desc = cls.getCommontHeader(header)
             header['Content-Type'] = 'application/x-www-form-urlencoded'
             try:
                 if isinstance(data, str):
                     from common.data.data_process import DataProcess
                     data = DataProcess.handle_data(data)
             except Exception as e:
                 logger.info(f'测试数据：{data} 转换异常:' + repr(e))
-            res = session.request(method=method, url=url, data=data, files=file, headers=header, cookies=cookie,
+            res = session.request(method=method, url=url, data=cls.dataEncode(data), files=file, headers=header, cookies=cookie,
                                   auth=_auth, verify=False)
             allure_api_step(desc, url, method, header_desc, data, file, res)
 
         elif parametric_key == 'form-data':
             if data is not None:
                 data = cls.handleFile(data)
                 m = MultipartEncoder(data)
@@ -120,14 +120,26 @@
                 header['Accept'] = '*/*'
         header_desc = copy.copy(header)
         from common.data.data_process import DataProcess
         header = DataProcess.setDictEncode(header)
         return header, header_desc
 
     @classmethod
+    def dataEncode(self,data):
+        _data = data
+        try:
+            from common.data.data_process import DataProcess
+            if DataProcess.is_contain_chinese(_data):
+                _data = _data.encode()
+                return _data
+        except Exception as e:
+            return _data
+        return _data
+
+    @classmethod
     def handleFile(self,data):
         if isinstance(data,dict):
             for key in data:
                 if isinstance(data[key], str):
                     from common.file.handle_system import adjust_path
                     _path = adjust_path(data[key])
                     if os.path.exists(path.join(TEST_FILE_PATH, _path)):
```

### Comparing `auto-test-common-2.0.4/common/common/constant.py` & `auto-test-common-2.0.5/common/common/constant.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.4/common/common/test.py` & `auto-test-common-2.0.5/common/common/test.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.4/common/config/config.py` & `auto-test-common-2.0.5/common/config/config.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.4/common/data/data_process.py` & `auto-test-common-2.0.5/common/data/data_process.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.4/common/data/faker_handle.py` & `auto-test-common-2.0.5/common/data/faker_handle.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.4/common/data/handle_common.py` & `auto-test-common-2.0.5/common/data/handle_common.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.4/common/data/template_data.py` & `auto-test-common-2.0.5/common/data/template_data.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.4/common/db/handle_db.py` & `auto-test-common-2.0.5/common/db/handle_db.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.4/common/db/handle_db_batch.py` & `auto-test-common-2.0.5/common/db/handle_db_batch.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.4/common/db/handle_mongo.py` & `auto-test-common-2.0.5/common/db/handle_mongo.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.4/common/db/handle_mysqldb.py` & `auto-test-common-2.0.5/common/db/handle_mysqldb.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.4/common/db/handle_oracle.py` & `auto-test-common-2.0.5/common/db/handle_oracle.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.4/common/db/handle_sqlserver.py` & `auto-test-common-2.0.5/common/db/handle_sqlserver.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.4/common/driver/ui_page.py` & `auto-test-common-2.0.5/common/driver/ui_page.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.4/common/file/ReadFile.py` & `auto-test-common-2.0.5/common/file/ReadFile.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.4/common/file/handle_excel.py` & `auto-test-common-2.0.5/common/file/handle_excel.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.4/common/file/handle_file.py` & `auto-test-common-2.0.5/common/file/handle_file.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.4/common/file/handle_reques.py` & `auto-test-common-2.0.5/common/file/handle_reques.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.4/common/file/handle_system.py` & `auto-test-common-2.0.5/common/file/handle_system.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.4/common/file/handle_yaml.py` & `auto-test-common-2.0.5/common/file/handle_yaml.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.4/common/mq/handle_rabbit.py` & `auto-test-common-2.0.5/common/mq/handle_rabbit.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.4/common/plat/ATF_platform.py` & `auto-test-common-2.0.5/common/plat/ATF_platform.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.4/common/plat/jenkin_platform.py` & `auto-test-common-2.0.5/common/plat/jenkin_platform.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.4/common/plat/jira_platform.py` & `auto-test-common-2.0.5/common/plat/jira_platform.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.4/common/plat/mysql_platform.py` & `auto-test-common-2.0.5/common/plat/mysql_platform.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.4/common/plat/service_platform.py` & `auto-test-common-2.0.5/common/plat/service_platform.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.4/common/plugin/allure_plugin.py` & `auto-test-common-2.0.5/common/plugin/allure_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.4/common/plugin/assert_plugin.py` & `auto-test-common-2.0.5/common/plugin/assert_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.4/common/plugin/atf_plugin.py` & `auto-test-common-2.0.5/common/plugin/atf_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.4/common/plugin/data_bus.py` & `auto-test-common-2.0.5/common/plugin/data_bus.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.4/common/plugin/data_plugin.py` & `auto-test-common-2.0.5/common/plugin/data_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.4/common/plugin/file_plugin.py` & `auto-test-common-2.0.5/common/plugin/file_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.4/common/plugin/hooks_plugin.py` & `auto-test-common-2.0.5/common/plugin/hooks_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.4/common/plugin/pytest_playwright.py` & `auto-test-common-2.0.5/common/plugin/pytest_playwright.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.4/common/plugin/pytest_plugin.py` & `auto-test-common-2.0.5/common/plugin/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.4/common/plugin/template_plugin.py` & `auto-test-common-2.0.5/common/plugin/template_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.4/common/plugin/yaml_plugin.py` & `auto-test-common-2.0.5/common/plugin/yaml_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.4/setup.py` & `auto-test-common-2.0.5/setup.py`

 * *Files identical despite different names*

