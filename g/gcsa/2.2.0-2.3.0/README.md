# Comparing `tmp/gcsa-2.2.0.tar.gz` & `tmp/gcsa-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gcsa-2.2.0.tar", last modified: Mon Nov 13 13:22:32 2023, max compression
+gzip compressed data, was "gcsa-2.3.0.tar", last modified: Fri May 10 10:13:08 2024, max compression
```

## Comparing `gcsa-2.2.0.tar` & `gcsa-2.3.0.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 ykuzmovy   (501) staff       (20)        0 2023-11-13 13:22:32.789084 gcsa-2.2.0/
--rw-r--r--   0 ykuzmovy   (501) staff       (20)     1057 2023-05-29 12:12:43.000000 gcsa-2.2.0/LICENSE
--rw-r--r--   0 ykuzmovy   (501) staff       (20)     3436 2023-11-13 13:22:32.788933 gcsa-2.2.0/PKG-INFO
--rw-r--r--   0 ykuzmovy   (501) staff       (20)     2428 2023-05-29 12:12:43.000000 gcsa-2.2.0/README.rst
-drwxr-xr-x   0 ykuzmovy   (501) staff       (20)        0 2023-11-13 13:22:32.779113 gcsa-2.2.0/gcsa/
--rw-r--r--   0 ykuzmovy   (501) staff       (20)        0 2023-05-29 12:12:43.000000 gcsa-2.2.0/gcsa/__init__.py
--rw-r--r--   0 ykuzmovy   (501) staff       (20)      124 2023-05-29 12:12:43.000000 gcsa-2.2.0/gcsa/_resource.py
-drwxr-xr-x   0 ykuzmovy   (501) staff       (20)        0 2023-11-13 13:22:32.782045 gcsa-2.2.0/gcsa/_services/
--rw-r--r--   0 ykuzmovy   (501) staff       (20)        0 2023-05-29 12:12:43.000000 gcsa-2.2.0/gcsa/_services/__init__.py
--rw-r--r--   0 ykuzmovy   (501) staff       (20)     5856 2023-05-29 12:12:43.000000 gcsa-2.2.0/gcsa/_services/acl_service.py
--rw-r--r--   0 ykuzmovy   (501) staff       (20)     6082 2023-11-10 14:01:50.000000 gcsa-2.2.0/gcsa/_services/authentication.py
--rw-r--r--   0 ykuzmovy   (501) staff       (20)     2324 2023-05-29 12:12:43.000000 gcsa-2.2.0/gcsa/_services/base_service.py
--rw-r--r--   0 ykuzmovy   (501) staff       (20)     5394 2023-05-29 12:12:43.000000 gcsa-2.2.0/gcsa/_services/calendar_lists_service.py
--rw-r--r--   0 ykuzmovy   (501) staff       (20)     3810 2023-05-29 12:12:43.000000 gcsa-2.2.0/gcsa/_services/calendars_service.py
--rw-r--r--   0 ykuzmovy   (501) staff       (20)      769 2023-05-29 12:12:43.000000 gcsa-2.2.0/gcsa/_services/colors_service.py
--rw-r--r--   0 ykuzmovy   (501) staff       (20)    17471 2023-05-29 12:12:43.000000 gcsa-2.2.0/gcsa/_services/events_service.py
--rw-r--r--   0 ykuzmovy   (501) staff       (20)     3816 2023-05-29 12:12:43.000000 gcsa-2.2.0/gcsa/_services/free_busy_service.py
--rw-r--r--   0 ykuzmovy   (501) staff       (20)      569 2023-05-29 12:12:43.000000 gcsa-2.2.0/gcsa/_services/settings_service.py
--rw-r--r--   0 ykuzmovy   (501) staff       (20)     2198 2023-05-29 12:12:43.000000 gcsa-2.2.0/gcsa/acl.py
--rw-r--r--   0 ykuzmovy   (501) staff       (20)     2824 2023-05-29 12:12:43.000000 gcsa-2.2.0/gcsa/attachment.py
--rw-r--r--   0 ykuzmovy   (501) staff       (20)     3023 2023-05-29 12:12:43.000000 gcsa-2.2.0/gcsa/attendee.py
--rw-r--r--   0 ykuzmovy   (501) staff       (20)    11248 2023-05-29 12:12:43.000000 gcsa-2.2.0/gcsa/calendar.py
--rw-r--r--   0 ykuzmovy   (501) staff       (20)    17924 2023-05-29 12:12:43.000000 gcsa-2.2.0/gcsa/conference.py
--rw-r--r--   0 ykuzmovy   (501) staff       (20)    13704 2023-11-10 13:50:13.000000 gcsa-2.2.0/gcsa/event.py
--rw-r--r--   0 ykuzmovy   (501) staff       (20)     3879 2023-05-29 12:12:43.000000 gcsa-2.2.0/gcsa/free_busy.py
--rw-r--r--   0 ykuzmovy   (501) staff       (20)     3512 2023-11-10 14:02:32.000000 gcsa-2.2.0/gcsa/google_calendar.py
--rw-r--r--   0 ykuzmovy   (501) staff       (20)     1447 2023-05-29 12:12:43.000000 gcsa-2.2.0/gcsa/person.py
--rw-r--r--   0 ykuzmovy   (501) staff       (20)    23036 2023-05-29 12:12:43.000000 gcsa-2.2.0/gcsa/recurrence.py
--rw-r--r--   0 ykuzmovy   (501) staff       (20)     1478 2023-05-29 12:12:43.000000 gcsa-2.2.0/gcsa/reminders.py
-drwxr-xr-x   0 ykuzmovy   (501) staff       (20)        0 2023-11-13 13:22:32.784428 gcsa-2.2.0/gcsa/serializers/
--rw-r--r--   0 ykuzmovy   (501) staff       (20)        0 2023-05-29 12:12:43.000000 gcsa-2.2.0/gcsa/serializers/__init__.py
--rw-r--r--   0 ykuzmovy   (501) staff       (20)      949 2023-05-29 12:12:43.000000 gcsa-2.2.0/gcsa/serializers/acl_rule_serializer.py
--rw-r--r--   0 ykuzmovy   (501) staff       (20)     1001 2023-05-29 12:12:43.000000 gcsa-2.2.0/gcsa/serializers/attachment_serializer.py
--rw-r--r--   0 ykuzmovy   (501) staff       (20)     1211 2023-05-29 12:12:43.000000 gcsa-2.2.0/gcsa/serializers/attendee_serializer.py
--rw-r--r--   0 ykuzmovy   (501) staff       (20)     2545 2023-05-29 12:12:43.000000 gcsa-2.2.0/gcsa/serializers/base_serializer.py
--rw-r--r--   0 ykuzmovy   (501) staff       (20)     4393 2023-05-29 12:12:43.000000 gcsa-2.2.0/gcsa/serializers/calendar_serializer.py
--rw-r--r--   0 ykuzmovy   (501) staff       (20)     4644 2023-05-29 12:12:43.000000 gcsa-2.2.0/gcsa/serializers/conference_serializer.py
--rw-r--r--   0 ykuzmovy   (501) staff       (20)     6860 2023-05-29 12:12:43.000000 gcsa-2.2.0/gcsa/serializers/event_serializer.py
--rw-r--r--   0 ykuzmovy   (501) staff       (20)     2860 2023-05-29 12:12:43.000000 gcsa-2.2.0/gcsa/serializers/free_busy_serializer.py
--rw-r--r--   0 ykuzmovy   (501) staff       (20)      712 2023-05-29 12:12:43.000000 gcsa-2.2.0/gcsa/serializers/person_serializer.py
--rw-r--r--   0 ykuzmovy   (501) staff       (20)      806 2023-05-29 12:12:43.000000 gcsa-2.2.0/gcsa/serializers/reminder_serializer.py
--rw-r--r--   0 ykuzmovy   (501) staff       (20)     2020 2023-05-29 12:12:43.000000 gcsa-2.2.0/gcsa/serializers/settings_serializer.py
--rw-r--r--   0 ykuzmovy   (501) staff       (20)     3791 2023-05-29 12:12:43.000000 gcsa-2.2.0/gcsa/settings.py
-drwxr-xr-x   0 ykuzmovy   (501) staff       (20)        0 2023-11-13 13:22:32.784816 gcsa-2.2.0/gcsa/util/
--rw-r--r--   0 ykuzmovy   (501) staff       (20)        0 2023-05-29 12:12:43.000000 gcsa-2.2.0/gcsa/util/__init__.py
--rw-r--r--   0 ykuzmovy   (501) staff       (20)      806 2023-05-29 12:12:43.000000 gcsa-2.2.0/gcsa/util/date_time_util.py
-drwxr-xr-x   0 ykuzmovy   (501) staff       (20)        0 2023-11-13 13:22:32.780112 gcsa-2.2.0/gcsa.egg-info/
--rw-r--r--   0 ykuzmovy   (501) staff       (20)     3436 2023-11-13 13:22:32.000000 gcsa-2.2.0/gcsa.egg-info/PKG-INFO
--rw-r--r--   0 ykuzmovy   (501) staff       (20)     1591 2023-11-13 13:22:32.000000 gcsa-2.2.0/gcsa.egg-info/SOURCES.txt
--rw-r--r--   0 ykuzmovy   (501) staff       (20)        1 2023-11-13 13:22:32.000000 gcsa-2.2.0/gcsa.egg-info/dependency_links.txt
--rw-r--r--   0 ykuzmovy   (501) staff       (20)        1 2023-06-01 13:05:08.000000 gcsa-2.2.0/gcsa.egg-info/not-zip-safe
--rw-r--r--   0 ykuzmovy   (501) staff       (20)      376 2023-11-13 13:22:32.000000 gcsa-2.2.0/gcsa.egg-info/requires.txt
--rw-r--r--   0 ykuzmovy   (501) staff       (20)        5 2023-11-13 13:22:32.000000 gcsa-2.2.0/gcsa.egg-info/top_level.txt
--rw-r--r--   0 ykuzmovy   (501) staff       (20)       38 2023-11-13 13:22:32.789155 gcsa-2.2.0/setup.cfg
--rwxr-xr-x   0 ykuzmovy   (501) staff       (20)     3469 2023-11-13 13:17:52.000000 gcsa-2.2.0/setup.py
-drwxr-xr-x   0 ykuzmovy   (501) staff       (20)        0 2023-11-13 13:22:32.788615 gcsa-2.2.0/tests/
--rw-r--r--   0 ykuzmovy   (501) staff       (20)     1766 2023-05-29 12:12:43.000000 gcsa-2.2.0/tests/test_acl_rule.py
--rw-r--r--   0 ykuzmovy   (501) staff       (20)     4063 2023-05-29 12:12:43.000000 gcsa-2.2.0/tests/test_attachment.py
--rw-r--r--   0 ykuzmovy   (501) staff       (20)     3343 2023-05-29 12:12:43.000000 gcsa-2.2.0/tests/test_attendee.py
--rw-r--r--   0 ykuzmovy   (501) staff       (20)     2187 2023-05-29 12:12:43.000000 gcsa-2.2.0/tests/test_base_serializer.py
--rw-r--r--   0 ykuzmovy   (501) staff       (20)    14086 2023-05-29 12:12:43.000000 gcsa-2.2.0/tests/test_calendar.py
--rw-r--r--   0 ykuzmovy   (501) staff       (20)    20208 2023-05-29 12:12:43.000000 gcsa-2.2.0/tests/test_conference.py
--rw-r--r--   0 ykuzmovy   (501) staff       (20)    29871 2023-05-29 12:12:43.000000 gcsa-2.2.0/tests/test_event.py
--rw-r--r--   0 ykuzmovy   (501) staff       (20)     7559 2023-05-29 12:12:43.000000 gcsa-2.2.0/tests/test_free_busy.py
--rw-r--r--   0 ykuzmovy   (501) staff       (20)     1379 2023-05-29 12:12:43.000000 gcsa-2.2.0/tests/test_person.py
--rw-r--r--   0 ykuzmovy   (501) staff       (20)    10584 2023-05-29 12:12:43.000000 gcsa-2.2.0/tests/test_recurrence.py
--rw-r--r--   0 ykuzmovy   (501) staff       (20)     2495 2023-05-29 12:12:43.000000 gcsa-2.2.0/tests/test_reminder.py
--rw-r--r--   0 ykuzmovy   (501) staff       (20)     3937 2023-05-29 12:12:43.000000 gcsa-2.2.0/tests/test_settings.py
--rw-r--r--   0 ykuzmovy   (501) staff       (20)      833 2023-05-29 12:12:43.000000 gcsa-2.2.0/tests/test_util.py
+drwxr-xr-x   0 ykuzmovy   (501) staff       (20)        0 2024-05-10 10:13:08.553292 gcsa-2.3.0/
+-rw-r--r--   0 ykuzmovy   (501) staff       (20)     1057 2023-05-29 12:12:43.000000 gcsa-2.3.0/LICENSE
+-rw-r--r--   0 ykuzmovy   (501) staff       (20)     4631 2024-05-10 10:13:08.553021 gcsa-2.3.0/PKG-INFO
+-rw-r--r--   0 ykuzmovy   (501) staff       (20)     2428 2023-05-29 12:12:43.000000 gcsa-2.3.0/README.rst
+drwxr-xr-x   0 ykuzmovy   (501) staff       (20)        0 2024-05-10 10:13:08.542684 gcsa-2.3.0/gcsa/
+-rw-r--r--   0 ykuzmovy   (501) staff       (20)        0 2023-05-29 12:12:43.000000 gcsa-2.3.0/gcsa/__init__.py
+-rw-r--r--   0 ykuzmovy   (501) staff       (20)      124 2023-05-29 12:12:43.000000 gcsa-2.3.0/gcsa/_resource.py
+drwxr-xr-x   0 ykuzmovy   (501) staff       (20)        0 2024-05-10 10:13:08.545802 gcsa-2.3.0/gcsa/_services/
+-rw-r--r--   0 ykuzmovy   (501) staff       (20)        0 2023-05-29 12:12:43.000000 gcsa-2.3.0/gcsa/_services/__init__.py
+-rw-r--r--   0 ykuzmovy   (501) staff       (20)     5856 2023-05-29 12:12:43.000000 gcsa-2.3.0/gcsa/_services/acl_service.py
+-rw-r--r--   0 ykuzmovy   (501) staff       (20)     6390 2024-05-07 13:31:05.000000 gcsa-2.3.0/gcsa/_services/authentication.py
+-rw-r--r--   0 ykuzmovy   (501) staff       (20)     2324 2023-05-29 12:12:43.000000 gcsa-2.3.0/gcsa/_services/base_service.py
+-rw-r--r--   0 ykuzmovy   (501) staff       (20)     5394 2023-05-29 12:12:43.000000 gcsa-2.3.0/gcsa/_services/calendar_lists_service.py
+-rw-r--r--   0 ykuzmovy   (501) staff       (20)     3810 2023-05-29 12:12:43.000000 gcsa-2.3.0/gcsa/_services/calendars_service.py
+-rw-r--r--   0 ykuzmovy   (501) staff       (20)      769 2023-05-29 12:12:43.000000 gcsa-2.3.0/gcsa/_services/colors_service.py
+-rw-r--r--   0 ykuzmovy   (501) staff       (20)    17471 2024-05-07 09:48:55.000000 gcsa-2.3.0/gcsa/_services/events_service.py
+-rw-r--r--   0 ykuzmovy   (501) staff       (20)     3816 2024-05-07 09:48:55.000000 gcsa-2.3.0/gcsa/_services/free_busy_service.py
+-rw-r--r--   0 ykuzmovy   (501) staff       (20)      569 2023-05-29 12:12:43.000000 gcsa-2.3.0/gcsa/_services/settings_service.py
+-rw-r--r--   0 ykuzmovy   (501) staff       (20)     2198 2023-05-29 12:12:43.000000 gcsa-2.3.0/gcsa/acl.py
+-rw-r--r--   0 ykuzmovy   (501) staff       (20)     2824 2023-05-29 12:12:43.000000 gcsa-2.3.0/gcsa/attachment.py
+-rw-r--r--   0 ykuzmovy   (501) staff       (20)     3023 2023-05-29 12:12:43.000000 gcsa-2.3.0/gcsa/attendee.py
+-rw-r--r--   0 ykuzmovy   (501) staff       (20)    11248 2024-05-07 09:48:55.000000 gcsa-2.3.0/gcsa/calendar.py
+-rw-r--r--   0 ykuzmovy   (501) staff       (20)    17924 2023-05-29 12:12:43.000000 gcsa-2.3.0/gcsa/conference.py
+-rw-r--r--   0 ykuzmovy   (501) staff       (20)    14230 2024-05-07 11:47:31.000000 gcsa-2.3.0/gcsa/event.py
+-rw-r--r--   0 ykuzmovy   (501) staff       (20)     3879 2023-05-29 12:12:43.000000 gcsa-2.3.0/gcsa/free_busy.py
+-rw-r--r--   0 ykuzmovy   (501) staff       (20)     3829 2024-05-07 11:47:33.000000 gcsa-2.3.0/gcsa/google_calendar.py
+-rw-r--r--   0 ykuzmovy   (501) staff       (20)     1447 2023-05-29 12:12:43.000000 gcsa-2.3.0/gcsa/person.py
+-rw-r--r--   0 ykuzmovy   (501) staff       (20)    23036 2024-05-07 09:48:55.000000 gcsa-2.3.0/gcsa/recurrence.py
+-rw-r--r--   0 ykuzmovy   (501) staff       (20)     5205 2024-04-16 17:00:29.000000 gcsa-2.3.0/gcsa/reminders.py
+drwxr-xr-x   0 ykuzmovy   (501) staff       (20)        0 2024-05-10 10:13:08.548113 gcsa-2.3.0/gcsa/serializers/
+-rw-r--r--   0 ykuzmovy   (501) staff       (20)        0 2023-05-29 12:12:43.000000 gcsa-2.3.0/gcsa/serializers/__init__.py
+-rw-r--r--   0 ykuzmovy   (501) staff       (20)      949 2023-05-29 12:12:43.000000 gcsa-2.3.0/gcsa/serializers/acl_rule_serializer.py
+-rw-r--r--   0 ykuzmovy   (501) staff       (20)     1001 2023-05-29 12:12:43.000000 gcsa-2.3.0/gcsa/serializers/attachment_serializer.py
+-rw-r--r--   0 ykuzmovy   (501) staff       (20)     1211 2023-05-29 12:12:43.000000 gcsa-2.3.0/gcsa/serializers/attendee_serializer.py
+-rw-r--r--   0 ykuzmovy   (501) staff       (20)     2545 2023-05-29 12:12:43.000000 gcsa-2.3.0/gcsa/serializers/base_serializer.py
+-rw-r--r--   0 ykuzmovy   (501) staff       (20)     4393 2023-05-29 12:12:43.000000 gcsa-2.3.0/gcsa/serializers/calendar_serializer.py
+-rw-r--r--   0 ykuzmovy   (501) staff       (20)     4644 2023-05-29 12:12:43.000000 gcsa-2.3.0/gcsa/serializers/conference_serializer.py
+-rw-r--r--   0 ykuzmovy   (501) staff       (20)     6621 2024-04-16 15:23:36.000000 gcsa-2.3.0/gcsa/serializers/event_serializer.py
+-rw-r--r--   0 ykuzmovy   (501) staff       (20)     2860 2023-05-29 12:12:43.000000 gcsa-2.3.0/gcsa/serializers/free_busy_serializer.py
+-rw-r--r--   0 ykuzmovy   (501) staff       (20)      712 2023-05-29 12:12:43.000000 gcsa-2.3.0/gcsa/serializers/person_serializer.py
+-rw-r--r--   0 ykuzmovy   (501) staff       (20)      806 2023-05-29 12:12:43.000000 gcsa-2.3.0/gcsa/serializers/reminder_serializer.py
+-rw-r--r--   0 ykuzmovy   (501) staff       (20)     2020 2023-05-29 12:12:43.000000 gcsa-2.3.0/gcsa/serializers/settings_serializer.py
+-rw-r--r--   0 ykuzmovy   (501) staff       (20)     3791 2023-05-29 12:12:43.000000 gcsa-2.3.0/gcsa/settings.py
+drwxr-xr-x   0 ykuzmovy   (501) staff       (20)        0 2024-05-10 10:13:08.548401 gcsa-2.3.0/gcsa/util/
+-rw-r--r--   0 ykuzmovy   (501) staff       (20)        0 2023-05-29 12:12:43.000000 gcsa-2.3.0/gcsa/util/__init__.py
+-rw-r--r--   0 ykuzmovy   (501) staff       (20)      806 2024-05-07 09:48:55.000000 gcsa-2.3.0/gcsa/util/date_time_util.py
+drwxr-xr-x   0 ykuzmovy   (501) staff       (20)        0 2024-05-10 10:13:08.543681 gcsa-2.3.0/gcsa.egg-info/
+-rw-r--r--   0 ykuzmovy   (501) staff       (20)     4631 2024-05-10 10:13:08.000000 gcsa-2.3.0/gcsa.egg-info/PKG-INFO
+-rw-r--r--   0 ykuzmovy   (501) staff       (20)     1591 2024-05-10 10:13:08.000000 gcsa-2.3.0/gcsa.egg-info/SOURCES.txt
+-rw-r--r--   0 ykuzmovy   (501) staff       (20)        1 2024-05-10 10:13:08.000000 gcsa-2.3.0/gcsa.egg-info/dependency_links.txt
+-rw-r--r--   0 ykuzmovy   (501) staff       (20)        1 2023-06-01 13:05:08.000000 gcsa-2.3.0/gcsa.egg-info/not-zip-safe
+-rw-r--r--   0 ykuzmovy   (501) staff       (20)      376 2024-05-10 10:13:08.000000 gcsa-2.3.0/gcsa.egg-info/requires.txt
+-rw-r--r--   0 ykuzmovy   (501) staff       (20)        5 2024-05-10 10:13:08.000000 gcsa-2.3.0/gcsa.egg-info/top_level.txt
+-rw-r--r--   0 ykuzmovy   (501) staff       (20)       38 2024-05-10 10:13:08.553356 gcsa-2.3.0/setup.cfg
+-rwxr-xr-x   0 ykuzmovy   (501) staff       (20)     4465 2024-05-10 08:51:56.000000 gcsa-2.3.0/setup.py
+drwxr-xr-x   0 ykuzmovy   (501) staff       (20)        0 2024-05-10 10:13:08.551780 gcsa-2.3.0/tests/
+-rw-r--r--   0 ykuzmovy   (501) staff       (20)     1766 2023-05-29 12:12:43.000000 gcsa-2.3.0/tests/test_acl_rule.py
+-rw-r--r--   0 ykuzmovy   (501) staff       (20)     4063 2023-05-29 12:12:43.000000 gcsa-2.3.0/tests/test_attachment.py
+-rw-r--r--   0 ykuzmovy   (501) staff       (20)     3343 2023-05-29 12:12:43.000000 gcsa-2.3.0/tests/test_attendee.py
+-rw-r--r--   0 ykuzmovy   (501) staff       (20)     2187 2023-05-29 12:12:43.000000 gcsa-2.3.0/tests/test_base_serializer.py
+-rw-r--r--   0 ykuzmovy   (501) staff       (20)    14086 2023-05-29 12:12:43.000000 gcsa-2.3.0/tests/test_calendar.py
+-rw-r--r--   0 ykuzmovy   (501) staff       (20)    20208 2023-05-29 12:12:43.000000 gcsa-2.3.0/tests/test_conference.py
+-rw-r--r--   0 ykuzmovy   (501) staff       (20)    32145 2024-04-16 16:06:11.000000 gcsa-2.3.0/tests/test_event.py
+-rw-r--r--   0 ykuzmovy   (501) staff       (20)     7559 2023-05-29 12:12:43.000000 gcsa-2.3.0/tests/test_free_busy.py
+-rw-r--r--   0 ykuzmovy   (501) staff       (20)     1379 2023-05-29 12:12:43.000000 gcsa-2.3.0/tests/test_person.py
+-rw-r--r--   0 ykuzmovy   (501) staff       (20)    10584 2023-05-29 12:12:43.000000 gcsa-2.3.0/tests/test_recurrence.py
+-rw-r--r--   0 ykuzmovy   (501) staff       (20)     5433 2024-04-16 15:13:34.000000 gcsa-2.3.0/tests/test_reminder.py
+-rw-r--r--   0 ykuzmovy   (501) staff       (20)     3937 2023-05-29 12:12:43.000000 gcsa-2.3.0/tests/test_settings.py
+-rw-r--r--   0 ykuzmovy   (501) staff       (20)      833 2023-05-29 12:12:43.000000 gcsa-2.3.0/tests/test_util.py
```

### Comparing `gcsa-2.2.0/LICENSE` & `gcsa-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gcsa-2.2.0/README.rst` & `gcsa-2.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `gcsa-2.2.0/gcsa/_services/acl_service.py` & `gcsa-2.3.0/gcsa/_services/acl_service.py`

 * *Files identical despite different names*

