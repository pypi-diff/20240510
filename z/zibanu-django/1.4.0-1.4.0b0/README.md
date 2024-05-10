# Comparing `tmp/zibanu_django-1.4.0.tar.gz` & `tmp/zibanu_django-1.4.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zibanu_django-1.4.0.tar", last modified: Fri May 10 10:13:50 2024, max compression
+gzip compressed data, was "zibanu_django-1.4.0b0.tar", last modified: Fri May  3 11:31:01 2024, max compression
```

## Comparing `zibanu_django-1.4.0.tar` & `zibanu_django-1.4.0b0.tar`

### file list

```diff
@@ -1,109 +1,109 @@
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-05-10 10:13:50.277907 zibanu_django-1.4.0/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)    35148 2022-05-01 19:35:15.000000 zibanu_django-1.4.0/LICENSE
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      105 2023-08-07 23:22:31.000000 zibanu_django-1.4.0/MANIFEST.in
--rw-r--r--   0 macercha  (1000) macercha  (1000)    68384 2024-05-10 10:13:50.277907 zibanu_django-1.4.0/PKG-INFO
--rw-rw-r--   0 macercha  (1000) macercha  (1000)    27020 2023-09-12 12:23:03.000000 zibanu_django-1.4.0/README.md
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1009 2024-05-03 10:34:00.000000 zibanu_django-1.4.0/pyproject.toml
--rw-r--r--   0 macercha  (1000) macercha  (1000)       38 2024-05-10 10:13:50.277907 zibanu_django-1.4.0/setup.cfg
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-05-10 10:13:50.260908 zibanu_django-1.4.0/zibanu/
--rw-r--r--   0 macercha  (1000) macercha  (1000)      618 2024-03-11 02:33:38.000000 zibanu_django-1.4.0/zibanu/__init__.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-05-10 10:13:50.261908 zibanu_django-1.4.0/zibanu/django/
--rw-r--r--   0 macercha  (1000) macercha  (1000)      576 2024-05-10 10:03:37.000000 zibanu_django-1.4.0/zibanu/django/__init__.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-05-10 10:13:50.261908 zibanu_django-1.4.0/zibanu/django/api/
--rw-r--r--   0 macercha  (1000) macercha  (1000)      312 2024-03-11 02:33:38.000000 zibanu_django-1.4.0/zibanu/django/api/__init__.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-05-10 10:13:50.262908 zibanu_django-1.4.0/zibanu/django/api/services/
--rw-r--r--   0 macercha  (1000) macercha  (1000)      512 2024-04-04 21:09:36.000000 zibanu_django-1.4.0/zibanu/django/api/services/__init__.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)     1040 2024-04-04 21:51:55.000000 zibanu_django-1.4.0/zibanu/django/api/services/dial_codes.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)     1301 2024-03-11 02:33:38.000000 zibanu_django-1.4.0/zibanu/django/api/services/language.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)     1280 2024-03-11 02:33:38.000000 zibanu_django-1.4.0/zibanu/django/api/services/timezone.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)     1147 2024-03-11 02:33:38.000000 zibanu_django-1.4.0/zibanu/django/apps.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-05-10 10:13:50.262908 zibanu_django-1.4.0/zibanu/django/db/
--rw-r--r--   0 macercha  (1000) macercha  (1000)      503 2024-03-11 02:33:38.000000 zibanu_django-1.4.0/zibanu/django/db/__init__.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-05-10 10:13:50.262908 zibanu_django-1.4.0/zibanu/django/db/backends/
--rw-r--r--   0 macercha  (1000) macercha  (1000)      500 2024-03-11 02:33:38.000000 zibanu_django-1.4.0/zibanu/django/db/backends/__init__.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-05-10 10:13:50.263908 zibanu_django-1.4.0/zibanu/django/db/backends/oracle/
--rw-r--r--   0 macercha  (1000) macercha  (1000)      500 2024-03-11 02:33:38.000000 zibanu_django-1.4.0/zibanu/django/db/backends/oracle/__init__.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)     1572 2024-03-11 02:33:38.000000 zibanu_django-1.4.0/zibanu/django/db/backends/oracle/base.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-05-10 10:13:50.263908 zibanu_django-1.4.0/zibanu/django/db/models/
--rw-r--r--   0 macercha  (1000) macercha  (1000)      799 2024-04-03 22:31:00.000000 zibanu_django-1.4.0/zibanu/django/db/models/__init__.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)     1120 2024-03-11 02:33:38.000000 zibanu_django-1.4.0/zibanu/django/db/models/dated_model.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-05-10 10:13:50.264908 zibanu_django-1.4.0/zibanu/django/db/models/fields/
--rw-r--r--   0 macercha  (1000) macercha  (1000)      372 2024-04-03 22:31:00.000000 zibanu_django-1.4.0/zibanu/django/db/models/fields/__init__.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)     2261 2024-04-04 21:09:36.000000 zibanu_django-1.4.0/zibanu/django/db/models/fields/phone_field.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)     1580 2024-05-03 11:24:21.000000 zibanu_django-1.4.0/zibanu/django/db/models/manager.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)     2082 2024-03-11 02:33:38.000000 zibanu_django-1.4.0/zibanu/django/db/models/model.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-05-10 10:13:50.264908 zibanu_django-1.4.0/zibanu/django/lib/
--rw-r--r--   0 macercha  (1000) macercha  (1000)      556 2024-04-03 22:31:00.000000 zibanu_django-1.4.0/zibanu/django/lib/__init__.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-05-10 10:13:50.265908 zibanu_django-1.4.0/zibanu/django/lib/classes/
--rw-r--r--   0 macercha  (1000) macercha  (1000)      644 2024-03-11 02:33:38.000000 zibanu_django-1.4.0/zibanu/django/lib/classes/__init__.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)     5879 2024-03-11 02:33:38.000000 zibanu_django-1.4.0/zibanu/django/lib/classes/code_generator.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)     1182 2024-03-11 02:33:38.000000 zibanu_django-1.4.0/zibanu/django/lib/classes/extended_json_encoder.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)      731 2024-03-11 02:33:38.000000 zibanu_django-1.4.0/zibanu/django/lib/classes/model_name.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-05-10 10:13:50.265908 zibanu_django-1.4.0/zibanu/django/lib/enums/
--rw-r--r--   0 macercha  (1000) macercha  (1000)      521 2024-04-04 21:09:36.000000 zibanu_django-1.4.0/zibanu/django/lib/enums/__init__.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)     1943 2024-04-04 22:29:20.000000 zibanu_django-1.4.0/zibanu/django/lib/enums/dial_codes.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-05-10 10:13:50.258908 zibanu_django-1.4.0/zibanu/django/locale/
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-05-10 10:13:50.258908 zibanu_django-1.4.0/zibanu/django/locale/es/
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-05-10 10:13:50.265908 zibanu_django-1.4.0/zibanu/django/locale/es/LC_MESSAGES/
--rw-r--r--   0 macercha  (1000) macercha  (1000)     3239 2024-05-03 11:26:43.000000 zibanu_django-1.4.0/zibanu/django/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0 macercha  (1000) macercha  (1000)     7517 2024-05-03 11:26:33.000000 zibanu_django-1.4.0/zibanu/django/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-05-10 10:13:50.266908 zibanu_django-1.4.0/zibanu/django/rest_framework/
--rw-r--r--   0 macercha  (1000) macercha  (1000)      503 2024-03-11 02:33:38.000000 zibanu_django-1.4.0/zibanu/django/rest_framework/__init__.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)     2197 2024-03-13 14:44:10.000000 zibanu_django-1.4.0/zibanu/django/rest_framework/decorators.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-05-10 10:13:50.268908 zibanu_django-1.4.0/zibanu/django/rest_framework/exceptions/
--rw-r--r--   0 macercha  (1000) macercha  (1000)     1171 2024-03-15 01:58:14.000000 zibanu_django-1.4.0/zibanu/django/rest_framework/exceptions/__init__.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)     3076 2024-03-15 01:58:14.000000 zibanu_django-1.4.0/zibanu/django/rest_framework/exceptions/api_exception.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)      850 2024-03-11 22:02:32.000000 zibanu_django-1.4.0/zibanu/django/rest_framework/exceptions/multiple_login_error.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)      957 2024-03-15 01:58:14.000000 zibanu_django-1.4.0/zibanu/django/rest_framework/exceptions/not_implemented_exception.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)     1058 2024-03-18 23:17:34.000000 zibanu_django-1.4.0/zibanu/django/rest_framework/exceptions/permission_denied.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-05-10 10:13:50.268908 zibanu_django-1.4.0/zibanu/django/rest_framework/fields/
--rw-r--r--   0 macercha  (1000) macercha  (1000)      718 2024-03-11 02:33:38.000000 zibanu_django-1.4.0/zibanu/django/rest_framework/fields/__init__.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)     1343 2024-03-11 02:33:38.000000 zibanu_django-1.4.0/zibanu/django/rest_framework/fields/current_user_default.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)     5815 2024-04-05 11:24:32.000000 zibanu_django-1.4.0/zibanu/django/rest_framework/fields/hybrid_image.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-05-10 10:13:50.269908 zibanu_django-1.4.0/zibanu/django/rest_framework/permissions/
--rw-r--r--   0 macercha  (1000) macercha  (1000)      652 2024-03-11 02:33:38.000000 zibanu_django-1.4.0/zibanu/django/rest_framework/permissions/__init__.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)     1174 2024-03-11 02:33:38.000000 zibanu_django-1.4.0/zibanu/django/rest_framework/permissions/is_owner_or_read_only.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-05-10 10:13:50.270908 zibanu_django-1.4.0/zibanu/django/rest_framework/serializers/
--rw-r--r--   0 macercha  (1000) macercha  (1000)     1649 2024-03-11 02:33:38.000000 zibanu_django-1.4.0/zibanu/django/rest_framework/serializers/__init__.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)      646 2024-03-11 02:33:38.000000 zibanu_django-1.4.0/zibanu/django/rest_framework/serializers/fields.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)      863 2024-03-11 02:33:38.000000 zibanu_django-1.4.0/zibanu/django/rest_framework/serializers/model_serializer.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)     1031 2024-03-19 00:59:35.000000 zibanu_django-1.4.0/zibanu/django/rest_framework/utils.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-05-10 10:13:50.271908 zibanu_django-1.4.0/zibanu/django/rest_framework/viewsets/
--rw-r--r--   0 macercha  (1000) macercha  (1000)      779 2024-03-19 00:59:46.000000 zibanu_django-1.4.0/zibanu/django/rest_framework/viewsets/__init__.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)    15232 2024-05-03 10:58:52.000000 zibanu_django-1.4.0/zibanu/django/rest_framework/viewsets/model_viewset.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)     1737 2024-03-11 02:33:38.000000 zibanu_django-1.4.0/zibanu/django/rest_framework/viewsets/viewset.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-05-10 10:13:50.271908 zibanu_django-1.4.0/zibanu/django/template/
--rw-r--r--   0 macercha  (1000) macercha  (1000)      501 2024-03-11 02:33:38.000000 zibanu_django-1.4.0/zibanu/django/template/__init__.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)      825 2024-03-11 02:33:38.000000 zibanu_django-1.4.0/zibanu/django/template/apps.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-05-10 10:13:50.272908 zibanu_django-1.4.0/zibanu/django/template/context_processors/
--rw-r--r--   0 macercha  (1000) macercha  (1000)      619 2024-03-11 02:33:38.000000 zibanu_django-1.4.0/zibanu/django/template/context_processors/__init__.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)     1055 2024-03-11 02:33:38.000000 zibanu_django-1.4.0/zibanu/django/template/context_processors/full_static_uri.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)      819 2024-03-11 02:33:38.000000 zibanu_django-1.4.0/zibanu/django/template/context_processors/site.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-05-10 10:13:50.259908 zibanu_django-1.4.0/zibanu/django/template/locale/
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-05-10 10:13:50.259908 zibanu_django-1.4.0/zibanu/django/template/locale/es/
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-05-10 10:13:50.272908 zibanu_django-1.4.0/zibanu/django/template/locale/es/LC_MESSAGES/
--rw-r--r--   0 macercha  (1000) macercha  (1000)      709 2024-03-11 02:33:38.000000 zibanu_django-1.4.0/zibanu/django/template/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0 macercha  (1000) macercha  (1000)     1083 2024-03-11 02:33:38.000000 zibanu_django-1.4.0/zibanu/django/template/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-05-10 10:13:50.274908 zibanu_django-1.4.0/zibanu/django/template/templatetags/
--rw-r--r--   0 macercha  (1000) macercha  (1000)      501 2024-03-11 02:33:38.000000 zibanu_django-1.4.0/zibanu/django/template/templatetags/__init__.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)     2317 2024-03-11 02:33:38.000000 zibanu_django-1.4.0/zibanu/django/template/templatetags/static_uri.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)      889 2024-03-11 02:33:38.000000 zibanu_django-1.4.0/zibanu/django/template/templatetags/string_concat.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)     2673 2024-03-11 02:33:38.000000 zibanu_django-1.4.0/zibanu/django/template/templatetags/subtotal_dict.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)     1549 2024-03-11 02:33:38.000000 zibanu_django-1.4.0/zibanu/django/template/templatetags/sum_dict.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)      809 2024-04-04 21:09:36.000000 zibanu_django-1.4.0/zibanu/django/urls.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-05-10 10:13:50.275908 zibanu_django-1.4.0/zibanu/django/utils/
--rw-r--r--   0 macercha  (1000) macercha  (1000)     1075 2024-03-12 21:02:22.000000 zibanu_django-1.4.0/zibanu/django/utils/__init__.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)     1986 2024-03-11 02:33:38.000000 zibanu_django-1.4.0/zibanu/django/utils/date_time.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)     1168 2024-03-11 02:33:38.000000 zibanu_django-1.4.0/zibanu/django/utils/error_messages.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)     1770 2024-05-03 10:58:52.000000 zibanu_django-1.4.0/zibanu/django/utils/generic_utils.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)     7608 2024-03-11 02:33:38.000000 zibanu_django-1.4.0/zibanu/django/utils/mail.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)     2423 2024-03-11 02:33:38.000000 zibanu_django-1.4.0/zibanu/django/utils/model_utils.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)     1263 2024-03-11 02:33:38.000000 zibanu_django-1.4.0/zibanu/django/utils/receivers_utils.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)     1511 2024-03-11 02:33:38.000000 zibanu_django-1.4.0/zibanu/django/utils/request_utils.py
--rw-r--r--   0 macercha  (1000) macercha  (1000)     1559 2024-03-11 02:33:38.000000 zibanu_django-1.4.0/zibanu/django/utils/user_utils.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-05-10 10:13:50.276908 zibanu_django-1.4.0/zibanu_django.egg-info/
--rw-r--r--   0 macercha  (1000) macercha  (1000)    68384 2024-05-10 10:13:50.000000 zibanu_django-1.4.0/zibanu_django.egg-info/PKG-INFO
--rw-r--r--   0 macercha  (1000) macercha  (1000)     3188 2024-05-10 10:13:50.000000 zibanu_django-1.4.0/zibanu_django.egg-info/SOURCES.txt
--rw-r--r--   0 macercha  (1000) macercha  (1000)        1 2024-05-10 10:13:50.000000 zibanu_django-1.4.0/zibanu_django.egg-info/dependency_links.txt
--rw-r--r--   0 macercha  (1000) macercha  (1000)       91 2024-05-10 10:13:50.000000 zibanu_django-1.4.0/zibanu_django.egg-info/requires.txt
--rw-r--r--   0 macercha  (1000) macercha  (1000)        7 2024-05-10 10:13:50.000000 zibanu_django-1.4.0/zibanu_django.egg-info/top_level.txt
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-05-03 11:31:01.395956 zibanu_django-1.4.0b0/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)    35148 2022-05-01 19:35:15.000000 zibanu_django-1.4.0b0/LICENSE
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      105 2023-08-07 23:22:31.000000 zibanu_django-1.4.0b0/MANIFEST.in
+-rw-r--r--   0 macercha  (1000) macercha  (1000)    68386 2024-05-03 11:31:01.394956 zibanu_django-1.4.0b0/PKG-INFO
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)    27020 2023-09-12 12:23:03.000000 zibanu_django-1.4.0b0/README.md
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1009 2024-05-03 10:34:00.000000 zibanu_django-1.4.0b0/pyproject.toml
+-rw-r--r--   0 macercha  (1000) macercha  (1000)       38 2024-05-03 11:31:01.395956 zibanu_django-1.4.0b0/setup.cfg
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-05-03 11:31:01.379957 zibanu_django-1.4.0b0/zibanu/
+-rw-r--r--   0 macercha  (1000) macercha  (1000)      618 2024-03-11 02:33:38.000000 zibanu_django-1.4.0b0/zibanu/__init__.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-05-03 11:31:01.380957 zibanu_django-1.4.0b0/zibanu/django/
+-rw-r--r--   0 macercha  (1000) macercha  (1000)      583 2024-05-03 11:17:35.000000 zibanu_django-1.4.0b0/zibanu/django/__init__.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-05-03 11:31:01.380957 zibanu_django-1.4.0b0/zibanu/django/api/
+-rw-r--r--   0 macercha  (1000) macercha  (1000)      312 2024-03-11 02:33:38.000000 zibanu_django-1.4.0b0/zibanu/django/api/__init__.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-05-03 11:31:01.381956 zibanu_django-1.4.0b0/zibanu/django/api/services/
+-rw-r--r--   0 macercha  (1000) macercha  (1000)      512 2024-04-04 21:09:36.000000 zibanu_django-1.4.0b0/zibanu/django/api/services/__init__.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     1040 2024-04-04 21:51:55.000000 zibanu_django-1.4.0b0/zibanu/django/api/services/dial_codes.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     1301 2024-03-11 02:33:38.000000 zibanu_django-1.4.0b0/zibanu/django/api/services/language.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     1280 2024-03-11 02:33:38.000000 zibanu_django-1.4.0b0/zibanu/django/api/services/timezone.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     1147 2024-03-11 02:33:38.000000 zibanu_django-1.4.0b0/zibanu/django/apps.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-05-03 11:31:01.381956 zibanu_django-1.4.0b0/zibanu/django/db/
+-rw-r--r--   0 macercha  (1000) macercha  (1000)      503 2024-03-11 02:33:38.000000 zibanu_django-1.4.0b0/zibanu/django/db/__init__.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-05-03 11:31:01.381956 zibanu_django-1.4.0b0/zibanu/django/db/backends/
+-rw-r--r--   0 macercha  (1000) macercha  (1000)      500 2024-03-11 02:33:38.000000 zibanu_django-1.4.0b0/zibanu/django/db/backends/__init__.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-05-03 11:31:01.382956 zibanu_django-1.4.0b0/zibanu/django/db/backends/oracle/
+-rw-r--r--   0 macercha  (1000) macercha  (1000)      500 2024-03-11 02:33:38.000000 zibanu_django-1.4.0b0/zibanu/django/db/backends/oracle/__init__.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     1572 2024-03-11 02:33:38.000000 zibanu_django-1.4.0b0/zibanu/django/db/backends/oracle/base.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-05-03 11:31:01.383957 zibanu_django-1.4.0b0/zibanu/django/db/models/
+-rw-r--r--   0 macercha  (1000) macercha  (1000)      799 2024-04-03 22:31:00.000000 zibanu_django-1.4.0b0/zibanu/django/db/models/__init__.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     1120 2024-03-11 02:33:38.000000 zibanu_django-1.4.0b0/zibanu/django/db/models/dated_model.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-05-03 11:31:01.383957 zibanu_django-1.4.0b0/zibanu/django/db/models/fields/
+-rw-r--r--   0 macercha  (1000) macercha  (1000)      372 2024-04-03 22:31:00.000000 zibanu_django-1.4.0b0/zibanu/django/db/models/fields/__init__.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     2261 2024-04-04 21:09:36.000000 zibanu_django-1.4.0b0/zibanu/django/db/models/fields/phone_field.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     1580 2024-05-03 11:24:21.000000 zibanu_django-1.4.0b0/zibanu/django/db/models/manager.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     2082 2024-03-11 02:33:38.000000 zibanu_django-1.4.0b0/zibanu/django/db/models/model.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-05-03 11:31:01.383957 zibanu_django-1.4.0b0/zibanu/django/lib/
+-rw-r--r--   0 macercha  (1000) macercha  (1000)      556 2024-04-03 22:31:00.000000 zibanu_django-1.4.0b0/zibanu/django/lib/__init__.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-05-03 11:31:01.384956 zibanu_django-1.4.0b0/zibanu/django/lib/classes/
+-rw-r--r--   0 macercha  (1000) macercha  (1000)      644 2024-03-11 02:33:38.000000 zibanu_django-1.4.0b0/zibanu/django/lib/classes/__init__.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     5879 2024-03-11 02:33:38.000000 zibanu_django-1.4.0b0/zibanu/django/lib/classes/code_generator.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     1182 2024-03-11 02:33:38.000000 zibanu_django-1.4.0b0/zibanu/django/lib/classes/extended_json_encoder.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)      731 2024-03-11 02:33:38.000000 zibanu_django-1.4.0b0/zibanu/django/lib/classes/model_name.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-05-03 11:31:01.385956 zibanu_django-1.4.0b0/zibanu/django/lib/enums/
+-rw-r--r--   0 macercha  (1000) macercha  (1000)      521 2024-04-04 21:09:36.000000 zibanu_django-1.4.0b0/zibanu/django/lib/enums/__init__.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     1943 2024-04-04 22:29:20.000000 zibanu_django-1.4.0b0/zibanu/django/lib/enums/dial_codes.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-05-03 11:31:01.377956 zibanu_django-1.4.0b0/zibanu/django/locale/
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-05-03 11:31:01.377956 zibanu_django-1.4.0b0/zibanu/django/locale/es/
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-05-03 11:31:01.385956 zibanu_django-1.4.0b0/zibanu/django/locale/es/LC_MESSAGES/
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     3239 2024-05-03 11:26:43.000000 zibanu_django-1.4.0b0/zibanu/django/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     7517 2024-05-03 11:26:33.000000 zibanu_django-1.4.0b0/zibanu/django/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-05-03 11:31:01.386956 zibanu_django-1.4.0b0/zibanu/django/rest_framework/
+-rw-r--r--   0 macercha  (1000) macercha  (1000)      503 2024-03-11 02:33:38.000000 zibanu_django-1.4.0b0/zibanu/django/rest_framework/__init__.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     2197 2024-03-13 14:44:10.000000 zibanu_django-1.4.0b0/zibanu/django/rest_framework/decorators.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-05-03 11:31:01.386956 zibanu_django-1.4.0b0/zibanu/django/rest_framework/exceptions/
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     1171 2024-03-15 01:58:14.000000 zibanu_django-1.4.0b0/zibanu/django/rest_framework/exceptions/__init__.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     3076 2024-03-15 01:58:14.000000 zibanu_django-1.4.0b0/zibanu/django/rest_framework/exceptions/api_exception.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)      850 2024-03-11 22:02:32.000000 zibanu_django-1.4.0b0/zibanu/django/rest_framework/exceptions/multiple_login_error.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)      957 2024-03-15 01:58:14.000000 zibanu_django-1.4.0b0/zibanu/django/rest_framework/exceptions/not_implemented_exception.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     1058 2024-03-18 23:17:34.000000 zibanu_django-1.4.0b0/zibanu/django/rest_framework/exceptions/permission_denied.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-05-03 11:31:01.387956 zibanu_django-1.4.0b0/zibanu/django/rest_framework/fields/
+-rw-r--r--   0 macercha  (1000) macercha  (1000)      718 2024-03-11 02:33:38.000000 zibanu_django-1.4.0b0/zibanu/django/rest_framework/fields/__init__.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     1343 2024-03-11 02:33:38.000000 zibanu_django-1.4.0b0/zibanu/django/rest_framework/fields/current_user_default.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     5815 2024-04-05 11:24:32.000000 zibanu_django-1.4.0b0/zibanu/django/rest_framework/fields/hybrid_image.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-05-03 11:31:01.387956 zibanu_django-1.4.0b0/zibanu/django/rest_framework/permissions/
+-rw-r--r--   0 macercha  (1000) macercha  (1000)      652 2024-03-11 02:33:38.000000 zibanu_django-1.4.0b0/zibanu/django/rest_framework/permissions/__init__.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     1174 2024-03-11 02:33:38.000000 zibanu_django-1.4.0b0/zibanu/django/rest_framework/permissions/is_owner_or_read_only.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-05-03 11:31:01.388956 zibanu_django-1.4.0b0/zibanu/django/rest_framework/serializers/
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     1649 2024-03-11 02:33:38.000000 zibanu_django-1.4.0b0/zibanu/django/rest_framework/serializers/__init__.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)      646 2024-03-11 02:33:38.000000 zibanu_django-1.4.0b0/zibanu/django/rest_framework/serializers/fields.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)      863 2024-03-11 02:33:38.000000 zibanu_django-1.4.0b0/zibanu/django/rest_framework/serializers/model_serializer.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     1031 2024-03-19 00:59:35.000000 zibanu_django-1.4.0b0/zibanu/django/rest_framework/utils.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-05-03 11:31:01.389956 zibanu_django-1.4.0b0/zibanu/django/rest_framework/viewsets/
+-rw-r--r--   0 macercha  (1000) macercha  (1000)      779 2024-03-19 00:59:46.000000 zibanu_django-1.4.0b0/zibanu/django/rest_framework/viewsets/__init__.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)    15232 2024-05-03 10:58:52.000000 zibanu_django-1.4.0b0/zibanu/django/rest_framework/viewsets/model_viewset.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     1737 2024-03-11 02:33:38.000000 zibanu_django-1.4.0b0/zibanu/django/rest_framework/viewsets/viewset.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-05-03 11:31:01.389956 zibanu_django-1.4.0b0/zibanu/django/template/
+-rw-r--r--   0 macercha  (1000) macercha  (1000)      501 2024-03-11 02:33:38.000000 zibanu_django-1.4.0b0/zibanu/django/template/__init__.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)      825 2024-03-11 02:33:38.000000 zibanu_django-1.4.0b0/zibanu/django/template/apps.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-05-03 11:31:01.390956 zibanu_django-1.4.0b0/zibanu/django/template/context_processors/
+-rw-r--r--   0 macercha  (1000) macercha  (1000)      619 2024-03-11 02:33:38.000000 zibanu_django-1.4.0b0/zibanu/django/template/context_processors/__init__.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     1055 2024-03-11 02:33:38.000000 zibanu_django-1.4.0b0/zibanu/django/template/context_processors/full_static_uri.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)      819 2024-03-11 02:33:38.000000 zibanu_django-1.4.0b0/zibanu/django/template/context_processors/site.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-05-03 11:31:01.378957 zibanu_django-1.4.0b0/zibanu/django/template/locale/
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-05-03 11:31:01.378957 zibanu_django-1.4.0b0/zibanu/django/template/locale/es/
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-05-03 11:31:01.390956 zibanu_django-1.4.0b0/zibanu/django/template/locale/es/LC_MESSAGES/
+-rw-r--r--   0 macercha  (1000) macercha  (1000)      709 2024-03-11 02:33:38.000000 zibanu_django-1.4.0b0/zibanu/django/template/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     1083 2024-03-11 02:33:38.000000 zibanu_django-1.4.0b0/zibanu/django/template/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-05-03 11:31:01.391956 zibanu_django-1.4.0b0/zibanu/django/template/templatetags/
+-rw-r--r--   0 macercha  (1000) macercha  (1000)      501 2024-03-11 02:33:38.000000 zibanu_django-1.4.0b0/zibanu/django/template/templatetags/__init__.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     2317 2024-03-11 02:33:38.000000 zibanu_django-1.4.0b0/zibanu/django/template/templatetags/static_uri.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)      889 2024-03-11 02:33:38.000000 zibanu_django-1.4.0b0/zibanu/django/template/templatetags/string_concat.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     2673 2024-03-11 02:33:38.000000 zibanu_django-1.4.0b0/zibanu/django/template/templatetags/subtotal_dict.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     1549 2024-03-11 02:33:38.000000 zibanu_django-1.4.0b0/zibanu/django/template/templatetags/sum_dict.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)      809 2024-04-04 21:09:36.000000 zibanu_django-1.4.0b0/zibanu/django/urls.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-05-03 11:31:01.393956 zibanu_django-1.4.0b0/zibanu/django/utils/
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     1075 2024-03-12 21:02:22.000000 zibanu_django-1.4.0b0/zibanu/django/utils/__init__.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     1986 2024-03-11 02:33:38.000000 zibanu_django-1.4.0b0/zibanu/django/utils/date_time.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     1168 2024-03-11 02:33:38.000000 zibanu_django-1.4.0b0/zibanu/django/utils/error_messages.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     1770 2024-05-03 10:58:52.000000 zibanu_django-1.4.0b0/zibanu/django/utils/generic_utils.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     7608 2024-03-11 02:33:38.000000 zibanu_django-1.4.0b0/zibanu/django/utils/mail.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     2423 2024-03-11 02:33:38.000000 zibanu_django-1.4.0b0/zibanu/django/utils/model_utils.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     1263 2024-03-11 02:33:38.000000 zibanu_django-1.4.0b0/zibanu/django/utils/receivers_utils.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     1511 2024-03-11 02:33:38.000000 zibanu_django-1.4.0b0/zibanu/django/utils/request_utils.py
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     1559 2024-03-11 02:33:38.000000 zibanu_django-1.4.0b0/zibanu/django/utils/user_utils.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2024-05-03 11:31:01.394956 zibanu_django-1.4.0b0/zibanu_django.egg-info/
+-rw-r--r--   0 macercha  (1000) macercha  (1000)    68386 2024-05-03 11:31:01.000000 zibanu_django-1.4.0b0/zibanu_django.egg-info/PKG-INFO
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     3188 2024-05-03 11:31:01.000000 zibanu_django-1.4.0b0/zibanu_django.egg-info/SOURCES.txt
+-rw-r--r--   0 macercha  (1000) macercha  (1000)        1 2024-05-03 11:31:01.000000 zibanu_django-1.4.0b0/zibanu_django.egg-info/dependency_links.txt
+-rw-r--r--   0 macercha  (1000) macercha  (1000)       91 2024-05-03 11:31:01.000000 zibanu_django-1.4.0b0/zibanu_django.egg-info/requires.txt
+-rw-r--r--   0 macercha  (1000) macercha  (1000)        7 2024-05-03 11:31:01.000000 zibanu_django-1.4.0b0/zibanu_django.egg-info/top_level.txt
```

### Comparing `zibanu_django-1.4.0/LICENSE` & `zibanu_django-1.4.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `zibanu_django-1.4.0/PKG-INFO` & `zibanu_django-1.4.0b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zibanu-django
-Version: 1.4.0
+Version: 1.4.0b0
 Summary: Zibanu library for django projects
 Author-email: Mario Cerón <mario.ceron@cqinversiones.co>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `zibanu_django-1.4.0/README.md` & `zibanu_django-1.4.0b0/README.md`

 * *Files identical despite different names*

### Comparing `zibanu_django-1.4.0/pyproject.toml` & `zibanu_django-1.4.0b0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `zibanu_django-1.4.0/zibanu/__init__.py` & `zibanu_django-1.4.0b0/zibanu/__init__.py`

 * *Files identical despite different names*

