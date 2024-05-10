# Comparing `tmp/django_viewrouter-0.1.0.tar.gz` & `tmp/django_viewrouter-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_viewrouter-0.1.0.tar", max compression
+gzip compressed data, was "django_viewrouter-0.1.1.tar", max compression
```

## Comparing `django_viewrouter-0.1.0.tar` & `django_viewrouter-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     3496 2024-05-03 08:51:49.119346 django_viewrouter-0.1.0/README.md
--rw-r--r--   0        0        0      343 2024-05-03 09:02:47.610334 django_viewrouter-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-03 08:51:49.119346 django_viewrouter-0.1.0/viewrouter/__init__.py
--rw-r--r--   0        0        0     4119 2024-05-03 08:51:49.119346 django_viewrouter-0.1.0/viewrouter/routers.py
--rw-r--r--   0        0        0       82 2024-05-03 08:51:49.119346 django_viewrouter-0.1.0/viewrouter/templates/viewrouter/actionview_index.html
--rw-r--r--   0        0        0     5025 2024-05-03 08:51:49.119346 django_viewrouter-0.1.0/viewrouter/tests.py
--rw-r--r--   0        0        0     3003 2024-05-03 08:51:49.119346 django_viewrouter-0.1.0/viewrouter/views.py
--rw-r--r--   0        0        0     3938 1970-01-01 00:00:00.000000 django_viewrouter-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     3496 2024-05-03 08:51:49.119346 django_viewrouter-0.1.1/README.md
+-rw-r--r--   0        0        0      343 2024-05-10 10:21:32.616809 django_viewrouter-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-03 08:51:49.119346 django_viewrouter-0.1.1/viewrouter/__init__.py
+-rw-r--r--   0        0        0     4119 2024-05-03 08:51:49.119346 django_viewrouter-0.1.1/viewrouter/routers.py
+-rw-r--r--   0        0        0       82 2024-05-03 08:51:49.119346 django_viewrouter-0.1.1/viewrouter/templates/viewrouter/actionview_index.html
+-rw-r--r--   0        0        0     5025 2024-05-03 08:51:49.119346 django_viewrouter-0.1.1/viewrouter/tests.py
+-rw-r--r--   0        0        0     3003 2024-05-03 08:51:49.119346 django_viewrouter-0.1.1/viewrouter/views.py
+-rw-r--r--   0        0        0     3938 1970-01-01 00:00:00.000000 django_viewrouter-0.1.1/PKG-INFO
```

### Comparing `django_viewrouter-0.1.0/README.md` & `django_viewrouter-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `django_viewrouter-0.1.0/viewrouter/routers.py` & `django_viewrouter-0.1.1/viewrouter/routers.py`

 * *Files identical despite different names*

### Comparing `django_viewrouter-0.1.0/viewrouter/tests.py` & `django_viewrouter-0.1.1/viewrouter/tests.py`

 * *Files identical despite different names*

### Comparing `django_viewrouter-0.1.0/viewrouter/views.py` & `django_viewrouter-0.1.1/viewrouter/views.py`

 * *Files identical despite different names*

### Comparing `django_viewrouter-0.1.0/PKG-INFO` & `django_viewrouter-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-viewrouter
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 License: MIT
 Author: Kamal Mustafa
 Author-email: k4ml@github.io
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