### Comparing `gcsa-2.2.0/gcsa/_services/authentication.py` & `gcsa-2.3.0/gcsa/_services/authentication.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os.path
 import glob
 from typing import List
 
 from googleapiclient import discovery
 from google_auth_oauthlib.flow import InstalledAppFlow
 from google.auth.transport.requests import Request
-from google.oauth2.credentials import Credentials
+from google.auth.credentials import Credentials
 
 
 class AuthenticatedService:
     """Handles authentication of the `GoogleCalendar`"""
 
     _READ_WRITE_SCOPES = 'https://www.googleapis.com/auth/calendar'
     _LIST_ORDERS = ("startTime", "updated")
@@ -20,15 +20,16 @@
             *,
             credentials: Credentials = None,
             credentials_path: str = None,
             token_path: str = None,
             save_token: bool = True,
             read_only: bool = False,
             authentication_flow_host: str = 'localhost',
-            authentication_flow_port: int = 8080
+            authentication_flow_port: int = 8080,
+            authentication_flow_bind_addr: str = None
     ):
         """
         Specify ``credentials`` to use in requests or ``credentials_path`` and ``token_path`` to get credentials from.
 
         :param credentials:
                 Credentials with token and refresh token.
                 If specified, ``credentials_path``, ``token_path``, and ``save_token`` are ignored.
@@ -45,14 +46,17 @@
                 Whether to pickle token after authentication flow for future uses
         :param read_only:
                 If require read only access. Default: False
         :param authentication_flow_host:
                 Host to receive response during authentication flow
         :param authentication_flow_port:
                 Port to receive response during authentication flow
+        :param authentication_flow_bind_addr:
+                Optional IP address for the redirect server to listen on when it is not the same as host
+                (e.g. in a container)
         """
 
         if credentials:
             self.credentials = self._ensure_refreshed(credentials)
         else:
             credentials_path = credentials_path or self._get_default_credentials_path()
             credentials_dir, credentials_file = os.path.split(credentials_path)
