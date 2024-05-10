# Comparing `tmp/odoo12-addon-vertical_carsharing-12.0.0.1.8.dev1.tar.gz` & `tmp/odoo12-addon-vertical_carsharing-12.0.0.1.9.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/odoo12-addon-vertical_carsharing-12.0.0.1.8.dev1.tar", last modified: Tue Oct 31 11:27:25 2023, max compression
+gzip compressed data, was "dist/odoo12-addon-vertical_carsharing-12.0.0.1.9.dev1.tar", last modified: Wed Nov  1 12:15:38 2023, max compression
```

## Comparing `odoo12-addon-vertical_carsharing-12.0.0.1.8.dev1.tar` & `odoo12-addon-vertical_carsharing-12.0.0.1.9.dev1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxr-x   0 somit     (1001) somit     (1001)        0 2023-10-31 11:27:25.000000 odoo12-addon-vertical_carsharing-12.0.0.1.8.dev1/
--rw-rw-r--   0 somit     (1001) somit     (1001)      363 2023-10-31 11:27:25.000000 odoo12-addon-vertical_carsharing-12.0.0.1.8.dev1/PKG-INFO
-drwxrwxr-x   0 somit     (1001) somit     (1001)        0 2023-10-31 11:27:25.000000 odoo12-addon-vertical_carsharing-12.0.0.1.8.dev1/odoo/
-drwxrwxr-x   0 somit     (1001) somit     (1001)        0 2023-10-31 11:27:25.000000 odoo12-addon-vertical_carsharing-12.0.0.1.8.dev1/odoo/addons/
-drwxrwxr-x   0 somit     (1001) somit     (1001)        0 2023-10-31 11:27:25.000000 odoo12-addon-vertical_carsharing-12.0.0.1.8.dev1/odoo/addons/vertical_carsharing/
--rw-rw-r--   0 somit     (1001) somit     (1001)       44 2023-07-24 07:10:05.000000 odoo12-addon-vertical_carsharing-12.0.0.1.8.dev1/odoo/addons/vertical_carsharing/__init__.py
--rw-rw-r--   0 somit     (1001) somit     (1001)      769 2023-10-31 11:10:23.000000 odoo12-addon-vertical_carsharing-12.0.0.1.8.dev1/odoo/addons/vertical_carsharing/__manifest__.py
-drwxrwxr-x   0 somit     (1001) somit     (1001)        0 2023-10-31 11:27:25.000000 odoo12-addon-vertical_carsharing-12.0.0.1.8.dev1/odoo/addons/vertical_carsharing/data/
--rw-rw-r--   0 somit     (1001) somit     (1001)     1639 2023-07-24 07:10:05.000000 odoo12-addon-vertical_carsharing-12.0.0.1.8.dev1/odoo/addons/vertical_carsharing/data/sm_account_journal.xml
-drwxrwxr-x   0 somit     (1001) somit     (1001)        0 2023-10-31 11:27:25.000000 odoo12-addon-vertical_carsharing-12.0.0.1.8.dev1/odoo/addons/vertical_carsharing/email_tmpl/
--rw-rw-r--   0 somit     (1001) somit     (1001)      972 2023-07-24 07:10:05.000000 odoo12-addon-vertical_carsharing-12.0.0.1.8.dev1/odoo/addons/vertical_carsharing/email_tmpl/notification_email.xml
-drwxrwxr-x   0 somit     (1001) somit     (1001)        0 2023-10-31 11:27:25.000000 odoo12-addon-vertical_carsharing-12.0.0.1.8.dev1/odoo/addons/vertical_carsharing/models/
--rw-rw-r--   0 somit     (1001) somit     (1001)      141 2023-10-31 09:15:01.000000 odoo12-addon-vertical_carsharing-12.0.0.1.8.dev1/odoo/addons/vertical_carsharing/models/__init__.py
--rw-rw-r--   0 somit     (1001) somit     (1001)     1692 2023-10-31 11:14:49.000000 odoo12-addon-vertical_carsharing-12.0.0.1.8.dev1/odoo/addons/vertical_carsharing/models/account_analytic.py
--rw-rw-r--   0 somit     (1001) somit     (1001)      618 2023-07-24 07:10:05.000000 odoo12-addon-vertical_carsharing-12.0.0.1.8.dev1/odoo/addons/vertical_carsharing/models/models_cs_task.py
--rw-rw-r--   0 somit     (1001) somit     (1001)      344 2023-07-24 07:10:05.000000 odoo12-addon-vertical_carsharing-12.0.0.1.8.dev1/odoo/addons/vertical_carsharing/models/models_sm_bank.py
--rw-rw-r--   0 somit     (1001) somit     (1001)     3426 2023-07-24 07:10:05.000000 odoo12-addon-vertical_carsharing-12.0.0.1.8.dev1/odoo/addons/vertical_carsharing/models/models_sm_member.py
--rw-rw-r--   0 somit     (1001) somit     (1001)      204 2023-10-31 09:00:36.000000 odoo12-addon-vertical_carsharing-12.0.0.1.8.dev1/odoo/addons/vertical_carsharing/models/product.py
-drwxrwxr-x   0 somit     (1001) somit     (1001)        0 2023-10-31 11:27:25.000000 odoo12-addon-vertical_carsharing-12.0.0.1.8.dev1/odoo/addons/vertical_carsharing/static/
-drwxrwxr-x   0 somit     (1001) somit     (1001)        0 2023-10-31 11:27:25.000000 odoo12-addon-vertical_carsharing-12.0.0.1.8.dev1/odoo/addons/vertical_carsharing/static/src/
-drwxrwxr-x   0 somit     (1001) somit     (1001)        0 2023-10-31 11:27:25.000000 odoo12-addon-vertical_carsharing-12.0.0.1.8.dev1/odoo/addons/vertical_carsharing/static/src/img/
--rw-rw-r--   0 somit     (1001) somit     (1001)    18655 2023-07-24 07:10:05.000000 odoo12-addon-vertical_carsharing-12.0.0.1.8.dev1/odoo/addons/vertical_carsharing/static/src/img/carsharing.png
-drwxrwxr-x   0 somit     (1001) somit     (1001)        0 2023-10-31 11:27:25.000000 odoo12-addon-vertical_carsharing-12.0.0.1.8.dev1/odoo/addons/vertical_carsharing/static/src/scss/
--rwxrwxr-x   0 somit     (1001) somit     (1001)     2831 2023-07-24 07:10:05.000000 odoo12-addon-vertical_carsharing-12.0.0.1.8.dev1/odoo/addons/vertical_carsharing/static/src/scss/primary_variables.scss
-drwxrwxr-x   0 somit     (1001) somit     (1001)        0 2023-10-31 11:27:25.000000 odoo12-addon-vertical_carsharing-12.0.0.1.8.dev1/odoo/addons/vertical_carsharing/views/
--rw-rw-r--   0 somit     (1001) somit     (1001)      780 2023-10-31 11:07:49.000000 odoo12-addon-vertical_carsharing-12.0.0.1.8.dev1/odoo/addons/vertical_carsharing/views/account_analytic_view.xml
--rw-rw-r--   0 somit     (1001) somit     (1001)      548 2023-10-31 11:10:01.000000 odoo12-addon-vertical_carsharing-12.0.0.1.8.dev1/odoo/addons/vertical_carsharing/views/product_view.xml
--rw-rw-r--   0 somit     (1001) somit     (1001)      458 2023-07-24 07:10:05.000000 odoo12-addon-vertical_carsharing-12.0.0.1.8.dev1/odoo/addons/vertical_carsharing/views/views.xml
--rw-rw-r--   0 somit     (1001) somit     (1001)      694 2023-07-24 07:10:05.000000 odoo12-addon-vertical_carsharing-12.0.0.1.8.dev1/odoo/addons/vertical_carsharing/views/views_cs_task.xml
--rw-rw-r--   0 somit     (1001) somit     (1001)     4966 2023-07-24 07:10:05.000000 odoo12-addon-vertical_carsharing-12.0.0.1.8.dev1/odoo/addons/vertical_carsharing/views/views_members.xml
-drwxrwxr-x   0 somit     (1001) somit     (1001)        0 2023-10-31 11:27:25.000000 odoo12-addon-vertical_carsharing-12.0.0.1.8.dev1/odoo12_addon_vertical_carsharing.egg-info/
--rw-rw-r--   0 somit     (1001) somit     (1001)      363 2023-10-31 11:27:24.000000 odoo12-addon-vertical_carsharing-12.0.0.1.8.dev1/odoo12_addon_vertical_carsharing.egg-info/PKG-INFO
--rw-rw-r--   0 somit     (1001) somit     (1001)     1305 2023-10-31 11:27:25.000000 odoo12-addon-vertical_carsharing-12.0.0.1.8.dev1/odoo12_addon_vertical_carsharing.egg-info/SOURCES.txt
--rw-rw-r--   0 somit     (1001) somit     (1001)        1 2023-10-31 11:27:24.000000 odoo12-addon-vertical_carsharing-12.0.0.1.8.dev1/odoo12_addon_vertical_carsharing.egg-info/dependency_links.txt
--rw-rw-r--   0 somit     (1001) somit     (1001)        1 2023-10-31 09:24:53.000000 odoo12-addon-vertical_carsharing-12.0.0.1.8.dev1/odoo12_addon_vertical_carsharing.egg-info/not-zip-safe
--rw-rw-r--   0 somit     (1001) somit     (1001)       51 2023-10-31 11:27:24.000000 odoo12-addon-vertical_carsharing-12.0.0.1.8.dev1/odoo12_addon_vertical_carsharing.egg-info/requires.txt
--rw-rw-r--   0 somit     (1001) somit     (1001)        5 2023-10-31 11:27:24.000000 odoo12-addon-vertical_carsharing-12.0.0.1.8.dev1/odoo12_addon_vertical_carsharing.egg-info/top_level.txt
--rw-rw-r--   0 somit     (1001) somit     (1001)       38 2023-10-31 11:27:25.000000 odoo12-addon-vertical_carsharing-12.0.0.1.8.dev1/setup.cfg
--rw-rw-r--   0 somit     (1001) somit     (1001)      100 2023-10-31 09:23:15.000000 odoo12-addon-vertical_carsharing-12.0.0.1.8.dev1/setup.py
+drwxrwxr-x   0 somit     (1001) somit     (1001)        0 2023-11-01 12:15:38.000000 odoo12-addon-vertical_carsharing-12.0.0.1.9.dev1/
+-rw-rw-r--   0 somit     (1001) somit     (1001)      363 2023-11-01 12:15:38.000000 odoo12-addon-vertical_carsharing-12.0.0.1.9.dev1/PKG-INFO
+drwxrwxr-x   0 somit     (1001) somit     (1001)        0 2023-11-01 12:15:38.000000 odoo12-addon-vertical_carsharing-12.0.0.1.9.dev1/odoo/
+drwxrwxr-x   0 somit     (1001) somit     (1001)        0 2023-11-01 12:15:38.000000 odoo12-addon-vertical_carsharing-12.0.0.1.9.dev1/odoo/addons/
+drwxrwxr-x   0 somit     (1001) somit     (1001)        0 2023-11-01 12:15:38.000000 odoo12-addon-vertical_carsharing-12.0.0.1.9.dev1/odoo/addons/vertical_carsharing/
+-rw-rw-r--   0 somit     (1001) somit     (1001)       44 2023-07-24 07:10:05.000000 odoo12-addon-vertical_carsharing-12.0.0.1.9.dev1/odoo/addons/vertical_carsharing/__init__.py
+-rw-rw-r--   0 somit     (1001) somit     (1001)      665 2023-11-01 12:12:08.000000 odoo12-addon-vertical_carsharing-12.0.0.1.9.dev1/odoo/addons/vertical_carsharing/__manifest__.py
+drwxrwxr-x   0 somit     (1001) somit     (1001)        0 2023-11-01 12:15:38.000000 odoo12-addon-vertical_carsharing-12.0.0.1.9.dev1/odoo/addons/vertical_carsharing/data/
+-rw-rw-r--   0 somit     (1001) somit     (1001)     1639 2023-07-24 07:10:05.000000 odoo12-addon-vertical_carsharing-12.0.0.1.9.dev1/odoo/addons/vertical_carsharing/data/sm_account_journal.xml
+drwxrwxr-x   0 somit     (1001) somit     (1001)        0 2023-11-01 12:15:38.000000 odoo12-addon-vertical_carsharing-12.0.0.1.9.dev1/odoo/addons/vertical_carsharing/email_tmpl/
+-rw-rw-r--   0 somit     (1001) somit     (1001)      972 2023-07-24 07:10:05.000000 odoo12-addon-vertical_carsharing-12.0.0.1.9.dev1/odoo/addons/vertical_carsharing/email_tmpl/notification_email.xml
+drwxrwxr-x   0 somit     (1001) somit     (1001)        0 2023-11-01 12:15:38.000000 odoo12-addon-vertical_carsharing-12.0.0.1.9.dev1/odoo/addons/vertical_carsharing/models/
+-rw-rw-r--   0 somit     (1001) somit     (1001)      141 2023-11-01 11:56:58.000000 odoo12-addon-vertical_carsharing-12.0.0.1.9.dev1/odoo/addons/vertical_carsharing/models/__init__.py
+-rw-rw-r--   0 somit     (1001) somit     (1001)     1692 2023-11-01 12:03:28.000000 odoo12-addon-vertical_carsharing-12.0.0.1.9.dev1/odoo/addons/vertical_carsharing/models/account_analytic.py
+-rw-rw-r--   0 somit     (1001) somit     (1001)      618 2023-07-24 07:10:05.000000 odoo12-addon-vertical_carsharing-12.0.0.1.9.dev1/odoo/addons/vertical_carsharing/models/models_cs_task.py
+-rw-rw-r--   0 somit     (1001) somit     (1001)      344 2023-07-24 07:10:05.000000 odoo12-addon-vertical_carsharing-12.0.0.1.9.dev1/odoo/addons/vertical_carsharing/models/models_sm_bank.py
+-rw-rw-r--   0 somit     (1001) somit     (1001)     3426 2023-07-24 07:10:05.000000 odoo12-addon-vertical_carsharing-12.0.0.1.9.dev1/odoo/addons/vertical_carsharing/models/models_sm_member.py
+-rw-rw-r--   0 somit     (1001) somit     (1001)      204 2023-10-31 09:00:36.000000 odoo12-addon-vertical_carsharing-12.0.0.1.9.dev1/odoo/addons/vertical_carsharing/models/product.py
+drwxrwxr-x   0 somit     (1001) somit     (1001)        0 2023-11-01 12:15:38.000000 odoo12-addon-vertical_carsharing-12.0.0.1.9.dev1/odoo/addons/vertical_carsharing/static/
+drwxrwxr-x   0 somit     (1001) somit     (1001)        0 2023-11-01 12:15:38.000000 odoo12-addon-vertical_carsharing-12.0.0.1.9.dev1/odoo/addons/vertical_carsharing/static/src/
+drwxrwxr-x   0 somit     (1001) somit     (1001)        0 2023-11-01 12:15:38.000000 odoo12-addon-vertical_carsharing-12.0.0.1.9.dev1/odoo/addons/vertical_carsharing/static/src/img/
+-rw-rw-r--   0 somit     (1001) somit     (1001)    18655 2023-07-24 07:10:05.000000 odoo12-addon-vertical_carsharing-12.0.0.1.9.dev1/odoo/addons/vertical_carsharing/static/src/img/carsharing.png
+drwxrwxr-x   0 somit     (1001) somit     (1001)        0 2023-11-01 12:15:38.000000 odoo12-addon-vertical_carsharing-12.0.0.1.9.dev1/odoo/addons/vertical_carsharing/static/src/scss/
+-rwxrwxr-x   0 somit     (1001) somit     (1001)     2831 2023-07-24 07:10:05.000000 odoo12-addon-vertical_carsharing-12.0.0.1.9.dev1/odoo/addons/vertical_carsharing/static/src/scss/primary_variables.scss
+drwxrwxr-x   0 somit     (1001) somit     (1001)        0 2023-11-01 12:15:38.000000 odoo12-addon-vertical_carsharing-12.0.0.1.9.dev1/odoo/addons/vertical_carsharing/views/
+-rw-rw-r--   0 somit     (1001) somit     (1001)      780 2023-11-01 11:56:58.000000 odoo12-addon-vertical_carsharing-12.0.0.1.9.dev1/odoo/addons/vertical_carsharing/views/account_analytic_view.xml
+-rw-rw-r--   0 somit     (1001) somit     (1001)      548 2023-11-01 11:52:31.000000 odoo12-addon-vertical_carsharing-12.0.0.1.9.dev1/odoo/addons/vertical_carsharing/views/product_view.xml
+-rw-rw-r--   0 somit     (1001) somit     (1001)      458 2023-07-24 07:10:05.000000 odoo12-addon-vertical_carsharing-12.0.0.1.9.dev1/odoo/addons/vertical_carsharing/views/views.xml
+-rw-rw-r--   0 somit     (1001) somit     (1001)      694 2023-07-24 07:10:05.000000 odoo12-addon-vertical_carsharing-12.0.0.1.9.dev1/odoo/addons/vertical_carsharing/views/views_cs_task.xml
+-rw-rw-r--   0 somit     (1001) somit     (1001)     4966 2023-07-24 07:10:05.000000 odoo12-addon-vertical_carsharing-12.0.0.1.9.dev1/odoo/addons/vertical_carsharing/views/views_members.xml
+drwxrwxr-x   0 somit     (1001) somit     (1001)        0 2023-11-01 12:15:38.000000 odoo12-addon-vertical_carsharing-12.0.0.1.9.dev1/odoo12_addon_vertical_carsharing.egg-info/
+-rw-rw-r--   0 somit     (1001) somit     (1001)      363 2023-11-01 12:15:38.000000 odoo12-addon-vertical_carsharing-12.0.0.1.9.dev1/odoo12_addon_vertical_carsharing.egg-info/PKG-INFO
+-rw-rw-r--   0 somit     (1001) somit     (1001)     1315 2023-11-01 12:15:38.000000 odoo12-addon-vertical_carsharing-12.0.0.1.9.dev1/odoo12_addon_vertical_carsharing.egg-info/SOURCES.txt
+-rw-rw-r--   0 somit     (1001) somit     (1001)        1 2023-11-01 12:15:38.000000 odoo12-addon-vertical_carsharing-12.0.0.1.9.dev1/odoo12_addon_vertical_carsharing.egg-info/dependency_links.txt
+-rw-rw-r--   0 somit     (1001) somit     (1001)        1 2023-11-01 12:15:38.000000 odoo12-addon-vertical_carsharing-12.0.0.1.9.dev1/odoo12_addon_vertical_carsharing.egg-info/not-zip-safe
+-rw-rw-r--   0 somit     (1001) somit     (1001)       51 2023-11-01 12:15:38.000000 odoo12-addon-vertical_carsharing-12.0.0.1.9.dev1/odoo12_addon_vertical_carsharing.egg-info/requires.txt
+-rw-rw-r--   0 somit     (1001) somit     (1001)        5 2023-11-01 12:15:38.000000 odoo12-addon-vertical_carsharing-12.0.0.1.9.dev1/odoo12_addon_vertical_carsharing.egg-info/top_level.txt
+-rw-rw-r--   0 somit     (1001) somit     (1001)       67 2023-11-01 12:15:38.000000 odoo12-addon-vertical_carsharing-12.0.0.1.9.dev1/setup.cfg
+-rw-rw-r--   0 somit     (1001) somit     (1001)      248 2023-11-01 11:50:48.000000 odoo12-addon-vertical_carsharing-12.0.0.1.9.dev1/setup.py
```

### Comparing `odoo12-addon-vertical_carsharing-12.0.0.1.8.dev1/odoo/addons/vertical_carsharing/data/sm_account_journal.xml` & `odoo12-addon-vertical_carsharing-12.0.0.1.9.dev1/odoo/addons/vertical_carsharing/data/sm_account_journal.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-vertical_carsharing-12.0.0.1.8.dev1/odoo/addons/vertical_carsharing/email_tmpl/notification_email.xml` & `odoo12-addon-vertical_carsharing-12.0.0.1.9.dev1/odoo/addons/vertical_carsharing/email_tmpl/notification_email.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-vertical_carsharing-12.0.0.1.8.dev1/odoo/addons/vertical_carsharing/models/account_analytic.py` & `odoo12-addon-vertical_carsharing-12.0.0.1.9.dev1/odoo/addons/vertical_carsharing/models/account_analytic.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-vertical_carsharing-12.0.0.1.8.dev1/odoo/addons/vertical_carsharing/models/models_cs_task.py` & `odoo12-addon-vertical_carsharing-12.0.0.1.9.dev1/odoo/addons/vertical_carsharing/models/models_cs_task.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-vertical_carsharing-12.0.0.1.8.dev1/odoo/addons/vertical_carsharing/models/models_sm_member.py` & `odoo12-addon-vertical_carsharing-12.0.0.1.9.dev1/odoo/addons/vertical_carsharing/models/models_sm_member.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-vertical_carsharing-12.0.0.1.8.dev1/odoo/addons/vertical_carsharing/static/src/img/carsharing.png` & `odoo12-addon-vertical_carsharing-12.0.0.1.9.dev1/odoo/addons/vertical_carsharing/static/src/img/carsharing.png`

 * *Files identical despite different names*

### Comparing `odoo12-addon-vertical_carsharing-12.0.0.1.8.dev1/odoo/addons/vertical_carsharing/static/src/scss/primary_variables.scss` & `odoo12-addon-vertical_carsharing-12.0.0.1.9.dev1/odoo/addons/vertical_carsharing/static/src/scss/primary_variables.scss`

 * *Files identical despite different names*

### Comparing `odoo12-addon-vertical_carsharing-12.0.0.1.8.dev1/odoo/addons/vertical_carsharing/views/account_analytic_view.xml` & `odoo12-addon-vertical_carsharing-12.0.0.1.9.dev1/odoo/addons/vertical_carsharing/views/account_analytic_view.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-vertical_carsharing-12.0.0.1.8.dev1/odoo/addons/vertical_carsharing/views/product_view.xml` & `odoo12-addon-vertical_carsharing-12.0.0.1.9.dev1/odoo/addons/vertical_carsharing/views/product_view.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-vertical_carsharing-12.0.0.1.8.dev1/odoo/addons/vertical_carsharing/views/views_cs_task.xml` & `odoo12-addon-vertical_carsharing-12.0.0.1.9.dev1/odoo/addons/vertical_carsharing/views/views_cs_task.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-vertical_carsharing-12.0.0.1.8.dev1/odoo/addons/vertical_carsharing/views/views_members.xml` & `odoo12-addon-vertical_carsharing-12.0.0.1.9.dev1/odoo/addons/vertical_carsharing/views/views_members.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-vertical_carsharing-12.0.0.1.8.dev1/odoo12_addon_vertical_carsharing.egg-info/SOURCES.txt` & `odoo12-addon-vertical_carsharing-12.0.0.1.9.dev1/odoo12_addon_vertical_carsharing.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+setup.cfg
 setup.py
 odoo/addons/vertical_carsharing/__init__.py
 odoo/addons/vertical_carsharing/__manifest__.py
 odoo/addons/vertical_carsharing/data/sm_account_journal.xml
 odoo/addons/vertical_carsharing/email_tmpl/notification_email.xml
 odoo/addons/vertical_carsharing/models/__init__.py
 odoo/addons/vertical_carsharing/models/account_analytic.py
```

