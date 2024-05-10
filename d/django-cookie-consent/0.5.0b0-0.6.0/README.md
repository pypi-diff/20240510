# Comparing `tmp/django-cookie-consent-0.5.0b0.tar.gz` & `tmp/django_cookie_consent-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-cookie-consent-0.5.0b0.tar", last modified: Sun Sep 24 14:27:38 2023, max compression
+gzip compressed data, was "django_cookie_consent-0.6.0.tar", last modified: Fri May 10 08:34:40 2024, max compression
```

## Comparing `django-cookie-consent-0.5.0b0.tar` & `django_cookie_consent-0.6.0.tar`

### file list

```diff
@@ -1,55 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-24 14:27:38.197833 django-cookie-consent-0.5.0b0/
--rw-r--r--   0 runner    (1001) docker     (127)      323 2023-09-24 14:27:27.000000 django-cookie-consent-0.5.0b0/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2023-09-24 14:27:27.000000 django-cookie-consent-0.5.0b0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      181 2023-09-24 14:27:27.000000 django-cookie-consent-0.5.0b0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4646 2023-09-24 14:27:38.197833 django-cookie-consent-0.5.0b0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2466 2023-09-24 14:27:27.000000 django-cookie-consent-0.5.0b0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-24 14:27:38.193833 django-cookie-consent-0.5.0b0/cookie_consent/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2023-09-24 14:27:27.000000 django-cookie-consent-0.5.0b0/cookie_consent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2023-09-24 14:27:27.000000 django-cookie-consent-0.5.0b0/cookie_consent/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      248 2023-09-24 14:27:27.000000 django-cookie-consent-0.5.0b0/cookie_consent/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     1446 2023-09-24 14:27:27.000000 django-cookie-consent-0.5.0b0/cookie_consent/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)      464 2023-09-24 14:27:27.000000 django-cookie-consent-0.5.0b0/cookie_consent/compat.py
--rw-r--r--   0 runner    (1001) docker     (127)      555 2023-09-24 14:27:27.000000 django-cookie-consent-0.5.0b0/cookie_consent/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-24 14:27:38.193833 django-cookie-consent-0.5.0b0/cookie_consent/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)     2449 2023-09-24 14:27:27.000000 django-cookie-consent-0.5.0b0/cookie_consent/fixtures/common_cookies.json
--rw-r--r--   0 runner    (1001) docker     (127)     1981 2023-09-24 14:27:27.000000 django-cookie-consent-0.5.0b0/cookie_consent/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-24 14:27:38.193833 django-cookie-consent-0.5.0b0/cookie_consent/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     4180 2023-09-24 14:27:27.000000 django-cookie-consent-0.5.0b0/cookie_consent/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)     1633 2023-09-24 14:27:27.000000 django-cookie-consent-0.5.0b0/cookie_consent/migrations/0002_auto__add_logitem.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-24 14:27:27.000000 django-cookie-consent-0.5.0b0/cookie_consent/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4242 2023-09-24 14:27:27.000000 django-cookie-consent-0.5.0b0/cookie_consent/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-24 14:27:38.189833 django-cookie-consent-0.5.0b0/cookie_consent/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-24 14:27:38.193833 django-cookie-consent-0.5.0b0/cookie_consent/static/cookie_consent/
--rw-r--r--   0 runner    (1001) docker     (127)     1919 2023-09-24 14:27:27.000000 django-cookie-consent-0.5.0b0/cookie_consent/static/cookie_consent/cookiebar.js
--rw-r--r--   0 runner    (1001) docker     (127)     7371 2023-09-24 14:27:27.000000 django-cookie-consent-0.5.0b0/cookie_consent/static/cookie_consent/cookiebar.module.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-24 14:27:38.189833 django-cookie-consent-0.5.0b0/cookie_consent/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-24 14:27:38.193833 django-cookie-consent-0.5.0b0/cookie_consent/templates/cookie_consent/
--rw-r--r--   0 runner    (1001) docker     (127)     1496 2023-09-24 14:27:27.000000 django-cookie-consent-0.5.0b0/cookie_consent/templates/cookie_consent/_cookie_group.html
--rw-r--r--   0 runner    (1001) docker     (127)       85 2023-09-24 14:27:27.000000 django-cookie-consent-0.5.0b0/cookie_consent/templates/cookie_consent/base.html
--rw-r--r--   0 runner    (1001) docker     (127)      308 2023-09-24 14:27:27.000000 django-cookie-consent-0.5.0b0/cookie_consent/templates/cookie_consent/cookiegroup_list.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-24 14:27:38.193833 django-cookie-consent-0.5.0b0/cookie_consent/templatetags/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2023-09-24 14:27:27.000000 django-cookie-consent-0.5.0b0/cookie_consent/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5175 2023-09-24 14:27:27.000000 django-cookie-consent-0.5.0b0/cookie_consent/templatetags/cookie_consent_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2023-09-24 14:27:27.000000 django-cookie-consent-0.5.0b0/cookie_consent/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     5948 2023-09-24 14:27:27.000000 django-cookie-consent-0.5.0b0/cookie_consent/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     4126 2023-09-24 14:27:27.000000 django-cookie-consent-0.5.0b0/cookie_consent/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-24 14:27:38.193833 django-cookie-consent-0.5.0b0/django_cookie_consent.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4646 2023-09-24 14:27:38.000000 django-cookie-consent-0.5.0b0/django_cookie_consent.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1371 2023-09-24 14:27:38.000000 django-cookie-consent-0.5.0b0/django_cookie_consent.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-24 14:27:38.000000 django-cookie-consent-0.5.0b0/django_cookie_consent.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-24 14:27:38.000000 django-cookie-consent-0.5.0b0/django_cookie_consent.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      191 2023-09-24 14:27:38.000000 django-cookie-consent-0.5.0b0/django_cookie_consent.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2023-09-24 14:27:38.000000 django-cookie-consent-0.5.0b0/django_cookie_consent.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2528 2023-09-24 14:27:38.197833 django-cookie-consent-0.5.0b0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-24 14:27:27.000000 django-cookie-consent-0.5.0b0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-24 14:27:38.193833 django-cookie-consent-0.5.0b0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2133 2023-09-24 14:27:27.000000 django-cookie-consent-0.5.0b0/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     2350 2023-09-24 14:27:27.000000 django-cookie-consent-0.5.0b0/tests/test_javascript_cookiebar.py
--rw-r--r--   0 runner    (1001) docker     (127)     2354 2023-09-24 14:27:27.000000 django-cookie-consent-0.5.0b0/tests/test_legacy_javascript_cookiebar.py
--rw-r--r--   0 runner    (1001) docker     (127)     4234 2023-09-24 14:27:27.000000 django-cookie-consent-0.5.0b0/tests/test_middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)     1575 2023-09-24 14:27:27.000000 django-cookie-consent-0.5.0b0/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1212 2023-09-24 14:27:27.000000 django-cookie-consent-0.5.0b0/tests/test_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2023-09-24 14:27:27.000000 django-cookie-consent-0.5.0b0/tests/test_templatetags.py
--rw-r--r--   0 runner    (1001) docker     (127)     4743 2023-09-24 14:27:27.000000 django-cookie-consent-0.5.0b0/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     5729 2023-09-24 14:27:27.000000 django-cookie-consent-0.5.0b0/tests/test_views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:34:40.315209 django_cookie_consent-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-10 08:34:22.000000 django_cookie_consent-0.6.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-10 08:34:22.000000 django_cookie_consent-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-10 08:34:22.000000 django_cookie_consent-0.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6041 2024-05-10 08:34:40.315209 django_cookie_consent-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-05-10 08:34:22.000000 django_cookie_consent-0.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:34:40.307209 django_cookie_consent-0.6.0/cookie_consent/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-10 08:34:22.000000 django_cookie_consent-0.6.0/cookie_consent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-05-10 08:34:22.000000 django_cookie_consent-0.6.0/cookie_consent/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-10 08:34:22.000000 django_cookie_consent-0.6.0/cookie_consent/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-05-10 08:34:22.000000 django_cookie_consent-0.6.0/cookie_consent/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-10 08:34:22.000000 django_cookie_consent-0.6.0/cookie_consent/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:34:40.307209 django_cookie_consent-0.6.0/cookie_consent/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-05-10 08:34:22.000000 django_cookie_consent-0.6.0/cookie_consent/fixtures/common_cookies.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-05-10 08:34:22.000000 django_cookie_consent-0.6.0/cookie_consent/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:34:40.307209 django_cookie_consent-0.6.0/cookie_consent/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     4180 2024-05-10 08:34:22.000000 django_cookie_consent-0.6.0/cookie_consent/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-05-10 08:34:22.000000 django_cookie_consent-0.6.0/cookie_consent/migrations/0002_auto__add_logitem.py
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2024-05-10 08:34:22.000000 django_cookie_consent-0.6.0/cookie_consent/migrations/0003_alter_cookiegroup_varname.py
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-05-10 08:34:22.000000 django_cookie_consent-0.6.0/cookie_consent/migrations/0004_cookie_natural_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 08:34:22.000000 django_cookie_consent-0.6.0/cookie_consent/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5520 2024-05-10 08:34:22.000000 django_cookie_consent-0.6.0/cookie_consent/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:34:40.303209 django_cookie_consent-0.6.0/cookie_consent/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:34:40.311210 django_cookie_consent-0.6.0/cookie_consent/static/cookie_consent/
+-rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-05-10 08:34:22.000000 django_cookie_consent-0.6.0/cookie_consent/static/cookie_consent/cookiebar.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5625 2024-05-10 08:34:38.000000 django_cookie_consent-0.6.0/cookie_consent/static/cookie_consent/cookiebar.module.js
+-rw-r--r--   0 runner    (1001) docker     (127)    14288 2024-05-10 08:34:38.000000 django_cookie_consent-0.6.0/cookie_consent/static/cookie_consent/cookiebar.module.js.map
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:34:40.303209 django_cookie_consent-0.6.0/cookie_consent/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:34:40.311210 django_cookie_consent-0.6.0/cookie_consent/templates/cookie_consent/
+-rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-05-10 08:34:22.000000 django_cookie_consent-0.6.0/cookie_consent/templates/cookie_consent/_cookie_group.html
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-10 08:34:22.000000 django_cookie_consent-0.6.0/cookie_consent/templates/cookie_consent/base.html
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-10 08:34:22.000000 django_cookie_consent-0.6.0/cookie_consent/templates/cookie_consent/cookiegroup_list.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:34:40.311210 django_cookie_consent-0.6.0/cookie_consent/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-10 08:34:22.000000 django_cookie_consent-0.6.0/cookie_consent/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5175 2024-05-10 08:34:22.000000 django_cookie_consent-0.6.0/cookie_consent/templatetags/cookie_consent_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-10 08:34:22.000000 django_cookie_consent-0.6.0/cookie_consent/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5948 2024-05-10 08:34:22.000000 django_cookie_consent-0.6.0/cookie_consent/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4173 2024-05-10 08:34:22.000000 django_cookie_consent-0.6.0/cookie_consent/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:34:40.315209 django_cookie_consent-0.6.0/django_cookie_consent.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6041 2024-05-10 08:34:40.000000 django_cookie_consent-0.6.0/django_cookie_consent.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-05-10 08:34:40.000000 django_cookie_consent-0.6.0/django_cookie_consent.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 08:34:40.000000 django_cookie_consent-0.6.0/django_cookie_consent.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-10 08:34:40.000000 django_cookie_consent-0.6.0/django_cookie_consent.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-10 08:34:40.000000 django_cookie_consent-0.6.0/django_cookie_consent.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-05-10 08:34:22.000000 django_cookie_consent-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-10 08:34:40.315209 django_cookie_consent-0.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:34:40.315209 django_cookie_consent-0.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-05-10 08:34:22.000000 django_cookie_consent-0.6.0/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-10 08:34:22.000000 django_cookie_consent-0.6.0/tests/test_cookie_group_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-05-10 08:34:22.000000 django_cookie_consent-0.6.0/tests/test_cookie_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2695 2024-05-10 08:34:22.000000 django_cookie_consent-0.6.0/tests/test_javascript_cookiebar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-05-10 08:34:22.000000 django_cookie_consent-0.6.0/tests/test_legacy_javascript_cookiebar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4234 2024-05-10 08:34:22.000000 django_cookie_consent-0.6.0/tests/test_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3415 2024-05-10 08:34:22.000000 django_cookie_consent-0.6.0/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-05-10 08:34:22.000000 django_cookie_consent-0.6.0/tests/test_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-10 08:34:22.000000 django_cookie_consent-0.6.0/tests/test_templatetags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4743 2024-05-10 08:34:22.000000 django_cookie_consent-0.6.0/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5729 2024-05-10 08:34:22.000000 django_cookie_consent-0.6.0/tests/test_views.py
```

### Comparing `django-cookie-consent-0.5.0b0/LICENSE` & `django_cookie_consent-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-cookie-consent-0.5.0b0/PKG-INFO` & `django_cookie_consent-0.6.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,59 +1,78 @@
 Metadata-Version: 2.1
 Name: django-cookie-consent