@@ -62,50 +66,52 @@
             self.credentials = self._get_credentials(
                 token_path,
                 credentials_dir,
                 credentials_file,
                 scopes,
                 save_token,
                 authentication_flow_host,
-                authentication_flow_port
+                authentication_flow_port,
+                authentication_flow_bind_addr
             )
 
         self.service = discovery.build('calendar', 'v3', credentials=self.credentials)
 
     @staticmethod
     def _ensure_refreshed(
             credentials: Credentials
     ) -> Credentials:
-        if not credentials.valid and credentials.expired and credentials.refresh_token:
+        if not credentials.valid and credentials.expired:
             credentials.refresh(Request())
         return credentials
 
     @staticmethod
     def _get_credentials(
             token_path: str,
             credentials_dir: str,
             credentials_file: str,
             scopes: List[str],
             save_token: bool,
             host: str,
-            port: int
+            port: int,
+            bind_addr: str
     ) -> Credentials:
         credentials = None
 
         if os.path.exists(token_path):
             with open(token_path, 'rb') as token_file:
                 credentials = pickle.load(token_file)
 
         if not credentials or not credentials.valid:
             if credentials and credentials.expired and credentials.refresh_token:
                 credentials.refresh(Request())
             else:
                 credentials_path = os.path.join(credentials_dir, credentials_file)
                 flow = InstalledAppFlow.from_client_secrets_file(credentials_path, scopes)
