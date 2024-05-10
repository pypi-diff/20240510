# Comparing `tmp/djangocms-column-2.0.0.tar.gz` & `tmp/djangocms_column-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djangocms-column-2.0.0.tar", last modified: Mon Apr 11 16:24:13 2022, max compression
+gzip compressed data, was "djangocms_column-2.1.0.tar", last modified: Fri May 10 15:27:16 2024, max compression
```

## Comparing `djangocms-column-2.0.0.tar` & `djangocms_column-2.1.0.tar`

### file list

```diff
@@ -1,326 +1,327 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.784478 djangocms-column-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1496 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)      258 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2458 2022-04-11 16:24:13.784478 djangocms-column-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1266 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.768478 djangocms-column-2.0.0/djangocms_column/
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1419 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/cms_plugins.py
--rw-r--r--   0 runner    (1001) docker     (121)      931 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.768478 djangocms-column-2.0.0/djangocms_column/locale/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.760477 djangocms-column-2.0.0/djangocms_column/locale/af/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.768478 djangocms-column-2.0.0/djangocms_column/locale/af/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      484 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/af/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1298 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/af/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.760477 djangocms-column-2.0.0/djangocms_column/locale/ar/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.768478 djangocms-column-2.0.0/djangocms_column/locale/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     1191 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/ar/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1599 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/ar/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.760477 djangocms-column-2.0.0/djangocms_column/locale/be/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.768478 djangocms-column-2.0.0/djangocms_column/locale/be/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      559 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/be/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1373 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/be/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.760477 djangocms-column-2.0.0/djangocms_column/locale/bg/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.768478 djangocms-column-2.0.0/djangocms_column/locale/bg/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      516 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/bg/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1299 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/bg/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.760477 djangocms-column-2.0.0/djangocms_column/locale/bn/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.768478 djangocms-column-2.0.0/djangocms_column/locale/bn/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     1193 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/bn/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1616 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/bn/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.760477 djangocms-column-2.0.0/djangocms_column/locale/ca/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.768478 djangocms-column-2.0.0/djangocms_column/locale/ca/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     1048 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/ca/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1460 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/ca/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.760477 djangocms-column-2.0.0/djangocms_column/locale/cmn/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.772478 djangocms-column-2.0.0/djangocms_column/locale/cmn/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      488 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/cmn/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1302 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/cmn/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.760477 djangocms-column-2.0.0/djangocms_column/locale/cs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.772478 djangocms-column-2.0.0/djangocms_column/locale/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/cs/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1531 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/cs/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.760477 djangocms-column-2.0.0/djangocms_column/locale/cy/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.772478 djangocms-column-2.0.0/djangocms_column/locale/cy/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      510 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/cy/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1324 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/cy/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.760477 djangocms-column-2.0.0/djangocms_column/locale/da/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.772478 djangocms-column-2.0.0/djangocms_column/locale/da/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     1022 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/da/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1426 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/da/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.760477 djangocms-column-2.0.0/djangocms_column/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.772478 djangocms-column-2.0.0/djangocms_column/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     1037 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1554 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.760477 djangocms-column-2.0.0/djangocms_column/locale/el/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.772478 djangocms-column-2.0.0/djangocms_column/locale/el/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     1130 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/el/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1541 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/el/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.760477 djangocms-column-2.0.0/djangocms_column/locale/en/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.772478 djangocms-column-2.0.0/djangocms_column/locale/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      378 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1219 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/en/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.760477 djangocms-column-2.0.0/djangocms_column/locale/es/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.772478 djangocms-column-2.0.0/djangocms_column/locale/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     1049 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1464 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.760477 djangocms-column-2.0.0/djangocms_column/locale/es_AR/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.772478 djangocms-column-2.0.0/djangocms_column/locale/es_AR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     1059 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/es_AR/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1474 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/es_AR/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.760477 djangocms-column-2.0.0/djangocms_column/locale/es_BO/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.772478 djangocms-column-2.0.0/djangocms_column/locale/es_BO/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      519 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/es_BO/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1302 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/es_BO/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.760477 djangocms-column-2.0.0/djangocms_column/locale/es_DO/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.772478 djangocms-column-2.0.0/djangocms_column/locale/es_DO/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      494 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/es_DO/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1308 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/es_DO/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.760477 djangocms-column-2.0.0/djangocms_column/locale/et/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.772478 djangocms-column-2.0.0/djangocms_column/locale/et/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      849 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/et/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1391 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/et/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.760477 djangocms-column-2.0.0/djangocms_column/locale/eu/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.772478 djangocms-column-2.0.0/djangocms_column/locale/eu/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     1036 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/eu/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1451 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/eu/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.760477 djangocms-column-2.0.0/djangocms_column/locale/fa/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.772478 djangocms-column-2.0.0/djangocms_column/locale/fa/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     1063 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/fa/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1480 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/fa/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.760477 djangocms-column-2.0.0/djangocms_column/locale/fi/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.772478 djangocms-column-2.0.0/djangocms_column/locale/fi/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     1044 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/fi/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1462 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/fi/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.760477 djangocms-column-2.0.0/djangocms_column/locale/fr/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.772478 djangocms-column-2.0.0/djangocms_column/locale/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     1056 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1566 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.760477 djangocms-column-2.0.0/djangocms_column/locale/ga/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.772478 djangocms-column-2.0.0/djangocms_column/locale/ga/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      518 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/ga/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1332 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/ga/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.760477 djangocms-column-2.0.0/djangocms_column/locale/gl/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.772478 djangocms-column-2.0.0/djangocms_column/locale/gl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     1046 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/gl/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1478 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/gl/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.760477 djangocms-column-2.0.0/djangocms_column/locale/gu/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.772478 djangocms-column-2.0.0/djangocms_column/locale/gu/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      483 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/gu/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1297 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/gu/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.764478 djangocms-column-2.0.0/djangocms_column/locale/he/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.772478 djangocms-column-2.0.0/djangocms_column/locale/he/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     1067 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/he/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1477 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/he/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.764478 djangocms-column-2.0.0/djangocms_column/locale/hi/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.776478 djangocms-column-2.0.0/djangocms_column/locale/hi/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      529 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/hi/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1312 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/hi/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.764478 djangocms-column-2.0.0/djangocms_column/locale/hr/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.776478 djangocms-column-2.0.0/djangocms_column/locale/hr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      578 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/hr/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1361 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/hr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.764478 djangocms-column-2.0.0/djangocms_column/locale/hu/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.776478 djangocms-column-2.0.0/djangocms_column/locale/hu/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     1061 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/hu/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1512 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/hu/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.764478 djangocms-column-2.0.0/djangocms_column/locale/id/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.776478 djangocms-column-2.0.0/djangocms_column/locale/id/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     1021 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/id/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1446 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/id/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.764478 djangocms-column-2.0.0/djangocms_column/locale/is/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.776478 djangocms-column-2.0.0/djangocms_column/locale/is/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     1037 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/is/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1454 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/is/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.764478 djangocms-column-2.0.0/djangocms_column/locale/is_IS/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.776478 djangocms-column-2.0.0/djangocms_column/locale/is_IS/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      500 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/is_IS/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1314 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/is_IS/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.764478 djangocms-column-2.0.0/djangocms_column/locale/it/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.776478 djangocms-column-2.0.0/djangocms_column/locale/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     1050 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/it/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1510 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/it/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.764478 djangocms-column-2.0.0/djangocms_column/locale/ja/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.776478 djangocms-column-2.0.0/djangocms_column/locale/ja/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     1049 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/ja/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1465 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/ja/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.764478 djangocms-column-2.0.0/djangocms_column/locale/ka/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.776478 djangocms-column-2.0.0/djangocms_column/locale/ka/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      510 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/ka/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1293 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/ka/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.764478 djangocms-column-2.0.0/djangocms_column/locale/kk/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.776478 djangocms-column-2.0.0/djangocms_column/locale/kk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     1075 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/kk/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1485 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/kk/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.764478 djangocms-column-2.0.0/djangocms_column/locale/km/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.776478 djangocms-column-2.0.0/djangocms_column/locale/km/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      501 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/km/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1284 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/km/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.764478 djangocms-column-2.0.0/djangocms_column/locale/ko/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.776478 djangocms-column-2.0.0/djangocms_column/locale/ko/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      474 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/ko/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1288 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/ko/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.764478 djangocms-column-2.0.0/djangocms_column/locale/ko_KR/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.776478 djangocms-column-2.0.0/djangocms_column/locale/ko_KR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     1030 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/ko_KR/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1437 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/ko_KR/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.764478 djangocms-column-2.0.0/djangocms_column/locale/ku_IQ/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.776478 djangocms-column-2.0.0/djangocms_column/locale/ku_IQ/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      519 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/ku_IQ/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1302 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/ku_IQ/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.764478 djangocms-column-2.0.0/djangocms_column/locale/lt/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.776478 djangocms-column-2.0.0/djangocms_column/locale/lt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      585 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/lt/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1368 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/lt/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.764478 djangocms-column-2.0.0/djangocms_column/locale/lv/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.776478 djangocms-column-2.0.0/djangocms_column/locale/lv/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      502 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/lv/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1316 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/lv/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.764478 djangocms-column-2.0.0/djangocms_column/locale/mn/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.776478 djangocms-column-2.0.0/djangocms_column/locale/mn/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      484 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/mn/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1298 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/mn/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.764478 djangocms-column-2.0.0/djangocms_column/locale/mn_MN/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.776478 djangocms-column-2.0.0/djangocms_column/locale/mn_MN/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      763 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/mn_MN/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1408 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/mn_MN/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.764478 djangocms-column-2.0.0/djangocms_column/locale/mt/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.776478 djangocms-column-2.0.0/djangocms_column/locale/mt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      555 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/mt/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1369 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/mt/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.764478 djangocms-column-2.0.0/djangocms_column/locale/nb/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.776478 djangocms-column-2.0.0/djangocms_column/locale/nb/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      514 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/nb/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1297 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/nb/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.764478 djangocms-column-2.0.0/djangocms_column/locale/nl/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.780478 djangocms-column-2.0.0/djangocms_column/locale/nl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     1034 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/nl/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1495 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/nl/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.764478 djangocms-column-2.0.0/djangocms_column/locale/no/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.780478 djangocms-column-2.0.0/djangocms_column/locale/no/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     1028 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/no/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1496 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/no/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.764478 djangocms-column-2.0.0/djangocms_column/locale/pl/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.780478 djangocms-column-2.0.0/djangocms_column/locale/pl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     1104 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/pl/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1497 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/pl/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.764478 djangocms-column-2.0.0/djangocms_column/locale/pt/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.780478 djangocms-column-2.0.0/djangocms_column/locale/pt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     1045 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/pt/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1463 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/pt/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.764478 djangocms-column-2.0.0/djangocms_column/locale/pt_BR/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.780478 djangocms-column-2.0.0/djangocms_column/locale/pt_BR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     1059 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/pt_BR/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1486 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/pt_BR/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.764478 djangocms-column-2.0.0/djangocms_column/locale/ro/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.780478 djangocms-column-2.0.0/djangocms_column/locale/ro/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     1085 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/ro/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1494 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/ro/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.764478 djangocms-column-2.0.0/djangocms_column/locale/ru/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.780478 djangocms-column-2.0.0/djangocms_column/locale/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     1204 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1609 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.764478 djangocms-column-2.0.0/djangocms_column/locale/sk/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.780478 djangocms-column-2.0.0/djangocms_column/locale/sk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      531 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/sk/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1314 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/sk/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.764478 djangocms-column-2.0.0/djangocms_column/locale/sl/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.780478 djangocms-column-2.0.0/djangocms_column/locale/sl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      536 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/sl/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1350 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/sl/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.764478 djangocms-column-2.0.0/djangocms_column/locale/sl_SI/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.780478 djangocms-column-2.0.0/djangocms_column/locale/sl_SI/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      576 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/sl_SI/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1359 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/sl_SI/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.764478 djangocms-column-2.0.0/djangocms_column/locale/sq/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.780478 djangocms-column-2.0.0/djangocms_column/locale/sq/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      483 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/sq/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1297 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/sq/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.764478 djangocms-column-2.0.0/djangocms_column/locale/sq_AL/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.780478 djangocms-column-2.0.0/djangocms_column/locale/sq_AL/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      499 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/sq_AL/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1313 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/sq_AL/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.764478 djangocms-column-2.0.0/djangocms_column/locale/sr/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.780478 djangocms-column-2.0.0/djangocms_column/locale/sr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      556 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/sr/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1370 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/sr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.764478 djangocms-column-2.0.0/djangocms_column/locale/sr@latin/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.780478 djangocms-column-2.0.0/djangocms_column/locale/sr@latin/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      599 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/sr@latin/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1382 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/sr@latin/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.764478 djangocms-column-2.0.0/djangocms_column/locale/sv/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.780478 djangocms-column-2.0.0/djangocms_column/locale/sv/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     1037 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/sv/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1462 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/sv/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.764478 djangocms-column-2.0.0/djangocms_column/locale/ta/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.780478 djangocms-column-2.0.0/djangocms_column/locale/ta/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      526 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/ta/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1309 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/ta/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.764478 djangocms-column-2.0.0/djangocms_column/locale/th/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.780478 djangocms-column-2.0.0/djangocms_column/locale/th/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      472 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/th/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1286 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/th/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.764478 djangocms-column-2.0.0/djangocms_column/locale/th_TH/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.780478 djangocms-column-2.0.0/djangocms_column/locale/th_TH/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      474 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/th_TH/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1288 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/th_TH/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.764478 djangocms-column-2.0.0/djangocms_column/locale/tlh/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.780478 djangocms-column-2.0.0/djangocms_column/locale/tlh/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      483 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/tlh/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1297 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/tlh/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.764478 djangocms-column-2.0.0/djangocms_column/locale/tr/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.780478 djangocms-column-2.0.0/djangocms_column/locale/tr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     1042 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/tr/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1460 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/tr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.768478 djangocms-column-2.0.0/djangocms_column/locale/ug/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.784478 djangocms-column-2.0.0/djangocms_column/locale/ug/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      459 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/ug/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1273 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/ug/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.768478 djangocms-column-2.0.0/djangocms_column/locale/uk/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.784478 djangocms-column-2.0.0/djangocms_column/locale/uk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     1205 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/uk/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1618 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/uk/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.768478 djangocms-column-2.0.0/djangocms_column/locale/ur/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.784478 djangocms-column-2.0.0/djangocms_column/locale/ur/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/ur/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1293 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/ur/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.768478 djangocms-column-2.0.0/djangocms_column/locale/vi/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.784478 djangocms-column-2.0.0/djangocms_column/locale/vi/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      478 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/vi/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1292 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/vi/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.768478 djangocms-column-2.0.0/djangocms_column/locale/vi_VN/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.784478 djangocms-column-2.0.0/djangocms_column/locale/vi_VN/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      495 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/vi_VN/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1309 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/vi_VN/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.768478 djangocms-column-2.0.0/djangocms_column/locale/zh/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.784478 djangocms-column-2.0.0/djangocms_column/locale/zh/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      475 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/zh/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1289 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/zh/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.768478 djangocms-column-2.0.0/djangocms_column/locale/zh_CN/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.784478 djangocms-column-2.0.0/djangocms_column/locale/zh_CN/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     1014 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/zh_CN/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1426 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/zh_CN/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.768478 djangocms-column-2.0.0/djangocms_column/locale/zh_TW/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.784478 djangocms-column-2.0.0/djangocms_column/locale/zh_TW/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     1030 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/zh_TW/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1438 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/locale/zh_TW/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.784478 djangocms-column-2.0.0/djangocms_column/migrations/
--rw-r--r--   0 runner    (1001) docker     (121)     1210 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (121)      841 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/migrations/0002_auto_20160915_0818.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1342 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/models.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.768478 djangocms-column-2.0.0/djangocms_column/templates/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.768478 djangocms-column-2.0.0/djangocms_column/templates/cms/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.784478 djangocms-column-2.0.0/djangocms_column/templates/cms/plugins/
--rw-r--r--   0 runner    (1001) docker     (121)      194 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/templates/cms/plugins/column.html
--rw-r--r--   0 runner    (1001) docker     (121)     1932 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/templates/cms/plugins/column_edit.html
--rw-r--r--   0 runner    (1001) docker     (121)      183 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/djangocms_column/templates/cms/plugins/multi_column.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 16:24:13.768478 djangocms-column-2.0.0/djangocms_column.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2458 2022-04-11 16:24:13.000000 djangocms-column-2.0.0/djangocms_column.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     8060 2022-04-11 16:24:13.000000 djangocms-column-2.0.0/djangocms_column.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-11 16:24:13.000000 djangocms-column-2.0.0/djangocms_column.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-11 16:24:11.000000 djangocms-column-2.0.0/djangocms_column.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       30 2022-04-11 16:24:13.000000 djangocms-column-2.0.0/djangocms_column.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-04-11 16:24:13.000000 djangocms-column-2.0.0/djangocms_column.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      371 2022-04-11 16:24:13.784478 djangocms-column-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1743 2022-04-11 16:24:02.000000 djangocms-column-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.521073 djangocms_column-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-05-10 15:27:16.521073 djangocms_column-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.489074 djangocms_column-2.1.0/djangocms_column/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/cms_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.485073 djangocms_column-2.1.0/djangocms_column/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.469074 djangocms_column-2.1.0/djangocms_column/locale/af/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.489074 djangocms_column-2.1.0/djangocms_column/locale/af/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/af/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/af/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.469074 djangocms_column-2.1.0/djangocms_column/locale/ar/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.489074 djangocms_column-2.1.0/djangocms_column/locale/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/ar/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/ar/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.469074 djangocms_column-2.1.0/djangocms_column/locale/be/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.489074 djangocms_column-2.1.0/djangocms_column/locale/be/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/be/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/be/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.469074 djangocms_column-2.1.0/djangocms_column/locale/bg/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.493074 djangocms_column-2.1.0/djangocms_column/locale/bg/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/bg/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/bg/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.469074 djangocms_column-2.1.0/djangocms_column/locale/bn/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.493074 djangocms_column-2.1.0/djangocms_column/locale/bn/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/bn/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/bn/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.469074 djangocms_column-2.1.0/djangocms_column/locale/ca/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.493074 djangocms_column-2.1.0/djangocms_column/locale/ca/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/ca/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/ca/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.469074 djangocms_column-2.1.0/djangocms_column/locale/cmn/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.493074 djangocms_column-2.1.0/djangocms_column/locale/cmn/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/cmn/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/cmn/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.469074 djangocms_column-2.1.0/djangocms_column/locale/cs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.493074 djangocms_column-2.1.0/djangocms_column/locale/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/cs/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/cs/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.469074 djangocms_column-2.1.0/djangocms_column/locale/cy/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.493074 djangocms_column-2.1.0/djangocms_column/locale/cy/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/cy/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/cy/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.469074 djangocms_column-2.1.0/djangocms_column/locale/da/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.493074 djangocms_column-2.1.0/djangocms_column/locale/da/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/da/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/da/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.469074 djangocms_column-2.1.0/djangocms_column/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.493074 djangocms_column-2.1.0/djangocms_column/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.469074 djangocms_column-2.1.0/djangocms_column/locale/el/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.493074 djangocms_column-2.1.0/djangocms_column/locale/el/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/el/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/el/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.469074 djangocms_column-2.1.0/djangocms_column/locale/en/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.493074 djangocms_column-2.1.0/djangocms_column/locale/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/en/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.469074 djangocms_column-2.1.0/djangocms_column/locale/es/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.493074 djangocms_column-2.1.0/djangocms_column/locale/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.473074 djangocms_column-2.1.0/djangocms_column/locale/es_AR/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.497074 djangocms_column-2.1.0/djangocms_column/locale/es_AR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/es_AR/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/es_AR/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.473074 djangocms_column-2.1.0/djangocms_column/locale/es_BO/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.497074 djangocms_column-2.1.0/djangocms_column/locale/es_BO/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/es_BO/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/es_BO/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.473074 djangocms_column-2.1.0/djangocms_column/locale/es_DO/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.497074 djangocms_column-2.1.0/djangocms_column/locale/es_DO/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/es_DO/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/es_DO/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.473074 djangocms_column-2.1.0/djangocms_column/locale/et/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.497074 djangocms_column-2.1.0/djangocms_column/locale/et/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/et/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/et/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.473074 djangocms_column-2.1.0/djangocms_column/locale/eu/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.497074 djangocms_column-2.1.0/djangocms_column/locale/eu/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/eu/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/eu/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.473074 djangocms_column-2.1.0/djangocms_column/locale/fa/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.497074 djangocms_column-2.1.0/djangocms_column/locale/fa/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/fa/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/fa/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.473074 djangocms_column-2.1.0/djangocms_column/locale/fi/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.497074 djangocms_column-2.1.0/djangocms_column/locale/fi/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/fi/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/fi/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.473074 djangocms_column-2.1.0/djangocms_column/locale/fr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.497074 djangocms_column-2.1.0/djangocms_column/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.473074 djangocms_column-2.1.0/djangocms_column/locale/ga/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.497074 djangocms_column-2.1.0/djangocms_column/locale/ga/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/ga/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/ga/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.473074 djangocms_column-2.1.0/djangocms_column/locale/gl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.497074 djangocms_column-2.1.0/djangocms_column/locale/gl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/gl/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/gl/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.473074 djangocms_column-2.1.0/djangocms_column/locale/gu/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.501073 djangocms_column-2.1.0/djangocms_column/locale/gu/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/gu/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/gu/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.473074 djangocms_column-2.1.0/djangocms_column/locale/he/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.501073 djangocms_column-2.1.0/djangocms_column/locale/he/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/he/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/he/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.473074 djangocms_column-2.1.0/djangocms_column/locale/hi/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.501073 djangocms_column-2.1.0/djangocms_column/locale/hi/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/hi/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/hi/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.473074 djangocms_column-2.1.0/djangocms_column/locale/hr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.501073 djangocms_column-2.1.0/djangocms_column/locale/hr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/hr/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/hr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.473074 djangocms_column-2.1.0/djangocms_column/locale/hu/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.501073 djangocms_column-2.1.0/djangocms_column/locale/hu/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/hu/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/hu/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.473074 djangocms_column-2.1.0/djangocms_column/locale/id/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.501073 djangocms_column-2.1.0/djangocms_column/locale/id/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/id/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/id/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.477074 djangocms_column-2.1.0/djangocms_column/locale/is/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.501073 djangocms_column-2.1.0/djangocms_column/locale/is/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/is/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/is/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.477074 djangocms_column-2.1.0/djangocms_column/locale/is_IS/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.501073 djangocms_column-2.1.0/djangocms_column/locale/is_IS/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/is_IS/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/is_IS/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.477074 djangocms_column-2.1.0/djangocms_column/locale/it/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.501073 djangocms_column-2.1.0/djangocms_column/locale/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/it/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/it/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.477074 djangocms_column-2.1.0/djangocms_column/locale/ja/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.501073 djangocms_column-2.1.0/djangocms_column/locale/ja/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/ja/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/ja/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.477074 djangocms_column-2.1.0/djangocms_column/locale/ka/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.501073 djangocms_column-2.1.0/djangocms_column/locale/ka/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/ka/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/ka/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.477074 djangocms_column-2.1.0/djangocms_column/locale/kk/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.505074 djangocms_column-2.1.0/djangocms_column/locale/kk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/kk/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/kk/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.477074 djangocms_column-2.1.0/djangocms_column/locale/km/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.505074 djangocms_column-2.1.0/djangocms_column/locale/km/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/km/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/km/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.477074 djangocms_column-2.1.0/djangocms_column/locale/ko/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.505074 djangocms_column-2.1.0/djangocms_column/locale/ko/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/ko/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/ko/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.477074 djangocms_column-2.1.0/djangocms_column/locale/ko_KR/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.505074 djangocms_column-2.1.0/djangocms_column/locale/ko_KR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/ko_KR/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/ko_KR/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.477074 djangocms_column-2.1.0/djangocms_column/locale/ku_IQ/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.505074 djangocms_column-2.1.0/djangocms_column/locale/ku_IQ/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/ku_IQ/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/ku_IQ/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.477074 djangocms_column-2.1.0/djangocms_column/locale/lt/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.505074 djangocms_column-2.1.0/djangocms_column/locale/lt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/lt/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/lt/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.477074 djangocms_column-2.1.0/djangocms_column/locale/lv/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.505074 djangocms_column-2.1.0/djangocms_column/locale/lv/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/lv/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/lv/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.477074 djangocms_column-2.1.0/djangocms_column/locale/mn/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.505074 djangocms_column-2.1.0/djangocms_column/locale/mn/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/mn/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/mn/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.477074 djangocms_column-2.1.0/djangocms_column/locale/mn_MN/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.505074 djangocms_column-2.1.0/djangocms_column/locale/mn_MN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/mn_MN/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/mn_MN/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.477074 djangocms_column-2.1.0/djangocms_column/locale/mt/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.505074 djangocms_column-2.1.0/djangocms_column/locale/mt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/mt/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/mt/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.477074 djangocms_column-2.1.0/djangocms_column/locale/nb/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.505074 djangocms_column-2.1.0/djangocms_column/locale/nb/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/nb/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/nb/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.481073 djangocms_column-2.1.0/djangocms_column/locale/nl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.509074 djangocms_column-2.1.0/djangocms_column/locale/nl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/nl/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/nl/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.481073 djangocms_column-2.1.0/djangocms_column/locale/no/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.509074 djangocms_column-2.1.0/djangocms_column/locale/no/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/no/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/no/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.481073 djangocms_column-2.1.0/djangocms_column/locale/pl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.509074 djangocms_column-2.1.0/djangocms_column/locale/pl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/pl/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/pl/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.481073 djangocms_column-2.1.0/djangocms_column/locale/pt/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.509074 djangocms_column-2.1.0/djangocms_column/locale/pt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/pt/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/pt/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.481073 djangocms_column-2.1.0/djangocms_column/locale/pt_BR/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.509074 djangocms_column-2.1.0/djangocms_column/locale/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/pt_BR/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/pt_BR/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.481073 djangocms_column-2.1.0/djangocms_column/locale/ro/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.509074 djangocms_column-2.1.0/djangocms_column/locale/ro/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/ro/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/ro/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.481073 djangocms_column-2.1.0/djangocms_column/locale/ru/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.509074 djangocms_column-2.1.0/djangocms_column/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.481073 djangocms_column-2.1.0/djangocms_column/locale/sk/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.509074 djangocms_column-2.1.0/djangocms_column/locale/sk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/sk/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/sk/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.481073 djangocms_column-2.1.0/djangocms_column/locale/sl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.509074 djangocms_column-2.1.0/djangocms_column/locale/sl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/sl/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/sl/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.481073 djangocms_column-2.1.0/djangocms_column/locale/sl_SI/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.509074 djangocms_column-2.1.0/djangocms_column/locale/sl_SI/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/sl_SI/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/sl_SI/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.481073 djangocms_column-2.1.0/djangocms_column/locale/sq/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.509074 djangocms_column-2.1.0/djangocms_column/locale/sq/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/sq/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/sq/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.481073 djangocms_column-2.1.0/djangocms_column/locale/sq_AL/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.513074 djangocms_column-2.1.0/djangocms_column/locale/sq_AL/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/sq_AL/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/sq_AL/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.481073 djangocms_column-2.1.0/djangocms_column/locale/sr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.513074 djangocms_column-2.1.0/djangocms_column/locale/sr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/sr/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/sr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.481073 djangocms_column-2.1.0/djangocms_column/locale/sr@latin/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.513074 djangocms_column-2.1.0/djangocms_column/locale/sr@latin/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/sr@latin/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/sr@latin/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.481073 djangocms_column-2.1.0/djangocms_column/locale/sv/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.513074 djangocms_column-2.1.0/djangocms_column/locale/sv/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/sv/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/sv/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.485073 djangocms_column-2.1.0/djangocms_column/locale/ta/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.513074 djangocms_column-2.1.0/djangocms_column/locale/ta/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/ta/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/ta/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.485073 djangocms_column-2.1.0/djangocms_column/locale/th/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.513074 djangocms_column-2.1.0/djangocms_column/locale/th/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/th/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/th/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.485073 djangocms_column-2.1.0/djangocms_column/locale/th_TH/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.513074 djangocms_column-2.1.0/djangocms_column/locale/th_TH/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/th_TH/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/th_TH/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.485073 djangocms_column-2.1.0/djangocms_column/locale/tlh/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.513074 djangocms_column-2.1.0/djangocms_column/locale/tlh/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/tlh/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/tlh/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.485073 djangocms_column-2.1.0/djangocms_column/locale/tr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.513074 djangocms_column-2.1.0/djangocms_column/locale/tr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/tr/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/tr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.485073 djangocms_column-2.1.0/djangocms_column/locale/ug/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.513074 djangocms_column-2.1.0/djangocms_column/locale/ug/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/ug/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/ug/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.485073 djangocms_column-2.1.0/djangocms_column/locale/uk/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.517073 djangocms_column-2.1.0/djangocms_column/locale/uk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/uk/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/uk/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.485073 djangocms_column-2.1.0/djangocms_column/locale/ur/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.517073 djangocms_column-2.1.0/djangocms_column/locale/ur/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/ur/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/ur/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.485073 djangocms_column-2.1.0/djangocms_column/locale/vi/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.517073 djangocms_column-2.1.0/djangocms_column/locale/vi/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/vi/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/vi/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.485073 djangocms_column-2.1.0/djangocms_column/locale/vi_VN/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.517073 djangocms_column-2.1.0/djangocms_column/locale/vi_VN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/vi_VN/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/vi_VN/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.485073 djangocms_column-2.1.0/djangocms_column/locale/zh/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.517073 djangocms_column-2.1.0/djangocms_column/locale/zh/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/zh/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/zh/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.485073 djangocms_column-2.1.0/djangocms_column/locale/zh_CN/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.517073 djangocms_column-2.1.0/djangocms_column/locale/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/zh_CN/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/zh_CN/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.485073 djangocms_column-2.1.0/djangocms_column/locale/zh_TW/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.517073 djangocms_column-2.1.0/djangocms_column/locale/zh_TW/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/zh_TW/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/locale/zh_TW/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.517073 djangocms_column-2.1.0/djangocms_column/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/migrations/0002_auto_20160915_0818.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/migrations/0003_alter_column_cmsplugin_ptr_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.485073 djangocms_column-2.1.0/djangocms_column/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.485073 djangocms_column-2.1.0/djangocms_column/templates/cms/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.517073 djangocms_column-2.1.0/djangocms_column/templates/cms/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/templates/cms/plugins/column.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/templates/cms/plugins/column_edit.html
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/djangocms_column/templates/cms/plugins/multi_column.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:27:16.517073 djangocms_column-2.1.0/djangocms_column.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-05-10 15:27:16.000000 djangocms_column-2.1.0/djangocms_column.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8132 2024-05-10 15:27:16.000000 djangocms_column-2.1.0/djangocms_column.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 15:27:16.000000 djangocms_column-2.1.0/djangocms_column.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 15:27:16.000000 djangocms_column-2.1.0/djangocms_column.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-10 15:27:16.000000 djangocms_column-2.1.0/djangocms_column.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-10 15:27:16.000000 djangocms_column-2.1.0/djangocms_column.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-10 15:27:16.521073 djangocms_column-2.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-05-10 15:27:12.000000 djangocms_column-2.1.0/setup.py
```

### Comparing `djangocms-column-2.0.0/LICENSE.txt` & `djangocms_column-2.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/PKG-INFO` & `djangocms_column-2.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,47 +1,53 @@
 Metadata-Version: 2.1
 Name: djangocms-column