### Comparing `zibanu_django-1.4.0/zibanu/django/__init__.py` & `zibanu_django-1.4.0b0/zibanu/django/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 # Date:         11/12/22 6:06 PM
 # Project:      Zibanu Django Project
 # Module Name:  __init__.py
 # Description:
 # ****************************************************************
 from datetime import datetime
 now = datetime.now()
-__version__ = "1.4.0"
+__version__ = "1.4.0-beta.0"
```

### Comparing `zibanu_django-1.4.0/zibanu/django/api/services/__init__.py` & `zibanu_django-1.4.0b0/zibanu/django/api/services/__init__.py`

 * *Files identical despite different names*

### Comparing `zibanu_django-1.4.0/zibanu/django/api/services/dial_codes.py` & `zibanu_django-1.4.0b0/zibanu/django/api/services/dial_codes.py`

 * *Files identical despite different names*

### Comparing `zibanu_django-1.4.0/zibanu/django/api/services/language.py` & `zibanu_django-1.4.0b0/zibanu/django/api/services/language.py`

 * *Files identical despite different names*

### Comparing `zibanu_django-1.4.0/zibanu/django/api/services/timezone.py` & `zibanu_django-1.4.0b0/zibanu/django/api/services/timezone.py`

 * *Files identical despite different names*

### Comparing `zibanu_django-1.4.0/zibanu/django/apps.py` & `zibanu_django-1.4.0b0/zibanu/django/apps.py`

 * *Files identical despite different names*

### Comparing `zibanu_django-1.4.0/zibanu/django/db/backends/oracle/base.py` & `zibanu_django-1.4.0b0/zibanu/django/db/backends/oracle/base.py`

 * *Files identical despite different names*

### Comparing `zibanu_django-1.4.0/zibanu/django/db/models/__init__.py` & `zibanu_django-1.4.0b0/zibanu/django/db/models/__init__.py`

 * *Files identical despite different names*

### Comparing `zibanu_django-1.4.0/zibanu/django/db/models/dated_model.py` & `zibanu_django-1.4.0b0/zibanu/django/db/models/dated_model.py`

 * *Files identical despite different names*

### Comparing `zibanu_django-1.4.0/zibanu/django/db/models/fields/phone_field.py` & `zibanu_django-1.4.0b0/zibanu/django/db/models/fields/phone_field.py`

 * *Files identical despite different names*

### Comparing `zibanu_django-1.4.0/zibanu/django/db/models/manager.py` & `zibanu_django-1.4.0b0/zibanu/django/db/models/manager.py`

 * *Files identical despite different names*

### Comparing `zibanu_django-1.4.0/zibanu/django/db/models/model.py` & `zibanu_django-1.4.0b0/zibanu/django/db/models/model.py`

 * *Files identical despite different names*

### Comparing `zibanu_django-1.4.0/zibanu/django/lib/__init__.py` & `zibanu_django-1.4.0b0/zibanu/django/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `zibanu_django-1.4.0/zibanu/django/lib/classes/__init__.py` & `zibanu_django-1.4.0b0/zibanu/django/lib/classes/__init__.py`

 * *Files identical despite different names*