-                credentials = flow.run_local_server(host=host, port=port)
+                credentials = flow.run_local_server(host=host, port=port, bind_addr=bind_addr)
 
             if save_token:
                 with open(token_path, 'wb') as token_file:
                     pickle.dump(credentials, token_file)
 
         return credentials
```

### Comparing `gcsa-2.2.0/gcsa/_services/base_service.py` & `gcsa-2.3.0/gcsa/_services/base_service.py`

 * *Files identical despite different names*

### Comparing `gcsa-2.2.0/gcsa/_services/calendar_lists_service.py` & `gcsa-2.3.0/gcsa/_services/calendar_lists_service.py`

 * *Files identical despite different names*

### Comparing `gcsa-2.2.0/gcsa/_services/calendars_service.py` & `gcsa-2.3.0/gcsa/_services/calendars_service.py`

 * *Files identical despite different names*

### Comparing `gcsa-2.2.0/gcsa/_services/colors_service.py` & `gcsa-2.3.0/gcsa/_services/colors_service.py`

 * *Files identical despite different names*

### Comparing `gcsa-2.2.0/gcsa/_services/events_service.py` & `gcsa-2.3.0/gcsa/_services/events_service.py`

 * *Files identical despite different names*

### Comparing `gcsa-2.2.0/gcsa/_services/free_busy_service.py` & `gcsa-2.3.0/gcsa/_services/free_busy_service.py`

 * *Files identical despite different names*

### Comparing `gcsa-2.2.0/gcsa/_services/settings_service.py` & `gcsa-2.3.0/gcsa/_services/settings_service.py`

 * *Files identical despite different names*

### Comparing `gcsa-2.2.0/gcsa/acl.py` & `gcsa-2.3.0/gcsa/acl.py`

 * *Files identical despite different names*

### Comparing `gcsa-2.2.0/gcsa/attachment.py` & `gcsa-2.3.0/gcsa/attachment.py`

 * *Files identical despite different names*

### Comparing `gcsa-2.2.0/gcsa/attendee.py` & `gcsa-2.3.0/gcsa/attendee.py`

 * *Files identical despite different names*

### Comparing `gcsa-2.2.0/gcsa/calendar.py` & `gcsa-2.3.0/gcsa/calendar.py`

 * *Files identical despite different names*

### Comparing `gcsa-2.2.0/gcsa/conference.py` & `gcsa-2.3.0/gcsa/conference.py`

 * *Files identical despite different names*

### Comparing `gcsa-2.2.0/gcsa/event.py` & `gcsa-2.3.0/gcsa/event.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from functools import total_ordering
 from typing import List, Union
 
 from beautiful_date import BeautifulDate
 from tzlocal import get_localzone_name