-Version: 0.5.0b0
+Version: 0.6.0
 Summary: Django cookie consent application
-Home-page: https://github.com/jazzband/django-cookie-consent
-Author: Informatika Mihelac
-Author-email: bmihelac@mihelac.org
-License: BSD
+Author-email: Informatika Mihelac <bmihelac@mihelac.org>
+License: Copyright (c) Bojan Mihelac and individual contributors.
+        All rights reserved.
+        
+        Redistribution and use in source and binary forms, with or without modification,
+        are permitted provided that the following conditions are met:
+        
+            1. Redistributions of source code must retain the above copyright notice, 
+               this list of conditions and the following disclaimer.
+            
+            2. Redistributions in binary form must reproduce the above copyright 
+               notice, this list of conditions and the following disclaimer in the
+               documentation and/or other materials provided with the distribution.
+        
+        THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND
+        ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
+        WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+        DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT OWNER OR CONTRIBUTORS BE LIABLE FOR
+        ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
+        (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
+        LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON
+        ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
+        (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
+        SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+        
 Project-URL: Documentation, https://django-cookie-consent.readthedocs.io/en/latest/
 Project-URL: Changelog, https://github.com/jazzband/django-cookie-consent/blob/master/docs/changelog.rst
 Project-URL: Bug Tracker, https://github.com/jazzband/django-cookie-consent/issues
 Project-URL: Source Code, https://github.com/jazzband/django-cookie-consent
 Keywords: cookies,cookie-consent,cookie bar
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.1
 Classifier: Framework :: Django :: 4.2
+Classifier: Framework :: Django :: 5.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS
-Requires-Dist: django>=3.2
+Requires-Dist: django>=4.2
 Requires-Dist: django-appconf
 Provides-Extra: tests
 Requires-Dist: pytest; extra == "tests"
 Requires-Dist: pytest-django; extra == "tests"
 Requires-Dist: pytest-playwright; extra == "tests"
 Requires-Dist: tox; extra == "tests"
 Requires-Dist: isort; extra == "tests"
 Requires-Dist: black; extra == "tests"
 Requires-Dist: flake8; extra == "tests"
-Provides-Extra: pep8
-Requires-Dist: flake8; extra == "pep8"
 Provides-Extra: coverage
 Requires-Dist: pytest-cov; extra == "coverage"
 Provides-Extra: docs
 Requires-Dist: sphinx; extra == "docs"
 Requires-Dist: sphinx-rtd-theme; extra == "docs"
 Provides-Extra: release
 Requires-Dist: tbump; extra == "release"
-Requires-Dist: twine; extra == "release"
 
 Django cookie consent
 =====================
 
 Manage cookie information and let visitors give or reject consent for them.
 
 [![Jazzband][badge:jazzband]][jazzband]
```

### Comparing `django-cookie-consent-0.5.0b0/README.md` & `django_cookie_consent-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `django-cookie-consent-0.5.0b0/cookie_consent/admin.py` & `django_cookie_consent-0.6.0/cookie_consent/admin.py`

 * *Files identical despite different names*

### Comparing `django-cookie-consent-0.5.0b0/cookie_consent/cache.py` & `django_cookie_consent-0.6.0/cookie_consent/cache.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # -*- coding: utf-8 -*-
 from django.core.cache import caches
 
-from cookie_consent.conf import settings
+from .conf import settings
+from .models import CookieGroup
 
 CACHE_KEY = "cookie_consent_cache"
-CACHE_TIMEOUT = 60 * 60
+CACHE_TIMEOUT = 60 * 60  # 60 minutes
 
 
 def _get_cache():
     """
     Lazily wrap around django.core.cache.
 
     This prevents the cache object to be resolved at import-time, which breaks the
@@ -19,28 +20,30 @@
 
 
 def delete_cache():
     cache = _get_cache()
     cache.delete(CACHE_KEY)
 
 
+def _get_cookie_groups_from_db():
+    qs = CookieGroup.objects.filter(is_required=False).prefetch_related("cookie_set")
+    return qs.in_bulk(field_name="varname")
+
+
 def all_cookie_groups():
+    """
+    Get all cookie groups that are optional.
+
+    Reads from the cache where possible, sets the value in the cache if there's a
+    cache miss.
+    """
     cache = _get_cache()
-    items = cache.get(CACHE_KEY)
-    if items is None:
-        from cookie_consent.models import CookieGroup
-
-        qs = CookieGroup.objects.filter(is_required=False)
-        qs = qs.prefetch_related("cookie_set")
-        # items = qs.in_bulk(field_name="varname")
-        # FIXME -> doesn't work because varname is not a unique fieldl, we need to
-        # make this unique
-        items = {group.varname: group for group in qs}
-        cache.set(CACHE_KEY, items, CACHE_TIMEOUT)
-    return items
+    return cache.get_or_set(
+        CACHE_KEY, _get_cookie_groups_from_db, timeout=CACHE_TIMEOUT
+    )
 
 
 def get_cookie_group(varname):
     return all_cookie_groups().get(varname)
 
 
 def get_cookie(cookie_group, name, domain):
```

### Comparing `django-cookie-consent-0.5.0b0/cookie_consent/conf.py` & `django_cookie_consent-0.6.0/cookie_consent/conf.py`

 * *Files identical despite different names*

### Comparing `django-cookie-consent-0.5.0b0/cookie_consent/fixtures/common_cookies.json` & `django_cookie_consent-0.6.0/cookie_consent/fixtures/common_cookies.json`

 * *Files identical despite different names*

### Comparing `django-cookie-consent-0.5.0b0/cookie_consent/middleware.py` & `django_cookie_consent-0.6.0/cookie_consent/middleware.py`

 * *Files identical despite different names*

### Comparing `django-cookie-consent-0.5.0b0/cookie_consent/migrations/0001_initial.py` & `django_cookie_consent-0.6.0/cookie_consent/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-cookie-consent-0.5.0b0/cookie_consent/migrations/0002_auto__add_logitem.py` & `django_cookie_consent-0.6.0/cookie_consent/migrations/0002_auto__add_logitem.py`

 * *Files identical despite different names*

### Comparing `django-cookie-consent-0.5.0b0/cookie_consent/models.py` & `django_cookie_consent-0.6.0/cookie_consent/models.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,40 +2,67 @@
 import re
 from typing import TypedDict
 
 from django.core.validators import RegexValidator
 from django.db import models
 from django.utils.translation import gettext_lazy as _
 
-from cookie_consent.cache import delete_cache
-
 COOKIE_NAME_RE = re.compile(r"^[-_a-zA-Z0-9]+$")
 validate_cookie_name = RegexValidator(
     COOKIE_NAME_RE,
     _(
         "Enter a valid 'varname' consisting of letters, numbers"
         ", underscores or hyphens."
     ),
     "invalid",
 )
 
 
+def clear_cache_after(func):
+    def wrapper(*args, **kwargs):
+        from .cache import delete_cache
+
+        return_value = func(*args, **kwargs)
+        delete_cache()
+        return return_value
+
+    return wrapper
+
+
 class CookieGroupDict(TypedDict):
     varname: str
     name: str
     description: str
     is_required: bool
     # TODO: should we output this? page cache busting would be
     # required if we do this. Alternatively, set up a JSONView to output these?
     # version: str
 
 
+class BaseQueryset(models.query.QuerySet):
+    @clear_cache_after
+    def delete(self):
+        return super().delete()
+
+    @clear_cache_after
+    def update(self, **kwargs):
+        return super().update(**kwargs)
+
+
+class CookieGroupManager(models.Manager.from_queryset(BaseQueryset)):
+    def get_by_natural_key(self, varname):
+        return self.get(varname=varname)
+
+
 class CookieGroup(models.Model):
     varname = models.CharField(
-        _("Variable name"), max_length=32, validators=[validate_cookie_name]
+        _("Variable name"),
+        max_length=32,
+        unique=True,
+        validators=[validate_cookie_name],
     )
     name = models.CharField(_("Name"), max_length=100, blank=True)
     description = models.TextField(_("Description"), blank=True)
     is_required = models.BooleanField(
         _("Is required"),
         help_text=_("Are cookies in this group required."),
         default=False,
@@ -44,81 +71,105 @@
         _("Is deletable?"),
         help_text=_("Can cookies in this group be deleted."),
         default=True,
     )
     ordering = models.IntegerField(_("Ordering"), default=0)
     created = models.DateTimeField(_("Created"), auto_now_add=True, blank=True)
 
+    objects = CookieGroupManager()
+
     class Meta:
         verbose_name = _("Cookie Group")
         verbose_name_plural = _("Cookie Groups")
         ordering = ["ordering"]
 
     def __str__(self):
         return self.name
 
+    @clear_cache_after
+    def save(self, *args, **kwargs):
+        super().save(*args, **kwargs)
+
+    @clear_cache_after
+    def delete(self, *args, **kwargs):
+        return super().delete(*args, **kwargs)
+
+    def natural_key(self):
+        return (self.varname,)
+
     def get_version(self) -> str:
         try:
             return str(self.cookie_set.all()[0].get_version())
         except IndexError:
             return ""
 
-    def delete(self, *args, **kwargs):
-        super(CookieGroup, self).delete(*args, **kwargs)
-        delete_cache()
-
-    def save(self, *args, **kwargs):
-        super(CookieGroup, self).save(*args, **kwargs)
-        delete_cache()
-
     def for_json(self) -> CookieGroupDict:
         return {
             "varname": self.varname,
             "name": self.name,
             "description": self.description,
             "is_required": self.is_required,
             # "version": self.get_version(),
         }
 
 
+class CookieManager(models.Manager.from_queryset(BaseQueryset)):
+    def get_by_natural_key(self, name, domain, cookiegroup):
+        group = CookieGroup.objects.get_by_natural_key(cookiegroup)
+        return self.get(cookiegroup=group, name=name, domain=domain)
+
+
 class Cookie(models.Model):
     cookiegroup = models.ForeignKey(
         CookieGroup,
         verbose_name=CookieGroup._meta.verbose_name,
         on_delete=models.CASCADE,
     )
     name = models.CharField(_("Name"), max_length=250)
     description = models.TextField(_("Description"), blank=True)
     path = models.TextField(_("Path"), blank=True, default="/")
     domain = models.CharField(_("Domain"), max_length=250, blank=True)
     created = models.DateTimeField(_("Created"), auto_now_add=True, blank=True)
 
+    objects = CookieManager()
+
     class Meta:
         verbose_name = _("Cookie")
         verbose_name_plural = _("Cookies")
+        constraints = [
+            models.UniqueConstraint(
+                fields=("cookiegroup", "name", "domain"),
+                name="natural_key",
+            ),
+        ]
         ordering = ["-created"]
 
     def __str__(self):
         return "%s %s%s" % (self.name, self.domain, self.path)
 
+    @clear_cache_after
+    def save(self, *args, **kwargs):
+        super().save(*args, **kwargs)
+
+    @clear_cache_after
+    def delete(self, *args, **kwargs):
+        return super().delete(*args, **kwargs)
+
+    def natural_key(self):
+        return (self.name, self.domain) + self.cookiegroup.natural_key()
+
+    natural_key.dependencies = ["cookie_consent.cookiegroup"]
+
     @property
     def varname(self):
         return "%s=%s:%s" % (self.cookiegroup.varname, self.name, self.domain)
 
     def get_version(self):
         return self.created.isoformat()
 
-    def delete(self, *args, **kwargs):
-        super(Cookie, self).delete(*args, **kwargs)
-        delete_cache()
-
-    def save(self, *args, **kwargs):
-        super(Cookie, self).save(*args, **kwargs)
-        delete_cache()
-
 
 ACTION_ACCEPTED = 1
 ACTION_DECLINED = -1
 ACTION_CHOICES = (
     (ACTION_DECLINED, _("Declined")),
     (ACTION_ACCEPTED, _("Accepted")),
 )
```

### Comparing `django-cookie-consent-0.5.0b0/cookie_consent/static/cookie_consent/cookiebar.js` & `django_cookie_consent-0.6.0/cookie_consent/static/cookie_consent/cookiebar.js`

 * *Files identical despite different names*

### Comparing `django-cookie-consent-0.5.0b0/cookie_consent/templates/cookie_consent/_cookie_group.html` & `django_cookie_consent-0.6.0/cookie_consent/templates/cookie_consent/_cookie_group.html`

 * *Files identical despite different names*

### Comparing `django-cookie-consent-0.5.0b0/cookie_consent/templatetags/cookie_consent_tags.py` & `django_cookie_consent-0.6.0/cookie_consent/templatetags/cookie_consent_tags.py`

 * *Files identical despite different names*

### Comparing `django-cookie-consent-0.5.0b0/cookie_consent/urls.py` & `django_cookie_consent-0.6.0/cookie_consent/urls.py`

 * *Files identical despite different names*

### Comparing `django-cookie-consent-0.5.0b0/cookie_consent/util.py` & `django_cookie_consent-0.6.0/cookie_consent/util.py`

 * *Files identical despite different names*

### Comparing `django-cookie-consent-0.5.0b0/cookie_consent/views.py` & `django_cookie_consent-0.6.0/cookie_consent/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # -*- coding: utf-8 -*-
+from django.contrib.auth.views import RedirectURLMixin
 from django.core.exceptions import SuspiciousOperation
 from django.http import HttpRequest, HttpResponse, HttpResponseRedirect, JsonResponse
 from django.middleware.csrf import get_token as get_csrf_token
 from django.urls import reverse
+from django.utils.http import url_has_allowed_host_and_scheme
 from django.views.generic import ListView, View
 
-from .compat import RedirectURLMixin, url_has_allowed_host_and_scheme
 from .models import CookieGroup
 from .util import (
     accept_cookies,
     decline_cookies,
     get_accepted_cookie_groups,
     get_declined_cookie_groups,
     get_not_accepted_or_declined_cookie_groups,
```

### Comparing `django-cookie-consent-0.5.0b0/django_cookie_consent.egg-info/PKG-INFO` & `django_cookie_consent-0.6.0/django_cookie_consent.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,59 +1,78 @@
 Metadata-Version: 2.1
 Name: django-cookie-consent
-Version: 0.5.0b0
+Version: 0.6.0
 Summary: Django cookie consent application
-Home-page: https://github.com/jazzband/django-cookie-consent
-Author: Informatika Mihelac
-Author-email: bmihelac@mihelac.org
-License: BSD
+Author-email: Informatika Mihelac <bmihelac@mihelac.org>
+License: Copyright (c) Bojan Mihelac and individual contributors.
+        All rights reserved.
+        
+        Redistribution and use in source and binary forms, with or without modification,
+        are permitted provided that the following conditions are met:
+        
+            1. Redistributions of source code must retain the above copyright notice, 
+               this list of conditions and the following disclaimer.
+            
+            2. Redistributions in binary form must reproduce the above copyright 
+               notice, this list of conditions and the following disclaimer in the
+               documentation and/or other materials provided with the distribution.
+        
+        THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND
+        ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
+        WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+        DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT OWNER OR CONTRIBUTORS BE LIABLE FOR
+        ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
+        (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
+        LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON
+        ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
+        (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
+        SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+        
 Project-URL: Documentation, https://django-cookie-consent.readthedocs.io/en/latest/
 Project-URL: Changelog, https://github.com/jazzband/django-cookie-consent/blob/master/docs/changelog.rst
 Project-URL: Bug Tracker, https://github.com/jazzband/django-cookie-consent/issues
 Project-URL: Source Code, https://github.com/jazzband/django-cookie-consent
 Keywords: cookies,cookie-consent,cookie bar
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.1
 Classifier: Framework :: Django :: 4.2
+Classifier: Framework :: Django :: 5.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS
-Requires-Dist: django>=3.2
+Requires-Dist: django>=4.2
 Requires-Dist: django-appconf
 Provides-Extra: tests
 Requires-Dist: pytest; extra == "tests"
 Requires-Dist: pytest-django; extra == "tests"
 Requires-Dist: pytest-playwright; extra == "tests"
 Requires-Dist: tox; extra == "tests"
 Requires-Dist: isort; extra == "tests"
 Requires-Dist: black; extra == "tests"
 Requires-Dist: flake8; extra == "tests"
-Provides-Extra: pep8
-Requires-Dist: flake8; extra == "pep8"
 Provides-Extra: coverage
 Requires-Dist: pytest-cov; extra == "coverage"
 Provides-Extra: docs
 Requires-Dist: sphinx; extra == "docs"
 Requires-Dist: sphinx-rtd-theme; extra == "docs"
 Provides-Extra: release
 Requires-Dist: tbump; extra == "release"
-Requires-Dist: twine; extra == "release"
 
 Django cookie consent
 =====================
 
 Manage cookie information and let visitors give or reject consent for them.
 
 [![Jazzband][badge:jazzband]][jazzband]
```

### Comparing `django-cookie-consent-0.5.0b0/django_cookie_consent.egg-info/SOURCES.txt` & `django_cookie_consent-0.6.0/django_cookie_consent.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,42 +1,45 @@
 AUTHORS
 LICENSE
 MANIFEST.in
 README.md
+pyproject.toml
 setup.cfg
-setup.py
 cookie_consent/__init__.py
 cookie_consent/admin.py
 cookie_consent/apps.py
 cookie_consent/cache.py
-cookie_consent/compat.py
 cookie_consent/conf.py
 cookie_consent/middleware.py
 cookie_consent/models.py
 cookie_consent/urls.py
 cookie_consent/util.py
 cookie_consent/views.py
 cookie_consent/fixtures/common_cookies.json
 cookie_consent/migrations/0001_initial.py
 cookie_consent/migrations/0002_auto__add_logitem.py
+cookie_consent/migrations/0003_alter_cookiegroup_varname.py
+cookie_consent/migrations/0004_cookie_natural_key.py
 cookie_consent/migrations/__init__.py
 cookie_consent/static/cookie_consent/cookiebar.js
 cookie_consent/static/cookie_consent/cookiebar.module.js
+cookie_consent/static/cookie_consent/cookiebar.module.js.map
 cookie_consent/templates/cookie_consent/_cookie_group.html
 cookie_consent/templates/cookie_consent/base.html
 cookie_consent/templates/cookie_consent/cookiegroup_list.html
 cookie_consent/templatetags/__init__.py
 cookie_consent/templatetags/cookie_consent_tags.py
 django_cookie_consent.egg-info/PKG-INFO
 django_cookie_consent.egg-info/SOURCES.txt
 django_cookie_consent.egg-info/dependency_links.txt
-django_cookie_consent.egg-info/not-zip-safe
 django_cookie_consent.egg-info/requires.txt
 django_cookie_consent.egg-info/top_level.txt
 tests/test_cache.py
+tests/test_cookie_group_model.py
+tests/test_cookie_model.py
 tests/test_javascript_cookiebar.py
 tests/test_legacy_javascript_cookiebar.py
 tests/test_middleware.py
 tests/test_models.py
 tests/test_settings.py
 tests/test_templatetags.py
 tests/test_util.py
```

### Comparing `django-cookie-consent-0.5.0b0/tests/test_cache.py` & `django_cookie_consent-0.6.0/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `django-cookie-consent-0.5.0b0/tests/test_javascript_cookiebar.py` & `django_cookie_consent-0.6.0/tests/test_javascript_cookiebar.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Test the behaviour of the dynamic (JS based) cookiebar module.
 
 See docs: https://playwright.dev/python/docs/test-runners for CLI options.
 """
+
 from django.urls import reverse
 
 import pytest
 from playwright.sync_api import Page, expect
 
 pytestmark = [pytest.mark.django_db, pytest.mark.e2e]
 
@@ -17,14 +18,16 @@
 """
 
 
 @pytest.fixture(scope="function", autouse=True)
 def before_each_after_each(live_server, page: Page, load_testapp_fixture):
     test_page_url = f"{live_server.url}{reverse('test_page')}"
     page.goto(test_page_url)
+    marker = page.get_by_text("page-done-loading")
+    expect(marker).to_be_visible()
     yield
 
 
 def test_cookiebar_shows_initially(page: Page):
     cookiebar = page.get_by_text(COOKIE_BAR_CONTENT)
     expect(cookiebar).to_be_visible()
 
@@ -64,13 +67,18 @@
     page.reload()
     expect(page.get_by_text(COOKIE_BAR_CONTENT)).not_to_be_visible()
 
 
 def test_on_accept_handler_runs_on_load(page: Page, live_server):
     accept_button = page.get_by_role("button", name="Accept")
     accept_button.click()
+    # wait for fetch calls to complete & avoid test race conditions...
+    share_button = page.get_by_role("button", name="SHARE")
+    expect(share_button).to_be_visible()
 
     test_page_url = f"{live_server.url}{reverse('test_page')}"
     page.goto(test_page_url)
+    marker = page.get_by_text("page-done-loading")
+    expect(marker).to_be_visible()
 
     share_button = page.get_by_role("button", name="SHARE")
     expect(share_button).to_be_visible()
```

### Comparing `django-cookie-consent-0.5.0b0/tests/test_legacy_javascript_cookiebar.py` & `django_cookie_consent-0.6.0/tests/test_legacy_javascript_cookiebar.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 These tests mostly exist to assert code coverage while giving library users time
 to transition to the new implementation.
 
 TODO: remove in django-cookie-consent 1.0
 """
+
 from django.urls import reverse
 
 import pytest
 from playwright.sync_api import Page, expect
 
 pytestmark = [pytest.mark.django_db, pytest.mark.e2e]
```

### Comparing `django-cookie-consent-0.5.0b0/tests/test_middleware.py` & `django_cookie_consent-0.6.0/tests/test_middleware.py`

 * *Files identical despite different names*

### Comparing `django-cookie-consent-0.5.0b0/tests/test_settings.py` & `django_cookie_consent-0.6.0/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `django-cookie-consent-0.5.0b0/tests/test_templatetags.py` & `django_cookie_consent-0.6.0/tests/test_templatetags.py`

 * *Files identical despite different names*

### Comparing `django-cookie-consent-0.5.0b0/tests/test_util.py` & `django_cookie_consent-0.6.0/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `django-cookie-consent-0.5.0b0/tests/test_views.py` & `django_cookie_consent-0.6.0/tests/test_views.py`

 * *Files identical despite different names*

