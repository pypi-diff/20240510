# Comparing `tmp/django-dbdiff-0.9.5.tar.gz` & `tmp/django-dbdiff-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-dbdiff-0.9.5.tar", last modified: Tue Jan 29 04:21:29 2019, max compression
+gzip compressed data, was "django-dbdiff-0.9.6.tar", last modified: Fri May 10 13:07:14 2024, max compression
```

## Comparing `django-dbdiff-0.9.5.tar` & `django-dbdiff-0.9.6.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2019-01-29 04:21:29.000000 django-dbdiff-0.9.5/
--rw-r--r--   0 jpic      (1000) jpic      (1000)     5990 2019-01-29 04:21:29.000000 django-dbdiff-0.9.5/PKG-INFO
--rw-r--r--   0 jpic      (1000) jpic      (1000)     4249 2019-01-29 04:19:59.000000 django-dbdiff-0.9.5/README.rst
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2019-01-29 04:21:29.000000 django-dbdiff-0.9.5/dbdiff/
--rw-r--r--   0 jpic      (1000) jpic      (1000)      117 2018-02-06 15:07:48.000000 django-dbdiff-0.9.5/dbdiff/__init__.py
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1414 2018-02-06 15:07:48.000000 django-dbdiff-0.9.5/dbdiff/apps.py
--rw-r--r--   0 jpic      (1000) jpic      (1000)     2251 2018-02-06 15:07:48.000000 django-dbdiff-0.9.5/dbdiff/exceptions.py
--rw-r--r--   0 jpic      (1000) jpic      (1000)     4523 2019-01-29 04:20:51.000000 django-dbdiff-0.9.5/dbdiff/fixture.py
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1031 2018-11-18 01:18:28.000000 django-dbdiff-0.9.5/dbdiff/plugin.py
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1791 2018-02-12 13:57:13.000000 django-dbdiff-0.9.5/dbdiff/sequence.py
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2019-01-29 04:21:29.000000 django-dbdiff-0.9.5/dbdiff/serializers/
--rw-r--r--   0 jpic      (1000) jpic      (1000)       53 2018-02-06 15:07:48.000000 django-dbdiff-0.9.5/dbdiff/serializers/__init__.py
--rw-r--r--   0 jpic      (1000) jpic      (1000)     2654 2018-02-06 15:07:48.000000 django-dbdiff-0.9.5/dbdiff/serializers/base.py
--rw-r--r--   0 jpic      (1000) jpic      (1000)      315 2018-02-06 15:07:48.000000 django-dbdiff-0.9.5/dbdiff/serializers/json.py
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1848 2018-02-06 17:54:31.000000 django-dbdiff-0.9.5/dbdiff/test.py
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2019-01-29 04:21:29.000000 django-dbdiff-0.9.5/dbdiff/tests/
--rw-r--r--   0 jpic      (1000) jpic      (1000)       35 2018-02-06 15:07:48.000000 django-dbdiff-0.9.5/dbdiff/tests/__init__.py
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2019-01-29 04:21:29.000000 django-dbdiff-0.9.5/dbdiff/tests/decimal_test/
--rw-r--r--   0 jpic      (1000) jpic      (1000)       52 2018-02-06 15:07:48.000000 django-dbdiff-0.9.5/dbdiff/tests/decimal_test/__init__.py
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2019-01-29 04:21:29.000000 django-dbdiff-0.9.5/dbdiff/tests/decimal_test/migrations/
--rw-r--r--   0 jpic      (1000) jpic      (1000)      510 2018-02-06 15:07:48.000000 django-dbdiff-0.9.5/dbdiff/tests/decimal_test/migrations/0001_initial.py
--rw-r--r--   0 jpic      (1000) jpic      (1000)      423 2018-02-06 15:07:48.000000 django-dbdiff-0.9.5/dbdiff/tests/decimal_test/migrations/0002_auto_20160102_0914.py
--rw-r--r--   0 jpic      (1000) jpic      (1000)        0 2018-02-06 15:07:48.000000 django-dbdiff-0.9.5/dbdiff/tests/decimal_test/migrations/__init__.py
--rw-r--r--   0 jpic      (1000) jpic      (1000)      131 2018-02-06 15:07:48.000000 django-dbdiff-0.9.5/dbdiff/tests/decimal_test/models.py
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2019-01-29 04:21:29.000000 django-dbdiff-0.9.5/dbdiff/tests/inheritance/
--rw-r--r--   0 jpic      (1000) jpic      (1000)       38 2018-02-12 14:45:46.000000 django-dbdiff-0.9.5/dbdiff/tests/inheritance/__init__.py
--rw-r--r--   0 jpic      (1000) jpic      (1000)      134 2018-02-12 13:29:30.000000 django-dbdiff-0.9.5/dbdiff/tests/inheritance/models.py
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2019-01-29 04:21:29.000000 django-dbdiff-0.9.5/dbdiff/tests/nonintpk/
--rw-r--r--   0 jpic      (1000) jpic      (1000)       54 2018-02-06 18:06:19.000000 django-dbdiff-0.9.5/dbdiff/tests/nonintpk/__init__.py
--rw-r--r--   0 jpic      (1000) jpic      (1000)      205 2018-02-06 17:50:00.000000 django-dbdiff-0.9.5/dbdiff/tests/nonintpk/models.py
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2019-01-29 04:21:29.000000 django-dbdiff-0.9.5/dbdiff/tests/project/
--rw-r--r--   0 jpic      (1000) jpic      (1000)       29 2018-02-06 15:07:48.000000 django-dbdiff-0.9.5/dbdiff/tests/project/__init__.py
--rw-r--r--   0 jpic      (1000) jpic      (1000)     2794 2018-02-12 13:29:44.000000 django-dbdiff-0.9.5/dbdiff/tests/project/settings.py
--rw-r--r--   0 jpic      (1000) jpic      (1000)      173 2018-02-09 13:02:43.000000 django-dbdiff-0.9.5/dbdiff/tests/project/settings_mysql.py
--rw-r--r--   0 jpic      (1000) jpic      (1000)      191 2018-02-06 15:07:48.000000 django-dbdiff-0.9.5/dbdiff/tests/project/settings_postgresql.py
--rw-r--r--   0 jpic      (1000) jpic      (1000)      148 2018-02-06 15:07:48.000000 django-dbdiff-0.9.5/dbdiff/tests/project/settings_sqlite.py
--rw-r--r--   0 jpic      (1000) jpic      (1000)       17 2018-02-06 15:07:48.000000 django-dbdiff-0.9.5/dbdiff/tests/project/urls.py
--rw-r--r--   0 jpic      (1000) jpic      (1000)     2811 2018-02-06 15:07:48.000000 django-dbdiff-0.9.5/dbdiff/tests/test_compare.py
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1562 2018-02-06 15:07:48.000000 django-dbdiff-0.9.5/dbdiff/tests/test_decimal.py
--rw-r--r--   0 jpic      (1000) jpic      (1000)      623 2018-02-06 15:07:48.000000 django-dbdiff-0.9.5/dbdiff/tests/test_fixture.py
--rw-r--r--   0 jpic      (1000) jpic      (1000)      715 2018-02-06 15:07:48.000000 django-dbdiff-0.9.5/dbdiff/tests/test_mixin.py
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1036 2018-02-12 14:45:21.000000 django-dbdiff-0.9.5/dbdiff/tests/test_plugin.py
--rw-r--r--   0 jpic      (1000) jpic      (1000)      407 2018-02-06 15:07:48.000000 django-dbdiff-0.9.5/dbdiff/tests/test_utils.py
--rw-r--r--   0 jpic      (1000) jpic      (1000)     3872 2018-02-06 15:07:48.000000 django-dbdiff-0.9.5/dbdiff/utils.py
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2019-01-29 04:21:29.000000 django-dbdiff-0.9.5/django_dbdiff.egg-info/
--rw-r--r--   0 jpic      (1000) jpic      (1000)     5990 2019-01-29 04:21:29.000000 django-dbdiff-0.9.5/django_dbdiff.egg-info/PKG-INFO
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1258 2019-01-29 04:21:29.000000 django-dbdiff-0.9.5/django_dbdiff.egg-info/SOURCES.txt
--rw-r--r--   0 jpic      (1000) jpic      (1000)        1 2019-01-29 04:21:29.000000 django-dbdiff-0.9.5/django_dbdiff.egg-info/dependency_links.txt
--rw-r--r--   0 jpic      (1000) jpic      (1000)       35 2019-01-29 04:21:29.000000 django-dbdiff-0.9.5/django_dbdiff.egg-info/entry_points.txt
--rw-r--r--   0 jpic      (1000) jpic      (1000)       21 2019-01-29 04:21:29.000000 django-dbdiff-0.9.5/django_dbdiff.egg-info/requires.txt
--rw-r--r--   0 jpic      (1000) jpic      (1000)        7 2019-01-29 04:21:29.000000 django-dbdiff-0.9.5/django_dbdiff.egg-info/top_level.txt
--rw-r--r--   0 jpic      (1000) jpic      (1000)       38 2019-01-29 04:21:29.000000 django-dbdiff-0.9.5/setup.cfg
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1422 2019-01-29 04:20:58.000000 django-dbdiff-0.9.5/setup.py
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2024-05-10 13:07:14.046669 django-dbdiff-0.9.6/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     5488 2024-05-10 13:07:14.046669 django-dbdiff-0.9.6/PKG-INFO
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     4248 2024-05-10 13:06:17.000000 django-dbdiff-0.9.6/README.rst
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2024-05-10 13:07:14.046669 django-dbdiff-0.9.6/dbdiff/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      117 2018-02-06 15:07:48.000000 django-dbdiff-0.9.6/dbdiff/__init__.py
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1414 2018-02-06 15:07:48.000000 django-dbdiff-0.9.6/dbdiff/apps.py
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     2251 2018-02-06 15:07:48.000000 django-dbdiff-0.9.6/dbdiff/exceptions.py
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     4523 2019-01-29 04:20:51.000000 django-dbdiff-0.9.6/dbdiff/fixture.py
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1031 2018-11-18 01:18:28.000000 django-dbdiff-0.9.6/dbdiff/plugin.py
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1791 2018-02-12 13:57:13.000000 django-dbdiff-0.9.6/dbdiff/sequence.py
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2024-05-10 13:07:14.046669 django-dbdiff-0.9.6/dbdiff/serializers/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)       53 2018-02-06 15:07:48.000000 django-dbdiff-0.9.6/dbdiff/serializers/__init__.py
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     2654 2018-02-06 15:07:48.000000 django-dbdiff-0.9.6/dbdiff/serializers/base.py
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      315 2018-02-06 15:07:48.000000 django-dbdiff-0.9.6/dbdiff/serializers/json.py
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1848 2018-02-06 17:54:31.000000 django-dbdiff-0.9.6/dbdiff/test.py
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2024-05-10 13:07:14.046669 django-dbdiff-0.9.6/dbdiff/tests/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)       35 2018-02-06 15:07:48.000000 django-dbdiff-0.9.6/dbdiff/tests/__init__.py
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2024-05-10 13:07:14.046669 django-dbdiff-0.9.6/dbdiff/tests/decimal_test/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)       52 2018-02-06 15:07:48.000000 django-dbdiff-0.9.6/dbdiff/tests/decimal_test/__init__.py
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2024-05-10 13:07:14.046669 django-dbdiff-0.9.6/dbdiff/tests/decimal_test/migrations/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      445 2024-05-10 13:06:17.000000 django-dbdiff-0.9.6/dbdiff/tests/decimal_test/migrations/0001_initial.py
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      358 2024-05-10 13:06:17.000000 django-dbdiff-0.9.6/dbdiff/tests/decimal_test/migrations/0002_auto_20160102_0914.py
+-rw-r--r--   0 jpic      (1000) jpic      (1000)        0 2018-02-06 15:07:48.000000 django-dbdiff-0.9.6/dbdiff/tests/decimal_test/migrations/__init__.py
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      131 2018-02-06 15:07:48.000000 django-dbdiff-0.9.6/dbdiff/tests/decimal_test/models.py
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2024-05-10 13:07:14.046669 django-dbdiff-0.9.6/dbdiff/tests/inheritance/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)       38 2018-02-12 14:45:46.000000 django-dbdiff-0.9.6/dbdiff/tests/inheritance/__init__.py
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      134 2018-02-12 13:29:30.000000 django-dbdiff-0.9.6/dbdiff/tests/inheritance/models.py
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2024-05-10 13:07:14.046669 django-dbdiff-0.9.6/dbdiff/tests/nonintpk/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)       54 2018-02-06 18:06:19.000000 django-dbdiff-0.9.6/dbdiff/tests/nonintpk/__init__.py
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      205 2018-02-06 17:50:00.000000 django-dbdiff-0.9.6/dbdiff/tests/nonintpk/models.py
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2024-05-10 13:07:14.046669 django-dbdiff-0.9.6/dbdiff/tests/project/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)       29 2018-02-06 15:07:48.000000 django-dbdiff-0.9.6/dbdiff/tests/project/__init__.py
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     2794 2018-02-12 13:29:44.000000 django-dbdiff-0.9.6/dbdiff/tests/project/settings.py
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      561 2024-05-10 13:06:17.000000 django-dbdiff-0.9.6/dbdiff/tests/project/settings_mysql.py
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      441 2024-05-10 13:06:17.000000 django-dbdiff-0.9.6/dbdiff/tests/project/settings_postgresql.py
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      148 2018-02-06 15:07:48.000000 django-dbdiff-0.9.6/dbdiff/tests/project/settings_sqlite.py
+-rw-r--r--   0 jpic      (1000) jpic      (1000)       17 2018-02-06 15:07:48.000000 django-dbdiff-0.9.6/dbdiff/tests/project/urls.py
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     2595 2024-05-10 13:06:17.000000 django-dbdiff-0.9.6/dbdiff/tests/test_compare.py
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1562 2018-02-06 15:07:48.000000 django-dbdiff-0.9.6/dbdiff/tests/test_decimal.py
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      623 2018-02-06 15:07:48.000000 django-dbdiff-0.9.6/dbdiff/tests/test_fixture.py
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      715 2018-02-06 15:07:48.000000 django-dbdiff-0.9.6/dbdiff/tests/test_mixin.py
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1036 2018-02-12 14:45:21.000000 django-dbdiff-0.9.6/dbdiff/tests/test_plugin.py
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      407 2018-02-06 15:07:48.000000 django-dbdiff-0.9.6/dbdiff/tests/test_utils.py
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     3895 2024-05-10 13:06:17.000000 django-dbdiff-0.9.6/dbdiff/utils.py
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2024-05-10 13:07:14.046669 django-dbdiff-0.9.6/django_dbdiff.egg-info/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     5488 2024-05-10 13:07:13.000000 django-dbdiff-0.9.6/django_dbdiff.egg-info/PKG-INFO
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1258 2024-05-10 13:07:13.000000 django-dbdiff-0.9.6/django_dbdiff.egg-info/SOURCES.txt
+-rw-r--r--   0 jpic      (1000) jpic      (1000)        1 2024-05-10 13:07:13.000000 django-dbdiff-0.9.6/django_dbdiff.egg-info/dependency_links.txt
+-rw-r--r--   0 jpic      (1000) jpic      (1000)       34 2024-05-10 13:07:13.000000 django-dbdiff-0.9.6/django_dbdiff.egg-info/entry_points.txt
+-rw-r--r--   0 jpic      (1000) jpic      (1000)       17 2024-05-10 13:07:13.000000 django-dbdiff-0.9.6/django_dbdiff.egg-info/requires.txt
+-rw-r--r--   0 jpic      (1000) jpic      (1000)        7 2024-05-10 13:07:13.000000 django-dbdiff-0.9.6/django_dbdiff.egg-info/top_level.txt
+-rw-r--r--   0 jpic      (1000) jpic      (1000)       38 2024-05-10 13:07:14.046669 django-dbdiff-0.9.6/setup.cfg
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1806 2024-05-10 13:06:45.000000 django-dbdiff-0.9.6/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `django-dbdiff-0.9.5/PKG-INFO` & `django-dbdiff-0.9.6/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,133 +1,142 @@
 Metadata-Version: 2.1
 Name: django-dbdiff
-Version: 0.9.5
+Version: 0.9.6
 Summary: Database data diffing against fixtures for testing
 Home-page: https://github.com/yourlabs/django-dbdiff
 Author: James Pic
 Author-email: jamespic@gmail.com
 License: MIT
-Description: .. image:: https://travis-ci.org/yourlabs/django-dbdiff.svg
-            :target: https://travis-ci.org/yourlabs/django-dbdiff
-        .. image:: https://codecov.io/github/yourlabs/django-dbdiff/coverage.svg?branch=master
-            :target: https://codecov.io/github/yourlabs/django-dbdiff?branch=master
-        .. image:: https://badge.fury.io/py/django-dbdiff.png
-           :target: http://badge.fury.io/py/django-dbdiff
-        
-        django-dbdiff
-        ~~~~~~~~~~~~~
-        
-        I'm pretty lazy when it comes to writing tests for existing code, however, I'm
-        even lazier when it comes to repetitive manual testing action.
-        
-        This package aims at de-duplicating the data import tests from
-        django-representatives and django-representatives-votes which is re-used in
-        django-cities-light.
-        
-        Database state assertion
-        ========================
-        
-        A nice way to test a data import script is to create a source data fixture with
-        a subset of data, ie. with only 10 cities instead of 28K or only 3 european
-        parliament representatives instead of 3600, feed the import function with that
-        and then compare the database state with a django fixture. This looks like what
-        I was used to do:
-        
-        - use such a command to create a small data extract
-          `shuf -n3 cities15000.txt > cities_light/tests/cities_test_fixture.txt`,
-        - use it against the import script on a clean database,
-        - verify the database manually, and run
-          `django-admin dumpdata --indent=4 cities_light > cities_light/tests/cities_test_expected.txt`
-        - then, make a test case that calls the import script against the fixture,
-        - write and maintain some funny (fuzzy ?) repetitive test code to ensure that
-          the database is in the expected state.
-        
-        When a bug is fixed, just add the case to the fixture and repeat the process to
-        create new expected data dumps, use coverage to ensure no case is missed.
-        
-        With django-dbdiff, I just need to maintain to initial data extract, and test
-        it with ``Fixture('appname/path/to/fixture',
-        models=[YourModelToTest]).assertNoDiff()`` in a
-        ``django.test.TransactionTestCase`` which has ``reset_sequences=True``:
-        
-        - if the fixture in question doesn't exist, it'll be automatically created on
-          with dumpdata for the concerned models on the first run, raising
-          "FixtureCreated" exception to fail the test and inform of the path of the
-          created fixture, so that it doesn't mislead the user in thinking the test
-          passed with an existing fixture,
-        - if the fixture exists, it'll run dumpdata on the models concerned and GNU
-          diff it against the fixture, if there's any output it'll be raised in the
-          "DiffFound" exception, failing the test and printing the diff.
-        
-        Usage
-        =====
-        
-        Example:
-        
-        .. code-block:: python
-        
-            from django import TransactionTestCase
-            from dbdiff.fixture import Fixture
-        
-        
-            class YourImportTest(test.TransactionTestCase):
-                reset_sequences = True
-        
-                def test_your_import(self):
-                    your_import()
-        
-                    Fixture('yourapp/tests/yourtest.json',
-                            models=[YourModel]).assertNoDiff()
-        
-        The first time, it will raise a ``FixtureCreated`` exception, and the test will
-        fail. This is to inform the user that the test didn't really run. On the next
-        run though, it will pass.
-        
-        If any difference is found between the database and the test fixture, then
-        ``diff()`` will return the diff as outputed by GNU diff.
-        
-        If you need to ignore fields globally, set the class-level variable exclude as such:
-        
-        .. code-block:: python
-        
-           Fixture.exclude = {'mrsrequest.mrsrequest': ['token']}
-        
-        Instead of deleting the fixtures manually before running the tests to
-        regenerate them, just run your tests with FIXTURE_REWRITE=1 environment
-        variable. This will overwrite the fixtures and make the tests look like it
-        passed.
-        
-        See tests and docstrings for crunchy details.
-        
-        Requirements
-        ============
-        
-        MySQL, SQLite and PostgreSQL, Python 2.7 and 3.4 are supported along with
-        Django 1.7 to 1.10 - it's always better to support django's master so that we
-        can **upgrade easily when it is released**, which is one of the selling points
-        for having 100% coverage.
-        
-        Install
-        =======
-        
-        Install ``django-dbdiff`` with pip and add ``dbdiff`` to ``INSTALLED_APPS``.
-        
-        Django model observer
-        =====================
-        
-        It is interresting to note that a related, perhaps sort-of similar app exists:
-        https://github.com/Griffosx/djmo
-        
 Keywords: django test database fixture diff
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
-Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
+Classifier: Framework :: Django
+Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
+Classifier: Framework :: Django :: 5.0
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Description-Content-Type: text/x-rst
+Requires-Dist: ijson
+Requires-Dist: json_delta
+
+.. image:: https://travis-ci.org/yourlabs/django-dbdiff.svg
+    :target: https://travis-ci.org/yourlabs/django-dbdiff
+.. image:: https://codecov.io/github/yourlabs/django-dbdiff/coverage.svg?branch=master
+    :target: https://codecov.io/github/yourlabs/django-dbdiff?branch=master
+.. image:: https://badge.fury.io/py/django-dbdiff.png
+   :target: http://badge.fury.io/py/django-dbdiff
+
+django-dbdiff
+~~~~~~~~~~~~~
+
+I'm pretty lazy when it comes to writing tests for existing code, however, I'm
+even lazier when it comes to repetitive manual testing action.
+
+This package aims at de-duplicating the data import tests from
+django-representatives and django-representatives-votes which is re-used in
+django-cities-light.
+
+Database state assertion
+========================
+
+A nice way to test a data import script is to create a source data fixture with
+a subset of data, ie. with only 10 cities instead of 28K or only 3 european
+parliament representatives instead of 3600, feed the import function with that
+and then compare the database state with a django fixture. This looks like what
+I was used to do:
+
+- use such a command to create a small data extract
+  `shuf -n3 cities15000.txt > cities_light/tests/cities_test_fixture.txt`,
+- use it against the import script on a clean database,
+- verify the database manually, and run
+  `django-admin dumpdata --indent=4 cities_light > cities_light/tests/cities_test_expected.txt`
+- then, make a test case that calls the import script against the fixture,
+- write and maintain some funny (fuzzy ?) repetitive test code to ensure that
+  the database is in the expected state.
+
+When a bug is fixed, just add the case to the fixture and repeat the process to
+create new expected data dumps, use coverage to ensure no case is missed.
+
+With django-dbdiff, I just need to maintain to initial data extract, and test
+it with ``Fixture('appname/path/to/fixture',
+models=[YourModelToTest]).assertNoDiff()`` in a
+``django.test.TransactionTestCase`` which has ``reset_sequences=True``:
+
+- if the fixture in question doesn't exist, it'll be automatically created on
+  with dumpdata for the concerned models on the first run, raising
+  "FixtureCreated" exception to fail the test and inform of the path of the
+  created fixture, so that it doesn't mislead the user in thinking the test
+  passed with an existing fixture,
+- if the fixture exists, it'll run dumpdata on the models concerned and GNU
+  diff it against the fixture, if there's any output it'll be raised in the
+  "DiffFound" exception, failing the test and printing the diff.
+
+Usage
+=====
+
+Example:
+
+.. code-block:: python
+
+    from django import TransactionTestCase
+    from dbdiff.fixture import Fixture
+
+
+    class YourImportTest(test.TransactionTestCase):
+        reset_sequences = True
+
+        def test_your_import(self):
+            your_import()
+
+            Fixture('yourapp/tests/yourtest.json',
+                    models=[YourModel]).assertNoDiff()
+
+The first time, it will raise a ``FixtureCreated`` exception, and the test will
+fail. This is to inform the user that the test didn't really run. On the next
+run though, it will pass.
+
+If any difference is found between the database and the test fixture, then
+``diff()`` will return the diff as outputed by GNU diff.
+
+If you need to ignore fields globally, set the class-level variable exclude as such:
+
+.. code-block:: python
+
+   Fixture.exclude = {'mrsrequest.mrsrequest': ['token']}
+
+Instead of deleting the fixtures manually before running the tests to
+regenerate them, just run your tests with FIXTURE_REWRITE=1 environment
+variable. This will overwrite the fixtures and make the tests look like it
+passed.
+
+See tests and docstrings for crunchy details.
+
+Requirements
+============
+
+MySQL, SQLite and PostgreSQL, Python 3.8 to 3.12 are supported along with
+Django 3.2 to 5.0 - it's always better to support django's master so that we
+can **upgrade easily when it is released**, which is one of the selling points
+for having 100% coverage.
+
+Install
+=======
+
+Install ``django-dbdiff`` with pip and add ``dbdiff`` to ``INSTALLED_APPS``.
+
+Django model observer
+=====================
+
+It is interresting to note that a related, perhaps sort-of similar app exists:
+https://github.com/Griffosx/djmo
```