### Comparing `zibanu_django-1.4.0/zibanu/django/lib/classes/code_generator.py` & `zibanu_django-1.4.0b0/zibanu/django/lib/classes/code_generator.py`

 * *Files identical despite different names*

### Comparing `zibanu_django-1.4.0/zibanu/django/lib/classes/extended_json_encoder.py` & `zibanu_django-1.4.0b0/zibanu/django/lib/classes/extended_json_encoder.py`

 * *Files identical despite different names*

### Comparing `zibanu_django-1.4.0/zibanu/django/lib/classes/model_name.py` & `zibanu_django-1.4.0b0/zibanu/django/lib/classes/model_name.py`

 * *Files identical despite different names*

### Comparing `zibanu_django-1.4.0/zibanu/django/lib/enums/__init__.py` & `zibanu_django-1.4.0b0/zibanu/django/lib/enums/__init__.py`

 * *Files identical despite different names*

### Comparing `zibanu_django-1.4.0/zibanu/django/lib/enums/dial_codes.py` & `zibanu_django-1.4.0b0/zibanu/django/lib/enums/dial_codes.py`

 * *Files identical despite different names*

### Comparing `zibanu_django-1.4.0/zibanu/django/locale/es/LC_MESSAGES/django.mo` & `zibanu_django-1.4.0b0/zibanu/django/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `zibanu_django-1.4.0/zibanu/django/locale/es/LC_MESSAGES/django.po` & `zibanu_django-1.4.0b0/zibanu/django/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `zibanu_django-1.4.0/zibanu/django/rest_framework/decorators.py` & `zibanu_django-1.4.0b0/zibanu/django/rest_framework/decorators.py`

 * *Files identical despite different names*

