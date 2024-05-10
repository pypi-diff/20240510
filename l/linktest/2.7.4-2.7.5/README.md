# Comparing `tmp/linktest-2.7.4.tar.gz` & `tmp/linktest-2.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linktest-2.7.4.tar", last modified: Thu May  9 08:03:31 2024, max compression
+gzip compressed data, was "linktest-2.7.5.tar", last modified: Fri May 10 05:50:58 2024, max compression
```

## Comparing `linktest-2.7.4.tar` & `linktest-2.7.5.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-05-09 08:03:31.361296 linktest-2.7.4/
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      111 2024-05-09 08:03:31.361001 linktest-2.7.4/PKG-INFO
-drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-05-09 08:03:31.353958 linktest-2.7.4/linktest/
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       22 2024-05-09 07:52:53.000000 linktest-2.7.4/linktest/__init__.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      487 2024-05-08 17:38:13.000000 linktest-2.7.4/linktest/android_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      187 2024-05-08 17:38:13.000000 linktest-2.7.4/linktest/api_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10759 2024-05-08 17:38:13.000000 linktest-2.7.4/linktest/appium_utils.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    29054 2024-05-08 17:38:13.000000 linktest-2.7.4/linktest/auto_generate_testcase_list.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10302 2024-05-08 17:38:13.000000 linktest-2.7.4/linktest/auto_generate_testcase_list_from_csv.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     9984 2024-05-08 17:38:13.000000 linktest-2.7.4/linktest/base_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1792 2024-05-08 17:38:13.000000 linktest-2.7.4/linktest/clean_data.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1403 2024-05-08 17:38:13.000000 linktest-2.7.4/linktest/conver_xml_into_db.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     7260 2024-05-08 17:38:13.000000 linktest-2.7.4/linktest/database_helper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2471 2024-05-08 17:38:13.000000 linktest-2.7.4/linktest/date_utilities.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      232 2024-05-08 17:38:13.000000 linktest-2.7.4/linktest/detect_delimiter.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    16684 2024-05-08 17:38:13.000000 linktest-2.7.4/linktest/doctor.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      959 2024-05-08 17:38:13.000000 linktest-2.7.4/linktest/framework_log.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    16093 2024-05-08 17:38:13.000000 linktest-2.7.4/linktest/generate_html_log.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      987 2024-05-08 17:38:13.000000 linktest-2.7.4/linktest/get_adb_devices.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      924 2024-05-08 17:38:13.000000 linktest-2.7.4/linktest/get_ios_devices_list.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1775 2024-05-08 17:38:13.000000 linktest-2.7.4/linktest/get_platform_info.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3137 2024-05-08 17:38:13.000000 linktest-2.7.4/linktest/get_project_info.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    33114 2024-05-09 07:56:31.000000 linktest-2.7.4/linktest/html_report.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      280 2024-05-08 17:38:13.000000 linktest-2.7.4/linktest/ios_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      195 2024-05-08 17:38:13.000000 linktest-2.7.4/linktest/linktest_setup.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     8745 2024-05-08 17:38:13.000000 linktest-2.7.4/linktest/logged_requests.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)   102428 2024-05-09 07:56:13.000000 linktest-2.7.4/linktest/main.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      982 2024-05-08 17:38:13.000000 linktest-2.7.4/linktest/memory_usage.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     4526 2024-05-08 17:38:13.000000 linktest-2.7.4/linktest/re_func.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1334 2024-05-08 17:38:13.000000 linktest-2.7.4/linktest/run.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2188 2024-05-08 17:38:13.000000 linktest-2.7.4/linktest/run_testcase_thread.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1048 2024-05-08 17:38:13.000000 linktest-2.7.4/linktest/scp_report_to_specified_path.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     9534 2024-05-08 18:03:39.000000 linktest-2.7.4/linktest/selenium_helper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      396 2024-05-08 17:38:13.000000 linktest-2.7.4/linktest/set_run_flag_thread.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      452 2024-05-09 07:53:03.000000 linktest-2.7.4/linktest/setup.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      173 2024-05-08 17:38:13.000000 linktest-2.7.4/linktest/testcase_order.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      140 2024-05-08 17:38:13.000000 linktest-2.7.4/linktest/testcase_timeout_exception.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      801 2024-05-08 17:38:13.000000 linktest-2.7.4/linktest/timeout_thread.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      931 2024-05-08 17:38:13.000000 linktest-2.7.4/linktest/ui_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3445 2024-05-08 17:38:13.000000 linktest-2.7.4/linktest/update_config.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    14288 2024-05-08 17:38:13.000000 linktest-2.7.4/linktest/webdriver_wrapper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    14075 2024-05-08 17:44:11.000000 linktest-2.7.4/linktest/webdriver_wrapper_chrome.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    13707 2024-05-08 17:38:13.000000 linktest-2.7.4/linktest/webdriver_wrapper_edge.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    13725 2024-05-08 17:38:13.000000 linktest-2.7.4/linktest/webdriver_wrapper_firefox.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    13695 2024-05-08 17:38:13.000000 linktest-2.7.4/linktest/webdriver_wrapper_ie.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    14139 2024-05-08 17:38:13.000000 linktest-2.7.4/linktest/webdriver_wrapper_safari.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      406 2024-05-08 17:38:13.000000 linktest-2.7.4/linktest/windows_helper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3544 2024-05-08 17:38:13.000000 linktest-2.7.4/linktest/xml_report.py
-drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-05-09 08:03:31.360617 linktest-2.7.4/linktest.egg-info/
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      111 2024-05-09 08:03:30.000000 linktest-2.7.4/linktest.egg-info/PKG-INFO
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1451 2024-05-09 08:03:30.000000 linktest-2.7.4/linktest.egg-info/SOURCES.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        1 2024-05-09 08:03:30.000000 linktest-2.7.4/linktest.egg-info/dependency_links.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      123 2024-05-09 08:03:30.000000 linktest-2.7.4/linktest.egg-info/requires.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        9 2024-05-09 08:03:30.000000 linktest-2.7.4/linktest.egg-info/top_level.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       38 2024-05-09 08:03:31.361343 linktest-2.7.4/setup.cfg
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      452 2024-05-09 08:03:25.000000 linktest-2.7.4/setup.py
+drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-05-10 05:50:58.554946 linktest-2.7.5/
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      111 2024-05-10 05:50:58.554713 linktest-2.7.5/PKG-INFO
+drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-05-10 05:50:58.552763 linktest-2.7.5/linktest/
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       22 2024-05-09 09:24:03.000000 linktest-2.7.5/linktest/__init__.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      487 2024-05-09 08:21:46.000000 linktest-2.7.5/linktest/android_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      187 2024-05-09 08:21:46.000000 linktest-2.7.5/linktest/api_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10759 2024-05-09 08:21:46.000000 linktest-2.7.5/linktest/appium_utils.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    29054 2024-05-09 08:21:46.000000 linktest-2.7.5/linktest/auto_generate_testcase_list.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10302 2024-05-09 08:21:46.000000 linktest-2.7.5/linktest/auto_generate_testcase_list_from_csv.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     9984 2024-05-09 08:21:46.000000 linktest-2.7.5/linktest/base_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1792 2024-05-09 08:21:46.000000 linktest-2.7.5/linktest/clean_data.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1403 2024-05-09 08:21:46.000000 linktest-2.7.5/linktest/conver_xml_into_db.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     7260 2024-05-09 08:21:46.000000 linktest-2.7.5/linktest/database_helper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2471 2024-05-09 08:21:46.000000 linktest-2.7.5/linktest/date_utilities.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      232 2024-05-09 08:21:46.000000 linktest-2.7.5/linktest/detect_delimiter.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    16684 2024-05-09 08:21:46.000000 linktest-2.7.5/linktest/doctor.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      959 2024-05-09 08:21:46.000000 linktest-2.7.5/linktest/framework_log.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    16093 2024-05-09 08:21:46.000000 linktest-2.7.5/linktest/generate_html_log.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      987 2024-05-09 08:21:46.000000 linktest-2.7.5/linktest/get_adb_devices.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      924 2024-05-09 08:21:46.000000 linktest-2.7.5/linktest/get_ios_devices_list.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1775 2024-05-09 08:21:46.000000 linktest-2.7.5/linktest/get_platform_info.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3137 2024-05-09 08:21:46.000000 linktest-2.7.5/linktest/get_project_info.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    33114 2024-05-09 08:21:46.000000 linktest-2.7.5/linktest/html_report.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      280 2024-05-09 08:21:46.000000 linktest-2.7.5/linktest/ios_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      195 2024-05-09 08:21:46.000000 linktest-2.7.5/linktest/linktest_setup.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     8676 2024-05-09 09:18:55.000000 linktest-2.7.5/linktest/logged_requests.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)   103040 2024-05-09 09:23:33.000000 linktest-2.7.5/linktest/main.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      982 2024-05-09 08:21:46.000000 linktest-2.7.5/linktest/memory_usage.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     4526 2024-05-09 08:21:46.000000 linktest-2.7.5/linktest/re_func.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1334 2024-05-09 08:21:46.000000 linktest-2.7.5/linktest/run.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2188 2024-05-09 08:21:46.000000 linktest-2.7.5/linktest/run_testcase_thread.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1048 2024-05-09 08:21:46.000000 linktest-2.7.5/linktest/scp_report_to_specified_path.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     9534 2024-05-09 08:21:46.000000 linktest-2.7.5/linktest/selenium_helper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      396 2024-05-09 08:21:46.000000 linktest-2.7.5/linktest/set_run_flag_thread.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      452 2024-05-09 09:24:08.000000 linktest-2.7.5/linktest/setup.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      173 2024-05-09 08:21:46.000000 linktest-2.7.5/linktest/testcase_order.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      140 2024-05-09 08:21:46.000000 linktest-2.7.5/linktest/testcase_timeout_exception.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      801 2024-05-09 08:21:46.000000 linktest-2.7.5/linktest/timeout_thread.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      931 2024-05-09 08:21:46.000000 linktest-2.7.5/linktest/ui_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3445 2024-05-09 08:21:46.000000 linktest-2.7.5/linktest/update_config.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    14288 2024-05-09 08:21:46.000000 linktest-2.7.5/linktest/webdriver_wrapper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    14075 2024-05-09 08:21:46.000000 linktest-2.7.5/linktest/webdriver_wrapper_chrome.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    13707 2024-05-09 08:21:46.000000 linktest-2.7.5/linktest/webdriver_wrapper_edge.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    13725 2024-05-09 08:21:46.000000 linktest-2.7.5/linktest/webdriver_wrapper_firefox.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    13695 2024-05-09 08:21:46.000000 linktest-2.7.5/linktest/webdriver_wrapper_ie.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    14139 2024-05-09 08:21:46.000000 linktest-2.7.5/linktest/webdriver_wrapper_safari.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      406 2024-05-09 08:21:46.000000 linktest-2.7.5/linktest/windows_helper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3544 2024-05-09 08:21:46.000000 linktest-2.7.5/linktest/xml_report.py
+drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-05-10 05:50:58.554427 linktest-2.7.5/linktest.egg-info/
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      111 2024-05-10 05:50:58.000000 linktest-2.7.5/linktest.egg-info/PKG-INFO
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1451 2024-05-10 05:50:58.000000 linktest-2.7.5/linktest.egg-info/SOURCES.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        1 2024-05-10 05:50:58.000000 linktest-2.7.5/linktest.egg-info/dependency_links.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      123 2024-05-10 05:50:58.000000 linktest-2.7.5/linktest.egg-info/requires.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        9 2024-05-10 05:50:58.000000 linktest-2.7.5/linktest.egg-info/top_level.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       38 2024-05-10 05:50:58.555004 linktest-2.7.5/setup.cfg
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      452 2024-05-10 05:50:52.000000 linktest-2.7.5/setup.py
```

### Comparing `linktest-2.7.4/linktest/appium_utils.py` & `linktest-2.7.5/linktest/appium_utils.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.4/linktest/auto_generate_testcase_list.py` & `linktest-2.7.5/linktest/auto_generate_testcase_list.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.4/linktest/auto_generate_testcase_list_from_csv.py` & `linktest-2.7.5/linktest/auto_generate_testcase_list_from_csv.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.4/linktest/base_testcase.py` & `linktest-2.7.5/linktest/base_testcase.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.4/linktest/clean_data.py` & `linktest-2.7.5/linktest/clean_data.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.4/linktest/conver_xml_into_db.py` & `linktest-2.7.5/linktest/conver_xml_into_db.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.4/linktest/database_helper.py` & `linktest-2.7.5/linktest/database_helper.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.4/linktest/date_utilities.py` & `linktest-2.7.5/linktest/date_utilities.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.4/linktest/doctor.py` & `linktest-2.7.5/linktest/doctor.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.4/linktest/framework_log.py` & `linktest-2.7.5/linktest/framework_log.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.4/linktest/generate_html_log.py` & `linktest-2.7.5/linktest/generate_html_log.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.4/linktest/get_adb_devices.py` & `linktest-2.7.5/linktest/get_adb_devices.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.4/linktest/get_ios_devices_list.py` & `linktest-2.7.5/linktest/get_ios_devices_list.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.4/linktest/get_platform_info.py` & `linktest-2.7.5/linktest/get_platform_info.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.4/linktest/get_project_info.py` & `linktest-2.7.5/linktest/get_project_info.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.4/linktest/html_report.py` & `linktest-2.7.5/linktest/html_report.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.4/linktest/logged_requests.py` & `linktest-2.7.5/linktest/logged_requests.py`

 * *Files 4% similar despite different names*

```diff
@@ -85,16 +85,16 @@
 
             return res
 
         return wrapper
 
     @log_curl
     def get(self, url, params=None, **kwargs):
