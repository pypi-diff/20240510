# Comparing `tmp/linktest-2.7.3.tar.gz` & `tmp/linktest-2.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linktest-2.7.3.tar", last modified: Mon May  6 08:54:39 2024, max compression
+gzip compressed data, was "linktest-2.7.4.tar", last modified: Thu May  9 08:03:31 2024, max compression
```

## Comparing `linktest-2.7.3.tar` & `linktest-2.7.4.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-05-06 08:54:39.464648 linktest-2.7.3/
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      111 2024-05-06 08:54:39.464359 linktest-2.7.3/PKG-INFO
-drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-05-06 08:54:39.461789 linktest-2.7.3/linktest/
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       22 2024-05-06 08:52:28.000000 linktest-2.7.3/linktest/__init__.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      487 2024-05-06 08:28:06.000000 linktest-2.7.3/linktest/android_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      187 2024-05-06 08:28:06.000000 linktest-2.7.3/linktest/api_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10759 2024-05-06 08:28:06.000000 linktest-2.7.3/linktest/appium_utils.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    29054 2024-05-06 08:28:06.000000 linktest-2.7.3/linktest/auto_generate_testcase_list.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10302 2024-05-06 08:28:06.000000 linktest-2.7.3/linktest/auto_generate_testcase_list_from_csv.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     9984 2024-05-06 08:28:06.000000 linktest-2.7.3/linktest/base_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1792 2024-05-06 08:28:06.000000 linktest-2.7.3/linktest/clean_data.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1403 2024-05-06 08:28:06.000000 linktest-2.7.3/linktest/conver_xml_into_db.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     7260 2024-05-06 08:28:06.000000 linktest-2.7.3/linktest/database_helper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2471 2024-05-06 08:28:06.000000 linktest-2.7.3/linktest/date_utilities.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      232 2024-05-06 08:28:06.000000 linktest-2.7.3/linktest/detect_delimiter.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    16684 2024-05-06 08:28:06.000000 linktest-2.7.3/linktest/doctor.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      959 2024-05-06 08:28:06.000000 linktest-2.7.3/linktest/framework_log.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    16093 2024-05-06 08:45:55.000000 linktest-2.7.3/linktest/generate_html_log.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      987 2024-05-06 08:28:06.000000 linktest-2.7.3/linktest/get_adb_devices.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      924 2024-05-06 08:28:06.000000 linktest-2.7.3/linktest/get_ios_devices_list.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1775 2024-05-06 08:28:06.000000 linktest-2.7.3/linktest/get_platform_info.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3137 2024-05-06 08:28:06.000000 linktest-2.7.3/linktest/get_project_info.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    33518 2024-05-06 08:28:06.000000 linktest-2.7.3/linktest/html_report.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      280 2024-05-06 08:28:06.000000 linktest-2.7.3/linktest/ios_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      195 2024-05-06 08:28:06.000000 linktest-2.7.3/linktest/linktest_setup.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     8745 2024-05-06 08:28:06.000000 linktest-2.7.3/linktest/logged_requests.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)   103054 2024-05-06 08:28:06.000000 linktest-2.7.3/linktest/main.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      982 2024-05-06 08:28:06.000000 linktest-2.7.3/linktest/memory_usage.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     4526 2024-05-06 08:28:06.000000 linktest-2.7.3/linktest/re_func.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1334 2024-05-06 08:28:06.000000 linktest-2.7.3/linktest/run.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2188 2024-05-06 08:28:06.000000 linktest-2.7.3/linktest/run_testcase_thread.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1048 2024-05-06 08:28:06.000000 linktest-2.7.3/linktest/scp_report_to_specified_path.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     9459 2024-05-06 08:51:29.000000 linktest-2.7.3/linktest/selenium_helper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      396 2024-05-06 08:28:06.000000 linktest-2.7.3/linktest/set_run_flag_thread.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      452 2024-05-06 08:52:23.000000 linktest-2.7.3/linktest/setup.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      173 2024-05-06 08:28:06.000000 linktest-2.7.3/linktest/testcase_order.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      140 2024-05-06 08:28:06.000000 linktest-2.7.3/linktest/testcase_timeout_exception.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      801 2024-05-06 08:28:06.000000 linktest-2.7.3/linktest/timeout_thread.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      931 2024-05-06 08:28:06.000000 linktest-2.7.3/linktest/ui_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3445 2024-05-06 08:28:06.000000 linktest-2.7.3/linktest/update_config.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    14288 2024-05-06 08:28:06.000000 linktest-2.7.3/linktest/webdriver_wrapper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    13936 2024-05-06 08:28:06.000000 linktest-2.7.3/linktest/webdriver_wrapper_chrome.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    13707 2024-05-06 08:28:06.000000 linktest-2.7.3/linktest/webdriver_wrapper_edge.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    13725 2024-05-06 08:28:06.000000 linktest-2.7.3/linktest/webdriver_wrapper_firefox.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    13695 2024-05-06 08:28:06.000000 linktest-2.7.3/linktest/webdriver_wrapper_ie.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    14139 2024-05-06 08:28:06.000000 linktest-2.7.3/linktest/webdriver_wrapper_safari.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      406 2024-05-06 08:28:06.000000 linktest-2.7.3/linktest/windows_helper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3544 2024-05-06 08:28:06.000000 linktest-2.7.3/linktest/xml_report.py
-drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-05-06 08:54:39.463945 linktest-2.7.3/linktest.egg-info/
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      111 2024-05-06 08:54:39.000000 linktest-2.7.3/linktest.egg-info/PKG-INFO
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1451 2024-05-06 08:54:39.000000 linktest-2.7.3/linktest.egg-info/SOURCES.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        1 2024-05-06 08:54:39.000000 linktest-2.7.3/linktest.egg-info/dependency_links.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      123 2024-05-06 08:54:39.000000 linktest-2.7.3/linktest.egg-info/requires.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        9 2024-05-06 08:54:39.000000 linktest-2.7.3/linktest.egg-info/top_level.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       38 2024-05-06 08:54:39.464711 linktest-2.7.3/setup.cfg
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      452 2024-05-06 08:54:32.000000 linktest-2.7.3/setup.py
+drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-05-09 08:03:31.361296 linktest-2.7.4/
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      111 2024-05-09 08:03:31.361001 linktest-2.7.4/PKG-INFO
+drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-05-09 08:03:31.353958 linktest-2.7.4/linktest/
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       22 2024-05-09 07:52:53.000000 linktest-2.7.4/linktest/__init__.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      487 2024-05-08 17:38:13.000000 linktest-2.7.4/linktest/android_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      187 2024-05-08 17:38:13.000000 linktest-2.7.4/linktest/api_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10759 2024-05-08 17:38:13.000000 linktest-2.7.4/linktest/appium_utils.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    29054 2024-05-08 17:38:13.000000 linktest-2.7.4/linktest/auto_generate_testcase_list.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10302 2024-05-08 17:38:13.000000 linktest-2.7.4/linktest/auto_generate_testcase_list_from_csv.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     9984 2024-05-08 17:38:13.000000 linktest-2.7.4/linktest/base_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1792 2024-05-08 17:38:13.000000 linktest-2.7.4/linktest/clean_data.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1403 2024-05-08 17:38:13.000000 linktest-2.7.4/linktest/conver_xml_into_db.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     7260 2024-05-08 17:38:13.000000 linktest-2.7.4/linktest/database_helper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2471 2024-05-08 17:38:13.000000 linktest-2.7.4/linktest/date_utilities.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      232 2024-05-08 17:38:13.000000 linktest-2.7.4/linktest/detect_delimiter.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    16684 2024-05-08 17:38:13.000000 linktest-2.7.4/linktest/doctor.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      959 2024-05-08 17:38:13.000000 linktest-2.7.4/linktest/framework_log.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    16093 2024-05-08 17:38:13.000000 linktest-2.7.4/linktest/generate_html_log.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      987 2024-05-08 17:38:13.000000 linktest-2.7.4/linktest/get_adb_devices.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      924 2024-05-08 17:38:13.000000 linktest-2.7.4/linktest/get_ios_devices_list.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1775 2024-05-08 17:38:13.000000 linktest-2.7.4/linktest/get_platform_info.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3137 2024-05-08 17:38:13.000000 linktest-2.7.4/linktest/get_project_info.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    33114 2024-05-09 07:56:31.000000 linktest-2.7.4/linktest/html_report.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      280 2024-05-08 17:38:13.000000 linktest-2.7.4/linktest/ios_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      195 2024-05-08 17:38:13.000000 linktest-2.7.4/linktest/linktest_setup.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     8745 2024-05-08 17:38:13.000000 linktest-2.7.4/linktest/logged_requests.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)   102428 2024-05-09 07:56:13.000000 linktest-2.7.4/linktest/main.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      982 2024-05-08 17:38:13.000000 linktest-2.7.4/linktest/memory_usage.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     4526 2024-05-08 17:38:13.000000 linktest-2.7.4/linktest/re_func.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1334 2024-05-08 17:38:13.000000 linktest-2.7.4/linktest/run.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2188 2024-05-08 17:38:13.000000 linktest-2.7.4/linktest/run_testcase_thread.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1048 2024-05-08 17:38:13.000000 linktest-2.7.4/linktest/scp_report_to_specified_path.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     9534 2024-05-08 18:03:39.000000 linktest-2.7.4/linktest/selenium_helper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      396 2024-05-08 17:38:13.000000 linktest-2.7.4/linktest/set_run_flag_thread.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      452 2024-05-09 07:53:03.000000 linktest-2.7.4/linktest/setup.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      173 2024-05-08 17:38:13.000000 linktest-2.7.4/linktest/testcase_order.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      140 2024-05-08 17:38:13.000000 linktest-2.7.4/linktest/testcase_timeout_exception.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      801 2024-05-08 17:38:13.000000 linktest-2.7.4/linktest/timeout_thread.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      931 2024-05-08 17:38:13.000000 linktest-2.7.4/linktest/ui_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3445 2024-05-08 17:38:13.000000 linktest-2.7.4/linktest/update_config.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    14288 2024-05-08 17:38:13.000000 linktest-2.7.4/linktest/webdriver_wrapper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    14075 2024-05-08 17:44:11.000000 linktest-2.7.4/linktest/webdriver_wrapper_chrome.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    13707 2024-05-08 17:38:13.000000 linktest-2.7.4/linktest/webdriver_wrapper_edge.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    13725 2024-05-08 17:38:13.000000 linktest-2.7.4/linktest/webdriver_wrapper_firefox.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    13695 2024-05-08 17:38:13.000000 linktest-2.7.4/linktest/webdriver_wrapper_ie.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    14139 2024-05-08 17:38:13.000000 linktest-2.7.4/linktest/webdriver_wrapper_safari.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      406 2024-05-08 17:38:13.000000 linktest-2.7.4/linktest/windows_helper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3544 2024-05-08 17:38:13.000000 linktest-2.7.4/linktest/xml_report.py
+drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-05-09 08:03:31.360617 linktest-2.7.4/linktest.egg-info/
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      111 2024-05-09 08:03:30.000000 linktest-2.7.4/linktest.egg-info/PKG-INFO
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1451 2024-05-09 08:03:30.000000 linktest-2.7.4/linktest.egg-info/SOURCES.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        1 2024-05-09 08:03:30.000000 linktest-2.7.4/linktest.egg-info/dependency_links.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      123 2024-05-09 08:03:30.000000 linktest-2.7.4/linktest.egg-info/requires.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        9 2024-05-09 08:03:30.000000 linktest-2.7.4/linktest.egg-info/top_level.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       38 2024-05-09 08:03:31.361343 linktest-2.7.4/setup.cfg
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      452 2024-05-09 08:03:25.000000 linktest-2.7.4/setup.py
```

### Comparing `linktest-2.7.3/linktest/appium_utils.py` & `linktest-2.7.4/linktest/appium_utils.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.3/linktest/auto_generate_testcase_list.py` & `linktest-2.7.4/linktest/auto_generate_testcase_list.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.3/linktest/auto_generate_testcase_list_from_csv.py` & `linktest-2.7.4/linktest/auto_generate_testcase_list_from_csv.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.3/linktest/base_testcase.py` & `linktest-2.7.4/linktest/base_testcase.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.3/linktest/clean_data.py` & `linktest-2.7.4/linktest/clean_data.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.3/linktest/conver_xml_into_db.py` & `linktest-2.7.4/linktest/conver_xml_into_db.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.3/linktest/database_helper.py` & `linktest-2.7.4/linktest/database_helper.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.3/linktest/date_utilities.py` & `linktest-2.7.4/linktest/date_utilities.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.3/linktest/doctor.py` & `linktest-2.7.4/linktest/doctor.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.3/linktest/framework_log.py` & `linktest-2.7.4/linktest/framework_log.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.3/linktest/generate_html_log.py` & `linktest-2.7.4/linktest/generate_html_log.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.3/linktest/get_adb_devices.py` & `linktest-2.7.4/linktest/get_adb_devices.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.3/linktest/get_ios_devices_list.py` & `linktest-2.7.4/linktest/get_ios_devices_list.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.3/linktest/get_platform_info.py` & `linktest-2.7.4/linktest/get_platform_info.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.3/linktest/get_project_info.py` & `linktest-2.7.4/linktest/get_project_info.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.3/linktest/html_report.py` & `linktest-2.7.4/linktest/html_report.py`

 * *Files 2% similar despite different names*

```diff
@@ -451,33 +451,31 @@
                         report_file_handler.write(
                             " <a title='%s'> (" % 'Please see the execution logs for more details' + failed_testcase.exception_info + ") </a>")
                     except BaseException:
                         print(traceback.format_exc())
 
                     if failed_testcase.rerun_tag == 0:
                         try:
-                            if getattr(settings, 'LOG_TO_FILE', True):
-                                report_file_handler.write(
-                                    "&nbsp; &nbsp; <strong style='color: #555555; '>Log Files: </strong><a target='_blank' style='white-space: nowrap;' data-bs-toggle='tooltip' data-bs-placement='right' title='View Detailed Log' href='%s'><font style='color: red'> &nbsp;[TXT </font></a>" %
-                                    failed_testcase.log_file_path)
-                                report_file_handler.write(
-                                    " | <a target='_blank' style='white-space: nowrap;' data-bs-toggle='tooltip' data-bs-placement='right' title='View Detailed Log' href='%s'><font style='color: red'> HTML]</font></a>" %
-                                    failed_testcase.log_file_path.replace("test.log", "test.html"))
+                            report_file_handler.write(
+                                "&nbsp; &nbsp; <strong style='color: #555555; '>Log Files: </strong><a target='_blank' style='white-space: nowrap;' data-bs-toggle='tooltip' data-bs-placement='right' title='View Detailed Log' href='%s'><font style='color: red'> &nbsp;[TXT </font></a>" %
+                                failed_testcase.log_file_path)
+                            report_file_handler.write(
+                                " | <a target='_blank' style='white-space: nowrap;' data-bs-toggle='tooltip' data-bs-placement='right' title='View Detailed Log' href='%s'><font style='color: red'> HTML]</font></a>" %
+                                failed_testcase.log_file_path.replace("test.log", "test.html"))
                         except BaseException:
                             print(traceback.format_exc())
 
                     elif failed_testcase.rerun_tag == 1:
                         try:
-                            if getattr(settings, 'LOG_TO_FILE', True):
-                                report_file_handler.write(
-                                    "&nbsp; &nbsp; <strong style='color: #555555; '>rerun Log Files: </strong><a target='_blank' style='white-space: nowrap;' data-bs-toggle='tooltip' data-bs-placement='right' title='View Detailed rerun Log' href='%s'> <font color='#DC3912'> &nbsp; [TXT </font> </a>" %
-                                    failed_testcase.log_file_path)
-                                report_file_handler.write(
-                                    " | <a target='_blank' style='white-space: nowrap;' data-bs-toggle='tooltip' data-bs-placement='right' title='View Detailed rerun Log' href='%s'> <font color='#DC3912'> HTML]</font> </a>" %
-                                    failed_testcase.log_file_path.replace("test.rerun.log", "test.rerun.html"))
+                            report_file_handler.write(
+                                "&nbsp; &nbsp; <strong style='color: #555555; '>rerun Log Files: </strong><a target='_blank' style='white-space: nowrap;' data-bs-toggle='tooltip' data-bs-placement='right' title='View Detailed rerun Log' href='%s'> <font color='#DC3912'> &nbsp; [TXT </font> </a>" %
+                                failed_testcase.log_file_path)
+                            report_file_handler.write(
+                                " | <a target='_blank' style='white-space: nowrap;' data-bs-toggle='tooltip' data-bs-placement='right' title='View Detailed rerun Log' href='%s'> <font color='#DC3912'> HTML]</font> </a>" %
+                                failed_testcase.log_file_path.replace("test.rerun.log", "test.rerun.html"))
                         except BaseException:
                             print(traceback.format_exc())
 
                     report_file_handler.write("</td>")
 
                     report_file_handler.write("<td width='200' align='center' >")
                     report_file_handler.write("<font>")