### Comparing `zibanu_django-1.4.0/zibanu/django/rest_framework/exceptions/__init__.py` & `zibanu_django-1.4.0b0/zibanu/django/rest_framework/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `zibanu_django-1.4.0/zibanu/django/rest_framework/exceptions/api_exception.py` & `zibanu_django-1.4.0b0/zibanu/django/rest_framework/exceptions/api_exception.py`

 * *Files identical despite different names*

### Comparing `zibanu_django-1.4.0/zibanu/django/rest_framework/exceptions/multiple_login_error.py` & `zibanu_django-1.4.0b0/zibanu/django/rest_framework/exceptions/multiple_login_error.py`

 * *Files identical despite different names*

### Comparing `zibanu_django-1.4.0/zibanu/django/rest_framework/exceptions/not_implemented_exception.py` & `zibanu_django-1.4.0b0/zibanu/django/rest_framework/exceptions/not_implemented_exception.py`

 * *Files identical despite different names*

### Comparing `zibanu_django-1.4.0/zibanu/django/rest_framework/exceptions/permission_denied.py` & `zibanu_django-1.4.0b0/zibanu/django/rest_framework/exceptions/permission_denied.py`

 * *Files identical despite different names*

### Comparing `zibanu_django-1.4.0/zibanu/django/rest_framework/fields/__init__.py` & `zibanu_django-1.4.0b0/zibanu/django/rest_framework/fields/__init__.py`

 * *Files identical despite different names*

