# Comparing `tmp/odoo12-addon-sm_partago_invoicing_rest_api-12.0.0.1.7.dev1.tar.gz` & `tmp/odoo12-addon-sm_partago_invoicing_rest_api-12.0.0.1.8.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odoo12-addon-sm_partago_invoicing_rest_api-12.0.0.1.7.dev1.tar", last modified: Thu Oct 26 09:48:09 2023, max compression
+gzip compressed data, was "odoo12-addon-sm_partago_invoicing_rest_api-12.0.0.1.8.dev1.tar", last modified: Fri Nov 10 13:30:36 2023, max compression
```

## Comparing `odoo12-addon-sm_partago_invoicing_rest_api-12.0.0.1.7.dev1.tar` & `odoo12-addon-sm_partago_invoicing_rest_api-12.0.0.1.8.dev1.tar`

### file list

```diff
@@ -1,29 +1,11 @@
-drwxr-xr-x   0 carla     (1000) carla     (1000)        0 2023-10-26 09:48:09.588781 odoo12-addon-sm_partago_invoicing_rest_api-12.0.0.1.7.dev1/
--rw-r--r--   0 carla     (1000) carla     (1000)      512 2023-10-26 09:48:09.588781 odoo12-addon-sm_partago_invoicing_rest_api-12.0.0.1.7.dev1/PKG-INFO
-drwxr-xr-x   0 carla     (1000) carla     (1000)        0 2023-10-26 09:48:09.585448 odoo12-addon-sm_partago_invoicing_rest_api-12.0.0.1.7.dev1/odoo/
-drwxr-xr-x   0 carla     (1000) carla     (1000)        0 2023-10-26 09:48:09.585448 odoo12-addon-sm_partago_invoicing_rest_api-12.0.0.1.7.dev1/odoo/addons/
-drwxr-xr-x   0 carla     (1000) carla     (1000)        0 2023-10-26 09:48:09.585448 odoo12-addon-sm_partago_invoicing_rest_api-12.0.0.1.7.dev1/odoo/addons/sm_partago_invoicing_rest_api/
--rwxr-xr-x   0 carla     (1000) carla     (1000)       68 2023-09-28 10:53:13.000000 odoo12-addon-sm_partago_invoicing_rest_api-12.0.0.1.7.dev1/odoo/addons/sm_partago_invoicing_rest_api/__init__.py
--rwxr-xr-x   0 carla     (1000) carla     (1000)      690 2023-10-26 09:45:25.000000 odoo12-addon-sm_partago_invoicing_rest_api-12.0.0.1.7.dev1/odoo/addons/sm_partago_invoicing_rest_api/__manifest__.py
-drwxr-xr-x   0 carla     (1000) carla     (1000)        0 2023-10-26 09:48:09.585448 odoo12-addon-sm_partago_invoicing_rest_api-12.0.0.1.7.dev1/odoo/addons/sm_partago_invoicing_rest_api/models/
--rw-r--r--   0 carla     (1000) carla     (1000)       76 2023-09-28 10:53:13.000000 odoo12-addon-sm_partago_invoicing_rest_api-12.0.0.1.7.dev1/odoo/addons/sm_partago_invoicing_rest_api/models/__init__.py
--rw-r--r--   0 carla     (1000) carla     (1000)      754 2023-09-28 10:53:13.000000 odoo12-addon-sm_partago_invoicing_rest_api-12.0.0.1.7.dev1/odoo/addons/sm_partago_invoicing_rest_api/models/models_sm_company.py
--rw-r--r--   0 carla     (1000) carla     (1000)      879 2023-09-28 10:53:13.000000 odoo12-addon-sm_partago_invoicing_rest_api-12.0.0.1.7.dev1/odoo/addons/sm_partago_invoicing_rest_api/models/models_sm_res_config_settings.py
-drwxr-xr-x   0 carla     (1000) carla     (1000)        0 2023-10-26 09:48:09.588781 odoo12-addon-sm_partago_invoicing_rest_api-12.0.0.1.7.dev1/odoo/addons/sm_partago_invoicing_rest_api/services/
--rw-r--r--   0 carla     (1000) carla     (1000)       34 2023-09-28 10:53:13.000000 odoo12-addon-sm_partago_invoicing_rest_api-12.0.0.1.7.dev1/odoo/addons/sm_partago_invoicing_rest_api/services/__init__.py
--rw-r--r--   0 carla     (1000) carla     (1000)     4534 2023-10-26 09:44:00.000000 odoo12-addon-sm_partago_invoicing_rest_api-12.0.0.1.7.dev1/odoo/addons/sm_partago_invoicing_rest_api/services/cs_invoice_services.py
--rw-r--r--   0 carla     (1000) carla     (1000)     1702 2023-10-02 09:55:11.000000 odoo12-addon-sm_partago_invoicing_rest_api-12.0.0.1.7.dev1/odoo/addons/sm_partago_invoicing_rest_api/services/schemas.py
-drwxr-xr-x   0 carla     (1000) carla     (1000)        0 2023-10-26 09:48:09.588781 odoo12-addon-sm_partago_invoicing_rest_api-12.0.0.1.7.dev1/odoo/addons/sm_partago_invoicing_rest_api/tests/
--rw-r--r--   0 carla     (1000) carla     (1000)       52 2023-09-28 10:53:13.000000 odoo12-addon-sm_partago_invoicing_rest_api-12.0.0.1.7.dev1/odoo/addons/sm_partago_invoicing_rest_api/tests/__init__.py
--rw-r--r--   0 carla     (1000) carla     (1000)      326 2023-09-28 10:53:13.000000 odoo12-addon-sm_partago_invoicing_rest_api-12.0.0.1.7.dev1/odoo/addons/sm_partago_invoicing_rest_api/tests/test_cs_invoice_services.py
-drwxr-xr-x   0 carla     (1000) carla     (1000)        0 2023-10-26 09:48:09.588781 odoo12-addon-sm_partago_invoicing_rest_api-12.0.0.1.7.dev1/odoo/addons/sm_partago_invoicing_rest_api/views/
--rw-r--r--   0 carla     (1000) carla     (1000)      960 2023-09-28 10:53:13.000000 odoo12-addon-sm_partago_invoicing_rest_api-12.0.0.1.7.dev1/odoo/addons/sm_partago_invoicing_rest_api/views/views_res_config_settings.xml
-drwxr-xr-x   0 carla     (1000) carla     (1000)        0 2023-10-26 09:48:09.588781 odoo12-addon-sm_partago_invoicing_rest_api-12.0.0.1.7.dev1/odoo12_addon_sm_partago_invoicing_rest_api.egg-info/
--rw-r--r--   0 carla     (1000) carla     (1000)      512 2023-10-26 09:48:09.000000 odoo12-addon-sm_partago_invoicing_rest_api-12.0.0.1.7.dev1/odoo12_addon_sm_partago_invoicing_rest_api.egg-info/PKG-INFO
--rw-r--r--   0 carla     (1000) carla     (1000)     1140 2023-10-26 09:48:09.000000 odoo12-addon-sm_partago_invoicing_rest_api-12.0.0.1.7.dev1/odoo12_addon_sm_partago_invoicing_rest_api.egg-info/SOURCES.txt
--rw-r--r--   0 carla     (1000) carla     (1000)        1 2023-10-26 09:48:09.000000 odoo12-addon-sm_partago_invoicing_rest_api-12.0.0.1.7.dev1/odoo12_addon_sm_partago_invoicing_rest_api.egg-info/dependency_links.txt
--rw-r--r--   0 carla     (1000) carla     (1000)        1 2023-10-02 09:35:01.000000 odoo12-addon-sm_partago_invoicing_rest_api-12.0.0.1.7.dev1/odoo12_addon_sm_partago_invoicing_rest_api.egg-info/not-zip-safe
--rw-r--r--   0 carla     (1000) carla     (1000)       93 2023-10-26 09:48:09.000000 odoo12-addon-sm_partago_invoicing_rest_api-12.0.0.1.7.dev1/odoo12_addon_sm_partago_invoicing_rest_api.egg-info/requires.txt
--rw-r--r--   0 carla     (1000) carla     (1000)        5 2023-10-26 09:48:09.000000 odoo12-addon-sm_partago_invoicing_rest_api-12.0.0.1.7.dev1/odoo12_addon_sm_partago_invoicing_rest_api.egg-info/top_level.txt
--rw-r--r--   0 carla     (1000) carla     (1000)       38 2023-10-26 09:48:09.588781 odoo12-addon-sm_partago_invoicing_rest_api-12.0.0.1.7.dev1/setup.cfg
--rw-r--r--   0 carla     (1000) carla     (1000)      100 2023-10-26 09:46:43.000000 odoo12-addon-sm_partago_invoicing_rest_api-12.0.0.1.7.dev1/setup.py
+drwxr-xr-x   0 carla     (1000) carla     (1000)        0 2023-11-10 13:30:36.946740 odoo12-addon-sm_partago_invoicing_rest_api-12.0.0.1.8.dev1/
+-rw-r--r--   0 carla     (1000) carla     (1000)      512 2023-11-10 13:30:36.946740 odoo12-addon-sm_partago_invoicing_rest_api-12.0.0.1.8.dev1/PKG-INFO
+drwxr-xr-x   0 carla     (1000) carla     (1000)        0 2023-11-10 13:30:36.946740 odoo12-addon-sm_partago_invoicing_rest_api-12.0.0.1.8.dev1/odoo12_addon_sm_partago_invoicing_rest_api.egg-info/
+-rw-r--r--   0 carla     (1000) carla     (1000)      512 2023-11-10 13:30:36.000000 odoo12-addon-sm_partago_invoicing_rest_api-12.0.0.1.8.dev1/odoo12_addon_sm_partago_invoicing_rest_api.egg-info/PKG-INFO
+-rw-r--r--   0 carla     (1000) carla     (1000)      402 2023-11-10 13:30:36.000000 odoo12-addon-sm_partago_invoicing_rest_api-12.0.0.1.8.dev1/odoo12_addon_sm_partago_invoicing_rest_api.egg-info/SOURCES.txt
+-rw-r--r--   0 carla     (1000) carla     (1000)        1 2023-11-10 13:30:36.000000 odoo12-addon-sm_partago_invoicing_rest_api-12.0.0.1.8.dev1/odoo12_addon_sm_partago_invoicing_rest_api.egg-info/dependency_links.txt
+-rw-r--r--   0 carla     (1000) carla     (1000)        1 2023-11-10 13:30:36.000000 odoo12-addon-sm_partago_invoicing_rest_api-12.0.0.1.8.dev1/odoo12_addon_sm_partago_invoicing_rest_api.egg-info/not-zip-safe
+-rw-r--r--   0 carla     (1000) carla     (1000)       93 2023-11-10 13:30:36.000000 odoo12-addon-sm_partago_invoicing_rest_api-12.0.0.1.8.dev1/odoo12_addon_sm_partago_invoicing_rest_api.egg-info/requires.txt
+-rw-r--r--   0 carla     (1000) carla     (1000)        5 2023-11-10 13:30:36.000000 odoo12-addon-sm_partago_invoicing_rest_api-12.0.0.1.8.dev1/odoo12_addon_sm_partago_invoicing_rest_api.egg-info/top_level.txt
+-rw-r--r--   0 carla     (1000) carla     (1000)       38 2023-11-10 13:30:36.946740 odoo12-addon-sm_partago_invoicing_rest_api-12.0.0.1.8.dev1/setup.cfg
+-rw-r--r--   0 carla     (1000) carla     (1000)      100 2023-11-10 13:29:57.000000 odoo12-addon-sm_partago_invoicing_rest_api-12.0.0.1.8.dev1/setup.py
```

### Comparing `odoo12-addon-sm_partago_invoicing_rest_api-12.0.0.1.7.dev1/PKG-INFO` & `odoo12-addon-sm_partago_invoicing_rest_api-12.0.0.1.8.dev1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: odoo12-addon-sm_partago_invoicing_rest_api
-Version: 12.0.0.1.7.dev1
+Version: 12.0.0.1.8.dev1
 Summary: Expose CS Invoice with REST API
 Home-page: https://git.coopdevs.org/coopdevs/odoo/odoo-addons/enhancements/enhancements-account-invoicing
 Author: Coopdevs Treball
 License: UNKNOWN
 Description: 
                 Expose CS Invoice with REST API
```

### Comparing `odoo12-addon-sm_partago_invoicing_rest_api-12.0.0.1.7.dev1/odoo12_addon_sm_partago_invoicing_rest_api.egg-info/PKG-INFO` & `odoo12-addon-sm_partago_invoicing_rest_api-12.0.0.1.8.dev1/odoo12_addon_sm_partago_invoicing_rest_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: odoo12-addon-sm-partago-invoicing-rest-api
-Version: 12.0.0.1.7.dev1
+Version: 12.0.0.1.8.dev1
 Summary: Expose CS Invoice with REST API
 Home-page: https://git.coopdevs.org/coopdevs/odoo/odoo-addons/enhancements/enhancements-account-invoicing
 Author: Coopdevs Treball
 License: UNKNOWN
 Description: 
                 Expose CS Invoice with REST API
```

