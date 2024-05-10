# Comparing `tmp/django_usefathom-2.0.1.tar.gz` & `tmp/django_usefathom-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_usefathom-2.0.1.tar", max compression
+gzip compressed data, was "django_usefathom-2.0.2.tar", max compression
```

## Comparing `django_usefathom-2.0.1.tar` & `django_usefathom-2.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1077 2022-12-10 08:20:04.474860 django_usefathom-2.0.1/LICENSE
--rw-r--r--   0        0        0     1816 2024-05-07 04:18:01.714122 django_usefathom-2.0.1/README.md
--rw-r--r--   0        0        0      518 2024-05-09 05:20:12.782440 django_usefathom-2.0.1/pyproject.toml
--rw-r--r--   0        0        0       31 2024-05-09 05:17:48.170058 django_usefathom-2.0.1/usefathom/__init__.py
--rw-r--r--   0        0        0      942 2024-05-07 03:58:16.406711 django_usefathom-2.0.1/usefathom/api.py
--rw-r--r--   0        0        0      147 2022-12-10 08:20:04.475887 django_usefathom-2.0.1/usefathom/apps.py
--rw-r--r--   0        0        0      194 2024-05-07 04:18:26.919739 django_usefathom-2.0.1/usefathom/context_processors.py
--rw-r--r--   0        0        0      104 2024-05-07 04:11:00.402889 django_usefathom-2.0.1/usefathom/templates/usefathom/click.html
--rw-r--r--   0        0        0      105 2024-05-07 04:11:15.241497 django_usefathom-2.0.1/usefathom/templates/usefathom/submit.html
--rw-r--r--   0        0        0      482 2024-05-07 04:18:39.450681 django_usefathom-2.0.1/usefathom/templates/usefathom/usefathom.html
--rw-r--r--   0        0        0      543 2024-05-07 04:10:45.604051 django_usefathom-2.0.1/usefathom/templatetags/fathom.py
--rw-r--r--   0        0        0       60 2022-12-10 08:20:04.476703 django_usefathom-2.0.1/usefathom/tests.py
--rw-r--r--   0        0        0     2520 1970-01-01 00:00:00.000000 django_usefathom-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1077 2022-12-10 08:20:04.474860 django_usefathom-2.0.2/LICENSE
+-rw-r--r--   0        0        0     1816 2024-05-07 04:18:01.714122 django_usefathom-2.0.2/README.md
+-rw-r--r--   0        0        0      518 2024-05-09 06:00:34.297491 django_usefathom-2.0.2/pyproject.toml
+-rw-r--r--   0        0        0       31 2024-05-09 05:17:48.170058 django_usefathom-2.0.2/usefathom/__init__.py
+-rw-r--r--   0        0        0      942 2024-05-07 03:58:16.406711 django_usefathom-2.0.2/usefathom/api.py
+-rw-r--r--   0        0        0      147 2022-12-10 08:20:04.475887 django_usefathom-2.0.2/usefathom/apps.py
+-rw-r--r--   0        0        0      194 2024-05-07 04:18:26.919739 django_usefathom-2.0.2/usefathom/context_processors.py
+-rw-r--r--   0        0        0      104 2024-05-07 04:11:00.402889 django_usefathom-2.0.2/usefathom/templates/usefathom/click.html
+-rw-r--r--   0        0        0      105 2024-05-07 04:11:15.241497 django_usefathom-2.0.2/usefathom/templates/usefathom/submit.html
+-rw-r--r--   0        0        0      483 2024-05-09 05:59:42.935743 django_usefathom-2.0.2/usefathom/templates/usefathom/usefathom.html
+-rw-r--r--   0        0        0      543 2024-05-07 04:10:45.604051 django_usefathom-2.0.2/usefathom/templatetags/fathom.py
+-rw-r--r--   0        0        0       60 2022-12-10 08:20:04.476703 django_usefathom-2.0.2/usefathom/tests.py
+-rw-r--r--   0        0        0     2520 1970-01-01 00:00:00.000000 django_usefathom-2.0.2/PKG-INFO
```

### Comparing `django_usefathom-2.0.1/LICENSE` & `django_usefathom-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django_usefathom-2.0.1/README.md` & `django_usefathom-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `django_usefathom-2.0.1/pyproject.toml` & `django_usefathom-2.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-usefathom"
-version = "2.0.1"
+version = "2.0.2"
 description = "A Django app to integrate Fathom Analytics into your project"
 authors = ["Paul Chubatyy <xobb@citylance.biz>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/paulchubatyy/django-usefathom"
 packages = [
     { include = "usefathom" },
```

### Comparing `django_usefathom-2.0.1/usefathom/api.py` & `django_usefathom-2.0.2/usefathom/api.py`

 * *Files identical despite different names*

### Comparing `django_usefathom-2.0.1/usefathom/templatetags/fathom.py` & `django_usefathom-2.0.2/usefathom/templatetags/fathom.py`

 * *Files identical despite different names*

### Comparing `django_usefathom-2.0.1/PKG-INFO` & `django_usefathom-2.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-usefathom
-Version: 2.0.1
+Version: 2.0.2
 Summary: A Django app to integrate Fathom Analytics into your project
 Home-page: https://github.com/paulchubatyy/django-usefathom
 License: MIT
 Author: Paul Chubatyy
 Author-email: xobb@citylance.biz
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