### Comparing `django-dbdiff-0.9.5/README.rst` & `django-dbdiff-0.9.6/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -89,16 +89,16 @@
 passed.
 
 See tests and docstrings for crunchy details.
 
 Requirements
 ============
 
-MySQL, SQLite and PostgreSQL, Python 2.7 and 3.4 are supported along with
-Django 1.7 to 1.10 - it's always better to support django's master so that we
+MySQL, SQLite and PostgreSQL, Python 3.8 to 3.12 are supported along with
+Django 3.2 to 5.0 - it's always better to support django's master so that we
 can **upgrade easily when it is released**, which is one of the selling points
 for having 100% coverage.
 
 Install
 =======
 
 Install ``django-dbdiff`` with pip and add ``dbdiff`` to ``INSTALLED_APPS``.
```

### Comparing `django-dbdiff-0.9.5/dbdiff/apps.py` & `django-dbdiff-0.9.6/dbdiff/apps.py`

 * *Files identical despite different names*

### Comparing `django-dbdiff-0.9.5/dbdiff/exceptions.py` & `django-dbdiff-0.9.6/dbdiff/exceptions.py`

 * *Files identical despite different names*

### Comparing `django-dbdiff-0.9.5/dbdiff/fixture.py` & `django-dbdiff-0.9.6/dbdiff/fixture.py`

 * *Files identical despite different names*

### Comparing `django-dbdiff-0.9.5/dbdiff/plugin.py` & `django-dbdiff-0.9.6/dbdiff/plugin.py`

 * *Files identical despite different names*

### Comparing `django-dbdiff-0.9.5/dbdiff/sequence.py` & `django-dbdiff-0.9.6/dbdiff/sequence.py`

 * *Files identical despite different names*

### Comparing `django-dbdiff-0.9.5/dbdiff/serializers/base.py` & `django-dbdiff-0.9.6/dbdiff/serializers/base.py`

 * *Files identical despite different names*

### Comparing `django-dbdiff-0.9.5/dbdiff/test.py` & `django-dbdiff-0.9.6/dbdiff/test.py`

 * *Files identical despite different names*

### Comparing `django-dbdiff-0.9.5/dbdiff/tests/project/settings.py` & `django-dbdiff-0.9.6/dbdiff/tests/project/settings.py`

 * *Files identical despite different names*

### Comparing `django-dbdiff-0.9.5/dbdiff/tests/test_compare.py` & `django-dbdiff-0.9.6/dbdiff/tests/test_compare.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,15 @@
 """Public API tests."""
 