@@ -547,40 +545,38 @@
                         report_file_handler.write("<font color='orange'> - Miss Attribute</font>")
 
                     report_file_handler.write("</font>")
                     report_file_handler.write("</font></a>")
 
                     try:
                         if passed_testcase.rerun_tag == 0:
-                            if getattr(settings, 'LOG_TO_FILE', True):
-                                report_file_handler.write(
-                                    "&nbsp; &nbsp; <strong style='color: #555555; '>Log Files: </strong><a target='_blank' style='white-space: nowrap;' data-bs-toggle='tooltip' data-bs-placement='right' title='View Detailed Log' href='%s'>   <font color='#3366CC'>&nbsp; [TXT </font> </a>" %
-                                    passed_testcase.log_file_path)
-                                report_file_handler.write(
-                                    " | <a target='_blank' style='white-space: nowrap;' data-bs-toggle='tooltip' data-bs-placement='right' title='View Detailed Log' href='%s'>   <font color='#3366CC'> HTML]</font> </a>" %
-                                    passed_testcase.log_file_path.replace("test.log", "test.html"))
+                            report_file_handler.write(
+                                "&nbsp; &nbsp; <strong style='color: #555555; '>Log Files: </strong><a target='_blank' style='white-space: nowrap;' data-bs-toggle='tooltip' data-bs-placement='right' title='View Detailed Log' href='%s'>   <font color='#3366CC'>&nbsp; [TXT </font> </a>" %
+                                passed_testcase.log_file_path)
+                            report_file_handler.write(
+                                " | <a target='_blank' style='white-space: nowrap;' data-bs-toggle='tooltip' data-bs-placement='right' title='View Detailed Log' href='%s'>   <font color='#3366CC'> HTML]</font> </a>" %
+                                passed_testcase.log_file_path.replace("test.log", "test.html"))
                     except BaseException:
                         print(traceback.format_exc())
 
                     try:
                         if passed_testcase.rerun_tag == 1:
-                            if getattr(settings, 'LOG_TO_FILE', True):
-                                report_file_handler.write(
-                                    "&nbsp; &nbsp; <strong style='color: #555555; '>Log Files: </strong><a title='Log' href='%s'> &nbsp;[TXT </a>" %
-                                    passed_testcase.log_file_path.replace("test.rerun.log", "test.log"))
-                                report_file_handler.write(
-                                    " | <a target='_blank' title='HTML Log' href='%s'> HTML] </a>" %
-                                    passed_testcase.log_file_path.replace("test.rerun.log", "test.html"))
-
-                                report_file_handler.write(
-                                    "&nbsp; &nbsp; <strong style='color: #555555; '>rerun Log Files: </strong><a title='rerun_Log' href='%s'> &nbsp;[TXT </a>" %
-                                    passed_testcase.log_file_path)
-                                report_file_handler.write(
-                                    " | <a target='_blank' title='rerun_Log' href='%s'> HTML] </a>" %
-                                    passed_testcase.log_file_path.replace("test.rerun.log", "test.rerun.html"))
+                            report_file_handler.write(
+                                "&nbsp; &nbsp; <strong style='color: #555555; '>Log Files: </strong><a title='Log' href='%s'> &nbsp;[TXT </a>" %
+                                passed_testcase.log_file_path.replace("test.rerun.log", "test.log"))
+                            report_file_handler.write(
+                                " | <a target='_blank' title='HTML Log' href='%s'> HTML] </a>" %
+                                passed_testcase.log_file_path.replace("test.rerun.log", "test.html"))
+
+                            report_file_handler.write(
+                                "&nbsp; &nbsp; <strong style='color: #555555; '>rerun Log Files: </strong><a title='rerun_Log' href='%s'> &nbsp;[TXT </a>" %
+                                passed_testcase.log_file_path)
+                            report_file_handler.write(
+                                " | <a target='_blank' title='rerun_Log' href='%s'> HTML] </a>" %
+                                passed_testcase.log_file_path.replace("test.rerun.log", "test.rerun.html"))
                     except BaseException:
                         print(traceback.format_exc())
 
                     report_file_handler.write("</td>")
 
                     report_file_handler.write("<td width='200' align='center'>")
                     report_file_handler.write("<font color='#333'>")