-from datetime import datetime, date, timedelta
+from datetime import datetime, date, timedelta, time
 
 from ._resource import Resource
 from .attachment import Attachment
 from .attendee import Attendee
 from .conference import ConferenceSolution, ConferenceSolutionCreateRequest
 from .person import Person
 from .reminders import PopupReminder, EmailReminder, Reminder
@@ -219,36 +219,49 @@
             self,
             attendee: Union[str, Attendee]
     ):
         """Adds attendee to an event. See :py:class:`~gcsa.attendee.Attendee`.
         Attendee may be given as email string or :py:class:`~gcsa.attendee.Attendee` object."""
         self.attendees.append(self._ensure_attendee_from_email(attendee))
 
+    def add_attendees(
+            self,
+            attendees: List[Union[str, Attendee]]
+    ):
+        """Adds multiple attendees to an event. See :py:class:`~gcsa.attendee.Attendee`.
+        Each attendee may be given as email string or :py:class:`~gcsa.attendee.Attendee` object."""
+        for a in attendees:
+            self.add_attendee(a)
+
     def add_attachment(
             self,
             file_url: str,
             title: str = None,
             mime_type: str = None
     ):
         """Adds attachment to an event. See :py:class:`~gcsa.attachment.Attachment`"""
         self.attachments.append(Attachment(file_url=file_url, title=title, mime_type=mime_type))
 
     def add_email_reminder(
             self,
-            minutes_before_start: int = 60
+            minutes_before_start: int = None,
+            days_before: int = None,
+            at: time = None
     ):
         """Adds email reminder to an event. See :py:class:`~gcsa.reminders.EmailReminder`"""