-from __future__ import unicode_literals
-
 import os
 import tempfile
 
 from django import test
 from django.contrib.auth.models import Group
 
-import six
-
 from ..exceptions import DiffFound, FixtureCreated
 from ..fixture import Fixture
 
 
 class SmokeTest(test.TransactionTestCase):
     def setUp(self):
         fd, self.fixture_path = tempfile.mkstemp(suffix='_dbdiff')
@@ -53,61 +49,54 @@
 
         # It should break now !
         Group.objects.all().update(name='BOOM')
         expected = '''
 1 instance(s) of auth.group have not expected fields
 #1:
   name:
-- u'testgroup'
-+ u'BOOM'
+- 'testgroup'
++ 'BOOM'
 '''
 
         with self.assertRaises(DiffFound) as result:
             fixture.assertNoDiff()
         self.assert_message_is(expected, result)
 
         # Excluding the name parameter, there should be no diff
         fixture.assertNoDiff(exclude={'auth.group': ['name']})
 
         # Assert it finds unexpected model
         Group.objects.create(name='unexpected')
         expected = '''
 1 unexpected instance(s) of auth.group found in the dump:
 #2:
-{u'name': u'unexpected', u'permissions': []}
+{'name': 'unexpected', 'permissions': []}
 1 instance(s) of auth.group have not expected fields
 #1:
   name:
-- u'testgroup'
-+ u'BOOM'
+- 'testgroup'
++ 'BOOM'
 '''
 
         with self.assertRaises(DiffFound) as result:
             fixture.assertNoDiff()
         self.assert_message_is(expected, result)
 
         # Assert it finds missing model
         Group.objects.get(pk=1).delete()
         expected = '''
 1 unexpected instance(s) of auth.group found in the dump:
 #2:
-{u'name': u'unexpected', u'permissions': []}
+{'name': 'unexpected', 'permissions': []}
 1 expected instance(s) of auth.group missing from dump:
 #1:
-{u'name': u'testgroup', u'permissions': []}
+{'name': 'testgroup', 'permissions': []}
 '''
 
         with self.assertRaises(DiffFound) as result:
             fixture.assertNoDiff()
         self.assert_message_is(expected, result)
 
     def assert_message_is(self, expected, result):