-        if hasattr(settings, "auto_log_request") and settings.auto_log_request is False:
-            return requests.get(url, params, **kwargs)
+        if not getattr(settings, "AUTO_LOG_HTTP_REQUEST", True):
+            return requests.post(url, data, json, **kwargs)
 
         self.logger.info(">>>>>>>>>>>>>>>>>>>>>>>>> GET Request Started >>>>>>>>>>>>>>>>>>>>>>>>>")
         self.logger.info("URL: " + url)
 
         if params is not None:
             self.logger.info("params: " + pformat(params))
 
@@ -118,16 +118,16 @@
 
         self.logger.info("<<<<<<<<<<<<<<<<<<<<<<<<< GET Request Completed <<<<<<<<<<<<<<<<<<<<<<<<<" + os.linesep)
 
         return response
 
     @log_curl
     def post(self, url, data=None, json=None, **kwargs):
-        #  为了 不重复记录 log,则 增加如下判断， 如果 settings.auto_log_request = False, 则不需要框架自动记录log!
-        if hasattr(settings, "auto_log_request") and settings.auto_log_request is False:
+        #  为了 不重复记录 log,则 增加如下判断， 如果 settings.AUTO_LOG_HTTP_REQUEST = False, 则不需要框架自动记录log!
+        if not getattr(settings, "AUTO_LOG_HTTP_REQUEST", True):
             return requests.post(url, data, json, **kwargs)
 
         self.logger.info(">>>>>>>>>>>>>>>>>>>>>>>>> POST Request Started >>>>>>>>>>>>>>>>>>>>>>>>>")
         self.logger.info("URL: " + url)
 
         if data is not None:
             self.logger.info("POST DATA:")