### Comparing `zibanu_django-1.4.0/zibanu/django/rest_framework/fields/current_user_default.py` & `zibanu_django-1.4.0b0/zibanu/django/rest_framework/fields/current_user_default.py`

 * *Files identical despite different names*

### Comparing `zibanu_django-1.4.0/zibanu/django/rest_framework/fields/hybrid_image.py` & `zibanu_django-1.4.0b0/zibanu/django/rest_framework/fields/hybrid_image.py`

 * *Files identical despite different names*

### Comparing `zibanu_django-1.4.0/zibanu/django/rest_framework/permissions/__init__.py` & `zibanu_django-1.4.0b0/zibanu/django/rest_framework/permissions/__init__.py`

 * *Files identical despite different names*

### Comparing `zibanu_django-1.4.0/zibanu/django/rest_framework/permissions/is_owner_or_read_only.py` & `zibanu_django-1.4.0b0/zibanu/django/rest_framework/permissions/is_owner_or_read_only.py`

 * *Files identical despite different names*

### Comparing `zibanu_django-1.4.0/zibanu/django/rest_framework/serializers/__init__.py` & `zibanu_django-1.4.0b0/zibanu/django/rest_framework/serializers/__init__.py`

 * *Files identical despite different names*

### Comparing `zibanu_django-1.4.0/zibanu/django/rest_framework/serializers/fields.py` & `zibanu_django-1.4.0b0/zibanu/django/rest_framework/serializers/fields.py`

 * *Files identical despite different names*