-Version: 2.0.0
+Version: 2.1.0
 Summary: Column Plugin for django CMS
 Home-page: https://github.com/django-cms/djangocms-column
 Author: Django CMS Association and contributors
 Author-email: info@django-cms.org
 License: LICENSE.txt
 Platform: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.2
+Classifier: Framework :: Django :: 5.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Communications
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content :: Message Boards
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
+Requires-Dist: django-cms>=3.8.0
+Requires-Dist: Django>=2.2
 
 djangocms-column
 ================
 
 A Multi Column Plugin for django CMS.
 
 
 Installation
 ------------
 
-This plugin requires `django CMS` 3.8 or higher to be properly installed.
+This plugin requires `django CMS` 3.8 or higher, or 4.0 or higher to be properly installed.
 
 * In your projects virtualenv, run ``pip install djangocms-column``.
 * Add ``'djangocms_column'`` to your ``INSTALLED_APPS`` setting.
 * Run ``manage.py migrate djangocms_column``.
 
 
 Usage
@@ -71,9 +77,7 @@
 
 Translations
 ------------
 
 If you want to help translate the plugin please do it on transifex:
 
 https://www.transifex.com/projects/p/django-cms/resource/djangocms-column/
-
-
```

### Comparing `djangocms-column-2.0.0/README.rst` & `djangocms_column-2.1.0/README.rst`

 * *Files 15% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 A Multi Column Plugin for django CMS.
 
 
 Installation
 ------------
 
-This plugin requires `django CMS` 3.8 or higher to be properly installed.
+This plugin requires `django CMS` 3.8 or higher, or 4.0 or higher to be properly installed.
 
 * In your projects virtualenv, run ``pip install djangocms-column``.
 * Add ``'djangocms_column'`` to your ``INSTALLED_APPS`` setting.
 * Run ``manage.py migrate djangocms_column``.
 
 
 Usage
```