-        if six.PY3:
-            expected = expected.replace("u'", "'")
-
-        msg = (
-            result.exception.message
-            if six.PY2 else result.exception.args[0]
-        )
-
+        msg = result.exception.args[0]
         out = '\n'.join(msg.split('\n')[1:])
         assert out.strip() == expected.strip()
```

### Comparing `django-dbdiff-0.9.5/dbdiff/tests/test_decimal.py` & `django-dbdiff-0.9.6/dbdiff/tests/test_decimal.py`

 * *Files identical despite different names*

### Comparing `django-dbdiff-0.9.5/dbdiff/tests/test_fixture.py` & `django-dbdiff-0.9.6/dbdiff/tests/test_fixture.py`

 * *Files identical despite different names*

### Comparing `django-dbdiff-0.9.5/dbdiff/tests/test_mixin.py` & `django-dbdiff-0.9.6/dbdiff/tests/test_mixin.py`

 * *Files identical despite different names*

### Comparing `django-dbdiff-0.9.5/dbdiff/tests/test_plugin.py` & `django-dbdiff-0.9.6/dbdiff/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `django-dbdiff-0.9.5/dbdiff/utils.py` & `django-dbdiff-0.9.6/dbdiff/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 """Utils for dbdiff."""
 
-import imp
 import os
 
 from django.apps import apps
 from django.db import connections
 
-import six
-
+from importlib.util import find_spec
 
 def get_tree(dump, exclude=None):
     """Return a tree of model -> pk -> fields."""
     exclude = exclude or {}
     tree = {}
 
     for instance in dump:
@@ -82,25 +80,26 @@
     """Return the absolute path to an app-relative path."""
     if path.startswith('/'):
         return path
 
     if path.startswith('.'):
         module_path = '.'
     else:
-        module_path = imp.find_module(path.split('/')[0])[1]
+        module_path = find_spec(path.split('/')[0]).submodule_search_locations[0]
+
     return os.path.abspath(os.path.join(
         module_path,
         *path.split('/')[1:]
     ))
 
 
 def get_model_names(model_classes):
     """Return model names for model classes."""
     return [
-        m if isinstance(m, six.string_types)
+        m if isinstance(m, str)
         else '%s.%s' % (m._meta.app_label, m._meta.model_name)
         for m in model_classes
     ]
 
 
 def get_models_tables(models):
     """Return the list of tables for the given models."""
```