@@ -166,16 +166,16 @@
 
         self.logger.info("<<<<<<<<<<<<<<<<<<<<<<<<< POST Request Completed <<<<<<<<<<<<<<<<<<<<<<<<<" + os.linesep)
 
         return response
 
     @log_curl
     def put(self, url, data=None, **kwargs):
-        if hasattr(settings, "auto_log_request") and settings.auto_log_request is False:
-            return requests.put(url, data, **kwargs)
+        if not getattr(settings, "AUTO_LOG_HTTP_REQUEST", True):
+            return requests.post(url, data, json, **kwargs)
 
         self.logger.info(">>>>>>>>>>>>>>>>>>>>>>>>> PUT Request Start >>>>>>>>>>>>>>>>>>>>>>>>>" + os.linesep)
         self.logger.info("URL: " + url)
 
         if data is not None:
             try:
                 self.logger.info("data: " + os.linesep + pformat(json_func.loads(data)))
@@ -198,16 +198,16 @@
 
         self.logger.info("<<<<<<<<<<<<<<<<<<<<<<<<< PUT Request Completed <<<<<<<<<<<<<<<<<<<<<<<<<" + os.linesep)
 
         return response
 
     @log_curl
     def delete(self, url, **kwargs):
-        if hasattr(settings, "auto_log_request") and settings.auto_log_request is False:
-            return requests.delete(url, **kwargs)
+        if not getattr(settings, "AUTO_LOG_HTTP_REQUEST", True):
+            return requests.post(url, data, json, **kwargs)
 
         self.logger.info(">>>>>>>>>>>>>>>>>>>>>>>>> DELETE Request Start >>>>>>>>>>>>>>>>>>>>>>>>>" + os.linesep)
         self.logger.info("URL: " + url)
 
         if len(kwargs.keys()) > 0:
             self.logger.info("kwargs: " + os.linesep + json_func.dumps(kwargs, ensure_ascii=False, indent=2))