```

### Comparing `linktest-2.7.3/linktest/logged_requests.py` & `linktest-2.7.4/linktest/logged_requests.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.3/linktest/main.py` & `linktest-2.7.4/linktest/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,16 +35,15 @@
     - generate_xunit_result (saves xunit report; default value is False; used for TestLink integration)
     - auto_log_request (default value is True; automatically logs request actions)
     - AUTO_DOWNLOAD_CHROMEDRIVER (default value is False; automatically downloads the appropriate Chromedriver based on the Chrome version)
 
     # ------ Configuration Related to the TestCase's Log ------
     - LOG_FORMAT = '[%(asctime)s] %(levelname)-8s %(name)-12s %(message)s'
     - LOG_LEVEL = logging.DEBUG # default value is DEBUG
-    - LOG_TO_FILE = True # default value is True
-    - LOG_TO_CONSOLE = True # default value is True
+    - LOG_TO_CONSOLE = True # default value is True, Always log to file
 
 2. settings/testcase_tags.py
     - The Tags class is used to define all test case tags.
     - Assign a tag to each test case (tags can be any non-blank string; you can create tags based on your specific needs, such as "smoke", "nightly", "regression", "p1", "ignore", etc.)
     - Note: If a test case's tag contains "ignore", it will only be added to the ignore_testcase_list, even if its tag attribute contains other tag names (e.g. tag = "nightly, smoke, ignore")
 
 Usage of the linktest automation framework:
@@ -525,27 +524,21 @@
             importlib.reload(logging)
 
             if not os.path.exists(testcase_full_folder):
                 os.makedirs(testcase_full_folder)
 
             logfile_full_name = testcase_full_folder + os.sep + logger_name
 
-            # Add FileHandler if LOG_TO_FILE is set to True in settings
-            if getattr(settings, 'LOG_TO_FILE', True):
-                handlers.append(logging.FileHandler(logfile_full_name))
+            # always write log to file
+            handlers.append(logging.FileHandler(logfile_full_name))
 
             # Add StreamHandler if LOG_TO_CONSOLE is set to True in settings
             if getattr(settings, 'LOG_TO_CONSOLE', True):
                 handlers.append(logging.StreamHandler(sys.stdout))
 
