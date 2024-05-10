# Comparing `tmp/django_harlequin-1.1.1.tar.gz` & `tmp/django_harlequin-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_harlequin-1.1.1.tar", last modified: Wed May  8 09:51:40 2024, max compression
+gzip compressed data, was "django_harlequin-1.1.2.tar", last modified: Fri May 10 09:51:44 2024, max compression
```

## Comparing `django_harlequin-1.1.1.tar` & `django_harlequin-1.1.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2024-05-08 09:51:40.807324 django_harlequin-1.1.1/
--rw-r--r--   0 adamjohnson   (501) staff       (20)      359 2024-05-08 09:51:37.000000 django_harlequin-1.1.1/CHANGELOG.rst
--rw-r--r--   0 adamjohnson   (501) staff       (20)     1069 2024-05-05 06:27:49.000000 django_harlequin-1.1.1/LICENSE
--rw-r--r--   0 adamjohnson   (501) staff       (20)      115 2024-05-05 06:26:38.000000 django_harlequin-1.1.1/MANIFEST.in
--rw-r--r--   0 adamjohnson   (501) staff       (20)     4333 2024-05-08 09:51:40.807122 django_harlequin-1.1.1/PKG-INFO
--rw-r--r--   0 adamjohnson   (501) staff       (20)     2913 2024-05-08 09:47:58.000000 django_harlequin-1.1.1/README.rst
--rw-r--r--   0 adamjohnson   (501) staff       (20)     2138 2024-05-08 09:51:37.000000 django_harlequin-1.1.1/pyproject.toml
--rw-r--r--   0 adamjohnson   (501) staff       (20)       38 2024-05-08 09:51:40.807374 django_harlequin-1.1.1/setup.cfg
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2024-05-08 09:51:40.804038 django_harlequin-1.1.1/src/
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2024-05-08 09:51:40.805457 django_harlequin-1.1.1/src/django_harlequin/
--rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2024-05-05 06:26:40.000000 django_harlequin-1.1.1/src/django_harlequin/__init__.py
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2024-05-08 09:51:40.806324 django_harlequin-1.1.1/src/django_harlequin/management/
--rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2024-05-05 06:26:40.000000 django_harlequin-1.1.1/src/django_harlequin/management/__init__.py
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2024-05-08 09:51:40.806553 django_harlequin-1.1.1/src/django_harlequin/management/commands/
--rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2024-05-05 06:26:40.000000 django_harlequin-1.1.1/src/django_harlequin/management/commands/__init__.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)     5844 2024-05-06 21:17:40.000000 django_harlequin-1.1.1/src/django_harlequin/management/commands/harlequin.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2024-05-05 06:26:40.000000 django_harlequin-1.1.1/src/django_harlequin/py.typed
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2024-05-08 09:51:40.806886 django_harlequin-1.1.1/src/django_harlequin.egg-info/
--rw-r--r--   0 adamjohnson   (501) staff       (20)     4333 2024-05-08 09:51:40.000000 django_harlequin-1.1.1/src/django_harlequin.egg-info/PKG-INFO
--rw-r--r--   0 adamjohnson   (501) staff       (20)      492 2024-05-08 09:51:40.000000 django_harlequin-1.1.1/src/django_harlequin.egg-info/SOURCES.txt
--rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2024-05-08 09:51:40.000000 django_harlequin-1.1.1/src/django_harlequin.egg-info/dependency_links.txt
--rw-r--r--   0 adamjohnson   (501) staff       (20)       22 2024-05-08 09:51:40.000000 django_harlequin-1.1.1/src/django_harlequin.egg-info/requires.txt
--rw-r--r--   0 adamjohnson   (501) staff       (20)       17 2024-05-08 09:51:40.000000 django_harlequin-1.1.1/src/django_harlequin.egg-info/top_level.txt
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2024-05-10 09:51:44.275514 django_harlequin-1.1.2/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      522 2024-05-10 09:51:41.000000 django_harlequin-1.1.2/CHANGELOG.rst
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1069 2024-05-05 06:27:49.000000 django_harlequin-1.1.2/LICENSE
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      115 2024-05-05 06:26:38.000000 django_harlequin-1.1.2/MANIFEST.in
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     4636 2024-05-10 09:51:44.275262 django_harlequin-1.1.2/PKG-INFO
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     3241 2024-05-10 09:44:14.000000 django_harlequin-1.1.2/README.rst
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     2123 2024-05-10 09:51:41.000000 django_harlequin-1.1.2/pyproject.toml
+-rw-r--r--   0 adamjohnson   (501) staff       (20)       38 2024-05-10 09:51:44.275604 django_harlequin-1.1.2/setup.cfg
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2024-05-10 09:51:44.271860 django_harlequin-1.1.2/src/
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2024-05-10 09:51:44.273429 django_harlequin-1.1.2/src/django_harlequin/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2024-05-05 06:26:40.000000 django_harlequin-1.1.2/src/django_harlequin/__init__.py
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2024-05-10 09:51:44.274219 django_harlequin-1.1.2/src/django_harlequin/management/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2024-05-05 06:26:40.000000 django_harlequin-1.1.2/src/django_harlequin/management/__init__.py
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2024-05-10 09:51:44.274465 django_harlequin-1.1.2/src/django_harlequin/management/commands/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2024-05-05 06:26:40.000000 django_harlequin-1.1.2/src/django_harlequin/management/commands/__init__.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     5844 2024-05-06 21:17:40.000000 django_harlequin-1.1.2/src/django_harlequin/management/commands/harlequin.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2024-05-05 06:26:40.000000 django_harlequin-1.1.2/src/django_harlequin/py.typed
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2024-05-10 09:51:44.274943 django_harlequin-1.1.2/src/django_harlequin.egg-info/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     4636 2024-05-10 09:51:44.000000 django_harlequin-1.1.2/src/django_harlequin.egg-info/PKG-INFO
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      492 2024-05-10 09:51:44.000000 django_harlequin-1.1.2/src/django_harlequin.egg-info/SOURCES.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2024-05-10 09:51:44.000000 django_harlequin-1.1.2/src/django_harlequin.egg-info/dependency_links.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)       12 2024-05-10 09:51:44.000000 django_harlequin-1.1.2/src/django_harlequin.egg-info/requires.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)       17 2024-05-10 09:51:44.000000 django_harlequin-1.1.2/src/django_harlequin.egg-info/top_level.txt
```

### Comparing `django_harlequin-1.1.1/LICENSE` & `django_harlequin-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django_harlequin-1.1.1/PKG-INFO` & `django_harlequin-1.1.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-harlequin
-Version: 1.1.1
+Version: 1.1.2
 Summary: Launch Harlequin, the SQL IDE for your Terminal, with your Django database configuration.
 Author-email: Adam Johnson <me@adamj.eu>
 License: MIT
 Project-URL: Changelog, https://github.com/adamchainz/django-harlequin/blob/main/CHANGELOG.rst
 Project-URL: Funding, https://adamj.eu/books/
 Project-URL: Repository, https://github.com/adamchainz/django-harlequin
 Keywords: Django