```

### Comparing `linktest-2.7.4/linktest/main.py` & `linktest-2.7.5/linktest/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,16 +29,22 @@
     - TESTCASE_TIMEOUT (if a test case's execution is not complete after Testcase_Timeout seconds, a TimeoutException will be thrown)
     - RERUN_FLAG (controls rerunning of failed test cases; default is False)
     - DEBUG_RUN (keeps the browser active after execution is done; default value is False)
     - Show_All_Chrome_Driver_Logs (determines whether to show all webdriver logs; default value is False)
     - QUEUE_SIZE (setting queue_size to 8, for example, means that a maximum of 8 test cases can be executed concurrently)
     - SAVE_LOG_TO_DB (saves execution logs into testdb; must be used in conjunction with linktest-dashboard)
     - generate_xunit_result (saves xunit report; default value is False; used for TestLink integration)
-    - auto_log_request (default value is True; automatically logs request actions)
+    - AUTO_LOG_HTTP_REQUEST (default value is True; automatically logs request actions)
     - AUTO_DOWNLOAD_CHROMEDRIVER (default value is False; automatically downloads the appropriate Chromedriver based on the Chrome version)
+    - AUTO_SCREENSHOT_ON_ACTION (default value is False; automatically generates a screenshot for each WebDriver action)
+    - DEFAULT_BROWSER_NAME (default browser name for UI test cases; default value is "chrome")
+    - HEAD_LESS (default value is False; runs the browser in headless mode)
+    - WEBDRIVER_IMPLICIT_WAIT (default value is 10 seconds; maximum time the WebDriver should wait for an element to be present before throwing an exception)
+    - LOG_TO_CONSOLE (default value is True; always logs to the console)
+    - ALWAYS_GENERATE_CURL (default value is False; always generates cURL commands)
 
     # ------ Configuration Related to the TestCase's Log ------
     - LOG_FORMAT = '[%(asctime)s] %(levelname)-8s %(name)-12s %(message)s'
     - LOG_LEVEL = logging.DEBUG # default value is DEBUG
     - LOG_TO_CONSOLE = True # default value is True, Always log to file
 
 2. settings/testcase_tags.py
```

### Comparing `linktest-2.7.4/linktest/memory_usage.py` & `linktest-2.7.5/linktest/memory_usage.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.4/linktest/re_func.py` & `linktest-2.7.5/linktest/re_func.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.4/linktest/run.py` & `linktest-2.7.5/linktest/run.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.4/linktest/run_testcase_thread.py` & `linktest-2.7.5/linktest/run_testcase_thread.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.4/linktest/scp_report_to_specified_path.py` & `linktest-2.7.5/linktest/scp_report_to_specified_path.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.4/linktest/selenium_helper.py` & `linktest-2.7.5/linktest/selenium_helper.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.4/linktest/timeout_thread.py` & `linktest-2.7.5/linktest/timeout_thread.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.4/linktest/ui_testcase.py` & `linktest-2.7.5/linktest/ui_testcase.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.4/linktest/update_config.py` & `linktest-2.7.5/linktest/update_config.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.4/linktest/webdriver_wrapper.py` & `linktest-2.7.5/linktest/webdriver_wrapper.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.4/linktest/webdriver_wrapper_chrome.py` & `linktest-2.7.5/linktest/webdriver_wrapper_chrome.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.4/linktest/webdriver_wrapper_edge.py` & `linktest-2.7.5/linktest/webdriver_wrapper_edge.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.4/linktest/webdriver_wrapper_firefox.py` & `linktest-2.7.5/linktest/webdriver_wrapper_firefox.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.4/linktest/webdriver_wrapper_ie.py` & `linktest-2.7.5/linktest/webdriver_wrapper_ie.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.4/linktest/webdriver_wrapper_safari.py` & `linktest-2.7.5/linktest/webdriver_wrapper_safari.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.4/linktest/xml_report.py` & `linktest-2.7.5/linktest/xml_report.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.4/linktest.egg-info/SOURCES.txt` & `linktest-2.7.5/linktest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