### Comparing `djangocms-column-2.0.0/djangocms_column/cms_plugins.py` & `djangocms_column-2.1.0/djangocms_column/cms_plugins.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from django.utils.translation import gettext_lazy as _
 
-from cms.models import CMSPlugin
+from cms import api
 from cms.plugin_base import CMSPluginBase
 from cms.plugin_pool import plugin_pool
 
 from .forms import MultiColumnForm
 from .models import Column, MultiColumns
 
 
@@ -18,21 +18,20 @@
     form = MultiColumnForm
 
     def save_model(self, request, obj, form, change):
         response = super().save_model(
             request, obj, form, change
         )
         for _x in range(int(form.cleaned_data['create'])):
-            col = Column(
-                parent=obj,
+            col = api.add_plugin(
                 placeholder=obj.placeholder,
+                plugin_type=ColumnPlugin.__name__,
                 language=obj.language,
+                target=obj,
                 width=form.cleaned_data['create_width'],
-                position=CMSPlugin.objects.filter(parent=obj).count(),
-                plugin_type=ColumnPlugin.__name__
             )
             col.save()
         return response
 
 
 class ColumnPlugin(CMSPluginBase):
     model = Column
```

### Comparing `djangocms-column-2.0.0/djangocms_column/forms.py` & `djangocms_column-2.1.0/djangocms_column/forms.py`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column/locale/af/LC_MESSAGES/django.po` & `djangocms_column-2.1.0/djangocms_column/locale/af/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column/locale/ar/LC_MESSAGES/django.mo` & `djangocms_column-2.1.0/djangocms_column/locale/ar/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column/locale/ar/LC_MESSAGES/django.po` & `djangocms_column-2.1.0/djangocms_column/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column/locale/be/LC_MESSAGES/django.mo` & `djangocms_column-2.1.0/djangocms_column/locale/be/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column/locale/be/LC_MESSAGES/django.po` & `djangocms_column-2.1.0/djangocms_column/locale/be/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column/locale/bg/LC_MESSAGES/django.mo` & `djangocms_column-2.1.0/djangocms_column/locale/bg/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column/locale/bg/LC_MESSAGES/django.po` & `djangocms_column-2.1.0/djangocms_column/locale/bg/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column/locale/bn/LC_MESSAGES/django.mo` & `djangocms_column-2.1.0/djangocms_column/locale/bn/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column/locale/bn/LC_MESSAGES/django.po` & `djangocms_column-2.1.0/djangocms_column/locale/bn/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column/locale/ca/LC_MESSAGES/django.mo` & `djangocms_column-2.1.0/djangocms_column/locale/ca/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column/locale/ca/LC_MESSAGES/django.po` & `djangocms_column-2.1.0/djangocms_column/locale/ca/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column/locale/cmn/LC_MESSAGES/django.po` & `djangocms_column-2.1.0/djangocms_column/locale/cmn/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column/locale/cs/LC_MESSAGES/django.mo` & `djangocms_column-2.1.0/djangocms_column/locale/cs/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column/locale/cs/LC_MESSAGES/django.po` & `djangocms_column-2.1.0/djangocms_column/locale/cs/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column/locale/cy/LC_MESSAGES/django.po` & `djangocms_column-2.1.0/djangocms_column/locale/cy/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column/locale/da/LC_MESSAGES/django.mo` & `djangocms_column-2.1.0/djangocms_column/locale/da/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column/locale/da/LC_MESSAGES/django.po` & `djangocms_column-2.1.0/djangocms_column/locale/da/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column/locale/de/LC_MESSAGES/django.mo` & `djangocms_column-2.1.0/djangocms_column/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column/locale/de/LC_MESSAGES/django.po` & `djangocms_column-2.1.0/djangocms_column/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column/locale/el/LC_MESSAGES/django.mo` & `djangocms_column-2.1.0/djangocms_column/locale/el/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column/locale/el/LC_MESSAGES/django.po` & `djangocms_column-2.1.0/djangocms_column/locale/el/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column/locale/en/LC_MESSAGES/django.po` & `djangocms_column-2.1.0/djangocms_column/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column/locale/es/LC_MESSAGES/django.mo` & `djangocms_column-2.1.0/djangocms_column/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column/locale/es/LC_MESSAGES/django.po` & `djangocms_column-2.1.0/djangocms_column/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column/locale/es_AR/LC_MESSAGES/django.mo` & `djangocms_column-2.1.0/djangocms_column/locale/es_AR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column/locale/es_AR/LC_MESSAGES/django.po` & `djangocms_column-2.1.0/djangocms_column/locale/es_AR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column/locale/es_BO/LC_MESSAGES/django.mo` & `djangocms_column-2.1.0/djangocms_column/locale/es_BO/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column/locale/es_BO/LC_MESSAGES/django.po` & `djangocms_column-2.1.0/djangocms_column/locale/es_BO/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column/locale/es_DO/LC_MESSAGES/django.po` & `djangocms_column-2.1.0/djangocms_column/locale/es_DO/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column/locale/et/LC_MESSAGES/django.mo` & `djangocms_column-2.1.0/djangocms_column/locale/et/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column/locale/et/LC_MESSAGES/django.po` & `djangocms_column-2.1.0/djangocms_column/locale/et/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column/locale/eu/LC_MESSAGES/django.mo` & `djangocms_column-2.1.0/djangocms_column/locale/eu/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column/locale/eu/LC_MESSAGES/django.po` & `djangocms_column-2.1.0/djangocms_column/locale/eu/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column/locale/fa/LC_MESSAGES/django.mo` & `djangocms_column-2.1.0/djangocms_column/locale/fa/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column/locale/fa/LC_MESSAGES/django.po` & `djangocms_column-2.1.0/djangocms_column/locale/fa/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column/locale/fi/LC_MESSAGES/django.mo` & `djangocms_column-2.1.0/djangocms_column/locale/fi/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column/locale/fi/LC_MESSAGES/django.po` & `djangocms_column-2.1.0/djangocms_column/locale/fi/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column/locale/fr/LC_MESSAGES/django.mo` & `djangocms_column-2.1.0/djangocms_column/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column/locale/fr/LC_MESSAGES/django.po` & `djangocms_column-2.1.0/djangocms_column/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column/locale/ga/LC_MESSAGES/django.mo` & `djangocms_column-2.1.0/djangocms_column/locale/ga/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column/locale/ga/LC_MESSAGES/django.po` & `djangocms_column-2.1.0/djangocms_column/locale/ga/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column/locale/gl/LC_MESSAGES/django.mo` & `djangocms_column-2.1.0/djangocms_column/locale/gl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column/locale/gl/LC_MESSAGES/django.po` & `djangocms_column-2.1.0/djangocms_column/locale/gl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column/locale/gu/LC_MESSAGES/django.po` & `djangocms_column-2.1.0/djangocms_column/locale/gu/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column/locale/he/LC_MESSAGES/django.mo` & `djangocms_column-2.1.0/djangocms_column/locale/he/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column/locale/he/LC_MESSAGES/django.po` & `djangocms_column-2.1.0/djangocms_column/locale/he/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column/locale/hi/LC_MESSAGES/django.mo` & `djangocms_column-2.1.0/djangocms_column/locale/hi/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column/locale/hi/LC_MESSAGES/django.po` & `djangocms_column-2.1.0/djangocms_column/locale/hi/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column/locale/hr/LC_MESSAGES/django.mo` & `djangocms_column-2.1.0/djangocms_column/locale/hr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column/locale/hr/LC_MESSAGES/django.po` & `djangocms_column-2.1.0/djangocms_column/locale/hr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column/locale/hu/LC_MESSAGES/django.mo` & `djangocms_column-2.1.0/djangocms_column/locale/hu/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column/locale/hu/LC_MESSAGES/django.po` & `djangocms_column-2.1.0/djangocms_column/locale/hu/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column/locale/id/LC_MESSAGES/django.mo` & `djangocms_column-2.1.0/djangocms_column/locale/id/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column/locale/id/LC_MESSAGES/django.po` & `djangocms_column-2.1.0/djangocms_column/locale/id/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column/locale/is/LC_MESSAGES/django.mo` & `djangocms_column-2.1.0/djangocms_column/locale/is/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column/locale/is/LC_MESSAGES/django.po` & `djangocms_column-2.1.0/djangocms_column/locale/is/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column/locale/is_IS/LC_MESSAGES/django.po` & `djangocms_column-2.1.0/djangocms_column/locale/is_IS/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column/locale/it/LC_MESSAGES/django.mo` & `djangocms_column-2.1.0/djangocms_column/locale/it/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column/locale/it/LC_MESSAGES/django.po` & `djangocms_column-2.1.0/djangocms_column/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column/locale/ja/LC_MESSAGES/django.mo` & `djangocms_column-2.1.0/djangocms_column/locale/ja/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column/locale/ja/LC_MESSAGES/django.po` & `djangocms_column-2.1.0/djangocms_column/locale/ja/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column/locale/ka/LC_MESSAGES/django.po` & `djangocms_column-2.1.0/djangocms_column/locale/ka/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column/locale/kk/LC_MESSAGES/django.mo` & `djangocms_column-2.1.0/djangocms_column/locale/kk/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column/locale/kk/LC_MESSAGES/django.po` & `djangocms_column-2.1.0/djangocms_column/locale/kk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column/locale/km/LC_MESSAGES/django.po` & `djangocms_column-2.1.0/djangocms_column/locale/km/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column/locale/ko/LC_MESSAGES/django.po` & `djangocms_column-2.1.0/djangocms_column/locale/ko/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column/locale/ko_KR/LC_MESSAGES/django.mo` & `djangocms_column-2.1.0/djangocms_column/locale/ko_KR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column/locale/ko_KR/LC_MESSAGES/django.po` & `djangocms_column-2.1.0/djangocms_column/locale/ko_KR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column/locale/ku_IQ/LC_MESSAGES/django.mo` & `djangocms_column-2.1.0/djangocms_column/locale/ku_IQ/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column/locale/ku_IQ/LC_MESSAGES/django.po` & `djangocms_column-2.1.0/djangocms_column/locale/ku_IQ/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column/locale/lt/LC_MESSAGES/django.mo` & `djangocms_column-2.1.0/djangocms_column/locale/lt/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column/locale/lt/LC_MESSAGES/django.po` & `djangocms_column-2.1.0/djangocms_column/locale/lt/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column/locale/lv/LC_MESSAGES/django.po` & `djangocms_column-2.1.0/djangocms_column/locale/lv/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column/locale/mn/LC_MESSAGES/django.po` & `djangocms_column-2.1.0/djangocms_column/locale/mn/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column/locale/mn_MN/LC_MESSAGES/django.mo` & `djangocms_column-2.1.0/djangocms_column/locale/mn_MN/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column/locale/mn_MN/LC_MESSAGES/django.po` & `djangocms_column-2.1.0/djangocms_column/locale/mn_MN/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column/locale/mt/LC_MESSAGES/django.mo` & `djangocms_column-2.1.0/djangocms_column/locale/mt/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column/locale/mt/LC_MESSAGES/django.po` & `djangocms_column-2.1.0/djangocms_column/locale/mt/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column/locale/nb/LC_MESSAGES/django.mo` & `djangocms_column-2.1.0/djangocms_column/locale/nb/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column/locale/nb/LC_MESSAGES/django.po` & `djangocms_column-2.1.0/djangocms_column/locale/nb/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column/locale/nl/LC_MESSAGES/django.mo` & `djangocms_column-2.1.0/djangocms_column/locale/nl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column/locale/nl/LC_MESSAGES/django.po` & `djangocms_column-2.1.0/djangocms_column/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column/locale/no/LC_MESSAGES/django.mo` & `djangocms_column-2.1.0/djangocms_column/locale/no/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column/locale/no/LC_MESSAGES/django.po` & `djangocms_column-2.1.0/djangocms_column/locale/no/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column/locale/pl/LC_MESSAGES/django.mo` & `djangocms_column-2.1.0/djangocms_column/locale/pl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column/locale/pl/LC_MESSAGES/django.po` & `djangocms_column-2.1.0/djangocms_column/locale/pl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column/locale/pt/LC_MESSAGES/django.mo` & `djangocms_column-2.1.0/djangocms_column/locale/pt/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column/locale/pt/LC_MESSAGES/django.po` & `djangocms_column-2.1.0/djangocms_column/locale/pt/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column/locale/pt_BR/LC_MESSAGES/django.mo` & `djangocms_column-2.1.0/djangocms_column/locale/pt_BR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column/locale/pt_BR/LC_MESSAGES/django.po` & `djangocms_column-2.1.0/djangocms_column/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column/locale/ro/LC_MESSAGES/django.mo` & `djangocms_column-2.1.0/djangocms_column/locale/ro/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column/locale/ro/LC_MESSAGES/django.po` & `djangocms_column-2.1.0/djangocms_column/locale/ro/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column/locale/ru/LC_MESSAGES/django.mo` & `djangocms_column-2.1.0/djangocms_column/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column/locale/ru/LC_MESSAGES/django.po` & `djangocms_column-2.1.0/djangocms_column/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column/locale/sk/LC_MESSAGES/django.mo` & `djangocms_column-2.1.0/djangocms_column/locale/sk/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column/locale/sk/LC_MESSAGES/django.po` & `djangocms_column-2.1.0/djangocms_column/locale/sk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column/locale/sl/LC_MESSAGES/django.mo` & `djangocms_column-2.1.0/djangocms_column/locale/sl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column/locale/sl/LC_MESSAGES/django.po` & `djangocms_column-2.1.0/djangocms_column/locale/sl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column/locale/sl_SI/LC_MESSAGES/django.mo` & `djangocms_column-2.1.0/djangocms_column/locale/sl_SI/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column/locale/sl_SI/LC_MESSAGES/django.po` & `djangocms_column-2.1.0/djangocms_column/locale/sl_SI/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column/locale/sq/LC_MESSAGES/django.po` & `djangocms_column-2.1.0/djangocms_column/locale/sq/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column/locale/sq_AL/LC_MESSAGES/django.po` & `djangocms_column-2.1.0/djangocms_column/locale/sq_AL/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column/locale/sr/LC_MESSAGES/django.mo` & `djangocms_column-2.1.0/djangocms_column/locale/sr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column/locale/sr/LC_MESSAGES/django.po` & `djangocms_column-2.1.0/djangocms_column/locale/sr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column/locale/sr@latin/LC_MESSAGES/django.mo` & `djangocms_column-2.1.0/djangocms_column/locale/sr@latin/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column/locale/sr@latin/LC_MESSAGES/django.po` & `djangocms_column-2.1.0/djangocms_column/locale/sr@latin/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column/locale/sv/LC_MESSAGES/django.mo` & `djangocms_column-2.1.0/djangocms_column/locale/sv/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column/locale/sv/LC_MESSAGES/django.po` & `djangocms_column-2.1.0/djangocms_column/locale/sv/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column/locale/ta/LC_MESSAGES/django.mo` & `djangocms_column-2.1.0/djangocms_column/locale/ta/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column/locale/ta/LC_MESSAGES/django.po` & `djangocms_column-2.1.0/djangocms_column/locale/ta/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column/locale/th/LC_MESSAGES/django.po` & `djangocms_column-2.1.0/djangocms_column/locale/th/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column/locale/th_TH/LC_MESSAGES/django.po` & `djangocms_column-2.1.0/djangocms_column/locale/th_TH/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column/locale/tlh/LC_MESSAGES/django.po` & `djangocms_column-2.1.0/djangocms_column/locale/tlh/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column/locale/tr/LC_MESSAGES/django.mo` & `djangocms_column-2.1.0/djangocms_column/locale/tr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column/locale/tr/LC_MESSAGES/django.po` & `djangocms_column-2.1.0/djangocms_column/locale/tr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column/locale/ug/LC_MESSAGES/django.po` & `djangocms_column-2.1.0/djangocms_column/locale/ug/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column/locale/uk/LC_MESSAGES/django.mo` & `djangocms_column-2.1.0/djangocms_column/locale/uk/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column/locale/uk/LC_MESSAGES/django.po` & `djangocms_column-2.1.0/djangocms_column/locale/uk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column/locale/ur/LC_MESSAGES/django.po` & `djangocms_column-2.1.0/djangocms_column/locale/ur/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column/locale/vi/LC_MESSAGES/django.po` & `djangocms_column-2.1.0/djangocms_column/locale/vi/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column/locale/vi_VN/LC_MESSAGES/django.po` & `djangocms_column-2.1.0/djangocms_column/locale/vi_VN/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column/locale/zh/LC_MESSAGES/django.po` & `djangocms_column-2.1.0/djangocms_column/locale/zh/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column/locale/zh_CN/LC_MESSAGES/django.mo` & `djangocms_column-2.1.0/djangocms_column/locale/zh_CN/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column/locale/zh_CN/LC_MESSAGES/django.po` & `djangocms_column-2.1.0/djangocms_column/locale/zh_CN/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column/locale/zh_TW/LC_MESSAGES/django.mo` & `djangocms_column-2.1.0/djangocms_column/locale/zh_TW/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column/locale/zh_TW/LC_MESSAGES/django.po` & `djangocms_column-2.1.0/djangocms_column/locale/zh_TW/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column/migrations/0001_initial.py` & `djangocms_column-2.1.0/djangocms_column/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column/migrations/0002_auto_20160915_0818.py` & `djangocms_column-2.1.0/djangocms_column/migrations/0002_auto_20160915_0818.py`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column/models.py` & `djangocms_column-2.1.0/djangocms_column/models.py`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column/templates/cms/plugins/column_edit.html` & `djangocms_column-2.1.0/djangocms_column/templates/cms/plugins/column_edit.html`

 * *Files identical despite different names*

### Comparing `djangocms-column-2.0.0/djangocms_column.egg-info/PKG-INFO` & `djangocms_column-2.1.0/djangocms_column.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,47 +1,53 @@
 Metadata-Version: 2.1
 Name: djangocms-column
-Version: 2.0.0
+Version: 2.1.0
 Summary: Column Plugin for django CMS
 Home-page: https://github.com/django-cms/djangocms-column
 Author: Django CMS Association and contributors
 Author-email: info@django-cms.org
 License: LICENSE.txt
 Platform: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.2
+Classifier: Framework :: Django :: 5.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Communications
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content :: Message Boards
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
+Requires-Dist: django-cms>=3.8.0
+Requires-Dist: Django>=2.2
 
 djangocms-column
 ================
 
 A Multi Column Plugin for django CMS.
 
 
 Installation
 ------------
 
-This plugin requires `django CMS` 3.8 or higher to be properly installed.
+This plugin requires `django CMS` 3.8 or higher, or 4.0 or higher to be properly installed.
 
 * In your projects virtualenv, run ``pip install djangocms-column``.
 * Add ``'djangocms_column'`` to your ``INSTALLED_APPS`` setting.
 * Run ``manage.py migrate djangocms_column``.
 
 
 Usage
@@ -71,9 +77,7 @@
 
 Translations
 ------------
 
 If you want to help translate the plugin please do it on transifex:
 
 https://www.transifex.com/projects/p/django-cms/resource/djangocms-column/
-
-
```

### Comparing `djangocms-column-2.0.0/djangocms_column.egg-info/SOURCES.txt` & `djangocms_column-2.1.0/djangocms_column.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -159,11 +159,12 @@
 djangocms_column/locale/zh/LC_MESSAGES/django.po
 djangocms_column/locale/zh_CN/LC_MESSAGES/django.mo
 djangocms_column/locale/zh_CN/LC_MESSAGES/django.po
 djangocms_column/locale/zh_TW/LC_MESSAGES/django.mo
 djangocms_column/locale/zh_TW/LC_MESSAGES/django.po
 djangocms_column/migrations/0001_initial.py
 djangocms_column/migrations/0002_auto_20160915_0818.py
+djangocms_column/migrations/0003_alter_column_cmsplugin_ptr_and_more.py
 djangocms_column/migrations/__init__.py
 djangocms_column/templates/cms/plugins/column.html
 djangocms_column/templates/cms/plugins/column_edit.html
 djangocms_column/templates/cms/plugins/multi_column.html
```

### Comparing `djangocms-column-2.0.0/setup.py` & `djangocms_column-2.1.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,23 +12,27 @@
 
 CLASSIFIERS = [
     'Development Status :: 5 - Production/Stable',
     'Environment :: Web Environment',
     'Framework :: Django',
     'Framework :: Django :: 2.2',
     'Framework :: Django :: 3.2',
+    'Framework :: Django :: 4.2',
+    'Framework :: Django :: 5.0',
     'Intended Audience :: Developers',
     'License :: OSI Approved :: BSD License',
     'Operating System :: OS Independent',
     'Programming Language :: Python',
     'Programming Language :: Python :: 3',
     'Programming Language :: Python :: 3.7',
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
+    'Programming Language :: Python :: 3.11',
+    'Programming Language :: Python :: 3.12',
     'Topic :: Communications',
     'Topic :: Internet :: WWW/HTTP :: Dynamic Content',
     'Topic :: Internet :: WWW/HTTP :: Dynamic Content :: Message Boards',
 ]
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.rst").read_text()
```