@@ -26,15 +26,14 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: Django>=3.2
-Requires-Dist: harlequin
 
 ================
 django-harlequin
 ================
 
 .. image:: https://img.shields.io/github/actions/workflow/status/adamchainz/django-harlequin/main.yml.svg?branch=main&style=for-the-badge
    :target: https://github.com/adamchainz/django-harlequin/actions?workflow=CI
@@ -74,20 +73,23 @@
 
 **First,** install with pip:
 
 .. code-block:: bash
 
     python -m pip install django-harlequin
 
-**Second,** install the appropriate Harlequin `adapter package <https://harlequin.sh/docs/adapters>`__ for your database backend, if necessary (SQLite is built-in).
-For example, for the `PostgreSQL adapter <https://harlequin.sh/docs/postgres/index>`__:
+**Second,** install Harlequin with appropriate Harlequin `adapter packages <https://harlequin.sh/docs/adapters>`__ for the database backends you use.
+For example, to install Harlequin with the `PostgreSQL adapter <https://harlequin.sh/docs/postgres/index>`__:
 
 .. code-block:: bash
 
-    python -m pip install harlequin-postgres
+    python -m pip 'harlequin[postgres]'
+
+Harlequin does not need to be installed in the same virtual environment as Django, as django-harlequin does not import it.
+You only need the ``harlequin`` command on your path, so you can install Harlequin globally, or in an isolated virtual environment with a tool like `pipx <https://pipx.pypa.io/latest/installation/>`__.
 
 **Third,** add the app to your ``INSTALLED_APPS`` setting:
 
 .. code-block:: python
 
     INSTALLED_APPS = [
         ...,
```

### Comparing `django_harlequin-1.1.1/README.rst` & `django_harlequin-1.1.2/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -40,20 +40,23 @@
 
 **First,** install with pip:
 
 .. code-block:: bash
 
     python -m pip install django-harlequin
 
-**Second,** install the appropriate Harlequin `adapter package <https://harlequin.sh/docs/adapters>`__ for your database backend, if necessary (SQLite is built-in).
-For example, for the `PostgreSQL adapter <https://harlequin.sh/docs/postgres/index>`__:
+**Second,** install Harlequin with appropriate Harlequin `adapter packages <https://harlequin.sh/docs/adapters>`__ for the database backends you use.
+For example, to install Harlequin with the `PostgreSQL adapter <https://harlequin.sh/docs/postgres/index>`__:
 
 .. code-block:: bash
 
-    python -m pip install harlequin-postgres
+    python -m pip 'harlequin[postgres]'
+
+Harlequin does not need to be installed in the same virtual environment as Django, as django-harlequin does not import it.
+You only need the ``harlequin`` command on your path, so you can install Harlequin globally, or in an isolated virtual environment with a tool like `pipx <https://pipx.pypa.io/latest/installation/>`__.
 
 **Third,** add the app to your ``INSTALLED_APPS`` setting:
 
 .. code-block:: python
 
     INSTALLED_APPS = [
         ...,
```

### Comparing `django_harlequin-1.1.1/pyproject.toml` & `django_harlequin-1.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 build-backend = "setuptools.build_meta"
 requires = [
   "setuptools",
 ]
 
 [project]
 name = "django-harlequin"
-version = "1.1.1"
+version = "1.1.2"
 description = "Launch Harlequin, the SQL IDE for your Terminal, with your Django database configuration."
 readme = {file = "README.rst", content-type = "text/x-rst"}
 keywords = [
   "Django",
 ]
 license = {text = "MIT"}
 authors = [{name = "Adam Johnson", email = "me@adamj.eu"}]
@@ -33,15 +33,14 @@
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
   "Programming Language :: Python :: Implementation :: CPython",
   "Typing :: Typed",
 ]
 dependencies = [
   "Django>=3.2",
-  "harlequin",
 ]
 [project.urls]
 Changelog = "https://github.com/adamchainz/django-harlequin/blob/main/CHANGELOG.rst"
 Funding = "https://adamj.eu/books/"
 Repository = "https://github.com/adamchainz/django-harlequin"
 
 [tool.isort]
```

### Comparing `django_harlequin-1.1.1/src/django_harlequin/management/commands/harlequin.py` & `django_harlequin-1.1.2/src/django_harlequin/management/commands/harlequin.py`

 * *Files identical despite different names*

### Comparing `django_harlequin-1.1.1/src/django_harlequin.egg-info/PKG-INFO` & `django_harlequin-1.1.2/src/django_harlequin.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-harlequin
-Version: 1.1.1
+Version: 1.1.2
 Summary: Launch Harlequin, the SQL IDE for your Terminal, with your Django database configuration.
 Author-email: Adam Johnson <me@adamj.eu>
 License: MIT
 Project-URL: Changelog, https://github.com/adamchainz/django-harlequin/blob/main/CHANGELOG.rst
 Project-URL: Funding, https://adamj.eu/books/
 Project-URL: Repository, https://github.com/adamchainz/django-harlequin
 Keywords: Django
@@ -26,15 +26,14 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: Django>=3.2
-Requires-Dist: harlequin
 
 ================
 django-harlequin
 ================
 
 .. image:: https://img.shields.io/github/actions/workflow/status/adamchainz/django-harlequin/main.yml.svg?branch=main&style=for-the-badge
    :target: https://github.com/adamchainz/django-harlequin/actions?workflow=CI
@@ -74,20 +73,23 @@
 
 **First,** install with pip:
 
 .. code-block:: bash
 
     python -m pip install django-harlequin
 
-**Second,** install the appropriate Harlequin `adapter package <https://harlequin.sh/docs/adapters>`__ for your database backend, if necessary (SQLite is built-in).
-For example, for the `PostgreSQL adapter <https://harlequin.sh/docs/postgres/index>`__:
+**Second,** install Harlequin with appropriate Harlequin `adapter packages <https://harlequin.sh/docs/adapters>`__ for the database backends you use.
+For example, to install Harlequin with the `PostgreSQL adapter <https://harlequin.sh/docs/postgres/index>`__:
 
 .. code-block:: bash
 
-    python -m pip install harlequin-postgres
+    python -m pip 'harlequin[postgres]'
+
+Harlequin does not need to be installed in the same virtual environment as Django, as django-harlequin does not import it.
+You only need the ``harlequin`` command on your path, so you can install Harlequin globally, or in an isolated virtual environment with a tool like `pipx <https://pipx.pypa.io/latest/installation/>`__.
 
 **Third,** add the app to your ``INSTALLED_APPS`` setting:
 
 .. code-block:: python
 
     INSTALLED_APPS = [
         ...,
```