-            # # If no handlers are specified, add FileHandler & StreamHandler as default, Note: None is not False
-            # if getattr(settings, 'LOG_TO_FILE', None) is None and getattr(settings, 'LOG_TO_CONSOLE', None) is None:
-            #     handlers.append(logging.FileHandler(logfile_full_name))
-            #     handlers.append(logging.StreamHandler(sys.stdout))
-
             # Define basic configuration
             logging.basicConfig(
                 # Define logging level
                 level=level,
                 # Declare the object we created to format the log messages
                 format=log_format,
                 # Declare handlers
@@ -1222,22 +1215,22 @@
                         if issubclass(testcase, ios_testcase.IOSTestCase):
                             # set executing_ios_testcase_flag as False after this ios testcase execution done
                             TestCaseExecutor.executing_ios_testcase_flag = False
 
                         if issubclass(testcase, android_testcase.AndroidTestCase):
                             setattr(TestCaseExecutor, device_name, False)
 
-                        # if getattr(settings, 'LOG_TO_FILE', False):
-                        #     with open(executing_testcase.logfile_full_name, "r", encoding="utf-8", errors="ignore") as logfile_full_name:
-                        #         execution_log = logfile_full_name.read()
-                        #         executing_testcase.execution_log = execution_log
+                        with open(executing_testcase.logfile_full_name, "r", encoding="utf-8",
+                                  errors="ignore") as logfile_full_name:
+                            execution_log = logfile_full_name.read()
+                            executing_testcase.execution_log = execution_log
+
                     finally:
                         try:
-                            if getattr(settings, 'LOG_TO_FILE', True):
-                                generate_html_log.generate_html_log(executing_testcase)
+                            generate_html_log.generate_html_log(executing_testcase)
                         except BaseException:
                             traceback.print_exc()
                             executing_testcase.logger.error(traceback.format_exc())
 
                         if os.sep + "jenkins" + os.sep + "workspace" + os.sep in project_info.project_path:
                             TestCaseExecutor.jenkins_job_name = \
                                 project_info.project_path.split(os.sep + "jenkins" + os.sep + "workspace" + os.sep)[
```

### Comparing `linktest-2.7.3/linktest/memory_usage.py` & `linktest-2.7.4/linktest/memory_usage.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.3/linktest/re_func.py` & `linktest-2.7.4/linktest/re_func.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.3/linktest/run.py` & `linktest-2.7.4/linktest/run.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.3/linktest/run_testcase_thread.py` & `linktest-2.7.4/linktest/run_testcase_thread.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.3/linktest/scp_report_to_specified_path.py` & `linktest-2.7.4/linktest/scp_report_to_specified_path.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.3/linktest/selenium_helper.py` & `linktest-2.7.4/linktest/selenium_helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,18 +11,19 @@
     traceback.print_exc()
 
 try:
     if hasattr(settings, "run_by_github_action") and settings.run_by_github_action is True:
         # todo 此次逻辑需要再优化一下
         pass
     else:
-        if getattr(settings, "AUTO_DOWNLOAD_CHROMEDRIVER", False):
-            import chromedriver_autoinstaller
+        if not getattr(settings, "CHROME_DRIVER_PATH", False):
+            if getattr(settings, "AUTO_DOWNLOAD_CHROMEDRIVER", False):
+                import chromedriver_autoinstaller
 
-            chromedriver_autoinstaller.install()
+                chromedriver_autoinstaller.install()
 except BaseException:
     traceback.print_exc()
 
 
 class SeleniumHelper(object):
     set_implicitly_wait_flag = False
```

### Comparing `linktest-2.7.3/linktest/timeout_thread.py` & `linktest-2.7.4/linktest/timeout_thread.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.3/linktest/ui_testcase.py` & `linktest-2.7.4/linktest/ui_testcase.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.3/linktest/update_config.py` & `linktest-2.7.4/linktest/update_config.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.3/linktest/webdriver_wrapper.py` & `linktest-2.7.4/linktest/webdriver_wrapper.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.3/linktest/webdriver_wrapper_chrome.py` & `linktest-2.7.4/linktest/webdriver_wrapper_chrome.py`

 * *Files 1% similar despite different names*

```diff
@@ -225,15 +225,17 @@
 class WebDriverWrapperChrome(Chrome):
     def __init__(self, ui_testcase, *args, **kwargs):
         self.logger = ui_testcase.logger
         self.ui_testcase = ui_testcase
 
         # Default options and service for Chrome, if not provided in kwargs
         options = kwargs.pop('options', Options())
-        service = None # todo macOS VS windows
+        # service = None # todo macOS VS windows
+        chrome_driver_path = getattr(settings, "CHROME_DRIVER_PATH", None)
+        service = Service(executable_path=chrome_driver_path)
         keep_alive = kwargs.pop('keep_alive', True)
 
         # Initialization of the Chrome WebDriver with the correct parameters
         super().__init__(options=options, service=service, keep_alive=keep_alive, *args, **kwargs)
 
     def _log_action(self, action, *args):
         if args:
```

### Comparing `linktest-2.7.3/linktest/webdriver_wrapper_edge.py` & `linktest-2.7.4/linktest/webdriver_wrapper_edge.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.3/linktest/webdriver_wrapper_firefox.py` & `linktest-2.7.4/linktest/webdriver_wrapper_firefox.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.3/linktest/webdriver_wrapper_ie.py` & `linktest-2.7.4/linktest/webdriver_wrapper_ie.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.3/linktest/webdriver_wrapper_safari.py` & `linktest-2.7.4/linktest/webdriver_wrapper_safari.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.3/linktest/xml_report.py` & `linktest-2.7.4/linktest/xml_report.py`

 * *Files identical despite different names*

### Comparing `linktest-2.7.3/linktest.egg-info/SOURCES.txt` & `linktest-2.7.4/linktest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