-        self.add_reminder(EmailReminder(minutes_before_start))
+        self.add_reminder(EmailReminder(minutes_before_start, days_before, at))
 
     def add_popup_reminder(
             self,
-            minutes_before_start: int = 30
+            minutes_before_start: int = None,
+            days_before: int = None,
+            at: time = None
     ):
         """Adds popup reminder to an event. See :py:class:`~gcsa.reminders.PopupReminder`"""
-        self.add_reminder(PopupReminder(minutes_before_start))
+        self.add_reminder(PopupReminder(minutes_before_start, days_before, at))
 
     def add_reminder(
             self,
             reminder: Reminder
     ):
         """Adds reminder to an event. See :py:mod:`~gcsa.reminders`"""
         if len(self.reminders) > 4:
```

### Comparing `gcsa-2.2.0/gcsa/free_busy.py` & `gcsa-2.3.0/gcsa/free_busy.py`

 * *Files identical despite different names*

### Comparing `gcsa-2.2.0/gcsa/google_calendar.py` & `gcsa-2.3.0/gcsa/google_calendar.py`

 * *Files 9% similar despite different names*

```diff
@@ -26,15 +26,16 @@
             *,
             credentials: Credentials = None,
             credentials_path: str = None,
             token_path: str = None,
             save_token: bool = True,
             read_only: bool = False,
             authentication_flow_host: str = 'localhost',
-            authentication_flow_port: int = 8080
+            authentication_flow_port: int = 8080,
+            authentication_flow_bind_addr: str = None
     ):
         """
         Specify ``credentials`` to use in requests or ``credentials_path`` and ``token_path`` to get credentials from.
 
         :param default_calendar:
                 Users email address or name/id of the calendar. Default: primary calendar of the user
 
@@ -59,18 +60,22 @@
                 Whether to pickle token after authentication flow for future uses
         :param read_only:
                 If require read only access. Default: False
         :param authentication_flow_host:
                 Host to receive response during authentication flow
         :param authentication_flow_port:
                 Port to receive response during authentication flow
+        :param authentication_flow_bind_addr:
+                Optional IP address for the redirect server to listen on when it is not the same as host
+                (e.g. in a container)
         """
         super().__init__(
             default_calendar=default_calendar,
             credentials=credentials,
             credentials_path=credentials_path,
             token_path=token_path,
             save_token=save_token,
             read_only=read_only,
             authentication_flow_host=authentication_flow_host,
-            authentication_flow_port=authentication_flow_port
+            authentication_flow_port=authentication_flow_port,
+            authentication_flow_bind_addr=authentication_flow_bind_addr
         )