### Comparing `zibanu_django-1.4.0/zibanu/django/rest_framework/serializers/model_serializer.py` & `zibanu_django-1.4.0b0/zibanu/django/rest_framework/serializers/model_serializer.py`

 * *Files identical despite different names*

### Comparing `zibanu_django-1.4.0/zibanu/django/rest_framework/utils.py` & `zibanu_django-1.4.0b0/zibanu/django/rest_framework/utils.py`

 * *Files identical despite different names*

### Comparing `zibanu_django-1.4.0/zibanu/django/rest_framework/viewsets/__init__.py` & `zibanu_django-1.4.0b0/zibanu/django/rest_framework/viewsets/__init__.py`

 * *Files identical despite different names*

### Comparing `zibanu_django-1.4.0/zibanu/django/rest_framework/viewsets/model_viewset.py` & `zibanu_django-1.4.0b0/zibanu/django/rest_framework/viewsets/model_viewset.py`

 * *Files identical despite different names*

### Comparing `zibanu_django-1.4.0/zibanu/django/rest_framework/viewsets/viewset.py` & `zibanu_django-1.4.0b0/zibanu/django/rest_framework/viewsets/viewset.py`

 * *Files identical despite different names*

### Comparing `zibanu_django-1.4.0/zibanu/django/template/apps.py` & `zibanu_django-1.4.0b0/zibanu/django/template/apps.py`

 * *Files identical despite different names*