### Comparing `django-dbdiff-0.9.5/django_dbdiff.egg-info/PKG-INFO` & `django-dbdiff-0.9.6/django_dbdiff.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,133 +1,142 @@
 Metadata-Version: 2.1
 Name: django-dbdiff
-Version: 0.9.5
+Version: 0.9.6
 Summary: Database data diffing against fixtures for testing
 Home-page: https://github.com/yourlabs/django-dbdiff
 Author: James Pic
 Author-email: jamespic@gmail.com
 License: MIT
-Description: .. image:: https://travis-ci.org/yourlabs/django-dbdiff.svg
-            :target: https://travis-ci.org/yourlabs/django-dbdiff
-        .. image:: https://codecov.io/github/yourlabs/django-dbdiff/coverage.svg?branch=master
-            :target: https://codecov.io/github/yourlabs/django-dbdiff?branch=master
-        .. image:: https://badge.fury.io/py/django-dbdiff.png
-           :target: http://badge.fury.io/py/django-dbdiff
-        
-        django-dbdiff
-        ~~~~~~~~~~~~~
-        
-        I'm pretty lazy when it comes to writing tests for existing code, however, I'm
-        even lazier when it comes to repetitive manual testing action.
-        
-        This package aims at de-duplicating the data import tests from
-        django-representatives and django-representatives-votes which is re-used in
-        django-cities-light.
-        
-        Database state assertion
-        ========================
-        
-        A nice way to test a data import script is to create a source data fixture with
-        a subset of data, ie. with only 10 cities instead of 28K or only 3 european
-        parliament representatives instead of 3600, feed the import function with that
-        and then compare the database state with a django fixture. This looks like what
-        I was used to do:
-        
-        - use such a command to create a small data extract
-          `shuf -n3 cities15000.txt > cities_light/tests/cities_test_fixture.txt`,
-        - use it against the import script on a clean database,
-        - verify the database manually, and run
-          `django-admin dumpdata --indent=4 cities_light > cities_light/tests/cities_test_expected.txt`
-        - then, make a test case that calls the import script against the fixture,
-        - write and maintain some funny (fuzzy ?) repetitive test code to ensure that
-          the database is in the expected state.
-        
-        When a bug is fixed, just add the case to the fixture and repeat the process to
-        create new expected data dumps, use coverage to ensure no case is missed.
-        
-        With django-dbdiff, I just need to maintain to initial data extract, and test
-        it with ``Fixture('appname/path/to/fixture',
-        models=[YourModelToTest]).assertNoDiff()`` in a
-        ``django.test.TransactionTestCase`` which has ``reset_sequences=True``:
-        
-        - if the fixture in question doesn't exist, it'll be automatically created on
-          with dumpdata for the concerned models on the first run, raising
-          "FixtureCreated" exception to fail the test and inform of the path of the
-          created fixture, so that it doesn't mislead the user in thinking the test
-          passed with an existing fixture,
-        - if the fixture exists, it'll run dumpdata on the models concerned and GNU
-          diff it against the fixture, if there's any output it'll be raised in the
-          "DiffFound" exception, failing the test and printing the diff.
-        
-        Usage
-        =====
-        
-        Example:
-        
-        .. code-block:: python
-        
-            from django import TransactionTestCase
-            from dbdiff.fixture import Fixture
-        
-        
-            class YourImportTest(test.TransactionTestCase):
-                reset_sequences = True
-        
-                def test_your_import(self):
-                    your_import()
-        
-                    Fixture('yourapp/tests/yourtest.json',
-                            models=[YourModel]).assertNoDiff()
-        
-        The first time, it will raise a ``FixtureCreated`` exception, and the test will
-        fail. This is to inform the user that the test didn't really run. On the next
-        run though, it will pass.
-        
-        If any difference is found between the database and the test fixture, then
-        ``diff()`` will return the diff as outputed by GNU diff.
-        
-        If you need to ignore fields globally, set the class-level variable exclude as such:
-        
-        .. code-block:: python
-        
-           Fixture.exclude = {'mrsrequest.mrsrequest': ['token']}
-        
-        Instead of deleting the fixtures manually before running the tests to
-        regenerate them, just run your tests with FIXTURE_REWRITE=1 environment
-        variable. This will overwrite the fixtures and make the tests look like it
-        passed.
-        
-        See tests and docstrings for crunchy details.
-        
-        Requirements
-        ============
-        
-        MySQL, SQLite and PostgreSQL, Python 2.7 and 3.4 are supported along with
-        Django 1.7 to 1.10 - it's always better to support django's master so that we
-        can **upgrade easily when it is released**, which is one of the selling points
-        for having 100% coverage.
-        
-        Install
-        =======
-        
-        Install ``django-dbdiff`` with pip and add ``dbdiff`` to ``INSTALLED_APPS``.
-        
-        Django model observer
-        =====================
-        
-        It is interresting to note that a related, perhaps sort-of similar app exists:
-        https://github.com/Griffosx/djmo
-        
 Keywords: django test database fixture diff
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
-Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
+Classifier: Framework :: Django
+Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
+Classifier: Framework :: Django :: 5.0
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Description-Content-Type: text/x-rst
+Requires-Dist: ijson
+Requires-Dist: json_delta
+
+.. image:: https://travis-ci.org/yourlabs/django-dbdiff.svg
+    :target: https://travis-ci.org/yourlabs/django-dbdiff
+.. image:: https://codecov.io/github/yourlabs/django-dbdiff/coverage.svg?branch=master
+    :target: https://codecov.io/github/yourlabs/django-dbdiff?branch=master
+.. image:: https://badge.fury.io/py/django-dbdiff.png
+   :target: http://badge.fury.io/py/django-dbdiff
+
+django-dbdiff
+~~~~~~~~~~~~~
+
+I'm pretty lazy when it comes to writing tests for existing code, however, I'm
+even lazier when it comes to repetitive manual testing action.
+
+This package aims at de-duplicating the data import tests from
+django-representatives and django-representatives-votes which is re-used in
+django-cities-light.
+
+Database state assertion
+========================
+
+A nice way to test a data import script is to create a source data fixture with
+a subset of data, ie. with only 10 cities instead of 28K or only 3 european
+parliament representatives instead of 3600, feed the import function with that
+and then compare the database state with a django fixture. This looks like what
+I was used to do:
+
+- use such a command to create a small data extract
+  `shuf -n3 cities15000.txt > cities_light/tests/cities_test_fixture.txt`,
+- use it against the import script on a clean database,
+- verify the database manually, and run
+  `django-admin dumpdata --indent=4 cities_light > cities_light/tests/cities_test_expected.txt`
+- then, make a test case that calls the import script against the fixture,
+- write and maintain some funny (fuzzy ?) repetitive test code to ensure that
+  the database is in the expected state.
+
+When a bug is fixed, just add the case to the fixture and repeat the process to
+create new expected data dumps, use coverage to ensure no case is missed.
+
+With django-dbdiff, I just need to maintain to initial data extract, and test
+it with ``Fixture('appname/path/to/fixture',
+models=[YourModelToTest]).assertNoDiff()`` in a
+``django.test.TransactionTestCase`` which has ``reset_sequences=True``:
+
+- if the fixture in question doesn't exist, it'll be automatically created on
+  with dumpdata for the concerned models on the first run, raising
+  "FixtureCreated" exception to fail the test and inform of the path of the
+  created fixture, so that it doesn't mislead the user in thinking the test
+  passed with an existing fixture,
+- if the fixture exists, it'll run dumpdata on the models concerned and GNU
+  diff it against the fixture, if there's any output it'll be raised in the
+  "DiffFound" exception, failing the test and printing the diff.
+
+Usage
+=====
+
+Example:
+
+.. code-block:: python
+
+    from django import TransactionTestCase
+    from dbdiff.fixture import Fixture
+
+
+    class YourImportTest(test.TransactionTestCase):
+        reset_sequences = True
+
+        def test_your_import(self):
+            your_import()
+
+            Fixture('yourapp/tests/yourtest.json',
+                    models=[YourModel]).assertNoDiff()
+
+The first time, it will raise a ``FixtureCreated`` exception, and the test will
+fail. This is to inform the user that the test didn't really run. On the next
+run though, it will pass.
+
+If any difference is found between the database and the test fixture, then
+``diff()`` will return the diff as outputed by GNU diff.
+
+If you need to ignore fields globally, set the class-level variable exclude as such:
+
+.. code-block:: python
+
+   Fixture.exclude = {'mrsrequest.mrsrequest': ['token']}
+
+Instead of deleting the fixtures manually before running the tests to
+regenerate them, just run your tests with FIXTURE_REWRITE=1 environment
+variable. This will overwrite the fixtures and make the tests look like it
+passed.
+
+See tests and docstrings for crunchy details.
+
+Requirements
+============
+
+MySQL, SQLite and PostgreSQL, Python 3.8 to 3.12 are supported along with
+Django 3.2 to 5.0 - it's always better to support django's master so that we
+can **upgrade easily when it is released**, which is one of the selling points
+for having 100% coverage.
+
+Install
+=======
+
+Install ``django-dbdiff`` with pip and add ``dbdiff`` to ``INSTALLED_APPS``.
+
+Django model observer
+=====================
+
+It is interresting to note that a related, perhaps sort-of similar app exists:
+https://github.com/Griffosx/djmo
```

### Comparing `django-dbdiff-0.9.5/django_dbdiff.egg-info/SOURCES.txt` & `django-dbdiff-0.9.6/django_dbdiff.egg-info/SOURCES.txt`

 * *Files identical despite different names*