```

### Comparing `gcsa-2.2.0/gcsa/person.py` & `gcsa-2.3.0/gcsa/person.py`

 * *Files identical despite different names*

### Comparing `gcsa-2.2.0/gcsa/recurrence.py` & `gcsa-2.3.0/gcsa/recurrence.py`

 * *Files identical despite different names*

### Comparing `gcsa-2.2.0/gcsa/serializers/acl_rule_serializer.py` & `gcsa-2.3.0/gcsa/serializers/acl_rule_serializer.py`

 * *Files identical despite different names*

### Comparing `gcsa-2.2.0/gcsa/serializers/attachment_serializer.py` & `gcsa-2.3.0/gcsa/serializers/attachment_serializer.py`

 * *Files identical despite different names*

### Comparing `gcsa-2.2.0/gcsa/serializers/attendee_serializer.py` & `gcsa-2.3.0/gcsa/serializers/attendee_serializer.py`

 * *Files identical despite different names*

### Comparing `gcsa-2.2.0/gcsa/serializers/base_serializer.py` & `gcsa-2.3.0/gcsa/serializers/base_serializer.py`

 * *Files identical despite different names*

### Comparing `gcsa-2.2.0/gcsa/serializers/calendar_serializer.py` & `gcsa-2.3.0/gcsa/serializers/calendar_serializer.py`

 * *Files identical despite different names*

### Comparing `gcsa-2.2.0/gcsa/serializers/conference_serializer.py` & `gcsa-2.3.0/gcsa/serializers/conference_serializer.py`

 * *Files identical despite different names*

### Comparing `gcsa-2.2.0/gcsa/serializers/event_serializer.py` & `gcsa-2.3.0/gcsa/serializers/event_serializer.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,18 +29,14 @@
             'colorId': event.color_id,
             'visibility': event.visibility,
             'attendees': [AttendeeSerializer.to_json(a) for a in event.attendees],
             'guestsCanInviteOthers': event.guests_can_invite_others,
             'guestsCanModify': event.guests_can_modify,
             'guestsCanSeeOtherGuests': event.guests_can_see_other_guests,
             'transparency': event.transparency,
-            'reminders': {
-                'useDefault': event.default_reminders,
-                'overrides': [ReminderSerializer.to_json(r) for r in event.reminders]
-            },
             'attachments': [AttachmentSerializer.to_json(a) for a in event.attachments],
             **event.other
         }
 
         if isinstance(event.start, datetime) and isinstance(event.end, datetime):
             data['start'] = {
                 'dateTime': event.start.isoformat(),
@@ -50,24 +46,22 @@
                 'dateTime': event.end.isoformat(),
                 'timeZone': event.timezone
             }
         elif isinstance(event.start, date) and isinstance(event.end, date):
             data['start'] = {'date': event.start.isoformat()}
             data['end'] = {'date': event.end.isoformat()}
 
-        if event.default_reminders:
-            data['reminders'] = {
-                'useDefault': True
-            }
-        else:
-            data['reminders'] = {
-                'useDefault': False
-            }
-            if event.reminders:
-                data['reminders']['overrides'] = [ReminderSerializer.to_json(r) for r in event.reminders]
+        data['reminders'] = {
+            'useDefault': event.default_reminders
+        }
+        if event.reminders:
+            data['reminders']['overrides'] = [
+                ReminderSerializer.to_json(r.convert_to_relative(event.start))
+                for r in event.reminders
+            ]
 
         if event.conference_solution is not None:
             if isinstance(event.conference_solution, ConferenceSolution):
                 data['conferenceData'] = ConferenceSolutionSerializer.to_json(event.conference_solution)
             elif isinstance(event.conference_solution, ConferenceSolutionCreateRequest):
                 data['conferenceData'] = ConferenceSolutionCreateRequestSerializer.to_json(event.conference_solution)
```

### Comparing `gcsa-2.2.0/gcsa/serializers/free_busy_serializer.py` & `gcsa-2.3.0/gcsa/serializers/free_busy_serializer.py`

 * *Files identical despite different names*

### Comparing `gcsa-2.2.0/gcsa/serializers/person_serializer.py` & `gcsa-2.3.0/gcsa/serializers/person_serializer.py`

 * *Files identical despite different names*

### Comparing `gcsa-2.2.0/gcsa/serializers/reminder_serializer.py` & `gcsa-2.3.0/gcsa/serializers/reminder_serializer.py`

 * *Files identical despite different names*

### Comparing `gcsa-2.2.0/gcsa/serializers/settings_serializer.py` & `gcsa-2.3.0/gcsa/serializers/settings_serializer.py`

 * *Files identical despite different names*

### Comparing `gcsa-2.2.0/gcsa/settings.py` & `gcsa-2.3.0/gcsa/settings.py`

 * *Files identical despite different names*

### Comparing `gcsa-2.2.0/gcsa/util/date_time_util.py` & `gcsa-2.3.0/gcsa/util/date_time_util.py`

 * *Files identical despite different names*

### Comparing `gcsa-2.2.0/gcsa.egg-info/SOURCES.txt` & `gcsa-2.3.0/gcsa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gcsa-2.2.0/tests/test_acl_rule.py` & `gcsa-2.3.0/tests/test_acl_rule.py`

 * *Files identical despite different names*

### Comparing `gcsa-2.2.0/tests/test_attachment.py` & `gcsa-2.3.0/tests/test_attachment.py`

 * *Files identical despite different names*

### Comparing `gcsa-2.2.0/tests/test_attendee.py` & `gcsa-2.3.0/tests/test_attendee.py`

 * *Files identical despite different names*

### Comparing `gcsa-2.2.0/tests/test_base_serializer.py` & `gcsa-2.3.0/tests/test_base_serializer.py`

 * *Files identical despite different names*

### Comparing `gcsa-2.2.0/tests/test_calendar.py` & `gcsa-2.3.0/tests/test_calendar.py`

 * *Files identical despite different names*

### Comparing `gcsa-2.2.0/tests/test_conference.py` & `gcsa-2.3.0/tests/test_conference.py`

 * *Files identical despite different names*

### Comparing `gcsa-2.2.0/tests/test_event.py` & `gcsa-2.3.0/tests/test_event.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from datetime import time
 from unittest import TestCase
 from beautiful_date import Jan, Feb, Mar, Apr, May, Jun, Jul, Aug, Sept, Oct, Dec, hours, days, Nov
 
 from gcsa.attachment import Attachment
 from gcsa.attendee import Attendee, ResponseStatus
 from gcsa.conference import ConferenceSolution, EntryPoint, SolutionType, ConferenceSolutionCreateRequest
 from gcsa.event import Event, Visibility