### Comparing `zibanu_django-1.4.0/zibanu/django/template/context_processors/__init__.py` & `zibanu_django-1.4.0b0/zibanu/django/template/context_processors/__init__.py`

 * *Files identical despite different names*

### Comparing `zibanu_django-1.4.0/zibanu/django/template/context_processors/full_static_uri.py` & `zibanu_django-1.4.0b0/zibanu/django/template/context_processors/full_static_uri.py`

 * *Files identical despite different names*

### Comparing `zibanu_django-1.4.0/zibanu/django/template/context_processors/site.py` & `zibanu_django-1.4.0b0/zibanu/django/template/context_processors/site.py`

 * *Files identical despite different names*

### Comparing `zibanu_django-1.4.0/zibanu/django/template/locale/es/LC_MESSAGES/django.mo` & `zibanu_django-1.4.0b0/zibanu/django/template/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `zibanu_django-1.4.0/zibanu/django/template/locale/es/LC_MESSAGES/django.po` & `zibanu_django-1.4.0b0/zibanu/django/template/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `zibanu_django-1.4.0/zibanu/django/template/templatetags/static_uri.py` & `zibanu_django-1.4.0b0/zibanu/django/template/templatetags/static_uri.py`

 * *Files identical despite different names*

### Comparing `zibanu_django-1.4.0/zibanu/django/template/templatetags/string_concat.py` & `zibanu_django-1.4.0b0/zibanu/django/template/templatetags/string_concat.py`

 * *Files identical despite different names*

