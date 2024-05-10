# Comparing `tmp/mercury-2.4.1.tar.gz` & `tmp/mercury-2.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mercury-2.4.1.tar", last modified: Wed May  8 11:36:42 2024, max compression
+gzip compressed data, was "mercury-2.4.2.tar", last modified: Fri May 10 13:11:11 2024, max compression
```

## Comparing `mercury-2.4.1.tar` & `mercury-2.4.2.tar`

### file list

```diff
@@ -1,228 +1,231 @@
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-08 11:36:42.277175 mercury-2.4.1/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    34575 2023-07-14 08:51:02.000000 mercury-2.4.1/LICENSE.txt
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      149 2022-04-19 12:37:24.000000 mercury-2.4.1/MANIFEST.in
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     8683 2024-05-08 11:36:42.277175 mercury-2.4.1/PKG-INFO
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     8039 2024-05-07 13:52:16.000000 mercury-2.4.1/README.md
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-08 11:36:42.261175 mercury-2.4.1/mercury/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)       54 2024-05-08 11:36:06.000000 mercury-2.4.1/mercury/__init__.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-08 11:36:42.261175 mercury-2.4.1/mercury/apps/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2022-03-09 11:04:20.000000 mercury-2.4.1/mercury/apps/__init__.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-08 11:36:42.261175 mercury-2.4.1/mercury/apps/accounts/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-03-01 11:11:00.000000 mercury-2.4.1/mercury/apps/accounts/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      459 2023-03-17 11:37:23.000000 mercury-2.4.1/mercury/apps/accounts/admin.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      153 2023-03-01 11:11:00.000000 mercury-2.4.1/mercury/apps/accounts/apps.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      801 2023-03-01 11:11:00.000000 mercury-2.4.1/mercury/apps/accounts/fields.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-08 11:36:42.261175 mercury-2.4.1/mercury/apps/accounts/migrations/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     9132 2023-03-29 09:06:05.000000 mercury-2.4.1/mercury/apps/accounts/migrations/0001_initial.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-03-01 11:11:00.000000 mercury-2.4.1/mercury/apps/accounts/migrations/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     4715 2023-03-28 08:49:03.000000 mercury-2.4.1/mercury/apps/accounts/models.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2086 2023-04-06 13:33:42.000000 mercury-2.4.1/mercury/apps/accounts/serializers.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2937 2023-03-27 12:26:01.000000 mercury-2.4.1/mercury/apps/accounts/tasks.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-08 11:36:42.261175 mercury-2.4.1/mercury/apps/accounts/templatetags/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2024-01-10 11:48:55.000000 mercury-2.4.1/mercury/apps/accounts/templatetags/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      293 2024-01-10 11:51:23.000000 mercury-2.4.1/mercury/apps/accounts/templatetags/replace.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-08 11:36:42.261175 mercury-2.4.1/mercury/apps/accounts/tests/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-03-16 13:27:44.000000 mercury-2.4.1/mercury/apps/accounts/tests/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     7289 2023-03-29 09:06:05.000000 mercury-2.4.1/mercury/apps/accounts/tests/test_accounts.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     5543 2023-03-31 10:36:11.000000 mercury-2.4.1/mercury/apps/accounts/tests/test_invitations.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     6078 2023-04-06 13:49:54.000000 mercury-2.4.1/mercury/apps/accounts/tests/test_secrets.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    11402 2023-06-22 08:59:21.000000 mercury-2.4.1/mercury/apps/accounts/tests/test_sites.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3426 2023-03-29 09:06:05.000000 mercury-2.4.1/mercury/apps/accounts/tests/test_subscription.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2645 2024-01-10 11:49:35.000000 mercury-2.4.1/mercury/apps/accounts/urls.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-08 11:36:42.261175 mercury-2.4.1/mercury/apps/accounts/views/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-03-17 08:20:29.000000 mercury-2.4.1/mercury/apps/accounts/views/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1979 2024-03-08 14:49:21.000000 mercury-2.4.1/mercury/apps/accounts/views/accounts.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     4308 2023-03-31 10:36:11.000000 mercury-2.4.1/mercury/apps/accounts/views/invitations.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      789 2023-03-24 08:45:58.000000 mercury-2.4.1/mercury/apps/accounts/views/permissions.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2922 2023-04-06 14:49:43.000000 mercury-2.4.1/mercury/apps/accounts/views/secrets.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     7505 2023-08-10 13:34:52.000000 mercury-2.4.1/mercury/apps/accounts/views/sites.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     4176 2024-03-08 14:45:37.000000 mercury-2.4.1/mercury/apps/accounts/views/subscription.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      892 2023-08-10 13:34:52.000000 mercury-2.4.1/mercury/apps/accounts/views/utils.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-08 11:36:42.261175 mercury-2.4.1/mercury/apps/nb/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-02-13 14:05:12.000000 mercury-2.4.1/mercury/apps/nb/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     5845 2023-04-06 13:49:54.000000 mercury-2.4.1/mercury/apps/nb/exporter.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     4523 2023-08-10 13:34:52.000000 mercury-2.4.1/mercury/apps/nb/nbrun.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-08 11:36:42.261175 mercury-2.4.1/mercury/apps/nb/tests/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-04-05 08:19:32.000000 mercury-2.4.1/mercury/apps/nb/tests/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1252 2023-07-18 10:35:22.000000 mercury-2.4.1/mercury/apps/nb/tests/test_nbrun.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1265 2023-03-17 12:41:34.000000 mercury-2.4.1/mercury/apps/nb/tests.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      403 2023-02-13 14:05:12.000000 mercury-2.4.1/mercury/apps/nb/utils.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-08 11:36:42.265175 mercury-2.4.1/mercury/apps/nbworker/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-02-13 14:05:12.000000 mercury-2.4.1/mercury/apps/nbworker/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1786 2024-05-06 12:35:47.000000 mercury-2.4.1/mercury/apps/nbworker/__main__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    19411 2024-05-07 11:02:27.000000 mercury-2.4.1/mercury/apps/nbworker/nb.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     9765 2024-05-07 08:10:41.000000 mercury-2.4.1/mercury/apps/nbworker/rest.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     4898 2023-06-28 11:59:58.000000 mercury-2.4.1/mercury/apps/nbworker/tests.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      701 2023-03-14 07:49:44.000000 mercury-2.4.1/mercury/apps/nbworker/utils.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2858 2024-03-05 09:51:03.000000 mercury-2.4.1/mercury/apps/nbworker/ws.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-08 11:36:42.265175 mercury-2.4.1/mercury/apps/notebooks/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2022-03-09 11:04:20.000000 mercury-2.4.1/mercury/apps/notebooks/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      277 2022-03-09 11:04:20.000000 mercury-2.4.1/mercury/apps/notebooks/admin.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      155 2022-03-09 11:04:20.000000 mercury-2.4.1/mercury/apps/notebooks/apps.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-08 11:36:42.265175 mercury-2.4.1/mercury/apps/notebooks/management/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2022-03-09 11:04:20.000000 mercury-2.4.1/mercury/apps/notebooks/management/__init__.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-08 11:36:42.265175 mercury-2.4.1/mercury/apps/notebooks/management/commands/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2022-03-09 11:04:20.000000 mercury-2.4.1/mercury/apps/notebooks/management/commands/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1279 2022-03-09 11:06:47.000000 mercury-2.4.1/mercury/apps/notebooks/management/commands/add.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      864 2022-03-09 11:06:47.000000 mercury-2.4.1/mercury/apps/notebooks/management/commands/delete.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      545 2022-03-09 11:06:47.000000 mercury-2.4.1/mercury/apps/notebooks/management/commands/list.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3702 2023-02-13 14:05:12.000000 mercury-2.4.1/mercury/apps/notebooks/management/commands/watch.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-08 11:36:42.265175 mercury-2.4.1/mercury/apps/notebooks/migrations/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2300 2023-03-29 09:06:05.000000 mercury-2.4.1/mercury/apps/notebooks/migrations/0001_initial.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2022-03-09 11:04:20.000000 mercury-2.4.1/mercury/apps/notebooks/migrations/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1067 2023-03-27 08:29:11.000000 mercury-2.4.1/mercury/apps/notebooks/models.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      617 2023-03-17 11:38:01.000000 mercury-2.4.1/mercury/apps/notebooks/serializers.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     4093 2022-05-18 10:19:32.000000 mercury-2.4.1/mercury/apps/notebooks/slides_themes.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    11759 2024-03-18 07:18:56.000000 mercury-2.4.1/mercury/apps/notebooks/tasks.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        1 2023-03-01 11:11:00.000000 mercury-2.4.1/mercury/apps/notebooks/tests.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      582 2023-04-25 12:40:05.000000 mercury-2.4.1/mercury/apps/notebooks/urls.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3798 2024-04-12 10:17:00.000000 mercury-2.4.1/mercury/apps/notebooks/views.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-08 11:36:42.265175 mercury-2.4.1/mercury/apps/storage/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-02-13 14:05:12.000000 mercury-2.4.1/mercury/apps/storage/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)       63 2023-02-13 14:05:12.000000 mercury-2.4.1/mercury/apps/storage/admin.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      151 2023-02-13 14:05:12.000000 mercury-2.4.1/mercury/apps/storage/apps.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-08 11:36:42.265175 mercury-2.4.1/mercury/apps/storage/migrations/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2949 2023-03-29 09:06:05.000000 mercury-2.4.1/mercury/apps/storage/migrations/0001_initial.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1404 2023-03-31 09:54:03.000000 mercury-2.4.1/mercury/apps/storage/migrations/0002_useruploadedfile.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-02-13 14:05:12.000000 mercury-2.4.1/mercury/apps/storage/migrations/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1787 2023-03-29 09:06:05.000000 mercury-2.4.1/mercury/apps/storage/models.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3540 2023-03-31 09:54:03.000000 mercury-2.4.1/mercury/apps/storage/s3utils.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      469 2023-03-31 14:19:15.000000 mercury-2.4.1/mercury/apps/storage/serializers.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    11511 2024-05-07 08:14:32.000000 mercury-2.4.1/mercury/apps/storage/storage.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3158 2023-03-17 08:55:41.000000 mercury-2.4.1/mercury/apps/storage/tests.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2602 2024-02-19 11:05:39.000000 mercury-2.4.1/mercury/apps/storage/urls.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      902 2024-01-10 11:15:09.000000 mercury-2.4.1/mercury/apps/storage/utils.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-08 11:36:42.265175 mercury-2.4.1/mercury/apps/storage/views/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-03-31 12:45:08.000000 mercury-2.4.1/mercury/apps/storage/views/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     6773 2024-02-19 11:25:22.000000 mercury-2.4.1/mercury/apps/storage/views/dashboardfiles.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     4935 2023-03-31 11:42:07.000000 mercury-2.4.1/mercury/apps/storage/views/notebookfiles.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3496 2023-08-10 13:34:52.000000 mercury-2.4.1/mercury/apps/storage/views/stylefiles.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3737 2023-03-31 11:42:07.000000 mercury-2.4.1/mercury/apps/storage/views/workerfiles.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-08 11:36:42.265175 mercury-2.4.1/mercury/apps/tasks/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2022-03-09 11:04:20.000000 mercury-2.4.1/mercury/apps/tasks/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      287 2022-03-09 11:04:20.000000 mercury-2.4.1/mercury/apps/tasks/admin.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      153 2022-03-09 11:04:20.000000 mercury-2.4.1/mercury/apps/tasks/apps.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      412 2022-03-09 11:06:47.000000 mercury-2.4.1/mercury/apps/tasks/clean_service.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     4018 2023-06-22 08:55:52.000000 mercury-2.4.1/mercury/apps/tasks/export_pdf.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3805 2023-04-06 13:49:54.000000 mercury-2.4.1/mercury/apps/tasks/export_png.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-08 11:36:42.265175 mercury-2.4.1/mercury/apps/tasks/migrations/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1328 2023-03-29 09:06:05.000000 mercury-2.4.1/mercury/apps/tasks/migrations/0001_initial.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2121 2024-05-07 08:11:51.000000 mercury-2.4.1/mercury/apps/tasks/migrations/0002_restapitask.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2022-03-09 11:04:20.000000 mercury-2.4.1/mercury/apps/tasks/migrations/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1735 2024-05-07 08:07:52.000000 mercury-2.4.1/mercury/apps/tasks/models.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3659 2023-02-13 14:05:12.000000 mercury-2.4.1/mercury/apps/tasks/notify.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      433 2022-03-09 11:06:47.000000 mercury-2.4.1/mercury/apps/tasks/serializers.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    15223 2023-02-23 14:52:12.000000 mercury-2.4.1/mercury/apps/tasks/tasks.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1335 2023-05-23 13:34:07.000000 mercury-2.4.1/mercury/apps/tasks/tasks_export.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      571 2023-03-14 07:49:44.000000 mercury-2.4.1/mercury/apps/tasks/tests.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1594 2024-05-07 11:42:50.000000 mercury-2.4.1/mercury/apps/tasks/urls.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    10866 2024-05-08 11:34:56.000000 mercury-2.4.1/mercury/apps/tasks/views.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-08 11:36:42.265175 mercury-2.4.1/mercury/apps/workers/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-03-14 07:49:44.000000 mercury-2.4.1/mercury/apps/workers/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)       63 2023-03-14 07:49:44.000000 mercury-2.4.1/mercury/apps/workers/admin.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      151 2023-03-14 07:49:44.000000 mercury-2.4.1/mercury/apps/workers/apps.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      532 2023-07-18 10:35:22.000000 mercury-2.4.1/mercury/apps/workers/constants.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-08 11:36:42.265175 mercury-2.4.1/mercury/apps/workers/migrations/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1286 2023-03-29 09:06:05.000000 mercury-2.4.1/mercury/apps/workers/migrations/0001_initial.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      911 2023-06-20 12:58:36.000000 mercury-2.4.1/mercury/apps/workers/migrations/0002_machine.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2842 2023-06-22 09:33:58.000000 mercury-2.4.1/mercury/apps/workers/migrations/0003_worker_run_by_workersession.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-03-14 07:49:44.000000 mercury-2.4.1/mercury/apps/workers/migrations/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1832 2024-04-12 09:41:31.000000 mercury-2.4.1/mercury/apps/workers/models.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      296 2023-03-14 07:49:44.000000 mercury-2.4.1/mercury/apps/workers/serializers.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     8697 2024-04-12 10:16:03.000000 mercury-2.4.1/mercury/apps/workers/tests.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1612 2024-05-07 08:04:54.000000 mercury-2.4.1/mercury/apps/workers/urls.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      468 2024-03-05 09:51:03.000000 mercury-2.4.1/mercury/apps/workers/utils.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    11279 2024-05-07 11:04:20.000000 mercury-2.4.1/mercury/apps/workers/views.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-08 11:36:42.269175 mercury-2.4.1/mercury/apps/ws/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-02-13 14:05:12.000000 mercury-2.4.1/mercury/apps/ws/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      141 2023-02-13 14:05:12.000000 mercury-2.4.1/mercury/apps/ws/apps.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     6689 2024-05-06 11:03:38.000000 mercury-2.4.1/mercury/apps/ws/client.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      947 2023-03-14 07:49:44.000000 mercury-2.4.1/mercury/apps/ws/middleware.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-08 11:36:42.269175 mercury-2.4.1/mercury/apps/ws/migrations/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-02-13 14:05:12.000000 mercury-2.4.1/mercury/apps/ws/migrations/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      386 2023-02-28 13:59:46.000000 mercury-2.4.1/mercury/apps/ws/routing.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3114 2024-03-08 15:03:14.000000 mercury-2.4.1/mercury/apps/ws/tasks.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      137 2023-06-21 07:54:00.000000 mercury-2.4.1/mercury/apps/ws/tests.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     5839 2024-03-08 14:48:55.000000 mercury-2.4.1/mercury/apps/ws/utils.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2470 2024-03-05 10:39:26.000000 mercury-2.4.1/mercury/apps/ws/worker.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     7191 2023-03-31 14:11:10.000000 mercury-2.4.1/mercury/demo.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-08 11:36:42.269175 mercury-2.4.1/mercury/frontend-dist/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1158 2024-05-08 11:36:41.000000 mercury-2.4.1/mercury/frontend-dist/asset-manifest.json
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    15406 2024-05-08 11:36:25.000000 mercury-2.4.1/mercury/frontend-dist/favicon-old.ico
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    15086 2024-05-08 11:36:25.000000 mercury-2.4.1/mercury/frontend-dist/favicon.ico
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3086 2024-05-08 11:36:41.000000 mercury-2.4.1/mercury/frontend-dist/index.html
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    17406 2024-05-08 11:36:25.000000 mercury-2.4.1/mercury/frontend-dist/jupyter-additional.css
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     4539 2024-05-08 11:36:25.000000 mercury-2.4.1/mercury/frontend-dist/jupyter-syntax.css
--rw-rw-r--   0 piotr     (1000) piotr     (1000)   580392 2024-05-08 11:36:25.000000 mercury-2.4.1/mercury/frontend-dist/jupyter-theme-light.css
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      324 2024-05-08 11:36:25.000000 mercury-2.4.1/mercury/frontend-dist/manifest.json
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     6237 2024-05-08 11:36:25.000000 mercury-2.4.1/mercury/frontend-dist/mercury_black_logo.svg
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     6997 2024-05-08 11:36:25.000000 mercury-2.4.1/mercury/frontend-dist/mercury_logo.svg
--rw-rw-r--   0 piotr     (1000) piotr     (1000)       67 2024-05-08 11:36:25.000000 mercury-2.4.1/mercury/frontend-dist/robots.txt
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-08 11:36:42.261175 mercury-2.4.1/mercury/frontend-dist/static/
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-08 11:36:42.269175 mercury-2.4.1/mercury/frontend-dist/static/css/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)   229115 2024-05-08 11:36:41.000000 mercury-2.4.1/mercury/frontend-dist/static/css/2.c6cf5ff9.chunk.css
--rw-rw-r--   0 piotr     (1000) piotr     (1000)   612316 2024-05-08 11:36:41.000000 mercury-2.4.1/mercury/frontend-dist/static/css/2.c6cf5ff9.chunk.css.map
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3071 2024-05-08 11:36:41.000000 mercury-2.4.1/mercury/frontend-dist/static/css/main.9848f1b3.chunk.css
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     5632 2024-05-08 11:36:41.000000 mercury-2.4.1/mercury/frontend-dist/static/css/main.9848f1b3.chunk.css.map
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-08 11:36:42.273175 mercury-2.4.1/mercury/frontend-dist/static/js/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)  1311795 2024-05-08 11:36:41.000000 mercury-2.4.1/mercury/frontend-dist/static/js/2.81b1917f.chunk.js
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3383 2024-05-08 11:36:41.000000 mercury-2.4.1/mercury/frontend-dist/static/js/2.81b1917f.chunk.js.LICENSE.txt
--rw-rw-r--   0 piotr     (1000) piotr     (1000)  4972959 2024-05-08 11:36:41.000000 mercury-2.4.1/mercury/frontend-dist/static/js/2.81b1917f.chunk.js.map
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    96124 2024-05-08 11:36:41.000000 mercury-2.4.1/mercury/frontend-dist/static/js/main.51571475.chunk.js
--rw-rw-r--   0 piotr     (1000) piotr     (1000)   286726 2024-05-08 11:36:41.000000 mercury-2.4.1/mercury/frontend-dist/static/js/main.51571475.chunk.js.map
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1557 2024-05-08 11:36:41.000000 mercury-2.4.1/mercury/frontend-dist/static/js/runtime-main.248907bc.js
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     8276 2024-05-08 11:36:41.000000 mercury-2.4.1/mercury/frontend-dist/static/js/runtime-main.248907bc.js.map
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-08 11:36:42.273175 mercury-2.4.1/mercury/frontend-dist/static/media/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)   165548 2024-05-08 11:36:41.000000 mercury-2.4.1/mercury/frontend-dist/static/media/fontawesome-webfont.1e59d233.ttf
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    77160 2024-05-08 11:36:41.000000 mercury-2.4.1/mercury/frontend-dist/static/media/fontawesome-webfont.20fd1704.woff2
--rw-rw-r--   0 piotr     (1000) piotr     (1000)   165742 2024-05-08 11:36:41.000000 mercury-2.4.1/mercury/frontend-dist/static/media/fontawesome-webfont.8b43027f.eot
--rw-rw-r--   0 piotr     (1000) piotr     (1000)   444379 2024-05-08 11:36:41.000000 mercury-2.4.1/mercury/frontend-dist/static/media/fontawesome-webfont.c1e38fd9.svg
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    98024 2024-05-08 11:36:41.000000 mercury-2.4.1/mercury/frontend-dist/static/media/fontawesome-webfont.f691f37e.woff
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      684 2022-03-09 11:04:20.000000 mercury-2.4.1/mercury/manage.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    10038 2024-05-07 09:50:27.000000 mercury-2.4.1/mercury/mercury.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      563 2024-04-12 08:02:38.000000 mercury-2.4.1/mercury/requirements.txt
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-08 11:36:42.277175 mercury-2.4.1/mercury/server/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)       68 2022-03-09 11:04:20.000000 mercury-2.4.1/mercury/server/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      837 2023-08-31 09:59:17.000000 mercury-2.4.1/mercury/server/asgi.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3376 2023-09-19 13:56:49.000000 mercury-2.4.1/mercury/server/celery.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    10336 2024-03-05 10:38:07.000000 mercury-2.4.1/mercury/server/settings.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1575 2023-04-25 12:38:18.000000 mercury-2.4.1/mercury/server/urls.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1645 2023-03-01 12:07:40.000000 mercury-2.4.1/mercury/server/views.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      405 2022-05-18 11:03:41.000000 mercury-2.4.1/mercury/server/wsgi.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2461 2023-06-21 11:57:21.000000 mercury-2.4.1/mercury/start_instance.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-08 11:36:42.277175 mercury-2.4.1/mercury/widgets/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-02-13 14:05:12.000000 mercury-2.4.1/mercury/widgets/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1475 2024-05-07 10:14:58.000000 mercury-2.4.1/mercury/widgets/apiresponse.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     5787 2024-01-10 11:15:09.000000 mercury-2.4.1/mercury/widgets/app.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     4062 2024-01-10 11:15:09.000000 mercury-2.4.1/mercury/widgets/button.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      826 2023-04-07 10:43:02.000000 mercury-2.4.1/mercury/widgets/chat.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     4599 2024-05-07 10:40:08.000000 mercury-2.4.1/mercury/widgets/checkbox.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      408 2023-04-07 10:32:14.000000 mercury-2.4.1/mercury/widgets/confetti.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     5514 2024-01-10 11:15:09.000000 mercury-2.4.1/mercury/widgets/file.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      851 2023-08-29 14:20:20.000000 mercury-2.4.1/mercury/widgets/in_mercury.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     4828 2023-02-21 07:28:26.000000 mercury-2.4.1/mercury/widgets/json.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     7486 2024-05-07 10:39:24.000000 mercury-2.4.1/mercury/widgets/manager.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      104 2023-02-21 07:28:26.000000 mercury-2.4.1/mercury/widgets/md.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     6251 2024-05-07 10:40:18.000000 mercury-2.4.1/mercury/widgets/multiselect.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2228 2024-01-10 11:15:09.000000 mercury-2.4.1/mercury/widgets/note.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3145 2023-08-29 14:20:20.000000 mercury-2.4.1/mercury/widgets/numberbox.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     6115 2024-01-10 11:15:09.000000 mercury-2.4.1/mercury/widgets/numeric.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1255 2023-02-21 07:48:36.000000 mercury-2.4.1/mercury/widgets/outputdir.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      463 2023-08-29 14:20:20.000000 mercury-2.4.1/mercury/widgets/pdf.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     6524 2024-05-08 09:08:28.000000 mercury-2.4.1/mercury/widgets/range.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     6524 2024-05-07 10:40:44.000000 mercury-2.4.1/mercury/widgets/select.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     6517 2024-05-07 10:40:49.000000 mercury-2.4.1/mercury/widgets/slider.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      222 2023-02-21 07:28:26.000000 mercury-2.4.1/mercury/widgets/stop.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      826 2024-03-20 14:17:46.000000 mercury-2.4.1/mercury/widgets/table.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     4784 2024-05-07 10:41:39.000000 mercury-2.4.1/mercury/widgets/text.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      814 2023-08-29 14:20:20.000000 mercury-2.4.1/mercury/widgets/user.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-08 11:36:42.261175 mercury-2.4.1/mercury.egg-info/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     8683 2024-05-08 11:36:42.000000 mercury-2.4.1/mercury.egg-info/PKG-INFO
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     6849 2024-05-08 11:36:42.000000 mercury-2.4.1/mercury.egg-info/SOURCES.txt
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        1 2024-05-08 11:36:42.000000 mercury-2.4.1/mercury.egg-info/dependency_links.txt
--rw-rw-r--   0 piotr     (1000) piotr     (1000)       49 2024-05-08 11:36:42.000000 mercury-2.4.1/mercury.egg-info/entry_points.txt
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      508 2024-05-08 11:36:42.000000 mercury-2.4.1/mercury.egg-info/requires.txt
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        8 2024-05-08 11:36:42.000000 mercury-2.4.1/mercury.egg-info/top_level.txt
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      106 2022-03-09 11:04:20.000000 mercury-2.4.1/pyproject.toml
--rw-rw-r--   0 piotr     (1000) piotr     (1000)       38 2024-05-08 11:36:42.277175 mercury-2.4.1/setup.cfg
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1386 2024-05-08 11:35:57.000000 mercury-2.4.1/setup.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-10 13:11:11.317097 mercury-2.4.2/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    34575 2023-07-14 08:51:02.000000 mercury-2.4.2/LICENSE.txt
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      149 2022-04-19 12:37:24.000000 mercury-2.4.2/MANIFEST.in
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     8683 2024-05-10 13:11:11.317097 mercury-2.4.2/PKG-INFO
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     8039 2024-05-07 13:52:16.000000 mercury-2.4.2/README.md
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-10 13:11:11.297097 mercury-2.4.2/mercury/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)       54 2024-05-10 13:10:24.000000 mercury-2.4.2/mercury/__init__.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-10 13:11:11.297097 mercury-2.4.2/mercury/apps/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2022-03-09 11:04:20.000000 mercury-2.4.2/mercury/apps/__init__.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-10 13:11:11.301097 mercury-2.4.2/mercury/apps/accounts/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-03-01 11:11:00.000000 mercury-2.4.2/mercury/apps/accounts/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      459 2023-03-17 11:37:23.000000 mercury-2.4.2/mercury/apps/accounts/admin.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      153 2023-03-01 11:11:00.000000 mercury-2.4.2/mercury/apps/accounts/apps.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      801 2023-03-01 11:11:00.000000 mercury-2.4.2/mercury/apps/accounts/fields.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-10 13:11:11.301097 mercury-2.4.2/mercury/apps/accounts/migrations/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     9132 2023-03-29 09:06:05.000000 mercury-2.4.2/mercury/apps/accounts/migrations/0001_initial.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      936 2024-05-09 09:02:47.000000 mercury-2.4.2/mercury/apps/accounts/migrations/0002_apikey.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-03-01 11:11:00.000000 mercury-2.4.2/mercury/apps/accounts/migrations/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     5299 2024-05-09 10:18:53.000000 mercury-2.4.2/mercury/apps/accounts/models.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2086 2023-04-06 13:33:42.000000 mercury-2.4.2/mercury/apps/accounts/serializers.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2937 2023-03-27 12:26:01.000000 mercury-2.4.2/mercury/apps/accounts/tasks.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-10 13:11:11.301097 mercury-2.4.2/mercury/apps/accounts/templatetags/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2024-01-10 11:48:55.000000 mercury-2.4.2/mercury/apps/accounts/templatetags/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      293 2024-01-10 11:51:23.000000 mercury-2.4.2/mercury/apps/accounts/templatetags/replace.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-10 13:11:11.301097 mercury-2.4.2/mercury/apps/accounts/tests/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-03-16 13:27:44.000000 mercury-2.4.2/mercury/apps/accounts/tests/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     7289 2023-03-29 09:06:05.000000 mercury-2.4.2/mercury/apps/accounts/tests/test_accounts.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3250 2024-05-09 09:27:16.000000 mercury-2.4.2/mercury/apps/accounts/tests/test_apikey.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     5543 2023-03-31 10:36:11.000000 mercury-2.4.2/mercury/apps/accounts/tests/test_invitations.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     6078 2023-04-06 13:49:54.000000 mercury-2.4.2/mercury/apps/accounts/tests/test_secrets.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    11402 2023-06-22 08:59:21.000000 mercury-2.4.2/mercury/apps/accounts/tests/test_sites.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3426 2023-03-29 09:06:05.000000 mercury-2.4.2/mercury/apps/accounts/tests/test_subscription.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2863 2024-05-09 08:30:27.000000 mercury-2.4.2/mercury/apps/accounts/urls.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-10 13:11:11.301097 mercury-2.4.2/mercury/apps/accounts/views/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-03-17 08:20:29.000000 mercury-2.4.2/mercury/apps/accounts/views/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1979 2024-03-08 14:49:21.000000 mercury-2.4.2/mercury/apps/accounts/views/accounts.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      792 2024-05-09 09:27:33.000000 mercury-2.4.2/mercury/apps/accounts/views/apikey.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4308 2023-03-31 10:36:11.000000 mercury-2.4.2/mercury/apps/accounts/views/invitations.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1117 2024-05-09 10:08:20.000000 mercury-2.4.2/mercury/apps/accounts/views/permissions.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2922 2023-04-06 14:49:43.000000 mercury-2.4.2/mercury/apps/accounts/views/secrets.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     7505 2023-08-10 13:34:52.000000 mercury-2.4.2/mercury/apps/accounts/views/sites.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4176 2024-03-08 14:45:37.000000 mercury-2.4.2/mercury/apps/accounts/views/subscription.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      892 2023-08-10 13:34:52.000000 mercury-2.4.2/mercury/apps/accounts/views/utils.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-10 13:11:11.301097 mercury-2.4.2/mercury/apps/nb/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-02-13 14:05:12.000000 mercury-2.4.2/mercury/apps/nb/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     5845 2023-04-06 13:49:54.000000 mercury-2.4.2/mercury/apps/nb/exporter.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4523 2023-08-10 13:34:52.000000 mercury-2.4.2/mercury/apps/nb/nbrun.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-10 13:11:11.301097 mercury-2.4.2/mercury/apps/nb/tests/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-04-05 08:19:32.000000 mercury-2.4.2/mercury/apps/nb/tests/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1252 2023-07-18 10:35:22.000000 mercury-2.4.2/mercury/apps/nb/tests/test_nbrun.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1265 2023-03-17 12:41:34.000000 mercury-2.4.2/mercury/apps/nb/tests.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      403 2023-02-13 14:05:12.000000 mercury-2.4.2/mercury/apps/nb/utils.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-10 13:11:11.301097 mercury-2.4.2/mercury/apps/nbworker/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-02-13 14:05:12.000000 mercury-2.4.2/mercury/apps/nbworker/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1786 2024-05-06 12:35:47.000000 mercury-2.4.2/mercury/apps/nbworker/__main__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    19411 2024-05-07 11:02:27.000000 mercury-2.4.2/mercury/apps/nbworker/nb.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     9792 2024-05-10 13:06:51.000000 mercury-2.4.2/mercury/apps/nbworker/rest.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4898 2023-06-28 11:59:58.000000 mercury-2.4.2/mercury/apps/nbworker/tests.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      701 2023-03-14 07:49:44.000000 mercury-2.4.2/mercury/apps/nbworker/utils.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2858 2024-03-05 09:51:03.000000 mercury-2.4.2/mercury/apps/nbworker/ws.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-10 13:11:11.301097 mercury-2.4.2/mercury/apps/notebooks/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2022-03-09 11:04:20.000000 mercury-2.4.2/mercury/apps/notebooks/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      277 2022-03-09 11:04:20.000000 mercury-2.4.2/mercury/apps/notebooks/admin.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      155 2022-03-09 11:04:20.000000 mercury-2.4.2/mercury/apps/notebooks/apps.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-10 13:11:11.301097 mercury-2.4.2/mercury/apps/notebooks/management/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2022-03-09 11:04:20.000000 mercury-2.4.2/mercury/apps/notebooks/management/__init__.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-10 13:11:11.301097 mercury-2.4.2/mercury/apps/notebooks/management/commands/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2022-03-09 11:04:20.000000 mercury-2.4.2/mercury/apps/notebooks/management/commands/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1279 2022-03-09 11:06:47.000000 mercury-2.4.2/mercury/apps/notebooks/management/commands/add.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      864 2022-03-09 11:06:47.000000 mercury-2.4.2/mercury/apps/notebooks/management/commands/delete.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      545 2022-03-09 11:06:47.000000 mercury-2.4.2/mercury/apps/notebooks/management/commands/list.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3702 2023-02-13 14:05:12.000000 mercury-2.4.2/mercury/apps/notebooks/management/commands/watch.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-10 13:11:11.301097 mercury-2.4.2/mercury/apps/notebooks/migrations/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2300 2023-03-29 09:06:05.000000 mercury-2.4.2/mercury/apps/notebooks/migrations/0001_initial.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2022-03-09 11:04:20.000000 mercury-2.4.2/mercury/apps/notebooks/migrations/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1067 2023-03-27 08:29:11.000000 mercury-2.4.2/mercury/apps/notebooks/models.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      617 2023-03-17 11:38:01.000000 mercury-2.4.2/mercury/apps/notebooks/serializers.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4093 2022-05-18 10:19:32.000000 mercury-2.4.2/mercury/apps/notebooks/slides_themes.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    11759 2024-03-18 07:18:56.000000 mercury-2.4.2/mercury/apps/notebooks/tasks.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        1 2023-03-01 11:11:00.000000 mercury-2.4.2/mercury/apps/notebooks/tests.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      582 2023-04-25 12:40:05.000000 mercury-2.4.2/mercury/apps/notebooks/urls.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3798 2024-04-12 10:17:00.000000 mercury-2.4.2/mercury/apps/notebooks/views.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-10 13:11:11.301097 mercury-2.4.2/mercury/apps/storage/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-02-13 14:05:12.000000 mercury-2.4.2/mercury/apps/storage/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)       63 2023-02-13 14:05:12.000000 mercury-2.4.2/mercury/apps/storage/admin.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      151 2023-02-13 14:05:12.000000 mercury-2.4.2/mercury/apps/storage/apps.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-10 13:11:11.305097 mercury-2.4.2/mercury/apps/storage/migrations/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2949 2023-03-29 09:06:05.000000 mercury-2.4.2/mercury/apps/storage/migrations/0001_initial.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1404 2023-03-31 09:54:03.000000 mercury-2.4.2/mercury/apps/storage/migrations/0002_useruploadedfile.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-02-13 14:05:12.000000 mercury-2.4.2/mercury/apps/storage/migrations/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1787 2023-03-29 09:06:05.000000 mercury-2.4.2/mercury/apps/storage/models.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3540 2023-03-31 09:54:03.000000 mercury-2.4.2/mercury/apps/storage/s3utils.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      469 2023-03-31 14:19:15.000000 mercury-2.4.2/mercury/apps/storage/serializers.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    11511 2024-05-07 08:14:32.000000 mercury-2.4.2/mercury/apps/storage/storage.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3158 2023-03-17 08:55:41.000000 mercury-2.4.2/mercury/apps/storage/tests.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2602 2024-02-19 11:05:39.000000 mercury-2.4.2/mercury/apps/storage/urls.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      902 2024-01-10 11:15:09.000000 mercury-2.4.2/mercury/apps/storage/utils.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-10 13:11:11.305097 mercury-2.4.2/mercury/apps/storage/views/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-03-31 12:45:08.000000 mercury-2.4.2/mercury/apps/storage/views/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     6773 2024-02-19 11:25:22.000000 mercury-2.4.2/mercury/apps/storage/views/dashboardfiles.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4935 2023-03-31 11:42:07.000000 mercury-2.4.2/mercury/apps/storage/views/notebookfiles.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3496 2023-08-10 13:34:52.000000 mercury-2.4.2/mercury/apps/storage/views/stylefiles.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3737 2023-03-31 11:42:07.000000 mercury-2.4.2/mercury/apps/storage/views/workerfiles.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-10 13:11:11.305097 mercury-2.4.2/mercury/apps/tasks/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2022-03-09 11:04:20.000000 mercury-2.4.2/mercury/apps/tasks/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      287 2022-03-09 11:04:20.000000 mercury-2.4.2/mercury/apps/tasks/admin.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      153 2022-03-09 11:04:20.000000 mercury-2.4.2/mercury/apps/tasks/apps.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      412 2022-03-09 11:06:47.000000 mercury-2.4.2/mercury/apps/tasks/clean_service.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4018 2023-06-22 08:55:52.000000 mercury-2.4.2/mercury/apps/tasks/export_pdf.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3805 2023-04-06 13:49:54.000000 mercury-2.4.2/mercury/apps/tasks/export_png.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-10 13:11:11.305097 mercury-2.4.2/mercury/apps/tasks/migrations/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1328 2023-03-29 09:06:05.000000 mercury-2.4.2/mercury/apps/tasks/migrations/0001_initial.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2121 2024-05-07 08:11:51.000000 mercury-2.4.2/mercury/apps/tasks/migrations/0002_restapitask.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2022-03-09 11:04:20.000000 mercury-2.4.2/mercury/apps/tasks/migrations/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1735 2024-05-07 08:07:52.000000 mercury-2.4.2/mercury/apps/tasks/models.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3659 2023-02-13 14:05:12.000000 mercury-2.4.2/mercury/apps/tasks/notify.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      433 2022-03-09 11:06:47.000000 mercury-2.4.2/mercury/apps/tasks/serializers.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    15223 2023-02-23 14:52:12.000000 mercury-2.4.2/mercury/apps/tasks/tasks.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1335 2023-05-23 13:34:07.000000 mercury-2.4.2/mercury/apps/tasks/tasks_export.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     6757 2024-05-09 10:21:23.000000 mercury-2.4.2/mercury/apps/tasks/tests.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1594 2024-05-07 11:42:50.000000 mercury-2.4.2/mercury/apps/tasks/urls.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    10911 2024-05-09 10:07:46.000000 mercury-2.4.2/mercury/apps/tasks/views.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-10 13:11:11.305097 mercury-2.4.2/mercury/apps/workers/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-03-14 07:49:44.000000 mercury-2.4.2/mercury/apps/workers/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)       63 2023-03-14 07:49:44.000000 mercury-2.4.2/mercury/apps/workers/admin.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      151 2023-03-14 07:49:44.000000 mercury-2.4.2/mercury/apps/workers/apps.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      532 2023-07-18 10:35:22.000000 mercury-2.4.2/mercury/apps/workers/constants.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-10 13:11:11.305097 mercury-2.4.2/mercury/apps/workers/migrations/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1286 2023-03-29 09:06:05.000000 mercury-2.4.2/mercury/apps/workers/migrations/0001_initial.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      911 2023-06-20 12:58:36.000000 mercury-2.4.2/mercury/apps/workers/migrations/0002_machine.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2842 2023-06-22 09:33:58.000000 mercury-2.4.2/mercury/apps/workers/migrations/0003_worker_run_by_workersession.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-03-14 07:49:44.000000 mercury-2.4.2/mercury/apps/workers/migrations/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1832 2024-04-12 09:41:31.000000 mercury-2.4.2/mercury/apps/workers/models.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      296 2023-03-14 07:49:44.000000 mercury-2.4.2/mercury/apps/workers/serializers.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     8697 2024-04-12 10:16:03.000000 mercury-2.4.2/mercury/apps/workers/tests.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1612 2024-05-07 08:04:54.000000 mercury-2.4.2/mercury/apps/workers/urls.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      468 2024-03-05 09:51:03.000000 mercury-2.4.2/mercury/apps/workers/utils.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    11279 2024-05-07 11:04:20.000000 mercury-2.4.2/mercury/apps/workers/views.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-10 13:11:11.305097 mercury-2.4.2/mercury/apps/ws/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-02-13 14:05:12.000000 mercury-2.4.2/mercury/apps/ws/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      141 2023-02-13 14:05:12.000000 mercury-2.4.2/mercury/apps/ws/apps.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     6689 2024-05-06 11:03:38.000000 mercury-2.4.2/mercury/apps/ws/client.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      947 2023-03-14 07:49:44.000000 mercury-2.4.2/mercury/apps/ws/middleware.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-10 13:11:11.305097 mercury-2.4.2/mercury/apps/ws/migrations/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-02-13 14:05:12.000000 mercury-2.4.2/mercury/apps/ws/migrations/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      386 2023-02-28 13:59:46.000000 mercury-2.4.2/mercury/apps/ws/routing.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3114 2024-03-08 15:03:14.000000 mercury-2.4.2/mercury/apps/ws/tasks.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      137 2023-06-21 07:54:00.000000 mercury-2.4.2/mercury/apps/ws/tests.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     5957 2024-05-10 13:06:51.000000 mercury-2.4.2/mercury/apps/ws/utils.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2470 2024-03-05 10:39:26.000000 mercury-2.4.2/mercury/apps/ws/worker.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     7191 2023-03-31 14:11:10.000000 mercury-2.4.2/mercury/demo.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-10 13:11:11.305097 mercury-2.4.2/mercury/frontend-dist/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1158 2024-05-10 13:11:10.000000 mercury-2.4.2/mercury/frontend-dist/asset-manifest.json
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    15406 2024-05-10 13:10:54.000000 mercury-2.4.2/mercury/frontend-dist/favicon-old.ico
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    15086 2024-05-10 13:10:54.000000 mercury-2.4.2/mercury/frontend-dist/favicon.ico
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3086 2024-05-10 13:11:10.000000 mercury-2.4.2/mercury/frontend-dist/index.html
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    17406 2024-05-10 13:10:54.000000 mercury-2.4.2/mercury/frontend-dist/jupyter-additional.css
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4539 2024-05-10 13:10:54.000000 mercury-2.4.2/mercury/frontend-dist/jupyter-syntax.css
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)   580392 2024-05-10 13:10:54.000000 mercury-2.4.2/mercury/frontend-dist/jupyter-theme-light.css
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      324 2024-05-10 13:10:54.000000 mercury-2.4.2/mercury/frontend-dist/manifest.json
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     6237 2024-05-10 13:10:54.000000 mercury-2.4.2/mercury/frontend-dist/mercury_black_logo.svg
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     6997 2024-05-10 13:10:54.000000 mercury-2.4.2/mercury/frontend-dist/mercury_logo.svg
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)       67 2024-05-10 13:10:54.000000 mercury-2.4.2/mercury/frontend-dist/robots.txt
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-10 13:11:11.297097 mercury-2.4.2/mercury/frontend-dist/static/
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-10 13:11:11.309097 mercury-2.4.2/mercury/frontend-dist/static/css/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)   229115 2024-05-10 13:11:10.000000 mercury-2.4.2/mercury/frontend-dist/static/css/2.c6cf5ff9.chunk.css
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)   612316 2024-05-10 13:11:10.000000 mercury-2.4.2/mercury/frontend-dist/static/css/2.c6cf5ff9.chunk.css.map
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3071 2024-05-10 13:11:10.000000 mercury-2.4.2/mercury/frontend-dist/static/css/main.9848f1b3.chunk.css
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     5632 2024-05-10 13:11:10.000000 mercury-2.4.2/mercury/frontend-dist/static/css/main.9848f1b3.chunk.css.map
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-10 13:11:11.313097 mercury-2.4.2/mercury/frontend-dist/static/js/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)  1311795 2024-05-10 13:11:10.000000 mercury-2.4.2/mercury/frontend-dist/static/js/2.81b1917f.chunk.js
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3383 2024-05-10 13:11:10.000000 mercury-2.4.2/mercury/frontend-dist/static/js/2.81b1917f.chunk.js.LICENSE.txt
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)  4972959 2024-05-10 13:11:10.000000 mercury-2.4.2/mercury/frontend-dist/static/js/2.81b1917f.chunk.js.map
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    95870 2024-05-10 13:11:10.000000 mercury-2.4.2/mercury/frontend-dist/static/js/main.71279c97.chunk.js
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)   285960 2024-05-10 13:11:10.000000 mercury-2.4.2/mercury/frontend-dist/static/js/main.71279c97.chunk.js.map
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1557 2024-05-10 13:11:10.000000 mercury-2.4.2/mercury/frontend-dist/static/js/runtime-main.248907bc.js
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     8276 2024-05-10 13:11:10.000000 mercury-2.4.2/mercury/frontend-dist/static/js/runtime-main.248907bc.js.map
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-10 13:11:11.313097 mercury-2.4.2/mercury/frontend-dist/static/media/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)   165548 2024-05-10 13:11:10.000000 mercury-2.4.2/mercury/frontend-dist/static/media/fontawesome-webfont.1e59d233.ttf
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    77160 2024-05-10 13:11:10.000000 mercury-2.4.2/mercury/frontend-dist/static/media/fontawesome-webfont.20fd1704.woff2
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)   165742 2024-05-10 13:11:10.000000 mercury-2.4.2/mercury/frontend-dist/static/media/fontawesome-webfont.8b43027f.eot
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)   444379 2024-05-10 13:11:10.000000 mercury-2.4.2/mercury/frontend-dist/static/media/fontawesome-webfont.c1e38fd9.svg
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    98024 2024-05-10 13:11:10.000000 mercury-2.4.2/mercury/frontend-dist/static/media/fontawesome-webfont.f691f37e.woff
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      684 2022-03-09 11:04:20.000000 mercury-2.4.2/mercury/manage.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    10038 2024-05-07 09:50:27.000000 mercury-2.4.2/mercury/mercury.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      565 2024-05-10 13:06:51.000000 mercury-2.4.2/mercury/requirements.txt
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-10 13:11:11.313097 mercury-2.4.2/mercury/server/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)       68 2022-03-09 11:04:20.000000 mercury-2.4.2/mercury/server/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      837 2023-08-31 09:59:17.000000 mercury-2.4.2/mercury/server/asgi.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3376 2023-09-19 13:56:49.000000 mercury-2.4.2/mercury/server/celery.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    10336 2024-03-05 10:38:07.000000 mercury-2.4.2/mercury/server/settings.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1575 2023-04-25 12:38:18.000000 mercury-2.4.2/mercury/server/urls.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1645 2023-03-01 12:07:40.000000 mercury-2.4.2/mercury/server/views.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      405 2022-05-18 11:03:41.000000 mercury-2.4.2/mercury/server/wsgi.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2461 2023-06-21 11:57:21.000000 mercury-2.4.2/mercury/start_instance.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-10 13:11:11.317097 mercury-2.4.2/mercury/widgets/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-02-13 14:05:12.000000 mercury-2.4.2/mercury/widgets/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1475 2024-05-07 10:14:58.000000 mercury-2.4.2/mercury/widgets/apiresponse.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     6070 2024-05-10 13:06:51.000000 mercury-2.4.2/mercury/widgets/app.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4062 2024-01-10 11:15:09.000000 mercury-2.4.2/mercury/widgets/button.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      826 2023-04-07 10:43:02.000000 mercury-2.4.2/mercury/widgets/chat.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4599 2024-05-07 10:40:08.000000 mercury-2.4.2/mercury/widgets/checkbox.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      408 2023-04-07 10:32:14.000000 mercury-2.4.2/mercury/widgets/confetti.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     5514 2024-01-10 11:15:09.000000 mercury-2.4.2/mercury/widgets/file.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      851 2023-08-29 14:20:20.000000 mercury-2.4.2/mercury/widgets/in_mercury.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4828 2023-02-21 07:28:26.000000 mercury-2.4.2/mercury/widgets/json.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     7486 2024-05-07 10:39:24.000000 mercury-2.4.2/mercury/widgets/manager.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      104 2023-02-21 07:28:26.000000 mercury-2.4.2/mercury/widgets/md.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     6316 2024-05-10 10:26:34.000000 mercury-2.4.2/mercury/widgets/multiselect.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2228 2024-01-10 11:15:09.000000 mercury-2.4.2/mercury/widgets/note.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3145 2023-08-29 14:20:20.000000 mercury-2.4.2/mercury/widgets/numberbox.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     6115 2024-01-10 11:15:09.000000 mercury-2.4.2/mercury/widgets/numeric.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1255 2023-02-21 07:48:36.000000 mercury-2.4.2/mercury/widgets/outputdir.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      463 2023-08-29 14:20:20.000000 mercury-2.4.2/mercury/widgets/pdf.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     6524 2024-05-08 09:08:28.000000 mercury-2.4.2/mercury/widgets/range.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     6524 2024-05-07 10:40:44.000000 mercury-2.4.2/mercury/widgets/select.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     6517 2024-05-07 10:40:49.000000 mercury-2.4.2/mercury/widgets/slider.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      222 2023-02-21 07:28:26.000000 mercury-2.4.2/mercury/widgets/stop.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      826 2024-03-20 14:17:46.000000 mercury-2.4.2/mercury/widgets/table.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4784 2024-05-07 10:41:39.000000 mercury-2.4.2/mercury/widgets/text.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      814 2023-08-29 14:20:20.000000 mercury-2.4.2/mercury/widgets/user.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-10 13:11:11.297097 mercury-2.4.2/mercury.egg-info/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     8683 2024-05-10 13:11:11.000000 mercury-2.4.2/mercury.egg-info/PKG-INFO
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     6978 2024-05-10 13:11:11.000000 mercury-2.4.2/mercury.egg-info/SOURCES.txt
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        1 2024-05-10 13:11:11.000000 mercury-2.4.2/mercury.egg-info/dependency_links.txt
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)       49 2024-05-10 13:11:11.000000 mercury-2.4.2/mercury.egg-info/entry_points.txt
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      508 2024-05-10 13:11:11.000000 mercury-2.4.2/mercury.egg-info/requires.txt
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        8 2024-05-10 13:11:11.000000 mercury-2.4.2/mercury.egg-info/top_level.txt
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      106 2022-03-09 11:04:20.000000 mercury-2.4.2/pyproject.toml
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)       38 2024-05-10 13:11:11.317097 mercury-2.4.2/setup.cfg
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1386 2024-05-10 13:10:14.000000 mercury-2.4.2/setup.py
```

### Comparing `mercury-2.4.1/LICENSE.txt` & `mercury-2.4.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mercury-2.4.1/PKG-INFO` & `mercury-2.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mercury
-Version: 2.4.1
+Version: 2.4.2
 Summary: Turn Jupyter Notebook to Web App and share with non-technical users
 Home-page: https://github.com/mljar/mercury
 Author: MLJAR Sp. z o.o.
 Maintainer: MLJAR Sp. z o.o.
 Maintainer-email: contact@mljar.com
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
```

### Comparing `mercury-2.4.1/README.md` & `mercury-2.4.2/README.md`

 * *Files identical despite different names*

### Comparing `mercury-2.4.1/mercury/apps/accounts/fields.py` & `mercury-2.4.2/mercury/apps/accounts/fields.py`

 * *Files identical despite different names*

### Comparing `mercury-2.4.1/mercury/apps/accounts/migrations/0001_initial.py` & `mercury-2.4.2/mercury/apps/accounts/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `mercury-2.4.1/mercury/apps/accounts/models.py` & `mercury-2.4.2/mercury/apps/accounts/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,20 @@
+import os
 import json
+import binascii
 from enum import Enum
 
 from django.contrib.auth.models import User
 from django.db import models
 from django.db.models.signals import post_save
 from django.dispatch import receiver
 
 from apps.accounts.fields import AutoCreatedField, AutoLastModifiedField
 from apps.accounts.views.utils import is_cloud_version
-
+from rest_framework.authtoken.models import Token
 
 class SiteStatus(str, Enum):
     CREATED = "Created"
     INITIALIZING = "Initializing"
     READY = "Ready"
     ERROR = "Error"
 
@@ -149,7 +151,25 @@
 
 class Secret(models.Model):
     name = models.CharField(max_length=256, blank=False, null=False)
     token = models.TextField(blank=False, null=False)
     created_at = AutoCreatedField()
     created_by = models.ForeignKey(User, on_delete=models.CASCADE)
     hosted_on = models.ForeignKey(Site, on_delete=models.CASCADE)
+
+
+class ApiKey(models.Model):
+    key = models.CharField(max_length=40, primary_key=True)
+    user = models.ForeignKey(User, on_delete=models.CASCADE)
+    created_at = models.DateTimeField(auto_now_add=True)
+
+    def save(self, *args, **kwargs):
+        if not self.key:
+            self.key = self.generate_key()
+        return super().save(*args, **kwargs)
+
+    @classmethod
+    def generate_key(cls):
+        return binascii.hexlify(os.urandom(20)).decode()
+
+    def __str__(self):
+        return self.key
```

### Comparing `mercury-2.4.1/mercury/apps/accounts/serializers.py` & `mercury-2.4.2/mercury/apps/accounts/serializers.py`

 * *Files identical despite different names*

### Comparing `mercury-2.4.1/mercury/apps/accounts/tasks.py` & `mercury-2.4.2/mercury/apps/accounts/tasks.py`

 * *Files identical despite different names*

### Comparing `mercury-2.4.1/mercury/apps/accounts/tests/test_accounts.py` & `mercury-2.4.2/mercury/apps/accounts/tests/test_accounts.py`

 * *Files identical despite different names*

### Comparing `mercury-2.4.1/mercury/apps/accounts/tests/test_invitations.py` & `mercury-2.4.2/mercury/apps/accounts/tests/test_invitations.py`

 * *Files identical despite different names*

### Comparing `mercury-2.4.1/mercury/apps/accounts/tests/test_secrets.py` & `mercury-2.4.2/mercury/apps/accounts/tests/test_secrets.py`

 * *Files identical despite different names*

### Comparing `mercury-2.4.1/mercury/apps/accounts/tests/test_sites.py` & `mercury-2.4.2/mercury/apps/accounts/tests/test_sites.py`

 * *Files identical despite different names*

### Comparing `mercury-2.4.1/mercury/apps/accounts/tests/test_subscription.py` & `mercury-2.4.2/mercury/apps/accounts/tests/test_subscription.py`

 * *Files identical despite different names*

### Comparing `mercury-2.4.1/mercury/apps/accounts/urls.py` & `mercury-2.4.2/mercury/apps/accounts/urls.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,14 +15,17 @@
     AddSecret,
     DeleteSecret,
     ListSecrets,
     WorkerListSecrets,
 )
 from apps.accounts.views.subscription import SubscriptionView
 
+from apps.accounts.views.apikey import (GetApiKey, RegenerateApiKey)
+
+
 router = DefaultRouter()
 router.register(r"api/v1/sites", SiteViewSet, basename="sites")
 router.register(r"api/v1/(?P<site_id>.+)/members", MembershipViewSet, basename="sites")
 
 accounts_urlpatterns = router.urls
 
 accounts_urlpatterns += [
@@ -65,8 +68,11 @@
         WorkerListSecrets.as_view(),
     ),
     re_path(
         "api/v1/subscription",
         SubscriptionView.as_view(),
     ),
     re_path("api/v1/auth/delete-account/", DeleteAccount.as_view()),
+    # api keys
+    re_path("api/v1/auth/api-key", GetApiKey.as_view()),
+    re_path("api/v1/auth/regenerate-api-key", RegenerateApiKey.as_view()),
 ]
```

### Comparing `mercury-2.4.1/mercury/apps/accounts/views/accounts.py` & `mercury-2.4.2/mercury/apps/accounts/views/accounts.py`

 * *Files identical despite different names*

### Comparing `mercury-2.4.1/mercury/apps/accounts/views/invitations.py` & `mercury-2.4.2/mercury/apps/accounts/views/invitations.py`

 * *Files identical despite different names*

### Comparing `mercury-2.4.1/mercury/apps/accounts/views/secrets.py` & `mercury-2.4.2/mercury/apps/accounts/views/secrets.py`

 * *Files identical despite different names*

### Comparing `mercury-2.4.1/mercury/apps/accounts/views/sites.py` & `mercury-2.4.2/mercury/apps/accounts/views/sites.py`

 * *Files identical despite different names*

### Comparing `mercury-2.4.1/mercury/apps/accounts/views/subscription.py` & `mercury-2.4.2/mercury/apps/accounts/views/subscription.py`

 * *Files identical despite different names*

### Comparing `mercury-2.4.1/mercury/apps/accounts/views/utils.py` & `mercury-2.4.2/mercury/apps/accounts/views/utils.py`

 * *Files identical despite different names*

### Comparing `mercury-2.4.1/mercury/apps/nb/exporter.py` & `mercury-2.4.2/mercury/apps/nb/exporter.py`

 * *Files identical despite different names*

### Comparing `mercury-2.4.1/mercury/apps/nb/nbrun.py` & `mercury-2.4.2/mercury/apps/nb/nbrun.py`

 * *Files identical despite different names*

### Comparing `mercury-2.4.1/mercury/apps/nb/tests/test_nbrun.py` & `mercury-2.4.2/mercury/apps/nb/tests/test_nbrun.py`

 * *Files identical despite different names*

### Comparing `mercury-2.4.1/mercury/apps/nb/tests.py` & `mercury-2.4.2/mercury/apps/nb/tests.py`

 * *Files identical despite different names*

### Comparing `mercury-2.4.1/mercury/apps/nbworker/__main__.py` & `mercury-2.4.2/mercury/apps/nbworker/__main__.py`

 * *Files identical despite different names*

### Comparing `mercury-2.4.1/mercury/apps/nbworker/nb.py` & `mercury-2.4.2/mercury/apps/nbworker/nb.py`

 * *Files identical despite different names*

### Comparing `mercury-2.4.1/mercury/apps/nbworker/rest.py` & `mercury-2.4.2/mercury/apps/nbworker/rest.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,14 +81,15 @@
             "show-prompt",
             "continuous_update",
             "static_notebook",
             "description",
             "show_sidebar",
             "full_screen",
             "allow_download",
+            "allow_share",
             "stop_on_error",
         ]:
             if new_params.get(property) is not None and nb_params.get(
                 property
             ) != new_params.get(property):
                 nb_params[property] = new_params.get(property)
                 update_database = True
```

### Comparing `mercury-2.4.1/mercury/apps/nbworker/tests.py` & `mercury-2.4.2/mercury/apps/nbworker/tests.py`

 * *Files identical despite different names*

### Comparing `mercury-2.4.1/mercury/apps/nbworker/utils.py` & `mercury-2.4.2/mercury/apps/nbworker/utils.py`

 * *Files identical despite different names*

### Comparing `mercury-2.4.1/mercury/apps/nbworker/ws.py` & `mercury-2.4.2/mercury/apps/nbworker/ws.py`

 * *Files identical despite different names*

### Comparing `mercury-2.4.1/mercury/apps/notebooks/management/commands/add.py` & `mercury-2.4.2/mercury/apps/notebooks/management/commands/add.py`

 * *Files identical despite different names*

### Comparing `mercury-2.4.1/mercury/apps/notebooks/management/commands/delete.py` & `mercury-2.4.2/mercury/apps/notebooks/management/commands/delete.py`

 * *Files identical despite different names*

### Comparing `mercury-2.4.1/mercury/apps/notebooks/management/commands/list.py` & `mercury-2.4.2/mercury/apps/notebooks/management/commands/list.py`

 * *Files identical despite different names*

### Comparing `mercury-2.4.1/mercury/apps/notebooks/management/commands/watch.py` & `mercury-2.4.2/mercury/apps/notebooks/management/commands/watch.py`

 * *Files identical despite different names*

### Comparing `mercury-2.4.1/mercury/apps/notebooks/migrations/0001_initial.py` & `mercury-2.4.2/mercury/apps/notebooks/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `mercury-2.4.1/mercury/apps/notebooks/models.py` & `mercury-2.4.2/mercury/apps/notebooks/models.py`

 * *Files identical despite different names*

### Comparing `mercury-2.4.1/mercury/apps/notebooks/serializers.py` & `mercury-2.4.2/mercury/apps/notebooks/serializers.py`

 * *Files identical despite different names*

### Comparing `mercury-2.4.1/mercury/apps/notebooks/slides_themes.py` & `mercury-2.4.2/mercury/apps/notebooks/slides_themes.py`

 * *Files identical despite different names*

### Comparing `mercury-2.4.1/mercury/apps/notebooks/tasks.py` & `mercury-2.4.2/mercury/apps/notebooks/tasks.py`

 * *Files identical despite different names*

### Comparing `mercury-2.4.1/mercury/apps/notebooks/urls.py` & `mercury-2.4.2/mercury/apps/notebooks/urls.py`

 * *Files identical despite different names*

### Comparing `mercury-2.4.1/mercury/apps/notebooks/views.py` & `mercury-2.4.2/mercury/apps/notebooks/views.py`

 * *Files identical despite different names*

### Comparing `mercury-2.4.1/mercury/apps/storage/migrations/0001_initial.py` & `mercury-2.4.2/mercury/apps/storage/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `mercury-2.4.1/mercury/apps/storage/migrations/0002_useruploadedfile.py` & `mercury-2.4.2/mercury/apps/storage/migrations/0002_useruploadedfile.py`

 * *Files identical despite different names*

### Comparing `mercury-2.4.1/mercury/apps/storage/models.py` & `mercury-2.4.2/mercury/apps/storage/models.py`

 * *Files identical despite different names*

### Comparing `mercury-2.4.1/mercury/apps/storage/s3utils.py` & `mercury-2.4.2/mercury/apps/storage/s3utils.py`

 * *Files identical despite different names*

### Comparing `mercury-2.4.1/mercury/apps/storage/storage.py` & `mercury-2.4.2/mercury/apps/storage/storage.py`

 * *Files identical despite different names*

### Comparing `mercury-2.4.1/mercury/apps/storage/tests.py` & `mercury-2.4.2/mercury/apps/storage/tests.py`

 * *Files identical despite different names*

### Comparing `mercury-2.4.1/mercury/apps/storage/urls.py` & `mercury-2.4.2/mercury/apps/storage/urls.py`

 * *Files identical despite different names*

### Comparing `mercury-2.4.1/mercury/apps/storage/utils.py` & `mercury-2.4.2/mercury/apps/storage/utils.py`

 * *Files identical despite different names*

### Comparing `mercury-2.4.1/mercury/apps/storage/views/dashboardfiles.py` & `mercury-2.4.2/mercury/apps/storage/views/dashboardfiles.py`

 * *Files identical despite different names*

### Comparing `mercury-2.4.1/mercury/apps/storage/views/notebookfiles.py` & `mercury-2.4.2/mercury/apps/storage/views/notebookfiles.py`

 * *Files identical despite different names*

### Comparing `mercury-2.4.1/mercury/apps/storage/views/stylefiles.py` & `mercury-2.4.2/mercury/apps/storage/views/stylefiles.py`

 * *Files identical despite different names*

### Comparing `mercury-2.4.1/mercury/apps/storage/views/workerfiles.py` & `mercury-2.4.2/mercury/apps/storage/views/workerfiles.py`

 * *Files identical despite different names*

### Comparing `mercury-2.4.1/mercury/apps/tasks/export_pdf.py` & `mercury-2.4.2/mercury/apps/tasks/export_pdf.py`

 * *Files identical despite different names*

### Comparing `mercury-2.4.1/mercury/apps/tasks/export_png.py` & `mercury-2.4.2/mercury/apps/tasks/export_png.py`

 * *Files identical despite different names*

### Comparing `mercury-2.4.1/mercury/apps/tasks/migrations/0001_initial.py` & `mercury-2.4.2/mercury/apps/tasks/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `mercury-2.4.1/mercury/apps/tasks/migrations/0002_restapitask.py` & `mercury-2.4.2/mercury/apps/tasks/migrations/0002_restapitask.py`

 * *Files identical despite different names*

### Comparing `mercury-2.4.1/mercury/apps/tasks/models.py` & `mercury-2.4.2/mercury/apps/tasks/models.py`

 * *Files identical despite different names*

### Comparing `mercury-2.4.1/mercury/apps/tasks/notify.py` & `mercury-2.4.2/mercury/apps/tasks/notify.py`

 * *Files identical despite different names*

### Comparing `mercury-2.4.1/mercury/apps/tasks/tasks.py` & `mercury-2.4.2/mercury/apps/tasks/tasks.py`

 * *Files identical despite different names*

### Comparing `mercury-2.4.1/mercury/apps/tasks/tasks_export.py` & `mercury-2.4.2/mercury/apps/tasks/tasks_export.py`

 * *Files identical despite different names*

### Comparing `mercury-2.4.1/mercury/apps/tasks/urls.py` & `mercury-2.4.2/mercury/apps/tasks/urls.py`

 * *Files identical despite different names*

### Comparing `mercury-2.4.1/mercury/apps/tasks/views.py` & `mercury-2.4.2/mercury/apps/tasks/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 from apps.workers.models import Worker
 from apps.ws.tasks import task_start_websocket_worker
 
 from apps.tasks.models import RestAPITask
 
 from rest_framework import permissions
-from apps.accounts.views.permissions import HasEditRights
+from apps.accounts.views.permissions import HasEditRights, apiKeyToUser
 
 
 class TaskCreateView(CreateAPIView):
     serializer_class = TaskSerializer
     queryset = Task.objects.all()
 
     def perform_create(self, serializer):
@@ -193,14 +193,15 @@
             notebook_id=notebook.id,
             session_id=self.kwargs["session_id"],
         )
 
 
 class CreateRestAPITask(APIView):
     def post(self, request, site_id, notebook_slug):
+        apiKeyToUser(request)
         try:
             notebook = (
                 notebooks_queryset(request, site_id).filter(slug=notebook_slug).latest("id")
             )
         except Notebook.DoesNotExist:
             raise Http404()
         try:
```

### Comparing `mercury-2.4.1/mercury/apps/workers/constants.py` & `mercury-2.4.2/mercury/apps/workers/constants.py`

 * *Files identical despite different names*

### Comparing `mercury-2.4.1/mercury/apps/workers/migrations/0001_initial.py` & `mercury-2.4.2/mercury/apps/workers/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `mercury-2.4.1/mercury/apps/workers/migrations/0002_machine.py` & `mercury-2.4.2/mercury/apps/workers/migrations/0002_machine.py`

 * *Files identical despite different names*

### Comparing `mercury-2.4.1/mercury/apps/workers/migrations/0003_worker_run_by_workersession.py` & `mercury-2.4.2/mercury/apps/workers/migrations/0003_worker_run_by_workersession.py`

 * *Files identical despite different names*

### Comparing `mercury-2.4.1/mercury/apps/workers/models.py` & `mercury-2.4.2/mercury/apps/workers/models.py`

 * *Files identical despite different names*

### Comparing `mercury-2.4.1/mercury/apps/workers/tests.py` & `mercury-2.4.2/mercury/apps/workers/tests.py`

 * *Files identical despite different names*

### Comparing `mercury-2.4.1/mercury/apps/workers/urls.py` & `mercury-2.4.2/mercury/apps/workers/urls.py`

 * *Files identical despite different names*

### Comparing `mercury-2.4.1/mercury/apps/workers/views.py` & `mercury-2.4.2/mercury/apps/workers/views.py`

 * *Files identical despite different names*

### Comparing `mercury-2.4.1/mercury/apps/ws/client.py` & `mercury-2.4.2/mercury/apps/ws/client.py`

 * *Files identical despite different names*

### Comparing `mercury-2.4.1/mercury/apps/ws/middleware.py` & `mercury-2.4.2/mercury/apps/ws/middleware.py`

 * *Files identical despite different names*

### Comparing `mercury-2.4.1/mercury/apps/ws/tasks.py` & `mercury-2.4.2/mercury/apps/ws/tasks.py`

 * *Files identical despite different names*

### Comparing `mercury-2.4.1/mercury/apps/ws/utils.py` & `mercury-2.4.2/mercury/apps/ws/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,14 +129,15 @@
                     if view.get("static_notebook") is not None:
                         params["static_notebook"] = view.get("static_notebook")
 
                     for property in [
                         "show_sidebar",
                         "full_screen",
                         "allow_download",
+                        "allow_share",
                         "stop_on_error",
                     ]:
                         if view.get(property) is not None:
                             params[property] = view.get(property)
 
                 else:
                     params["params"][widget_key] = WidgetsManager.frontend_format(view)
@@ -155,14 +156,16 @@
         params["static_notebook"] = not mercury_package_imported
     if params.get("show_sidebar") is None:
         params["show_sidebar"] = True
     if params.get("full_screen") is None:
         params["full_screen"] = True
     if params.get("allow_download") is None:
         params["allow_download"] = True
+    if params.get("allow_share") is None:
+        params["allow_share"] = True
     if params.get("stop_on_error") is None:
         params["stop_on_error"] = False
 
     if no_outputs:
         params["version"] = "2"
         params["show-code"] = False
         params["show-prompt"] = False
```

### Comparing `mercury-2.4.1/mercury/apps/ws/worker.py` & `mercury-2.4.2/mercury/apps/ws/worker.py`

 * *Files identical despite different names*

### Comparing `mercury-2.4.1/mercury/demo.py` & `mercury-2.4.2/mercury/demo.py`

 * *Files identical despite different names*

### Comparing `mercury-2.4.1/mercury/frontend-dist/asset-manifest.json` & `mercury-2.4.2/mercury/frontend-dist/asset-manifest.json`

 * *Files 13% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8974358974358974%*

 * *Differences: {"'entrypoints'": "{insert: [(4, 'static/js/main.71279c97.chunk.js')], delete: [4]}",*

 * * "'files'": "{'main.js': '/static/js/main.71279c97.chunk.js', 'main.js.map': "*

 * *            "'/static/js/main.71279c97.chunk.js.map'}"}*

```diff
@@ -1,20 +1,20 @@
 {
     "entrypoints": [
         "static/js/runtime-main.248907bc.js",
         "static/css/2.c6cf5ff9.chunk.css",
         "static/js/2.81b1917f.chunk.js",
         "static/css/main.9848f1b3.chunk.css",
-        "static/js/main.51571475.chunk.js"
+        "static/js/main.71279c97.chunk.js"
     ],
     "files": {
         "index.html": "/index.html",
         "main.css": "/static/css/main.9848f1b3.chunk.css",
-        "main.js": "/static/js/main.51571475.chunk.js",
-        "main.js.map": "/static/js/main.51571475.chunk.js.map",
+        "main.js": "/static/js/main.71279c97.chunk.js",
+        "main.js.map": "/static/js/main.71279c97.chunk.js.map",
         "runtime-main.js": "/static/js/runtime-main.248907bc.js",
         "runtime-main.js.map": "/static/js/runtime-main.248907bc.js.map",
         "static/css/2.c6cf5ff9.chunk.css": "/static/css/2.c6cf5ff9.chunk.css",
         "static/css/2.c6cf5ff9.chunk.css.map": "/static/css/2.c6cf5ff9.chunk.css.map",
         "static/css/main.9848f1b3.chunk.css.map": "/static/css/main.9848f1b3.chunk.css.map",
         "static/js/2.81b1917f.chunk.js": "/static/js/2.81b1917f.chunk.js",
         "static/js/2.81b1917f.chunk.js.LICENSE.txt": "/static/js/2.81b1917f.chunk.js.LICENSE.txt",
```

### Comparing `mercury-2.4.1/mercury/frontend-dist/favicon-old.ico` & `mercury-2.4.2/mercury/frontend-dist/favicon-old.ico`

 * *Files identical despite different names*

### Comparing `mercury-2.4.1/mercury/frontend-dist/favicon.ico` & `mercury-2.4.2/mercury/frontend-dist/favicon.ico`

 * *Files identical despite different names*

### Comparing `mercury-2.4.1/mercury/frontend-dist/index.html` & `mercury-2.4.2/mercury/frontend-dist/index.html`

 * *Files 1% similar despite different names*

```diff
@@ -1 +1 @@
-<!doctype html><html lang="en"><head><meta charset="utf-8"/><link rel="icon" href="/static/favicon.ico"/><meta name="viewport" content="width=device-width,initial-scale=1"/><meta name="theme-color" content="#000000"/><meta name="description" content="Mercury: Easily share your Python notebooks"/><link rel="manifest" href="/static/manifest.json"/><script src="https://cdnjs.cloudflare.com/ajax/libs/require.js/2.1.10/require.min.js"></script><link rel="stylesheet" href="/static/jupyter-syntax.css"/><link rel="stylesheet" href="/static/jupyter-additional.css"/><link rel="stylesheet" href="/static/jupyter-theme-light.css"/><title>Mercury - Turn Jupyter Notebook to Web App</title><script src="https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.7/latest.js?config=TeX-AMS_CHTML-full,Safe"></script><script>init_mathjax=function(){window.MathJax&&(MathJax.Hub.Config({showProcessingMessages:!1,TeX:{equationNumbers:{autoNumber:"AMS",useLabelIds:!0}},tex2jax:{inlineMath:[["$","$"],["\\(","\\)"]],displayMath:[["$$","$$"],["\\[","\\]"]],processEscapes:!0,processEnvironments:!0},displayAlign:"center",CommonHTML:{linebreaks:{automatic:!0}}}),MathJax.Hub.Queue(["Typeset",MathJax.Hub]))},init_mathjax()</script><link href="/static/css/2.c6cf5ff9.chunk.css" rel="stylesheet"><link href="/static/css/main.9848f1b3.chunk.css" rel="stylesheet"></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="root"></div><script>!function(e){function r(r){for(var n,f,l=r[0],i=r[1],a=r[2],c=0,s=[];c<l.length;c++)f=l[c],Object.prototype.hasOwnProperty.call(o,f)&&o[f]&&s.push(o[f][0]),o[f]=0;for(n in i)Object.prototype.hasOwnProperty.call(i,n)&&(e[n]=i[n]);for(p&&p(r);s.length;)s.shift()();return u.push.apply(u,a||[]),t()}function t(){for(var e,r=0;r<u.length;r++){for(var t=u[r],n=!0,l=1;l<t.length;l++){var i=t[l];0!==o[i]&&(n=!1)}n&&(u.splice(r--,1),e=f(f.s=t[0]))}return e}var n={},o={1:0},u=[];function f(r){if(n[r])return n[r].exports;var t=n[r]={i:r,l:!1,exports:{}};return e[r].call(t.exports,t,t.exports,f),t.l=!0,t.exports}f.m=e,f.c=n,f.d=function(e,r,t){f.o(e,r)||Object.defineProperty(e,r,{enumerable:!0,get:t})},f.r=function(e){"undefined"!=typeof Symbol&&Symbol.toStringTag&&Object.defineProperty(e,Symbol.toStringTag,{value:"Module"}),Object.defineProperty(e,"__esModule",{value:!0})},f.t=function(e,r){if(1&r&&(e=f(e)),8&r)return e;if(4&r&&"object"==typeof e&&e&&e.__esModule)return e;var t=Object.create(null);if(f.r(t),Object.defineProperty(t,"default",{enumerable:!0,value:e}),2&r&&"string"!=typeof e)for(var n in e)f.d(t,n,function(r){return e[r]}.bind(null,n));return t},f.n=function(e){var r=e&&e.__esModule?function(){return e.default}:function(){return e};return f.d(r,"a",r),r},f.o=function(e,r){return Object.prototype.hasOwnProperty.call(e,r)},f.p="/";var l=this.webpackJsonpfrontend=this.webpackJsonpfrontend||[],i=l.push.bind(l);l.push=r,l=l.slice();for(var a=0;a<l.length;a++)r(l[a]);var p=i;t()}([])</script><script src="/static/js/2.81b1917f.chunk.js"></script><script src="/static/js/main.51571475.chunk.js"></script></body></html>
+<!doctype html><html lang="en"><head><meta charset="utf-8"/><link rel="icon" href="/static/favicon.ico"/><meta name="viewport" content="width=device-width,initial-scale=1"/><meta name="theme-color" content="#000000"/><meta name="description" content="Mercury: Easily share your Python notebooks"/><link rel="manifest" href="/static/manifest.json"/><script src="https://cdnjs.cloudflare.com/ajax/libs/require.js/2.1.10/require.min.js"></script><link rel="stylesheet" href="/static/jupyter-syntax.css"/><link rel="stylesheet" href="/static/jupyter-additional.css"/><link rel="stylesheet" href="/static/jupyter-theme-light.css"/><title>Mercury - Turn Jupyter Notebook to Web App</title><script src="https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.7/latest.js?config=TeX-AMS_CHTML-full,Safe"></script><script>init_mathjax=function(){window.MathJax&&(MathJax.Hub.Config({showProcessingMessages:!1,TeX:{equationNumbers:{autoNumber:"AMS",useLabelIds:!0}},tex2jax:{inlineMath:[["$","$"],["\\(","\\)"]],displayMath:[["$$","$$"],["\\[","\\]"]],processEscapes:!0,processEnvironments:!0},displayAlign:"center",CommonHTML:{linebreaks:{automatic:!0}}}),MathJax.Hub.Queue(["Typeset",MathJax.Hub]))},init_mathjax()</script><link href="/static/css/2.c6cf5ff9.chunk.css" rel="stylesheet"><link href="/static/css/main.9848f1b3.chunk.css" rel="stylesheet"></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="root"></div><script>!function(e){function r(r){for(var n,f,l=r[0],i=r[1],a=r[2],c=0,s=[];c<l.length;c++)f=l[c],Object.prototype.hasOwnProperty.call(o,f)&&o[f]&&s.push(o[f][0]),o[f]=0;for(n in i)Object.prototype.hasOwnProperty.call(i,n)&&(e[n]=i[n]);for(p&&p(r);s.length;)s.shift()();return u.push.apply(u,a||[]),t()}function t(){for(var e,r=0;r<u.length;r++){for(var t=u[r],n=!0,l=1;l<t.length;l++){var i=t[l];0!==o[i]&&(n=!1)}n&&(u.splice(r--,1),e=f(f.s=t[0]))}return e}var n={},o={1:0},u=[];function f(r){if(n[r])return n[r].exports;var t=n[r]={i:r,l:!1,exports:{}};return e[r].call(t.exports,t,t.exports,f),t.l=!0,t.exports}f.m=e,f.c=n,f.d=function(e,r,t){f.o(e,r)||Object.defineProperty(e,r,{enumerable:!0,get:t})},f.r=function(e){"undefined"!=typeof Symbol&&Symbol.toStringTag&&Object.defineProperty(e,Symbol.toStringTag,{value:"Module"}),Object.defineProperty(e,"__esModule",{value:!0})},f.t=function(e,r){if(1&r&&(e=f(e)),8&r)return e;if(4&r&&"object"==typeof e&&e&&e.__esModule)return e;var t=Object.create(null);if(f.r(t),Object.defineProperty(t,"default",{enumerable:!0,value:e}),2&r&&"string"!=typeof e)for(var n in e)f.d(t,n,function(r){return e[r]}.bind(null,n));return t},f.n=function(e){var r=e&&e.__esModule?function(){return e.default}:function(){return e};return f.d(r,"a",r),r},f.o=function(e,r){return Object.prototype.hasOwnProperty.call(e,r)},f.p="/";var l=this.webpackJsonpfrontend=this.webpackJsonpfrontend||[],i=l.push.bind(l);l.push=r,l=l.slice();for(var a=0;a<l.length;a++)r(l[a]);var p=i;t()}([])</script><script src="/static/js/2.81b1917f.chunk.js"></script><script src="/static/js/main.71279c97.chunk.js"></script></body></html>
```

### Comparing `mercury-2.4.1/mercury/frontend-dist/jupyter-additional.css` & `mercury-2.4.2/mercury/frontend-dist/jupyter-additional.css`

 * *Files identical despite different names*

### Comparing `mercury-2.4.1/mercury/frontend-dist/jupyter-syntax.css` & `mercury-2.4.2/mercury/frontend-dist/jupyter-syntax.css`

 * *Files identical despite different names*

### Comparing `mercury-2.4.1/mercury/frontend-dist/jupyter-theme-light.css` & `mercury-2.4.2/mercury/frontend-dist/jupyter-theme-light.css`

 * *Files identical despite different names*

### Comparing `mercury-2.4.1/mercury/frontend-dist/mercury_black_logo.svg` & `mercury-2.4.2/mercury/frontend-dist/mercury_black_logo.svg`

 * *Files identical despite different names*

### Comparing `mercury-2.4.1/mercury/frontend-dist/mercury_logo.svg` & `mercury-2.4.2/mercury/frontend-dist/mercury_logo.svg`

 * *Files identical despite different names*

### Comparing `mercury-2.4.1/mercury/frontend-dist/static/css/2.c6cf5ff9.chunk.css` & `mercury-2.4.2/mercury/frontend-dist/static/css/2.c6cf5ff9.chunk.css`

 * *Files identical despite different names*

### Comparing `mercury-2.4.1/mercury/frontend-dist/static/css/2.c6cf5ff9.chunk.css.map` & `mercury-2.4.2/mercury/frontend-dist/static/css/2.c6cf5ff9.chunk.css.map`

 * *Files identical despite different names*

### Comparing `mercury-2.4.1/mercury/frontend-dist/static/css/main.9848f1b3.chunk.css` & `mercury-2.4.2/mercury/frontend-dist/static/css/main.9848f1b3.chunk.css`

 * *Files identical despite different names*

### Comparing `mercury-2.4.1/mercury/frontend-dist/static/css/main.9848f1b3.chunk.css.map` & `mercury-2.4.2/mercury/frontend-dist/static/css/main.9848f1b3.chunk.css.map`

 * *Files identical despite different names*

### Comparing `mercury-2.4.1/mercury/frontend-dist/static/js/2.81b1917f.chunk.js` & `mercury-2.4.2/mercury/frontend-dist/static/js/2.81b1917f.chunk.js`

 * *Files identical despite different names*

### Comparing `mercury-2.4.1/mercury/frontend-dist/static/js/2.81b1917f.chunk.js.LICENSE.txt` & `mercury-2.4.2/mercury/frontend-dist/static/js/2.81b1917f.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mercury-2.4.1/mercury/frontend-dist/static/js/2.81b1917f.chunk.js.map` & `mercury-2.4.2/mercury/frontend-dist/static/js/2.81b1917f.chunk.js.map`

 * *Files identical despite different names*

### Comparing `mercury-2.4.1/mercury/frontend-dist/static/js/main.51571475.chunk.js` & `mercury-2.4.2/mercury/frontend-dist/static/js/main.71279c97.chunk.js`

 * *Files 7% similar despite different names*

#### js-beautify {}

```diff
@@ -627,16 +627,15 @@
                         currentTask: {},
                         historicTask: {},
                         showCurrent: !0,
                         previousTask: {},
                         exportingToPDF: !1,
                         exportToPDFJobId: "",
                         exportToPDFCounter: 0,
-                        executionHistory: [],
-                        restTasks: []
+                        executionHistory: []
                     },
                     reducers: {
                         setShowCurrent: function(e, t) {
                             e.showCurrent = t.payload
                         },
                         setCurrentTask: function(e, t) {
                             e.currentTask = t.payload
@@ -666,57 +665,53 @@
                             e.exportingToPDF = !1, e.exportToPDFJobId = "", e.exportToPDFCounter = 0
                         },
                         setExecutionHistory: function(e, t) {
                             e.executionHistory = t.payload
                         },
                         clearExecutionHistory: function(e) {
                             e.executionHistory = []
-                        },
-                        setRestTasks: function(e, t) {
-                            e.restTasks = t.payload
                         }
                     }
                 }),
                 ot = at.reducer,
                 it = at.actions,
                 st = (it.setShowCurrent, it.setCurrentTask, it.setHistoricTask, it.setPreviousTask, it.copyCurrentToPreviousTask, it.setExportingToPDF),
                 rt = it.setExportToPDFJobId,
                 ct = it.resetExportToPDFCounter,
                 lt = it.increaseExportToPDFCounter,
                 dt = it.stopPDFExport,
                 ut = (it.setExecutionHistory, it.clearExecutionHistory),
-                bt = it.setRestTasks,
-                pt = function(e) {
+                bt = function(e) {
                     return e.tasks.currentTask
                 },
-                jt = function(e) {
+                pt = function(e) {
                     return e.tasks.historicTask
                 },
-                ht = function(e) {
+                jt = function(e) {
                     return e.tasks.previousTask
                 },
-                vt = function(e) {
+                ht = function(e) {
                     return e.tasks.exportingToPDF
                 },
-                ft = function(e) {
+                vt = function(e) {
                     return e.tasks.exportToPDFJobId
                 },
-                mt = function(e) {
+                ft = function(e) {
                     return e.tasks.exportToPDFCounter
                 },
-                xt = function() {
+                mt = function() {
                     try {
                         var e, t, n = document.getElementById("main-iframe"),
                             a = null === n || void 0 === n || null === (e = n.contentWindow) || void 0 === e || null === (t = e.location) || void 0 === t ? void 0 : t.hash;
                         if (a) return a
                     } catch (o) {}
                     return ""
                 };
 
-            function Ot(e) {
+            function xt(e) {
                 var t = e.widgetKey,
                     n = e.label,
                     o = e.value,
                     i = e.disabled,
                     r = e.hidden,
                     l = e.runNb,
                     d = e.url_key,
@@ -761,15 +756,15 @@
                             color: i ? "#555" : "#212529"
                         },
                         children: n
                     })]
                 })
             }
 
-            function gt(e) {
+            function Ot(e) {
                 var t = e.widgetKey,
                     n = e.label,
                     o = e.value,
                     i = e.min,
                     r = e.max,
                     l = e.step,
                     d = e.disabled,
@@ -859,17 +854,17 @@
                                 border: "none"
                             },
                             children: "Press enter or click to apply"
                         })
                     })]
                 })
             }
-            var yt = n(58);
+            var gt = n(58);
 
-            function wt(e) {
+            function yt(e) {
                 var t = e.widgetKey,
                     n = e.label,
                     o = e.value,
                     i = e.min,
                     r = e.max,
                     l = e.step,
                     d = (e.vertical, e.disabled),
@@ -913,15 +908,15 @@
                     }), Object(E.jsx)("div", {
                         style: {
                             paddingTop: "12px",
                             display: "flex",
                             justifyContent: "center",
                             flexWrap: "wrap"
                         },
-                        children: Object(E.jsx)(yt.Range, {
+                        children: Object(E.jsx)(gt.Range, {
                             disabled: d,
                             values: k,
                             step: v,
                             min: j,
                             max: h,
                             onChange: function(e) {
                                 g(!0), f(Ie()), f(Ue({
@@ -945,15 +940,15 @@
                                     }),
                                     children: Object(E.jsxs)("div", {
                                         ref: t.ref,
                                         style: {
                                             height: "5px",
                                             width: "100%",
                                             borderRadius: "4px",
-                                            background: Object(yt.getTrackBackground)({
+                                            background: Object(gt.getTrackBackground)({
                                                 values: k,
                                                 colors: ["#ccc", d ? "rgba(0, 0, 0, 0.3)" : "#2684ff", "#ccc"],
                                                 min: j,
                                                 max: h
                                             }),
                                             alignSelf: "center"
                                         },
@@ -1018,17 +1013,17 @@
                                     })]
                                 }))
                             }
                         })
                     })]
                 })
             }
-            var kt = n(172);
+            var wt = n(172);
 
-            function Nt(e) {
+            function kt(e) {
                 var t = e.widgetKey,
                     n = e.label,
                     o = e.value,
                     i = e.choices,
                     r = e.multi,
                     l = e.disabled,
                     d = e.hidden,
@@ -1100,15 +1095,15 @@
                     },
                     children: [Object(E.jsx)("label", {
                         htmlFor: "select-".concat(n),
                         style: {
                             color: l ? "#555" : "#212529"
                         },
                         children: n
-                    }), Object(E.jsx)(kt.a, {
+                    }), Object(E.jsx)(wt.a, {
                         id: "select-".concat(n),
                         isDisabled: l,
                         name: n || "Select",
                         styles: m,
                         value: r ? y : g,
                         options: w,
                         isMulti: r,
@@ -1132,15 +1127,15 @@
                                     }))
                                 }
                         }
                     })]
                 })
             }
 
-            function St(e) {
+            function Nt(e) {
                 var t = e.widgetKey,
                     n = e.label,
                     o = e.value,
                     i = e.min,
                     r = e.max,
                     l = e.step,
                     d = (e.vertical, e.disabled),
@@ -1182,15 +1177,15 @@
                     }), Object(E.jsx)("div", {
                         style: {
                             paddingTop: "12px",
                             display: "flex",
                             justifyContent: "center",
                             flexWrap: "wrap"
                         },
-                        children: Object(E.jsx)(yt.Range, {
+                        children: Object(E.jsx)(gt.Range, {
                             disabled: d,
                             values: k,
                             step: g,
                             min: x,
                             max: O,
                             onChange: function(e) {
                                 m(!0), j(Ue({
@@ -1214,15 +1209,15 @@
                                     }),
                                     children: Object(E.jsxs)("div", {
                                         ref: t.ref,
                                         style: {
                                             height: "5px",
                                             width: "100%",
                                             borderRadius: "4px",
-                                            background: Object(yt.getTrackBackground)({
+                                            background: Object(gt.getTrackBackground)({
                                                 values: k,
                                                 colors: [d ? "rgba(0, 0, 0, 0.3)" : "#2684ff", "#ccc"],
                                                 min: x,
                                                 max: O
                                             }),
                                             alignSelf: "center"
                                         },
@@ -1286,23 +1281,23 @@
                                     })]
                                 }))
                             }
                         })
                     })]
                 })
             }
-            var _t = n(101),
-                Tt = n(127),
-                Pt = n.n(Tt),
-                Ct = n(128),
-                Rt = n.n(Ct),
-                Et = n(129),
-                At = n.n(Et);
+            var St = n(101),
+                _t = n(127),
+                Tt = n.n(_t),
+                Pt = n(128),
+                Ct = n.n(Pt),
+                Rt = n(129),
+                Et = n.n(Rt);
 
-            function Lt(e) {
+            function At(e) {
                 var t = e.widgetKey,
                     n = e.label,
                     o = e.maxFileSize,
                     r = e.disabled,
                     c = e.hidden,
                     l = e.value,
                     b = e.runNb,
@@ -1464,15 +1459,15 @@
                     children: [Object(E.jsx)("label", {
                         htmlFor: "file-".concat(n),
                         style: {
                             color: r ? "#555" : "#212529"
                         },
                         children: n
                     }), Object(E.jsx)("div", {
-                        children: Object(E.jsx)(_t.FilePond, {
+                        children: Object(E.jsx)(St.FilePond, {
                             disabled: r,
                             maxFileSize: w,
                             onprocessfile: function(e, n) {
                                 x(!0), j(Ue({
                                     key: t,
                                     value: [n.filename, n.serverId]
                                 }))
@@ -1480,15 +1475,15 @@
                             server: "media" === O ? k : N,
                             labelIdle: 'Drag & Drop your file or <span class="filepond--label-action">Browse</span>'
                         })
                     })]
                 })
             }
 
-            function Dt(e) {
+            function Lt(e) {
                 var t = e.widgetKey,
                     n = e.label,
                     o = e.value,
                     i = e.rows,
                     r = e.disabled,
                     l = e.hidden,
                     d = e.runNb,
@@ -1591,50 +1586,50 @@
                                 border: "none"
                             },
                             children: "Apply"
                         })
                     })]
                 })
             }
-            Object(_t.registerPlugin)(Pt.a, Rt.a, At.a);
-            var Ft, Ut, Wt = n(312),
-                It = n(314),
-                Mt = n(87),
-                Ht = n(90),
-                zt = n(88);
+            Object(St.registerPlugin)(Tt.a, Ct.a, Et.a);
+            var Dt, Ft, Ut = n(312),
+                Wt = n(314),
+                It = n(87),
+                Mt = n(90),
+                Ht = n(88);
 
-            function Bt(e) {
+            function zt(e) {
                 var t = e.value,
                     n = e.disabled;
                 return Object(E.jsx)("div", {
                     className: "form-group mb-3",
                     style: {
                         color: n ? "#555" : "#212529"
                     },
-                    children: Object(E.jsx)(Wt.a, {
-                        rehypePlugins: [Mt.a, It.a, Ht.a, zt.a],
+                    children: Object(E.jsx)(Ut.a, {
+                        rehypePlugins: [It.a, Wt.a, Mt.a, Ht.a],
                         children: t
                     })
                 })
             }! function(e) {
                 e.Connecting = "Connecting", e.Connected = "Connected", e.Unknown = "Unknown", e.Disconnected = "Disconnected"
-            }(Ft || (Ft = {})),
+            }(Dt || (Dt = {})),
             function(e) {
                 e.Unknown = "Unknown", e.Starting = "Starting", e.Running = "Running", e.Missing = "Missing", e.Busy = "Busy", e.Queued = "Queued", e.MaxRunTimeReached = "MaxRunTimeReached", e.MaxIdleTimeReached = "MaxIdleTimeReached", e.UsageLimitReached = "UsageLimitReached"
-            }(Ut || (Ut = {}));
-            var Vt = {
-                    webSocketState: Ft.Unknown,
-                    workerState: Ut.Unknown,
+            }(Ft || (Ft = {}));
+            var Bt = {
+                    webSocketState: Dt.Unknown,
+                    workerState: Ft.Unknown,
                     workerId: void 0,
                     notebookSrc: "",
                     tryConnectCount: 0
                 },
-                Kt = Object(b.b)({
+                Vt = Object(b.b)({
                     name: "ws",
-                    initialState: Vt,
+                    initialState: Bt,
                     reducers: {
                         setWebSocketState: function(e, t) {
                             e.webSocketState = t.payload
                         },
                         setWorkerState: function(e, t) {
                             e.workerState = t.payload
                         },
@@ -1648,97 +1643,97 @@
                             e.tryConnectCount += 1
                         },
                         resetTryConnectCount: function(e) {
                             e.tryConnectCount = 0
                         }
                     }
                 }),
-                Jt = Kt.reducer,
-                qt = Kt.actions,
-                Yt = qt.setWebSocketState,
-                Gt = qt.setWorkerState,
-                Qt = qt.setWorkerId,
-                Zt = qt.setNotebookSrc,
-                Xt = qt.increaseTryConnectCount,
-                $t = qt.resetTryConnectCount,
-                en = function(e) {
+                Kt = Vt.reducer,
+                Jt = Vt.actions,
+                qt = Jt.setWebSocketState,
+                Yt = Jt.setWorkerState,
+                Gt = Jt.setWorkerId,
+                Qt = Jt.setNotebookSrc,
+                Zt = Jt.increaseTryConnectCount,
+                Xt = Jt.resetTryConnectCount,
+                $t = function(e) {
                     return e.ws.webSocketState
                 },
-                tn = function(e) {
+                en = function(e) {
                     return e.ws.workerState
                 },
-                nn = function(e) {
+                tn = function(e) {
                     return e.ws.workerId
                 },
-                an = function(e) {
+                nn = function(e) {
                     return e.ws.notebookSrc
                 },
-                on = function(e) {
+                an = function(e) {
                     return e.ws.tryConnectCount
                 },
-                sn = function(e) {
+                on = function(e) {
                     return {
                         purpose: "run-notebook",
                         widgets: e
                     }
                 },
-                rn = Object(a.createContext)(void 0),
-                cn = "ws://127.0.0.1:8000",
-                ln = !0;
+                sn = Object(a.createContext)(void 0),
+                rn = "ws://127.0.0.1:8000",
+                cn = !0;
             Object({
                 NODE_ENV: "production",
                 PUBLIC_URL: "",
                 WDS_SOCKET_HOST: void 0,
                 WDS_SOCKET_PATH: void 0,
                 WDS_SOCKET_PORT: void 0,
                 FAST_REFRESH: !0,
                 REACT_APP_LOCAL_URL: "/static"
-            }).REACT_APP_SERVER_WS ? (cn = Object({
+            }).REACT_APP_SERVER_WS ? (rn = Object({
                 NODE_ENV: "production",
                 PUBLIC_URL: "",
                 WDS_SOCKET_HOST: void 0,
                 WDS_SOCKET_PATH: void 0,
                 WDS_SOCKET_PORT: void 0,
                 FAST_REFRESH: !0,
                 REACT_APP_LOCAL_URL: "/static"
-            }).REACT_APP_SERVER_WS, ln = !1) : "http://localhost:3000" === window.location.origin ? (cn = "ws://127.0.0.1:8000", ln = !0) : (cn = window.location.origin.replace("http://", "ws://").replace("https://", "wss://"), ln = !1), window.location.origin.endsWith("hf.space") && (cn = window.location.origin.replace("http://", "ws://").replace("https://", "wss://"), ln = !1);
-            var dn = 0,
-                un = void 0;
+            }).REACT_APP_SERVER_WS, cn = !1) : "http://localhost:3000" === window.location.origin ? (rn = "ws://127.0.0.1:8000", cn = !0) : (rn = window.location.origin.replace("http://", "ws://").replace("https://", "wss://"), cn = !1), window.location.origin.endsWith("hf.space") && (rn = window.location.origin.replace("http://", "ws://").replace("https://", "wss://"), cn = !1);
+            var ln = 0,
+                dn = void 0;
 
-            function bn(e) {
+            function un(e) {
                 var t = e.children;
                 console.log("WebSocketProvider");
                 var n = Object(s.b)(),
                     o = Object(s.c)(xe),
                     r = Object(s.c)(Ye),
                     c = Object(s.c)(T),
                     l = Object(s.c)(Ge),
                     b = void 0,
                     p = "Unknown";
                 Object(a.useEffect)((function() {
-                    return dn = 0,
+                    return ln = 0,
                         function() {
                             var e;
-                            dn = 6, null === (e = un) || void 0 === e || e.close()
+                            ln = 6, null === (e = dn) || void 0 === e || e.close()
                         }
                 }), []);
                 var j = function(e) {
                     void 0 !== b && b.readyState === b.OPEN && b.send(e)
                 };
 
                 function h(e) {
-                    n($t()), j(JSON.stringify({
+                    n(Xt()), j(JSON.stringify({
                         purpose: "server-address",
-                        address: cn
-                    })), n(Yt(Ft.Connected)), g()
+                        address: rn
+                    })), n(qt(Dt.Connected)), g()
                 }
 
                 function v(e) {
                     var t, a = JSON.parse(e.data);
-                    "purpose" in a && ("worker-state" === a.purpose ? (console.log("worker-state", a.state), p = a.state, n(Gt(a.state)), n(Qt(a.workerId)), (p === Ut.MaxIdleTimeReached || p === Ut.MaxRunTimeReached) && (null === (t = b) || void 0 === t || t.close())) : "executed-notebook" === a.purpose ? ((null === a || void 0 === a ? void 0 : a.reloadNotebook) && void 0 !== r && n(function(e, t) {
+                    "purpose" in a && ("worker-state" === a.purpose ? (console.log("worker-state", a.state), p = a.state, n(Yt(a.state)), n(Gt(a.workerId)), (p === Ft.MaxIdleTimeReached || p === Ft.MaxRunTimeReached) && (null === (t = b) || void 0 === t || t.close())) : "executed-notebook" === a.purpose ? ((null === a || void 0 === a ? void 0 : a.reloadNotebook) && void 0 !== r && n(function(e, t) {
                         var n = arguments.length > 2 && void 0 !== arguments[2] && arguments[2];
                         return function() {
                             var a = Object(u.a)(d.a.mark((function a(o) {
                                 var s, r, c, l, u, b;
                                 return d.a.wrap((function(a) {
                                     for (;;) switch (a.prev = a.next) {
                                         case 0:
@@ -1758,107 +1753,108 @@
                                     [0, 16]
                                 ])
                             })));
                             return function(e) {
                                 return a.apply(this, arguments)
                             }
                         }()
-                    }(o, r)), n(Zt(a.body))) : "update-widgets" === a.purpose ? n(De(a)) : "hide-widgets" === a.purpose ? n(Fe(a)) : "init-widgets" === a.purpose ? (n(Me(a)), n(Be(!0))) : "update-title" === a.purpose ? n(He(a.title)) : "update-show-code" === a.purpose ? n(ze(a.showCode)) : "download-html" !== a.purpose && "download-pdf" !== a.purpose || a.url && a.filename && (n(st(!1)), x(a.url, a.filename)))
+                    }(o, r)), n(Qt(a.body))) : "update-widgets" === a.purpose ? n(De(a)) : "hide-widgets" === a.purpose ? n(Fe(a)) : "init-widgets" === a.purpose ? (n(Me(a)), n(Be(!0))) : "update-title" === a.purpose ? n(He(a.title)) : "update-show-code" === a.purpose ? n(ze(a.showCode)) : "download-html" !== a.purpose && "download-pdf" !== a.purpose || a.url && a.filename && (n(st(!1)), x(a.url, a.filename)))
                 }
 
                 function m(e) {
-                    n(Yt(Ft.Disconnected)), n(Gt(Ut.Unknown))
+                    n(qt(Dt.Disconnected)), n(Yt(Ft.Unknown))
                 }
 
                 function O(e) {
-                    n(Yt(Ft.Disconnected)), b = void 0, p !== Ut.MaxIdleTimeReached && p !== Ut.MaxRunTimeReached && (n(Gt(Ut.Unknown)), n(Qt(void 0)), dn < 5 && setTimeout((function() {
+                    n(qt(Dt.Disconnected)), b = void 0, p !== Ft.MaxIdleTimeReached && p !== Ft.MaxRunTimeReached && (n(Yt(Ft.Unknown)), n(Gt(void 0)), ln < 5 && setTimeout((function() {
                         return y()
                     }), 5e3))
                 }
 
                 function g() {
                     j(JSON.stringify({
                         purpose: "worker-ping"
                     })), void 0 !== b && b.readyState === b.OPEN && setTimeout((function() {
                         return g()
                     }), 1e4)
                 }
 
                 function y() {
-                    if ((ln || !l) && void 0 !== r && void 0 === b && p !== Ut.MaxIdleTimeReached && p !== Ut.MaxRunTimeReached && dn < 5) {
-                        console.log("WS connect ..." + p + " " + dn), n(Xt());
-                        var e = "".concat(cn, "/ws/client/").concat(r, "/").concat(f(), "/");
-                        void 0 !== c && null !== c && "" !== c && (e += "?token=".concat(c)), (b = new WebSocket(e)).onopen = h, b.onmessage = v, b.onerror = m, b.onclose = O, un = b, (dn += 1) >= 5 && n(fe(ue.NetworkError))
+                    if ((cn || !l) && void 0 !== r && void 0 === b && p !== Ft.MaxIdleTimeReached && p !== Ft.MaxRunTimeReached && ln < 5) {
+                        console.log("WS connect ..." + p + " " + ln), n(Zt());
+                        var e = "".concat(rn, "/ws/client/").concat(r, "/").concat(f(), "/");
+                        void 0 !== c && null !== c && "" !== c && (e += "?token=".concat(c)), (b = new WebSocket(e)).onopen = h, b.onmessage = v, b.onerror = m, b.onclose = O, dn = b, (ln += 1) >= 5 && n(fe(ue.NetworkError))
                     }
                 }
                 y();
                 var w = {
                     sendMessage: j
                 };
-                return Object(E.jsx)(rn.Provider, {
+                return Object(E.jsx)(sn.Provider, {
                     value: w,
                     children: t
                 })
             }
 
-            function pn(e) {
+            function bn(e) {
                 var t = e.allowDownload,
-                    n = e.waiting,
-                    o = (e.continuousUpdate, e.staticNotebook),
-                    r = e.notebookId,
-                    c = e.notebookPath,
-                    l = e.notebookTitle,
-                    b = e.runDownloadHTML,
-                    j = e.runDownloadPDF,
-                    h = Object(s.b)(),
-                    v = Object(s.c)(en),
-                    m = Object(s.c)(tn),
-                    O = Object(s.c)(on),
-                    g = Object(s.c)(xe);
+                    n = e.allowShare,
+                    o = e.waiting,
+                    r = (e.continuousUpdate, e.staticNotebook),
+                    c = e.notebookId,
+                    l = e.notebookPath,
+                    b = e.notebookTitle,
+                    j = e.runDownloadHTML,
+                    h = e.runDownloadPDF,
+                    v = Object(s.b)(),
+                    m = Object(s.c)($t),
+                    O = Object(s.c)(en),
+                    g = Object(s.c)(an),
+                    y = Object(s.c)(xe);
                 Object(a.useEffect)((function() {
-                    O >= 5 && h(fe(ue.LostConnection))
-                }), [h, O]);
-                var y = "orange";
-                v === Ft.Connected ? y = "green" : v !== Ft.Disconnected && v !== Ft.Unknown || (y = "red");
+                    g >= 5 && v(fe(ue.LostConnection))
+                }), [v, g]);
                 var w = "orange";
-                return m === Ut.Running || m === Ut.Busy ? w = "green" : m !== Ut.Missing && m !== Ut.Unknown || (w = "red"), Object(E.jsxs)("div", {
+                m === Dt.Connected ? w = "green" : m !== Dt.Disconnected && m !== Dt.Unknown || (w = "red");
+                var k = "orange";
+                return O === Ft.Running || O === Ft.Busy ? k = "green" : O !== Ft.Missing && O !== Ft.Unknown || (k = "red"), Object(E.jsxs)("div", {
                     style: {
                         paddingBottom: "25px"
                     },
-                    children: [void 0 !== r && !o && Object(E.jsxs)(E.Fragment, {
+                    children: [void 0 !== c && !r && Object(E.jsxs)(E.Fragment, {
                         children: [Object(E.jsx)("span", {
-                            title: "WebSocket: ".concat(v),
+                            title: "WebSocket: ".concat(m),
                             children: Object(E.jsxs)("svg", {
                                 xmlns: "http://www.w3.org/2000/svg",
                                 width: "16",
                                 height: "16",
-                                fill: y,
+                                fill: w,
                                 className: "bi bi-wifi",
                                 viewBox: "0 0 16 16",
                                 children: [Object(E.jsx)("path", {
                                     d: "M15.384 6.115a.485.485 0 0 0-.047-.736A12.444 12.444 0 0 0 8 3C5.259 3 2.723 3.882.663 5.379a.485.485 0 0 0-.048.736.518.518 0 0 0 .668.05A11.448 11.448 0 0 1 8 4c2.507 0 4.827.802 6.716 2.164.205.148.49.13.668-.049z"
                                 }), Object(E.jsx)("path", {
                                     d: "M13.229 8.271a.482.482 0 0 0-.063-.745A9.455 9.455 0 0 0 8 6c-1.905 0-3.68.56-5.166 1.526a.48.48 0 0 0-.063.745.525.525 0 0 0 .652.065A8.46 8.46 0 0 1 8 7a8.46 8.46 0 0 1 4.576 1.336c.206.132.48.108.653-.065zm-2.183 2.183c.226-.226.185-.605-.1-.75A6.473 6.473 0 0 0 8 9c-1.06 0-2.062.254-2.946.704-.285.145-.326.524-.1.75l.015.015c.16.16.407.19.611.09A5.478 5.478 0 0 1 8 10c.868 0 1.69.201 2.42.56.203.1.45.07.61-.091l.016-.015zM9.06 12.44c.196-.196.198-.52-.04-.66A1.99 1.99 0 0 0 8 11.5a1.99 1.99 0 0 0-1.02.28c-.238.14-.236.464-.04.66l.706.706a.5.5 0 0 0 .707 0l.707-.707z"
                                 })]
                             })
                         }), " ", Object(E.jsx)("span", {
-                            title: "Worker: ".concat(m, "\nSession Id: ").concat(f()),
+                            title: "Worker: ".concat(O, "\nSession Id: ").concat(f()),
                             children: Object(E.jsx)("svg", {
                                 xmlns: "http://www.w3.org/2000/svg",
                                 width: "16",
                                 height: "16",
-                                fill: w,
+                                fill: k,
                                 className: "bi bi-cpu",
                                 viewBox: "0 0 16 16",
                                 children: Object(E.jsx)("path", {
                                     d: "M5 0a.5.5 0 0 1 .5.5V2h1V.5a.5.5 0 0 1 1 0V2h1V.5a.5.5 0 0 1 1 0V2h1V.5a.5.5 0 0 1 1 0V2A2.5 2.5 0 0 1 14 4.5h1.5a.5.5 0 0 1 0 1H14v1h1.5a.5.5 0 0 1 0 1H14v1h1.5a.5.5 0 0 1 0 1H14v1h1.5a.5.5 0 0 1 0 1H14a2.5 2.5 0 0 1-2.5 2.5v1.5a.5.5 0 0 1-1 0V14h-1v1.5a.5.5 0 0 1-1 0V14h-1v1.5a.5.5 0 0 1-1 0V14h-1v1.5a.5.5 0 0 1-1 0V14A2.5 2.5 0 0 1 2 11.5H.5a.5.5 0 0 1 0-1H2v-1H.5a.5.5 0 0 1 0-1H2v-1H.5a.5.5 0 0 1 0-1H2v-1H.5a.5.5 0 0 1 0-1H2A2.5 2.5 0 0 1 4.5 2V.5A.5.5 0 0 1 5 0zm-.5 3A1.5 1.5 0 0 0 3 4.5v7A1.5 1.5 0 0 0 4.5 13h7a1.5 1.5 0 0 0 1.5-1.5v-7A1.5 1.5 0 0 0 11.5 3h-7zM5 6.5A1.5 1.5 0 0 1 6.5 5h3A1.5 1.5 0 0 1 11 6.5v3A1.5 1.5 0 0 1 9.5 11h-3A1.5 1.5 0 0 1 5 9.5v-3zM6.5 6a.5.5 0 0 0-.5.5v3a.5.5 0 0 0 .5.5h3a.5.5 0 0 0 .5-.5v-3a.5.5 0 0 0-.5-.5h-3z"
                                 })
                             })
                         })]
-                    }), m === Ut.Busy && Object(E.jsxs)("span", {
+                    }), O === Ft.Busy && Object(E.jsxs)("span", {
                         title: "Worker is busy",
                         children: [" ", Object(E.jsx)("svg", {
                             xmlns: "http://www.w3.org/2000/svg",
                             width: "16",
                             height: "16",
                             fill: "green",
                             className: "bi bi-activity",
@@ -1875,15 +1871,15 @@
                         children: [t && Object(E.jsxs)("div", {
                             className: "dropdown mx-2 btn-group",
                             style: {},
                             children: [Object(E.jsxs)("button", {
                                 className: "btn btn-sm btn-primary dropdown-toggle",
                                 type: "button",
                                 "data-bs-toggle": "dropdown",
-                                disabled: n,
+                                disabled: o,
                                 children: [Object(E.jsxs)("svg", {
                                     xmlns: "http://www.w3.org/2000/svg",
                                     width: "14",
                                     height: "14",
                                     viewBox: "0 0 24 24",
                                     strokeWidth: "2",
                                     stroke: "currentColor",
@@ -1911,15 +1907,15 @@
                                     children: Object(E.jsxs)("button", {
                                         type: "button",
                                         style: {
                                             cursor: "pointer"
                                         },
                                         className: "dropdown-item",
                                         onClick: function() {
-                                            o ? x("".concat(i.a.defaults.baseURL).concat(c), "".concat(l, ".html")) : b()
+                                            r ? x("".concat(i.a.defaults.baseURL).concat(l), "".concat(b, ".html")) : j()
                                         },
                                         children: [Object(E.jsx)("i", {
                                             className: "fa fa-file-code-o",
                                             "aria-hidden": "true"
                                         }), " ", "Download as HTML"]
                                     })
                                 }), Object(E.jsx)("li", {
@@ -1927,15 +1923,15 @@
                                         className: "dropdown-divider"
                                     })
                                 }), Object(E.jsx)("li", {
                                     children: Object(E.jsxs)("button", {
                                         type: "button",
                                         className: "dropdown-item",
                                         onClick: function() {
-                                            o ? h(function(e, t, n) {
+                                            r ? v(function(e, t, n) {
                                                 return function() {
                                                     var a = Object(u.a)(d.a.mark((function a(o) {
                                                         var s, r, c, l;
                                                         return d.a.wrap((function(a) {
                                                             for (;;) switch (a.prev = a.next) {
                                                                 case 0:
                                                                     return a.prev = 0, o(st(!0)), o(ct()), o(rt("")), s = f(), r = {
@@ -1957,29 +1953,29 @@
                                                             [0, 14]
                                                         ])
                                                     })));
                                                     return function(e) {
                                                         return a.apply(this, arguments)
                                                     }
                                                 }()
-                                            }(g, r, c)) : (h(st(!0)), j())
+                                            }(y, c, l)) : (v(st(!0)), h())
                                         },
                                         children: [Object(E.jsx)("i", {
                                             className: "fa fa-file-pdf-o",
                                             "aria-hidden": "true"
                                         }), " ", "Download as PDF"]
                                     })
                                 })]
                             })]
-                        }), Object(E.jsxs)("button", {
+                        }), n && Object(E.jsxs)("button", {
                             className: "btn btn-sm btn-primary",
                             onClick: function() {
-                                return h(J(!0))
+                                return v(J(!0))
                             },
-                            disabled: n,
+                            disabled: o,
                             children: [Object(E.jsxs)("svg", {
                                 xmlns: "http://www.w3.org/2000/svg",
                                 width: "14",
                                 height: "14",
                                 viewBox: "0 0 24 24",
                                 strokeWidth: "2",
                                 stroke: "currentColor",
@@ -2003,15 +1999,15 @@
                                 })]
                             }), " ", "Share"]
                         })]
                     })]
                 })
             }
 
-            function jn(e) {
+            function pn(e) {
                 var t = e.widgetKey,
                     n = e.label,
                     o = e.style,
                     i = e.value,
                     r = e.disabled,
                     c = e.hidden,
                     l = e.runNb,
@@ -2039,351 +2035,324 @@
                         },
                         disabled: r,
                         children: n
                     })
                 })
             }
 
-            function hn(e) {
+            function jn(e) {
                 var t = e.runNb,
                     n = e.waiting,
                     a = e.workerState;
                 return Object(E.jsxs)("button", {
                     type: "button",
                     className: "btn btn-success",
                     style: {
                         marginRight: "10px",
                         width: "100%"
                     },
                     onClick: function() {
                         t()
                     },
-                    disabled: n || a !== Ut.Running,
-                    children: [a === Ut.Running && Object(E.jsxs)("span", {
+                    disabled: n || a !== Ft.Running,
+                    children: [a === Ft.Running && Object(E.jsxs)("span", {
                         children: [Object(E.jsx)("i", {
                             className: "fa fa-play",
                             "aria-hidden": "true"
                         }), " Run"]
-                    }), a === Ut.Busy && Object(E.jsxs)("span", {
+                    }), a === Ft.Busy && Object(E.jsxs)("span", {
                         children: [Object(E.jsx)("svg", {
                             xmlns: "http://www.w3.org/2000/svg",
                             width: "16",
                             height: "16",
                             fill: "white",
                             className: "bi bi-activity",
                             viewBox: "0 0 16 16",
                             children: Object(E.jsx)("path", {
                                 fillRule: "evenodd",
                                 d: "M6 2a.5.5 0 0 1 .47.33L10 12.036l1.53-4.208A.5.5 0 0 1 12 7.5h3.5a.5.5 0 0 1 0 1h-3.15l-1.88 5.17a.5.5 0 0 1-.94 0L6 3.964 4.47 8.171A.5.5 0 0 1 4 8.5H.5a.5.5 0 0 1 0-1h3.15l1.88-5.17A.5.5 0 0 1 6 2Z"
                             })
                         }), " ", "Busy"]
-                    }), a !== Ut.Busy && a !== Ut.Running && Object(E.jsx)("span", {
+                    }), a !== Ft.Busy && a !== Ft.Running && Object(E.jsx)("span", {
                         children: "Waiting ..."
                     })]
                 })
             }
-            var vn = n(49);
+            var hn = n(49);
 
-            function fn(e) {
+            function vn(e) {
                 var t = e.notebookTitle,
                     n = e.notebookId,
                     o = (e.notebookSchedule, e.taskCreatedAt, e.loadingState, e.waiting),
-                    r = e.widgetsParams,
-                    c = e.watchMode,
-                    l = e.notebookPath,
-                    b = e.displayEmbed,
-                    p = e.showFiles,
-                    j = e.isPresentation,
-                    h = (e.notebookParseErrors, e.continuousUpdate),
-                    v = e.staticNotebook,
-                    f = e.allowDownload,
-                    m = Object(s.b)(),
-                    x = Object(s.c)(Xe),
-                    O = Object(s.c)($e),
-                    g = Object(s.c)(tn),
-                    y = Object(s.c)(et),
-                    w = Object(s.c)(tt),
-                    k = Object(s.c)(xe),
-                    N = Object(a.useContext)(rn),
-                    S = function() {
-                        h && _()
-                    },
-                    _ = function() {
-                        var e = xt();
-                        if (m(Le(e)), O) {
-                            for (var t = {}, n = 0, a = Object.entries(r); n < a.length; n++) {
+                    i = e.widgetsParams,
+                    r = e.watchMode,
+                    c = e.notebookPath,
+                    l = e.displayEmbed,
+                    d = e.showFiles,
+                    u = e.isPresentation,
+                    b = (e.notebookParseErrors, e.continuousUpdate),
+                    p = e.staticNotebook,
+                    j = e.allowDownload,
+                    h = e.allowShare,
+                    v = Object(s.b)(),
+                    f = Object(s.c)(Xe),
+                    m = Object(s.c)($e),
+                    x = Object(s.c)(en),
+                    O = Object(s.c)(et),
+                    g = Object(s.c)(tt),
+                    y = Object(a.useContext)(sn),
+                    w = function() {
+                        b && k()
+                    },
+                    k = function() {
+                        var e = mt();
+                        if (v(Le(e)), m) {
+                            for (var t = {}, n = 0, a = Object.entries(i); n < a.length; n++) {
                                 var o = Object(R.a)(a[n], 2),
-                                    i = o[0];
+                                    s = o[0];
                                 o[1];
-                                i in O ? (t[i] = O[i], m(Ue({
-                                    key: i,
-                                    value: t[i]
-                                }))) : i in x && (t[i] = x[i])
+                                s in m ? (t[s] = m[s], v(Ue({
+                                    key: s,
+                                    value: t[s]
+                                }))) : s in f && (t[s] = f[s])
                             }
-                            N.sendMessage(JSON.stringify(sn(JSON.stringify(t)))), m(Ie())
-                        } else N.sendMessage(JSON.stringify(sn(JSON.stringify(x))))
+                            y.sendMessage(JSON.stringify(on(JSON.stringify(t)))), v(Ie())
+                        } else y.sendMessage(JSON.stringify(on(JSON.stringify(f))))
                     };
                 Object(a.useEffect)((function() {
-                    void 0 !== k && void 0 !== n && m(function(e, t) {
-                        return function() {
-                            var n = Object(u.a)(d.a.mark((function n(a) {
-                                var o, s, r;
-                                return d.a.wrap((function(n) {
-                                    for (;;) switch (n.prev = n.next) {
-                                        case 0:
-                                            return n.prev = 0, a(bt([])), o = "/api/v1/".concat(e, "/").concat(t, "/list-rest-tasks/"), n.next = 5, i.a.get(o);
-                                        case 5:
-                                            s = n.sent, r = s.data, a(bt(r)), n.next = 13;
-                                            break;
-                                        case 10:
-                                            n.prev = 10, n.t0 = n.catch(0), a(bt([]));
-                                        case 13:
-                                        case "end":
-                                            return n.stop()
-                                    }
-                                }), n, null, [
-                                    [0, 10]
-                                ])
-                            })));
-                            return function(e) {
-                                return n.apply(this, arguments)
-                            }
-                        }()
-                    }(k, n))
-                }), [m, n, k]), Object(a.useEffect)((function() {
-                    y && w && (_(), m(Ve(!1)), m(Be(!1)))
-                }), [y, w]);
+                    O && g && (k(), v(Ve(!1)), v(Be(!1)))
+                }), [O, g]);
                 Object(a.useEffect)((function() {
-                    if (r)
-                        for (var e = 0, t = Object.entries(r); e < t.length; e++) {
+                    if (i)
+                        for (var e = 0, t = Object.entries(i); e < t.length; e++) {
                             var n = Object(R.a)(t[e], 2),
                                 a = n[0],
                                 o = n[1];
-                            a in x || ("file" === o.input ? m(Ue({
+                            a in f || ("file" === o.input ? v(Ue({
                                 key: a,
                                 value: []
-                            })) : "text" === o.input ? m(Ue({
+                            })) : "text" === o.input ? v(Ue({
                                 key: a,
                                 value: o.value ? o.value : ""
-                            })) : ce(o) || (re(o) ? m(Ue({
+                            })) : ce(o) || (re(o) ? v(Ue({
                                 key: a,
                                 value: "output-dir"
-                            })) : m(Ue({
+                            })) : v(Ue({
                                 key: a,
                                 value: o.value
                             }))))
                         }
-                }), [m, r, x]);
-                var T = [],
-                    P = [];
-                if (r && !v) {
-                    for (var C = [], A = 0, L = Object.keys(r); A < L.length; A++) {
-                        var D = L[A],
-                            U = D.split(".");
-                        C.push([D, parseFloat("".concat(U[1], ".").concat(U[2]))])
+                }), [v, i, f]);
+                var N = [],
+                    S = [];
+                if (i && !p) {
+                    for (var _ = [], T = 0, P = Object.keys(i); T < P.length; T++) {
+                        var C = P[T],
+                            A = C.split(".");
+                        _.push([C, parseFloat("".concat(A[1], ".").concat(A[2]))])
                     }
-                    C.sort((function(e, t) {
+                    _.sort((function(e, t) {
                         return e[1] - t[1]
                     }));
-                    for (var W = 0, I = C; W < I.length; W++) {
-                        var M = I[W][0],
-                            z = r[M];
-                        ee(z) ? T.push(Object(E.jsx)(Nt, {
-                            widgetKey: M,
-                            disabled: o || (null === z || void 0 === z ? void 0 : z.disabled),
-                            hidden: null === z || void 0 === z ? void 0 : z.hidden,
-                            label: null === z || void 0 === z ? void 0 : z.label,
-                            value: x[M],
-                            choices: null === z || void 0 === z ? void 0 : z.choices,
-                            multi: null === z || void 0 === z ? void 0 : z.multi,
-                            runNb: S,
-                            url_key: null === z || void 0 === z ? void 0 : z.url_key
-                        }, M)) : te(z) ? T.push(Object(E.jsx)(Ot, {
-                            widgetKey: M,
-                            disabled: o || (null === z || void 0 === z ? void 0 : z.disabled),
-                            hidden: null === z || void 0 === z ? void 0 : z.hidden,
-                            label: null === z || void 0 === z ? void 0 : z.label,
-                            value: x[M],
-                            runNb: S,
-                            url_key: null === z || void 0 === z ? void 0 : z.url_key
-                        }, M)) : ne(z) ? T.push(Object(E.jsx)(gt, {
-                            widgetKey: M,
-                            disabled: o || (null === z || void 0 === z ? void 0 : z.disabled),
-                            hidden: null === z || void 0 === z ? void 0 : z.hidden,
-                            label: null === z || void 0 === z ? void 0 : z.label,
-                            value: x[M],
-                            min: null === z || void 0 === z ? void 0 : z.min,
-                            max: null === z || void 0 === z ? void 0 : z.max,
-                            step: null === z || void 0 === z ? void 0 : z.step,
-                            runNb: S,
-                            continuousUpdate: h,
-                            url_key: null === z || void 0 === z ? void 0 : z.url_key
-                        }, M)) : ae(z) ? T.push(Object(E.jsx)(St, {
-                            widgetKey: M,
-                            disabled: o || (null === z || void 0 === z ? void 0 : z.disabled),
-                            hidden: null === z || void 0 === z ? void 0 : z.hidden,
-                            label: null === z || void 0 === z ? void 0 : z.label,
-                            value: x[M],
-                            min: null === z || void 0 === z ? void 0 : z.min,
-                            max: null === z || void 0 === z ? void 0 : z.max,
-                            step: null === z || void 0 === z ? void 0 : z.step,
-                            vertical: null === z || void 0 === z ? void 0 : z.vertical,
-                            runNb: S,
-                            url_key: null === z || void 0 === z ? void 0 : z.url_key
-                        }, M)) : oe(z) ? T.push(Object(E.jsx)(wt, {
-                            widgetKey: M,
-                            disabled: o || (null === z || void 0 === z ? void 0 : z.disabled),
-                            hidden: null === z || void 0 === z ? void 0 : z.hidden,
-                            label: null === z || void 0 === z ? void 0 : z.label,
-                            value: x[M],
-                            min: null === z || void 0 === z ? void 0 : z.min,
-                            max: null === z || void 0 === z ? void 0 : z.max,
-                            step: null === z || void 0 === z ? void 0 : z.step,
-                            vertical: null === z || void 0 === z ? void 0 : z.vertical,
-                            runNb: S,
-                            url_key: z.url_key
-                        }, M)) : ie(z) ? (T.push(Object(E.jsx)(Lt, {
-                            widgetKey: M,
-                            disabled: o || (null === z || void 0 === z ? void 0 : z.disabled),
-                            hidden: null === z || void 0 === z ? void 0 : z.hidden,
-                            label: null === z || void 0 === z ? void 0 : z.label,
-                            maxFileSize: null === z || void 0 === z ? void 0 : z.maxFileSize,
-                            value: x[M],
-                            runNb: S
-                        }, M)), P.push(M)) : se(z) ? T.push(Object(E.jsx)(Dt, {
-                            widgetKey: M,
-                            disabled: o || (null === z || void 0 === z ? void 0 : z.disabled),
-                            hidden: null === z || void 0 === z ? void 0 : z.hidden,
-                            label: null === z || void 0 === z ? void 0 : z.label,
-                            value: x[M],
-                            rows: null === z || void 0 === z ? void 0 : z.rows,
-                            runNb: S,
-                            continuousUpdate: h,
-                            url_key: null === z || void 0 === z ? void 0 : z.url_key,
-                            sanitize: null === z || void 0 === z ? void 0 : z.sanitize
-                        }, M)) : ce(z) ? T.push(Object(E.jsx)(Bt, {
-                            value: z.value,
+                    for (var L = 0, D = _; L < D.length; L++) {
+                        var U = D[L][0],
+                            W = i[U];
+                        ee(W) ? N.push(Object(E.jsx)(kt, {
+                            widgetKey: U,
+                            disabled: o || (null === W || void 0 === W ? void 0 : W.disabled),
+                            hidden: null === W || void 0 === W ? void 0 : W.hidden,
+                            label: null === W || void 0 === W ? void 0 : W.label,
+                            value: f[U],
+                            choices: null === W || void 0 === W ? void 0 : W.choices,
+                            multi: null === W || void 0 === W ? void 0 : W.multi,
+                            runNb: w,
+                            url_key: null === W || void 0 === W ? void 0 : W.url_key
+                        }, U)) : te(W) ? N.push(Object(E.jsx)(xt, {
+                            widgetKey: U,
+                            disabled: o || (null === W || void 0 === W ? void 0 : W.disabled),
+                            hidden: null === W || void 0 === W ? void 0 : W.hidden,
+                            label: null === W || void 0 === W ? void 0 : W.label,
+                            value: f[U],
+                            runNb: w,
+                            url_key: null === W || void 0 === W ? void 0 : W.url_key
+                        }, U)) : ne(W) ? N.push(Object(E.jsx)(Ot, {
+                            widgetKey: U,
+                            disabled: o || (null === W || void 0 === W ? void 0 : W.disabled),
+                            hidden: null === W || void 0 === W ? void 0 : W.hidden,
+                            label: null === W || void 0 === W ? void 0 : W.label,
+                            value: f[U],
+                            min: null === W || void 0 === W ? void 0 : W.min,
+                            max: null === W || void 0 === W ? void 0 : W.max,
+                            step: null === W || void 0 === W ? void 0 : W.step,
+                            runNb: w,
+                            continuousUpdate: b,
+                            url_key: null === W || void 0 === W ? void 0 : W.url_key
+                        }, U)) : ae(W) ? N.push(Object(E.jsx)(Nt, {
+                            widgetKey: U,
+                            disabled: o || (null === W || void 0 === W ? void 0 : W.disabled),
+                            hidden: null === W || void 0 === W ? void 0 : W.hidden,
+                            label: null === W || void 0 === W ? void 0 : W.label,
+                            value: f[U],
+                            min: null === W || void 0 === W ? void 0 : W.min,
+                            max: null === W || void 0 === W ? void 0 : W.max,
+                            step: null === W || void 0 === W ? void 0 : W.step,
+                            vertical: null === W || void 0 === W ? void 0 : W.vertical,
+                            runNb: w,
+                            url_key: null === W || void 0 === W ? void 0 : W.url_key
+                        }, U)) : oe(W) ? N.push(Object(E.jsx)(yt, {
+                            widgetKey: U,
+                            disabled: o || (null === W || void 0 === W ? void 0 : W.disabled),
+                            hidden: null === W || void 0 === W ? void 0 : W.hidden,
+                            label: null === W || void 0 === W ? void 0 : W.label,
+                            value: f[U],
+                            min: null === W || void 0 === W ? void 0 : W.min,
+                            max: null === W || void 0 === W ? void 0 : W.max,
+                            step: null === W || void 0 === W ? void 0 : W.step,
+                            vertical: null === W || void 0 === W ? void 0 : W.vertical,
+                            runNb: w,
+                            url_key: W.url_key
+                        }, U)) : ie(W) ? (N.push(Object(E.jsx)(At, {
+                            widgetKey: U,
+                            disabled: o || (null === W || void 0 === W ? void 0 : W.disabled),
+                            hidden: null === W || void 0 === W ? void 0 : W.hidden,
+                            label: null === W || void 0 === W ? void 0 : W.label,
+                            maxFileSize: null === W || void 0 === W ? void 0 : W.maxFileSize,
+                            value: f[U],
+                            runNb: w
+                        }, U)), S.push(U)) : se(W) ? N.push(Object(E.jsx)(Lt, {
+                            widgetKey: U,
+                            disabled: o || (null === W || void 0 === W ? void 0 : W.disabled),
+                            hidden: null === W || void 0 === W ? void 0 : W.hidden,
+                            label: null === W || void 0 === W ? void 0 : W.label,
+                            value: f[U],
+                            rows: null === W || void 0 === W ? void 0 : W.rows,
+                            runNb: w,
+                            continuousUpdate: b,
+                            url_key: null === W || void 0 === W ? void 0 : W.url_key,
+                            sanitize: null === W || void 0 === W ? void 0 : W.sanitize
+                        }, U)) : ce(W) ? N.push(Object(E.jsx)(zt, {
+                            value: W.value,
                             disabled: o
-                        }, M)) : le(z) ? T.push(Object(E.jsx)(jn, {
-                            widgetKey: M,
-                            disabled: o || (null === z || void 0 === z ? void 0 : z.disabled),
-                            hidden: null === z || void 0 === z ? void 0 : z.hidden,
-                            label: null === z || void 0 === z ? void 0 : z.label,
-                            value: x[M],
-                            style: null === z || void 0 === z ? void 0 : z.style,
-                            runNb: S
-                        }, M)) : re(z) || ("apiresponse" === z.output || console.log("Unknown widget type", z))
+                        }, U)) : le(W) ? N.push(Object(E.jsx)(pn, {
+                            widgetKey: U,
+                            disabled: o || (null === W || void 0 === W ? void 0 : W.disabled),
+                            hidden: null === W || void 0 === W ? void 0 : W.hidden,
+                            label: null === W || void 0 === W ? void 0 : W.label,
+                            value: f[U],
+                            style: null === W || void 0 === W ? void 0 : W.style,
+                            runNb: w
+                        }, U)) : re(W) || ("apiresponse" === W.output || console.log("Unknown widget type", W))
                     }
                 }
-                var B = {};
-                b && (B = {
+                var I = {};
+                l && (I = {
                     padding: "0px"
                 });
-                var K = void 0 === t || null === t || "" === t;
+                var M = void 0 === t || null === t || "" === t;
                 return Object(E.jsx)("nav", {
                     id: "sidebarMenu",
                     className: "col-lg-3 d-md-block bg-light sidebar",
-                    style: Object(F.a)(Object(F.a)({}, B), {}, {
+                    style: Object(F.a)(Object(F.a)({}, I), {}, {
                         overflowY: "auto"
                     }),
-                    children: Object(E.jsx)(vn.a, {
+                    children: Object(E.jsx)(hn.a, {
                         blocking: !1,
                         message: "",
                         children: Object(E.jsxs)("div", {
                             className: "position-sticky p-3",
                             children: [Object(E.jsxs)("h4", {
                                 children: [t, Object(E.jsx)("button", {
                                     className: "btn btn-sm  btn-outline-primary",
                                     type: "button",
                                     style: {
                                         float: "right",
                                         zIndex: "101"
                                     },
                                     onClick: function() {
-                                        return m(V(!1))
+                                        return v(V(!1))
                                     },
                                     "data-toggle": "tooltip",
                                     "data-placement": "right",
                                     title: "Hide sidebar",
                                     children: Object(E.jsx)("i", {
                                         className: "fa fa-chevron-left",
                                         "aria-hidden": "true"
                                     })
                                 })]
                             }), Object(E.jsx)("div", {
                                 style: {
                                     padding: "0px"
                                 },
                                 children: Object(E.jsxs)("form", {
-                                    children: [T, K && Object(E.jsx)("div", {
+                                    children: [N, M && Object(E.jsx)("div", {
                                         style: {
                                             padding: "15px"
                                         }
                                     }), Object(E.jsx)("div", {
                                         className: "form-group mb-3 pb-1 pt-2",
-                                        children: !h && Object(E.jsx)(hn, {
-                                            runNb: _,
+                                        children: !b && Object(E.jsx)(jn, {
+                                            runNb: k,
                                             waiting: o,
-                                            workerState: g
+                                            workerState: x
                                         })
-                                    }), g === Ut.UsageLimitReached && Object(E.jsxs)("div", {
+                                    }), x === Ft.UsageLimitReached && Object(E.jsxs)("div", {
                                         className: "alert alert-info mb-3 mt-3",
                                         role: "alert",
                                         children: [Object(E.jsx)("i", {
                                             className: "fa fa-info-circle",
                                             "aria-hidden": "true"
                                         }), " Usage limit was reached. Please upgrade the plan."]
-                                    }), g === Ut.MaxIdleTimeReached && Object(E.jsxs)("div", {
+                                    }), x === Ft.MaxIdleTimeReached && Object(E.jsxs)("div", {
                                         className: "alert alert-info mb-3 mt-3",
                                         role: "alert",
                                         children: [Object(E.jsx)("i", {
                                             className: "fa fa-info-circle",
                                             "aria-hidden": "true"
                                         }), " Your worker was idle for too long, that's why we have stopped it. Do you need a worker?", Object(E.jsx)("br", {}), Object(E.jsx)("button", {
                                             className: "btn btn-sm btn-primary my-2",
                                             onClick: function() {
                                                 return window.location.reload()
                                             },
                                             children: "Restart worker"
                                         })]
-                                    }), g === Ut.MaxRunTimeReached && Object(E.jsxs)("div", {
+                                    }), x === Ft.MaxRunTimeReached && Object(E.jsxs)("div", {
                                         className: "alert alert-info mb-3 mt-3",
                                         role: "alert",
                                         children: [Object(E.jsx)("i", {
                                             className: "fa fa-info-circle",
                                             "aria-hidden": "true"
                                         }), " Your worker was running for too long, that's why we have stopped it. Do you need a worker?", Object(E.jsx)("br", {}), Object(E.jsx)("button", {
                                             className: "btn btn-sm btn-primary my-2",
                                             onClick: function() {
                                                 return window.location.reload()
                                             },
                                             children: "Restart worker"
                                         })]
-                                    }), o && (g === Ut.Unknown || g === Ut.Queued) && Object(E.jsxs)("div", {
+                                    }), o && (x === Ft.Unknown || x === Ft.Queued) && Object(E.jsxs)("div", {
                                         className: "alert alert-warning mb-3 mt-3",
                                         role: "alert",
                                         children: [Object(E.jsx)("i", {
                                             className: "fa fa-cogs",
                                             "aria-hidden": "true"
                                         }), " Waiting for worker ..."]
-                                    }), o && g === Ut.Starting && Object(E.jsxs)("div", {
+                                    }), o && x === Ft.Starting && Object(E.jsxs)("div", {
                                         className: "alert alert-success mb-3 mt-3",
                                         role: "alert",
                                         children: [Object(E.jsx)("i", {
                                             className: "fa fa-cogs",
                                             "aria-hidden": "true"
                                         }), " Initializing worker ..."]
-                                    }), c && Object(E.jsxs)("div", {
+                                    }), r && Object(E.jsxs)("div", {
                                         className: "alert alert-secondary mb-3 mt-3",
                                         role: "alert",
                                         children: [Object(E.jsx)("i", {
                                             className: "fa fa-refresh",
                                             "aria-hidden": "true"
                                         }), " Notebook in watch mode. All changes to Notebook will be automatically visible in Mercury."]
-                                    }), j && Object(E.jsxs)("div", {
+                                    }), u && Object(E.jsxs)("div", {
                                         className: "alert alert-primary mb-3",
                                         role: "alert",
                                         children: [Object(E.jsx)("i", {
                                             className: "fa fa-television",
                                             "aria-hidden": "true"
                                         }), " Click on presentation and press ", Object(E.jsx)("b", {
                                             children: "F"
@@ -2393,73 +2362,74 @@
                                             className: "fa fa-arrows",
                                             "aria-hidden": "true"
                                         }), " Click on presentation and press ", Object(E.jsx)("b", {
                                             children: "Esc"
                                         }), " to navigate slides."]
                                     })]
                                 })
-                            }), p && Object(E.jsxs)("div", {
+                            }), d && Object(E.jsxs)("div", {
                                 children: [Object(E.jsx)("hr", {}), Object(E.jsxs)("button", {
                                     className: "btn btn-sm btn-outline-secondary",
                                     style: {
                                         border: "none"
                                     },
                                     onClick: function() {
-                                        m(H("app"))
+                                        v(H("app"))
                                     },
                                     children: [Object(E.jsx)("i", {
                                         className: "fa fa-laptop",
                                         "aria-hidden": "true"
                                     }), " App"]
                                 }), Object(E.jsxs)("button", {
                                     className: "btn btn-sm btn-outline-secondary",
                                     style: {
                                         border: "none"
                                     },
                                     onClick: function() {
-                                        m(H("files"))
+                                        v(H("files"))
                                     },
                                     children: [Object(E.jsx)("i", {
                                         className: "fa fa-folder-open-o",
                                         "aria-hidden": "true"
                                     }), " ", "Output Files"]
                                 })]
                             }), Object(E.jsxs)("div", {
                                 children: [Object(E.jsx)("hr", {}), Object(E.jsxs)("div", {
                                     style: {
                                         paddingLeft: "10px"
                                     },
-                                    children: [Object(E.jsx)(pn, {
+                                    children: [Object(E.jsx)(bn, {
                                         notebookId: n,
-                                        notebookPath: l,
+                                        notebookPath: c,
                                         notebookTitle: t,
-                                        staticNotebook: v,
-                                        allowDownload: f,
+                                        staticNotebook: p,
+                                        allowDownload: j,
+                                        allowShare: h,
                                         waiting: o,
-                                        continuousUpdate: h,
+                                        continuousUpdate: b,
                                         runDownloadHTML: function() {
-                                            v || N.sendMessage(JSON.stringify({
+                                            p || y.sendMessage(JSON.stringify({
                                                 purpose: "download-html"
                                             }))
                                         },
                                         runDownloadPDF: function() {
-                                            v || N.sendMessage(JSON.stringify({
+                                            p || y.sendMessage(JSON.stringify({
                                                 purpose: "download-pdf"
                                             }))
                                         }
                                     }), " "]
                                 })]
                             })]
                         })
                     })
                 })
             }
-            var mn = n(170);
+            var fn = n(170);
 
-            function xn(e) {
+            function mn(e) {
                 var t = e.appView,
                     n = e.loadingState,
                     o = e.notebookPath,
                     r = e.waiting,
                     l = e.errorMsg,
                     d = e.watchMode,
                     u = e.displayEmbed,
@@ -2482,15 +2452,15 @@
                                     return window.removeEventListener("resize", e)
                                 }
                         }), []), n
                     }().height,
                     m = u ? f - 10 : f - 58,
                     x = Object(s.b)(),
                     O = Object(s.c)(qe),
-                    g = Object(s.c)(an),
+                    g = Object(s.c)(nn),
                     y = !1;
                 if (void 0 !== O && void 0 !== O.params && void 0 !== O.params["show-code"] && null !== O.params["show-code"] && (y = O.params["show-code"]), "" !== g && !h && (g = "<script>init_mathjax();<\/script>" + g, !y)) {
                     g = '<style type="text/css">\n      .jp-mod-noOutputs {\n          padding: 0px; \n      }\n      .jp-mod-noInput {\n        padding-top: 0px;\n        padding-bottom: 0px;\n      }\n      </style>' + g
                 }
                 if ("" !== g && h && "" !== p && -1 === g.indexOf("Reveal.slide(")) {
                     var w = p.split("/"),
                         k = "";
@@ -2499,15 +2469,15 @@
                 Object(a.useEffect)((function() {
                     if (void 0 !== o && "" === g) {
                         var e = o;
                         "http://localhost:3000" === window.location.origin && e.startsWith("/media") && (e = "http://127.0.0.1:8000" + e), window.location.origin.startsWith("https") && (e = e.replace("http://", "https://"));
                         var t = i.a.defaults.headers.common.Authorization;
                         e.includes("s3.amazonaws.com") && delete i.a.defaults.headers.common.Authorization, i.a.get("".concat(e).concat(p)).then((function(e) {
                             var t = e.data;
-                            h || (t = (t = (t = (t = (t = (t = t.replace(/<head>[\s\S]*?<\/head>/, "")).replace("<html>", "")).replace("</html>", "")).replace("<body", "<div")).replace("</body>", "</div>")).replace("<!DOCTYPE html>", "")), x(Zt(t))
+                            h || (t = (t = (t = (t = (t = (t = t.replace(/<head>[\s\S]*?<\/head>/, "")).replace("<html>", "")).replace("</html>", "")).replace("<body", "<div")).replace("</body>", "</div>")).replace("<!DOCTYPE html>", "")), x(Qt(t))
                         })), e.includes("s3.amazonaws.com") && (i.a.defaults.headers.common.Authorization = t)
                     }
                 }), [x, o, p, h, g]);
                 var N = {
                         paddingTop: "0px",
                         paddingRight: "0px",
                         paddingLeft: v ? "12px" : "0px",
@@ -2518,15 +2488,15 @@
                     maxWidth: "1140px",
                     margin: "auto"
                 });
                 var _ = !1;
                 return j < 12 && window.innerWidth < 992 && (_ = !0), Object(E.jsx)("main", {
                     className: "ms-sm-auto col-".concat(j),
                     style: N,
-                    children: Object(E.jsx)(vn.a, {
+                    children: Object(E.jsx)(hn.a, {
                         tag: "div",
                         blocking: !_ && r,
                         children: Object(E.jsxs)("div", {
                             style: S,
                             children: ["loading" === n && !d && Object(E.jsx)("p", {
                                 children: "Loading notebook. Please wait ..."
                             }), "error" === n && Object(E.jsx)("p", {
@@ -2562,23 +2532,23 @@
                                 height: m,
                                 srcDoc: g,
                                 title: "display",
                                 id: "main-iframe",
                                 onError: function() {
                                     console.log("iframe error")
                                 }
-                            }, o), "" !== g && !h && Object(E.jsx)(mn.a, {
+                            }, o), "" !== g && !h && Object(E.jsx)(fn.a, {
                                 html: g
                             })]
                         })
                     })
                 })
             }
 
-            function On(e) {
+            function xn(e) {
                 var t = e.fname,
                     n = e.downloadLink,
                     a = e.firstItem,
                     o = e.lastItem;
                 return Object(E.jsxs)("div", {
                     style: {
                         border: "1px solid #ddd",
@@ -2621,28 +2591,28 @@
                                 "aria-hidden": "true"
                             }), " Download"]
                         })
                     })]
                 })
             }
 
-            function gn(e) {
+            function On(e) {
                 var t, n = e.files,
                     a = e.filesState,
                     o = e.waiting,
                     r = Object(s.b)(),
                     c = [],
                     l = Object(U.a)(n);
                 try {
                     for (l.s(); !(t = l.n()).done;) {
                         var d, u = t.value,
                             b = u.split("/").pop();
                         if (b = null === (d = b) || void 0 === d ? void 0 : d.split("?")[0], u && b) {
                             var p = "".concat(i.a.defaults.baseURL).concat(u);
-                            u.includes("s3.amazonaws.com") && (p = u), c.push(Object(E.jsx)(On, {
+                            u.includes("s3.amazonaws.com") && (p = u), c.push(Object(E.jsx)(xn, {
                                 fname: b,
                                 downloadLink: p,
                                 firstItem: u === n[0],
                                 lastItem: u === n[n.length - 1]
                             }))
                         }
                     }
@@ -2665,15 +2635,15 @@
                             style: {
                                 paddingBottom: "10px"
                             },
                             children: [Object(E.jsx)("i", {
                                 className: "fa fa-folder-open-o",
                                 "aria-hidden": "true"
                             }), " Output Files"]
-                        }), Object(E.jsx)(vn.a, {
+                        }), Object(E.jsx)(hn.a, {
                             tag: "div",
                             blocking: o,
                             children: Object(E.jsxs)("div", {
                                 children: ["loaded" === a && c, "loaded" === a && 0 === c.length && Object(E.jsx)("div", {
                                     children: "No files available for download"
                                 }), "unknown" === a && Object(E.jsx)("p", {
                                     children: "Please run the notebook to produce output files ..."
@@ -2698,15 +2668,15 @@
                             className: "fa fa-arrow-left",
                             "aria-hidden": "true"
                         }), " Back to App"]
                     })]
                 })
             }
 
-            function yn() {
+            function gn() {
                 return Object(E.jsx)("a", {
                     href: "https://runmercury.com",
                     target: "_blank",
                     rel: "noreferrer",
                     children: Object(E.jsxs)("div", {
                         className: "poweredby",
                         children: [Object(E.jsxs)("div", {
@@ -2726,15 +2696,15 @@
                                 }
                             })
                         })]
                     })
                 })
             }
 
-            function wn(e) {
+            function yn(e) {
                 for (var t = e.slug, n = e.widgetsParams, o = e.notebookPath, r = e.columnsWidth, c = e.taskSessionId, l = Object(a.useState)(JSON.stringify({
                         msg: "Example output"
                     })), b = Object(R.a)(l, 2), p = b[0], j = b[1], h = Object(s.c)(Xe), v = {}, f = 0, m = Object.entries(n); f < m.length; f++) {
                     var x = Object(R.a)(m[f], 2),
                         O = x[0];
                     x[1].input && (v[O] = h[O])
                 }
@@ -2817,19 +2787,19 @@
                         }), Object(E.jsx)("pre", {
                             children: p
                         })]
                     })]
                 })
             }
 
-            function kn() {
+            function wn() {
                 var e = Object(s.b)(),
-                    t = Object(s.c)(mt),
-                    n = Object(s.c)(ft),
-                    o = Object(s.c)(vt);
+                    t = Object(s.c)(ft),
+                    n = Object(s.c)(vt),
+                    o = Object(s.c)(ht);
                 return Object(a.useEffect)((function() {
                     "" !== n && o && (t < 120 ? setTimeout((function() {
                         e(function(e) {
                             return function() {
                                 var t = Object(u.a)(d.a.mark((function t(n) {
                                     var a, o, s;
                                     return d.a.wrap((function(t) {
@@ -2856,15 +2826,15 @@
                         }(n))
                     }), 1e3) : (e(dt()), p.b.error("Problem with PDF export. Please try again later or ask your admin for help.", {
                         autoClose: 6e3
                     })))
                 }), [e, t, n, o]), Object(E.jsx)("div", {})
             }
 
-            function Nn(e) {
+            function kn(e) {
                 var t = e.widgetsParams,
                     n = Object(s.b)(),
                     a = Object(s.c)(X),
                     o = Object(s.c)(Xe),
                     i = !0,
                     r = "?";
                 if (void 0 !== t && null !== t && void 0 !== o && null !== o) {
@@ -3002,46 +2972,46 @@
                                     })
                                 })]
                             })
                         })
                     })
                 })
             }
-            var Sn = "/static/mercury_logo.svg";
-            var _n = function(e) {
+            var Nn = "/static/mercury_logo.svg";
+            var Sn = function(e) {
                 e.isSingleApp;
                 var t, n, o, r, c, l, b = e.notebookSlug,
                     p = e.displayEmbed,
                     j = Object(s.b)(),
                     h = Object(s.c)(qe),
                     v = Object(s.c)(Qe),
-                    m = Object(s.c)(pt),
-                    x = Object(s.c)(jt),
-                    O = Object(s.c)(ht),
+                    m = Object(s.c)(bt),
+                    x = Object(s.c)(pt),
+                    O = Object(s.c)(jt),
                     g = Object(s.c)(q),
                     y = Object(s.c)(G),
                     w = Object(s.c)(Y),
                     k = Object(s.c)(P),
                     N = Object(s.c)(T),
                     S = Object(s.c)(Ze),
                     _ = Object(s.c)(Q),
-                    C = Object(s.c)(vt),
-                    A = Object(s.c)(nn),
-                    L = Object(s.c)(tn),
+                    C = Object(s.c)(ht),
+                    A = Object(s.c)(tn),
+                    L = Object(s.c)(en),
                     U = Object(s.c)(xe),
                     W = Object(s.c)(ge),
                     I = Object(s.c)(we),
                     M = Object(a.useState)("loading"),
                     H = Object(R.a)(M, 2),
                     K = H[0],
                     J = H[1],
                     Z = Object(s.c)(ye),
                     X = function() {
                         var e;
-                        return !(null === h || void 0 === h || null === (e = h.params) || void 0 === e ? void 0 : e.static_notebook) && (L !== Ut.UsageLimitReached && L !== Ut.MaxIdleTimeReached && L !== Ut.MaxRunTimeReached && L !== Ut.Running)
+                        return !(null === h || void 0 === h || null === (e = h.params) || void 0 === e ? void 0 : e.static_notebook) && (L !== Ft.UsageLimitReached && L !== Ft.MaxIdleTimeReached && L !== Ft.MaxRunTimeReached && L !== Ft.Running)
                     },
                     $ = function() {
                         return "WATCH_READY" === h.state || "WATCH_WAIT" === h.state || "WATCH_ERROR" === h.state
                     };
                 Object(a.useEffect)((function() {
                     void 0 !== U && j(function(e, t) {
                         var n = arguments.length > 2 && void 0 !== arguments[2] && arguments[2];
@@ -3103,33 +3073,33 @@
                 }), [j, g, h, A]);
                 var ee = h.default_view_path;
                 m.state && "DONE" === m.state && m.result && (ee = m.result);
                 var te = "";
                 m.state && m.result && "ERROR" === m.state && (te = m.result), x.state && "DONE" === x.state && x.result && (ee = x.result), x.state && x.result && "ERROR" === x.state && (te = x.result), ee === h.default_view_path && O.state && "DONE" === O.state && O.result && (ee = O.result);
                 var ne = !1;
                 return h.output && h.output.toLowerCase().startsWith("rest") && (ne = !0), Object(a.useEffect)((function() {
-                    "" === Z ? J(Sn) : i.a.get("/api/v1/get-style/".concat(U, "/").concat(Z)).then((function(e) {
+                    "" === Z ? J(Nn) : i.a.get("/api/v1/get-style/".concat(U, "/").concat(Z)).then((function(e) {
                         var t = e.data.url;
                         J(t)
                     }))
                 }), [j, Z, U]), Object(E.jsxs)("div", {
                     className: "App",
                     children: [!p && Object(E.jsx)(D, {
                         isSitePublic: W,
                         username: k,
                         logoSrc: K,
                         navbarColor: I
-                    }), Object(E.jsxs)(vn.a, {
+                    }), Object(E.jsxs)(hn.a, {
                         blocking: C,
                         message: "Exporting to PDF. Please wait ...",
-                        children: [C && Object(E.jsx)(kn, {}), Object(E.jsx)("div", {
+                        children: [C && Object(E.jsx)(wn, {}), Object(E.jsx)("div", {
                             className: "container-fluid",
                             children: Object(E.jsxs)("div", {
                                 className: "row",
-                                children: [_ && Object(E.jsx)(fn, {
+                                children: [_ && Object(E.jsx)(vn, {
                                     notebookTitle: h.title,
                                     notebookId: h.id,
                                     notebookSchedule: h.schedule,
                                     taskCreatedAt: m.created_at,
                                     loadingState: v,
                                     waiting: X(),
                                     widgetsParams: null === h || void 0 === h || null === (t = h.params) || void 0 === t ? void 0 : t.params,
@@ -3146,14 +3116,18 @@
                                     isPresentation: void 0 !== h.output && "slides" === h.output,
                                     notebookParseErrors: h.errors,
                                     continuousUpdate: null === h || void 0 === h || null === (o = h.params) || void 0 === o ? void 0 : o.continuous_update,
                                     staticNotebook: null === h || void 0 === h || null === (r = h.params) || void 0 === r ? void 0 : r.static_notebook,
                                     allowDownload: function() {
                                         var e, t;
                                         return void 0 === h || null === h || (void 0 === (null === h || void 0 === h || null === (e = h.params) || void 0 === e ? void 0 : e.allow_download) || null === (null === h || void 0 === h || null === (t = h.params) || void 0 === t ? void 0 : t.allow_download) || h.params.allow_download)
+                                    }(),
+                                    allowShare: function() {
+                                        var e, t;
+                                        return void 0 === h || null === h || (void 0 === (null === h || void 0 === h || null === (e = h.params) || void 0 === e ? void 0 : e.allow_share) || null === (null === h || void 0 === h || null === (t = h.params) || void 0 === t ? void 0 : t.allow_share) || h.params.allow_share)
                                     }()
                                 }), !_ && Object(E.jsx)("div", {
                                     children: Object(E.jsx)("button", {
                                         className: "btn btn-sm  btn-outline-primary",
                                         type: "button",
                                         style: {
                                             position: "absolute",
@@ -3168,21 +3142,21 @@
                                         "data-placement": "right",
                                         title: "Show sidebar",
                                         children: Object(E.jsx)("i", {
                                             className: "fa fa-chevron-right",
                                             "aria-hidden": "true"
                                         })
                                     })
-                                }), ne && Object(E.jsx)(wn, {
+                                }), ne && Object(E.jsx)(yn, {
                                     slug: h.slug,
                                     widgetsParams: null === h || void 0 === h || null === (c = h.params) || void 0 === c ? void 0 : c.params,
                                     notebookPath: ee,
                                     columnsWidth: _ ? 9 : 12,
                                     taskSessionId: m.session_id
-                                }), Object(E.jsx)(xn, {
+                                }), Object(E.jsx)(mn, {
                                     appView: g,
                                     loadingState: v,
                                     notebookPath: ee,
                                     errorMsg: te,
                                     waiting: X(),
                                     watchMode: $(),
                                     displayEmbed: p,
@@ -3190,39 +3164,39 @@
                                     slidesHash: S,
                                     columnsWidth: _ ? 9 : 12,
                                     isPresentation: void 0 !== h.output && "slides" === h.output,
                                     fullScreen: function() {
                                         var e, t;
                                         return void 0 === h || null === h || (void 0 === (null === h || void 0 === h || null === (e = h.params) || void 0 === e ? void 0 : e.full_screen) || null === (null === h || void 0 === h || null === (t = h.params) || void 0 === t ? void 0 : t.full_screen) || h.params.full_screen)
                                     }()
-                                }), "files" === g && Object(E.jsx)(gn, {
+                                }), "files" === g && Object(E.jsx)(On, {
                                     files: y,
                                     filesState: w,
                                     waiting: X()
-                                }), Object(E.jsx)(Nn, {
+                                }), Object(E.jsx)(kn, {
                                     widgetsParams: null === h || void 0 === h || null === (l = h.params) || void 0 === l ? void 0 : l.params
                                 })]
                             })
                         })]
-                    }), p && K === Sn && Object(E.jsx)(yn, {})]
+                    }), p && K === Nn && Object(E.jsx)(gn, {})]
                 })
             };
 
-            function Tn() {
+            function _n() {
                 var e = Object(r.q)().slug,
                     t = Object(r.q)().embed,
                     n = !(!t || "embed" !== t);
-                return Object(E.jsx)(_n, {
+                return Object(E.jsx)(Sn, {
                     isSingleApp: !1,
                     notebookSlug: e,
                     displayEmbed: n
                 })
             }
 
-            function Pn(e) {
+            function Tn(e) {
                 var t = e.footerText;
                 return Object(E.jsxs)("footer", {
                     className: "footer",
                     style: {
                         position: "absolute",
                         bottom: "0",
                         width: "100%",
@@ -3299,15 +3273,15 @@
                             },
                             children: t
                         })
                     })]
                 })
             }
 
-            function Cn(e) {
+            function Pn(e) {
                 var t = e.isSitePublic,
                     n = e.username,
                     a = e.logoSrc,
                     o = e.navbarColor,
                     i = "",
                     s = {};
                 return "" === o ? i = "bg-dark" : s = {
@@ -3352,15 +3326,15 @@
                                 username: n
                             })]
                         })]
                     })
                 })
             }
 
-            function Rn() {
+            function Cn() {
                 var e = Object(s.b)(),
                     t = Object(a.useState)(""),
                     n = Object(R.a)(t, 2),
                     o = n[0],
                     r = n[1],
                     c = Object(a.useState)(""),
                     l = Object(R.a)(c, 2),
@@ -3403,21 +3377,21 @@
                             ])
                         })));
                         return function(t) {
                             return e.apply(this, arguments)
                         }
                     }())
                 }), [e]), Object(a.useEffect)((function() {
-                    void 0 !== T && ("" === S ? y(Sn) : i.a.get("/api/v1/get-style/".concat(T, "/").concat(S)).then((function(e) {
+                    void 0 !== T && ("" === S ? y(Nn) : i.a.get("/api/v1/get-style/".concat(T, "/").concat(S)).then((function(e) {
                         var t = e.data.url;
                         y(t)
                     })))
                 }), [e, S, T]), Object(E.jsxs)("div", {
                     className: "App",
-                    children: [Object(E.jsx)(Cn, {
+                    children: [Object(E.jsx)(Pn, {
                         isSitePublic: N,
                         username: w,
                         logoSrc: g,
                         navbarColor: A
                     }), Object(E.jsx)("div", {
                         className: "container",
                         children: Object(E.jsxs)("div", {
@@ -3566,20 +3540,20 @@
                                             disabled: "" === o || "" === b || "" === f,
                                             children: "Change password"
                                         })
                                     })]
                                 })]
                             })]
                         })
-                    }), Object(E.jsx)(Pn, {
+                    }), Object(E.jsx)(Tn, {
                         footerText: L
                     })]
                 })
             }
-            var En = Object(b.b)({
+            var Rn = Object(b.b)({
                     name: "version",
                     initialState: {
                         fetchingIsPro: !0,
                         isPro: !1,
                         welcome: ""
                     },
                     reducers: {
@@ -3588,26 +3562,26 @@
                             e.isPro = n, e.fetchingIsPro = !1
                         },
                         setWelcome: function(e, t) {
                             e.welcome = t.payload
                         }
                     }
                 }),
-                An = En.reducer,
-                Ln = En.actions,
-                Dn = (Ln.setVersion, Ln.setWelcome),
-                Fn = function(e) {
+                En = Rn.reducer,
+                An = Rn.actions,
+                Ln = (An.setVersion, An.setWelcome),
+                Dn = function(e) {
                     return e.version.welcome
                 };
 
-            function Un() {
+            function Fn() {
                 var e = Object(s.b)(),
                     t = Object(s.c)(Ke),
                     n = Object(s.c)(Je),
-                    o = Object(s.c)(Fn),
+                    o = Object(s.c)(Dn),
                     r = Object(s.c)(P),
                     l = Object(s.c)(T),
                     b = Object(a.useState)(""),
                     p = Object(R.a)(b, 2),
                     j = p[0],
                     h = p[1],
                     v = Object(s.c)(xe),
@@ -3619,29 +3593,29 @@
                     y = O[1],
                     w = Object(s.c)(ye),
                     k = Object(s.c)(we),
                     N = Object(s.c)(ke);
                 Object(a.useEffect)((function() {
                     console.log({
                         logoFilename: w
-                    }), void 0 !== v && ("" === w ? y(Sn) : i.a.get("/api/v1/get-style/".concat(v, "/").concat(w)).then((function(e) {
+                    }), void 0 !== v && ("" === w ? y(Nn) : i.a.get("/api/v1/get-style/".concat(v, "/").concat(w)).then((function(e) {
                         var t = e.data.url;
                         y(t)
                     })))
                 }), [e, w, v]), Object(a.useEffect)((function() {
                     void 0 !== v && (e(nt(v)), void 0 !== m && "" !== m || e(function(e) {
                         return function() {
                             var t = Object(u.a)(d.a.mark((function t(n) {
                                 var a, o, s;
                                 return d.a.wrap((function(t) {
                                     for (;;) switch (t.prev = t.next) {
                                         case 0:
                                             return t.prev = 0, a = "/api/v1/".concat(e, "/welcome/"), t.next = 4, i.a.get(a);
                                         case 4:
-                                            o = t.sent, s = o.data, n(Dn(s.msg)), t.next = 12;
+                                            o = t.sent, s = o.data, n(Ln(s.msg)), t.next = 12;
                                             break;
                                         case 9:
                                             t.prev = 9, t.t0 = t.catch(0), console.log("Problem during loading Mercury welcome message. ".concat(t.t0));
                                         case 12:
                                         case "end":
                                             return t.stop()
                                     }
@@ -3705,42 +3679,45 @@
                                         children: [Object(E.jsx)("h5", {
                                             className: "card-title",
                                             children: S(e.title, 40)
                                         }), Object(E.jsx)("p", {
                                             className: "card-text",
                                             children: S(e.params.description, 100)
                                         })]
-                                    }), j === e.slug && Object(E.jsx)("button", {
+                                    }), j === e.slug && Object(E.jsxs)("button", {
                                         className: "btn btn-outline-primary",
                                         type: "button",
                                         style: {
                                             zIndex: "101",
                                             border: "none",
                                             margin: "5px",
                                             position: "absolute",
                                             right: "0px",
                                             bottom: "0px"
                                         },
                                         "data-toggle": "tooltip",
                                         "data-placement": "right",
                                         title: "Open ".concat(e.title),
-                                        children: Object(E.jsx)("i", {
+                                        children: [Object(E.jsx)("i", {
                                             className: "fa fa-chevron-right",
                                             "aria-hidden": "true"
-                                        })
+                                        }), Object(E.jsx)("i", {
+                                            className: "fa fa-chevron-right",
+                                            "aria-hidden": "true"
+                                        })]
                                     })]
                                 })]
                             })
                         }, "notebook-".concat(e.id, "}"))
                     }));
                 document.body.style.backgroundColor = "white";
                 var C = m;
                 return void 0 !== C && "" !== C || (C = o), Object(E.jsxs)("div", {
                     className: "App",
-                    children: [Object(E.jsx)(Cn, {
+                    children: [Object(E.jsx)(Pn, {
                         isSitePublic: f,
                         username: r,
                         logoSrc: g,
                         navbarColor: k
                     }), Object(E.jsxs)("div", {
                         className: "container",
                         style: {
@@ -3753,37 +3730,37 @@
                             },
                             children: "Welcome!"
                         }), "" !== C && Object(E.jsx)("div", {
                             style: {
                                 paddingTop: "20px",
                                 paddingBottom: "10px"
                             },
-                            children: Object(E.jsx)(Wt.a, {
-                                rehypePlugins: [Mt.a, It.a, Ht.a, zt.a],
+                            children: Object(E.jsx)(Ut.a, {
+                                rehypePlugins: [It.a, Wt.a, Mt.a, Ht.a],
                                 children: C
                             })
                         }), Object(E.jsxs)("div", {
                             className: "row",
                             children: ["loading" === n && Object(E.jsx)("p", {
                                 children: "Loading notebooks. Please wait ..."
                             }), "loaded" === n && 0 === t.length && Object(E.jsx)("div", {
                                 children: Object(E.jsx)("p", {
                                     children: "There are no notebooks available."
                                 })
                             }), "error" === n && Object(E.jsx)("p", {
                                 children: "Problem while loading notebooks. Please try again later or contact Mercury administrator."
                             }), _]
                         })]
-                    }), Object(E.jsx)(Pn, {
+                    }), Object(E.jsx)(Tn, {
                         footerText: N
                     })]
                 })
             }
 
-            function Wn() {
+            function Un() {
                 var e = Object(s.b)(),
                     t = Object(r.o)(),
                     n = Object(a.useState)(""),
                     o = Object(R.a)(n, 2),
                     c = o[0],
                     l = o[1],
                     b = Object(a.useState)(""),
@@ -3803,21 +3780,21 @@
                 var T = "/",
                     P = Object(r.m)();
                 if (P && P.state) {
                     var C = P.state.from;
                     T = C.pathname
                 }
                 return Object(a.useEffect)((function() {
-                    void 0 !== w && ("" === y ? g(Sn) : i.a.get("/api/v1/get-style/".concat(w, "/").concat(y)).then((function(e) {
+                    void 0 !== w && ("" === y ? g(Nn) : i.a.get("/api/v1/get-style/".concat(w, "/").concat(y)).then((function(e) {
                         var t = e.data.url;
                         g(t)
                     })))
                 }), [e, y, w]), Object(E.jsxs)("div", {
                     className: "App",
-                    children: [Object(E.jsx)(Cn, {
+                    children: [Object(E.jsx)(Pn, {
                         isSitePublic: f,
                         username: "",
                         logoSrc: O,
                         navbarColor: k
                     }), Object(E.jsxs)("div", {
                         className: "div-signin text-center",
                         children: [Object(E.jsxs)("form", {
@@ -3901,21 +3878,21 @@
                                 marginTop: "40px"
                             },
                             children: Object(E.jsxs)("p", {
                                 className: "text-muted",
                                 children: ["No account? ", Object(E.jsx)("br", {}), " Please contact administrator to create account for you."]
                             })
                         })]
-                    }), Object(E.jsx)(Pn, {
+                    }), Object(E.jsx)(Tn, {
                         footerText: _
                     })]
                 })
             }
 
-            function In() {
+            function Wn() {
                 return Object(E.jsx)("div", {
                     className: "App",
                     children: Object(E.jsxs)("div", {
                         style: {
                             width: "100%",
                             maxWidth: "500px",
                             padding: "15px",
@@ -3926,15 +3903,15 @@
                         }), Object(E.jsx)("p", {
                             children: "App lost connection to the server. Please try again in a moment or contact administrator."
                         })]
                     })
                 })
             }
 
-            function Mn() {
+            function In() {
                 return Object(E.jsx)("div", {
                     className: "App",
                     children: Object(E.jsxs)("div", {
                         style: {
                             width: "100%",
                             maxWidth: "500px",
                             padding: "15px",
@@ -3948,15 +3925,15 @@
                                 children: "login"
                             }), " to access site."]
                         })]
                     })
                 })
             }
 
-            function Hn() {
+            function Mn() {
                 return Object(E.jsx)("div", {
                     className: "App",
                     children: Object(E.jsx)("div", {
                         style: {
                             width: "100%",
                             maxWidth: "500px",
                             padding: "15px",
@@ -3968,15 +3945,15 @@
                             },
                             children: "Please wait. Loading site ..."
                         })
                     })
                 })
             }
 
-            function zn() {
+            function Hn() {
                 return Object(E.jsx)("div", {
                     className: "App",
                     children: Object(E.jsxs)("div", {
                         style: {
                             width: "100%",
                             maxWidth: "500px",
                             padding: "15px",
@@ -3987,15 +3964,15 @@
                         }), Object(E.jsx)("p", {
                             children: "Please check if you have internet connection and server is running. In case of problems, please contact administrator."
                         })]
                     })
                 })
             }
 
-            function Bn() {
+            function zn() {
                 return Object(E.jsx)("div", {
                     className: "App",
                     children: Object(E.jsxs)("div", {
                         style: {
                             width: "100%",
                             maxWidth: "500px",
                             padding: "15px",
@@ -4006,15 +3983,15 @@
                         }), Object(E.jsx)("p", {
                             children: "We can't find site you are looking for. Please make sure that URL address is correct."
                         })]
                     })
                 })
             }
 
-            function Vn() {
+            function Bn() {
                 return Object(E.jsx)("div", {
                     className: "App",
                     children: Object(E.jsxs)("div", {
                         style: {
                             width: "100%",
                             maxWidth: "500px",
                             padding: "15px",
@@ -4025,15 +4002,15 @@
                         }), Object(E.jsx)("p", {
                             children: "Please try to refresh the website ..."
                         })]
                     })
                 })
             }
 
-            function Kn() {
+            function Vn() {
                 return Object(E.jsx)("div", {
                     className: "App",
                     children: Object(E.jsxs)("div", {
                         style: {
                             width: "100%",
                             maxWidth: "500px",
                             padding: "15px",
@@ -4050,15 +4027,15 @@
                             },
                             children: "Refresh"
                         })]
                     })
                 })
             }
 
-            function Jn() {
+            function Kn() {
                 return Object(E.jsx)("div", {
                     className: "App",
                     children: Object(E.jsxs)("div", {
                         style: {
                             width: "100%",
                             maxWidth: "500px",
                             padding: "15px",
@@ -4069,33 +4046,33 @@
                         }), Object(E.jsx)("p", {
                             children: "We can't find your notebook. Please double check the URL address and permissions."
                         })]
                     })
                 })
             }
 
-            function qn(e) {
+            function Jn(e) {
                 var t = e.children,
                     n = Object(s.c)(T),
                     o = Object(s.c)(ge),
                     i = Object(r.m)(),
                     c = Object(s.b)(),
                     l = Object(s.c)(me);
                 return Object(a.useEffect)((function() {
                     c(Ne())
-                }), [c]), l === ue.Unknown ? Object(E.jsx)(Hn, {}) : l === ue.NotFound ? Object(E.jsx)(Bn, {}) : l === ue.NotReady ? Object(E.jsx)(Kn, {}) : l === ue.AccessForbidden ? Object(E.jsx)(Mn, {}) : l === ue.NetworkError ? Object(E.jsx)(zn, {}) : l === ue.PleaseRefresh ? Object(E.jsx)(Vn, {}) : l === ue.LostConnection ? (window.location.reload(), Object(E.jsx)(In, {})) : l === ue.NotebookNotFound ? Object(E.jsx)(Jn, {}) : o || n ? t : Object(E.jsx)(r.a, {
+                }), [c]), l === ue.Unknown ? Object(E.jsx)(Mn, {}) : l === ue.NotFound ? Object(E.jsx)(zn, {}) : l === ue.NotReady ? Object(E.jsx)(Vn, {}) : l === ue.AccessForbidden ? Object(E.jsx)(In, {}) : l === ue.NetworkError ? Object(E.jsx)(Hn, {}) : l === ue.PleaseRefresh ? Object(E.jsx)(Bn, {}) : l === ue.LostConnection ? (window.location.reload(), Object(E.jsx)(Wn, {})) : l === ue.NotebookNotFound ? Object(E.jsx)(Kn, {}) : o || n ? t : Object(E.jsx)(r.a, {
                     to: "/login",
                     state: {
                         from: i
                     },
                     replace: !0
                 })
             }
 
-            function Yn() {
+            function qn() {
                 var e = Object(s.b)(),
                     t = Object(s.c)(xe),
                     n = Object(s.c)(Ke);
                 Object(a.useEffect)((function() {
                     void 0 !== t && e(nt(t))
                 }), [e, t]);
                 var o = n.map((function(e) {
@@ -4123,88 +4100,88 @@
                     r = ', "/api/v1/get/{task_id}": {\n    "get" : {\n      "operationId": "Get state and result of processed request",\n      "description": "Use this endpoint to check if request processing state and result",\n      "parameters": [\n        {\n          "name": "task_id",\n          "in": "path",\n          "description": "task_id of your request",\n          "required": true,\n          "schema": {\n            "type": "string"\n          }\n        }\n      ],\n      '.concat('"responses": {\n    "200": {\n        "description": "Request processing completed successfully",\n        "content": {\n            "application/json": {\n                "schema": {\n                    "type": "object",\n                    "properties": {\n                      "state": {\n                        "type": "string"\n                      },\n                      "message": {\n                        "type": "string"\n                      },\n                      "result": {\n                        "type": "string"\n                      }\n                  }\n                }\n            }\n        }\n    },\n    "202": {\n      "description": "Request is still processing, please retry in 3 seconds",\n      "content": {\n          "application/json": {\n              "schema": {\n                  "type": "object",\n                  "properties": {\n                    "state": {\n                      "type": "string"\n                    },\n                    "message": {\n                      "type": "string"\n                    }\n                  }\n                }\n              }\n            }\n          }  \n        }', "\n      }\n    }"),
                     c = '{\n    "openapi": "3.0",\n    "info": {\n        "description": "Execute Python notebook and get JSON response",\n        "title": "Mercury OpenAPI",\n        "version": "1.0.0"\n    },\n    "servers": [\n        {\n            "url": "'.concat(i.a.defaults.baseURL, '"\n        }\n    ],\n    "paths": {\n        ').concat(o.join(","), "\n        ").concat(r, "\n  }\n}");
                 return Object(E.jsx)("pre", {
                     children: c
                 })
             }
 
-            function Gn(e) {
+            function Yn(e) {
                 var t = e.children;
                 return Object(E.jsx)(E.Fragment, {
                     children: t
                 })
             }
 
-            function Qn() {
-                return Object(E.jsx)(qn, {
+            function Gn() {
+                return Object(E.jsx)(Jn, {
                     children: Object(E.jsx)(E.Fragment, {
                         children: Object(E.jsx)(r.b, {})
                     })
                 })
             }
 
-            function Zn() {
+            function Qn() {
                 var e = Object(s.b)();
                 return Object(a.useEffect)((function() {
                     f(!0), localStorage.getItem("token") && e(N(localStorage.getItem("token"))), localStorage.getItem("username") && e(S(localStorage.getItem("username"))), e(Ne())
                 }), []), Object(E.jsx)(c.a, {
-                    children: Object(E.jsx)(Gn, {
+                    children: Object(E.jsx)(Yn, {
                         children: Object(E.jsxs)(r.e, {
                             children: [Object(E.jsxs)(r.c, {
                                 path: "/",
-                                element: Object(E.jsx)(Qn, {}),
+                                element: Object(E.jsx)(Gn, {}),
                                 children: [Object(E.jsx)(r.c, {
                                     path: "/",
-                                    element: Object(E.jsx)(Un, {})
+                                    element: Object(E.jsx)(Fn, {})
                                 }), Object(E.jsx)(r.c, {
                                     path: "/app/:slug/:embed?",
-                                    element: Object(E.jsx)(bn, {
-                                        children: Object(E.jsx)(Tn, {})
+                                    element: Object(E.jsx)(un, {
+                                        children: Object(E.jsx)(_n, {})
                                     })
                                 }), Object(E.jsx)(r.c, {
                                     path: "/account",
-                                    element: Object(E.jsx)(Rn, {})
+                                    element: Object(E.jsx)(Cn, {})
                                 }), Object(E.jsx)(r.c, {
                                     path: "/openapi",
-                                    element: Object(E.jsx)(Yn, {})
+                                    element: Object(E.jsx)(qn, {})
                                 })]
                             }), Object(E.jsx)(r.c, {
                                 path: "/login",
-                                element: Object(E.jsx)(Wn, {})
+                                element: Object(E.jsx)(Un, {})
                             })]
                         })
                     })
                 })
             }
-            var Xn = function(e) {
+            var Zn = function(e) {
                     var t = e.store;
                     e.history;
                     return Object(E.jsx)(s.a, {
                         store: t,
-                        children: Object(E.jsx)(Zn, {})
+                        children: Object(E.jsx)(Qn, {})
                     })
                 },
-                $n = n(15),
-                ea = n(171),
-                ta = n(32);
-            var na, aa = Object(ea.a)(),
-                oa = Object(ta.b)({
+                Xn = n(15),
+                $n = n(171),
+                ea = n(32);
+            var ta, na = Object($n.a)(),
+                aa = Object(ea.b)({
                     notebooks: Te,
                     tasks: ot,
-                    version: An,
+                    version: En,
                     app: I,
                     auth: w,
-                    ws: Jt,
+                    ws: Kt,
                     sites: je
                 }),
-                ia = Object($n.a)(Object(b.c)()),
-                sa = (n(285), n(286), n(288), n(289), n(290), n(291), n(292), n(293), Object(b.a)({
-                    reducer: oa,
-                    middleware: ia,
-                    preloadedState: na
+                oa = Object(Xn.a)(Object(b.c)()),
+                ia = (n(285), n(286), n(288), n(289), n(290), n(291), n(292), n(293), Object(b.a)({
+                    reducer: aa,
+                    middleware: oa,
+                    preloadedState: ta
                 }));
             Object({
                 NODE_ENV: "production",
                 PUBLIC_URL: "",
                 WDS_SOCKET_HOST: void 0,
                 WDS_SOCKET_PATH: void 0,
                 WDS_SOCKET_PORT: void 0,
@@ -4216,17 +4193,17 @@
                 WDS_SOCKET_HOST: void 0,
                 WDS_SOCKET_PATH: void 0,
                 WDS_SOCKET_PORT: void 0,
                 FAST_REFRESH: !0,
                 REACT_APP_LOCAL_URL: "/static"
             }).REACT_APP_SERVER_URL : "http://localhost:3000" === window.location.origin ? i.a.defaults.baseURL = "http://127.0.0.1:8000" : i.a.defaults.baseURL = window.location.origin, window.location.origin.endsWith("hf.space") && (i.a.defaults.baseURL = window.location.origin), i.a.defaults.baseURL = i.a.defaults.baseURL.split("+")[0], i.a.defaults.baseURL = i.a.defaults.baseURL.split("?")[0], i.a.defaults.baseURL = i.a.defaults.baseURL.split("#")[0], document.addEventListener("DOMContentLoaded", (function() {
                 return Object(o.render)(Object(E.jsxs)("div", {
-                    children: [Object(E.jsx)(Xn, {
-                        store: sa,
-                        history: aa
+                    children: [Object(E.jsx)(Zn, {
+                        store: ia,
+                        history: na
                     }), Object(E.jsx)(p.a, {
                         position: "top-right",
                         autoClose: 3e3,
                         hideProgressBar: !0,
                         newestOnTop: !0,
                         closeOnClick: !0,
                         pauseOnHover: !0
@@ -4235,8 +4212,8 @@
             }))
         }
     },
     [
         [294, 1, 2]
     ]
 ]);
-//# sourceMappingURL=main.51571475.chunk.js.map
+//# sourceMappingURL=main.71279c97.chunk.js.map
```

### Comparing `mercury-2.4.1/mercury/frontend-dist/static/js/main.51571475.chunk.js.map` & `mercury-2.4.2/mercury/frontend-dist/static/js/main.71279c97.chunk.js.map`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8427388217710797%*

 * *Differences: {"'file'": "'static/js/main.71279c97.chunk.js'",*

 * * "'mappings'": "'8QAKaA,EAAe,WAA2C,IAA1CC,EAAyC,wDAC9DC,EAAYC,eAAeC,QAAQ,aAKvC,OAJkB,OAAdF,IAAsC,IAAhBD,IACtBC,EAAYG,eACZF,eAAeG,QAAQ,YAAaJ,IAEjCA,GAGEK,EAAoB,SAACC,GACT,qBAAVA,GAAyBA,EAEhCC,IAAMC,SAASC,QAAQC,OAAvB,cAAiD,SAAWJ,SAGrDC,IAAMC,SAASC,QAAQC,OAAvB,eAIFC,EAAiB,SAACC,EAAaC,GACxCN,IACKO,IAAIF,EAAK,CACNG,aAAc,SAEjBC,MAAK,SAACC,GACHC,IAAaD,EAAIE,KAAMN,MAE1BO,OAAM,SAACC,GACJC,IAAMC,MAAN,uBAA4BV,EAA5B,kBCnBRW,EAAY,KACZC,aAAavB,QAAQ,WACvBsB,EAAYC,aAAavB,QAA […]*

```diff
@@ -1,10 +1,10 @@
 {
-    "file": "static/js/main.51571475.chunk.js",
-    "mappings": "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",
+    "file": "static/js/main.71279c97.chunk.js",
+    "mappings": "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",
     "names": [
         "getSessionId",
         "forceReload",
         "sessionId",
         "sessionStorage",
         "getItem",
         "uuidv4",
@@ -249,27 +249,25 @@
         "historicTask",
         "showCurrent",
         "previousTask",
         "exportingToPDF",
         "exportToPDFJobId",
         "exportToPDFCounter",
         "executionHistory",
-        "restTasks",
         "setShowCurrent",
         "setCurrentTask",
         "setHistoricTask",
         "setPreviousTask",
         "copyCurrentToPreviousTask",
         "setExportingToPDF",
         "setExportToPDFJobId",
         "resetExportToPDFCounter",
         "increaseExportToPDFCounter",
         "stopPDFExport",
         "setExecutionHistory",
-        "setRestTasks",
         "getCurrentTask",
         "tasks",
         "getHistoricTask",
         "getPreviousTask",
         "getExportingToPDF",
         "getExportToPDFJobId",
         "getExportToPDFCounter",
@@ -477,14 +475,15 @@
         "onopen",
         "onmessage",
         "onerror",
         "onclose",
         "Provider",
         "StatusBar",
         "allowDownload",
+        "allowShare",
         "waiting",
         "staticNotebook",
         "notebookId",
         "notebookPath",
         "notebookTitle",
         "runDownloadHTML",
         "runDownloadPDF",
@@ -523,15 +522,14 @@
         "showFiles",
         "isPresentation",
         "notebookParseErrors",
         "widgetsValues",
         "useContext",
         "execNb",
         "entries",
-        "listRestTasks",
         "widgetParams",
         "fileKeys",
         "widgetKeys",
         "parts",
         "sort",
         "b",
         "additionalStyle",
@@ -632,14 +630,16 @@
         "schedule",
         "created_at",
         "areOutputFilesAvailable",
         "errors",
         "continuous_update",
         "allow_download",
         "doAllowDownload",
+        "allow_share",
+        "doAllowShare",
         "full_screen",
         "isFullScreen",
         "MyApp",
         "useParams",
         "embed",
         "Footer",
         "bottom",
@@ -805,45 +805,45 @@
         "import React from \"react\";\nimport { Link } from \"react-router-dom\";\n\nexport default function LoginButton() {\n  return (\n    <div style={{ color: \"white\", padding: \"5px\", float: \"right\" }}>\n      <Link to=\"/login\" className=\"btn btn-primary btn-sm \">\n        <i className=\"fa fa-sign-in\" aria-hidden=\"true\"></i> Log in\n      </Link>\n    </div>\n  );\n}\n",
         "/* eslint-disable jsx-a11y/anchor-is-valid */\nimport React from \"react\";\nimport { useDispatch } from \"react-redux\";\nimport { Link, useNavigate } from \"react-router-dom\";\nimport { logout } from \"../slices/authSlice\";\n\ntype UserButtonProps = {\n  username: string;\n};\n\nexport default function UserButton({ username }: UserButtonProps) {\n  const dispatch = useDispatch();\n  const navigate = useNavigate();\n  return (\n    <div>\n      <div className=\"dropdown\" style={{ float: \"right\" }}>\n        <a\n          className=\"btn btn-secondary btn-sm dropdown-toggle\"\n          style={{ margin: \"5px\" }}\n          href=\"#\"\n          role=\"button\"\n          id=\"dropdownMenuLink\"\n          data-bs-toggle=\"dropdown\"\n          aria-expanded=\"false\"\n        >\n          {username}\n        </a>\n\n        <ul\n          className=\"dropdown-menu dropdown-menu-end\"\n          aria-labelledby=\"dropdownMenuLink\"\n        >\n          <li>\n            <Link className=\"dropdown-item\" to=\"/account\">\n              <i className=\"fa fa-user\" aria-hidden=\"true\"></i> Account\n            </Link>\n          </li>\n          <li>\n            <hr className=\"dropdown-divider\" />\n          </li>\n          <li>\n            <Link\n              to={\"/\"}\n              className=\"dropdown-item\"\n              onClick={() => dispatch(logout(navigate))}\n            >\n              <i className=\"fa fa-sign-out\" aria-hidden=\"true\"></i> Log out\n            </Link>\n          </li>\n        </ul>\n      </div>\n    </div>\n  );\n}\n",
         "/* eslint-disable jsx-a11y/anchor-is-valid */\nimport React from \"react\";\nimport { Link } from \"react-router-dom\";\nimport LoginButton from \"./LoginButton\";\nimport UserButton from \"./UserButton\";\n\ntype NavBarProps = {\n  isSitePublic: boolean;\n  username: string;\n  logoSrc: string;\n  navbarColor: string;\n};\n\nexport default function NavBar({\n  isSitePublic,\n  username,\n  logoSrc,\n  navbarColor,\n}: NavBarProps) {\n  \n  let headerBgClass = \"\";\n  let headerStyle = {};\n  if (navbarColor === \"\") {\n    headerBgClass = \"bg-dark\";\n  } else {\n    headerStyle = {\n      backgroundColor: navbarColor,\n    };\n  }\n\n  return (\n    <header\n      className={`navbar navbar-dark sticky-top ${headerBgClass} flex-md-nowrap p-0`}\n      style={headerStyle}\n    >\n      <Link className=\"navbar-brand col-md-3 col-lg-3 me-0 px-3\" to=\"/\">\n        {logoSrc !== \"\" && logoSrc !== \"loading\" && (\n          <img\n            alt=\"\"\n            src={logoSrc}\n            style={{ height: \"28px\", paddingLeft: \"10px\" }}\n          />\n        )}\n      </Link>\n\n      {!isSitePublic && username === \"\" && <LoginButton />}\n      {username !== \"\" && <UserButton username={username} />}\n    </header>\n  );\n}\n",
         "/* eslint-disable import/no-cycle */\r\nimport {\r\n  createSlice,\r\n  PayloadAction,\r\n  AnyAction,\r\n  Dispatch,\r\n} from '@reduxjs/toolkit';\r\nimport axios from 'axios';\r\n\r\nimport { RootState } from '../store';\r\nimport { getSessionId } from '../utils';\r\n\r\n\r\nconst initialState = {\r\n  view: \"app\",\r\n  files: [] as string[],\r\n  filesState: \"unknown\",\r\n  showSideBar: true,\r\n  storageType: \"media\",\r\n  showShareDialog: false,\r\n};\r\n\r\nconst appSlice = createSlice({\r\n  name: 'app',\r\n  initialState,\r\n  reducers: {\r\n    setView(state, action: PayloadAction<string>) {\r\n      state.view = action.payload;\r\n    },\r\n    setFilesState(state, action: PayloadAction<string>) {\r\n      state.filesState = action.payload;\r\n    },\r\n    setFiles(state, action: PayloadAction<string[]>) {\r\n      state.files = action.payload;\r\n    },\r\n    setShowSideBar(state, action: PayloadAction<boolean>) {\r\n      state.showSideBar = action.payload;\r\n    },\r\n    toggleShowSideBar(state) {\r\n      state.showSideBar = !state.showSideBar;\r\n    },\r\n    setStorageType(state, action: PayloadAction<string>) {\r\n      state.storageType = action.payload;\r\n    },\r\n    setShowShareDialog(state, action: PayloadAction<boolean>) {\r\n      state.showShareDialog = action.payload;\r\n    }\r\n  },\r\n});\r\n\r\nexport default appSlice.reducer;\r\n\r\nexport const {\r\n  setView,\r\n  setFilesState,\r\n  setFiles,\r\n  setShowSideBar,\r\n  toggleShowSideBar,\r\n  setStorageType,\r\n  setShowShareDialog,\r\n} = appSlice.actions;\r\n\r\n\r\nexport const getView = (state: RootState) => state.app.view;\r\nexport const getOutputFilesState = (state: RootState) => state.app.filesState;\r\nexport const getOutputFiles = (state: RootState) => state.app.files;\r\nexport const getShowSideBar = (state: RootState) => state.app.showSideBar;\r\nexport const getStorageType = (state: RootState) => state.app.storageType;\r\nexport const getShowShareDialog = (state: RootState) => state.app.showShareDialog;\r\n\r\n\r\nexport const fetchOutputFiles =\r\n  (taskId: number) =>\r\n    async (dispatch: Dispatch<AnyAction>) => {\r\n      try {\r\n        dispatch(setFilesState(\"loading\"))\r\n        dispatch(setFiles([]));\r\n        const sessionId = getSessionId();\r\n        const url = `/api/v1/output_files/${sessionId}/${taskId}/`;\r\n        const { data } = await axios.get(url);\r\n        dispatch(setFiles(data));\r\n        dispatch(setFilesState(\"loaded\"))\r\n      } catch (error) {\r\n        dispatch(setFilesState(\"error\"))\r\n        console.error(`Problem during loading output files. ${error}`);\r\n      }\r\n\r\n    };\r\n\r\nexport const fetchWorkerOutputFiles =\r\n  (workerId: number, notebookId: number) =>\r\n    async (dispatch: Dispatch<AnyAction>) => {\r\n      try {\r\n        dispatch(setFilesState(\"loading\"))\r\n        dispatch(setFiles([]));\r\n        const sessionId = getSessionId();\r\n        const url = `/api/v1/worker-output-files/${sessionId}/${workerId}/${notebookId}/`;\r\n        const { data } = await axios.get(url);\r\n        dispatch(setFiles(data));\r\n        dispatch(setFilesState(\"loaded\"))\r\n      } catch (error) {\r\n        dispatch(setFilesState(\"error\"))\r\n        console.error(`Problem during loading worker output files. ${error}`);\r\n      }\r\n\r\n    };\r\n\r\n\r\nexport const fetchStorageType =\r\n  () =>\r\n    async (dispatch: Dispatch<AnyAction>) => {\r\n      try {\r\n        const url = `/api/v1/storage-type`;\r\n        const { data } = await axios.get(url);\r\n        dispatch(setStorageType(data.storage_type));\r\n\r\n      } catch (error) {\r\n        console.error(`Get storage type error. ${error}`);\r\n      }\r\n\r\n    };\r\n\r\nexport const userFileUploaded =\r\n  (siteId: number, sessionId: string, filename: string) =>\r\n    async (dispatch: Dispatch<AnyAction>) => {\r\n      try {\r\n        const data = { site_id: siteId, session_id: sessionId, filename }\r\n        const url = `/api/v1/nb-file-uploaded`;\r\n        await axios.post(url, data);\r\n      } catch (error) {\r\n        console.error(`Problem with file upload. ${error}`);\r\n      }\r\n    };\r\n\r\n\r\nexport const deleteUserFileUploaded =\r\n  (siteId: number, sessionId: string, filename: string) =>\r\n    async (dispatch: Dispatch<AnyAction>) => {\r\n      try {\r\n        const data = { site_id: siteId, session_id: sessionId, filename }\r\n        const url = `/api/v1/nb-delete-file`;\r\n        await axios.post(url, data);\r\n      } catch (error) {\r\n        console.error(`Problem with file upload. ${error}`);\r\n      }\r\n    };",
         "export interface ISelectWidget {\n  label: string | null;\n  value: string | null;\n  input: string;\n  choices: string[];\n  multi: boolean | undefined;\n  url_key: string;\n  disabled: boolean;\n  hidden: boolean;\n}\n\nexport interface ICheckboxWidget {\n  label: string | null;\n  value: boolean | null;\n  input: string;\n  url_key: string;\n  disabled: boolean;\n  hidden: boolean;\n}\n\nexport interface INumericWidget {\n  label: string | null;\n  value: number | null;\n  input: string;\n  min: number;\n  max: number;\n  step: number;\n  url_key: string;\n  disabled: boolean;\n  hidden: boolean;\n}\n\nexport interface ISliderWidget {\n  vertical: boolean | null;\n  label: string | null;\n  value: number | null;\n  input: string;\n  min: number | null;\n  max: number | null;\n  step: number | null;\n  url_key: string;\n  urlValue: number | null;\n  disabled: boolean;\n  hidden: boolean;\n}\n\nexport interface IRangeWidget {\n  vertical: boolean | null;\n  label: string | null;\n  value: [number, number] | null;\n  input: string;\n  min: number | null;\n  max: number | null;\n  step: number | null;\n  url_key: string;\n  disabled: boolean;\n  hidden: boolean;\n}\n\nexport interface IFileWidget {\n  label: string | null;\n  value: string | null;\n  input: string;\n  maxFileSize: string | null;\n  disabled: boolean;\n  hidden: boolean;\n}\n\nexport interface ITextWidget {\n  label: string | null;\n  value: string | undefined;\n  input: string;\n  rows: number | null;\n  url_key: string;\n  disabled: boolean;\n  hidden: boolean;\n  sanitize: boolean;\n}\n\nexport interface IOutputFilesWidget {\n  output: string;\n  input: null;\n  value: null;\n}\n\nexport interface IMarkdownWidget {\n  output: string;\n  input: null;  // we need to add input to be IWidget\n  value: string;\n}\n\nexport interface IButtonWidget {\n  label: string | null;\n  style: string;\n  input: string;\n  value: string | boolean | null;\n  disabled: boolean;\n  hidden: boolean;\n}\n\nexport interface IAPIResponseWidget {\n  output: string\n  input: null;\n  value: string;\n}\n\n\nexport type IWidget =\n  | ISelectWidget\n  | ICheckboxWidget\n  | INumericWidget\n  | ISliderWidget\n  | IRangeWidget\n  | IFileWidget\n  | ITextWidget\n  | IOutputFilesWidget\n  | IMarkdownWidget\n  | IButtonWidget\n  | IAPIResponseWidget;\n\nexport function isSelectWidget(widget: IWidget): widget is ISelectWidget {\n  return (widget as ISelectWidget).input === \"select\";\n}\n\nexport function isCheckboxWidget(widget: IWidget): widget is ICheckboxWidget {\n  return (widget as ICheckboxWidget).input === \"checkbox\";\n}\n\nexport function isNumericWidget(widget: IWidget): widget is INumericWidget {\n  return (widget as INumericWidget).input === \"numeric\";\n}\n\nexport function isSliderWidget(widget: IWidget): widget is ISliderWidget {\n  return (widget as ISliderWidget).input === \"slider\";\n}\n\nexport function isRangeWidget(widget: IWidget): widget is IRangeWidget {\n  return (widget as IRangeWidget).input === \"range\";\n}\n\nexport function isFileWidget(widget: IWidget): widget is IFileWidget {\n  return (widget as IFileWidget).input === \"file\";\n}\n\nexport function isTextWidget(widget: IWidget): widget is ITextWidget {\n  return (widget as ITextWidget).input === \"text\";\n}\n\nexport function isOutputFilesWidget(widget: IWidget): widget is IOutputFilesWidget {\n  return (widget as IOutputFilesWidget).output === \"dir\";\n}\n\nexport function isMarkdownWidget(widget: IWidget): widget is IMarkdownWidget {\n  return (widget as IMarkdownWidget).output === \"markdown\";\n}\n\nexport function isButtonWidget(widget: IWidget): widget is IButtonWidget {\n  return (widget as IButtonWidget).input === \"button\";\n}\n\nexport function isAPIResponseWidget(widget: IWidget): widget is IAPIResponseWidget {\n  return (widget as IAPIResponseWidget).output === \"apiresponse\";\n}\n",
         "// code from https://stackoverflow.com/questions/36862334/get-viewport-window-height-in-reactjs\nimport { useState, useEffect } from \"react\";\n\nexport function getWindowDimensions() {\n  const { innerWidth: width, innerHeight: height } = window;\n  return {\n    width,\n    height,\n  };\n}\n\nexport default function useWindowDimensions() {\n  const [windowDimensions, setWindowDimensions] = useState(\n    getWindowDimensions()\n  );\n\n  useEffect(() => {\n    function handleResize() {\n      setWindowDimensions(getWindowDimensions());\n    }\n\n    window.addEventListener(\"resize\", handleResize);\n    return () => window.removeEventListener(\"resize\", handleResize);\n  }, []);\n\n  return windowDimensions;\n}\n",
         "/* eslint-disable import/no-cycle */\r\nimport {\r\n  createSlice,\r\n  PayloadAction,\r\n  AnyAction,\r\n  Dispatch,\r\n} from \"@reduxjs/toolkit\";\r\nimport axios, { AxiosError } from \"axios\";\r\n\r\nimport { RootState } from \"../store\";\r\nimport { setToken, setUsername } from \"./authSlice\";\r\n\r\n\r\nexport const SITE_PUBLIC = \"PUBLIC\";\r\nexport const SITE_PRIVATE = \"PRIVATE\";\r\n\r\nexport interface Site {\r\n  id: number;\r\n  title: string;\r\n  slug: string;\r\n  share: string;\r\n  welcome: string;\r\n  active: boolean;\r\n  version: string;\r\n  created_at: Date;\r\n  updated_at: Date;\r\n  created_by: number;\r\n  info: string;\r\n}\r\n\r\nexport enum SiteStatus {\r\n  Unknown = \"Unknown\",\r\n  Loaded = \"Loaded\",\r\n  NotFound = \"Not found\",\r\n  AccessForbidden = \"Access forbidden\",\r\n  NetworkError = \"Network Error\",\r\n  PleaseRefresh = \"Please refresh\",\r\n  LostConnection = \"Lost connection\",\r\n  NotReady = \"Not Ready\",\r\n  NotebookNotFound = \"Notebook not found\",\r\n}\r\n\r\nconst initialState = {\r\n  site: {} as Site,\r\n  siteStatus: SiteStatus.Unknown,\r\n};\r\n\r\nconst sitesSlice = createSlice({\r\n  name: \"sites\",\r\n  initialState,\r\n  reducers: {\r\n    setSite(state, action: PayloadAction<Site>) {\r\n      state.site = action.payload;\r\n    },\r\n    setSiteStatus(state, action: PayloadAction<SiteStatus>) {\r\n      state.siteStatus = action.payload;\r\n    }\r\n  },\r\n});\r\n\r\nexport default sitesSlice.reducer;\r\n\r\nexport const { setSite, setSiteStatus } = sitesSlice.actions;\r\n\r\nexport const getSite = (state: RootState) => state.sites.site;\r\nexport const getSiteStatus = (state: RootState) => state.sites.siteStatus;\r\nexport const getSiteId = (state: RootState) => state.sites.site.id;\r\nexport const getSiteWelcome = (state: RootState) => state.sites.site.welcome;\r\nexport const isPublic = (state: RootState) => {\r\n  return state.sites.site.share === SITE_PUBLIC;\r\n};\r\n\r\nexport const getLogoFilename = (state: RootState) => {\r\n  if (state.sites.site.info === undefined || state.sites.site.info === \"\") {\r\n    return \"\";\r\n  }\r\n  const info = JSON.parse(state.sites.site.info);\r\n  if(info?.logoFilename === undefined) {\r\n    return \"\";\r\n  }\r\n  return info?.logoFilename\r\n};\r\nexport const getNavbarColor = (state: RootState) => {\r\n  if (state.sites.site.info === undefined || state.sites.site.info === \"\") {\r\n    return \"\";\r\n  }\r\n  const info = JSON.parse(state.sites.site.info);\r\n  if(info?.navbarColor === undefined) {\r\n    return \"\";\r\n  }\r\n  return info?.navbarColor;\r\n};\r\nexport const getFooterText = (state: RootState) => {\r\n  if (state.sites.site.info === undefined || state.sites.site.info === \"\") {\r\n    return \"\";\r\n  }\r\n  const info = JSON.parse(state.sites.site.info);\r\n  if(info?.footerText === undefined) {\r\n    return \"\";\r\n  }\r\n  return info?.footerText;\r\n};\r\n\r\n\r\nexport const fetchSite = () => async (dispatch: Dispatch<AnyAction>) => {\r\n  try {\r\n    dispatch(setSite({} as Site));\r\n    dispatch(setSiteStatus(SiteStatus.Unknown));\r\n\r\n    let siteSlug = \"single-site\";\r\n    if (process.env.REACT_APP_SERVER_URL) {\r\n      siteSlug = window.location.host.split(':')[0]\r\n    }\r\n    if (window.location.origin.endsWith(\"hf.space\")) {\r\n      siteSlug = \"localhost\";\r\n    }\r\n\r\n    const url = `/api/v1/get-site/${siteSlug}/`;\r\n    const { data } = await axios.get(url);\r\n\r\n    dispatch(setSite(data as Site));\r\n    if (data?.status !== \"Ready\") {\r\n      dispatch(setSiteStatus(SiteStatus.NotReady));\r\n    } else {\r\n      dispatch(setSiteStatus(SiteStatus.Loaded));\r\n    }\r\n  } catch (error) {\r\n    const err = error as AxiosError;\r\n    console.log(err.message)\r\n    if (err?.message === \"Network Error\") {\r\n      dispatch(setSiteStatus(SiteStatus.NetworkError));\r\n    } else if (err.response!.status === 403) {\r\n      dispatch(setSiteStatus(SiteStatus.AccessForbidden));\r\n    } else if (err.response!.status === 404) {\r\n      dispatch(setSiteStatus(SiteStatus.NotFound));\r\n    } else if (err.response!.status === 401) {\r\n      // invalid token, clear token ...\r\n      dispatch(setToken(\"\"));\r\n      dispatch(setUsername(\"\"));\r\n      dispatch(setSiteStatus(SiteStatus.PleaseRefresh));\r\n    } else {\r\n      console.error(`Problem during loading site information. ${error}`);\r\n    }\r\n  }\r\n};\r\n",
-        "/* eslint-disable import/no-cycle */\r\nimport {\r\n  createSlice,\r\n  PayloadAction,\r\n  AnyAction,\r\n  Dispatch,\r\n} from \"@reduxjs/toolkit\";\r\nimport axios, { AxiosError } from \"axios\";\r\n\r\nimport { RootState } from \"../store\";\r\nimport { clearExecutionHistory } from \"./tasksSlice\";\r\nimport { setShowSideBar } from \"./appSlice\";\r\nimport {\r\n  IWidget,\r\n  isSelectWidget,\r\n  isSliderWidget,\r\n  isTextWidget,\r\n  isRangeWidget,\r\n  isCheckboxWidget,\r\n  isNumericWidget,\r\n  isMarkdownWidget,\r\n  isButtonWidget,\r\n  isFileWidget,\r\n} from \"../widgets/Types\";\r\nimport { getWindowDimensions } from \"../components/WindowDimensions\";\r\nimport { setSiteStatus, SiteStatus } from \"./sitesSlice\";\r\n\r\nexport const RUN_DELAY = 600; // ms\r\nexport const RUN_DELAY_FAST = 100; // ms\r\n\r\nexport interface INotebookParams {\r\n  title: string | null;\r\n  description: string | null;\r\n  date: string | null;\r\n  author: string | null;\r\n  \"show-code\": boolean | null;\r\n  params: Record<string, IWidget>; //IWidget[];\r\n  version: string;\r\n  continuous_update: boolean;\r\n  static_notebook: boolean;\r\n  show_sidebar: boolean;\r\n  full_screen: boolean;\r\n  allow_download: boolean;\r\n}\r\n\r\nexport interface INotebook {\r\n  id: number;\r\n  created_at: Date;\r\n  file_updated_at: Date;\r\n  title: string;\r\n  slug: string;\r\n  path: string;\r\n  share: string;\r\n  params: INotebookParams;\r\n  state: string;\r\n  default_view_path: string;\r\n  output: string;\r\n  format: string;\r\n  slidesHash: string;\r\n  schedule: string;\r\n  errors: string;\r\n}\r\n\r\nexport type WidgetValueType =\r\n  | string\r\n  | boolean\r\n  | number\r\n  | [number, number]\r\n  | string[]\r\n  | null\r\n  | undefined\r\n  | unknown;\r\n\r\nconst initialState = {\r\n  notebooks: [] as INotebook[],\r\n  loadingState: \"loading\",\r\n  selectedNotebook: {} as INotebook,\r\n  selectedNotebookId: undefined as undefined | number,\r\n  loadingStateSelected: \"loading\",\r\n  watchModeCounter: 0,\r\n  slidesHash: \"\",\r\n  widgets: {} as Record<string, WidgetValueType>,\r\n  widgetsUrlValues: {} as Record<string, WidgetValueType>,\r\n  nbIframes: {} as Record<string, string>, // slug -> signed URL\r\n  widgetsInitialized: false,\r\n  urlValuesUsed: false,\r\n};\r\n\r\nconst notebooksSlice = createSlice({\r\n  name: \"notebooks\",\r\n  initialState,\r\n  reducers: {\r\n    setWidgetValue(\r\n      state,\r\n      action: PayloadAction<{ key: string; value: WidgetValueType }>\r\n    ) {\r\n      const { key, value } = action.payload;\r\n      state.widgets[key] = value;\r\n      //console.log({ key, value });\r\n    },\r\n    setWidgetUrlValue(\r\n      state,\r\n      action: PayloadAction<{ key: string; value: WidgetValueType }>\r\n    ) {\r\n      const { key, value } = action.payload;\r\n      state.widgetsUrlValues[key] = value;\r\n    },\r\n    clearWidgets(state) {\r\n      state.widgets = {};\r\n    },\r\n    clearWidgetsUrlValues(state) {\r\n      state.widgetsUrlValues = {};\r\n    },\r\n    setNotebooks(state, action: PayloadAction<INotebook[]>) {\r\n      state.notebooks = action.payload;\r\n    },\r\n    setLoadingState(state, action: PayloadAction<string>) {\r\n      state.loadingState = action.payload;\r\n    },\r\n    setSelectedNotebook(state, action: PayloadAction<INotebook>) {\r\n      if (\r\n        action.payload.state.startsWith(\"WATCH\") &&\r\n        state.selectedNotebook.file_updated_at ===\r\n        action.payload.file_updated_at\r\n      ) {\r\n        // console.log(\"skip notebook update\")\r\n      } else {\r\n        state.selectedNotebook = action.payload;\r\n        state.selectedNotebookId = state.selectedNotebook.id;\r\n      }\r\n      if (action.payload.state.startsWith(\"WATCH\")) {\r\n        state.watchModeCounter += 1;\r\n      }\r\n    },\r\n    setLoadingStateSelected(state, action: PayloadAction<string>) {\r\n      state.loadingStateSelected = action.payload;\r\n    },\r\n    setSlidesHash(state, action: PayloadAction<string>) {\r\n      state.slidesHash = action.payload;\r\n    },\r\n    updateWidgetsParams(state, action: PayloadAction<any>) {\r\n      const { widgetKey } = action.payload;\r\n\r\n      let updated = false;\r\n\r\n      let noMatch = true;\r\n\r\n      for (let key of Object.keys(state.selectedNotebook.params.params)) {\r\n        if (key === widgetKey) {\r\n          noMatch = false;\r\n          let widget = { ...state.selectedNotebook.params.params[widgetKey] };\r\n\r\n          if (isRangeWidget(widget)) {\r\n            if (widget.disabled !== action.payload.disabled) {\r\n              widget.disabled = action.payload.disabled;\r\n              state.widgets[key] = action.payload.value;\r\n              updated = true;\r\n            }\r\n            if (widget.hidden !== action.payload.hidden) {\r\n              widget.hidden = action.payload.hidden;\r\n              state.widgets[key] = action.payload.value;\r\n              updated = true;\r\n            }\r\n            if (widget.min !== action.payload.min) {\r\n              widget.min = action.payload.min;\r\n              state.widgets[key] = action.payload.value;\r\n              updated = true;\r\n            }\r\n            if (widget.max !== action.payload.max) {\r\n              widget.max = action.payload.max;\r\n              state.widgets[key] = action.payload.value;\r\n              updated = true;\r\n            }\r\n            if (widget.step !== action.payload.step) {\r\n              widget.step = action.payload.step;\r\n              state.widgets[key] = action.payload.value;\r\n              updated = true;\r\n            }\r\n            if (widget.label !== action.payload.label) {\r\n              widget.label = action.payload.label;\r\n              updated = true;\r\n            }\r\n          } else if (isTextWidget(widget)) {\r\n            if (widget.disabled !== action.payload.disabled) {\r\n              widget.disabled = action.payload.disabled;\r\n              state.widgets[key] = action.payload.value;\r\n              updated = true;\r\n            }\r\n            if (widget.hidden !== action.payload.hidden) {\r\n              widget.hidden = action.payload.hidden;\r\n              state.widgets[key] = action.payload.value;\r\n              updated = true;\r\n            }\r\n            if (widget.rows !== action.payload.rows) {\r\n              widget.rows = action.payload.rows;\r\n              updated = true;\r\n            }\r\n            if (widget.label !== action.payload.label) {\r\n              widget.label = action.payload.label;\r\n              updated = true;\r\n            }\r\n          } else if (isSliderWidget(widget)) {\r\n            if (widget.disabled !== action.payload.disabled) {\r\n              widget.disabled = action.payload.disabled;\r\n              state.widgets[key] = action.payload.value;\r\n              updated = true;\r\n            }\r\n            if (widget.hidden !== action.payload.hidden) {\r\n              widget.hidden = action.payload.hidden;\r\n              state.widgets[key] = action.payload.value;\r\n              updated = true;\r\n            }\r\n            if (widget.min !== action.payload.min) {\r\n              widget.min = action.payload.min;\r\n              state.widgets[key] = action.payload.value;\r\n              updated = true;\r\n            }\r\n            if (widget.max !== action.payload.max) {\r\n              widget.max = action.payload.max;\r\n              state.widgets[key] = action.payload.value;\r\n              updated = true;\r\n            }\r\n            if (widget.step !== action.payload.step) {\r\n              widget.step = action.payload.step;\r\n              state.widgets[key] = action.payload.value;\r\n              updated = true;\r\n            }\r\n            if (widget.label !== action.payload.label) {\r\n              widget.label = action.payload.label;\r\n              updated = true;\r\n            }\r\n          } else if (isSelectWidget(widget)) {\r\n            if (widget.disabled !== action.payload.disabled) {\r\n              widget.disabled = action.payload.disabled;\r\n              state.widgets[key] = action.payload.value;\r\n              updated = true;\r\n            }\r\n            if (widget.hidden !== action.payload.hidden) {\r\n              widget.hidden = action.payload.hidden;\r\n              state.widgets[key] = action.payload.value;\r\n              updated = true;\r\n            }\r\n            if (\r\n              widget.choices.toString() !== action.payload.choices.toString()\r\n            ) {\r\n              widget.choices = action.payload.choices;\r\n              state.widgets[key] = action.payload.value;\r\n              updated = true;\r\n            }\r\n            if (widget.label !== action.payload.label) {\r\n              widget.label = action.payload.label;\r\n              updated = true;\r\n            }\r\n          } else if (isCheckboxWidget(widget)) {\r\n            if (widget.disabled !== action.payload.disabled) {\r\n              widget.disabled = action.payload.disabled;\r\n              state.widgets[key] = action.payload.value;\r\n              updated = true;\r\n            }\r\n            if (widget.hidden !== action.payload.hidden) {\r\n              widget.hidden = action.payload.hidden;\r\n              state.widgets[key] = action.payload.value;\r\n              updated = true;\r\n            }\r\n            if (widget.label !== action.payload.label) {\r\n              widget.label = action.payload.label;\r\n              updated = true;\r\n            }\r\n          } else if (isNumericWidget(widget)) {\r\n            if (widget.disabled !== action.payload.disabled) {\r\n              widget.disabled = action.payload.disabled;\r\n              state.widgets[key] = action.payload.value;\r\n              updated = true;\r\n            }\r\n            if (widget.hidden !== action.payload.hidden) {\r\n              widget.hidden = action.payload.hidden;\r\n              state.widgets[key] = action.payload.value;\r\n              updated = true;\r\n            }\r\n            if (widget.min !== action.payload.min) {\r\n              widget.min = action.payload.min;\r\n              state.widgets[key] = action.payload.value;\r\n              updated = true;\r\n            }\r\n            if (widget.max !== action.payload.max) {\r\n              widget.max = action.payload.max;\r\n              state.widgets[key] = action.payload.value;\r\n              updated = true;\r\n            }\r\n            if (widget.step !== action.payload.step) {\r\n              widget.step = action.payload.step;\r\n              state.widgets[key] = action.payload.value;\r\n              updated = true;\r\n            }\r\n            if (widget.label !== action.payload.label) {\r\n              widget.label = action.payload.label;\r\n              updated = true;\r\n            }\r\n          } else if (isMarkdownWidget(widget)) {\r\n            if (widget.value !== action.payload.value) {\r\n              widget.value = action.payload.value;\r\n              updated = true;\r\n            }\r\n          } else if (isButtonWidget(widget)) {\r\n            state.widgets[key] = action.payload.value;\r\n            if (widget.disabled !== action.payload.disabled) {\r\n              widget.disabled = action.payload.disabled;\r\n              state.widgets[key] = action.payload.value;\r\n              updated = true;\r\n            }\r\n            if (widget.hidden !== action.payload.hidden) {\r\n              widget.hidden = action.payload.hidden;\r\n              state.widgets[key] = action.payload.value;\r\n              updated = true;\r\n            }\r\n            if (widget.label !== action.payload.label) {\r\n              widget.label = action.payload.label;\r\n              updated = true;\r\n            }\r\n            if (widget.style !== action.payload.style) {\r\n              widget.style = action.payload.style;\r\n              updated = true;\r\n            }\r\n          } else if (isFileWidget(widget)) {\r\n            state.widgets[key] = action.payload.value;\r\n            if (widget.disabled !== action.payload.disabled) {\r\n              widget.disabled = action.payload.disabled;\r\n              state.widgets[key] = action.payload.value;\r\n              updated = true;\r\n            }\r\n            if (widget.hidden !== action.payload.hidden) {\r\n              widget.hidden = action.payload.hidden;\r\n              state.widgets[key] = action.payload.value;\r\n              updated = true;\r\n            }\r\n            if (widget.label !== action.payload.label) {\r\n              widget.label = action.payload.label;\r\n              updated = true;\r\n            }\r\n          }\r\n\r\n          if (updated) {\r\n            state.selectedNotebook.params.params[widgetKey] = widget;\r\n          }\r\n        }\r\n      }\r\n      if (noMatch) {\r\n        state.selectedNotebook.params.params[widgetKey] = action.payload;\r\n      }\r\n    },\r\n    hideWidgets(state, action: PayloadAction<any>) {\r\n      const { keys } = action.payload;\r\n      for (let key of keys) {\r\n        if (key in state.selectedNotebook.params.params) {\r\n          delete state.selectedNotebook.params.params[key];\r\n        }\r\n      }\r\n    },\r\n    initWidgets(state, action: PayloadAction<any>) {\r\n      const { widgets } = action.payload;\r\n      state.selectedNotebook.params.params = {}\r\n      state.widgets = {}\r\n      for (let widget of widgets) {\r\n        state.selectedNotebook.params.params[widget.widgetKey] = widget;\r\n        state.widgets[widget.widgetKey] = widget.value;\r\n      }\r\n    },\r\n    updateTitle(state, action: PayloadAction<string>) {\r\n      state.selectedNotebook.title = action.payload;\r\n    },\r\n    updateShowCode(state, action: PayloadAction<boolean>) {\r\n      state.selectedNotebook.params[\"show-code\"] = action.payload;\r\n    },\r\n    setNbIframes(state, action: PayloadAction<Record<string, string>>) {\r\n      state.nbIframes = action.payload;\r\n    },\r\n    setWidgetsInitialized(state, action: PayloadAction<boolean>) {\r\n      state.widgetsInitialized = action.payload;\r\n    },\r\n    setUrlValuesUsed(state, action: PayloadAction<boolean>) {\r\n      state.urlValuesUsed = action.payload;\r\n    }\r\n  },\r\n});\r\n\r\nexport default notebooksSlice.reducer;\r\n\r\nexport const {\r\n  setNotebooks,\r\n  setLoadingState,\r\n  setSelectedNotebook,\r\n  setLoadingStateSelected,\r\n  setSlidesHash,\r\n  updateWidgetsParams,\r\n  hideWidgets,\r\n  setWidgetValue,\r\n  setWidgetUrlValue,\r\n  clearWidgets,\r\n  clearWidgetsUrlValues,\r\n  initWidgets,\r\n  updateTitle,\r\n  updateShowCode,\r\n  setNbIframes,\r\n  setWidgetsInitialized,\r\n  setUrlValuesUsed\r\n} = notebooksSlice.actions;\r\n\r\nexport const getNotebooks = (state: RootState) => state.notebooks.notebooks;\r\nexport const getLoadingState = (state: RootState) =>\r\n  state.notebooks.loadingState;\r\nexport const getSelectedNotebook = (state: RootState) =>\r\n  state.notebooks.selectedNotebook;\r\nexport const getSelectedNotebookId = (state: RootState) =>\r\n  state.notebooks.selectedNotebookId;\r\nexport const isStaticNotebook = (state: RootState) => {\r\n  let st = state.notebooks.selectedNotebook?.params?.static_notebook;\r\n  if (st === undefined) {\r\n    return false;\r\n  }\r\n  return st;\r\n};\r\nexport const getLoadingStateSelected = (state: RootState) =>\r\n  state.notebooks.loadingStateSelected;\r\nexport const getWatchModeCounter = (state: RootState) =>\r\n  state.notebooks.watchModeCounter;\r\nexport const getSlidesHash = (state: RootState) => state.notebooks.slidesHash;\r\n\r\nexport const getWidgetsValues = (state: RootState): Record<string, WidgetValueType> => state.notebooks.widgets;\r\nexport const getWidgetsUrlValues = (state: RootState): Record<string, WidgetValueType> => state.notebooks.widgetsUrlValues;\r\n\r\n\r\nexport const getNbIframes = (state: RootState) => state.notebooks.nbIframes;\r\nexport const getWidgetsInitialized = (state: RootState) => state.notebooks.widgetsInitialized;\r\nexport const getUrlValuesUsed = (state: RootState) => state.notebooks.urlValuesUsed;\r\n\r\nexport const fetchNbIframes = (siteId: number) => async (dispatch: Dispatch<AnyAction>) => {\r\n  try {\r\n    const url = `/api/v1/${siteId}/nb-iframes/`;\r\n    const { data } = await axios.get(url);\r\n    dispatch(setNbIframes(data));\r\n  } catch (error) {\r\n    console.error(`Problem during loading notebooks iframes. ${error}`);\r\n  }\r\n};\r\n\r\n\r\nexport const fetchNotebooks = (siteId: number) => async (dispatch: Dispatch<AnyAction>) => {\r\n  try {\r\n    dispatch(setSlidesHash(\"\"));\r\n    dispatch(setLoadingState(\"loading\"));\r\n    dispatch(clearExecutionHistory());\r\n    const url = `/api/v1/${siteId}/notebooks/`;\r\n    const { data } = await axios.get(url);\r\n    const parsedNotebooks = data.map((notebook: any) => {\r\n      const parsedParams = JSON.parse(notebook.params);\r\n\r\n      return {\r\n        ...notebook,\r\n        params: parsedParams as INotebookParams,\r\n      };\r\n    });\r\n    dispatch(setNotebooks(parsedNotebooks));\r\n    dispatch(setLoadingState(\"loaded\"));\r\n  } catch (error) {\r\n    dispatch(setLoadingState(\"error\"));\r\n    console.error(`Problem during loading recent notebooks. ${error}`);\r\n  }\r\n};\r\n\r\nexport const fetchNotebook =\r\n  (siteId: number, id: number, silent = false) =>\r\n    async (dispatch: Dispatch<AnyAction>) => {\r\n      try {\r\n        if (!silent) {\r\n          dispatch(setSlidesHash(\"\"));\r\n          dispatch(clearExecutionHistory());\r\n        }\r\n\r\n        const { width } = getWindowDimensions();\r\n        dispatch(setShowSideBar(width > 992));\r\n\r\n        if (!silent) {\r\n          dispatch(setLoadingStateSelected(\"loading\"));\r\n        }\r\n        const url = `/api/v1/${siteId}/notebooks/${id}/`;\r\n        const { data } = await axios.get(url);\r\n        const parsedParams = JSON.parse(data.params) as INotebookParams;\r\n        dispatch(\r\n          setSelectedNotebook({\r\n            ...data,\r\n            params: parsedParams,\r\n          })\r\n        );\r\n        if (!silent) {\r\n          dispatch(setLoadingStateSelected(\"loaded\"));\r\n        }\r\n        if (parsedParams?.show_sidebar !== null && parsedParams?.show_sidebar !== undefined) {\r\n          dispatch(setShowSideBar(parsedParams?.show_sidebar));\r\n        }\r\n      } catch (error) {\r\n        if (!silent) {\r\n          dispatch(setLoadingStateSelected(\"error\"));\r\n        }\r\n        console.error(\r\n          `Problem during loading selected notebook (${id}). ${error}`\r\n        );\r\n      }\r\n    };\r\n\r\nexport const fetchNotebookWithSlug =\r\n  (siteId: number, slug: string, silent = false) =>\r\n    async (dispatch: Dispatch<AnyAction>) => {\r\n      try {\r\n        if (!silent) {\r\n          dispatch(setSlidesHash(\"\"));\r\n          dispatch(clearExecutionHistory());\r\n        }\r\n\r\n        const { width } = getWindowDimensions();\r\n        dispatch(setShowSideBar(width > 992));\r\n\r\n        if (!silent) {\r\n          dispatch(setLoadingStateSelected(\"loading\"));\r\n        }\r\n        const url = `/api/v1/${siteId}/getnb/${slug}/`;\r\n        const { data } = await axios.get(url);\r\n        const parsedParams = JSON.parse(data.params) as INotebookParams;\r\n        dispatch(\r\n          setSelectedNotebook({\r\n            ...data,\r\n            params: parsedParams,\r\n          })\r\n        );\r\n        if (!silent) {\r\n          dispatch(setLoadingStateSelected(\"loaded\"));\r\n        }\r\n        if (parsedParams?.show_sidebar !== null && parsedParams?.show_sidebar !== undefined) {\r\n          dispatch(setShowSideBar(parsedParams?.show_sidebar));\r\n        }\r\n      } catch (error) {\r\n        const err = error as AxiosError;\r\n\r\n        if (!silent) {\r\n          dispatch(setLoadingStateSelected(\"error\"));\r\n\r\n          if (err.response?.status === 404) {\r\n            // switch to notebook not found view\r\n            dispatch(setSiteStatus(SiteStatus.NotebookNotFound))\r\n          }\r\n        }\r\n        console.error(\r\n          `Problem during loading selected notebook (${slug}). ${error}`\r\n        );\r\n\r\n\r\n      }\r\n    };\r\n",
-        "/* eslint-disable import/no-cycle */\r\nimport {\r\n    createSlice,\r\n    AnyAction,\r\n    Dispatch,\r\n    PayloadAction,\r\n} from '@reduxjs/toolkit';\r\nimport axios from 'axios';\r\nimport { RootState } from '../store';\r\nimport { toast } from \"react-toastify\";\r\nimport { getSessionId, handleDownload } from '../utils';\r\nimport { setSlidesHash } from './notebooksSlice';\r\n\r\nexport interface ITask {\r\n    id: number;\r\n    task_id: string;\r\n    session_id: string;\r\n    created_at: Date;\r\n    state: \"CREATED\" | \"RECEIVED\" | \"DONE\" | \"ERROR\";\r\n    params: string;\r\n    result: string;\r\n}\r\n\r\nexport interface IRestTask {\r\n    id: number;\r\n    state: \"CREATED\" | \"RECEIVED\" | \"DONE\" | \"ERROR\";\r\n    params: string;\r\n    response: string;\r\n    session_id: string;\r\n    created_at: Date;\r\n    updated_at: Date;\r\n}\r\n\r\nconst initialState = {\r\n    currentTask: {} as ITask,\r\n    historicTask: {} as ITask,\r\n    showCurrent: true,\r\n    previousTask: {} as ITask,\r\n    exportingToPDF: false,\r\n    exportToPDFJobId: '',\r\n    exportToPDFCounter: 0,\r\n    executionHistory: [] as ITask[],\r\n    restTasks: [] as IRestTask[],\r\n};\r\n\r\nconst tasksSlice = createSlice({\r\n    name: 'tasks',\r\n    initialState,\r\n    reducers: {\r\n        setShowCurrent(state, action: PayloadAction<boolean>) {\r\n            state.showCurrent = action.payload;\r\n        },\r\n        setCurrentTask(state, action: PayloadAction<ITask>) {\r\n            state.currentTask = action.payload;\r\n        },\r\n        setHistoricTask(state, action: PayloadAction<ITask>) {\r\n            state.historicTask = action.payload;\r\n        },\r\n        setPreviousTask(state, action: PayloadAction<ITask>) {\r\n            state.previousTask = action.payload;\r\n        },\r\n        copyCurrentToPreviousTask(state) {\r\n            state.previousTask = state.currentTask;\r\n        },\r\n        setExportingToPDF(state, action: PayloadAction<boolean>) {\r\n            state.exportingToPDF = action.payload;\r\n        },\r\n        setExportToPDFJobId(state, action: PayloadAction<string>) {\r\n            state.exportToPDFJobId = action.payload;\r\n        },\r\n        resetExportToPDFCounter(state) {\r\n            state.exportToPDFCounter = 0;\r\n        },\r\n        increaseExportToPDFCounter(state) {\r\n            state.exportToPDFCounter += 1;\r\n        },\r\n        stopPDFExport(state) {\r\n            state.exportingToPDF = false;\r\n            state.exportToPDFJobId = \"\";\r\n            state.exportToPDFCounter = 0;\r\n        },\r\n        setExecutionHistory(state, action: PayloadAction<ITask[]>) {\r\n            state.executionHistory = action.payload;\r\n        },\r\n        clearExecutionHistory(state) {\r\n            state.executionHistory = [];\r\n        },\r\n        setRestTasks(state, action: PayloadAction<IRestTask[]>) {\r\n            state.restTasks = action.payload;\r\n        }\r\n    },\r\n});\r\n\r\nexport default tasksSlice.reducer;\r\n\r\nexport const {\r\n    setShowCurrent,\r\n    setCurrentTask,\r\n    setHistoricTask,\r\n    setPreviousTask,\r\n    copyCurrentToPreviousTask,\r\n    setExportingToPDF,\r\n    setExportToPDFJobId,\r\n    resetExportToPDFCounter,\r\n    increaseExportToPDFCounter,\r\n    stopPDFExport,\r\n    setExecutionHistory,\r\n    clearExecutionHistory,\r\n    setRestTasks\r\n} = tasksSlice.actions;\r\n\r\nexport const getShowCurrent = (state: RootState) => state.tasks.showCurrent;\r\nexport const getCurrentTask = (state: RootState) => state.tasks.currentTask;\r\nexport const getHistoricTask = (state: RootState) => state.tasks.historicTask;\r\nexport const getPreviousTask = (state: RootState) => state.tasks.previousTask;\r\nexport const getExportingToPDF = (state: RootState) => state.tasks.exportingToPDF;\r\nexport const getExportToPDFJobId = (state: RootState) => state.tasks.exportToPDFJobId;\r\nexport const getExportToPDFCounter = (state: RootState) => state.tasks.exportToPDFCounter;\r\nexport const getExecutionHistory = (state: RootState) => state.tasks.executionHistory;\r\nexport const getRestTasks = (state: RootState) => state.tasks.restTasks;\r\n\r\nexport const fetchCurrentTask =\r\n    (notebookId: number) =>\r\n        async (dispatch: Dispatch<AnyAction>) => {\r\n\r\n            const sessionId = getSessionId();\r\n\r\n            try {\r\n                const url = `/api/v1/latest_task/${notebookId}/${sessionId}/`;\r\n                const { data } = await axios.get(url);\r\n                dispatch(setCurrentTask(data))\r\n\r\n            } catch (error) {\r\n                // console.clear();\r\n                dispatch(setCurrentTask({} as ITask));\r\n            }\r\n\r\n        };\r\n\r\nexport const scrapeSlidesHash = () => {\r\n    try {\r\n        const iframeElement = (document.getElementById(\"main-iframe\") as HTMLIFrameElement);\r\n        const hash = iframeElement?.contentWindow?.location?.hash;\r\n        if (hash) {\r\n            return hash;\r\n        }\r\n    } catch (error) { }\r\n    return \"\";\r\n}\r\n\r\n\r\nexport const executeNotebook =\r\n    (notebookId: number) =>\r\n        async (dispatch: Dispatch<AnyAction>, getState: () => any) => {\r\n            const { widgets } = getState().widgets;\r\n            const sessionId = getSessionId();\r\n\r\n            const slidesHash = scrapeSlidesHash();\r\n            dispatch(setSlidesHash(slidesHash));\r\n\r\n            try {\r\n                const task = {\r\n                    session_id: sessionId,\r\n                    params: JSON.stringify(widgets),\r\n                }\r\n                const url = `/api/v1/execute/${notebookId}/`;\r\n                const { data } = await axios.post(url, task);\r\n                dispatch(setCurrentTask(data))\r\n\r\n            } catch (error) {\r\n                console.error(`Problem during notebook execution. ${error}`);\r\n            }\r\n\r\n        };\r\n\r\n\r\nexport const clearTasks =\r\n    (notebookId: number) =>\r\n        async (dispatch: Dispatch<AnyAction>) => {\r\n            try {\r\n                const sessionId = getSessionId();\r\n                const url = `/api/v1/clear_tasks/${notebookId}/${sessionId}/`;\r\n                await axios.post(url);\r\n                dispatch(setCurrentTask({} as ITask));\r\n                dispatch(setHistoricTask({} as ITask));\r\n                dispatch(setPreviousTask({} as ITask));\r\n                dispatch(setExecutionHistory([]));\r\n                toast.success(\"All previous tasks deleted. The default view of the app is displayed.\")\r\n            } catch (error) {\r\n                toast.error(`Trying to clear previous tasks. The error occured. ${error}`)\r\n            }\r\n        };\r\n\r\n\r\nexport const exportToPDF =\r\n    (siteId: number, notebookId: number, notebookPath: string) =>\r\n        async (dispatch: Dispatch<AnyAction>) => {\r\n            try {\r\n                dispatch(setExportingToPDF(true));\r\n                dispatch(resetExportToPDFCounter());\r\n                dispatch(setExportToPDFJobId(\"\"));\r\n\r\n                const sessionId = getSessionId();\r\n                const url = `/api/v1/export_pdf/`;\r\n                // convert from JS camel case to Python undescore variables\r\n                const params = {\r\n                    site_id: siteId,\r\n                    session_id: sessionId,\r\n                    notebook_id: notebookId,\r\n                    notebook_path: notebookPath,\r\n                }\r\n                const { data } = await axios.post(url, params);\r\n                dispatch(setExportToPDFJobId(data.job_id))\r\n            } catch (error) {\r\n                toast.error(`The error occured during PDF export. ${error}`);\r\n                dispatch(stopPDFExport());\r\n            }\r\n        };\r\n\r\nexport const getPDF =\r\n    (jobId: string) =>\r\n        async (dispatch: Dispatch<AnyAction>) => {\r\n            try {\r\n                const url = `/api/v1/get_pdf/${jobId}/`;\r\n                const { data } = await axios.get(url);\r\n                if (data.ready) {\r\n                    dispatch(stopPDFExport());\r\n                    if (data.error !== \"\") {\r\n                        toast.error(data.error);\r\n                    } else {\r\n                        handleDownload(\r\n                            `${axios.defaults.baseURL}${data.url}`,\r\n                            `${data.title}`\r\n                        )\r\n                    }\r\n                } else {\r\n                    dispatch(increaseExportToPDFCounter());\r\n                }\r\n            } catch (error) {\r\n                toast.error(`The error occured during PDF export. ${error}`);\r\n                dispatch(stopPDFExport());\r\n            }\r\n        };\r\n\r\n\r\n\r\nexport const fetchExecutionHistory =\r\n    (notebookId: number, clearPreviousHistory = true) =>\r\n        async (dispatch: Dispatch<AnyAction>) => {\r\n\r\n            dispatch(setHistoricTask({} as ITask));\r\n            if (clearPreviousHistory) {\r\n                dispatch(clearExecutionHistory());\r\n            }\r\n\r\n            const sessionId = getSessionId();\r\n\r\n            try {\r\n                const url = `/api/v1/execution_history/${notebookId}/${sessionId}/`;\r\n                const { data } = await axios.get(url);\r\n                dispatch(setExecutionHistory(data))\r\n            } catch (error) {\r\n                dispatch(clearExecutionHistory());\r\n            }\r\n\r\n        };\r\n\r\n\r\nexport const listRestTasks =\r\n    (siteId: number, notebookId: number) =>\r\n        async (dispatch: Dispatch<AnyAction>) => {\r\n            try {\r\n                dispatch(setRestTasks([]));\r\n                const url = `/api/v1/${siteId}/${notebookId}/list-rest-tasks/`;\r\n                const { data } = await axios.get(url);\r\n                dispatch(setRestTasks(data));\r\n            } catch (error) {\r\n                dispatch(setRestTasks([]));\r\n            }\r\n        };\r\n\r\n",
+        "/* eslint-disable import/no-cycle */\r\nimport {\r\n  createSlice,\r\n  PayloadAction,\r\n  AnyAction,\r\n  Dispatch,\r\n} from \"@reduxjs/toolkit\";\r\nimport axios, { AxiosError } from \"axios\";\r\n\r\nimport { RootState } from \"../store\";\r\nimport { clearExecutionHistory } from \"./tasksSlice\";\r\nimport { setShowSideBar } from \"./appSlice\";\r\nimport {\r\n  IWidget,\r\n  isSelectWidget,\r\n  isSliderWidget,\r\n  isTextWidget,\r\n  isRangeWidget,\r\n  isCheckboxWidget,\r\n  isNumericWidget,\r\n  isMarkdownWidget,\r\n  isButtonWidget,\r\n  isFileWidget,\r\n} from \"../widgets/Types\";\r\nimport { getWindowDimensions } from \"../components/WindowDimensions\";\r\nimport { setSiteStatus, SiteStatus } from \"./sitesSlice\";\r\n\r\nexport const RUN_DELAY = 600; // ms\r\nexport const RUN_DELAY_FAST = 100; // ms\r\n\r\nexport interface INotebookParams {\r\n  title: string | null;\r\n  description: string | null;\r\n  date: string | null;\r\n  author: string | null;\r\n  \"show-code\": boolean | null;\r\n  params: Record<string, IWidget>; //IWidget[];\r\n  version: string;\r\n  continuous_update: boolean;\r\n  static_notebook: boolean;\r\n  show_sidebar: boolean;\r\n  full_screen: boolean;\r\n  allow_download: boolean;\r\n  allow_share: boolean;\r\n}\r\n\r\nexport interface INotebook {\r\n  id: number;\r\n  created_at: Date;\r\n  file_updated_at: Date;\r\n  title: string;\r\n  slug: string;\r\n  path: string;\r\n  share: string;\r\n  params: INotebookParams;\r\n  state: string;\r\n  default_view_path: string;\r\n  output: string;\r\n  format: string;\r\n  slidesHash: string;\r\n  schedule: string;\r\n  errors: string;\r\n}\r\n\r\nexport type WidgetValueType =\r\n  | string\r\n  | boolean\r\n  | number\r\n  | [number, number]\r\n  | string[]\r\n  | null\r\n  | undefined\r\n  | unknown;\r\n\r\nconst initialState = {\r\n  notebooks: [] as INotebook[],\r\n  loadingState: \"loading\",\r\n  selectedNotebook: {} as INotebook,\r\n  selectedNotebookId: undefined as undefined | number,\r\n  loadingStateSelected: \"loading\",\r\n  watchModeCounter: 0,\r\n  slidesHash: \"\",\r\n  widgets: {} as Record<string, WidgetValueType>,\r\n  widgetsUrlValues: {} as Record<string, WidgetValueType>,\r\n  nbIframes: {} as Record<string, string>, // slug -> signed URL\r\n  widgetsInitialized: false,\r\n  urlValuesUsed: false,\r\n};\r\n\r\nconst notebooksSlice = createSlice({\r\n  name: \"notebooks\",\r\n  initialState,\r\n  reducers: {\r\n    setWidgetValue(\r\n      state,\r\n      action: PayloadAction<{ key: string; value: WidgetValueType }>\r\n    ) {\r\n      const { key, value } = action.payload;\r\n      state.widgets[key] = value;\r\n      //console.log({ key, value });\r\n    },\r\n    setWidgetUrlValue(\r\n      state,\r\n      action: PayloadAction<{ key: string; value: WidgetValueType }>\r\n    ) {\r\n      const { key, value } = action.payload;\r\n      state.widgetsUrlValues[key] = value;\r\n    },\r\n    clearWidgets(state) {\r\n      state.widgets = {};\r\n    },\r\n    clearWidgetsUrlValues(state) {\r\n      state.widgetsUrlValues = {};\r\n    },\r\n    setNotebooks(state, action: PayloadAction<INotebook[]>) {\r\n      state.notebooks = action.payload;\r\n    },\r\n    setLoadingState(state, action: PayloadAction<string>) {\r\n      state.loadingState = action.payload;\r\n    },\r\n    setSelectedNotebook(state, action: PayloadAction<INotebook>) {\r\n      if (\r\n        action.payload.state.startsWith(\"WATCH\") &&\r\n        state.selectedNotebook.file_updated_at ===\r\n        action.payload.file_updated_at\r\n      ) {\r\n        // console.log(\"skip notebook update\")\r\n      } else {\r\n        state.selectedNotebook = action.payload;\r\n        state.selectedNotebookId = state.selectedNotebook.id;\r\n      }\r\n      if (action.payload.state.startsWith(\"WATCH\")) {\r\n        state.watchModeCounter += 1;\r\n      }\r\n    },\r\n    setLoadingStateSelected(state, action: PayloadAction<string>) {\r\n      state.loadingStateSelected = action.payload;\r\n    },\r\n    setSlidesHash(state, action: PayloadAction<string>) {\r\n      state.slidesHash = action.payload;\r\n    },\r\n    updateWidgetsParams(state, action: PayloadAction<any>) {\r\n      const { widgetKey } = action.payload;\r\n\r\n      let updated = false;\r\n\r\n      let noMatch = true;\r\n\r\n      for (let key of Object.keys(state.selectedNotebook.params.params)) {\r\n        if (key === widgetKey) {\r\n          noMatch = false;\r\n          let widget = { ...state.selectedNotebook.params.params[widgetKey] };\r\n\r\n          if (isRangeWidget(widget)) {\r\n            if (widget.disabled !== action.payload.disabled) {\r\n              widget.disabled = action.payload.disabled;\r\n              state.widgets[key] = action.payload.value;\r\n              updated = true;\r\n            }\r\n            if (widget.hidden !== action.payload.hidden) {\r\n              widget.hidden = action.payload.hidden;\r\n              state.widgets[key] = action.payload.value;\r\n              updated = true;\r\n            }\r\n            if (widget.min !== action.payload.min) {\r\n              widget.min = action.payload.min;\r\n              state.widgets[key] = action.payload.value;\r\n              updated = true;\r\n            }\r\n            if (widget.max !== action.payload.max) {\r\n              widget.max = action.payload.max;\r\n              state.widgets[key] = action.payload.value;\r\n              updated = true;\r\n            }\r\n            if (widget.step !== action.payload.step) {\r\n              widget.step = action.payload.step;\r\n              state.widgets[key] = action.payload.value;\r\n              updated = true;\r\n            }\r\n            if (widget.label !== action.payload.label) {\r\n              widget.label = action.payload.label;\r\n              updated = true;\r\n            }\r\n          } else if (isTextWidget(widget)) {\r\n            if (widget.disabled !== action.payload.disabled) {\r\n              widget.disabled = action.payload.disabled;\r\n              state.widgets[key] = action.payload.value;\r\n              updated = true;\r\n            }\r\n            if (widget.hidden !== action.payload.hidden) {\r\n              widget.hidden = action.payload.hidden;\r\n              state.widgets[key] = action.payload.value;\r\n              updated = true;\r\n            }\r\n            if (widget.rows !== action.payload.rows) {\r\n              widget.rows = action.payload.rows;\r\n              updated = true;\r\n            }\r\n            if (widget.label !== action.payload.label) {\r\n              widget.label = action.payload.label;\r\n              updated = true;\r\n            }\r\n          } else if (isSliderWidget(widget)) {\r\n            if (widget.disabled !== action.payload.disabled) {\r\n              widget.disabled = action.payload.disabled;\r\n              state.widgets[key] = action.payload.value;\r\n              updated = true;\r\n            }\r\n            if (widget.hidden !== action.payload.hidden) {\r\n              widget.hidden = action.payload.hidden;\r\n              state.widgets[key] = action.payload.value;\r\n              updated = true;\r\n            }\r\n            if (widget.min !== action.payload.min) {\r\n              widget.min = action.payload.min;\r\n              state.widgets[key] = action.payload.value;\r\n              updated = true;\r\n            }\r\n            if (widget.max !== action.payload.max) {\r\n              widget.max = action.payload.max;\r\n              state.widgets[key] = action.payload.value;\r\n              updated = true;\r\n            }\r\n            if (widget.step !== action.payload.step) {\r\n              widget.step = action.payload.step;\r\n              state.widgets[key] = action.payload.value;\r\n              updated = true;\r\n            }\r\n            if (widget.label !== action.payload.label) {\r\n              widget.label = action.payload.label;\r\n              updated = true;\r\n            }\r\n          } else if (isSelectWidget(widget)) {\r\n            if (widget.disabled !== action.payload.disabled) {\r\n              widget.disabled = action.payload.disabled;\r\n              state.widgets[key] = action.payload.value;\r\n              updated = true;\r\n            }\r\n            if (widget.hidden !== action.payload.hidden) {\r\n              widget.hidden = action.payload.hidden;\r\n              state.widgets[key] = action.payload.value;\r\n              updated = true;\r\n            }\r\n            if (\r\n              widget.choices.toString() !== action.payload.choices.toString()\r\n            ) {\r\n              widget.choices = action.payload.choices;\r\n              state.widgets[key] = action.payload.value;\r\n              updated = true;\r\n            }\r\n            if (widget.label !== action.payload.label) {\r\n              widget.label = action.payload.label;\r\n              updated = true;\r\n            }\r\n          } else if (isCheckboxWidget(widget)) {\r\n            if (widget.disabled !== action.payload.disabled) {\r\n              widget.disabled = action.payload.disabled;\r\n              state.widgets[key] = action.payload.value;\r\n              updated = true;\r\n            }\r\n            if (widget.hidden !== action.payload.hidden) {\r\n              widget.hidden = action.payload.hidden;\r\n              state.widgets[key] = action.payload.value;\r\n              updated = true;\r\n            }\r\n            if (widget.label !== action.payload.label) {\r\n              widget.label = action.payload.label;\r\n              updated = true;\r\n            }\r\n          } else if (isNumericWidget(widget)) {\r\n            if (widget.disabled !== action.payload.disabled) {\r\n              widget.disabled = action.payload.disabled;\r\n              state.widgets[key] = action.payload.value;\r\n              updated = true;\r\n            }\r\n            if (widget.hidden !== action.payload.hidden) {\r\n              widget.hidden = action.payload.hidden;\r\n              state.widgets[key] = action.payload.value;\r\n              updated = true;\r\n            }\r\n            if (widget.min !== action.payload.min) {\r\n              widget.min = action.payload.min;\r\n              state.widgets[key] = action.payload.value;\r\n              updated = true;\r\n            }\r\n            if (widget.max !== action.payload.max) {\r\n              widget.max = action.payload.max;\r\n              state.widgets[key] = action.payload.value;\r\n              updated = true;\r\n            }\r\n            if (widget.step !== action.payload.step) {\r\n              widget.step = action.payload.step;\r\n              state.widgets[key] = action.payload.value;\r\n              updated = true;\r\n            }\r\n            if (widget.label !== action.payload.label) {\r\n              widget.label = action.payload.label;\r\n              updated = true;\r\n            }\r\n          } else if (isMarkdownWidget(widget)) {\r\n            if (widget.value !== action.payload.value) {\r\n              widget.value = action.payload.value;\r\n              updated = true;\r\n            }\r\n          } else if (isButtonWidget(widget)) {\r\n            state.widgets[key] = action.payload.value;\r\n            if (widget.disabled !== action.payload.disabled) {\r\n              widget.disabled = action.payload.disabled;\r\n              state.widgets[key] = action.payload.value;\r\n              updated = true;\r\n            }\r\n            if (widget.hidden !== action.payload.hidden) {\r\n              widget.hidden = action.payload.hidden;\r\n              state.widgets[key] = action.payload.value;\r\n              updated = true;\r\n            }\r\n            if (widget.label !== action.payload.label) {\r\n              widget.label = action.payload.label;\r\n              updated = true;\r\n            }\r\n            if (widget.style !== action.payload.style) {\r\n              widget.style = action.payload.style;\r\n              updated = true;\r\n            }\r\n          } else if (isFileWidget(widget)) {\r\n            state.widgets[key] = action.payload.value;\r\n            if (widget.disabled !== action.payload.disabled) {\r\n              widget.disabled = action.payload.disabled;\r\n              state.widgets[key] = action.payload.value;\r\n              updated = true;\r\n            }\r\n            if (widget.hidden !== action.payload.hidden) {\r\n              widget.hidden = action.payload.hidden;\r\n              state.widgets[key] = action.payload.value;\r\n              updated = true;\r\n            }\r\n            if (widget.label !== action.payload.label) {\r\n              widget.label = action.payload.label;\r\n              updated = true;\r\n            }\r\n          }\r\n\r\n          if (updated) {\r\n            state.selectedNotebook.params.params[widgetKey] = widget;\r\n          }\r\n        }\r\n      }\r\n      if (noMatch) {\r\n        state.selectedNotebook.params.params[widgetKey] = action.payload;\r\n      }\r\n    },\r\n    hideWidgets(state, action: PayloadAction<any>) {\r\n      const { keys } = action.payload;\r\n      for (let key of keys) {\r\n        if (key in state.selectedNotebook.params.params) {\r\n          delete state.selectedNotebook.params.params[key];\r\n        }\r\n      }\r\n    },\r\n    initWidgets(state, action: PayloadAction<any>) {\r\n      const { widgets } = action.payload;\r\n      state.selectedNotebook.params.params = {}\r\n      state.widgets = {}\r\n      for (let widget of widgets) {\r\n        state.selectedNotebook.params.params[widget.widgetKey] = widget;\r\n        state.widgets[widget.widgetKey] = widget.value;\r\n      }\r\n    },\r\n    updateTitle(state, action: PayloadAction<string>) {\r\n      state.selectedNotebook.title = action.payload;\r\n    },\r\n    updateShowCode(state, action: PayloadAction<boolean>) {\r\n      state.selectedNotebook.params[\"show-code\"] = action.payload;\r\n    },\r\n    setNbIframes(state, action: PayloadAction<Record<string, string>>) {\r\n      state.nbIframes = action.payload;\r\n    },\r\n    setWidgetsInitialized(state, action: PayloadAction<boolean>) {\r\n      state.widgetsInitialized = action.payload;\r\n    },\r\n    setUrlValuesUsed(state, action: PayloadAction<boolean>) {\r\n      state.urlValuesUsed = action.payload;\r\n    }\r\n  },\r\n});\r\n\r\nexport default notebooksSlice.reducer;\r\n\r\nexport const {\r\n  setNotebooks,\r\n  setLoadingState,\r\n  setSelectedNotebook,\r\n  setLoadingStateSelected,\r\n  setSlidesHash,\r\n  updateWidgetsParams,\r\n  hideWidgets,\r\n  setWidgetValue,\r\n  setWidgetUrlValue,\r\n  clearWidgets,\r\n  clearWidgetsUrlValues,\r\n  initWidgets,\r\n  updateTitle,\r\n  updateShowCode,\r\n  setNbIframes,\r\n  setWidgetsInitialized,\r\n  setUrlValuesUsed\r\n} = notebooksSlice.actions;\r\n\r\nexport const getNotebooks = (state: RootState) => state.notebooks.notebooks;\r\nexport const getLoadingState = (state: RootState) =>\r\n  state.notebooks.loadingState;\r\nexport const getSelectedNotebook = (state: RootState) =>\r\n  state.notebooks.selectedNotebook;\r\nexport const getSelectedNotebookId = (state: RootState) =>\r\n  state.notebooks.selectedNotebookId;\r\nexport const isStaticNotebook = (state: RootState) => {\r\n  let st = state.notebooks.selectedNotebook?.params?.static_notebook;\r\n  if (st === undefined) {\r\n    return false;\r\n  }\r\n  return st;\r\n};\r\nexport const getLoadingStateSelected = (state: RootState) =>\r\n  state.notebooks.loadingStateSelected;\r\nexport const getWatchModeCounter = (state: RootState) =>\r\n  state.notebooks.watchModeCounter;\r\nexport const getSlidesHash = (state: RootState) => state.notebooks.slidesHash;\r\n\r\nexport const getWidgetsValues = (state: RootState): Record<string, WidgetValueType> => state.notebooks.widgets;\r\nexport const getWidgetsUrlValues = (state: RootState): Record<string, WidgetValueType> => state.notebooks.widgetsUrlValues;\r\n\r\n\r\nexport const getNbIframes = (state: RootState) => state.notebooks.nbIframes;\r\nexport const getWidgetsInitialized = (state: RootState) => state.notebooks.widgetsInitialized;\r\nexport const getUrlValuesUsed = (state: RootState) => state.notebooks.urlValuesUsed;\r\n\r\nexport const fetchNbIframes = (siteId: number) => async (dispatch: Dispatch<AnyAction>) => {\r\n  try {\r\n    const url = `/api/v1/${siteId}/nb-iframes/`;\r\n    const { data } = await axios.get(url);\r\n    dispatch(setNbIframes(data));\r\n  } catch (error) {\r\n    console.error(`Problem during loading notebooks iframes. ${error}`);\r\n  }\r\n};\r\n\r\n\r\nexport const fetchNotebooks = (siteId: number) => async (dispatch: Dispatch<AnyAction>) => {\r\n  try {\r\n    dispatch(setSlidesHash(\"\"));\r\n    dispatch(setLoadingState(\"loading\"));\r\n    dispatch(clearExecutionHistory());\r\n    const url = `/api/v1/${siteId}/notebooks/`;\r\n    const { data } = await axios.get(url);\r\n    const parsedNotebooks = data.map((notebook: any) => {\r\n      const parsedParams = JSON.parse(notebook.params);\r\n\r\n      return {\r\n        ...notebook,\r\n        params: parsedParams as INotebookParams,\r\n      };\r\n    });\r\n    dispatch(setNotebooks(parsedNotebooks));\r\n    dispatch(setLoadingState(\"loaded\"));\r\n  } catch (error) {\r\n    dispatch(setLoadingState(\"error\"));\r\n    console.error(`Problem during loading recent notebooks. ${error}`);\r\n  }\r\n};\r\n\r\nexport const fetchNotebook =\r\n  (siteId: number, id: number, silent = false) =>\r\n    async (dispatch: Dispatch<AnyAction>) => {\r\n      try {\r\n        if (!silent) {\r\n          dispatch(setSlidesHash(\"\"));\r\n          dispatch(clearExecutionHistory());\r\n        }\r\n\r\n        const { width } = getWindowDimensions();\r\n        dispatch(setShowSideBar(width > 992));\r\n\r\n        if (!silent) {\r\n          dispatch(setLoadingStateSelected(\"loading\"));\r\n        }\r\n        const url = `/api/v1/${siteId}/notebooks/${id}/`;\r\n        const { data } = await axios.get(url);\r\n        const parsedParams = JSON.parse(data.params) as INotebookParams;\r\n        dispatch(\r\n          setSelectedNotebook({\r\n            ...data,\r\n            params: parsedParams,\r\n          })\r\n        );\r\n        if (!silent) {\r\n          dispatch(setLoadingStateSelected(\"loaded\"));\r\n        }\r\n        if (parsedParams?.show_sidebar !== null && parsedParams?.show_sidebar !== undefined) {\r\n          dispatch(setShowSideBar(parsedParams?.show_sidebar));\r\n        }\r\n      } catch (error) {\r\n        if (!silent) {\r\n          dispatch(setLoadingStateSelected(\"error\"));\r\n        }\r\n        console.error(\r\n          `Problem during loading selected notebook (${id}). ${error}`\r\n        );\r\n      }\r\n    };\r\n\r\nexport const fetchNotebookWithSlug =\r\n  (siteId: number, slug: string, silent = false) =>\r\n    async (dispatch: Dispatch<AnyAction>) => {\r\n      try {\r\n        if (!silent) {\r\n          dispatch(setSlidesHash(\"\"));\r\n          dispatch(clearExecutionHistory());\r\n        }\r\n\r\n        const { width } = getWindowDimensions();\r\n        dispatch(setShowSideBar(width > 992));\r\n\r\n        if (!silent) {\r\n          dispatch(setLoadingStateSelected(\"loading\"));\r\n        }\r\n        const url = `/api/v1/${siteId}/getnb/${slug}/`;\r\n        const { data } = await axios.get(url);\r\n        const parsedParams = JSON.parse(data.params) as INotebookParams;\r\n        dispatch(\r\n          setSelectedNotebook({\r\n            ...data,\r\n            params: parsedParams,\r\n          })\r\n        );\r\n        if (!silent) {\r\n          dispatch(setLoadingStateSelected(\"loaded\"));\r\n        }\r\n        if (parsedParams?.show_sidebar !== null && parsedParams?.show_sidebar !== undefined) {\r\n          dispatch(setShowSideBar(parsedParams?.show_sidebar));\r\n        }\r\n      } catch (error) {\r\n        const err = error as AxiosError;\r\n\r\n        if (!silent) {\r\n          dispatch(setLoadingStateSelected(\"error\"));\r\n\r\n          if (err.response?.status === 404) {\r\n            // switch to notebook not found view\r\n            dispatch(setSiteStatus(SiteStatus.NotebookNotFound))\r\n          }\r\n        }\r\n        console.error(\r\n          `Problem during loading selected notebook (${slug}). ${error}`\r\n        );\r\n\r\n\r\n      }\r\n    };\r\n",
+        "/* eslint-disable import/no-cycle */\r\nimport {\r\n    createSlice,\r\n    AnyAction,\r\n    Dispatch,\r\n    PayloadAction,\r\n} from '@reduxjs/toolkit';\r\nimport axios from 'axios';\r\nimport { RootState } from '../store';\r\nimport { toast } from \"react-toastify\";\r\nimport { getSessionId, handleDownload } from '../utils';\r\nimport { setSlidesHash } from './notebooksSlice';\r\n\r\nexport interface ITask {\r\n    id: number;\r\n    task_id: string;\r\n    session_id: string;\r\n    created_at: Date;\r\n    state: \"CREATED\" | \"RECEIVED\" | \"DONE\" | \"ERROR\";\r\n    params: string;\r\n    result: string;\r\n}\r\n\r\nconst initialState = {\r\n    currentTask: {} as ITask,\r\n    historicTask: {} as ITask,\r\n    showCurrent: true,\r\n    previousTask: {} as ITask,\r\n    exportingToPDF: false,\r\n    exportToPDFJobId: '',\r\n    exportToPDFCounter: 0,\r\n    executionHistory: [] as ITask[],\r\n};\r\n\r\nconst tasksSlice = createSlice({\r\n    name: 'tasks',\r\n    initialState,\r\n    reducers: {\r\n        setShowCurrent(state, action: PayloadAction<boolean>) {\r\n            state.showCurrent = action.payload;\r\n        },\r\n        setCurrentTask(state, action: PayloadAction<ITask>) {\r\n            state.currentTask = action.payload;\r\n        },\r\n        setHistoricTask(state, action: PayloadAction<ITask>) {\r\n            state.historicTask = action.payload;\r\n        },\r\n        setPreviousTask(state, action: PayloadAction<ITask>) {\r\n            state.previousTask = action.payload;\r\n        },\r\n        copyCurrentToPreviousTask(state) {\r\n            state.previousTask = state.currentTask;\r\n        },\r\n        setExportingToPDF(state, action: PayloadAction<boolean>) {\r\n            state.exportingToPDF = action.payload;\r\n        },\r\n        setExportToPDFJobId(state, action: PayloadAction<string>) {\r\n            state.exportToPDFJobId = action.payload;\r\n        },\r\n        resetExportToPDFCounter(state) {\r\n            state.exportToPDFCounter = 0;\r\n        },\r\n        increaseExportToPDFCounter(state) {\r\n            state.exportToPDFCounter += 1;\r\n        },\r\n        stopPDFExport(state) {\r\n            state.exportingToPDF = false;\r\n            state.exportToPDFJobId = \"\";\r\n            state.exportToPDFCounter = 0;\r\n        },\r\n        setExecutionHistory(state, action: PayloadAction<ITask[]>) {\r\n            state.executionHistory = action.payload;\r\n        },\r\n        clearExecutionHistory(state) {\r\n            state.executionHistory = [];\r\n        }\r\n    },\r\n});\r\n\r\nexport default tasksSlice.reducer;\r\n\r\nexport const {\r\n    setShowCurrent,\r\n    setCurrentTask,\r\n    setHistoricTask,\r\n    setPreviousTask,\r\n    copyCurrentToPreviousTask,\r\n    setExportingToPDF,\r\n    setExportToPDFJobId,\r\n    resetExportToPDFCounter,\r\n    increaseExportToPDFCounter,\r\n    stopPDFExport,\r\n    setExecutionHistory,\r\n    clearExecutionHistory\r\n} = tasksSlice.actions;\r\n\r\nexport const getShowCurrent = (state: RootState) => state.tasks.showCurrent;\r\nexport const getCurrentTask = (state: RootState) => state.tasks.currentTask;\r\nexport const getHistoricTask = (state: RootState) => state.tasks.historicTask;\r\nexport const getPreviousTask = (state: RootState) => state.tasks.previousTask;\r\nexport const getExportingToPDF = (state: RootState) => state.tasks.exportingToPDF;\r\nexport const getExportToPDFJobId = (state: RootState) => state.tasks.exportToPDFJobId;\r\nexport const getExportToPDFCounter = (state: RootState) => state.tasks.exportToPDFCounter;\r\nexport const getExecutionHistory = (state: RootState) => state.tasks.executionHistory;\r\n\r\nexport const fetchCurrentTask =\r\n    (notebookId: number) =>\r\n        async (dispatch: Dispatch<AnyAction>) => {\r\n\r\n            const sessionId = getSessionId();\r\n\r\n            try {\r\n                const url = `/api/v1/latest_task/${notebookId}/${sessionId}/`;\r\n                const { data } = await axios.get(url);\r\n                dispatch(setCurrentTask(data))\r\n\r\n            } catch (error) {\r\n                // console.clear();\r\n                dispatch(setCurrentTask({} as ITask));\r\n            }\r\n\r\n        };\r\n\r\nexport const scrapeSlidesHash = () => {\r\n    try {\r\n        const iframeElement = (document.getElementById(\"main-iframe\") as HTMLIFrameElement);\r\n        const hash = iframeElement?.contentWindow?.location?.hash;\r\n        if (hash) {\r\n            return hash;\r\n        }\r\n    } catch (error) { }\r\n    return \"\";\r\n}\r\n\r\n\r\nexport const executeNotebook =\r\n    (notebookId: number) =>\r\n        async (dispatch: Dispatch<AnyAction>, getState: () => any) => {\r\n            const { widgets } = getState().widgets;\r\n            const sessionId = getSessionId();\r\n\r\n            const slidesHash = scrapeSlidesHash();\r\n            dispatch(setSlidesHash(slidesHash));\r\n\r\n            try {\r\n                const task = {\r\n                    session_id: sessionId,\r\n                    params: JSON.stringify(widgets),\r\n                }\r\n                const url = `/api/v1/execute/${notebookId}/`;\r\n                const { data } = await axios.post(url, task);\r\n                dispatch(setCurrentTask(data))\r\n\r\n            } catch (error) {\r\n                console.error(`Problem during notebook execution. ${error}`);\r\n            }\r\n\r\n        };\r\n\r\n\r\nexport const clearTasks =\r\n    (notebookId: number) =>\r\n        async (dispatch: Dispatch<AnyAction>) => {\r\n            try {\r\n                const sessionId = getSessionId();\r\n                const url = `/api/v1/clear_tasks/${notebookId}/${sessionId}/`;\r\n                await axios.post(url);\r\n                dispatch(setCurrentTask({} as ITask));\r\n                dispatch(setHistoricTask({} as ITask));\r\n                dispatch(setPreviousTask({} as ITask));\r\n                dispatch(setExecutionHistory([]));\r\n                toast.success(\"All previous tasks deleted. The default view of the app is displayed.\")\r\n            } catch (error) {\r\n                toast.error(`Trying to clear previous tasks. The error occured. ${error}`)\r\n            }\r\n        };\r\n\r\n\r\nexport const exportToPDF =\r\n    (siteId: number, notebookId: number, notebookPath: string) =>\r\n        async (dispatch: Dispatch<AnyAction>) => {\r\n            try {\r\n                dispatch(setExportingToPDF(true));\r\n                dispatch(resetExportToPDFCounter());\r\n                dispatch(setExportToPDFJobId(\"\"));\r\n\r\n                const sessionId = getSessionId();\r\n                const url = `/api/v1/export_pdf/`;\r\n                // convert from JS camel case to Python undescore variables\r\n                const params = {\r\n                    site_id: siteId,\r\n                    session_id: sessionId,\r\n                    notebook_id: notebookId,\r\n                    notebook_path: notebookPath,\r\n                }\r\n                const { data } = await axios.post(url, params);\r\n                dispatch(setExportToPDFJobId(data.job_id))\r\n            } catch (error) {\r\n                toast.error(`The error occured during PDF export. ${error}`);\r\n                dispatch(stopPDFExport());\r\n            }\r\n        };\r\n\r\nexport const getPDF =\r\n    (jobId: string) =>\r\n        async (dispatch: Dispatch<AnyAction>) => {\r\n            try {\r\n                const url = `/api/v1/get_pdf/${jobId}/`;\r\n                const { data } = await axios.get(url);\r\n                if (data.ready) {\r\n                    dispatch(stopPDFExport());\r\n                    if (data.error !== \"\") {\r\n                        toast.error(data.error);\r\n                    } else {\r\n                        handleDownload(\r\n                            `${axios.defaults.baseURL}${data.url}`,\r\n                            `${data.title}`\r\n                        )\r\n                    }\r\n                } else {\r\n                    dispatch(increaseExportToPDFCounter());\r\n                }\r\n            } catch (error) {\r\n                toast.error(`The error occured during PDF export. ${error}`);\r\n                dispatch(stopPDFExport());\r\n            }\r\n        };\r\n\r\n\r\n\r\nexport const fetchExecutionHistory =\r\n    (notebookId: number, clearPreviousHistory = true) =>\r\n        async (dispatch: Dispatch<AnyAction>) => {\r\n\r\n            dispatch(setHistoricTask({} as ITask));\r\n            if (clearPreviousHistory) {\r\n                dispatch(clearExecutionHistory());\r\n            }\r\n\r\n            const sessionId = getSessionId();\r\n\r\n            try {\r\n                const url = `/api/v1/execution_history/${notebookId}/${sessionId}/`;\r\n                const { data } = await axios.get(url);\r\n                dispatch(setExecutionHistory(data))\r\n            } catch (error) {\r\n                dispatch(clearExecutionHistory());\r\n            }\r\n\r\n        };\r\n\r\n",
         "/* eslint-disable jsx-a11y/anchor-is-valid */\nimport React, { useEffect, useState } from \"react\";\nimport { useDispatch } from \"react-redux\";\nimport { useSearchParams } from \"react-router-dom\";\n\nimport {\n  setUrlValuesUsed,\n  setWidgetUrlValue,\n  setWidgetValue,\n} from \"../slices/notebooksSlice\";\n\ntype CheckboxProps = {\n  widgetKey: string;\n  label: string | null;\n  value: boolean | null;\n  disabled: boolean;\n  hidden: boolean;\n  runNb: () => void;\n  url_key: string;\n};\n\nexport default function CheckboxWidget({\n  widgetKey,\n  label,\n  value,\n  disabled,\n  hidden,\n  runNb,\n  url_key,\n}: CheckboxProps) {\n  const dispatch = useDispatch();\n  const [updated, userInteraction] = useState(false);\n\n  const [searchParams] = useSearchParams();\n\n  useEffect(() => {\n    if (url_key !== undefined && url_key !== \"\") {\n      const urlValue = searchParams.get(url_key)?.toLowerCase();\n\n      if (\n        !updated &&\n        urlValue !== undefined &&\n        (urlValue === \"true\" || urlValue === \"false\")\n      ) {\n        dispatch(\n          setWidgetUrlValue({\n            key: widgetKey,\n            value: urlValue === \"true\",\n          })\n        );\n        dispatch(setUrlValuesUsed(true));\n      }\n    }\n  }, [dispatch, searchParams, updated, url_key, widgetKey]);\n\n  useEffect(() => {\n    if (updated) {\n      runNb();\n    }\n    // eslint-disable-next-line react-hooks/exhaustive-deps\n  }, [value]);\n\n  return (\n    <div className=\"form-group form-check form-switch mb-3\"  style={{ display: hidden ? \"none\" : \"\" }}>\n      <input\n        className=\"form-check-input\"\n        type=\"checkbox\"\n        id={`checkbox-${label}`}\n        disabled={disabled}\n        onChange={() => {\n          userInteraction(true);\n          dispatch(setWidgetValue({ key: widgetKey, value: !value }));\n        }}\n        checked={value != null ? value : false}\n      />\n      <label\n        className=\"form-check-label\"\n        htmlFor={`checkbox-${label}`}\n        style={{ color: disabled ? \"#555\" : \"#212529\" }}\n      >\n        {label}\n      </label>\n    </div>\n  );\n}\n",
         "import React, { useEffect, useState } from \"react\";\nimport { useDispatch } from \"react-redux\";\nimport { useSearchParams } from \"react-router-dom\";\nimport {\n  setUrlValuesUsed,\n  setWidgetUrlValue,\n  setWidgetValue,\n} from \"../slices/notebooksSlice\";\n\ntype NumericProps = {\n  widgetKey: string;\n  label: string | null;\n  value: number | null;\n  min: number | null;\n  max: number | null;\n  step: number | null;\n  disabled: boolean;\n  hidden: boolean;\n  runNb: () => void;\n  continuousUpdate: boolean;\n  url_key: string;\n};\n\nexport default function NumericWidget({\n  widgetKey,\n  label,\n  value,\n  min,\n  max,\n  step,\n  disabled,\n  hidden,\n  runNb,\n  continuousUpdate,\n  url_key,\n}: NumericProps) {\n  const dispatch = useDispatch();\n  const [apply, showApply] = useState(false);\n  const [updated, userInteraction] = useState(false);\n\n  let minValue = 0;\n  let maxValue = 10;\n  let stepValue = 1;\n  if (min !== null) {\n    minValue = min;\n  }\n  if (max !== null) {\n    maxValue = max;\n  }\n  if (step !== null) {\n    stepValue = step;\n  }\n  let displayValue = value !== null && value !== undefined ? value : 0;\n\n  const [searchParams] = useSearchParams();\n  useEffect(() => {\n    if (url_key !== undefined && url_key !== \"\") {\n      const urlValue = searchParams.get(url_key);\n      if (\n        !updated &&\n        urlValue !== undefined &&\n        urlValue !== null &&\n        !isNaN(parseFloat(urlValue)) &&\n        parseFloat(urlValue) >= minValue &&\n        parseFloat(urlValue) <= maxValue\n      ) {\n        dispatch(\n          setWidgetUrlValue({\n            key: widgetKey,\n            value: parseFloat(urlValue),\n          })\n        );\n        dispatch(setUrlValuesUsed(true));\n      }\n    }\n  }, [dispatch, maxValue, minValue, searchParams, updated, url_key, widgetKey]);\n\n  const validateValue = () => {\n    if (min !== null && value !== null && value < min) {\n      dispatch(setWidgetValue({ key: widgetKey, value: min }));\n    }\n    if (max !== null && value !== null && value > max) {\n      dispatch(setWidgetValue({ key: widgetKey, value: max }));\n    }\n  };\n\n  return (\n    <div className=\"form-group mb-3\" style={{ display: hidden ? \"none\" : \"\" }}>\n      <label\n        htmlFor={`checkbox-${label}`}\n        style={{ color: disabled ? \"#555\" : \"#212529\" }}\n      >\n        {label}\n      </label>\n      <input\n        className=\"form-control\"\n        type=\"number\"\n        value={displayValue} // {displayValue as number | string}\n        onChange={(e) => {\n          userInteraction(true);\n          showApply(true);\n          dispatch(setWidgetValue({ key: widgetKey, value: e.target.value }));\n        }}\n        onBlur={(e) => {\n          validateValue();\n        }}\n        onKeyPress={(e) => {\n          if (e.key === \"Enter\") {\n            validateValue();\n            runNb();\n            showApply(false);\n            e.preventDefault();\n          }\n        }}\n        min={minValue}\n        max={maxValue}\n        step={stepValue}\n        disabled={disabled}\n      />\n      {apply && continuousUpdate && (\n        <div\n          style={{\n            float: \"right\",\n            position: \"relative\",\n            top: \"0px\",\n            left: \"0px\",\n          }}\n        >\n          <button\n            className=\"btn btn-sm btn-outline-primary\"\n            onClick={(e) => {\n              validateValue();\n              runNb();\n              showApply(false);\n              e.preventDefault();\n            }}\n            style={{\n              fontSize: \"0.7em\",\n              border: \"none\",\n            }}\n          >\n            Press enter or click to apply\n          </button>\n        </div>\n      )}\n    </div>\n  );\n}\n",
         "import React, { useEffect, useState } from \"react\";\nimport { useDispatch } from \"react-redux\";\nimport {\n  clearWidgetsUrlValues,\n  setUrlValuesUsed,\n  setWidgetUrlValue,\n  setWidgetValue,\n} from \"../slices/notebooksSlice\";\nimport { Range, getTrackBackground } from \"react-range\";\nimport { useSearchParams } from \"react-router-dom\";\n\ntype RangeProps = {\n  widgetKey: string;\n  label: string | null;\n  value: [number, number] | null;\n  min: number | null;\n  max: number | null;\n  step: number | null;\n  vertical: boolean | null;\n  disabled: boolean;\n  hidden: boolean;\n  runNb: () => void;\n  url_key: string;\n};\n\nexport default function RangeWidget({\n  widgetKey,\n  label,\n  value,\n  min,\n  max,\n  step,\n  vertical,\n  disabled,\n  hidden,\n  runNb,\n  url_key,\n}: RangeProps) {\n  let minValue = 0;\n  let maxValue = 100;\n  let stepValue = 1;\n  if (min) {\n    minValue = min;\n  }\n  if (max) {\n    maxValue = max;\n  }\n  if (step) {\n    stepValue = step;\n  }\n\n  const dispatch = useDispatch();\n  const [updated, userInteraction] = useState(false);\n  const [searchParams] = useSearchParams();\n\n  useEffect(() => {\n    if (url_key !== undefined && url_key !== \"\") {\n      const urlValue = searchParams\n        .get(url_key)\n        ?.split(\",\")\n        .map((i) => parseFloat(i));\n      if (\n        !updated &&\n        urlValue !== undefined &&\n        urlValue.length === 2 &&\n        urlValue[0] !== undefined &&\n        !isNaN(urlValue[0]) &&\n        urlValue[1] !== undefined &&\n        !isNaN(urlValue[1]) &&\n        urlValue[0] <= urlValue[1] &&\n        urlValue[0] >= minValue &&\n        urlValue[1] <= maxValue\n      ) {\n        dispatch(\n          setWidgetUrlValue({\n            key: widgetKey,\n            value: urlValue as [number, number],\n          })\n        );\n        dispatch(setUrlValuesUsed(true));\n      }\n    }\n  }, [dispatch, maxValue, minValue, searchParams, updated, url_key, widgetKey]);\n\n  const values =\n    value != null && value !== undefined && value.length === 2\n      ? value\n      : [minValue, maxValue];\n\n  return (\n    <div className=\"form-group mb-3\" style={{ display: hidden ? \"none\" : \"\" }}>\n      <label\n        htmlFor={`range-slider-${label}`}\n        style={{ color: disabled ? \"#555\" : \"#212529\" }}\n      >\n        {label}\n      </label>\n\n      <div\n        style={{\n          paddingTop: \"12px\",\n          display: \"flex\",\n          justifyContent: \"center\",\n          flexWrap: \"wrap\",\n        }}\n      >\n        <Range\n          disabled={disabled}\n          values={values}\n          step={stepValue}\n          min={minValue}\n          max={maxValue}\n          onChange={(values) => {\n            userInteraction(true);\n            dispatch(clearWidgetsUrlValues());\n            dispatch(\n              setWidgetValue({\n                key: widgetKey,\n                value: values as [number, number],\n              })\n            );\n          }}\n          onFinalChange={(values) => {\n            runNb();\n          }}\n          renderTrack={({ props, children }) => (\n            <div\n              onMouseDown={props.onMouseDown}\n              onTouchStart={props.onTouchStart}\n              style={{\n                ...props.style,\n                height: \"36px\",\n                display: \"flex\",\n                width: \"100%\",\n              }}\n            >\n              <div\n                ref={props.ref}\n                style={{\n                  height: \"5px\",\n                  width: \"100%\",\n                  borderRadius: \"4px\",\n                  background: getTrackBackground({\n                    values,\n                    colors: [\n                      \"#ccc\",\n                      disabled ? \"rgba(0, 0, 0, 0.3)\" : \"#2684ff\",\n                      \"#ccc\",\n                    ],\n                    min: minValue,\n                    max: maxValue,\n                  }),\n                  alignSelf: \"center\",\n                }}\n              >\n                {children}\n\n                <div\n                  style={{\n                    display: \"inline-block\",\n                    width: \"100%\",\n                    fontSize: \"12px\",\n                    paddingTop: \"13px\",\n                  }}\n                >\n                  <div style={{ float: \"left\" }}>{minValue}</div>\n                  <div style={{ float: \"right\" }}>{maxValue}</div>\n                </div>\n              </div>\n            </div>\n          )}\n          renderThumb={({ index, props, isDragged }) => (\n            <div\n              {...props}\n              style={{\n                ...props.style,\n                height: \"18px\",\n                width: \"18px\",\n                border: \"None !important\",\n                borderRadius: \"4px\",\n                backgroundColor: \"#FFF\",\n                display: \"flex\",\n                justifyContent: \"center\",\n                alignItems: \"center\",\n                boxShadow: \"0px 2px 6px #AAA\",\n                outline: \"none\",\n              }}\n            >\n              <div\n                style={{\n                  position: \"absolute\",\n                  top: \"-24px\",\n                  color: \"#fff\",\n                  fontWeight: \"bold\",\n                  fontSize: \"12px\",\n                  fontFamily: \"Arial,Helvetica Neue,Helvetica,sans-serif\",\n                  padding: \"2px\",\n                  borderRadius: \"3px\",\n                  backgroundColor: disabled ? \"rgba(0, 0, 0, 0.3)\" : \"#2684ff\",\n                }}\n              >\n                {values[index]}\n              </div>\n              <div\n                style={{\n                  height: \"12px\",\n                  width: \"3px\",\n                  backgroundColor: isDragged ? \"#2684ff\" : \"#CCC\",\n                }}\n              />\n            </div>\n          )}\n        />\n      </div>\n    </div>\n  );\n}\n",
         "/* eslint-disable jsx-a11y/anchor-is-valid */\nimport React, { useEffect, useState } from \"react\";\nimport { useDispatch } from \"react-redux\";\nimport { useSearchParams } from \"react-router-dom\";\nimport Select, { MultiValue } from \"react-select\";\nimport {\n  setUrlValuesUsed,\n  setWidgetUrlValue,\n  setWidgetValue,\n} from \"../slices/notebooksSlice\";\n\ntype SingleOption = { value: string; label: string };\ntype MultiOption = MultiValue<{ value: string; label: string } | undefined>;\n\nexport function isSingleOption(\n  options: SingleOption | MultiOption\n): options is SingleOption {\n  return (options as SingleOption).value !== undefined;\n}\n\ntype SelectProps = {\n  widgetKey: string;\n  label: string | null;\n  value: string | string[] | null;\n  choices: string[];\n  multi: boolean | undefined;\n  disabled: boolean;\n  hidden: boolean;\n  runNb: () => void;\n  url_key: string;\n};\n\nexport default function SelectWidget({\n  widgetKey,\n  label,\n  value,\n  choices,\n  multi,\n  disabled,\n  hidden,\n  runNb,\n  url_key,\n}: SelectProps) {\n  const dispatch = useDispatch();\n  const [updated, userInteraction] = useState(false);\n\n  const selectStyles = {\n    menu: (base: any) => ({\n      ...base,\n      zIndex: 100,\n    }),\n  };\n\n  const [searchParams] = useSearchParams();\n  useEffect(() => {\n    if (url_key !== undefined && url_key !== \"\") {\n      const urlValue = searchParams.get(url_key);\n      if (!updated && urlValue !== undefined && urlValue !== null) {\n        if (multi) {\n          const arr = urlValue.split(\",\");\n          if (arr) {\n            dispatch(\n              setWidgetUrlValue({\n                key: widgetKey,\n                value: arr.filter((a) => choices.includes(a)),\n              })\n            );\n            dispatch(setUrlValuesUsed(true));\n          }\n        } else {\n          if (choices.includes(urlValue)) {\n            dispatch(\n              setWidgetUrlValue({\n                key: widgetKey,\n                value: urlValue,\n              })\n            );\n            dispatch(setUrlValuesUsed(true));\n          }\n        }\n      }\n    }\n  }, [choices, dispatch, multi, searchParams, updated, url_key, widgetKey]);\n\n  let selectedValue: SingleOption = { value: \"\", label: \"\" };\n  let selectedValues: SingleOption[] = [{ value: \"\", label: \"\" }];\n\n  let options: { value: string; label: string }[] = choices.map((choice) => {\n    if (value && choice === value && !multi) {\n      selectedValue = { value: choice, label: choice };\n    }\n    return { value: choice, label: choice };\n  });\n\n  if (multi) {\n    selectedValues = [];\n    choices.map((choice) => {\n      if (value && value.includes(choice) && multi) {\n        selectedValues.push({ value: choice, label: choice });\n      }\n      return { value: choice, label: choice };\n    });\n  }\n\n  useEffect(() => {\n    if (!updated) return;\n    runNb();\n    // const timeOutId = setTimeout(() => {\n    //   // console.log(\"run from select\");\n    //   runNb();\n    // }, RUN_DELAY_FAST);\n    // return () => clearTimeout(timeOutId);\n    // eslint-disable-next-line react-hooks/exhaustive-deps\n  }, [value]);\n\n  return (\n    <div className=\"form-group mb-3\" style={{ display: hidden ? \"none\" : \"\" }}>\n      <label\n        htmlFor={`select-${label}`}\n        style={{ color: disabled ? \"#555\" : \"#212529\" }}\n      >\n        {label}\n      </label>\n      <Select\n        id={`select-${label}`}\n        isDisabled={disabled}\n        name={label ? label : \"Select\"}\n        styles={selectStyles}\n        value={multi ? selectedValues : selectedValue}\n        options={options}\n        isMulti={multi}\n        onChange={(e) => {\n          if (e) {\n            userInteraction(true);\n            if (isSingleOption(e)) {\n              dispatch(setWidgetValue({ key: widgetKey, value: e.value }));\n            } else {\n              // console.log({ msg: \"values\", values: e.values() });\n              const vs = Array.from(e.values()).filter(\n                (i) => i !== undefined\n              ) as { label: string; value: string }[];\n              // console.log({\n              //   key: widgetKey,\n              // });\n              dispatch(\n                setWidgetValue({\n                  key: widgetKey,\n                  value: vs.map((i) => i.value) as string[],\n                })\n              );\n            }\n          }\n        }}\n      />\n    </div>\n  );\n}\n",
         "import React, { useEffect, useState } from \"react\";\nimport { useDispatch } from \"react-redux\";\nimport {\n  setUrlValuesUsed,\n  setWidgetUrlValue,\n  setWidgetValue,\n} from \"../slices/notebooksSlice\";\nimport { Range, getTrackBackground } from \"react-range\";\nimport { useSearchParams } from \"react-router-dom\";\n\ntype SliderProps = {\n  widgetKey: string;\n  label: string | null;\n  value: number | null;\n  min: number | null;\n  max: number | null;\n  step: number | null;\n  vertical: boolean | null;\n  disabled: boolean;\n  hidden: boolean;\n  runNb: () => void;\n  url_key: string;\n};\n\nexport default function SliderWidget({\n  widgetKey,\n  label,\n  value,\n  min,\n  max,\n  step,\n  vertical,\n  disabled,\n  hidden,\n  runNb,\n  url_key,\n}: SliderProps) {\n  const dispatch = useDispatch();\n  const [updated, userInteraction] = useState(false);\n\n  let minValue = 0;\n  let maxValue = 100;\n  let stepValue = 1;\n  if (min) {\n    minValue = min;\n  }\n  if (max) {\n    maxValue = max;\n  }\n  if (step) {\n    stepValue = step;\n  }\n  const [searchParams] = useSearchParams();\n  useEffect(() => {\n    if (url_key !== undefined && url_key !== \"\") {\n      const urlValue = searchParams.get(url_key);\n      if (\n        !updated &&\n        urlValue !== undefined &&\n        urlValue !== null &&\n        !isNaN(parseFloat(urlValue)) &&\n        parseFloat(urlValue) >= minValue &&\n        parseFloat(urlValue) <= maxValue\n      ) {\n        dispatch(\n          setWidgetUrlValue({\n            key: widgetKey,\n            value: parseFloat(urlValue),\n          })\n        );\n        dispatch(setUrlValuesUsed(true));\n      }\n    }\n  }, [dispatch, maxValue, minValue, searchParams, updated, url_key, widgetKey]);\n\n  const vals: number[] = [value !== null ? value : maxValue];\n\n  return (\n    <div className=\"form-group mb-3\" style={{ display: hidden ? \"none\" : \"\" }}>\n      <label\n        htmlFor={`slider-${label}`}\n        style={{ color: disabled ? \"#555\" : \"#212529\" }}\n      >\n        {label}\n      </label>\n\n      <div\n        style={{\n          paddingTop: \"12px\",\n          display: \"flex\",\n          justifyContent: \"center\",\n          flexWrap: \"wrap\",\n        }}\n      >\n        <Range\n          disabled={disabled}\n          values={vals}\n          step={stepValue}\n          min={minValue}\n          max={maxValue}\n          onChange={(values) => {\n            userInteraction(true);\n            dispatch(setWidgetValue({ key: widgetKey, value: values[0] }));\n          }}\n          onFinalChange={(values) => {\n            runNb();\n          }}\n          renderTrack={({ props, children }) => (\n            <div\n              onMouseDown={props.onMouseDown}\n              onTouchStart={props.onTouchStart}\n              style={{\n                ...props.style,\n                height: \"36px\",\n                display: \"flex\",\n                width: \"100%\",\n              }}\n            >\n              <div\n                ref={props.ref}\n                style={{\n                  height: \"5px\",\n                  width: \"100%\",\n                  borderRadius: \"4px\",\n                  background: getTrackBackground({\n                    values: vals,\n                    colors: [\n                      disabled ? \"rgba(0, 0, 0, 0.3)\" : \"#2684ff\", // \"#548BF4\",\n                      \"#ccc\",\n                    ],\n                    min: minValue,\n                    max: maxValue,\n                  }),\n                  alignSelf: \"center\",\n                }}\n              >\n                {children}\n\n                <div\n                  style={{\n                    display: \"inline-block\",\n                    width: \"100%\",\n                    fontSize: \"12px\",\n                    paddingTop: \"13px\",\n                  }}\n                >\n                  <div style={{ float: \"left\" }}>{minValue}</div>\n                  <div style={{ float: \"right\" }}>{maxValue}</div>\n                </div>\n              </div>\n            </div>\n          )}\n          renderThumb={({ props, isDragged }) => (\n            <div\n              {...props}\n              style={{\n                ...props.style,\n                height: \"18px\",\n                width: \"18px\",\n                border: \"None\",\n                borderRadius: \"4px\",\n                backgroundColor: \"#FFF\",\n                display: \"flex\",\n                justifyContent: \"center\",\n                alignItems: \"center\",\n                boxShadow: \"0px 2px 6px #AAA\",\n                outline: \"none\",\n              }}\n            >\n              <div\n                style={{\n                  position: \"absolute\",\n                  top: \"-24px\",\n                  color: \"#fff\",\n                  fontWeight: \"bold\",\n                  fontSize: \"12px\",\n                  fontFamily: \"Arial,Helvetica Neue,Helvetica,sans-serif\",\n                  padding: \"2px\",\n                  borderRadius: \"3px\",\n                  backgroundColor: disabled ? \"rgba(0, 0, 0, 0.3)\" : \"#2684ff\",\n                }}\n              >\n                {vals[0]}\n              </div>\n              <div\n                style={{\n                  height: \"12px\",\n                  width: \"3px\",\n                  backgroundColor: isDragged ? \"#2684ff\" : \"#CCC\",\n                }}\n              />\n            </div>\n          )}\n        />\n      </div>\n    </div>\n  );\n}\n",
         "import React, { useEffect, useState } from \"react\";\nimport { useDispatch, useSelector } from \"react-redux\";\n\nimport axios, { AxiosProgressEvent } from \"axios\";\n\nimport { setWidgetValue } from \"../slices/notebooksSlice\";\n\nimport { FilePond, registerPlugin } from \"react-filepond\";\nimport FilePondPluginImageExifOrientation from \"filepond-plugin-image-exif-orientation\";\nimport FilePondPluginImagePreview from \"filepond-plugin-image-preview\";\nimport FilePondPluginFileValidateSize from \"filepond-plugin-file-validate-size\";\nimport {\n  deleteUserFileUploaded,\n  fetchStorageType,\n  getStorageType,\n  userFileUploaded,\n} from \"../slices/appSlice\";\nimport { toast } from \"react-toastify\";\nimport { getSiteId } from \"../slices/sitesSlice\";\nimport { getSessionId } from \"../utils\";\n\nregisterPlugin(\n  FilePondPluginImageExifOrientation,\n  FilePondPluginImagePreview,\n  FilePondPluginFileValidateSize\n);\n\ntype FileProps = {\n  widgetKey: string;\n  label: string | null;\n  maxFileSize: string | null;\n  disabled: boolean;\n  hidden: boolean;\n  value: string[];\n  runNb: () => void;\n};\n\nexport default function FileWidget({\n  widgetKey,\n  label,\n  maxFileSize,\n  disabled,\n  hidden,\n  value,\n  runNb,\n}: FileProps) {\n  const dispatch = useDispatch();\n  const [updated, userInteraction] = useState(false);\n  const storageType = useSelector(getStorageType);\n  const siteId = useSelector(getSiteId);\n  const sessionId = useSelector(getSessionId);\n\n  let fileSizeLimit = \"100MB\";\n  if (maxFileSize) {\n    fileSizeLimit = maxFileSize;\n  }\n  useEffect(() => {\n    if (updated && value !== undefined && value.length === 2) {\n      //console.log(\"run from file\");\n      runNb();\n    }\n    // eslint-disable-next-line react-hooks/exhaustive-deps\n  }, [value]);\n\n  useEffect(() => {\n    dispatch(fetchStorageType());\n  }, [dispatch]);\n\n  const mediaServerActions = {\n    url: `${axios.defaults.baseURL}/api/v1/fp`,\n    process: \"/process/\",\n    revert: async (\n      uniqueFileId: any,\n      load: () => void,\n      error: (arg0: string) => void\n    ) => {\n      try {\n        await axios.delete(`${axios.defaults.baseURL}/api/v1/fp/revert`, {\n          data: uniqueFileId,\n        });\n        dispatch(setWidgetValue({ key: widgetKey, value: [] }));\n        // Should call the load method when done, no parameters required\n        load();\n      } catch (e) {\n        // Can call the error method if something is wrong, should exit after\n        error(\"Problem with uploaded file removal\");\n      }\n    },\n  };\n  const s3ServerActions = {\n    process: (\n      fieldName: string,\n      file: { name: any; size: any },\n      metadata: any,\n      load: (arg0: any) => void,\n      error: any,\n      progress: (arg0: boolean, arg1: any, arg2: number) => void,\n      abort: () => void\n    ) => {\n      const abortController = new AbortController();\n\n      axios\n        .get(\n          `/api/v1/nb-file-put/${siteId}/${sessionId}/${file.name}/${file.size}`\n        )\n        .then((response) => {\n          const { url } = response.data;\n\n          let token = axios.defaults.headers.common[\"Authorization\"];\n\n          delete axios.defaults.headers.common[\"Authorization\"];\n\n          const config = {\n            onUploadProgress: (progressEvent: AxiosProgressEvent) => {\n              progress(\n                progressEvent.total !== undefined,\n                progressEvent.loaded,\n                progressEvent.total as number\n              );\n            },\n          };\n\n          axios\n            .put(url, file, {\n              headers: {\n                \"Content-Type\": \"\",\n              },\n              onUploadProgress: config.onUploadProgress,\n              signal: abortController.signal,\n            })\n            .then((response) => {\n              // file uploaded\n              // set it as uploaded in filepond\n              load(file.name);\n              // save it in database\n              if (siteId !== undefined) {\n                dispatch(userFileUploaded(siteId, sessionId, file.name));\n              }\n            })\n            .catch((error) => {\n              toast.error(\"Error when uploading new files\");\n            });\n\n          axios.defaults.headers.common[\"Authorization\"] = token;\n        })\n        .catch((error) => {\n          toast.error(\"Cant upload new files\");\n        });\n\n      // Should expose an abort method so the request can be cancelled\n      return {\n        abort: () => {\n          // This function is entered if the user has tapped the cancel button\n          abortController.abort();\n          // Let FilePond know the request has been cancelled\n          abort();\n        },\n      };\n    },\n    revert: async (\n      uniqueFileId: any,\n      load: () => void,\n      error: (arg0: string) => void\n    ) => {\n      try {\n        if (siteId !== undefined) {\n          dispatch(deleteUserFileUploaded(siteId, sessionId, uniqueFileId));\n        }\n        // Should call the load method when done, no parameters required\n        load();\n      } catch (e) {\n        // Can call the error method if something is wrong, should exit after\n        error(\"Problem with uploaded file removal\");\n      }\n    },\n  };\n\n  return (\n    <div className=\"form-group mb-3\" style={{ display: hidden ? \"none\" : \"\" }}>\n      <label\n        htmlFor={`file-${label}`}\n        style={{ color: disabled ? \"#555\" : \"#212529\" }}\n      >\n        {label}\n      </label>\n      <div>\n        <FilePond\n          disabled={disabled}\n          maxFileSize={fileSizeLimit}\n          onprocessfile={(error, file) => {\n            userInteraction(true);\n            dispatch(\n              setWidgetValue({\n                key: widgetKey,\n                value: [file.filename, file.serverId],\n              })\n            );\n          }}\n          server={\n            storageType === \"media\" ? mediaServerActions : s3ServerActions\n          }\n          labelIdle='Drag & Drop your file or <span class=\"filepond--label-action\">Browse</span>'\n        />\n      </div>\n    </div>\n  );\n}\n",
         "import React, { useEffect, useState } from \"react\";\nimport { useDispatch } from \"react-redux\";\nimport { useSearchParams } from \"react-router-dom\";\nimport { setUrlValuesUsed, setWidgetUrlValue, setWidgetValue } from \"../slices/notebooksSlice\";\n\ntype TextProps = {\n  widgetKey: string;\n  label: string | null;\n  value: string | undefined;\n  rows: number | null;\n  disabled: boolean;\n  hidden: boolean;\n  runNb: () => void;\n  continuousUpdate: boolean;\n  url_key: string;\n  sanitize: boolean;\n};\n\nexport default function TextWidget({\n  widgetKey,\n  label,\n  value,\n  rows,\n  disabled,\n  hidden,\n  runNb,\n  continuousUpdate,\n  url_key,\n  sanitize,\n}: TextProps) {\n  const dispatch = useDispatch();\n  const [apply, showApply] = useState(false);\n  const [updated, userInteraction] = useState(false);\n  let rowsValue: number = rows ? rows : 1;\n\n  const sanitizeString = (input_string: string) => {\n    return input_string.replace(/[\"'(){}[\\]`^]/gim, \"\");\n  };\n\n  const [searchParams] = useSearchParams();\n  useEffect(() => {\n    if (url_key !== undefined && url_key !== \"\") {\n      const urlValue = searchParams.get(url_key);\n      if (!updated && urlValue !== undefined && urlValue !== null) {\n        dispatch(\n          setWidgetUrlValue({\n            key: widgetKey,\n            value: urlValue,\n          })\n        );\n        dispatch(setUrlValuesUsed(true));\n      }\n    }\n  }, [dispatch, searchParams, updated, url_key, widgetKey]);\n\n  return (\n    <div className=\"form-group mb-3\" style={{ display: hidden ? \"none\" : \"\" }}>\n      <label\n        htmlFor={`textarea-${label}`}\n        style={{ color: disabled ? \"#555\" : \"#212529\" }}\n      >\n        {label}\n      </label>\n      {rowsValue === 1 && (\n        <input\n          className=\"form-control\"\n          type=\"text\"\n          id={`text-${label}`}\n          value={value ? value : \"\"}\n          onChange={(e) => {\n            userInteraction(true);\n            showApply(true);\n            dispatch(\n              setWidgetValue({\n                key: widgetKey,\n                value: sanitize ? sanitizeString(e.target.value) : e.target.value,\n              })\n            );\n          }}\n          onKeyPress={(e) => {\n            if (e.key === \"Enter\") {\n              runNb();\n              showApply(false);\n              e.preventDefault();\n            }\n          }}\n          disabled={disabled}\n        />\n      )}\n      {rowsValue > 1 && (\n        <textarea\n          className=\"form-control\"\n          id={`text-area-${label}`}\n          rows={rowsValue}\n          value={value ? value : \"\"}\n          onChange={(e) => {\n            userInteraction(true);\n            showApply(true);\n            dispatch(\n              setWidgetValue({\n                key: widgetKey,\n                value: sanitize ? sanitizeString(e.target.value) : e.target.value,\n              })\n            );\n          }}\n          disabled={disabled}\n        />\n      )}\n\n      {apply && continuousUpdate && rowsValue === 1 && (\n        // <div\n        //   style={{\n        //     fontSize: \"0.7em\",\n        //     float: \"right\",\n        //     position: \"relative\",\n        //     top: \"0px\",\n        //     left: \"-5px\",\n        //     color: \"#2684ff\",\n        //   }}\n        // >\n        //   Press enter to apply\n        // </div>\n\n        <div\n          style={{\n            float: \"right\",\n            position: \"relative\",\n            top: \"2px\",\n            left: \"0px\",\n          }}\n        >\n          <button\n            className=\"btn btn-sm btn-outline-primary\"\n            onClick={(e) => {\n              runNb();\n              showApply(false);\n              e.preventDefault();\n            }}\n            style={{\n              fontSize: \"0.7em\",\n              border: \"none\",\n            }}\n          >\n            Press enter or click to apply\n          </button>\n        </div>\n      )}\n      {apply && continuousUpdate && rowsValue > 1 && (\n        <div\n          style={{\n            float: \"right\",\n            position: \"relative\",\n            top: \"2px\",\n            left: \"0px\",\n          }}\n        >\n          <button\n            className=\"btn btn-sm btn-outline-primary\"\n            onClick={(e) => {\n              runNb();\n              showApply(false);\n              e.preventDefault();\n            }}\n            style={{\n              fontSize: \"0.7em\",\n              border: \"none\",\n            }}\n          >\n            Apply\n          </button>\n        </div>\n      )}\n    </div>\n  );\n}\n",
         "/* eslint-disable import/no-cycle */\nimport { createSlice, PayloadAction } from \"@reduxjs/toolkit\";\nimport { RootState } from \"../store\";\n\nexport enum WebSocketState {\n  Connecting = \"Connecting\",\n  Connected = \"Connected\",\n  Unknown = \"Unknown\",\n  Disconnected = \"Disconnected\",\n}\n\nexport enum WorkerState {\n  Unknown = \"Unknown\",\n  Starting = \"Starting\",\n  Running = \"Running\",\n  Missing = \"Missing\",\n  Busy = \"Busy\",\n  Queued = \"Queued\",\n  MaxRunTimeReached = \"MaxRunTimeReached\",\n  MaxIdleTimeReached = \"MaxIdleTimeReached\",\n  UsageLimitReached = \"UsageLimitReached\",\n  //InstallPackages = \"InstallPackages\",\n}\n\nconst initialState = {\n  webSocketState: WebSocketState.Unknown,\n  workerState: WorkerState.Unknown,\n  workerId: undefined as undefined | number,\n  notebookSrc: \"\",\n  tryConnectCount: 0,\n};\n\nconst wsSlice = createSlice({\n  name: \"ws\",\n  initialState,\n  reducers: {\n    setWebSocketState(state, action: PayloadAction<WebSocketState>) {\n      state.webSocketState = action.payload;\n    },\n    setWorkerState(state, action: PayloadAction<WorkerState>) {\n      state.workerState = action.payload;\n    },\n    setWorkerId(state, action: PayloadAction<undefined | number>) {\n      state.workerId = action.payload;\n    },\n    setNotebookSrc(state, action: PayloadAction<string>) {\n      state.notebookSrc = action.payload;\n    },\n    increaseTryConnectCount(state) {\n      state.tryConnectCount += 1;\n    },\n    resetTryConnectCount(state) {\n      state.tryConnectCount = 0;\n    },\n  },\n});\n\nexport default wsSlice.reducer;\n\nexport const {\n  setWebSocketState,\n  setWorkerState,\n  setWorkerId,\n  setNotebookSrc,\n  increaseTryConnectCount,\n  resetTryConnectCount,\n} = wsSlice.actions;\n\nexport const getWebSocketState = (state: RootState) => state.ws.webSocketState;\nexport const getWorkerState = (state: RootState) => state.ws.workerState;\nexport const getWorkerId = (state: RootState) => state.ws.workerId;\nexport const getNotebookSrc = (state: RootState) => state.ws.notebookSrc;\nexport const getTryConnectCount = (state: RootState) =>\n  state.ws.tryConnectCount;\n\nexport const runNotebook = (widgets_params: string) => {\n  return {\n    purpose: \"run-notebook\",\n    widgets: widgets_params,\n  };\n};\n\nexport const saveNotebook = () => {\n  return {\n    purpose: \"save-notebook\",\n  };\n};\n\nexport const displayNotebook = (taskId: number) => {\n  return {\n    purpose: \"display-notebook\",\n    taskId,\n  };\n};\n\nexport const downloadHTML = () => {\n  return {\n    purpose: \"download-html\",\n  };\n};\n\nexport const downloadPDF = () => {\n  return {\n    purpose: \"download-pdf\",\n  };\n};\n",
         "/* eslint-disable jsx-a11y/anchor-is-valid */\nimport React from \"react\";\n\nimport ReactMarkdown from \"react-markdown\";\nimport rehypeHighlight from \"rehype-highlight\";\nimport remarkGfm from \"remark-gfm\";\nimport emoji from \"remark-emoji\";\nimport rehypeRaw from \"rehype-raw\";\n\ntype MarkdownProps = {\n  value: string;\n  disabled: boolean;\n};\n\nexport default function MarkdownWidget({ value, disabled }: MarkdownProps) {\n  return (\n    <div\n      className=\"form-group mb-3\"\n      style={{ color: disabled ? \"#555\" : \"#212529\" }}\n    >\n      <ReactMarkdown\n        rehypePlugins={[remarkGfm, rehypeHighlight, emoji, rehypeRaw]}\n      >\n        {value}\n      </ReactMarkdown>\n    </div>\n  );\n}\n",
         "import React, { createContext, useEffect } from \"react\";\nimport { useDispatch } from \"react-redux\";\nimport {\n  getSelectedNotebookId,\n  hideWidgets,\n  isStaticNotebook,\n  updateWidgetsParams,\n  initWidgets,\n  fetchNotebook,\n  updateTitle,\n  updateShowCode,\n  setWidgetsInitialized,\n} from \"../slices/notebooksSlice\";\nimport {\n  setNotebookSrc,\n  setWebSocketState,\n  setWorkerState,\n  setWorkerId,\n  WebSocketState,\n  WorkerState,\n  resetTryConnectCount,\n  increaseTryConnectCount,\n} from \"../slices/wsSlice\";\n\nimport { useSelector } from \"react-redux\";\nimport { getSessionId, handleDownload } from \"../utils\";\nimport { setExportingToPDF } from \"../slices/tasksSlice\";\nimport { getSiteId, setSiteStatus, SiteStatus } from \"../slices/sitesSlice\";\nimport { getToken } from \"../slices/authSlice\";\n\nconst WebSocketContext = createContext(undefined as any);\n\nexport { WebSocketContext };\n\nlet wsServer = \"ws://127.0.0.1:8000\";\nlet localServer = true;\nif (process.env.REACT_APP_SERVER_WS) {\n  wsServer = process.env.REACT_APP_SERVER_WS;\n  localServer = false;\n} else {\n  if (window.location.origin === \"http://localhost:3000\") {\n    wsServer = \"ws://127.0.0.1:8000\";\n    localServer = true;\n  } else {\n    wsServer = window.location.origin\n      .replace(\"http://\", \"ws://\")\n      .replace(\"https://\", \"wss://\");\n    localServer = false;\n  }\n}\n\nif (window.location.origin.endsWith(\"hf.space\")) {\n  wsServer = window.location.origin\n    .replace(\"http://\", \"ws://\")\n    .replace(\"https://\", \"wss://\");\n  localServer = false;\n}\n\nconst MAX_CONNECT_COUNT = 5;\nlet connectCounter = 0;\nlet globalConnection: WebSocket | undefined = undefined;\n\nexport default function WebSocketProvider({\n  children,\n}: {\n  children: JSX.Element;\n}) {\n  console.log(\"WebSocketProvider\");\n\n  const dispatch = useDispatch();\n  const siteId = useSelector(getSiteId);\n  const selectedNotebookId = useSelector(getSelectedNotebookId);\n  const token = useSelector(getToken);\n  const isStatic = useSelector(isStaticNotebook);\n\n  let connection: WebSocket | undefined = undefined;\n  let workerState = \"Unknown\" as WorkerState;\n\n  useEffect(() => {\n    connectCounter = 0;\n    // returned function will be called on component unmount\n    return () => {\n      connectCounter = MAX_CONNECT_COUNT + 1;\n      globalConnection?.close();\n    };\n    // eslint-disable-next-line react-hooks/exhaustive-deps\n  }, []);\n\n  const sendMessage = (payload: string) => {\n    if (connection !== undefined && connection.readyState === connection.OPEN) {\n      connection.send(payload);\n    }\n  };\n\n  function onOpen(event: any): void {\n    dispatch(resetTryConnectCount());\n    sendMessage(\n      JSON.stringify({\n        purpose: \"server-address\",\n        address: wsServer,\n      })\n    );\n    dispatch(setWebSocketState(WebSocketState.Connected));\n    ping();\n  }\n\n  function onMessage(event: any): void {\n    // console.log(\"reveived from server\", event.data);\n\n    const response = JSON.parse(event.data);\n    if (\"purpose\" in response) {\n      if (response.purpose === \"worker-state\") {\n        console.log(\"worker-state\", response.state);\n        workerState = response.state;\n\n        dispatch(setWorkerState(response.state));\n        dispatch(setWorkerId(response.workerId));\n\n        if (\n          workerState === WorkerState.MaxIdleTimeReached ||\n          workerState === WorkerState.MaxRunTimeReached\n        ) {\n          connection?.close();\n        }\n      } else if (response.purpose === \"executed-notebook\") {\n        //console.log(response?.reloadNotebook, selectedNotebookId);\n        if (response?.reloadNotebook && selectedNotebookId !== undefined) {\n          //console.log(\"reload notebook ...........................\");\n          dispatch(fetchNotebook(siteId, selectedNotebookId));\n        }\n        dispatch(setNotebookSrc(response.body));\n        // } else if (response.purpose === \"saved-notebook\") {\n        //   if (selectedNotebookId !== undefined) {\n        //     dispatch(fetchExecutionHistory(selectedNotebookId, false));\n        //   }\n      } else if (response.purpose === \"update-widgets\") {\n        dispatch(updateWidgetsParams(response));\n      } else if (response.purpose === \"hide-widgets\") {\n        dispatch(hideWidgets(response));\n      } else if (response.purpose === \"init-widgets\") {\n        dispatch(initWidgets(response));\n        dispatch(setWidgetsInitialized(true));\n      } else if (response.purpose === \"update-title\") {\n        dispatch(updateTitle(response.title));\n      } else if (response.purpose === \"update-show-code\") {\n        dispatch(updateShowCode(response.showCode));\n      } else if (\n        response.purpose === \"download-html\" ||\n        response.purpose === \"download-pdf\"\n      ) {\n        if (response.url && response.filename) {\n          dispatch(setExportingToPDF(false));\n          handleDownload(response.url, response.filename);\n        }\n      }\n    }\n  }\n\n  function onError(event: any): void {\n    dispatch(setWebSocketState(WebSocketState.Disconnected));\n    dispatch(setWorkerState(WorkerState.Unknown));\n  }\n\n  function onClose(event: any): void {\n    dispatch(setWebSocketState(WebSocketState.Disconnected));\n    connection = undefined;\n    if (\n      workerState !== WorkerState.MaxIdleTimeReached &&\n      workerState !== WorkerState.MaxRunTimeReached\n    ) {\n      dispatch(setWorkerState(WorkerState.Unknown));\n      dispatch(setWorkerId(undefined));\n      if (connectCounter < MAX_CONNECT_COUNT) {\n        setTimeout(() => connect(), 5000);\n      }\n    }\n  }\n\n  function ping(): void {\n    sendMessage(\n      JSON.stringify({\n        purpose: \"worker-ping\",\n      })\n    );\n    if (connection !== undefined && connection.readyState === connection.OPEN) {\n      setTimeout(() => ping(), 10000);\n    }\n  }\n\n  function connect() {\n    if (\n      (localServer || !isStatic) &&\n      selectedNotebookId !== undefined &&\n      connection === undefined &&\n      workerState !== WorkerState.MaxIdleTimeReached &&\n      workerState !== WorkerState.MaxRunTimeReached &&\n      connectCounter < MAX_CONNECT_COUNT\n    ) {\n      console.log(\"WS connect ...\" + workerState + \" \" + connectCounter);\n      dispatch(increaseTryConnectCount());\n      let url = `${wsServer}/ws/client/${selectedNotebookId}/${getSessionId()}/`;\n      if (token !== undefined && token !== null && token !== \"\") {\n        url += `?token=${token}`;\n      }\n      connection = new WebSocket(url);\n      connection.onopen = onOpen;\n      connection.onmessage = onMessage;\n      connection.onerror = onError;\n      connection.onclose = onClose;\n      connectCounter += 1;\n\n      globalConnection = connection;\n      if (connectCounter >= MAX_CONNECT_COUNT) {\n        dispatch(setSiteStatus(SiteStatus.NetworkError));\n      }\n    }\n  }\n  connect();\n\n  const ws = {\n    sendMessage,\n  };\n\n  return (\n    <WebSocketContext.Provider value={ws}>{children}</WebSocketContext.Provider>\n  );\n}\n",
-        "import React, { useEffect } from \"react\";\nimport { useDispatch, useSelector } from \"react-redux\";\nimport { getSessionId, handleDownload } from \"../utils\";\nimport {\n  WorkerState,\n  WebSocketState,\n  getWebSocketState,\n  getWorkerState,\n  getTryConnectCount,\n} from \"../slices/wsSlice\";\nimport { getSiteId, setSiteStatus, SiteStatus } from \"../slices/sitesSlice\";\nimport axios from \"axios\";\nimport { exportToPDF, setExportingToPDF } from \"../slices/tasksSlice\";\nimport { setShowShareDialog } from \"../slices/appSlice\";\n\ntype Props = {\n  allowDownload: boolean;\n  waiting: boolean;\n  continuousUpdate: boolean;\n  staticNotebook: boolean;\n  notebookId: number;\n  notebookPath: string;\n  notebookTitle: string;\n  runDownloadHTML: () => void;\n  runDownloadPDF: () => void;\n};\n\nexport default function StatusBar({\n  allowDownload,\n  waiting,\n  continuousUpdate,\n  staticNotebook,\n  notebookId,\n  notebookPath,\n  notebookTitle,\n  runDownloadHTML,\n  runDownloadPDF,\n}: Props) {\n  const dispatch = useDispatch();\n  const wsStatus = useSelector(getWebSocketState);\n  const workerState = useSelector(getWorkerState);\n  const tryConnectCount = useSelector(getTryConnectCount);\n  const siteId = useSelector(getSiteId);\n\n  useEffect(() => {\n    if (tryConnectCount >= 5) {\n      dispatch(setSiteStatus(SiteStatus.LostConnection));\n    }\n  }, [dispatch, tryConnectCount]);\n\n  let wifiColor = \"orange\";\n  if (wsStatus === WebSocketState.Connected) {\n    wifiColor = \"green\";\n  } else if (\n    wsStatus === WebSocketState.Disconnected ||\n    wsStatus === WebSocketState.Unknown\n  ) {\n    wifiColor = \"red\";\n  }\n\n  let workerColor = \"orange\";\n  if (workerState === WorkerState.Running || workerState === WorkerState.Busy) {\n    workerColor = \"green\";\n  } else if (\n    workerState === WorkerState.Missing ||\n    workerState === WorkerState.Unknown\n  ) {\n    workerColor = \"red\";\n  }\n\n  return (\n    <div style={{ paddingBottom: \"25px\" }}>\n      {notebookId !== undefined && !staticNotebook && (\n        <>\n          <span title={`WebSocket: ${wsStatus}`}>\n            <svg\n              xmlns=\"http://www.w3.org/2000/svg\"\n              width=\"16\"\n              height=\"16\"\n              fill={wifiColor}\n              className=\"bi bi-wifi\"\n              viewBox=\"0 0 16 16\"\n            >\n              <path d=\"M15.384 6.115a.485.485 0 0 0-.047-.736A12.444 12.444 0 0 0 8 3C5.259 3 2.723 3.882.663 5.379a.485.485 0 0 0-.048.736.518.518 0 0 0 .668.05A11.448 11.448 0 0 1 8 4c2.507 0 4.827.802 6.716 2.164.205.148.49.13.668-.049z\" />\n              <path d=\"M13.229 8.271a.482.482 0 0 0-.063-.745A9.455 9.455 0 0 0 8 6c-1.905 0-3.68.56-5.166 1.526a.48.48 0 0 0-.063.745.525.525 0 0 0 .652.065A8.46 8.46 0 0 1 8 7a8.46 8.46 0 0 1 4.576 1.336c.206.132.48.108.653-.065zm-2.183 2.183c.226-.226.185-.605-.1-.75A6.473 6.473 0 0 0 8 9c-1.06 0-2.062.254-2.946.704-.285.145-.326.524-.1.75l.015.015c.16.16.407.19.611.09A5.478 5.478 0 0 1 8 10c.868 0 1.69.201 2.42.56.203.1.45.07.61-.091l.016-.015zM9.06 12.44c.196-.196.198-.52-.04-.66A1.99 1.99 0 0 0 8 11.5a1.99 1.99 0 0 0-1.02.28c-.238.14-.236.464-.04.66l.706.706a.5.5 0 0 0 .707 0l.707-.707z\" />\n            </svg>\n          </span>{\" \"}\n          <span title={`Worker: ${workerState}\\nSession Id: ${getSessionId()}`}>\n            <svg\n              xmlns=\"http://www.w3.org/2000/svg\"\n              width=\"16\"\n              height=\"16\"\n              fill={workerColor}\n              className=\"bi bi-cpu\"\n              viewBox=\"0 0 16 16\"\n            >\n              <path d=\"M5 0a.5.5 0 0 1 .5.5V2h1V.5a.5.5 0 0 1 1 0V2h1V.5a.5.5 0 0 1 1 0V2h1V.5a.5.5 0 0 1 1 0V2A2.5 2.5 0 0 1 14 4.5h1.5a.5.5 0 0 1 0 1H14v1h1.5a.5.5 0 0 1 0 1H14v1h1.5a.5.5 0 0 1 0 1H14v1h1.5a.5.5 0 0 1 0 1H14a2.5 2.5 0 0 1-2.5 2.5v1.5a.5.5 0 0 1-1 0V14h-1v1.5a.5.5 0 0 1-1 0V14h-1v1.5a.5.5 0 0 1-1 0V14h-1v1.5a.5.5 0 0 1-1 0V14A2.5 2.5 0 0 1 2 11.5H.5a.5.5 0 0 1 0-1H2v-1H.5a.5.5 0 0 1 0-1H2v-1H.5a.5.5 0 0 1 0-1H2v-1H.5a.5.5 0 0 1 0-1H2A2.5 2.5 0 0 1 4.5 2V.5A.5.5 0 0 1 5 0zm-.5 3A1.5 1.5 0 0 0 3 4.5v7A1.5 1.5 0 0 0 4.5 13h7a1.5 1.5 0 0 0 1.5-1.5v-7A1.5 1.5 0 0 0 11.5 3h-7zM5 6.5A1.5 1.5 0 0 1 6.5 5h3A1.5 1.5 0 0 1 11 6.5v3A1.5 1.5 0 0 1 9.5 11h-3A1.5 1.5 0 0 1 5 9.5v-3zM6.5 6a.5.5 0 0 0-.5.5v3a.5.5 0 0 0 .5.5h3a.5.5 0 0 0 .5-.5v-3a.5.5 0 0 0-.5-.5h-3z\" />\n            </svg>\n          </span>\n        </>\n      )}\n      {workerState === WorkerState.Busy && (\n        <span title=\"Worker is busy\">\n          {\" \"}\n          <svg\n            xmlns=\"http://www.w3.org/2000/svg\"\n            width=\"16\"\n            height=\"16\"\n            fill=\"green\"\n            className=\"bi bi-activity\"\n            viewBox=\"0 0 16 16\"\n          >\n            <path\n              fillRule=\"evenodd\"\n              d=\"M6 2a.5.5 0 0 1 .47.33L10 12.036l1.53-4.208A.5.5 0 0 1 12 7.5h3.5a.5.5 0 0 1 0 1h-3.15l-1.88 5.17a.5.5 0 0 1-.94 0L6 3.964 4.47 8.171A.5.5 0 0 1 4 8.5H.5a.5.5 0 0 1 0-1h3.15l1.88-5.17A.5.5 0 0 1 6 2Z\"\n            />\n          </svg>\n        </span>\n      )}\n      <div style={{ float: \"right\" }}>\n        {allowDownload && (\n          <div\n            className=\"dropdown mx-2 btn-group\"\n            style={{\n              //display: \"inline\",\n              // width: \"47%\",\n              // float: continuousUpdate ? \"left\" : \"right\",\n            }}\n          >\n            <button\n              className=\"btn btn-sm btn-primary dropdown-toggle\"\n              // style={{ margin: \"0px\", width: \"100%\" }}\n              type=\"button\"\n              data-bs-toggle=\"dropdown\"\n              disabled={waiting}\n            >\n              <svg\n                xmlns=\"http://www.w3.org/2000/svg\"\n                width=\"14\"\n                height=\"14\"\n                viewBox=\"0 0 24 24\"\n                strokeWidth=\"2\"\n                stroke=\"currentColor\"\n                fill=\"none\"\n                strokeLinecap=\"round\"\n                strokeLinejoin=\"round\"\n                style={{ paddingBottom: \"1px\" }}\n              >\n                <path stroke=\"none\" d=\"M0 0h24v24H0z\" fill=\"none\"></path>\n                <path d=\"M4 17v2a2 2 0 0 0 2 2h12a2 2 0 0 0 2 -2v-2\"></path>\n                <path d=\"M7 11l5 5l5 -5\"></path>\n                <path d=\"M12 4l0 12\"></path>\n              </svg>{\" \"}\n              Download\n            </button>\n\n            {/* dropdown-menu-end */}\n            <ul className=\"dropdown-menu my-2\">\n              <li>\n                <button\n                  type=\"button\"\n                  style={{ cursor: \"pointer\" }}\n                  className=\"dropdown-item\"\n                  onClick={() => {\n                    if (staticNotebook) {\n                      handleDownload(\n                        `${axios.defaults.baseURL}${notebookPath}`,\n                        `${notebookTitle}.html`\n                      );\n                    } else {\n                      runDownloadHTML();\n                    }\n                  }}\n                >\n                  <i className=\"fa fa-file-code-o\" aria-hidden=\"true\"></i>{\" \"}\n                  Download as HTML\n                </button>\n              </li>\n              <li>\n                <hr className=\"dropdown-divider\" />\n              </li>\n              <li>\n                <button\n                  type=\"button\"\n                  className=\"dropdown-item\"\n                  onClick={() => {\n                    if (staticNotebook) {\n                      dispatch(exportToPDF(siteId, notebookId, notebookPath));\n                    } else {\n                      dispatch(setExportingToPDF(true));\n                      runDownloadPDF();\n                    }\n                  }}\n                >\n                  <i className=\"fa fa-file-pdf-o\" aria-hidden=\"true\"></i>{\" \"}\n                  Download as PDF\n                </button>\n              </li>\n            </ul>\n          </div>\n        )}\n        <button\n          className=\"btn btn-sm btn-primary\"\n          onClick={() => dispatch(setShowShareDialog(true))}\n          disabled={waiting}\n        >\n          <svg\n            xmlns=\"http://www.w3.org/2000/svg\"\n            width=\"14\"\n            height=\"14\"\n            viewBox=\"0 0 24 24\"\n            strokeWidth=\"2\"\n            stroke=\"currentColor\"\n            fill=\"none\"\n            strokeLinecap=\"round\"\n            strokeLinejoin=\"round\"\n          >\n            <path stroke=\"none\" d=\"M0 0h24v24H0z\" fill=\"none\"></path>\n            <path d=\"M6 12m-3 0a3 3 0 1 0 6 0a3 3 0 1 0 -6 0\"></path>\n            <path d=\"M18 6m-3 0a3 3 0 1 0 6 0a3 3 0 1 0 -6 0\"></path>\n            <path d=\"M18 18m-3 0a3 3 0 1 0 6 0a3 3 0 1 0 -6 0\"></path>\n            <path d=\"M8.7 10.7l6.6 -3.4\"></path>\n            <path d=\"M8.7 13.3l6.6 3.4\"></path>\n          </svg>{\" \"}\n          Share\n        </button>\n      </div>\n    </div>\n  );\n}\n",
+        "import React, { useEffect } from \"react\";\nimport { useDispatch, useSelector } from \"react-redux\";\nimport { getSessionId, handleDownload } from \"../utils\";\nimport {\n  WorkerState,\n  WebSocketState,\n  getWebSocketState,\n  getWorkerState,\n  getTryConnectCount,\n} from \"../slices/wsSlice\";\nimport { getSiteId, setSiteStatus, SiteStatus } from \"../slices/sitesSlice\";\nimport axios from \"axios\";\nimport { exportToPDF, setExportingToPDF } from \"../slices/tasksSlice\";\nimport { setShowShareDialog } from \"../slices/appSlice\";\n\ntype Props = {\n  allowDownload: boolean;\n  allowShare: boolean;\n  waiting: boolean;\n  continuousUpdate: boolean;\n  staticNotebook: boolean;\n  notebookId: number;\n  notebookPath: string;\n  notebookTitle: string;\n  runDownloadHTML: () => void;\n  runDownloadPDF: () => void;\n};\n\nexport default function StatusBar({\n  allowDownload,\n  allowShare,\n  waiting,\n  continuousUpdate,\n  staticNotebook,\n  notebookId,\n  notebookPath,\n  notebookTitle,\n  runDownloadHTML,\n  runDownloadPDF,\n}: Props) {\n  const dispatch = useDispatch();\n  const wsStatus = useSelector(getWebSocketState);\n  const workerState = useSelector(getWorkerState);\n  const tryConnectCount = useSelector(getTryConnectCount);\n  const siteId = useSelector(getSiteId);\n\n  useEffect(() => {\n    if (tryConnectCount >= 5) {\n      dispatch(setSiteStatus(SiteStatus.LostConnection));\n    }\n  }, [dispatch, tryConnectCount]);\n\n  let wifiColor = \"orange\";\n  if (wsStatus === WebSocketState.Connected) {\n    wifiColor = \"green\";\n  } else if (\n    wsStatus === WebSocketState.Disconnected ||\n    wsStatus === WebSocketState.Unknown\n  ) {\n    wifiColor = \"red\";\n  }\n\n  let workerColor = \"orange\";\n  if (workerState === WorkerState.Running || workerState === WorkerState.Busy) {\n    workerColor = \"green\";\n  } else if (\n    workerState === WorkerState.Missing ||\n    workerState === WorkerState.Unknown\n  ) {\n    workerColor = \"red\";\n  }\n\n  return (\n    <div style={{ paddingBottom: \"25px\" }}>\n      {notebookId !== undefined && !staticNotebook && (\n        <>\n          <span title={`WebSocket: ${wsStatus}`}>\n            <svg\n              xmlns=\"http://www.w3.org/2000/svg\"\n              width=\"16\"\n              height=\"16\"\n              fill={wifiColor}\n              className=\"bi bi-wifi\"\n              viewBox=\"0 0 16 16\"\n            >\n              <path d=\"M15.384 6.115a.485.485 0 0 0-.047-.736A12.444 12.444 0 0 0 8 3C5.259 3 2.723 3.882.663 5.379a.485.485 0 0 0-.048.736.518.518 0 0 0 .668.05A11.448 11.448 0 0 1 8 4c2.507 0 4.827.802 6.716 2.164.205.148.49.13.668-.049z\" />\n              <path d=\"M13.229 8.271a.482.482 0 0 0-.063-.745A9.455 9.455 0 0 0 8 6c-1.905 0-3.68.56-5.166 1.526a.48.48 0 0 0-.063.745.525.525 0 0 0 .652.065A8.46 8.46 0 0 1 8 7a8.46 8.46 0 0 1 4.576 1.336c.206.132.48.108.653-.065zm-2.183 2.183c.226-.226.185-.605-.1-.75A6.473 6.473 0 0 0 8 9c-1.06 0-2.062.254-2.946.704-.285.145-.326.524-.1.75l.015.015c.16.16.407.19.611.09A5.478 5.478 0 0 1 8 10c.868 0 1.69.201 2.42.56.203.1.45.07.61-.091l.016-.015zM9.06 12.44c.196-.196.198-.52-.04-.66A1.99 1.99 0 0 0 8 11.5a1.99 1.99 0 0 0-1.02.28c-.238.14-.236.464-.04.66l.706.706a.5.5 0 0 0 .707 0l.707-.707z\" />\n            </svg>\n          </span>{\" \"}\n          <span title={`Worker: ${workerState}\\nSession Id: ${getSessionId()}`}>\n            <svg\n              xmlns=\"http://www.w3.org/2000/svg\"\n              width=\"16\"\n              height=\"16\"\n              fill={workerColor}\n              className=\"bi bi-cpu\"\n              viewBox=\"0 0 16 16\"\n            >\n              <path d=\"M5 0a.5.5 0 0 1 .5.5V2h1V.5a.5.5 0 0 1 1 0V2h1V.5a.5.5 0 0 1 1 0V2h1V.5a.5.5 0 0 1 1 0V2A2.5 2.5 0 0 1 14 4.5h1.5a.5.5 0 0 1 0 1H14v1h1.5a.5.5 0 0 1 0 1H14v1h1.5a.5.5 0 0 1 0 1H14v1h1.5a.5.5 0 0 1 0 1H14a2.5 2.5 0 0 1-2.5 2.5v1.5a.5.5 0 0 1-1 0V14h-1v1.5a.5.5 0 0 1-1 0V14h-1v1.5a.5.5 0 0 1-1 0V14h-1v1.5a.5.5 0 0 1-1 0V14A2.5 2.5 0 0 1 2 11.5H.5a.5.5 0 0 1 0-1H2v-1H.5a.5.5 0 0 1 0-1H2v-1H.5a.5.5 0 0 1 0-1H2v-1H.5a.5.5 0 0 1 0-1H2A2.5 2.5 0 0 1 4.5 2V.5A.5.5 0 0 1 5 0zm-.5 3A1.5 1.5 0 0 0 3 4.5v7A1.5 1.5 0 0 0 4.5 13h7a1.5 1.5 0 0 0 1.5-1.5v-7A1.5 1.5 0 0 0 11.5 3h-7zM5 6.5A1.5 1.5 0 0 1 6.5 5h3A1.5 1.5 0 0 1 11 6.5v3A1.5 1.5 0 0 1 9.5 11h-3A1.5 1.5 0 0 1 5 9.5v-3zM6.5 6a.5.5 0 0 0-.5.5v3a.5.5 0 0 0 .5.5h3a.5.5 0 0 0 .5-.5v-3a.5.5 0 0 0-.5-.5h-3z\" />\n            </svg>\n          </span>\n        </>\n      )}\n      {workerState === WorkerState.Busy && (\n        <span title=\"Worker is busy\">\n          {\" \"}\n          <svg\n            xmlns=\"http://www.w3.org/2000/svg\"\n            width=\"16\"\n            height=\"16\"\n            fill=\"green\"\n            className=\"bi bi-activity\"\n            viewBox=\"0 0 16 16\"\n          >\n            <path\n              fillRule=\"evenodd\"\n              d=\"M6 2a.5.5 0 0 1 .47.33L10 12.036l1.53-4.208A.5.5 0 0 1 12 7.5h3.5a.5.5 0 0 1 0 1h-3.15l-1.88 5.17a.5.5 0 0 1-.94 0L6 3.964 4.47 8.171A.5.5 0 0 1 4 8.5H.5a.5.5 0 0 1 0-1h3.15l1.88-5.17A.5.5 0 0 1 6 2Z\"\n            />\n          </svg>\n        </span>\n      )}\n      <div style={{ float: \"right\" }}>\n        {allowDownload && (\n          <div\n            className=\"dropdown mx-2 btn-group\"\n            style={\n              {\n                //display: \"inline\",\n                // width: \"47%\",\n                // float: continuousUpdate ? \"left\" : \"right\",\n              }\n            }\n          >\n            <button\n              className=\"btn btn-sm btn-primary dropdown-toggle\"\n              // style={{ margin: \"0px\", width: \"100%\" }}\n              type=\"button\"\n              data-bs-toggle=\"dropdown\"\n              disabled={waiting}\n            >\n              <svg\n                xmlns=\"http://www.w3.org/2000/svg\"\n                width=\"14\"\n                height=\"14\"\n                viewBox=\"0 0 24 24\"\n                strokeWidth=\"2\"\n                stroke=\"currentColor\"\n                fill=\"none\"\n                strokeLinecap=\"round\"\n                strokeLinejoin=\"round\"\n                style={{ paddingBottom: \"1px\" }}\n              >\n                <path stroke=\"none\" d=\"M0 0h24v24H0z\" fill=\"none\"></path>\n                <path d=\"M4 17v2a2 2 0 0 0 2 2h12a2 2 0 0 0 2 -2v-2\"></path>\n                <path d=\"M7 11l5 5l5 -5\"></path>\n                <path d=\"M12 4l0 12\"></path>\n              </svg>{\" \"}\n              Download\n            </button>\n\n            {/* dropdown-menu-end */}\n            <ul className=\"dropdown-menu my-2\">\n              <li>\n                <button\n                  type=\"button\"\n                  style={{ cursor: \"pointer\" }}\n                  className=\"dropdown-item\"\n                  onClick={() => {\n                    if (staticNotebook) {\n                      handleDownload(\n                        `${axios.defaults.baseURL}${notebookPath}`,\n                        `${notebookTitle}.html`\n                      );\n                    } else {\n                      runDownloadHTML();\n                    }\n                  }}\n                >\n                  <i className=\"fa fa-file-code-o\" aria-hidden=\"true\"></i>{\" \"}\n                  Download as HTML\n                </button>\n              </li>\n              <li>\n                <hr className=\"dropdown-divider\" />\n              </li>\n              <li>\n                <button\n                  type=\"button\"\n                  className=\"dropdown-item\"\n                  onClick={() => {\n                    if (staticNotebook) {\n                      dispatch(exportToPDF(siteId, notebookId, notebookPath));\n                    } else {\n                      dispatch(setExportingToPDF(true));\n                      runDownloadPDF();\n                    }\n                  }}\n                >\n                  <i className=\"fa fa-file-pdf-o\" aria-hidden=\"true\"></i>{\" \"}\n                  Download as PDF\n                </button>\n              </li>\n            </ul>\n          </div>\n        )}\n        {allowShare && (\n          <button\n            className=\"btn btn-sm btn-primary\"\n            onClick={() => dispatch(setShowShareDialog(true))}\n            disabled={waiting}\n          >\n            <svg\n              xmlns=\"http://www.w3.org/2000/svg\"\n              width=\"14\"\n              height=\"14\"\n              viewBox=\"0 0 24 24\"\n              strokeWidth=\"2\"\n              stroke=\"currentColor\"\n              fill=\"none\"\n              strokeLinecap=\"round\"\n              strokeLinejoin=\"round\"\n            >\n              <path stroke=\"none\" d=\"M0 0h24v24H0z\" fill=\"none\"></path>\n              <path d=\"M6 12m-3 0a3 3 0 1 0 6 0a3 3 0 1 0 -6 0\"></path>\n              <path d=\"M18 6m-3 0a3 3 0 1 0 6 0a3 3 0 1 0 -6 0\"></path>\n              <path d=\"M18 18m-3 0a3 3 0 1 0 6 0a3 3 0 1 0 -6 0\"></path>\n              <path d=\"M8.7 10.7l6.6 -3.4\"></path>\n              <path d=\"M8.7 13.3l6.6 3.4\"></path>\n            </svg>{\" \"}\n            Share\n          </button>\n        )}\n      </div>\n    </div>\n  );\n}\n",
         "import React, { useEffect } from \"react\";\nimport { useDispatch } from \"react-redux\";\nimport { setWidgetValue } from \"../slices/notebooksSlice\";\n\ntype ButtonProps = {\n  widgetKey: string;\n  label: string | null;\n  style: string;\n  value: string | boolean | null;\n  disabled: boolean;\n  hidden: boolean;\n  runNb: () => void;\n};\n\nexport default function ButtonWidget({\n  widgetKey,\n  label,\n  style,\n  value,\n  disabled,\n  hidden,\n  runNb,\n}: ButtonProps) {\n  const dispatch = useDispatch();\n\n  let selectedClass = \"btn-primary\";\n  if (style === \"success\") {\n    selectedClass = \"btn-success\";\n  } else if (style === \"danger\") {\n    selectedClass = \"btn-danger\";\n  } else if (style === \"info\") {\n    selectedClass = \"btn-info\";\n  } else if (style === \"warning\") {\n    selectedClass = \"btn-warning\";\n  }\n\n  useEffect(() => {\n    if (value) {\n      runNb();\n    }\n    // eslint-disable-next-line react-hooks/exhaustive-deps\n  }, [value]);\n\n  return (\n    <div className=\"form-group mb-3\" style={{ display: hidden ? \"none\" : \"\" }}>\n      <button\n        type=\"button\"\n        className={`btn ${selectedClass}`}\n        style={{ marginRight: \"10px\", width: \"47%\" }}\n        onClick={() => {\n          dispatch(\n            setWidgetValue({\n              key: widgetKey,\n              value: true,\n            })\n          );\n        }}\n        disabled={disabled}\n      >\n        {label}\n      </button>\n    </div>\n  );\n}\n",
         "/* eslint-disable jsx-a11y/anchor-is-valid */\nimport React from \"react\";\nimport { WorkerState } from \"../slices/wsSlice\";\n\ntype RunButtonProps = {\n  runNb: () => void;\n  waiting: boolean;\n  workerState: WorkerState;\n};\n\nexport default function RunButton({\n  runNb,\n  waiting,\n  workerState,\n}: RunButtonProps) {\n  return (\n    <button\n      type=\"button\"\n      className=\"btn btn-success\"\n      style={{ marginRight: \"10px\", width: \"100%\" }}\n      onClick={() => {\n        runNb();\n      }}\n      disabled={\n        waiting ||\n        // !allFilesUploaded() ||\n        workerState !== WorkerState.Running\n      }\n    >\n      {workerState === WorkerState.Running && (\n        <span>\n          <i className=\"fa fa-play\" aria-hidden=\"true\"></i> Run\n        </span>\n      )}\n      {workerState === WorkerState.Busy && (\n        <span>\n          <svg\n            xmlns=\"http://www.w3.org/2000/svg\"\n            width=\"16\"\n            height=\"16\"\n            fill=\"white\"\n            className=\"bi bi-activity\"\n            viewBox=\"0 0 16 16\"\n          >\n            <path\n              fillRule=\"evenodd\"\n              d=\"M6 2a.5.5 0 0 1 .47.33L10 12.036l1.53-4.208A.5.5 0 0 1 12 7.5h3.5a.5.5 0 0 1 0 1h-3.15l-1.88 5.17a.5.5 0 0 1-.94 0L6 3.964 4.47 8.171A.5.5 0 0 1 4 8.5H.5a.5.5 0 0 1 0-1h3.15l1.88-5.17A.5.5 0 0 1 6 2Z\"\n            />\n          </svg>{\" \"}\n          Busy\n        </span>\n      )}\n      {workerState !== WorkerState.Busy &&\n        workerState !== WorkerState.Running && <span>Waiting ...</span>}\n    </button>\n  );\n}\n",
-        "/* eslint-disable jsx-a11y/anchor-is-valid */\nimport React, { useContext } from \"react\";\nimport { useEffect } from \"react\";\nimport { useDispatch, useSelector } from \"react-redux\";\nimport { listRestTasks, scrapeSlidesHash } from \"../slices/tasksSlice\";\nimport CheckboxWidget from \"../widgets/Checkbox\";\nimport NumericWidget from \"../widgets/Numeric\";\nimport RangeWidget from \"../widgets/Range\";\nimport SelectWidget from \"../widgets/Select\";\nimport SliderWidget from \"../widgets/Slider\";\n\nimport {\n  isCheckboxWidget,\n  isFileWidget,\n  isNumericWidget,\n  isRangeWidget,\n  isSelectWidget,\n  isSliderWidget,\n  isTextWidget,\n  isMarkdownWidget,\n  IWidget,\n  isOutputFilesWidget,\n  isButtonWidget,\n  isAPIResponseWidget,\n} from \"../widgets/Types\";\n\nimport {\n  clearWidgetsUrlValues,\n  getUrlValuesUsed,\n  getWidgetsInitialized,\n  getWidgetsUrlValues,\n  getWidgetsValues,\n  setSlidesHash,\n  setUrlValuesUsed,\n  setWidgetsInitialized,\n  setWidgetValue,\n  WidgetValueType,\n} from \"../slices/notebooksSlice\";\nimport FileWidget from \"../widgets/File\";\nimport TextWidget from \"../widgets/Text\";\nimport { setShowSideBar, setView } from \"../slices/appSlice\";\nimport MarkdownWidget from \"../widgets/Markdown\";\n\nimport { WebSocketContext } from \"../websocket/Provider\";\nimport WebSocketStateBar from \"./StatusBar\";\nimport {\n  downloadHTML,\n  downloadPDF,\n  getWorkerState,\n  runNotebook,\n  WorkerState,\n} from \"../slices/wsSlice\";\nimport ButtonWidget from \"../widgets/Button\";\nimport RunButton from \"./RunButton\";\nimport BlockUi from \"react-block-ui\";\nimport { getSiteId } from \"../slices/sitesSlice\";\n\ntype SideBarProps = {\n  notebookTitle: string;\n  notebookId: number;\n  notebookSchedule: string;\n  taskCreatedAt: Date;\n  loadingState: string;\n  waiting: boolean;\n  widgetsParams: Record<string, IWidget>;\n  watchMode: boolean;\n  notebookPath: string;\n  displayEmbed: boolean;\n  showFiles: boolean;\n  isPresentation: boolean;\n  notebookParseErrors: string;\n  continuousUpdate: boolean;\n  staticNotebook: boolean;\n  allowDownload: boolean;\n};\n\nexport default function SideBar({\n  notebookTitle,\n  notebookId,\n  notebookSchedule,\n  taskCreatedAt,\n  loadingState,\n  waiting,\n  widgetsParams,\n  watchMode,\n  notebookPath,\n  displayEmbed,\n  showFiles,\n  isPresentation,\n  notebookParseErrors,\n  continuousUpdate,\n  staticNotebook,\n  allowDownload,\n}: SideBarProps) {\n  const dispatch = useDispatch();\n  const widgetsValues: Record<string, WidgetValueType> = useSelector(\n    getWidgetsValues\n  ) as Record<string, WidgetValueType>;\n  const widgetsUrlValues = useSelector(getWidgetsUrlValues);\n  const workerState = useSelector(getWorkerState);\n  const widgetsInitialized = useSelector(getWidgetsInitialized);\n  const urlValuesUsed = useSelector(getUrlValuesUsed);\n  const siteId = useSelector(getSiteId);\n  const ws = useContext(WebSocketContext);\n\n  const runNb = () => {\n    if (continuousUpdate) {\n      execNb();\n    }\n  };\n\n  const execNb = () => {\n    const slidesHash = scrapeSlidesHash();\n    dispatch(setSlidesHash(slidesHash));\n\n    if (widgetsUrlValues) {\n      let params = {} as Record<string, WidgetValueType>;\n      // eslint-disable-next-line @typescript-eslint/no-unused-vars\n      for (let [key, widgetParams] of Object.entries(widgetsParams)) {\n        if (key in widgetsUrlValues) {\n          params[key] = widgetsUrlValues[key];\n          dispatch(setWidgetValue({ key, value: params[key] }));\n        } else if (key in widgetsValues) {\n          params[key] = widgetsValues[key];\n        }\n      }\n      ws.sendMessage(JSON.stringify(runNotebook(JSON.stringify(params))));\n      dispatch(clearWidgetsUrlValues());\n    } else {\n      ws.sendMessage(\n        JSON.stringify(runNotebook(JSON.stringify(widgetsValues)))\n      );\n    }\n  };\n\n  useEffect(() => {\n    if (siteId !== undefined && notebookId !== undefined) {\n      dispatch(listRestTasks(siteId, notebookId));\n    }\n  }, [dispatch, notebookId, siteId]);\n\n  useEffect(() => {\n    if (widgetsInitialized && urlValuesUsed) {\n      execNb();\n      dispatch(setUrlValuesUsed(false));\n      dispatch(setWidgetsInitialized(false));\n    }\n    // eslint-disable-next-line react-hooks/exhaustive-deps\n  }, [widgetsInitialized, urlValuesUsed]);\n\n  const runDownloadHTML = () => {\n    if (!staticNotebook) {\n      ws.sendMessage(JSON.stringify(downloadHTML()));\n    }\n  };\n\n  const runDownloadPDF = () => {\n    if (!staticNotebook) {\n      ws.sendMessage(JSON.stringify(downloadPDF()));\n    }\n  };\n\n  useEffect(() => {\n    if (widgetsParams) {\n      for (let [key, widgetParams] of Object.entries(widgetsParams)) {\n        if (key in widgetsValues) {\n          continue;\n        }\n\n        if (widgetParams.input === \"file\") {\n          dispatch(setWidgetValue({ key, value: [] as string[] }));\n        } else if (widgetParams.input === \"text\") {\n          dispatch(\n            setWidgetValue({\n              key,\n              value: widgetParams.value ? widgetParams.value : \"\",\n            })\n          );\n        } else if (isMarkdownWidget(widgetParams)) {\n          // do nothing\n          // dont put value into store\n        } else if (isOutputFilesWidget(widgetParams)) {\n          dispatch(setWidgetValue({ key, value: \"output-dir\" }));\n        } else {\n          dispatch(setWidgetValue({ key, value: widgetParams.value }));\n        }\n      }\n    }\n  }, [dispatch, widgetsParams, widgetsValues]);\n\n  let widgets = [];\n  let fileKeys = [] as string[]; // keys to file widgets, all need to be selected to enable RUN button\n\n  if (widgetsParams && !staticNotebook) {\n    // sort widgets keys based on cell index and code line number\n    let widgetKeys = [];\n    for (let key of Object.keys(widgetsParams)) {\n      const parts = key.split(\".\");\n      widgetKeys.push([key, parseFloat(`${parts[1]}.${parts[2]}`)]);\n    }\n    widgetKeys.sort(function (a, b) {\n      const a1 = a[1] as number;\n      const b1 = b[1] as number;\n      return a1 - b1;\n    });\n\n    for (let wKey of widgetKeys) {\n      const key = wKey[0] as string;\n      const widgetParams = widgetsParams[key];\n\n      if (isSelectWidget(widgetParams)) {\n        widgets.push(\n          <SelectWidget\n            widgetKey={key}\n            disabled={waiting || widgetParams?.disabled}\n            hidden={widgetParams?.hidden}\n            label={widgetParams?.label}\n            value={widgetsValues[key] as string}\n            choices={widgetParams?.choices}\n            multi={widgetParams?.multi}\n            key={key}\n            runNb={runNb}\n            url_key={widgetParams?.url_key}\n          />\n        );\n      } else if (isCheckboxWidget(widgetParams)) {\n        widgets.push(\n          <CheckboxWidget\n            widgetKey={key}\n            disabled={waiting || widgetParams?.disabled}\n            hidden={widgetParams?.hidden}\n            label={widgetParams?.label}\n            value={widgetsValues[key] as boolean}\n            key={key}\n            runNb={runNb}\n            url_key={widgetParams?.url_key}\n          />\n        );\n      } else if (isNumericWidget(widgetParams)) {\n        widgets.push(\n          <NumericWidget\n            widgetKey={key}\n            disabled={waiting || widgetParams?.disabled}\n            hidden={widgetParams?.hidden}\n            label={widgetParams?.label}\n            value={widgetsValues[key] as number}\n            min={widgetParams?.min}\n            max={widgetParams?.max}\n            step={widgetParams?.step}\n            key={key}\n            runNb={runNb}\n            continuousUpdate={continuousUpdate}\n            url_key={widgetParams?.url_key}\n          />\n        );\n      } else if (isSliderWidget(widgetParams)) {\n        widgets.push(\n          <SliderWidget\n            widgetKey={key}\n            disabled={waiting || widgetParams?.disabled}\n            hidden={widgetParams?.hidden}\n            label={widgetParams?.label}\n            value={widgetsValues[key] as number}\n            min={widgetParams?.min}\n            max={widgetParams?.max}\n            step={widgetParams?.step}\n            vertical={widgetParams?.vertical}\n            key={key}\n            runNb={runNb}\n            url_key={widgetParams?.url_key}\n          />\n        );\n      } else if (isRangeWidget(widgetParams)) {\n        widgets.push(\n          <RangeWidget\n            widgetKey={key}\n            disabled={waiting || widgetParams?.disabled}\n            hidden={widgetParams?.hidden}\n            label={widgetParams?.label}\n            value={widgetsValues[key] as [number, number]}\n            min={widgetParams?.min}\n            max={widgetParams?.max}\n            step={widgetParams?.step}\n            vertical={widgetParams?.vertical}\n            key={key}\n            runNb={runNb}\n            url_key={widgetParams.url_key}\n          />\n        );\n      } else if (isFileWidget(widgetParams)) {\n        widgets.push(\n          <FileWidget\n            widgetKey={key}\n            disabled={waiting || widgetParams?.disabled}\n            hidden={widgetParams?.hidden}\n            label={widgetParams?.label}\n            maxFileSize={widgetParams?.maxFileSize}\n            key={key}\n            value={widgetsValues[key] as string[]}\n            runNb={runNb}\n          />\n        );\n        fileKeys.push(key);\n      } else if (isTextWidget(widgetParams)) {\n        widgets.push(\n          <TextWidget\n            widgetKey={key}\n            disabled={waiting || widgetParams?.disabled}\n            hidden={widgetParams?.hidden}\n            label={widgetParams?.label}\n            value={widgetsValues[key] as string}\n            rows={widgetParams?.rows}\n            key={key}\n            runNb={runNb}\n            continuousUpdate={continuousUpdate}\n            url_key={widgetParams?.url_key}\n            sanitize={widgetParams?.sanitize}\n          />\n        );\n      } else if (isMarkdownWidget(widgetParams)) {\n        widgets.push(\n          <MarkdownWidget\n            value={widgetParams.value as string}\n            disabled={waiting}\n            key={key}\n          />\n        );\n      } else if (isButtonWidget(widgetParams)) {\n        widgets.push(\n          <ButtonWidget\n            widgetKey={key}\n            disabled={waiting || widgetParams?.disabled}\n            hidden={widgetParams?.hidden}\n            label={widgetParams?.label}\n            value={widgetsValues[key] as boolean}\n            style={widgetParams?.style}\n            key={key}\n            runNb={runNb}\n          />\n        );\n      } else if (isOutputFilesWidget(widgetParams)) {\n        // do nothing\n      } else if (isAPIResponseWidget(widgetParams)) {\n        // do nothing\n      } else {\n        console.log(\"Unknown widget type\", widgetParams);\n      }\n    }\n  }\n\n  let additionalStyle = {};\n  if (displayEmbed) {\n    additionalStyle = { padding: \"0px\" };\n  }\n\n  const addSpaceInsteadTitle =\n    notebookTitle === undefined ||\n    notebookTitle === null ||\n    notebookTitle === \"\";\n\n  return (\n    <nav\n      id=\"sidebarMenu\"\n      className=\"col-lg-3 d-md-block bg-light sidebar\"\n      style={{ ...additionalStyle, overflowY: \"auto\" }}\n    >\n      <BlockUi blocking={false} message=\"\">\n        <div className=\"position-sticky p-3\">\n          <h4>\n            {notebookTitle}\n            <button\n              className=\"btn btn-sm  btn-outline-primary\"\n              type=\"button\"\n              style={{\n                float: \"right\",\n                zIndex: \"101\",\n              }}\n              onClick={() => dispatch(setShowSideBar(false))}\n              data-toggle=\"tooltip\"\n              data-placement=\"right\"\n              title=\"Hide sidebar\"\n            >\n              <i className=\"fa fa-chevron-left\" aria-hidden=\"true\" />\n            </button>\n          </h4>\n\n          <div style={{ padding: \"0px\" }}>\n            <form>\n              {widgets}\n\n              {addSpaceInsteadTitle && <div style={{ padding: \"15px\" }}></div>}\n\n              <div className=\"form-group mb-3 pb-1 pt-2\">\n                {!continuousUpdate && (\n                  <RunButton\n                    runNb={execNb}\n                    waiting={waiting}\n                    workerState={workerState}\n                  />\n                )}\n              </div>\n\n              {workerState === WorkerState.UsageLimitReached && (\n                <div className=\"alert alert-info mb-3 mt-3\" role=\"alert\">\n                  <i className=\"fa fa-info-circle\" aria-hidden=\"true\"></i> Usage\n                  limit was reached. Please upgrade the plan.\n                </div>\n              )}\n\n              {workerState === WorkerState.MaxIdleTimeReached && (\n                <div className=\"alert alert-info mb-3 mt-3\" role=\"alert\">\n                  <i className=\"fa fa-info-circle\" aria-hidden=\"true\"></i> Your\n                  worker was idle for too long, that's why we have stopped it.\n                  Do you need a worker?\n                  <br />\n                  <button\n                    className=\"btn btn-sm btn-primary my-2\"\n                    onClick={() => window.location.reload()}\n                  >\n                    Restart worker\n                  </button>\n                </div>\n              )}\n              {workerState === WorkerState.MaxRunTimeReached && (\n                <div className=\"alert alert-info mb-3 mt-3\" role=\"alert\">\n                  <i className=\"fa fa-info-circle\" aria-hidden=\"true\"></i> Your\n                  worker was running for too long, that's why we have stopped\n                  it. Do you need a worker?\n                  <br />\n                  <button\n                    className=\"btn btn-sm btn-primary my-2\"\n                    onClick={() => window.location.reload()}\n                  >\n                    Restart worker\n                  </button>\n                </div>\n              )}\n              {waiting &&\n                (workerState === WorkerState.Unknown ||\n                  workerState === WorkerState.Queued) && (\n                  <div className=\"alert alert-warning mb-3 mt-3\" role=\"alert\">\n                    <i className=\"fa fa-cogs\" aria-hidden=\"true\"></i> Waiting\n                    for worker ...\n                  </div>\n                )}\n              {waiting && workerState === WorkerState.Starting && (\n                <div className=\"alert alert-success mb-3 mt-3\" role=\"alert\">\n                  <i className=\"fa fa-cogs\" aria-hidden=\"true\"></i> Initializing\n                  worker ...\n                </div>\n              )}\n              {watchMode && (\n                <div className=\"alert alert-secondary mb-3 mt-3\" role=\"alert\">\n                  <i className=\"fa fa-refresh\" aria-hidden=\"true\"></i> Notebook\n                  in watch mode. All changes to Notebook will be automatically\n                  visible in Mercury.\n                </div>\n              )}\n\n              {isPresentation && (\n                <div className=\"alert alert-primary mb-3\" role=\"alert\">\n                  <i className=\"fa fa-television\" aria-hidden=\"true\"></i> Click\n                  on presentation and press <b>F</b> for full screen. Press{\" \"}\n                  <b>Esc</b> to quit.\n                  <br />\n                  <br />\n                  <i className=\"fa fa-arrows\" aria-hidden=\"true\"></i> Click on\n                  presentation and press <b>Esc</b> to navigate slides.\n                </div>\n              )}\n\n              {/* {notebookParseErrors && (\n                <div className=\"alert alert-danger mb-3\" role=\"alert\">\n                  <i\n                    className=\"fa fa-exclamation-circle\"\n                    aria-hidden=\"true\"\n                  ></i>{\" \"}\n                  <b>Errors in the YAML</b>\n                  <br />\n                  {notebookParseErrors}\n                </div>\n              )} */}\n            </form>\n          </div>\n\n          {showFiles && (\n            <div>\n              <hr />\n              <button\n                className=\"btn btn-sm btn-outline-secondary\"\n                style={{\n                  border: \"none\",\n                  //fontWeight: 500,\n                }}\n                onClick={() => {\n                  dispatch(setView(\"app\"));\n                }}\n              >\n                <i className=\"fa fa-laptop\" aria-hidden=\"true\"></i> App\n              </button>\n\n              <button\n                className=\"btn btn-sm btn-outline-secondary\"\n                style={{\n                  border: \"none\",\n                  //fontWeight: 500,\n                }}\n                onClick={() => {\n                  dispatch(setView(\"files\"));\n                }}\n              >\n                <i className=\"fa fa-folder-open-o\" aria-hidden=\"true\"></i>{\" \"}\n                Output Files\n              </button>\n            </div>\n          )}\n\n          <div>\n            <hr />\n            <div style={{ paddingLeft: \"10px\" }}>\n              <WebSocketStateBar\n                notebookId={notebookId}\n                notebookPath={notebookPath}\n                notebookTitle={notebookTitle}\n                staticNotebook={staticNotebook}\n                allowDownload={allowDownload}\n                waiting={waiting}\n                continuousUpdate={continuousUpdate}\n                runDownloadHTML={runDownloadHTML}\n                runDownloadPDF={runDownloadPDF}\n              />{\" \"}\n            </div>\n          </div>\n        </div>\n      </BlockUi>\n    </nav>\n  );\n}\n",
+        "/* eslint-disable jsx-a11y/anchor-is-valid */\nimport React, { useContext } from \"react\";\nimport { useEffect } from \"react\";\nimport { useDispatch, useSelector } from \"react-redux\";\nimport { scrapeSlidesHash } from \"../slices/tasksSlice\";\nimport CheckboxWidget from \"../widgets/Checkbox\";\nimport NumericWidget from \"../widgets/Numeric\";\nimport RangeWidget from \"../widgets/Range\";\nimport SelectWidget from \"../widgets/Select\";\nimport SliderWidget from \"../widgets/Slider\";\n\nimport {\n  isCheckboxWidget,\n  isFileWidget,\n  isNumericWidget,\n  isRangeWidget,\n  isSelectWidget,\n  isSliderWidget,\n  isTextWidget,\n  isMarkdownWidget,\n  IWidget,\n  isOutputFilesWidget,\n  isButtonWidget,\n  isAPIResponseWidget,\n} from \"../widgets/Types\";\n\nimport {\n  clearWidgetsUrlValues,\n  getUrlValuesUsed,\n  getWidgetsInitialized,\n  getWidgetsUrlValues,\n  getWidgetsValues,\n  setSlidesHash,\n  setUrlValuesUsed,\n  setWidgetsInitialized,\n  setWidgetValue,\n  WidgetValueType,\n} from \"../slices/notebooksSlice\";\nimport FileWidget from \"../widgets/File\";\nimport TextWidget from \"../widgets/Text\";\nimport { setShowSideBar, setView } from \"../slices/appSlice\";\nimport MarkdownWidget from \"../widgets/Markdown\";\n\nimport { WebSocketContext } from \"../websocket/Provider\";\nimport WebSocketStateBar from \"./StatusBar\";\nimport {\n  downloadHTML,\n  downloadPDF,\n  getWorkerState,\n  runNotebook,\n  WorkerState,\n} from \"../slices/wsSlice\";\nimport ButtonWidget from \"../widgets/Button\";\nimport RunButton from \"./RunButton\";\nimport BlockUi from \"react-block-ui\";\n\ntype SideBarProps = {\n  notebookTitle: string;\n  notebookId: number;\n  notebookSchedule: string;\n  taskCreatedAt: Date;\n  loadingState: string;\n  waiting: boolean;\n  widgetsParams: Record<string, IWidget>;\n  watchMode: boolean;\n  notebookPath: string;\n  displayEmbed: boolean;\n  showFiles: boolean;\n  isPresentation: boolean;\n  notebookParseErrors: string;\n  continuousUpdate: boolean;\n  staticNotebook: boolean;\n  allowDownload: boolean;\n  allowShare: boolean;\n};\n\nexport default function SideBar({\n  notebookTitle,\n  notebookId,\n  notebookSchedule,\n  taskCreatedAt,\n  loadingState,\n  waiting,\n  widgetsParams,\n  watchMode,\n  notebookPath,\n  displayEmbed,\n  showFiles,\n  isPresentation,\n  notebookParseErrors,\n  continuousUpdate,\n  staticNotebook,\n  allowDownload,\n  allowShare,\n}: SideBarProps) {\n  const dispatch = useDispatch();\n  const widgetsValues: Record<string, WidgetValueType> = useSelector(\n    getWidgetsValues\n  ) as Record<string, WidgetValueType>;\n  const widgetsUrlValues = useSelector(getWidgetsUrlValues);\n  const workerState = useSelector(getWorkerState);\n  const widgetsInitialized = useSelector(getWidgetsInitialized);\n  const urlValuesUsed = useSelector(getUrlValuesUsed);\n  const ws = useContext(WebSocketContext);\n\n  const runNb = () => {\n    if (continuousUpdate) {\n      execNb();\n    }\n  };\n\n  const execNb = () => {\n    const slidesHash = scrapeSlidesHash();\n    dispatch(setSlidesHash(slidesHash));\n\n    if (widgetsUrlValues) {\n      let params = {} as Record<string, WidgetValueType>;\n      // eslint-disable-next-line @typescript-eslint/no-unused-vars\n      for (let [key, widgetParams] of Object.entries(widgetsParams)) {\n        if (key in widgetsUrlValues) {\n          params[key] = widgetsUrlValues[key];\n          dispatch(setWidgetValue({ key, value: params[key] }));\n        } else if (key in widgetsValues) {\n          params[key] = widgetsValues[key];\n        }\n      }\n      ws.sendMessage(JSON.stringify(runNotebook(JSON.stringify(params))));\n      dispatch(clearWidgetsUrlValues());\n    } else {\n      ws.sendMessage(\n        JSON.stringify(runNotebook(JSON.stringify(widgetsValues)))\n      );\n    }\n  };\n\n  useEffect(() => {\n    if (widgetsInitialized && urlValuesUsed) {\n      execNb();\n      dispatch(setUrlValuesUsed(false));\n      dispatch(setWidgetsInitialized(false));\n    }\n    // eslint-disable-next-line react-hooks/exhaustive-deps\n  }, [widgetsInitialized, urlValuesUsed]);\n\n  const runDownloadHTML = () => {\n    if (!staticNotebook) {\n      ws.sendMessage(JSON.stringify(downloadHTML()));\n    }\n  };\n\n  const runDownloadPDF = () => {\n    if (!staticNotebook) {\n      ws.sendMessage(JSON.stringify(downloadPDF()));\n    }\n  };\n\n  useEffect(() => {\n    if (widgetsParams) {\n      for (let [key, widgetParams] of Object.entries(widgetsParams)) {\n        if (key in widgetsValues) {\n          continue;\n        }\n\n        if (widgetParams.input === \"file\") {\n          dispatch(setWidgetValue({ key, value: [] as string[] }));\n        } else if (widgetParams.input === \"text\") {\n          dispatch(\n            setWidgetValue({\n              key,\n              value: widgetParams.value ? widgetParams.value : \"\",\n            })\n          );\n        } else if (isMarkdownWidget(widgetParams)) {\n          // do nothing\n          // dont put value into store\n        } else if (isOutputFilesWidget(widgetParams)) {\n          dispatch(setWidgetValue({ key, value: \"output-dir\" }));\n        } else {\n          dispatch(setWidgetValue({ key, value: widgetParams.value }));\n        }\n      }\n    }\n  }, [dispatch, widgetsParams, widgetsValues]);\n\n  let widgets = [];\n  let fileKeys = [] as string[]; // keys to file widgets, all need to be selected to enable RUN button\n\n  if (widgetsParams && !staticNotebook) {\n    // sort widgets keys based on cell index and code line number\n    let widgetKeys = [];\n    for (let key of Object.keys(widgetsParams)) {\n      const parts = key.split(\".\");\n      widgetKeys.push([key, parseFloat(`${parts[1]}.${parts[2]}`)]);\n    }\n    widgetKeys.sort(function (a, b) {\n      const a1 = a[1] as number;\n      const b1 = b[1] as number;\n      return a1 - b1;\n    });\n\n    for (let wKey of widgetKeys) {\n      const key = wKey[0] as string;\n      const widgetParams = widgetsParams[key];\n\n      if (isSelectWidget(widgetParams)) {\n        widgets.push(\n          <SelectWidget\n            widgetKey={key}\n            disabled={waiting || widgetParams?.disabled}\n            hidden={widgetParams?.hidden}\n            label={widgetParams?.label}\n            value={widgetsValues[key] as string}\n            choices={widgetParams?.choices}\n            multi={widgetParams?.multi}\n            key={key}\n            runNb={runNb}\n            url_key={widgetParams?.url_key}\n          />\n        );\n      } else if (isCheckboxWidget(widgetParams)) {\n        widgets.push(\n          <CheckboxWidget\n            widgetKey={key}\n            disabled={waiting || widgetParams?.disabled}\n            hidden={widgetParams?.hidden}\n            label={widgetParams?.label}\n            value={widgetsValues[key] as boolean}\n            key={key}\n            runNb={runNb}\n            url_key={widgetParams?.url_key}\n          />\n        );\n      } else if (isNumericWidget(widgetParams)) {\n        widgets.push(\n          <NumericWidget\n            widgetKey={key}\n            disabled={waiting || widgetParams?.disabled}\n            hidden={widgetParams?.hidden}\n            label={widgetParams?.label}\n            value={widgetsValues[key] as number}\n            min={widgetParams?.min}\n            max={widgetParams?.max}\n            step={widgetParams?.step}\n            key={key}\n            runNb={runNb}\n            continuousUpdate={continuousUpdate}\n            url_key={widgetParams?.url_key}\n          />\n        );\n      } else if (isSliderWidget(widgetParams)) {\n        widgets.push(\n          <SliderWidget\n            widgetKey={key}\n            disabled={waiting || widgetParams?.disabled}\n            hidden={widgetParams?.hidden}\n            label={widgetParams?.label}\n            value={widgetsValues[key] as number}\n            min={widgetParams?.min}\n            max={widgetParams?.max}\n            step={widgetParams?.step}\n            vertical={widgetParams?.vertical}\n            key={key}\n            runNb={runNb}\n            url_key={widgetParams?.url_key}\n          />\n        );\n      } else if (isRangeWidget(widgetParams)) {\n        widgets.push(\n          <RangeWidget\n            widgetKey={key}\n            disabled={waiting || widgetParams?.disabled}\n            hidden={widgetParams?.hidden}\n            label={widgetParams?.label}\n            value={widgetsValues[key] as [number, number]}\n            min={widgetParams?.min}\n            max={widgetParams?.max}\n            step={widgetParams?.step}\n            vertical={widgetParams?.vertical}\n            key={key}\n            runNb={runNb}\n            url_key={widgetParams.url_key}\n          />\n        );\n      } else if (isFileWidget(widgetParams)) {\n        widgets.push(\n          <FileWidget\n            widgetKey={key}\n            disabled={waiting || widgetParams?.disabled}\n            hidden={widgetParams?.hidden}\n            label={widgetParams?.label}\n            maxFileSize={widgetParams?.maxFileSize}\n            key={key}\n            value={widgetsValues[key] as string[]}\n            runNb={runNb}\n          />\n        );\n        fileKeys.push(key);\n      } else if (isTextWidget(widgetParams)) {\n        widgets.push(\n          <TextWidget\n            widgetKey={key}\n            disabled={waiting || widgetParams?.disabled}\n            hidden={widgetParams?.hidden}\n            label={widgetParams?.label}\n            value={widgetsValues[key] as string}\n            rows={widgetParams?.rows}\n            key={key}\n            runNb={runNb}\n            continuousUpdate={continuousUpdate}\n            url_key={widgetParams?.url_key}\n            sanitize={widgetParams?.sanitize}\n          />\n        );\n      } else if (isMarkdownWidget(widgetParams)) {\n        widgets.push(\n          <MarkdownWidget\n            value={widgetParams.value as string}\n            disabled={waiting}\n            key={key}\n          />\n        );\n      } else if (isButtonWidget(widgetParams)) {\n        widgets.push(\n          <ButtonWidget\n            widgetKey={key}\n            disabled={waiting || widgetParams?.disabled}\n            hidden={widgetParams?.hidden}\n            label={widgetParams?.label}\n            value={widgetsValues[key] as boolean}\n            style={widgetParams?.style}\n            key={key}\n            runNb={runNb}\n          />\n        );\n      } else if (isOutputFilesWidget(widgetParams)) {\n        // do nothing\n      } else if (isAPIResponseWidget(widgetParams)) {\n        // do nothing\n      } else {\n        console.log(\"Unknown widget type\", widgetParams);\n      }\n    }\n  }\n\n  let additionalStyle = {};\n  if (displayEmbed) {\n    additionalStyle = { padding: \"0px\" };\n  }\n\n  const addSpaceInsteadTitle =\n    notebookTitle === undefined ||\n    notebookTitle === null ||\n    notebookTitle === \"\";\n\n  return (\n    <nav\n      id=\"sidebarMenu\"\n      className=\"col-lg-3 d-md-block bg-light sidebar\"\n      style={{ ...additionalStyle, overflowY: \"auto\" }}\n    >\n      <BlockUi blocking={false} message=\"\">\n        <div className=\"position-sticky p-3\">\n          <h4>\n            {notebookTitle}\n            <button\n              className=\"btn btn-sm  btn-outline-primary\"\n              type=\"button\"\n              style={{\n                float: \"right\",\n                zIndex: \"101\",\n              }}\n              onClick={() => dispatch(setShowSideBar(false))}\n              data-toggle=\"tooltip\"\n              data-placement=\"right\"\n              title=\"Hide sidebar\"\n            >\n              <i className=\"fa fa-chevron-left\" aria-hidden=\"true\" />\n            </button>\n          </h4>\n\n          <div style={{ padding: \"0px\" }}>\n            <form>\n              {widgets}\n\n              {addSpaceInsteadTitle && <div style={{ padding: \"15px\" }}></div>}\n\n              <div className=\"form-group mb-3 pb-1 pt-2\">\n                {!continuousUpdate && (\n                  <RunButton\n                    runNb={execNb}\n                    waiting={waiting}\n                    workerState={workerState}\n                  />\n                )}\n              </div>\n\n              {workerState === WorkerState.UsageLimitReached && (\n                <div className=\"alert alert-info mb-3 mt-3\" role=\"alert\">\n                  <i className=\"fa fa-info-circle\" aria-hidden=\"true\"></i> Usage\n                  limit was reached. Please upgrade the plan.\n                </div>\n              )}\n\n              {workerState === WorkerState.MaxIdleTimeReached && (\n                <div className=\"alert alert-info mb-3 mt-3\" role=\"alert\">\n                  <i className=\"fa fa-info-circle\" aria-hidden=\"true\"></i> Your\n                  worker was idle for too long, that's why we have stopped it.\n                  Do you need a worker?\n                  <br />\n                  <button\n                    className=\"btn btn-sm btn-primary my-2\"\n                    onClick={() => window.location.reload()}\n                  >\n                    Restart worker\n                  </button>\n                </div>\n              )}\n              {workerState === WorkerState.MaxRunTimeReached && (\n                <div className=\"alert alert-info mb-3 mt-3\" role=\"alert\">\n                  <i className=\"fa fa-info-circle\" aria-hidden=\"true\"></i> Your\n                  worker was running for too long, that's why we have stopped\n                  it. Do you need a worker?\n                  <br />\n                  <button\n                    className=\"btn btn-sm btn-primary my-2\"\n                    onClick={() => window.location.reload()}\n                  >\n                    Restart worker\n                  </button>\n                </div>\n              )}\n              {waiting &&\n                (workerState === WorkerState.Unknown ||\n                  workerState === WorkerState.Queued) && (\n                  <div className=\"alert alert-warning mb-3 mt-3\" role=\"alert\">\n                    <i className=\"fa fa-cogs\" aria-hidden=\"true\"></i> Waiting\n                    for worker ...\n                  </div>\n                )}\n              {waiting && workerState === WorkerState.Starting && (\n                <div className=\"alert alert-success mb-3 mt-3\" role=\"alert\">\n                  <i className=\"fa fa-cogs\" aria-hidden=\"true\"></i> Initializing\n                  worker ...\n                </div>\n              )}\n              {watchMode && (\n                <div className=\"alert alert-secondary mb-3 mt-3\" role=\"alert\">\n                  <i className=\"fa fa-refresh\" aria-hidden=\"true\"></i> Notebook\n                  in watch mode. All changes to Notebook will be automatically\n                  visible in Mercury.\n                </div>\n              )}\n\n              {isPresentation && (\n                <div className=\"alert alert-primary mb-3\" role=\"alert\">\n                  <i className=\"fa fa-television\" aria-hidden=\"true\"></i> Click\n                  on presentation and press <b>F</b> for full screen. Press{\" \"}\n                  <b>Esc</b> to quit.\n                  <br />\n                  <br />\n                  <i className=\"fa fa-arrows\" aria-hidden=\"true\"></i> Click on\n                  presentation and press <b>Esc</b> to navigate slides.\n                </div>\n              )}\n\n              {/* {notebookParseErrors && (\n                <div className=\"alert alert-danger mb-3\" role=\"alert\">\n                  <i\n                    className=\"fa fa-exclamation-circle\"\n                    aria-hidden=\"true\"\n                  ></i>{\" \"}\n                  <b>Errors in the YAML</b>\n                  <br />\n                  {notebookParseErrors}\n                </div>\n              )} */}\n            </form>\n          </div>\n\n          {showFiles && (\n            <div>\n              <hr />\n              <button\n                className=\"btn btn-sm btn-outline-secondary\"\n                style={{\n                  border: \"none\",\n                  //fontWeight: 500,\n                }}\n                onClick={() => {\n                  dispatch(setView(\"app\"));\n                }}\n              >\n                <i className=\"fa fa-laptop\" aria-hidden=\"true\"></i> App\n              </button>\n\n              <button\n                className=\"btn btn-sm btn-outline-secondary\"\n                style={{\n                  border: \"none\",\n                  //fontWeight: 500,\n                }}\n                onClick={() => {\n                  dispatch(setView(\"files\"));\n                }}\n              >\n                <i className=\"fa fa-folder-open-o\" aria-hidden=\"true\"></i>{\" \"}\n                Output Files\n              </button>\n            </div>\n          )}\n\n          <div>\n            <hr />\n            <div style={{ paddingLeft: \"10px\" }}>\n              <WebSocketStateBar\n                notebookId={notebookId}\n                notebookPath={notebookPath}\n                notebookTitle={notebookTitle}\n                staticNotebook={staticNotebook}\n                allowDownload={allowDownload}\n                allowShare={allowShare}\n                waiting={waiting}\n                continuousUpdate={continuousUpdate}\n                runDownloadHTML={runDownloadHTML}\n                runDownloadPDF={runDownloadPDF}\n              />{\" \"}\n            </div>\n          </div>\n        </div>\n      </BlockUi>\n    </nav>\n  );\n}\n",
         "/* eslint-disable jsx-a11y/anchor-is-valid */\nimport React, { useEffect } from \"react\";\nimport axios from \"axios\";\nimport useWindowDimensions from \"./WindowDimensions\";\n\nimport BlockUi from \"react-block-ui\";\nimport { useDispatch, useSelector } from \"react-redux\";\nimport { getNotebookSrc, setNotebookSrc } from \"../slices/wsSlice\";\n\nimport InnerHTML from \"dangerously-set-html-content\";\nimport { getSelectedNotebook } from \"../slices/notebooksSlice\";\nimport { Link } from \"react-router-dom\";\n\ntype MainViewProps = {\n  appView: string;\n  loadingState: string;\n  notebookPath: string;\n  waiting: boolean;\n  errorMsg: string;\n  watchMode: boolean;\n  displayEmbed: boolean;\n  username: string;\n  slidesHash: string;\n  columnsWidth: number;\n  isPresentation: boolean;\n  fullScreen: boolean;\n};\n\nexport default function MainView({\n  appView,\n  loadingState,\n  notebookPath,\n  waiting,\n  errorMsg,\n  watchMode,\n  displayEmbed,\n  username,\n  slidesHash,\n  columnsWidth,\n  isPresentation,\n  fullScreen,\n}: MainViewProps) {\n  const { height } = useWindowDimensions();\n\n  const iframeHeight = displayEmbed ? height - 10 : height - 58;\n  const dispatch = useDispatch();\n  let nb = useSelector(getSelectedNotebook);\n  let notebookSrc = useSelector(getNotebookSrc);\n\n  let showCode = false;\n  if (nb !== undefined && nb.params !== undefined) {\n    if (\n      nb.params[\"show-code\"] !== undefined &&\n      nb.params[\"show-code\"] !== null\n    ) {\n      showCode = nb.params[\"show-code\"];\n    }\n  }\n\n  if (notebookSrc !== \"\" && !isPresentation) {\n    notebookSrc = \"<script>init_mathjax();</script>\" + notebookSrc;\n\n    if (!showCode) {\n      const hideCodeStyle = `<style type=\"text/css\">\n      .jp-mod-noOutputs {\n          padding: 0px; \n      }\n      .jp-mod-noInput {\n        padding-top: 0px;\n        padding-bottom: 0px;\n      }\n      </style>`;\n      notebookSrc = hideCodeStyle + notebookSrc;\n    }\n  }\n\n  if (notebookSrc !== \"\" && isPresentation && slidesHash !== \"\") {\n    if (notebookSrc.indexOf(\"Reveal.slide(\") === -1) {\n      const splitted = slidesHash.split(\"/\");\n      let injectCode = \"\";\n      if (splitted.length === 4) {\n        injectCode = `Reveal.slide(${splitted[1]}, ${splitted[2]}, ${splitted[3]});`;\n      } else if (splitted.length === 3) {\n        injectCode = `Reveal.slide(${splitted[1]}, ${splitted[2]});`;\n      } else if (splitted.length === 2) {\n        injectCode = `Reveal.slide(${splitted[1]});`;\n      }\n\n      if (injectCode !== \"\") {\n        notebookSrc = notebookSrc.replace(\n          \"setScrollingSlide);\",\n          `setScrollingSlide); Reveal.on( 'ready', event => { try{ Reveal.configure({transition: \"none\"}); ${injectCode} Reveal.configure({transition: \"slide\"}); } catch(error) {} } );`\n        );\n      }\n    }\n  }\n\n  useEffect(() => {\n    if (notebookPath !== undefined && notebookSrc === \"\") {\n      let nbPath = notebookPath;\n\n      if (window.location.origin === \"http://localhost:3000\") {\n        if (nbPath.startsWith(\"/media\")) {\n          nbPath = \"http://127.0.0.1:8000\" + nbPath;\n        }\n      }\n      if (window.location.origin.startsWith(\"https\")) {\n        nbPath = nbPath.replace(\"http://\", \"https://\");\n      }\n\n      let token = axios.defaults.headers.common[\"Authorization\"];\n      if (nbPath.includes(\"s3.amazonaws.com\")) {\n        // we cant do requests to s3 with auth token\n        // we need to remove auth token before request\n        delete axios.defaults.headers.common[\"Authorization\"];\n      }\n      axios.get(`${nbPath}${slidesHash}`).then((response) => {\n        let nbSrc = response.data;\n        if (!isPresentation) {\n          nbSrc = nbSrc.replace(/<head>[\\s\\S]*?<\\/head>/, \"\");\n          nbSrc = nbSrc.replace(\"<html>\", \"\");\n          nbSrc = nbSrc.replace(\"</html>\", \"\");\n          nbSrc = nbSrc.replace(\"<body\", \"<div\");\n          nbSrc = nbSrc.replace(\"</body>\", \"</div>\");\n          nbSrc = nbSrc.replace(\"<!DOCTYPE html>\", \"\");\n        }\n        dispatch(setNotebookSrc(nbSrc));\n      });\n      if (nbPath.includes(\"s3.amazonaws.com\")) {\n        // after request we set token back\n        axios.defaults.headers.common[\"Authorization\"] = token;\n      }\n    }\n  }, [dispatch, notebookPath, slidesHash, isPresentation, notebookSrc]);\n\n  let mainStyle = {\n    paddingTop: \"0px\",\n    paddingRight: \"0px\",\n    paddingLeft: fullScreen ? \"12px\" : \"0px\",\n    display: appView === \"files\" ? \"none\" : \"block\",\n  };\n\n  let divStyle = {};\n  if (!fullScreen) {\n    divStyle = { maxWidth: \"1140px\", margin: \"auto\" };\n  }\n\n  // hide blocking for small screens when sidebar is only showed\n  // because it causes some strange shadow\n  // see https://github.com/mljar/mercury/issues/250\n  let hideBlockUi = false;\n  if (columnsWidth < 12 && window.innerWidth < 992) {\n    hideBlockUi = true;\n  }\n\n  return (\n    <main className={`ms-sm-auto col-${columnsWidth}`} style={mainStyle}>\n      <BlockUi tag=\"div\" blocking={!hideBlockUi && waiting}>\n        <div style={divStyle}>\n          {loadingState === \"loading\" && !watchMode && (\n            <p>Loading notebook. Please wait ...</p>\n          )}\n          {loadingState === \"error\" && (\n            <p style={{ margin: \"20px\" }}>\n              Problem while loading notebook. Please try again later or contact\n              Mercury administrator.\n            </p>\n          )}\n\n          {loadingState === \"error\" && username === \"\" && (\n            <p style={{ margin: \"20px\" }}>\n              <h5>Please log in to see the notebook</h5>\n              <Link to=\"/login\" className=\"btn btn-primary btn-sm\" reloadDocument>\n                <i className=\"fa fa-sign-in\" aria-hidden=\"true\"></i> Log in\n              </Link>\n            </p>\n          )}\n\n          {errorMsg && (\n            <div className=\"alert alert-danger mb-3\" role=\"alert\">\n              <b>Notebook is executed with errors.</b>\n              <p>{errorMsg}</p>\n            </div>\n          )}\n\n          {errorMsg === \"\" &&\n            loadingState !== \"loading\" &&\n            isPresentation &&\n            notebookSrc !== \"\" && (\n              <iframe\n                width=\"100%\"\n                height={iframeHeight}\n                key={notebookPath}\n                srcDoc={notebookSrc}\n                title=\"display\"\n                id=\"main-iframe\"\n                onError={() => {\n                  console.log(\"iframe error\");\n                }}\n              ></iframe>\n            )}\n\n          {notebookSrc !== \"\" && !isPresentation && (\n            <InnerHTML html={notebookSrc} />\n          )}\n        </div>\n      </BlockUi>\n      \n    </main>\n  );\n}\n",
         "import axios from \"axios\";\nimport fileDownload from \"js-file-download\";\n\ntype Props = {\n  fname: string;\n  downloadLink: string;\n  firstItem: boolean;\n  lastItem: boolean;\n};\n\nexport default function FileItem({\n  fname,\n  downloadLink,\n  firstItem,\n  lastItem,\n}: Props) {\n  const handleDownload = (url: string, filename: string) => {\n    let token = axios.defaults.headers.common[\"Authorization\"];\n\n    if (url.includes(\"s3.amazonaws.com\")) {\n      // we cant do requests to s3 with auth token\n      // we need to remove auth token before request\n      delete axios.defaults.headers.common[\"Authorization\"];\n    }\n\n    axios\n      .get(url, {\n        responseType: \"blob\",\n      })\n      .then((res) => {\n        fileDownload(res.data, filename);\n      });\n\n    if (url.includes(\"s3.amazonaws.com\")) {\n      // after request we set token back\n      axios.defaults.headers.common[\"Authorization\"] = token;\n    }\n  };\n\n  return (\n    <div\n      style={{\n        border: \"1px solid #ddd\",\n        marginBottom: \"-1px\",\n        padding: \"13px\",\n        borderTopRightRadius: firstItem ? \"7px\" : \"0px\",\n        borderTopLeftRadius: firstItem ? \"7px\" : \"0px\",\n        borderBottomRightRadius: lastItem ? \"7px\" : \"0px\",\n        borderBottomLeftRadius: lastItem ? \"7px\" : \"0px\",\n      }}\n    >\n      <i\n        className=\"fa fa-file-text-o\"\n        aria-hidden=\"true\"\n        style={{ paddingRight: \"5px\" }}\n      ></i>{\" \"}\n      {fname}\n      <div style={{ float: \"right\", margin: \"-4px\" }}>\n        <button\n          style={{ float: \"right\" }}\n          type=\"button\"\n          className=\"btn btn-outline-primary btn-sm\"\n          onClick={() => handleDownload(downloadLink, fname!)}\n        >\n          <i className=\"fa fa-download\" aria-hidden=\"true\"></i> Download\n        </button>\n      </div>\n    </div>\n  );\n}\n",
         "/* eslint-disable jsx-a11y/anchor-is-valid */\nimport React from \"react\";\nimport { useDispatch } from \"react-redux\";\nimport axios from \"axios\";\nimport BlockUi from \"react-block-ui\";\nimport { setView } from \"../slices/appSlice\";\nimport FileItem from \"./FileItem\";\n\ntype FilesViewProps = {\n  files: string[];\n  filesState: string;\n  waiting: boolean;\n};\n\nexport default function FilesView({\n  files,\n  filesState,\n  waiting,\n}: FilesViewProps) {\n  const dispatch = useDispatch();\n\n  let filesLinks = [];\n\n  for (let f of files) {\n    let fname = f.split(\"/\").pop();\n    fname = fname?.split(\"?\")[0];\n\n    if (f && fname) {\n      let downloadLink = `${axios.defaults.baseURL}${f}`;\n      if (f.includes(\"s3.amazonaws.com\")) {\n        downloadLink = f;\n      }\n      filesLinks.push(\n        <FileItem\n          fname={fname}\n          downloadLink={downloadLink}\n          firstItem={f === files[0]}\n          lastItem={f === files[files.length - 1]}\n        />\n      );\n    }\n  }\n\n  return (\n    <main className=\"col-md-9 ms-sm-auto col-lg-9\" style={{ padding: \"20px\" }}>\n      <div className=\"col-12\" style={{ maxWidth: \"900px\" }}>\n        <h3 style={{ paddingBottom: \"10px\" }}>\n          <i className=\"fa fa-folder-open-o\" aria-hidden=\"true\"></i> Output\n          Files\n        </h3>\n        <BlockUi tag=\"div\" blocking={waiting}>\n          <div>\n            {filesState === \"loaded\" && filesLinks}\n            {filesState === \"loaded\" && filesLinks.length === 0 && (\n              <div>No files available for download</div>\n            )}\n            {filesState === \"unknown\" && (\n              <p>Please run the notebook to produce output files ...</p>\n            )}\n            {filesState === \"loading\" && <p>Loading files please wait ...</p>}\n            {filesState === \"error\" && (\n              <div className=\"alert alert-danger mb-3\" role=\"alert\">\n                There was an error during loading files. Please try to run the\n                app again or contact the administrator.\n              </div>\n            )}\n          </div>\n        </BlockUi>\n      </div>\n\n      <button\n        className=\"btn btn-secondary btn-sm\"\n        style={{ marginTop: \"20px\" }}\n        onClick={() => {\n          dispatch(setView(\"app\"));\n        }}\n      >\n        <i className=\"fa fa-arrow-left\" aria-hidden=\"true\"></i> Back to App\n      </button>\n    </main>\n  );\n}\n",
         "import React from \"react\";\n\nexport default function MadeWithDiv() {\n  return (\n    <a href=\"https://runmercury.com\" target=\"_blank\" rel=\"noreferrer\">\n      <div className=\"poweredby\">\n        <div className=\"text-center\">\n          {\" \"}\n          <b style={{ fontSize: \"0.9em\" }}>created with</b>{\" \"}\n        </div>\n        <div>\n          <img\n            alt=\"Mercury\"\n            src={\n              process.env.PUBLIC_URL +\n              process.env.REACT_APP_LOCAL_URL +\n              \"/mercury_black_logo.svg\"\n            }\n            style={{ height: \"27px\" }}\n          />\n        </div>\n      </div>\n    </a>\n  );\n}\n",
         "/* eslint-disable jsx-a11y/anchor-is-valid */\nimport React, { useEffect, useState } from \"react\";\nimport axios from \"axios\";\nimport { IWidget } from \"../widgets/Types\";\nimport { useSelector } from \"react-redux\";\nimport { getWidgetsValues } from \"../slices/notebooksSlice\";\n\ntype Props = {\n  slug: string;\n  widgetsParams: Record<string, IWidget>;  \n  notebookPath: string;\n  columnsWidth: number;\n  taskSessionId: string | undefined;\n};\n\nexport default function RestAPIView({\n  slug,\n  widgetsParams,\n  notebookPath,\n  columnsWidth,\n  taskSessionId,\n}: Props) {\n  const [response, setResponse] = useState(\n    JSON.stringify({ msg: \"Example output\" })\n  );\n  const widgetsValues = useSelector(getWidgetsValues);\n\n  let examplePostData = {} as Record<\n    string,\n    | string\n    | number\n    | null\n    | undefined\n    | boolean\n    | [number, number]\n    | string[]\n    | unknown\n  >;\n  for (let [key, widgetParams] of Object.entries(widgetsParams)) {\n    if (widgetParams.input) {\n      examplePostData[key] = widgetsValues[key];\n    }\n  }\n\n  async function fetchResponse() {\n    try {\n      const { data } = await axios.get(`get/${taskSessionId}`);\n      setResponse(JSON.stringify(data));\n    } catch (error) {}\n  }\n\n  useEffect(() => {\n    if (taskSessionId) {\n      fetchResponse();\n    }\n    // eslint-disable-next-line react-hooks/exhaustive-deps\n  }, [taskSessionId, notebookPath]);\n\n  let sessionId = \"id-with-some-random-string\";\n  if (taskSessionId) {\n    sessionId = taskSessionId;\n  }\n\n  let postRequest = `curl -X POST -H \"Content-Type: application/json\" -d '${JSON.stringify(\n    examplePostData\n  )}' ${axios.defaults.baseURL}/run/${slug}`;\n  return (\n    <div\n      className={`ms-sm-auto col-lg-${columnsWidth}`}\n      style={{\n        border: \"none\",\n        paddingTop: \"0px\",\n        paddingRight: \"0px\",\n        paddingLeft: \"0px\",\n        padding: \"10px\",\n      }}\n    >\n      <h4>Notebook as REST API</h4>\n      <p>\n        This notebook can be executed as REST API. Please see the examples below\n        on how to access the notebook.\n      </p>\n\n      <div className=\"alert alert-secondary\" role=\"alert\">\n        <h5>POST request to execute the notebook</h5>\n        <textarea\n          disabled\n          style={{ width: \"100%\" }}\n          rows={3}\n          value={postRequest}\n        ></textarea>\n        The above request should return a JSON with `id`. The `id` should be\n        used in the GET request to fetch the result.\n        <br />\n        Example response:\n        <pre>{`{\"id\": \"${sessionId}\"}`}</pre>\n      </div>\n      <div className=\"alert alert-secondary\" role=\"alert\">\n        <h5>GET request to get execution result in JSON</h5>\n        <textarea\n          disabled\n          style={{ width: \"100%\" }}\n          rows={1}\n          value={`curl ${axios.defaults.baseURL}/get/${sessionId}`}\n        ></textarea>\n      </div>\n\n      <div className=\"alert alert-primary\" role=\"alert\">\n        <h5>Response</h5>\n        <pre>{response}</pre>\n      </div>\n    </div>\n  );\n}\n",
         "import React, { useEffect } from \"react\";\nimport { useDispatch, useSelector } from \"react-redux\";\nimport { toast } from \"react-toastify\";\nimport { getExportingToPDF, getExportToPDFCounter, getExportToPDFJobId, getPDF, stopPDFExport } from \"../slices/tasksSlice\";\n\nexport default function WaitPDFExport() {\n  const dispatch = useDispatch();\n  const counter = useSelector(getExportToPDFCounter);\n  const jobId = useSelector(getExportToPDFJobId);\n  const exportingPDF = useSelector(getExportingToPDF);\n\n  useEffect(() => {\n    if(jobId === '') {\n      return;\n    } \n    if(!exportingPDF) {\n      return;\n    }\n    // raise error after 2 minutes of waiting ...\n    if (counter < 120) {\n      setTimeout(() => {\n        dispatch(getPDF(jobId));\n      }, 1000); // every 1 second\n    } else {\n      dispatch(stopPDFExport());\n      toast.error(\"Problem with PDF export. Please try again later or ask your admin for help.\", { autoClose: 6000 })\n    }\n  }, [dispatch, counter, jobId, exportingPDF]);\n\n  return <div></div>;\n}\n",
         "import React from \"react\";\nimport { useDispatch, useSelector } from \"react-redux\";\nimport {\n  isCheckboxWidget,\n  isNumericWidget,\n  isRangeWidget,\n  isSelectWidget,\n  isSliderWidget,\n  isTextWidget,\n  IWidget,\n} from \"../widgets/Types\";\nimport { getWidgetsValues, WidgetValueType } from \"../slices/notebooksSlice\";\nimport { getShowShareDialog, setShowShareDialog } from \"../slices/appSlice\";\n\ntype Props = {\n  //widgetsValues: Record<string, WidgetValueType>;\n  widgetsParams: Record<string, IWidget>;\n};\n\nexport default function ShareDialog({\n  //widgetsValues,\n  widgetsParams,\n}: Props) {\n  const dispatch = useDispatch();\n  const showShareDialog = useSelector(getShowShareDialog);\n  const widgetsValues: Record<string, WidgetValueType> = useSelector(\n    getWidgetsValues\n  ) as Record<string, WidgetValueType>;\n\n  let noUrlKeys = true;\n  let urlParams = \"?\";\n  if (\n    widgetsParams !== undefined &&\n    widgetsParams !== null &&\n    widgetsValues !== undefined &&\n    widgetsValues !== null\n  ) {\n    for (let [key, widgetParams] of Object.entries(widgetsParams)) {\n      if (widgetsValues[key] === undefined) {\n        continue;\n      }\n\n      if (\n        isCheckboxWidget(widgetParams) ||\n        isNumericWidget(widgetParams) ||\n        isRangeWidget(widgetParams) ||\n        isSelectWidget(widgetParams) ||\n        isSliderWidget(widgetParams) ||\n        isTextWidget(widgetParams)\n      ) {\n        if (widgetParams?.url_key !== null && widgetParams?.url_key !== \"\") {\n          noUrlKeys = false;\n        }\n      }\n\n      if (\n        isCheckboxWidget(widgetParams) ||\n        isNumericWidget(widgetParams) ||\n        isSliderWidget(widgetParams) ||\n        isTextWidget(widgetParams)\n      ) {\n        if (widgetParams?.url_key !== null && widgetParams?.url_key !== \"\") {\n          urlParams += `${widgetParams?.url_key}=${widgetsValues[key]}&`;\n        }\n      }\n\n      if (isRangeWidget(widgetParams)) {\n        if (widgetParams?.url_key !== null && widgetParams?.url_key !== \"\") {\n          const v = widgetsValues[key] as [number, number];\n\n          urlParams += `${widgetParams?.url_key}=${v[0]},${v[1]}&`;\n        }\n      }\n      if (isSelectWidget(widgetParams)) {\n        if (widgetParams?.url_key !== null && widgetParams?.url_key !== \"\") {\n          if (widgetParams?.multi) {\n            const v = widgetsValues[key] as string[];\n\n            urlParams += `${widgetParams?.url_key}=${v.join(\",\")}&`;\n          } else {\n            const v = widgetsValues[key] as string;\n            urlParams += `${widgetParams?.url_key}=${v}&`;\n          }\n        }\n      }\n    }\n    if (urlParams !== \"?\") {\n      urlParams = urlParams.slice(0, urlParams.length - 1);\n    }\n  }\n\n  return (\n    <div\n      className=\"\"\n      style={{\n        position: \"fixed\",\n        top: \"0\",\n        left: \"0\",\n        width: \"100%\",\n        height: \"100%\",\n        background: \"rgba(0, 0, 0, 0.6)\",\n        display: showShareDialog ? \"block\" : \"none\",\n        zIndex: 100\n      }}\n    >\n      <section\n        className=\"\"\n        style={{\n          position: \"fixed\",\n          width: \"100%\",\n          height: \"auto\",\n          top: \"50%\",\n          left: \"50%\",\n          transform: \"translate(-50%,-50%)\",\n        }}\n      >\n        <div className=\"modal-dialog\">\n          <div className=\"modal-content\">\n            <div className=\"modal-header\">\n              <h3 className=\"modal-title\">\n                <svg\n                  xmlns=\"http://www.w3.org/2000/svg\"\n                  width=\"24\"\n                  height=\"24\"\n                  viewBox=\"0 0 24 24\"\n                  strokeWidth=\"2\"\n                  stroke=\"currentColor\"\n                  fill=\"none\"\n                  strokeLinecap=\"round\"\n                  strokeLinejoin=\"round\"\n                >\n                  <path stroke=\"none\" d=\"M0 0h24v24H0z\" fill=\"none\"></path>\n                  <path d=\"M6 12m-3 0a3 3 0 1 0 6 0a3 3 0 1 0 -6 0\"></path>\n                  <path d=\"M18 6m-3 0a3 3 0 1 0 6 0a3 3 0 1 0 -6 0\"></path>\n                  <path d=\"M18 18m-3 0a3 3 0 1 0 6 0a3 3 0 1 0 -6 0\"></path>\n                  <path d=\"M8.7 10.7l6.6 -3.4\"></path>\n                  <path d=\"M8.7 13.3l6.6 3.4\"></path>\n                </svg>{\" \"}\n                Share\n              </h3>\n              <button\n                type=\"button\"\n                className=\"btn-close\"\n                aria-label=\"Close\"\n                onClick={() => dispatch(setShowShareDialog(false))}\n              ></button>\n            </div>\n            <div className=\"modal-body\">\n              <div className=\"py-2\">\n                <label>App address</label>\n                <input\n                  type=\"text\"\n                  className=\"form-control\"\n                  disabled={true}\n                  value={window.location.origin + window.location.pathname}\n                ></input>\n              </div>\n\n              {!noUrlKeys && (\n                <div className=\"py-2\">\n                  <label>App address with current paramters</label>\n                  <textarea\n                    rows={5}\n                    className=\"form-control\"\n                    disabled={true}\n                    value={window.location.origin + window.location.pathname + urlParams}\n                  />\n                </div>\n              )}\n              {noUrlKeys && (\n                <div className=\"py-2\">\n                  There are no <code>url_key</code> defined for any widget. You\n                  can easily share URL to your notebook with preset values by\n                  using <code>url_key</code> in the widget. Please check{\" \"}\n                  <a\n                    href=\"https://runmercury.com/docs/input-widgets/\"\n                    target=\"_blank\"\n                    rel=\"noreferrer\"\n                  >\n                    documentation\n                  </a>\n                  .\n                </div>\n              )}\n              <div className=\"py-2\"></div>\n            </div>\n            <div className=\"modal-footer\">\n              <button\n                type=\"button\"\n                className=\"btn btn-secondary\"\n                onClick={() => dispatch(setShowShareDialog(false))}\n              >\n                Close\n              </button>\n            </div>\n          </div>\n        </div>\n      </section>\n    </div>\n  );\n}\n",
         "export default process.env.PUBLIC_URL +\n  process.env.REACT_APP_LOCAL_URL +\n  \"/mercury_logo.svg\";\n",
-        "import React, { useEffect, useState } from \"react\";\nimport { useDispatch, useSelector } from \"react-redux\";\nimport \"./App.css\";\nimport NavBar from \"../components/NavBar\";\nimport SideBar from \"../components/SideBar\";\nimport MainView from \"../components/MainView\";\n\nimport {\n  fetchNotebookWithSlug,\n  getLoadingStateSelected,\n  getSelectedNotebook,\n  getSlidesHash,\n  // getWatchModeCounter,\n} from \"../slices/notebooksSlice\";\nimport {\n  //fetchCurrentTask,\n  //fetchExecutionHistory,\n  getCurrentTask,\n  getExportingToPDF,\n  getHistoricTask,\n  getPreviousTask,\n  //ITask,\n  //setPreviousTask,\n} from \"../slices/tasksSlice\";\nimport { isOutputFilesWidget, IWidget } from \"../widgets/Types\";\nimport {\n  fetchWorkerOutputFiles,\n  getOutputFiles,\n  getOutputFilesState,\n  getShowSideBar,\n  getView,\n  setShowSideBar,\n} from \"../slices/appSlice\";\nimport FilesView from \"../components/FilesView\";\nimport { getToken, getUsername } from \"../slices/authSlice\";\nimport MadeWithDiv from \"../components/MadeWithDiv\";\nimport RestAPIView from \"../components/RestAPIView\";\nimport BlockUi from \"react-block-ui\";\nimport WaitPDFExport from \"../components/WaitPDFExport\";\nimport { getWorkerId, getWorkerState, WorkerState } from \"../slices/wsSlice\";\nimport {\n  getLogoFilename,\n  getNavbarColor,\n  getSiteId,\n  isPublic,\n} from \"../slices/sitesSlice\";\nimport ShareDialog from \"../components/ShareDialog\";\nimport axios from \"axios\";\nimport DefaultLogoSrc from \"../components/DefaultLogo\";\n\ntype AppProps = {\n  isSingleApp: boolean;\n  notebookSlug: string;\n  displayEmbed: boolean;\n};\n\nfunction App({ isSingleApp, notebookSlug, displayEmbed }: AppProps) {\n  const dispatch = useDispatch();\n  const notebook = useSelector(getSelectedNotebook);\n  const loadingState = useSelector(getLoadingStateSelected);\n  const task = useSelector(getCurrentTask);\n  const historicTask = useSelector(getHistoricTask);\n  const previousTask = useSelector(getPreviousTask);\n  const appView = useSelector(getView);\n  const outputFiles = useSelector(getOutputFiles);\n  const outputFilesState = useSelector(getOutputFilesState);\n  const username = useSelector(getUsername);\n  const token = useSelector(getToken);\n  const slidesHash = useSelector(getSlidesHash);\n  const showSideBar = useSelector(getShowSideBar);\n  const exportingToPDF = useSelector(getExportingToPDF);\n  const workerId = useSelector(getWorkerId);\n  const workerState = useSelector(getWorkerState);\n  const siteId = useSelector(getSiteId);\n  const isSitePublic = useSelector(isPublic);\n  const navbarColor = useSelector(getNavbarColor);\n  const [logoSrc, setLogoSrc] = useState(\"loading\");\n  const logoFilename = useSelector(getLogoFilename);\n\n  const pleaseWait = () => {\n    if (notebook?.params?.static_notebook) {\n      return false;\n    }\n    if (\n      workerState === WorkerState.UsageLimitReached ||\n      workerState === WorkerState.MaxIdleTimeReached ||\n      workerState === WorkerState.MaxRunTimeReached\n    ) {\n      return false;\n    }\n    return workerState !== WorkerState.Running;\n  };\n\n  const isWatchMode = () => {\n    return (\n      notebook.state === \"WATCH_READY\" ||\n      notebook.state === \"WATCH_WAIT\" ||\n      notebook.state === \"WATCH_ERROR\"\n    );\n  };\n\n  useEffect(() => {\n    if (siteId !== undefined) {\n      dispatch(fetchNotebookWithSlug(siteId, notebookSlug));\n    }\n  }, [dispatch, siteId, notebookSlug, token]);\n\n  useEffect(() => {\n    if (\n      appView === \"files\" &&\n      notebook?.params?.version === \"2\" &&\n      workerId !== undefined &&\n      notebook.id !== undefined\n    ) {\n      dispatch(fetchWorkerOutputFiles(workerId, notebook.id));\n    }\n  }, [dispatch, appView, notebook, workerId]);\n\n  let notebookPath = notebook.default_view_path;\n  if (task.state && task.state === \"DONE\" && task.result) {\n    notebookPath = task.result;\n  }\n  let errorMsg = \"\";\n  if (task.state && task.result && task.state === \"ERROR\") {\n    errorMsg = task.result;\n  }\n\n  // set historic task to display if available\n  if (\n    historicTask.state &&\n    historicTask.state === \"DONE\" &&\n    historicTask.result\n  ) {\n    notebookPath = historicTask.result;\n  }\n  if (\n    historicTask.state &&\n    historicTask.result &&\n    historicTask.state === \"ERROR\"\n  ) {\n    errorMsg = historicTask.result;\n  }\n\n  // if we have previous task to show, just show it\n  if (\n    notebookPath === notebook.default_view_path &&\n    previousTask.state &&\n    previousTask.state === \"DONE\" &&\n    previousTask.result\n  ) {\n    notebookPath = previousTask.result;\n  }\n\n  const areOutputFilesAvailable = (\n    widgetsParams: Record<string, IWidget>\n  ): boolean => {\n    if (widgetsParams) {\n      for (let [, widgetParams] of Object.entries(widgetsParams)) {\n        if (isOutputFilesWidget(widgetParams)) {\n          return true;\n        }\n      }\n    }\n    return false;\n  };\n\n  let showRestApi = false;\n  if (notebook.output && notebook.output.toLowerCase().startsWith(\"rest\")) {\n    showRestApi = true;\n  }\n\n  const isFullScreen = () => {\n    if (notebook !== undefined && notebook !== null) {\n      return notebook?.params?.full_screen !== undefined &&\n        notebook?.params?.full_screen !== null\n        ? notebook.params.full_screen\n        : true;\n    }\n    return true;\n  };\n\n  const doAllowDownload = () => {\n    if (notebook !== undefined && notebook !== null) {\n      return notebook?.params?.allow_download !== undefined &&\n        notebook?.params?.allow_download !== null\n        ? notebook.params.allow_download\n        : true;\n    }\n    return true;\n  };\n\n  useEffect(() => {\n    if (logoFilename === \"\") {\n      setLogoSrc(DefaultLogoSrc);\n    } else {\n      axios\n        .get(`/api/v1/get-style/${siteId}/${logoFilename}`)\n        .then((response) => {\n          const { url } = response.data;\n          setLogoSrc(url);\n        });\n    }\n  }, [dispatch, logoFilename, siteId]);\n\n  return (\n    <div className=\"App\">\n      {!displayEmbed && (\n        <NavBar\n          isSitePublic={isSitePublic}\n          username={username}\n          logoSrc={logoSrc}\n          navbarColor={navbarColor}\n        />\n      )}\n      <BlockUi\n        blocking={exportingToPDF}\n        message=\"Exporting to PDF. Please wait ...\"\n      >\n        {exportingToPDF && <WaitPDFExport />}\n        <div className=\"container-fluid\">\n          <div className=\"row\">\n            {/* {notebook.schedule !== undefined && notebook.schedule !== \"\" && (\n              <AutoRefresh notebookId={notebookId} />\n            )} */}\n\n            {showSideBar && (\n              <SideBar\n                notebookTitle={notebook.title}\n                notebookId={notebook.id}\n                notebookSchedule={notebook.schedule}\n                taskCreatedAt={task.created_at}\n                loadingState={loadingState}\n                waiting={pleaseWait()}\n                widgetsParams={notebook?.params?.params}\n                watchMode={isWatchMode()}\n                notebookPath={notebookPath}\n                displayEmbed={displayEmbed}\n                showFiles={areOutputFilesAvailable(notebook?.params?.params)}\n                isPresentation={\n                  notebook.output !== undefined && notebook.output === \"slides\"\n                }\n                notebookParseErrors={notebook.errors}\n                continuousUpdate={notebook?.params?.continuous_update}\n                staticNotebook={notebook?.params?.static_notebook}\n                allowDownload={doAllowDownload()}\n              />\n            )}\n\n            {!showSideBar && (\n              <div>\n                <button\n                  className=\"btn btn-sm  btn-outline-primary\"\n                  type=\"button\"\n                  style={{\n                    position: \"absolute\",\n                    top: displayEmbed ? \"5px\" : \"50px\",\n                    left: \"5px\",\n                    zIndex: \"2000\",\n                  }}\n                  onClick={() => dispatch(setShowSideBar(true))}\n                  data-toggle=\"tooltip\"\n                  data-placement=\"right\"\n                  title=\"Show sidebar\"\n                >\n                  <i className=\"fa fa-chevron-right\" aria-hidden=\"true\" />\n                </button>\n              </div>\n            )}\n\n            {showRestApi && (\n              <RestAPIView\n                slug={notebook.slug}\n                widgetsParams={notebook?.params?.params}\n                notebookPath={notebookPath}\n                columnsWidth={showSideBar ? 9 : 12}\n                taskSessionId={task.session_id}\n              />\n            )}\n\n            <MainView\n              appView={appView}\n              loadingState={loadingState}\n              notebookPath={notebookPath}\n              errorMsg={errorMsg}\n              waiting={pleaseWait()}\n              watchMode={isWatchMode()}\n              displayEmbed={displayEmbed}\n              username={username}\n              slidesHash={slidesHash}\n              columnsWidth={showSideBar ? 9 : 12}\n              isPresentation={\n                notebook.output !== undefined && notebook.output === \"slides\"\n              }\n              fullScreen={isFullScreen()}\n            />\n\n            {appView === \"files\" && (\n              <FilesView\n                files={outputFiles}\n                filesState={outputFilesState}\n                waiting={pleaseWait()}\n              />\n            )}\n\n            <ShareDialog widgetsParams={notebook?.params?.params} />\n          </div>\n        </div>\n      </BlockUi>\n      {/* dont show created with logo for embedded notebooks when we are using custom logo */}\n      {displayEmbed && logoSrc === DefaultLogoSrc && <MadeWithDiv />}\n    </div>\n  );\n}\n\nconst AppView = App;\nexport default AppView;\n",
+        "import React, { useEffect, useState } from \"react\";\nimport { useDispatch, useSelector } from \"react-redux\";\nimport \"./App.css\";\nimport NavBar from \"../components/NavBar\";\nimport SideBar from \"../components/SideBar\";\nimport MainView from \"../components/MainView\";\n\nimport {\n  fetchNotebookWithSlug,\n  getLoadingStateSelected,\n  getSelectedNotebook,\n  getSlidesHash,\n  // getWatchModeCounter,\n} from \"../slices/notebooksSlice\";\nimport {\n  //fetchCurrentTask,\n  //fetchExecutionHistory,\n  getCurrentTask,\n  getExportingToPDF,\n  getHistoricTask,\n  getPreviousTask,\n  //ITask,\n  //setPreviousTask,\n} from \"../slices/tasksSlice\";\nimport { isOutputFilesWidget, IWidget } from \"../widgets/Types\";\nimport {\n  fetchWorkerOutputFiles,\n  getOutputFiles,\n  getOutputFilesState,\n  getShowSideBar,\n  getView,\n  setShowSideBar,\n} from \"../slices/appSlice\";\nimport FilesView from \"../components/FilesView\";\nimport { getToken, getUsername } from \"../slices/authSlice\";\nimport MadeWithDiv from \"../components/MadeWithDiv\";\nimport RestAPIView from \"../components/RestAPIView\";\nimport BlockUi from \"react-block-ui\";\nimport WaitPDFExport from \"../components/WaitPDFExport\";\nimport { getWorkerId, getWorkerState, WorkerState } from \"../slices/wsSlice\";\nimport {\n  getLogoFilename,\n  getNavbarColor,\n  getSiteId,\n  isPublic,\n} from \"../slices/sitesSlice\";\nimport ShareDialog from \"../components/ShareDialog\";\nimport axios from \"axios\";\nimport DefaultLogoSrc from \"../components/DefaultLogo\";\n\ntype AppProps = {\n  isSingleApp: boolean;\n  notebookSlug: string;\n  displayEmbed: boolean;\n};\n\nfunction App({ isSingleApp, notebookSlug, displayEmbed }: AppProps) {\n  const dispatch = useDispatch();\n  const notebook = useSelector(getSelectedNotebook);\n  const loadingState = useSelector(getLoadingStateSelected);\n  const task = useSelector(getCurrentTask);\n  const historicTask = useSelector(getHistoricTask);\n  const previousTask = useSelector(getPreviousTask);\n  const appView = useSelector(getView);\n  const outputFiles = useSelector(getOutputFiles);\n  const outputFilesState = useSelector(getOutputFilesState);\n  const username = useSelector(getUsername);\n  const token = useSelector(getToken);\n  const slidesHash = useSelector(getSlidesHash);\n  const showSideBar = useSelector(getShowSideBar);\n  const exportingToPDF = useSelector(getExportingToPDF);\n  const workerId = useSelector(getWorkerId);\n  const workerState = useSelector(getWorkerState);\n  const siteId = useSelector(getSiteId);\n  const isSitePublic = useSelector(isPublic);\n  const navbarColor = useSelector(getNavbarColor);\n  const [logoSrc, setLogoSrc] = useState(\"loading\");\n  const logoFilename = useSelector(getLogoFilename);\n\n  const pleaseWait = () => {\n    if (notebook?.params?.static_notebook) {\n      return false;\n    }\n    if (\n      workerState === WorkerState.UsageLimitReached ||\n      workerState === WorkerState.MaxIdleTimeReached ||\n      workerState === WorkerState.MaxRunTimeReached\n    ) {\n      return false;\n    }\n    return workerState !== WorkerState.Running;\n  };\n\n  const isWatchMode = () => {\n    return (\n      notebook.state === \"WATCH_READY\" ||\n      notebook.state === \"WATCH_WAIT\" ||\n      notebook.state === \"WATCH_ERROR\"\n    );\n  };\n\n  useEffect(() => {\n    if (siteId !== undefined) {\n      dispatch(fetchNotebookWithSlug(siteId, notebookSlug));\n    }\n  }, [dispatch, siteId, notebookSlug, token]);\n\n  useEffect(() => {\n    if (\n      appView === \"files\" &&\n      notebook?.params?.version === \"2\" &&\n      workerId !== undefined &&\n      notebook.id !== undefined\n    ) {\n      dispatch(fetchWorkerOutputFiles(workerId, notebook.id));\n    }\n  }, [dispatch, appView, notebook, workerId]);\n\n  let notebookPath = notebook.default_view_path;\n  if (task.state && task.state === \"DONE\" && task.result) {\n    notebookPath = task.result;\n  }\n  let errorMsg = \"\";\n  if (task.state && task.result && task.state === \"ERROR\") {\n    errorMsg = task.result;\n  }\n\n  // set historic task to display if available\n  if (\n    historicTask.state &&\n    historicTask.state === \"DONE\" &&\n    historicTask.result\n  ) {\n    notebookPath = historicTask.result;\n  }\n  if (\n    historicTask.state &&\n    historicTask.result &&\n    historicTask.state === \"ERROR\"\n  ) {\n    errorMsg = historicTask.result;\n  }\n\n  // if we have previous task to show, just show it\n  if (\n    notebookPath === notebook.default_view_path &&\n    previousTask.state &&\n    previousTask.state === \"DONE\" &&\n    previousTask.result\n  ) {\n    notebookPath = previousTask.result;\n  }\n\n  const areOutputFilesAvailable = (\n    widgetsParams: Record<string, IWidget>\n  ): boolean => {\n    if (widgetsParams) {\n      for (let [, widgetParams] of Object.entries(widgetsParams)) {\n        if (isOutputFilesWidget(widgetParams)) {\n          return true;\n        }\n      }\n    }\n    return false;\n  };\n\n  let showRestApi = false;\n  if (notebook.output && notebook.output.toLowerCase().startsWith(\"rest\")) {\n    showRestApi = true;\n  }\n\n  const isFullScreen = () => {\n    if (notebook !== undefined && notebook !== null) {\n      return notebook?.params?.full_screen !== undefined &&\n        notebook?.params?.full_screen !== null\n        ? notebook.params.full_screen\n        : true;\n    }\n    return true;\n  };\n\n  const doAllowDownload = () => {\n    if (notebook !== undefined && notebook !== null) {\n      return notebook?.params?.allow_download !== undefined &&\n        notebook?.params?.allow_download !== null\n        ? notebook.params.allow_download\n        : true;\n    }\n    return true;\n  };\n\n  const doAllowShare = () => {\n    if (notebook !== undefined && notebook !== null) {\n      return notebook?.params?.allow_share !== undefined &&\n        notebook?.params?.allow_share !== null\n        ? notebook.params.allow_share\n        : true;\n    }\n    return true;\n  }\n\n  useEffect(() => {\n    if (logoFilename === \"\") {\n      setLogoSrc(DefaultLogoSrc);\n    } else {\n      axios\n        .get(`/api/v1/get-style/${siteId}/${logoFilename}`)\n        .then((response) => {\n          const { url } = response.data;\n          setLogoSrc(url);\n        });\n    }\n  }, [dispatch, logoFilename, siteId]);\n\n  return (\n    <div className=\"App\">\n      {!displayEmbed && (\n        <NavBar\n          isSitePublic={isSitePublic}\n          username={username}\n          logoSrc={logoSrc}\n          navbarColor={navbarColor}\n        />\n      )}\n      <BlockUi\n        blocking={exportingToPDF}\n        message=\"Exporting to PDF. Please wait ...\"\n      >\n        {exportingToPDF && <WaitPDFExport />}\n        <div className=\"container-fluid\">\n          <div className=\"row\">\n            {/* {notebook.schedule !== undefined && notebook.schedule !== \"\" && (\n              <AutoRefresh notebookId={notebookId} />\n            )} */}\n\n            {showSideBar && (\n              <SideBar\n                notebookTitle={notebook.title}\n                notebookId={notebook.id}\n                notebookSchedule={notebook.schedule}\n                taskCreatedAt={task.created_at}\n                loadingState={loadingState}\n                waiting={pleaseWait()}\n                widgetsParams={notebook?.params?.params}\n                watchMode={isWatchMode()}\n                notebookPath={notebookPath}\n                displayEmbed={displayEmbed}\n                showFiles={areOutputFilesAvailable(notebook?.params?.params)}\n                isPresentation={\n                  notebook.output !== undefined && notebook.output === \"slides\"\n                }\n                notebookParseErrors={notebook.errors}\n                continuousUpdate={notebook?.params?.continuous_update}\n                staticNotebook={notebook?.params?.static_notebook}\n                allowDownload={doAllowDownload()}\n                allowShare={doAllowShare()}\n              />\n            )}\n\n            {!showSideBar && (\n              <div>\n                <button\n                  className=\"btn btn-sm  btn-outline-primary\"\n                  type=\"button\"\n                  style={{\n                    position: \"absolute\",\n                    top: displayEmbed ? \"5px\" : \"50px\",\n                    left: \"5px\",\n                    zIndex: \"2000\",\n                  }}\n                  onClick={() => dispatch(setShowSideBar(true))}\n                  data-toggle=\"tooltip\"\n                  data-placement=\"right\"\n                  title=\"Show sidebar\"\n                >\n                  <i className=\"fa fa-chevron-right\" aria-hidden=\"true\" />\n                </button>\n              </div>\n            )}\n\n            {showRestApi && (\n              <RestAPIView\n                slug={notebook.slug}\n                widgetsParams={notebook?.params?.params}\n                notebookPath={notebookPath}\n                columnsWidth={showSideBar ? 9 : 12}\n                taskSessionId={task.session_id}\n              />\n            )}\n\n            <MainView\n              appView={appView}\n              loadingState={loadingState}\n              notebookPath={notebookPath}\n              errorMsg={errorMsg}\n              waiting={pleaseWait()}\n              watchMode={isWatchMode()}\n              displayEmbed={displayEmbed}\n              username={username}\n              slidesHash={slidesHash}\n              columnsWidth={showSideBar ? 9 : 12}\n              isPresentation={\n                notebook.output !== undefined && notebook.output === \"slides\"\n              }\n              fullScreen={isFullScreen()}\n            />\n\n            {appView === \"files\" && (\n              <FilesView\n                files={outputFiles}\n                filesState={outputFilesState}\n                waiting={pleaseWait()}\n              />\n            )}\n\n            <ShareDialog widgetsParams={notebook?.params?.params} />\n          </div>\n        </div>\n      </BlockUi>\n      {/* dont show created with logo for embedded notebooks when we are using custom logo */}\n      {displayEmbed && logoSrc === DefaultLogoSrc && <MadeWithDiv />}\n    </div>\n  );\n}\n\nconst AppView = App;\nexport default AppView;\n",
         "import { useParams } from \"react-router-dom\";\nimport AppView from \"./AppView\";\n\nexport default function MyApp() {\n  const { slug } = useParams<{ slug: string }>();\n  const { embed } = useParams<{ embed: string }>();\n  const displayEmbed = !!(embed && embed === \"embed\");\n\n  return (\n    <AppView\n      isSingleApp={false}\n      notebookSlug={slug as string}\n      displayEmbed={displayEmbed}\n    />\n  );\n}\n",
         "import React from \"react\";\n\ntype FooterProps = {\n  footerText: string;\n};\n\nexport default function Footer({ footerText }: FooterProps) {\n  return (\n    <footer\n      className=\"footer\"\n      style={{\n        position: \"absolute\",\n        bottom: \"0\",\n        width: \"100%\",\n        height: \"40px\",\n        lineHeight: \"40px\",\n        backgroundColor: \"#f5f5f5\",\n        borderTop: \"1px solid #e5e5e5\",\n      }}\n    >\n      {footerText === \"\" && (\n        <div className=\"container\" style={{ textAlign: \"center\"}}>\n          \n          <span className=\"text-muted\" style={{ color: \"gray\", float: \"left\" }}>\n            {\" \"}\n            <a\n              style={{ textDecoration: \"none\", color: \"gray\" }}\n              href=\"/openapi\"\n            >\n              OpenAPI\n            </a>\n          </span>\n\n          <span className=\"text-muted\" style={{ color: \"gray\", margin: \"auto\", display: \"inline-block\" }}>\n            {\" \"}\n            <a\n              style={{ textDecoration: \"none\", color: \"gray\" }}\n              href=\"https://runmercury.com\"\n              target=\"_blank\"\n              rel=\"noreferrer\"\n            >\n              Notebooks served as Web Apps with Mercury\n            </a>\n          </span>\n\n          <span className=\"text-muted\" style={{ float: \"right\" }}>\n            <a\n              style={{ textDecoration: \"none\", color: \"gray\" }}\n              href=\"https://github.com/mljar/mercury\"\n              target=\"_blank\"\n              rel=\"noreferrer\"\n            >\n              Mercury\n            </a>{\" \"}\n            <i className=\"fa fa-github\" aria-hidden=\"true\"></i>\n          </span>\n        </div>\n      )}\n      {footerText !== \"\" && (\n        <div\n          className=\"container\"\n          style={{ color: \"gray\", textAlign: \"center\" }}\n        >\n          <span className=\"text-muted\" style={{ color: \"gray\" }}>\n            {footerText}\n          </span>\n        </div>\n      )}\n    </footer>\n  );\n}\n",
         "/* eslint-disable jsx-a11y/anchor-is-valid */\nimport React from \"react\";\nimport { Link } from \"react-router-dom\";\nimport LoginButton from \"./LoginButton\";\nimport UserButton from \"./UserButton\";\n\ntype NavBarProps = {\n  isSitePublic: boolean;\n  username: string;\n  logoSrc: string;\n  navbarColor: string;\n};\n\nexport default function NavBar({\n  isSitePublic,\n  username,\n  logoSrc,\n  navbarColor,\n}: NavBarProps) {\n  let headerBgClass = \"\";\n  let headerStyle = {};\n  if (navbarColor === \"\") {\n    headerBgClass = \"bg-dark\";\n  } else {\n    headerStyle = {\n      backgroundColor: navbarColor,\n    };\n  }\n\n  return (\n    <header\n      className={`navbar navbar-dark sticky-top p-0 ${headerBgClass}`}\n      style={headerStyle}\n    >\n      <div className=\"row\" style={{ width: \"100%\", paddingRight: \"0px\" }}>\n        <div className=\"col-4\"></div>\n        <div className=\"col-4 text-center\">\n          {logoSrc !== \"\" && logoSrc !== \"loading\" && (\n            <Link to=\"/\">\n              <img alt=\"\" src={logoSrc} style={{ height: \"40px\" }} />\n            </Link>\n          )}\n          {logoSrc === \"loading\" && (\n            <Link to=\"/\">\n              <div style={{ height: \"40px\" }} />\n            </Link>\n          )}\n        </div>\n        <div\n          className=\"col-4\"\n          style={{ marginRight: \"0px\", paddingRight: \"0px\" }}\n        >\n          {!isSitePublic && username === \"\" && <LoginButton />}\n          {username !== \"\" && <UserButton username={username} />}\n        </div>\n      </div>\n    </header>\n  );\n}\n",
         "/* eslint-disable jsx-a11y/anchor-is-valid */\nimport React, { useEffect, useState } from \"react\";\nimport { useDispatch, useSelector } from \"react-redux\";\nimport {\n  changePassword,\n  fetchUserInfo,\n  getUserInfo,\n  getUsername,\n} from \"../slices/authSlice\";\nimport Footer from \"../components/Footer\";\nimport HomeNavBar from \"../components/HomeNavBar\";\nimport {\n  getFooterText,\n  getLogoFilename,\n  getNavbarColor,\n  getSiteId,\n  isPublic,\n} from \"../slices/sitesSlice\";\nimport axios from \"axios\";\n\nimport DefaultLogoSrc from \"../components/DefaultLogo\";\n\nexport default function AccountView() {\n  const dispatch = useDispatch();\n  const [oldPassword, setOldPassword] = useState(\"\");\n  const [newPassword1, setNewPassword1] = useState(\"\");\n  const [newPassword2, setNewPassword2] = useState(\"\");\n  const [logoSrc, setLogoSrc] = useState(\"loading\");\n\n  const username = useSelector(getUsername);\n  const user = useSelector(getUserInfo);\n  const isSitePublic = useSelector(isPublic);\n  const logoFilename = useSelector(getLogoFilename);\n  const siteId = useSelector(getSiteId);\n  const navbarColor = useSelector(getNavbarColor);\n  const footerText = useSelector(getFooterText);\n\n  document.body.style.backgroundColor = \"white\";\n\n  useEffect(() => {\n    dispatch(fetchUserInfo());\n  }, [dispatch]);\n\n  useEffect(() => {\n    if (siteId !== undefined) {\n      if (logoFilename === \"\") {\n        setLogoSrc(DefaultLogoSrc);\n      } else {\n        axios\n          .get(`/api/v1/get-style/${siteId}/${logoFilename}`)\n          .then((response) => {\n            const { url } = response.data;\n            setLogoSrc(url);\n          });\n      }\n    }\n  }, [dispatch, logoFilename, siteId]);\n\n  return (\n    <div className=\"App\">\n      <HomeNavBar\n        isSitePublic={isSitePublic}\n        username={username}\n        logoSrc={logoSrc}\n        navbarColor={navbarColor}\n      />\n\n      <div className=\"container\">\n        <div className=\"mx-auto\" style={{ width: \"700px\" }}>\n          <div className=\"row\" style={{ marginTop: \"40px\" }}>\n            <h2>\n              <i className=\"fa fa-user\" aria-hidden=\"true\"></i> Account\n            </h2>\n            <form>\n              <div className=\"mb-3\">\n                <label className=\"form-label\">Username</label>\n                <input\n                  className=\"form-control\"\n                  value={user.username}\n                  disabled\n                />\n              </div>\n              <div className=\"mb-3\">\n                <label className=\"form-label\">First name</label>\n                <input\n                  className=\"form-control\"\n                  value={user.first_name}\n                  disabled\n                />\n              </div>\n              <div className=\"mb-3\">\n                <label className=\"form-label\">Last name</label>\n                <input\n                  className=\"form-control\"\n                  value={user.last_name}\n                  disabled\n                />\n              </div>\n\n              <div className=\"mb-3\">\n                <label className=\"form-label\">Email address</label>\n                <input className=\"form-control\" value={user.email} disabled />\n              </div>\n            </form>\n          </div>\n          <hr />\n          <div className=\"row\">\n            <h2>\n              <i className=\"fa fa-key\" aria-hidden=\"true\"></i> Change password\n            </h2>\n            <div>\n              <div className=\"mb-3\">\n                <label className=\"form-label\">Old password</label>\n                <input\n                  type=\"password\"\n                  className=\"form-control\"\n                  value={oldPassword}\n                  onChange={(e) => setOldPassword(e.target.value)}\n                />\n              </div>\n              <div className=\"mb-3\">\n                <label className=\"form-label\">New password</label>\n                <input\n                  type=\"password\"\n                  className=\"form-control\"\n                  value={newPassword1}\n                  onChange={(e) => setNewPassword1(e.target.value)}\n                />\n              </div>\n              <div className=\"mb-3\">\n                <label className=\"form-label\">Repeat new password</label>\n                <input\n                  type=\"password\"\n                  className=\"form-control\"\n                  value={newPassword2}\n                  onChange={(e) => setNewPassword2(e.target.value)}\n                />\n              </div>\n              <div className=\"mb-3\" style={{ paddingBottom: \"50px\" }}>\n                <button\n                  className=\"btn btn-primary\"\n                  onClick={() =>\n                    dispatch(\n                      changePassword(oldPassword, newPassword1, newPassword2)\n                    )\n                  }\n                  disabled={\n                    oldPassword === \"\" ||\n                    newPassword1 === \"\" ||\n                    newPassword2 === \"\"\n                  }\n                >\n                  Change password\n                </button>\n              </div>\n            </div>\n          </div>\n        </div>\n      </div>\n\n      <Footer footerText={footerText} />\n    </div>\n  );\n}\n",
         "/* eslint-disable import/no-cycle */\r\nimport {\r\n  createSlice,\r\n  PayloadAction,\r\n  AnyAction,\r\n  Dispatch,\r\n} from '@reduxjs/toolkit';\r\nimport axios from 'axios';\r\n\r\nimport { RootState } from '../store';\r\nimport { setToken, setUsername } from './authSlice';\r\n\r\n\r\nconst initialState = {\r\n  fetchingIsPro: true,\r\n  isPro: false,\r\n  welcome: \"\"\r\n};\r\n\r\nconst versionSlice = createSlice({\r\n  name: 'version',\r\n  initialState,\r\n  reducers: {\r\n    setVersion(state, action: PayloadAction<{ isPro: boolean }>) {\r\n      const { isPro } = action.payload;\r\n      state.isPro = isPro;\r\n      state.fetchingIsPro = false;\r\n    },\r\n    setWelcome(state, action: PayloadAction<string>) {\r\n      state.welcome = action.payload;\r\n    }\r\n  },\r\n});\r\n\r\nexport default versionSlice.reducer;\r\n\r\nexport const {\r\n  setVersion,\r\n  setWelcome,\r\n} = versionSlice.actions;\r\n\r\nexport const getIsPro = (state: RootState) => state.version.isPro;\r\nexport const getFetchingIsPro = (state: RootState) => state.version.fetchingIsPro;\r\nexport const getWelcome = (state: RootState) => state.version.welcome;\r\n\r\nexport const fetchVersion =\r\n  () =>\r\n    async (dispatch: Dispatch<AnyAction>) => {\r\n\r\n      try {\r\n        const url = '/api/v1/version/';\r\n        const { data } = await axios.get(url);\r\n        dispatch(setVersion(data));\r\n      } catch (error) {\r\n        console.log(`Problem during loading Mercury version. ${error}`);\r\n        if (axios.isAxiosError(error)) {\r\n          if (error.response?.status === 401) {\r\n            // clear auth data \r\n            dispatch(setToken(null));\r\n            dispatch(setUsername(null));\r\n            window.location.reload();\r\n          }\r\n        }\r\n      }\r\n    };\r\n\r\n\r\nexport const fetchWelcome =\r\n  (siteId: number) =>\r\n    async (dispatch: Dispatch<AnyAction>) => {\r\n\r\n      try {\r\n        const url = `/api/v1/${siteId}/welcome/`;\r\n        const { data } = await axios.get(url);\r\n        dispatch(setWelcome(data.msg));\r\n      } catch (error) {\r\n        console.log(`Problem during loading Mercury welcome message. ${error}`);\r\n      }\r\n\r\n    };\r\n\r\n",
-        "/* eslint-disable jsx-a11y/anchor-is-valid */\nimport React, { useEffect, useState } from \"react\";\nimport { useDispatch, useSelector } from \"react-redux\";\n\nimport HomeNavBar from \"../components/HomeNavBar\";\nimport Footer from \"../components/Footer\";\nimport {\n  // fetchNbIframes,\n  fetchNotebooks,\n  getLoadingState,\n  // getNbIframes,\n  getNotebooks,\n} from \"../slices/notebooksSlice\";\nimport { fetchWelcome, getWelcome } from \"../slices/versionSlice\";\n\nimport ReactMarkdown from \"react-markdown\";\nimport rehypeHighlight from \"rehype-highlight\";\nimport remarkGfm from \"remark-gfm\";\nimport emoji from \"remark-emoji\";\nimport rehypeRaw from \"rehype-raw\";\nimport { getToken, getUsername } from \"../slices/authSlice\";\nimport {\n  getFooterText,\n  getLogoFilename,\n  getNavbarColor,\n  getSiteId,\n  getSiteWelcome,\n  isPublic,\n} from \"../slices/sitesSlice\";\nimport axios from \"axios\";\n\nimport DefaultLogoSrc from \"../components/DefaultLogo\";\nimport { Link } from \"react-router-dom\";\n\nexport default function HomeView() {\n  const dispatch = useDispatch();\n  const notebooks = useSelector(getNotebooks);\n  const loadingState = useSelector(getLoadingState);\n  const welcome = useSelector(getWelcome);\n  const username = useSelector(getUsername);\n  const token = useSelector(getToken);\n  const [showButton, setShowButton] = useState(\"\");\n  const siteId = useSelector(getSiteId);\n  const isSitePublic = useSelector(isPublic);\n  const siteWelcome = useSelector(getSiteWelcome);\n  const [logoSrc, setLogoSrc] = useState(\"loading\");\n  const logoFilename = useSelector(getLogoFilename);\n  const navbarColor = useSelector(getNavbarColor);\n  const footerText = useSelector(getFooterText);\n\n  useEffect(() => {\n    console.log({logoFilename})\n    if (siteId !== undefined) {\n      if (logoFilename === \"\") {\n        setLogoSrc(DefaultLogoSrc);\n      } else {\n        axios\n          .get(`/api/v1/get-style/${siteId}/${logoFilename}`)\n          .then((response) => {\n            const { url } = response.data;\n            setLogoSrc(url);\n          });\n      }\n    }\n  }, [dispatch, logoFilename, siteId]);\n\n  useEffect(() => {\n    if (siteId !== undefined) {\n      dispatch(fetchNotebooks(siteId));\n      if (siteWelcome === undefined || siteWelcome === \"\") {\n        dispatch(fetchWelcome(siteId));\n      }\n    }\n    // fetchNotebooks depends on token\n    // if token is set then private notebooks are returned\n  }, [dispatch, siteId, token, siteWelcome]);\n\n  const firstLetters = (text: string | null, count: number): string => {\n    if (text !== null && text !== undefined) {\n      return text.slice(0, count) + (text.length > count ? \" ...\" : \"\");\n    }\n    return \"\";\n  };\n\n  const notebookItems = notebooks.map((notebook, index) => {\n    let nbPath = notebook.default_view_path;\n\n    if (window.location.origin.startsWith(\"https\")) {\n      nbPath = nbPath.replace(\"http://\", \"https://\");\n    }\n\n    if (window.location.origin === \"http://localhost:3000\") {\n      if (nbPath.startsWith(\"/media\")) {\n        nbPath = \"https://127.0.0.1:8000\" + nbPath;\n      }\n    }\n\n    // if (window.location.origin !== \"http://localhost:3000\") {\n    //   if (nbPath.startsWith(\"https://127.0.0.1:8000\")) {\n    //     nbPath = nbPath.replace(\n    //       \"https://127.0.0.1:8000\",\n    //       window.location.origin\n    //     );\n    //   }\n    //   if (nbPath.startsWith(\"http://127.0.0.1:8000\")) {\n    //     nbPath = nbPath.replace(\n    //       \"http://127.0.0.1:8000\",\n    //       window.location.origin\n    //     );\n    //   }\n    // }\n\n    return (\n      <div\n        className=\"col-md-4\"\n        style={{ paddingBottom: \"20px\" }}\n        key={`notebook-${notebook.id}}`}\n      >\n        <div className=\"card\">\n          <div\n            style={{\n              height: \"200px\",\n              width: \"100%\",\n              padding: \"1px\",\n              overflow: \"hidden\",\n            }}\n          >\n            <iframe\n              className=\"thumbnailIframe\"\n              width=\"200%\"\n              height={800}\n              src={nbPath}\n              title=\"display\"\n              scrolling=\"no\"\n            ></iframe>\n\n            {/* <img\n              alt=\"some alt\" \n              \n              width=\"100%\"\n              src={`${notebook.default_view_path.replace(\".html\", \".png\")}`}\n            ></img> */}\n          </div>\n          <Link\n            to={`/app/${notebook.slug}`}\n            style={{ textDecoration: \"none\", color: \"black\" }}\n            className=\"title-card\"\n            onMouseEnter={() => {\n              setShowButton(notebook.slug);\n            }}\n            onMouseLeave={() => {\n              setShowButton(\"\");\n            }}\n            reloadDocument\n          >\n            <div\n              className=\"card-body\"\n              style={{\n                borderTop: \"1px solid rgba(0,0,0,0.1)\",\n                height: \"110px\",\n              }}\n            >\n              <h5 className=\"card-title\">{firstLetters(notebook.title, 40)}</h5>\n\n              <p className=\"card-text\">\n                {firstLetters(notebook.params.description, 100)}\n              </p>\n            </div>\n            {showButton === notebook.slug && (\n              <button\n                className=\"btn btn-outline-primary\"\n                type=\"button\"\n                style={{\n                  zIndex: \"101\",\n                  border: \"none\",\n                  margin: \"5px\",\n                  position: \"absolute\",\n                  right: \"0px\",\n                  bottom: \"0px\",\n                }}\n                data-toggle=\"tooltip\"\n                data-placement=\"right\"\n                title={`Open ${notebook.title}`}\n              >\n                <i className=\"fa fa-chevron-right\" aria-hidden=\"true\" />\n              </button>\n            )}\n          </Link>\n        </div>\n      </div>\n    );\n  });\n\n  document.body.style.backgroundColor = \"white\";\n\n  let welcomeMd = siteWelcome;\n  if (welcomeMd === undefined || welcomeMd === \"\") {\n    welcomeMd = welcome;\n  }\n\n  return (\n    <div className=\"App\">\n      <HomeNavBar\n        isSitePublic={isSitePublic}\n        username={username}\n        logoSrc={logoSrc}\n        navbarColor={navbarColor}\n      />\n      <div className=\"container\" style={{ paddingBottom: \"50px\" }}>\n        {welcomeMd === \"\" && (\n          <h1 style={{ padding: \"30px\", textAlign: \"center\" }}>Welcome!</h1>\n        )}\n        {welcomeMd !== \"\" && (\n          <div style={{ paddingTop: \"20px\", paddingBottom: \"10px\" }}>\n            <ReactMarkdown\n              rehypePlugins={[remarkGfm, rehypeHighlight, emoji, rehypeRaw]}\n            >\n              {welcomeMd}\n            </ReactMarkdown>\n          </div>\n        )}\n\n        <div className=\"row\">\n          {loadingState === \"loading\" && (\n            <p>Loading notebooks. Please wait ...</p>\n          )}\n\n          {loadingState === \"loaded\" && notebooks.length === 0 && (\n            <div>\n              <p>There are no notebooks available.</p>\n            </div>\n          )}\n          {loadingState === \"error\" && (\n            <p>\n              Problem while loading notebooks. Please try again later or contact\n              Mercury administrator.\n            </p>\n          )}\n          {notebookItems}\n        </div>\n      </div>\n      <Footer footerText={footerText} />\n    </div>\n  );\n}\n",
+        "/* eslint-disable jsx-a11y/anchor-is-valid */\nimport React, { useEffect, useState } from \"react\";\nimport { useDispatch, useSelector } from \"react-redux\";\n\nimport HomeNavBar from \"../components/HomeNavBar\";\nimport Footer from \"../components/Footer\";\nimport {\n  // fetchNbIframes,\n  fetchNotebooks,\n  getLoadingState,\n  // getNbIframes,\n  getNotebooks,\n} from \"../slices/notebooksSlice\";\nimport { fetchWelcome, getWelcome } from \"../slices/versionSlice\";\n\nimport ReactMarkdown from \"react-markdown\";\nimport rehypeHighlight from \"rehype-highlight\";\nimport remarkGfm from \"remark-gfm\";\nimport emoji from \"remark-emoji\";\nimport rehypeRaw from \"rehype-raw\";\nimport { getToken, getUsername } from \"../slices/authSlice\";\nimport {\n  getFooterText,\n  getLogoFilename,\n  getNavbarColor,\n  getSiteId,\n  getSiteWelcome,\n  isPublic,\n} from \"../slices/sitesSlice\";\nimport axios from \"axios\";\n\nimport DefaultLogoSrc from \"../components/DefaultLogo\";\nimport { Link } from \"react-router-dom\";\n\nexport default function HomeView() {\n  const dispatch = useDispatch();\n  const notebooks = useSelector(getNotebooks);\n  const loadingState = useSelector(getLoadingState);\n  const welcome = useSelector(getWelcome);\n  const username = useSelector(getUsername);\n  const token = useSelector(getToken);\n  const [showButton, setShowButton] = useState(\"\");\n  const siteId = useSelector(getSiteId);\n  const isSitePublic = useSelector(isPublic);\n  const siteWelcome = useSelector(getSiteWelcome);\n  const [logoSrc, setLogoSrc] = useState(\"loading\");\n  const logoFilename = useSelector(getLogoFilename);\n  const navbarColor = useSelector(getNavbarColor);\n  const footerText = useSelector(getFooterText);\n\n  useEffect(() => {\n    console.log({logoFilename})\n    if (siteId !== undefined) {\n      if (logoFilename === \"\") {\n        setLogoSrc(DefaultLogoSrc);\n      } else {\n        axios\n          .get(`/api/v1/get-style/${siteId}/${logoFilename}`)\n          .then((response) => {\n            const { url } = response.data;\n            setLogoSrc(url);\n          });\n      }\n    }\n  }, [dispatch, logoFilename, siteId]);\n\n  useEffect(() => {\n    if (siteId !== undefined) {\n      dispatch(fetchNotebooks(siteId));\n      if (siteWelcome === undefined || siteWelcome === \"\") {\n        dispatch(fetchWelcome(siteId));\n      }\n    }\n    // fetchNotebooks depends on token\n    // if token is set then private notebooks are returned\n  }, [dispatch, siteId, token, siteWelcome]);\n\n  const firstLetters = (text: string | null, count: number): string => {\n    if (text !== null && text !== undefined) {\n      return text.slice(0, count) + (text.length > count ? \" ...\" : \"\");\n    }\n    return \"\";\n  };\n\n  const notebookItems = notebooks.map((notebook, index) => {\n    let nbPath = notebook.default_view_path;\n\n    if (window.location.origin.startsWith(\"https\")) {\n      nbPath = nbPath.replace(\"http://\", \"https://\");\n    }\n\n    if (window.location.origin === \"http://localhost:3000\") {\n      if (nbPath.startsWith(\"/media\")) {\n        nbPath = \"https://127.0.0.1:8000\" + nbPath;\n      }\n    }\n\n    // if (window.location.origin !== \"http://localhost:3000\") {\n    //   if (nbPath.startsWith(\"https://127.0.0.1:8000\")) {\n    //     nbPath = nbPath.replace(\n    //       \"https://127.0.0.1:8000\",\n    //       window.location.origin\n    //     );\n    //   }\n    //   if (nbPath.startsWith(\"http://127.0.0.1:8000\")) {\n    //     nbPath = nbPath.replace(\n    //       \"http://127.0.0.1:8000\",\n    //       window.location.origin\n    //     );\n    //   }\n    // }\n\n    return (\n      <div\n        className=\"col-md-4\"\n        style={{ paddingBottom: \"20px\" }}\n        key={`notebook-${notebook.id}}`}\n      >\n        <div className=\"card\">\n          <div\n            style={{\n              height: \"200px\",\n              width: \"100%\",\n              padding: \"1px\",\n              overflow: \"hidden\",\n            }}\n          >\n            <iframe\n              className=\"thumbnailIframe\"\n              width=\"200%\"\n              height={800}\n              src={nbPath}\n              title=\"display\"\n              scrolling=\"no\"\n            ></iframe>\n\n            {/* <img\n              alt=\"some alt\" \n              \n              width=\"100%\"\n              src={`${notebook.default_view_path.replace(\".html\", \".png\")}`}\n            ></img> */}\n          </div>\n          <Link\n            to={`/app/${notebook.slug}`}\n            style={{ textDecoration: \"none\", color: \"black\" }}\n            className=\"title-card\"\n            onMouseEnter={() => {\n              setShowButton(notebook.slug);\n            }}\n            onMouseLeave={() => {\n              setShowButton(\"\");\n            }}\n            reloadDocument\n          >\n            <div\n              className=\"card-body\"\n              style={{\n                borderTop: \"1px solid rgba(0,0,0,0.1)\",\n                height: \"110px\",\n              }}\n            >\n              <h5 className=\"card-title\">{firstLetters(notebook.title, 40)}</h5>\n\n              <p className=\"card-text\">\n                {firstLetters(notebook.params.description, 100)}\n              </p>\n            </div>\n            {showButton === notebook.slug && (\n              <button\n                className=\"btn btn-outline-primary\"\n                type=\"button\"\n                style={{\n                  zIndex: \"101\",\n                  border: \"none\",\n                  margin: \"5px\",\n                  position: \"absolute\",\n                  right: \"0px\",\n                  bottom: \"0px\",\n                }}\n                data-toggle=\"tooltip\"\n                data-placement=\"right\"\n                title={`Open ${notebook.title}`}\n              >\n                <i className=\"fa fa-chevron-right\" aria-hidden=\"true\" />\n                <i className=\"fa fa-chevron-right\" aria-hidden=\"true\" />\n              </button>\n            )}\n            \n          </Link>\n        </div>\n      </div>\n    );\n  });\n\n  document.body.style.backgroundColor = \"white\";\n\n  let welcomeMd = siteWelcome;\n  if (welcomeMd === undefined || welcomeMd === \"\") {\n    welcomeMd = welcome;\n  }\n\n  return (\n    <div className=\"App\">\n      <HomeNavBar\n        isSitePublic={isSitePublic}\n        username={username}\n        logoSrc={logoSrc}\n        navbarColor={navbarColor}\n      />\n      <div className=\"container\" style={{ paddingBottom: \"50px\" }}>\n        {welcomeMd === \"\" && (\n          <h1 style={{ padding: \"30px\", textAlign: \"center\" }}>Welcome!</h1>\n        )}\n        {welcomeMd !== \"\" && (\n          <div style={{ paddingTop: \"20px\", paddingBottom: \"10px\" }}>\n            <ReactMarkdown\n              rehypePlugins={[remarkGfm, rehypeHighlight, emoji, rehypeRaw]}\n            >\n              {welcomeMd}\n            </ReactMarkdown>\n          </div>\n        )}\n\n        <div className=\"row\">\n          {loadingState === \"loading\" && (\n            <p>Loading notebooks. Please wait ...</p>\n          )}\n\n          {loadingState === \"loaded\" && notebooks.length === 0 && (\n            <div>\n              <p>There are no notebooks available.</p>\n            </div>\n          )}\n          {loadingState === \"error\" && (\n            <p>\n              Problem while loading notebooks. Please try again later or contact\n              Mercury administrator.\n            </p>\n          )}\n          {notebookItems}\n        </div>\n      </div>\n      <Footer footerText={footerText} />\n    </div>\n  );\n}\n",
         "/* eslint-disable jsx-a11y/anchor-is-valid */\nimport React, { useEffect, useState } from \"react\";\nimport { useDispatch, useSelector } from \"react-redux\";\nimport { fetchToken } from \"../slices/authSlice\";\nimport Footer from \"../components/Footer\";\nimport HomeNavBar from \"../components/HomeNavBar\";\n\nimport { useLocation, useNavigate } from \"react-router-dom\";\nimport {\n  getFooterText,\n  getLogoFilename,\n  getNavbarColor,\n  getSiteId,\n  isPublic,\n} from \"../slices/sitesSlice\";\nimport axios from \"axios\";\n\nimport DefaultLogoSrc from \"../components/DefaultLogo\";\n\ntype LocationState = {\n  from: {\n    pathname: string;\n  };\n};\n\nexport default function LoginView() {\n  const dispatch = useDispatch();\n  const navigate = useNavigate();\n  const [email, setEmail] = useState(\"\");\n  const [password, setPassword] = useState(\"\");\n  const isSitePublic = useSelector(isPublic);\n  const [logoSrc, setLogoSrc] = useState(\"loading\");\n  const logoFilename = useSelector(getLogoFilename);\n  const siteId = useSelector(getSiteId);\n  const navbarColor = useSelector(getNavbarColor);\n  const footerText = useSelector(getFooterText);\n\n  document.body.style.backgroundColor = \"#f5f5f5\";\n\n  let redirectPath = \"/\";\n  let location = useLocation();\n  if (location && location.state) {\n    // redirect from ...\n    const { from } = location.state as LocationState;\n    redirectPath = from.pathname;\n  }\n\n  useEffect(() => {\n    if (siteId !== undefined) {\n      if (logoFilename === \"\") {\n        setLogoSrc(DefaultLogoSrc);\n      } else {\n        axios\n          .get(`/api/v1/get-style/${siteId}/${logoFilename}`)\n          .then((response) => {\n            const { url } = response.data;\n            setLogoSrc(url);\n          });\n      }\n    }\n  }, [dispatch, logoFilename, siteId]);\n\n  return (\n    <div className=\"App\">\n      <HomeNavBar\n        isSitePublic={isSitePublic}\n        username={\"\"}\n        logoSrc={logoSrc}\n        navbarColor={navbarColor}\n      />\n\n      <div className=\"div-signin text-center\">\n        <form\n          className=\"form-signin\"\n          onSubmit={(e) => {\n            e.preventDefault();\n            e.stopPropagation();\n            dispatch(fetchToken(email, password, redirectPath, navigate));\n          }}\n        >\n          <h3 className=\"h3 mb-3 font-weight-normal\">Please sign in</h3>\n          <label className=\"sr-only\">Email</label>\n          <input\n            type=\"email\"\n            id=\"inputEmail\"\n            className=\"form-control\"\n            placeholder=\"Email\"\n            value={email}\n            onChange={(e) => {\n              setEmail(e.target.value);\n            }}\n            required\n          />\n          <label className=\"sr-only\">Password</label>\n          <input\n            type=\"password\"\n            id=\"inputPassword\"\n            className=\"form-control\"\n            placeholder=\"Password\"\n            value={password}\n            onChange={(e) => {\n              setPassword(e.target.value);\n            }}\n            required\n          />\n          <button\n            className=\"btn btn-lg btn-primary btn-block\"\n            type=\"submit\"\n            style={{ margin: \"5px\" }}\n            disabled={email === \"\" || password === \"\"}\n          >\n            <i className=\"fa fa-sign-in\" aria-hidden=\"true\"></i> Log in\n          </button>\n        </form>\n        <div className=\"mx-auto\" style={{ width: \"400px\", marginTop: \"40px\" }}>\n          <p className=\"text-muted\">\n            No account? <br /> Please contact administrator to create account\n            for you.\n          </p>\n        </div>\n      </div>\n\n      <Footer footerText={footerText} />\n    </div>\n  );\n}\n",
         "/* eslint-disable jsx-a11y/anchor-is-valid */\nimport React from \"react\";\n\nexport default function LostConnection() {\n  return (\n    <div className=\"App\">\n      <div\n        style={{\n          width: \"100%\",\n          maxWidth: \"500px\",\n          padding: \"15px\",\n          margin: \"0 auto\",\n        }}\n      >\n        <h3>Lost connection</h3>\n        <p>\n          App lost connection to the server. Please try again in a moment or\n          contact administrator.\n        </p>\n      </div>\n    </div>\n  );\n}\n",
         "/* eslint-disable jsx-a11y/anchor-is-valid */\nimport React from \"react\";\nimport { Link } from \"react-router-dom\";\n\nexport default function SiteAccessForbiddenView() {\n  return (\n    <div className=\"App\">\n      <div\n        style={{\n          width: \"100%\",\n          maxWidth: \"500px\",\n          padding: \"15px\",\n          margin: \"0 auto\",\n        }}\n      >\n        <h3>Access forbidden</h3>\n        <p>\n          Please <Link to=\"/login\">login</Link> to access site.\n        </p>\n      </div>\n    </div>\n  );\n}\n",
         "/* eslint-disable jsx-a11y/anchor-is-valid */\nimport React from \"react\";\n\nexport default function SiteLoadingView() {\n  return (\n    <div className=\"App\">\n      <div\n        style={{\n          width: \"100%\",\n          maxWidth: \"500px\",\n          padding: \"15px\",\n          margin: \"0 auto\",\n        }}\n      >\n        <p style={{ color: \"gray\" }}>Please wait. Loading site ...</p>\n      </div>\n    </div>\n  );\n}\n",
         "/* eslint-disable jsx-a11y/anchor-is-valid */\nimport React from \"react\";\n\nexport default function SiteNetworkErrorView() {\n  return (\n    <div className=\"App\">\n      <div\n        style={{\n          width: \"100%\",\n          maxWidth: \"500px\",\n          padding: \"15px\",\n          margin: \"0 auto\",\n        }}\n      >\n        <h3>Network Error</h3>\n        <p>\n          Please check if you have internet connection and server is running. In\n          case of problems, please contact administrator.\n        </p>\n      </div>\n    </div>\n  );\n}\n",
         "/* eslint-disable jsx-a11y/anchor-is-valid */\nimport React from \"react\";\n\nexport default function SiteNotFoundView() {\n  return (\n    <div className=\"App\">\n      <div\n        style={{\n          width: \"100%\",\n          maxWidth: \"500px\",\n          padding: \"15px\",\n          margin: \"0 auto\",\n        }}\n      >\n        <h3>Site does not exist</h3>\n        <p>\n          We can't find site you are looking for. Please make sure that URL\n          address is correct.\n        </p>\n      </div>\n    </div>\n  );\n}\n",
         "/* eslint-disable jsx-a11y/anchor-is-valid */\nimport React from \"react\";\n\nexport default function SitePleaseRefreshView() {\n  return (\n    <div className=\"App\">\n      <div\n        style={{\n          width: \"100%\",\n          maxWidth: \"500px\",\n          padding: \"15px\",\n          margin: \"0 auto\",\n        }}\n      >\n        <h3>Please refresh</h3>\n        <p>Please try to refresh the website ...</p>\n      </div>\n    </div>\n  );\n}\n",
```

### Comparing `mercury-2.4.1/mercury/frontend-dist/static/js/runtime-main.248907bc.js` & `mercury-2.4.2/mercury/frontend-dist/static/js/runtime-main.248907bc.js`

 * *Files identical despite different names*

### Comparing `mercury-2.4.1/mercury/frontend-dist/static/js/runtime-main.248907bc.js.map` & `mercury-2.4.2/mercury/frontend-dist/static/js/runtime-main.248907bc.js.map`

 * *Files identical despite different names*

### Comparing `mercury-2.4.1/mercury/frontend-dist/static/media/fontawesome-webfont.1e59d233.ttf` & `mercury-2.4.2/mercury/frontend-dist/static/media/fontawesome-webfont.1e59d233.ttf`

 * *Files identical despite different names*

### Comparing `mercury-2.4.1/mercury/frontend-dist/static/media/fontawesome-webfont.20fd1704.woff2` & `mercury-2.4.2/mercury/frontend-dist/static/media/fontawesome-webfont.20fd1704.woff2`

 * *Files identical despite different names*

### Comparing `mercury-2.4.1/mercury/frontend-dist/static/media/fontawesome-webfont.8b43027f.eot` & `mercury-2.4.2/mercury/frontend-dist/static/media/fontawesome-webfont.8b43027f.eot`

 * *Files identical despite different names*

### Comparing `mercury-2.4.1/mercury/frontend-dist/static/media/fontawesome-webfont.c1e38fd9.svg` & `mercury-2.4.2/mercury/frontend-dist/static/media/fontawesome-webfont.c1e38fd9.svg`

 * *Files identical despite different names*

### Comparing `mercury-2.4.1/mercury/frontend-dist/static/media/fontawesome-webfont.f691f37e.woff` & `mercury-2.4.2/mercury/frontend-dist/static/media/fontawesome-webfont.f691f37e.woff`

 * *Files identical despite different names*

### Comparing `mercury-2.4.1/mercury/manage.py` & `mercury-2.4.2/mercury/manage.py`

 * *Files identical despite different names*

### Comparing `mercury-2.4.1/mercury/mercury.py` & `mercury-2.4.2/mercury/mercury.py`

 * *Files identical despite different names*

### Comparing `mercury-2.4.1/mercury/requirements.txt` & `mercury-2.4.2/mercury/requirements.txt`

 * *Files 0% similar despite different names*

```diff
@@ -22,7 +22,8 @@
 ipywidgets==8.0.3 # cant update ipywidgets!
 dj-rest-auth[with_social]==3.0.0
 boto3==1.26.83
 cryptography
 pyopenssl>=23.1.1
 bleach>=6.0.0
 itables>=2.0.0
+
```

### Comparing `mercury-2.4.1/mercury/server/asgi.py` & `mercury-2.4.2/mercury/server/asgi.py`

 * *Files identical despite different names*

### Comparing `mercury-2.4.1/mercury/server/celery.py` & `mercury-2.4.2/mercury/server/celery.py`

 * *Files identical despite different names*

### Comparing `mercury-2.4.1/mercury/server/settings.py` & `mercury-2.4.2/mercury/server/settings.py`

 * *Files identical despite different names*

### Comparing `mercury-2.4.1/mercury/server/urls.py` & `mercury-2.4.2/mercury/server/urls.py`

 * *Files identical despite different names*

### Comparing `mercury-2.4.1/mercury/server/views.py` & `mercury-2.4.2/mercury/server/views.py`

 * *Files identical despite different names*

### Comparing `mercury-2.4.1/mercury/start_instance.py` & `mercury-2.4.2/mercury/start_instance.py`

 * *Files identical despite different names*

### Comparing `mercury-2.4.1/mercury/widgets/apiresponse.py` & `mercury-2.4.2/mercury/widgets/apiresponse.py`

 * *Files identical despite different names*

### Comparing `mercury-2.4.1/mercury/widgets/app.py` & `mercury-2.4.2/mercury/widgets/app.py`

 * *Files 16% similar despite different names*

```diff
@@ -65,14 +65,18 @@
         If True (the default), the notebook is displayed with full width. Set to 
         False to limit notebook width to 1140px.
 
     allow_download : bool, default True
         If True (the default), a Download button is available to export results as 
         a PDF or HTML file. Set to False to hide the Download button.
 
+    allow_share : bool, default True
+        If True (the default), a Share button is available to export results as a 
+        URL. Set to False to hide the Share button.
+
     stop_on_error : bool, default False
         If True, the notebook will stop execution when an error occurs in a cell. 
         The default is False, meaning the notebook will execute all cells even with 
         errors.
 
     Examples
     --------
@@ -96,14 +100,15 @@
         schedule="",
         notify={},
         continuous_update=True,
         static_notebook=False,
         show_sidebar=True,
         full_screen=True,
         allow_download=True,
+        allow_share=True,
         stop_on_error=False,
     ):
         self.code_uid = WidgetsManager.get_code_uid("App")
         self.title = title
         self.description = description
         self.show_code = show_code
         self.show_prompt = show_prompt
@@ -111,14 +116,15 @@
         self.schedule = schedule
         self.notify = notify
         self.continuous_update = continuous_update
         self.static_notebook = static_notebook
         self.show_sidebar = show_sidebar
         self.full_screen = full_screen
         self.allow_download = allow_download
+        self.allow_share = allow_share
         self.stop_on_error = stop_on_error
         display(self)
 
     def __repr__(self):
         return f"mercury.App"
 
     def _repr_mimebundle_(self, **kwargs):
@@ -137,13 +143,14 @@
             "schedule": self.schedule,
             "notify": json.dumps(self.notify),
             "continuous_update": self.continuous_update,
             "static_notebook": self.static_notebook,
             "show_sidebar": self.show_sidebar,
             "full_screen": self.full_screen,
             "allow_download": self.allow_download,
+            "allow_share": self.allow_share,
             "stop_on_error": self.stop_on_error,
             "model_id": "mercury-app",
             "code_uid": self.code_uid,
         }
         data["application/mercury+json"] = json.dumps(view, indent=4)
         return data
```

### Comparing `mercury-2.4.1/mercury/widgets/button.py` & `mercury-2.4.2/mercury/widgets/button.py`

 * *Files identical despite different names*

### Comparing `mercury-2.4.1/mercury/widgets/chat.py` & `mercury-2.4.2/mercury/widgets/chat.py`

 * *Files identical despite different names*

### Comparing `mercury-2.4.1/mercury/widgets/checkbox.py` & `mercury-2.4.2/mercury/widgets/checkbox.py`

 * *Files identical despite different names*

### Comparing `mercury-2.4.1/mercury/widgets/file.py` & `mercury-2.4.2/mercury/widgets/file.py`

 * *Files identical despite different names*

### Comparing `mercury-2.4.1/mercury/widgets/in_mercury.py` & `mercury-2.4.2/mercury/widgets/in_mercury.py`

 * *Files identical despite different names*

### Comparing `mercury-2.4.1/mercury/widgets/json.py` & `mercury-2.4.2/mercury/widgets/json.py`

 * *Files identical despite different names*

### Comparing `mercury-2.4.1/mercury/widgets/manager.py` & `mercury-2.4.2/mercury/widgets/manager.py`

 * *Files identical despite different names*

### Comparing `mercury-2.4.1/mercury/widgets/multiselect.py` & `mercury-2.4.2/mercury/widgets/multiselect.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,15 +79,17 @@
     >>> # corresponding options reflected in the "options" URL parameter.
     >>> print(my_options.value)
     """
 
     def __init__(
         self, value=[], choices=[], label="MultiSelect", url_key="", disabled=False, hidden=False
     ):
-        if not value and len(choices) > 1:
+        if value is None:
+            value = [choices[0]]
+        if len(value) == 0 and len(choices) > 1:
             value = [choices[0]]
 
         self.code_uid = WidgetsManager.get_code_uid("MultiSelect", key=url_key)
         self.url_key = url_key
         self.hidden = hidden
         choices = [i for i in list(choices) if isinstance(i, str)]
         value = [i for i in list(value) if isinstance(i, str)]
```

### Comparing `mercury-2.4.1/mercury/widgets/note.py` & `mercury-2.4.2/mercury/widgets/note.py`

 * *Files identical despite different names*

### Comparing `mercury-2.4.1/mercury/widgets/numberbox.py` & `mercury-2.4.2/mercury/widgets/numberbox.py`

 * *Files identical despite different names*

### Comparing `mercury-2.4.1/mercury/widgets/numeric.py` & `mercury-2.4.2/mercury/widgets/numeric.py`

 * *Files identical despite different names*

### Comparing `mercury-2.4.1/mercury/widgets/outputdir.py` & `mercury-2.4.2/mercury/widgets/outputdir.py`

 * *Files identical despite different names*

### Comparing `mercury-2.4.1/mercury/widgets/range.py` & `mercury-2.4.2/mercury/widgets/range.py`

 * *Files identical despite different names*

### Comparing `mercury-2.4.1/mercury/widgets/select.py` & `mercury-2.4.2/mercury/widgets/select.py`

 * *Files identical despite different names*

### Comparing `mercury-2.4.1/mercury/widgets/slider.py` & `mercury-2.4.2/mercury/widgets/slider.py`

 * *Files identical despite different names*

### Comparing `mercury-2.4.1/mercury/widgets/table.py` & `mercury-2.4.2/mercury/widgets/table.py`

 * *Files identical despite different names*

### Comparing `mercury-2.4.1/mercury/widgets/text.py` & `mercury-2.4.2/mercury/widgets/text.py`

 * *Files identical despite different names*

### Comparing `mercury-2.4.1/mercury/widgets/user.py` & `mercury-2.4.2/mercury/widgets/user.py`

 * *Files identical despite different names*

### Comparing `mercury-2.4.1/mercury.egg-info/PKG-INFO` & `mercury-2.4.2/mercury.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mercury
-Version: 2.4.1
+Version: 2.4.2
 Summary: Turn Jupyter Notebook to Web App and share with non-technical users
 Home-page: https://github.com/mljar/mercury
 Author: MLJAR Sp. z o.o.
 Maintainer: MLJAR Sp. z o.o.
 Maintainer-email: contact@mljar.com
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
```

### Comparing `mercury-2.4.1/mercury.egg-info/SOURCES.txt` & `mercury-2.4.2/mercury.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -21,25 +21,28 @@
 mercury/apps/accounts/apps.py
 mercury/apps/accounts/fields.py
 mercury/apps/accounts/models.py
 mercury/apps/accounts/serializers.py
 mercury/apps/accounts/tasks.py
 mercury/apps/accounts/urls.py
 mercury/apps/accounts/migrations/0001_initial.py
+mercury/apps/accounts/migrations/0002_apikey.py
 mercury/apps/accounts/migrations/__init__.py
 mercury/apps/accounts/templatetags/__init__.py
 mercury/apps/accounts/templatetags/replace.py
 mercury/apps/accounts/tests/__init__.py
 mercury/apps/accounts/tests/test_accounts.py
+mercury/apps/accounts/tests/test_apikey.py
 mercury/apps/accounts/tests/test_invitations.py
 mercury/apps/accounts/tests/test_secrets.py
 mercury/apps/accounts/tests/test_sites.py
 mercury/apps/accounts/tests/test_subscription.py
 mercury/apps/accounts/views/__init__.py
 mercury/apps/accounts/views/accounts.py
+mercury/apps/accounts/views/apikey.py
 mercury/apps/accounts/views/invitations.py
 mercury/apps/accounts/views/permissions.py
 mercury/apps/accounts/views/secrets.py
 mercury/apps/accounts/views/sites.py
 mercury/apps/accounts/views/subscription.py
 mercury/apps/accounts/views/utils.py
 mercury/apps/nb/__init__.py
@@ -147,16 +150,16 @@
 mercury/frontend-dist/static/css/2.c6cf5ff9.chunk.css
 mercury/frontend-dist/static/css/2.c6cf5ff9.chunk.css.map
 mercury/frontend-dist/static/css/main.9848f1b3.chunk.css
 mercury/frontend-dist/static/css/main.9848f1b3.chunk.css.map
 mercury/frontend-dist/static/js/2.81b1917f.chunk.js
 mercury/frontend-dist/static/js/2.81b1917f.chunk.js.LICENSE.txt
 mercury/frontend-dist/static/js/2.81b1917f.chunk.js.map
-mercury/frontend-dist/static/js/main.51571475.chunk.js
-mercury/frontend-dist/static/js/main.51571475.chunk.js.map
+mercury/frontend-dist/static/js/main.71279c97.chunk.js
+mercury/frontend-dist/static/js/main.71279c97.chunk.js.map
 mercury/frontend-dist/static/js/runtime-main.248907bc.js
 mercury/frontend-dist/static/js/runtime-main.248907bc.js.map
 mercury/frontend-dist/static/media/fontawesome-webfont.1e59d233.ttf
 mercury/frontend-dist/static/media/fontawesome-webfont.20fd1704.woff2
 mercury/frontend-dist/static/media/fontawesome-webfont.8b43027f.eot
 mercury/frontend-dist/static/media/fontawesome-webfont.c1e38fd9.svg
 mercury/frontend-dist/static/media/fontawesome-webfont.f691f37e.woff
```

### Comparing `mercury-2.4.1/setup.py` & `mercury-2.4.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     for (path, directories, filenames) in os.walk(directory):
         for filename in filenames:
             paths.append(os.path.join(path, filename))
     return paths
 
 setup(
     name="mercury",
-    version="2.4.1",
+    version="2.4.2",
     author="MLJAR Sp. z o.o.",
     maintainer="MLJAR Sp. z o.o.",
     maintainer_email="contact@mljar.com",
     description="Turn Jupyter Notebook to Web App and share with non-technical users",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=open("mercury/requirements.txt").readlines(),
```