@@ -93,32 +94,50 @@
         self.assertEqual(e.reminders[0].minutes_before_start, 35)
 
         e.add_popup_reminder(41)
         self.assertEqual(len(e.reminders), 2)
         self.assertIsInstance(e.reminders[1], PopupReminder)
         self.assertEqual(e.reminders[1].minutes_before_start, 41)
 
+        e.add_popup_reminder(days_before=1, at=time(12, 0))
+        self.assertEqual(len(e.reminders), 3)
+        self.assertIsInstance(e.reminders[2], PopupReminder)
+        self.assertEqual(e.reminders[2].days_before, 1)
+        self.assertEqual(e.reminders[2].at, time(12, 0))
+
+        e.add_email_reminder(days_before=1, at=time(13, 30))
+        self.assertEqual(len(e.reminders), 4)
+        self.assertIsInstance(e.reminders[3], EmailReminder)
+        self.assertEqual(e.reminders[3].days_before, 1)
+        self.assertEqual(e.reminders[3].at, time(13, 30))
+
     def test_add_attendees(self):
         e = Event('Good day',
                   start=(17 / Jul / 2020),
                   timezone=TEST_TIMEZONE,
                   attendees=[
                       Attendee(email="attendee@gmail.com"),
                       "attendee2@gmail.com",
                   ])
 
         self.assertEqual(len(e.attendees), 2)
         e.add_attendee(Attendee("attendee3@gmail.com"))
         e.add_attendee(Attendee(email="attendee4@gmail.com"))
-        self.assertEqual(len(e.attendees), 4)
+        e.add_attendees([
+            Attendee(email="attendee5@gmail.com"),
+            "attendee6@gmail.com"
+        ])
+        self.assertEqual(len(e.attendees), 6)
 
         self.assertEqual(e.attendees[0].email, "attendee@gmail.com")
         self.assertEqual(e.attendees[1].email, "attendee2@gmail.com")
         self.assertEqual(e.attendees[2].email, "attendee3@gmail.com")
         self.assertEqual(e.attendees[3].email, "attendee4@gmail.com")
+        self.assertEqual(e.attendees[4].email, "attendee5@gmail.com")
+        self.assertEqual(e.attendees[5].email, "attendee6@gmail.com")
 
     def test_reminders_checks(self):
         with self.assertRaises(ValueError):
             Event('Too many reminders',
                   start=20 / Jul / 2020,
                   reminders=[EmailReminder()] * 6)
 
@@ -343,14 +362,46 @@
                 ],
                 'useDefault': False
             },
             'attachments': [],
             'guestsCanInviteOthers': True,
             'guestsCanModify': False,
             'guestsCanSeeOtherGuests': True,
+        }
+        self.assertDictEqual(EventSerializer.to_json(e), expected_event_json)
+
+        e = Event('Good day',
+                  start=(1 / Jan / 2019)[11:22:33],
+                  timezone=TEST_TIMEZONE,
+                  reminders=[
+                      PopupReminder(35),
+                      EmailReminder(45),
+                      PopupReminder(days_before=3, at=time(12, 30)),
+                      EmailReminder(days_before=2, at=time(11, 25)),
+                  ])
+        expected_event_json = {
+            'summary': 'Good day',
+            'start': {'dateTime': '2019-01-01T11:22:33+13:00', 'timeZone': TEST_TIMEZONE},
+            'end': {'dateTime': '2019-01-01T12:22:33+13:00', 'timeZone': TEST_TIMEZONE},
+            'recurrence': [],
+            'visibility': 'default',
+            'attendees': [],
+            'reminders': {
+                'overrides': [
+                    {'method': 'popup', 'minutes': 35},
+                    {'method': 'email', 'minutes': 45},
+                    {'method': 'popup', 'minutes': (11 * 60 + 22) + (2 * 24 * 60 + 11 * 60 + 30)},
+                    {'method': 'email', 'minutes': (11 * 60 + 22) + (1 * 24 * 60 + 12 * 60 + 35)},
+                ],
+                'useDefault': False
+            },
+            'attachments': [],
+            'guestsCanInviteOthers': True,
+            'guestsCanModify': False,
+            'guestsCanSeeOtherGuests': True,
         }
         self.assertDictEqual(EventSerializer.to_json(e), expected_event_json)
 
     def test_to_json_attendees(self):
         e = Event('Good day',
                   start=(1 / Jul / 2020)[11:22:33],
                   timezone=TEST_TIMEZONE,
```

### Comparing `gcsa-2.2.0/tests/test_free_busy.py` & `gcsa-2.3.0/tests/test_free_busy.py`

 * *Files identical despite different names*

### Comparing `gcsa-2.2.0/tests/test_person.py` & `gcsa-2.3.0/tests/test_person.py`

 * *Files identical despite different names*

### Comparing `gcsa-2.2.0/tests/test_recurrence.py` & `gcsa-2.3.0/tests/test_recurrence.py`

 * *Files identical despite different names*

### Comparing `gcsa-2.2.0/tests/test_settings.py` & `gcsa-2.3.0/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `gcsa-2.2.0/tests/test_util.py` & `gcsa-2.3.0/tests/test_util.py`

 * *Files identical despite different names*