### Comparing `zibanu_django-1.4.0/zibanu/django/template/templatetags/subtotal_dict.py` & `zibanu_django-1.4.0b0/zibanu/django/template/templatetags/subtotal_dict.py`

 * *Files identical despite different names*

### Comparing `zibanu_django-1.4.0/zibanu/django/template/templatetags/sum_dict.py` & `zibanu_django-1.4.0b0/zibanu/django/template/templatetags/sum_dict.py`

 * *Files identical despite different names*

### Comparing `zibanu_django-1.4.0/zibanu/django/urls.py` & `zibanu_django-1.4.0b0/zibanu/django/urls.py`

 * *Files identical despite different names*

### Comparing `zibanu_django-1.4.0/zibanu/django/utils/__init__.py` & `zibanu_django-1.4.0b0/zibanu/django/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `zibanu_django-1.4.0/zibanu/django/utils/date_time.py` & `zibanu_django-1.4.0b0/zibanu/django/utils/date_time.py`

 * *Files identical despite different names*

### Comparing `zibanu_django-1.4.0/zibanu/django/utils/error_messages.py` & `zibanu_django-1.4.0b0/zibanu/django/utils/error_messages.py`

 * *Files identical despite different names*

### Comparing `zibanu_django-1.4.0/zibanu/django/utils/generic_utils.py` & `zibanu_django-1.4.0b0/zibanu/django/utils/generic_utils.py`

 * *Files identical despite different names*

### Comparing `zibanu_django-1.4.0/zibanu/django/utils/mail.py` & `zibanu_django-1.4.0b0/zibanu/django/utils/mail.py`

 * *Files identical despite different names*

### Comparing `zibanu_django-1.4.0/zibanu/django/utils/model_utils.py` & `zibanu_django-1.4.0b0/zibanu/django/utils/model_utils.py`

 * *Files identical despite different names*

### Comparing `zibanu_django-1.4.0/zibanu/django/utils/receivers_utils.py` & `zibanu_django-1.4.0b0/zibanu/django/utils/receivers_utils.py`

 * *Files identical despite different names*

### Comparing `zibanu_django-1.4.0/zibanu/django/utils/request_utils.py` & `zibanu_django-1.4.0b0/zibanu/django/utils/request_utils.py`

 * *Files identical despite different names*

### Comparing `zibanu_django-1.4.0/zibanu/django/utils/user_utils.py` & `zibanu_django-1.4.0b0/zibanu/django/utils/user_utils.py`

 * *Files identical despite different names*

### Comparing `zibanu_django-1.4.0/zibanu_django.egg-info/PKG-INFO` & `zibanu_django-1.4.0b0/zibanu_django.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zibanu-django
-Version: 1.4.0
+Version: 1.4.0b0
 Summary: Zibanu library for django projects
 Author-email: Mario Cerón <mario.ceron@cqinversiones.co>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `zibanu_django-1.4.0/zibanu_django.egg-info/SOURCES.txt` & `zibanu_django-1.4.0b0/zibanu_django.egg-info/SOURCES.txt`

 * *Files identical despite different names*

