# Comparing `tmp/django-flex-report-0.8.0.tar.gz` & `tmp/django-flex-report-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-flex-report-0.8.0.tar", last modified: Fri May  3 20:59:45 2024, max compression
+gzip compressed data, was "django-flex-report-0.8.1.tar", last modified: Fri May 10 16:09:32 2024, max compression
```

## Comparing `django-flex-report-0.8.0.tar` & `django-flex-report-0.8.1.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxrwxr-x   0 saman     (1000) saman     (1000)        0 2024-05-03 20:59:45.880765 django-flex-report-0.8.0/
--rw-rw-r--   0 saman     (1000) saman     (1000)     1076 2024-03-28 15:09:39.000000 django-flex-report-0.8.0/LICENSE
--rw-rw-r--   0 saman     (1000) saman     (1000)      721 2024-03-28 15:09:39.000000 django-flex-report-0.8.0/MANIFEST.in
--rw-r--r--   0 saman     (1000) saman     (1000)     1933 2024-05-03 20:59:45.880765 django-flex-report-0.8.0/PKG-INFO
-drwxrwxr-x   0 saman     (1000) saman     (1000)        0 2024-05-03 20:59:45.876765 django-flex-report-0.8.0/django_flex_report.egg-info/
--rw-r--r--   0 saman     (1000) saman     (1000)     1933 2024-05-03 20:59:45.000000 django-flex-report-0.8.0/django_flex_report.egg-info/PKG-INFO
--rw-rw-r--   0 saman     (1000) saman     (1000)     1734 2024-05-03 20:59:45.000000 django-flex-report-0.8.0/django_flex_report.egg-info/SOURCES.txt
--rw-rw-r--   0 saman     (1000) saman     (1000)        1 2024-05-03 20:59:45.000000 django-flex-report-0.8.0/django_flex_report.egg-info/dependency_links.txt
--rw-rw-r--   0 saman     (1000) saman     (1000)        1 2024-05-03 20:59:45.000000 django-flex-report-0.8.0/django_flex_report.egg-info/not-zip-safe
--rw-rw-r--   0 saman     (1000) saman     (1000)      447 2024-05-03 20:59:45.000000 django-flex-report-0.8.0/django_flex_report.egg-info/requires.txt
--rw-rw-r--   0 saman     (1000) saman     (1000)       19 2024-05-03 20:59:45.000000 django-flex-report-0.8.0/django_flex_report.egg-info/top_level.txt
-drwxrwxr-x   0 saman     (1000) saman     (1000)        0 2024-05-03 20:59:45.876765 django-flex-report-0.8.0/flex_report/
--rw-rw-r--   0 saman     (1000) saman     (1000)     1728 2024-05-03 20:59:28.000000 django-flex-report-0.8.0/flex_report/__init__.py
--rw-rw-r--   0 saman     (1000) saman     (1000)       57 2024-05-03 20:59:45.000000 django-flex-report-0.8.0/flex_report/_version.py
--rw-rw-r--   0 saman     (1000) saman     (1000)     2423 2024-05-03 20:59:28.000000 django-flex-report-0.8.0/flex_report/admin.py
--rw-rw-r--   0 saman     (1000) saman     (1000)     4855 2024-05-03 20:59:28.000000 django-flex-report-0.8.0/flex_report/app_settings.py
--rw-rw-r--   0 saman     (1000) saman     (1000)      149 2024-05-03 20:59:28.000000 django-flex-report-0.8.0/flex_report/apps.py
--rw-rw-r--   0 saman     (1000) saman     (1000)      256 2024-05-03 20:59:28.000000 django-flex-report-0.8.0/flex_report/choices.py
--rw-rw-r--   0 saman     (1000) saman     (1000)     3555 2024-05-03 20:59:28.000000 django-flex-report-0.8.0/flex_report/constants.py
--rw-rw-r--   0 saman     (1000) saman     (1000)      707 2024-05-03 20:59:28.000000 django-flex-report-0.8.0/flex_report/fields.py
--rw-rw-r--   0 saman     (1000) saman     (1000)     4580 2024-05-03 20:59:28.000000 django-flex-report-0.8.0/flex_report/filterset.py
--rw-rw-r--   0 saman     (1000) saman     (1000)     2606 2024-05-03 20:59:28.000000 django-flex-report-0.8.0/flex_report/forms.py
--rw-rw-r--   0 saman     (1000) saman     (1000)      223 2024-05-03 20:59:28.000000 django-flex-report-0.8.0/flex_report/managers.py
-drwxrwxr-x   0 saman     (1000) saman     (1000)        0 2024-05-03 20:59:45.876765 django-flex-report-0.8.0/flex_report/migrations/
--rw-rw-r--   0 saman     (1000) saman     (1000)     8753 2024-05-03 20:59:28.000000 django-flex-report-0.8.0/flex_report/migrations/0001_initial.py
--rw-rw-r--   0 saman     (1000) saman     (1000)      413 2024-05-03 20:59:28.000000 django-flex-report-0.8.0/flex_report/migrations/0002_alter_column_title.py
--rw-rw-r--   0 saman     (1000) saman     (1000)     2362 2024-05-03 20:59:28.000000 django-flex-report-0.8.0/flex_report/migrations/0003_column_groups_column_users_tablebutton_groups_and_more.py
--rw-rw-r--   0 saman     (1000) saman     (1000)      767 2024-05-03 20:59:28.000000 django-flex-report-0.8.0/flex_report/migrations/0004_column_creator.py
--rw-rw-r--   0 saman     (1000) saman     (1000)      480 2024-05-03 20:59:28.000000 django-flex-report-0.8.0/flex_report/migrations/0005_template_model_user_path.py
--rw-rw-r--   0 saman     (1000) saman     (1000)      475 2024-05-03 20:59:28.000000 django-flex-report-0.8.0/flex_report/migrations/0006_tablebutton_query_strings.py
--rw-rw-r--   0 saman     (1000) saman     (1000)      755 2024-05-03 20:59:28.000000 django-flex-report-0.8.0/flex_report/migrations/0007_remove_template_buttons_alter_template_columns.py
--rw-rw-r--   0 saman     (1000) saman     (1000)      715 2024-05-03 20:59:28.000000 django-flex-report-0.8.0/flex_report/migrations/0008_template_buttons.py
--rw-rw-r--   0 saman     (1000) saman     (1000)      616 2024-05-03 20:59:28.000000 django-flex-report-0.8.0/flex_report/migrations/0009_alter_template_buttons.py
--rw-rw-r--   0 saman     (1000) saman     (1000)     1311 2024-05-03 20:59:28.000000 django-flex-report-0.8.0/flex_report/migrations/0010_alter_column_model_alter_template_model_and_more.py
--rw-rw-r--   0 saman     (1000) saman     (1000)      593 2024-05-03 20:59:28.000000 django-flex-report-0.8.0/flex_report/migrations/0011_alter_template_model_user_path.py
--rw-rw-r--   0 saman     (1000) saman     (1000)     1323 2024-05-03 20:59:28.000000 django-flex-report-0.8.0/flex_report/migrations/0012_tablebuttoncolor_alter_tablebutton_color.py
--rw-rw-r--   0 saman     (1000) saman     (1000)      592 2024-05-03 20:59:28.000000 django-flex-report-0.8.0/flex_report/migrations/0013_column_column_type.py
--rw-rw-r--   0 saman     (1000) saman     (1000)      572 2024-05-03 20:59:28.000000 django-flex-report-0.8.0/flex_report/migrations/0014_alter_column_column_type.py
--rw-rw-r--   0 saman     (1000) saman     (1000)      342 2024-05-03 20:59:28.000000 django-flex-report-0.8.0/flex_report/migrations/0015_remove_column_column_type.py
--rw-rw-r--   0 saman     (1000) saman     (1000)      546 2024-05-03 20:59:28.000000 django-flex-report-0.8.0/flex_report/migrations/0016_column_column_type.py
--rw-rw-r--   0 saman     (1000) saman     (1000)        0 2024-05-03 20:59:28.000000 django-flex-report-0.8.0/flex_report/migrations/__init__.py
--rw-rw-r--   0 saman     (1000) saman     (1000)    14511 2024-05-03 20:59:28.000000 django-flex-report-0.8.0/flex_report/mixins.py
--rw-rw-r--   0 saman     (1000) saman     (1000)     9042 2024-05-03 20:59:28.000000 django-flex-report-0.8.0/flex_report/models.py
-drwxrwxr-x   0 saman     (1000) saman     (1000)        0 2024-05-03 20:59:45.876765 django-flex-report-0.8.0/flex_report/templatetags/
--rw-rw-r--   0 saman     (1000) saman     (1000)        0 2024-05-03 20:59:28.000000 django-flex-report-0.8.0/flex_report/templatetags/__init__.py
--rw-rw-r--   0 saman     (1000) saman     (1000)     5207 2024-05-03 20:59:28.000000 django-flex-report-0.8.0/flex_report/templatetags/flex_report_filters.py
--rw-rw-r--   0 saman     (1000) saman     (1000)     1674 2024-05-03 20:59:28.000000 django-flex-report-0.8.0/flex_report/urls.py
--rw-rw-r--   0 saman     (1000) saman     (1000)    25156 2024-05-03 20:59:28.000000 django-flex-report-0.8.0/flex_report/utils.py
--rw-rw-r--   0 saman     (1000) saman     (1000)    11418 2024-05-03 20:59:28.000000 django-flex-report-0.8.0/flex_report/views.py
--rw-rw-r--   0 saman     (1000) saman     (1000)     1666 2024-03-28 15:09:39.000000 django-flex-report-0.8.0/pyproject.toml
--rw-rw-r--   0 saman     (1000) saman     (1000)      447 2024-03-28 15:09:39.000000 django-flex-report-0.8.0/requirements.txt
--rw-rw-r--   0 saman     (1000) saman     (1000)       38 2024-05-03 20:59:45.880765 django-flex-report-0.8.0/setup.cfg
--rw-rw-r--   0 saman     (1000) saman     (1000)       73 2024-03-28 15:09:39.000000 django-flex-report-0.8.0/setup.py
+drwx------   0 erfan     (1000) erfan     (1000)        0 2024-05-10 16:09:32.499946 django-flex-report-0.8.1/
+-rwx------   0 erfan     (1000) erfan     (1000)     1076 2024-05-10 15:40:57.000000 django-flex-report-0.8.1/LICENSE
+-rwx------   0 erfan     (1000) erfan     (1000)      721 2024-05-10 15:40:57.000000 django-flex-report-0.8.1/MANIFEST.in
+-rwx------   0 erfan     (1000) erfan     (1000)     1933 2024-05-10 16:09:32.499487 django-flex-report-0.8.1/PKG-INFO
+drwx------   0 erfan     (1000) erfan     (1000)        0 2024-05-10 16:09:32.498942 django-flex-report-0.8.1/django_flex_report.egg-info/
+-rwx------   0 erfan     (1000) erfan     (1000)     1933 2024-05-10 16:09:32.000000 django-flex-report-0.8.1/django_flex_report.egg-info/PKG-INFO
+-rwx------   0 erfan     (1000) erfan     (1000)     1734 2024-05-10 16:09:32.000000 django-flex-report-0.8.1/django_flex_report.egg-info/SOURCES.txt
+-rwx------   0 erfan     (1000) erfan     (1000)        1 2024-05-10 16:09:32.000000 django-flex-report-0.8.1/django_flex_report.egg-info/dependency_links.txt
+-rwx------   0 erfan     (1000) erfan     (1000)        1 2024-05-10 16:09:32.000000 django-flex-report-0.8.1/django_flex_report.egg-info/not-zip-safe
+-rwx------   0 erfan     (1000) erfan     (1000)      447 2024-05-10 16:09:32.000000 django-flex-report-0.8.1/django_flex_report.egg-info/requires.txt
+-rwx------   0 erfan     (1000) erfan     (1000)       19 2024-05-10 16:09:32.000000 django-flex-report-0.8.1/django_flex_report.egg-info/top_level.txt
+drwx------   0 erfan     (1000) erfan     (1000)        0 2024-05-10 16:09:32.488726 django-flex-report-0.8.1/flex_report/
+-rwx------   0 erfan     (1000) erfan     (1000)     1728 2024-05-10 15:40:57.000000 django-flex-report-0.8.1/flex_report/__init__.py
+-rwx------   0 erfan     (1000) erfan     (1000)       57 2024-05-10 16:09:31.000000 django-flex-report-0.8.1/flex_report/_version.py
+-rwx------   0 erfan     (1000) erfan     (1000)     2423 2024-05-10 15:40:57.000000 django-flex-report-0.8.1/flex_report/admin.py
+-rwx------   0 erfan     (1000) erfan     (1000)     4855 2024-05-10 16:09:26.000000 django-flex-report-0.8.1/flex_report/app_settings.py
+-rwx------   0 erfan     (1000) erfan     (1000)      149 2024-05-10 15:40:57.000000 django-flex-report-0.8.1/flex_report/apps.py
+-rwx------   0 erfan     (1000) erfan     (1000)      256 2024-05-10 15:40:57.000000 django-flex-report-0.8.1/flex_report/choices.py
+-rwx------   0 erfan     (1000) erfan     (1000)     3555 2024-05-10 15:40:57.000000 django-flex-report-0.8.1/flex_report/constants.py
+-rwx------   0 erfan     (1000) erfan     (1000)      707 2024-05-10 15:40:57.000000 django-flex-report-0.8.1/flex_report/fields.py
+-rwx------   0 erfan     (1000) erfan     (1000)     4580 2024-05-10 15:40:57.000000 django-flex-report-0.8.1/flex_report/filterset.py
+-rwx------   0 erfan     (1000) erfan     (1000)     2606 2024-05-10 16:09:26.000000 django-flex-report-0.8.1/flex_report/forms.py
+-rwx------   0 erfan     (1000) erfan     (1000)      223 2024-05-10 15:40:57.000000 django-flex-report-0.8.1/flex_report/managers.py
+drwx------   0 erfan     (1000) erfan     (1000)        0 2024-05-10 16:09:32.497419 django-flex-report-0.8.1/flex_report/migrations/
+-rwx------   0 erfan     (1000) erfan     (1000)     8753 2024-05-10 15:40:57.000000 django-flex-report-0.8.1/flex_report/migrations/0001_initial.py
+-rwx------   0 erfan     (1000) erfan     (1000)      413 2024-05-10 15:40:57.000000 django-flex-report-0.8.1/flex_report/migrations/0002_alter_column_title.py
+-rwx------   0 erfan     (1000) erfan     (1000)     2362 2024-05-10 15:40:57.000000 django-flex-report-0.8.1/flex_report/migrations/0003_column_groups_column_users_tablebutton_groups_and_more.py
+-rwx------   0 erfan     (1000) erfan     (1000)      767 2024-05-10 15:40:57.000000 django-flex-report-0.8.1/flex_report/migrations/0004_column_creator.py
+-rwx------   0 erfan     (1000) erfan     (1000)      480 2024-05-10 15:40:57.000000 django-flex-report-0.8.1/flex_report/migrations/0005_template_model_user_path.py
+-rwx------   0 erfan     (1000) erfan     (1000)      475 2024-05-10 15:40:57.000000 django-flex-report-0.8.1/flex_report/migrations/0006_tablebutton_query_strings.py
+-rwx------   0 erfan     (1000) erfan     (1000)      755 2024-05-10 15:40:57.000000 django-flex-report-0.8.1/flex_report/migrations/0007_remove_template_buttons_alter_template_columns.py
+-rwx------   0 erfan     (1000) erfan     (1000)      715 2024-05-10 15:40:57.000000 django-flex-report-0.8.1/flex_report/migrations/0008_template_buttons.py
+-rwx------   0 erfan     (1000) erfan     (1000)      616 2024-05-10 15:40:57.000000 django-flex-report-0.8.1/flex_report/migrations/0009_alter_template_buttons.py
+-rwx------   0 erfan     (1000) erfan     (1000)     1311 2024-05-10 15:40:57.000000 django-flex-report-0.8.1/flex_report/migrations/0010_alter_column_model_alter_template_model_and_more.py
+-rwx------   0 erfan     (1000) erfan     (1000)      593 2024-05-10 15:40:57.000000 django-flex-report-0.8.1/flex_report/migrations/0011_alter_template_model_user_path.py
+-rwx------   0 erfan     (1000) erfan     (1000)     1323 2024-05-10 15:40:57.000000 django-flex-report-0.8.1/flex_report/migrations/0012_tablebuttoncolor_alter_tablebutton_color.py
+-rwx------   0 erfan     (1000) erfan     (1000)      592 2024-05-10 15:40:57.000000 django-flex-report-0.8.1/flex_report/migrations/0013_column_column_type.py
+-rwx------   0 erfan     (1000) erfan     (1000)      572 2024-05-10 15:40:57.000000 django-flex-report-0.8.1/flex_report/migrations/0014_alter_column_column_type.py
+-rwx------   0 erfan     (1000) erfan     (1000)      342 2024-05-10 15:40:57.000000 django-flex-report-0.8.1/flex_report/migrations/0015_remove_column_column_type.py
+-rwx------   0 erfan     (1000) erfan     (1000)      546 2024-05-10 15:40:57.000000 django-flex-report-0.8.1/flex_report/migrations/0016_column_column_type.py
+-rwx------   0 erfan     (1000) erfan     (1000)        0 2024-05-10 15:40:57.000000 django-flex-report-0.8.1/flex_report/migrations/__init__.py
+-rwx------   0 erfan     (1000) erfan     (1000)    14511 2024-05-10 16:09:26.000000 django-flex-report-0.8.1/flex_report/mixins.py
+-rwx------   0 erfan     (1000) erfan     (1000)     9042 2024-05-10 15:40:57.000000 django-flex-report-0.8.1/flex_report/models.py
+drwx------   0 erfan     (1000) erfan     (1000)        0 2024-05-10 16:09:32.498350 django-flex-report-0.8.1/flex_report/templatetags/
+-rwx------   0 erfan     (1000) erfan     (1000)        0 2024-05-10 15:40:57.000000 django-flex-report-0.8.1/flex_report/templatetags/__init__.py
+-rwx------   0 erfan     (1000) erfan     (1000)     5207 2024-05-10 15:40:57.000000 django-flex-report-0.8.1/flex_report/templatetags/flex_report_filters.py
+-rwx------   0 erfan     (1000) erfan     (1000)     1674 2024-05-10 15:40:57.000000 django-flex-report-0.8.1/flex_report/urls.py
+-rwx------   0 erfan     (1000) erfan     (1000)    25177 2024-05-10 15:49:07.000000 django-flex-report-0.8.1/flex_report/utils.py
+-rwx------   0 erfan     (1000) erfan     (1000)    11418 2024-05-10 16:09:26.000000 django-flex-report-0.8.1/flex_report/views.py
+-rwx------   0 erfan     (1000) erfan     (1000)     1666 2024-05-10 15:40:57.000000 django-flex-report-0.8.1/pyproject.toml
+-rwx------   0 erfan     (1000) erfan     (1000)      447 2024-05-10 15:40:57.000000 django-flex-report-0.8.1/requirements.txt
+-rwx------   0 erfan     (1000) erfan     (1000)       38 2024-05-10 16:09:32.500042 django-flex-report-0.8.1/setup.cfg
+-rwx------   0 erfan     (1000) erfan     (1000)       73 2024-05-10 15:40:57.000000 django-flex-report-0.8.1/setup.py
```

### Comparing `django-flex-report-0.8.0/LICENSE` & `django-flex-report-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.8.0/MANIFEST.in` & `django-flex-report-0.8.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.8.0/PKG-INFO` & `django-flex-report-0.8.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-flex-report
-Version: 0.8.0
+Version: 0.8.1
 Summary: A Django app to create flexible reports
 Author-email: Saman Zand Haghighi <samanzandh@gmail.com>
 License: MIT
 Project-URL: Homepage, http://github.com/saman-zand-h/django-flex-report
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `django-flex-report-0.8.0/django_flex_report.egg-info/PKG-INFO` & `django-flex-report-0.8.1/django_flex_report.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-flex-report
-Version: 0.8.0
+Version: 0.8.1
 Summary: A Django app to create flexible reports
 Author-email: Saman Zand Haghighi <samanzandh@gmail.com>
 License: MIT
 Project-URL: Homepage, http://github.com/saman-zand-h/django-flex-report
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `django-flex-report-0.8.0/django_flex_report.egg-info/SOURCES.txt` & `django-flex-report-0.8.1/django_flex_report.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.8.0/flex_report/__init__.py` & `django-flex-report-0.8.1/flex_report/__init__.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.8.0/flex_report/admin.py` & `django-flex-report-0.8.1/flex_report/admin.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.8.0/flex_report/app_settings.py` & `django-flex-report-0.8.1/flex_report/app_settings.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.8.0/flex_report/constants.py` & `django-flex-report-0.8.1/flex_report/constants.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.8.0/flex_report/fields.py` & `django-flex-report-0.8.1/flex_report/fields.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.8.0/flex_report/filterset.py` & `django-flex-report-0.8.1/flex_report/filterset.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.8.0/flex_report/forms.py` & `django-flex-report-0.8.1/flex_report/forms.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.8.0/flex_report/migrations/0001_initial.py` & `django-flex-report-0.8.1/flex_report/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.8.0/flex_report/migrations/0003_column_groups_column_users_tablebutton_groups_and_more.py` & `django-flex-report-0.8.1/flex_report/migrations/0003_column_groups_column_users_tablebutton_groups_and_more.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.8.0/flex_report/migrations/0004_column_creator.py` & `django-flex-report-0.8.1/flex_report/migrations/0004_column_creator.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.8.0/flex_report/migrations/0007_remove_template_buttons_alter_template_columns.py` & `django-flex-report-0.8.1/flex_report/migrations/0007_remove_template_buttons_alter_template_columns.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.8.0/flex_report/migrations/0008_template_buttons.py` & `django-flex-report-0.8.1/flex_report/migrations/0008_template_buttons.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.8.0/flex_report/migrations/0009_alter_template_buttons.py` & `django-flex-report-0.8.1/flex_report/migrations/0009_alter_template_buttons.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.8.0/flex_report/migrations/0010_alter_column_model_alter_template_model_and_more.py` & `django-flex-report-0.8.1/flex_report/migrations/0010_alter_column_model_alter_template_model_and_more.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.8.0/flex_report/migrations/0011_alter_template_model_user_path.py` & `django-flex-report-0.8.1/flex_report/migrations/0011_alter_template_model_user_path.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.8.0/flex_report/migrations/0012_tablebuttoncolor_alter_tablebutton_color.py` & `django-flex-report-0.8.1/flex_report/migrations/0012_tablebuttoncolor_alter_tablebutton_color.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.8.0/flex_report/migrations/0013_column_column_type.py` & `django-flex-report-0.8.1/flex_report/migrations/0013_column_column_type.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.8.0/flex_report/migrations/0014_alter_column_column_type.py` & `django-flex-report-0.8.1/flex_report/migrations/0014_alter_column_column_type.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.8.0/flex_report/migrations/0016_column_column_type.py` & `django-flex-report-0.8.1/flex_report/migrations/0016_column_column_type.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.8.0/flex_report/mixins.py` & `django-flex-report-0.8.1/flex_report/mixins.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.8.0/flex_report/models.py` & `django-flex-report-0.8.1/flex_report/models.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.8.0/flex_report/templatetags/flex_report_filters.py` & `django-flex-report-0.8.1/flex_report/templatetags/flex_report_filters.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.8.0/flex_report/urls.py` & `django-flex-report-0.8.1/flex_report/urls.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.8.0/flex_report/utils.py` & `django-flex-report-0.8.1/flex_report/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -526,15 +526,15 @@
     def export(self):
         headers_name = self.get_export_headers()
         columns = headers_name.keys()
         queryset = self.get_export_qs()
         sheet_name = str(self.get_export_kwargs().get("sheet_name", "default"))
         cell_fn = self.get_export_kwargs().get("cell_fn", self._default_cell_fn)
 
-        workbook = xlwt.Workbook(encoding="utf-8")
+        workbook = xlwt.Workbook(encoding="utf-8", style_compression=2)
         default_style = xlwt.XFStyle()
         sheet = workbook.add_sheet(
             sheet_name
             or str(nested_getattr(queryset, "model._meta.verbose_name_plural", "sheet"))
         )
 
         for num, column in enumerate(columns):
```

### Comparing `django-flex-report-0.8.0/flex_report/views.py` & `django-flex-report-0.8.1/flex_report/views.py`

 * *Files identical despite different names*

### Comparing `django-flex-report-0.8.0/pyproject.toml` & `django-flex-report-0.8.1/pyproject.toml`

 * *Files identical despite different names*

